# Comparing `tmp/catalystwan-0.33.7.dev1.tar.gz` & `tmp/catalystwan-0.33.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalystwan-0.33.7.dev1.tar", max compression
+gzip compressed data, was "catalystwan-0.33.7.dev2.tar", max compression
```

## Comparing `catalystwan-0.33.7.dev1.tar` & `catalystwan-0.33.7.dev2.tar`

### file list

```diff
@@ -1,548 +1,569 @@
--rw-r--r--   0        0        0    11375 2024-05-23 10:34:23.261722 catalystwan-0.33.7.dev1/LICENSE
--rw-r--r--   0        0        0    13533 2024-05-23 10:34:23.261722 catalystwan-0.33.7.dev1/README.md
--rw-r--r--   0        0        0     2558 2024-05-23 10:34:23.261722 catalystwan-0.33.7.dev1/catalystwan/__init__.py
--rw-r--r--   0        0        0     1532 2024-05-23 10:34:23.261722 catalystwan-0.33.7.dev1/catalystwan/abstractions.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/__init__.py
--rw-r--r--   0        0        0     6689 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/admin_tech_api.py
--rw-r--r--   0        0        0    14935 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/administration.py
--rw-r--r--   0        0        0     6314 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/alarms_api.py
--rw-r--r--   0        0        0     3293 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/api_container.py
--rw-r--r--   0        0        0    11636 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/basic_api.py
--rw-r--r--   0        0        0      386 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/__init__.py
--rw-r--r--   0        0        0     2017 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/builder_factory.py
--rw-r--r--   0        0        0     2679 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/cli.py
--rw-r--r--   0        0        0     2696 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/other.py
--rw-r--r--   0        0        0     3146 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/report.py
--rw-r--r--   0        0        0     5727 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/service.py
--rw-r--r--   0        0        0     2768 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/system.py
--rw-r--r--   0        0        0     4328 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/transport.py
--rw-r--r--   0        0        0     2053 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/config_device_inventory_api.py
--rw-r--r--   0        0        0     4760 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/config_group_api.py
--rw-r--r--   0        0        0     6672 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/configuration_groups/parcel.py
--rw-r--r--   0        0        0     7315 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/dashboard_api.py
--rw-r--r--   0        0        0     7360 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/device_action_api.py
--rw-r--r--   0        0        0    53328 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/feature_profile_api.py
--rw-r--r--   0        0        0     1919 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/logs_api.py
--rw-r--r--   0        0        0     2449 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/monitoring_status_api.py
--rw-r--r--   0        0        0     6036 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/mtt_aaa_api.py
--rw-r--r--   0        0        0     4394 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/omp_api.py
--rw-r--r--   0        0        0     5691 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/packet_capture_api.py
--rw-r--r--   0        0        0     1654 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/parcel_api.py
--rw-r--r--   0        0        0     5600 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/partition_manager_api.py
--rw-r--r--   0        0        0    36861 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/policy_api.py
--rw-r--r--   0        0        0     2284 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/resource_pool_api.py
--rw-r--r--   0        0        0    11320 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/software_action_api.py
--rw-r--r--   0        0        0     5473 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/speedtest_api.py
--rw-r--r--   0        0        0     7149 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/task_status_api.py
--rw-r--r--   0        0        0    30133 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/template_api.py
--rw-r--r--   0        0        0     3540 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/README.md
--rw-r--r--   0        0        0      251 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/bool_str.py
--rw-r--r--   0        0        0     7481 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/cli_template.py
--rw-r--r--   0        0        0     3425 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/device_template/device_template.py
--rw-r--r--   0        0        0      571 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/device_template/device_template_payload.json.j2
--rw-r--r--   0        0        0      137 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/device_variable.py
--rw-r--r--   0        0        0     5029 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template.py
--rw-r--r--   0        0        0     6576 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template_field.py
--rw-r--r--   0        0        0      661 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template_payload.py
--rw-r--r--   0        0        0     3244 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_aaa_model.py
--rw-r--r--   0        0        0      667 2024-05-23 10:34:23.265722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_banner_model.py
--rw-r--r--   0        0        0     2180 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_bfd_model.py
--rw-r--r--   0        0        0    12522 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_bgp_model.py
--rw-r--r--   0        0        0     3436 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_logging_model.py
--rw-r--r--   0        0        0     1584 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ntp_model.py
--rw-r--r--   0        0        0     3835 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_omp_model.py
--rw-r--r--   0        0        0     6749 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ospf.py
--rw-r--r--   0        0        0    13901 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ospfv3.py
--rw-r--r--   0        0        0     9589 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
--rw-r--r--   0        0        0     2581 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_snmp_model.py
--rw-r--r--   0        0        0     8986 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_system.py
--rw-r--r--   0        0        0    21665 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_vpn_interface_model.py
--rw-r--r--   0        0        0    15836 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_vpn_model.py
--rw-r--r--   0        0        0      472 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cli_template.py
--rw-r--r--   0        0        0     1835 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/omp_vsmart_model.py
--rw-r--r--   0        0        0      806 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/security_vsmart_model.py
--rw-r--r--   0        0        0     1882 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/supported.py
--rw-r--r--   0        0        0     2624 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/models/system_vsmart_model.py
--rw-r--r--   0        0        0     2261 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/aaa_model.py
--rw-r--r--   0        0        0    11178 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
--rw-r--r--   0        0        0     1041 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
--rw-r--r--   0        0        0     4264 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
--rw-r--r--   0        0        0     3735 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
--rw-r--r--   0        0        0     1999 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
--rw-r--r--   0        0        0     2558 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
--rw-r--r--   0        0        0     4547 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
--rw-r--r--   0        0        0     1843 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
--rw-r--r--   0        0        0     2247 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
--rw-r--r--   0        0        0     2098 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
--rw-r--r--   0        0        0      683 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
--rw-r--r--   0        0        0     7113 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/tenant/tenant.json.j2
--rw-r--r--   0        0        0     1460 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/tenant/tenant_model.py
--rw-r--r--   0        0        0     5013 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/tenant_backup_restore_api.py
--rw-r--r--   0        0        0     4406 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/tenant_management_api.py
--rw-r--r--   0        0        0     5090 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/tenant_migration_api.py
--rw-r--r--   0        0        0    13729 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/api/versions_utils.py
--rw-r--r--   0        0        0    21802 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/dataclasses.py
--rw-r--r--   0        0        0    27207 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/__init__.py
--rw-r--r--   0        0        0    11938 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/administration_user_and_group.py
--rw-r--r--   0        0        0     6731 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/certificate_management_device.py
--rw-r--r--   0        0        0     1476 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/certificate_management_vmanage.py
--rw-r--r--   0        0        0     4035 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/client.py
--rw-r--r--   0        0        0     2722 2024-05-23 10:34:23.269722 catalystwan-0.33.7.dev1/catalystwan/endpoints/cluster_management.py
--rw-r--r--   0        0        0      983 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/device/software_update.py
--rw-r--r--   0        0        0     9447 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/disaster_recovery.py
--rw-r--r--   0        0        0     3876 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
--rw-r--r--   0        0        0     2406 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
--rw-r--r--   0        0        0     3557 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
--rw-r--r--   0        0        0     3735 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
--rw-r--r--   0        0        0     2600 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
--rw-r--r--   0        0        0     4037 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
--rw-r--r--   0        0        0     2747 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
--rw-r--r--   0        0        0     3315 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
--rw-r--r--   0        0        0    10040 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
--rw-r--r--   0        0        0     3679 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
--rw-r--r--   0        0        0     6471 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
--rw-r--r--   0        0        0     1361 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/abstractions.py
--rw-r--r--   0        0        0     1969 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     2024 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2046 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/aip.py
--rw-r--r--   0        0        0     2046 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/amp.py
--rw-r--r--   0        0        0     1756 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/cflowd.py
--rw-r--r--   0        0        0     2025 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/control.py
--rw-r--r--   0        0        0     2170 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/device_access.py
--rw-r--r--   0        0        0     2239 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     1853 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/dns_security.py
--rw-r--r--   0        0        0     2099 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     1995 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
--rw-r--r--   0        0        0     1954 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/mesh.py
--rw-r--r--   0        0        0     1991 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/qos_map.py
--rw-r--r--   0        0        0     2065 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/rewrite.py
--rw-r--r--   0        0        0     1798 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/route_policy.py
--rw-r--r--   0        0        0     1967 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/rule_set.py
--rw-r--r--   0        0        0     2092 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/security_group.py
--rw-r--r--   0        0        0     1879 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
--rw-r--r--   0        0        0     1985 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
--rw-r--r--   0        0        0     2029 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     1869 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
--rw-r--r--   0        0        0     2184 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0     2111 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1740 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/app.py
--rw-r--r--   0        0        0     1900 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/app_probe.py
--rw-r--r--   0        0        0     1793 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/as_path.py
--rw-r--r--   0        0        0     1813 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/class_map.py
--rw-r--r--   0        0        0     1772 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/color.py
--rw-r--r--   0        0        0     1854 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/community.py
--rw-r--r--   0        0        0     1971 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0     1873 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/data_prefix.py
--rw-r--r--   0        0        0     2023 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/expanded_community.py
--rw-r--r--   0        0        0     1978 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/extended_community.py
--rw-r--r--   0        0        0     1752 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/fqdn.py
--rw-r--r--   0        0        0     1893 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/geo_location.py
--rw-r--r--   0        0        0     1930 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1873 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0     1833 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/local_app.py
--rw-r--r--   0        0        0     1893 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/local_domain.py
--rw-r--r--   0        0        0     1792 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/mirror.py
--rw-r--r--   0        0        0     1817 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/policer.py
--rw-r--r--   0        0        0     1752 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/port.py
--rw-r--r--   0        0        0     2065 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1852 2024-05-23 10:34:23.273723 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/prefix.py
--rw-r--r--   0        0        0     1930 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1683 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/region.py
--rw-r--r--   0        0        0     1892 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/site.py
--rw-r--r--   0        0        0     1782 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/sla.py
--rw-r--r--   0        0        0     1940 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0     1752 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/tloc.py
--rw-r--r--   0        0        0     1872 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
--rw-r--r--   0        0        0     1930 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
--rw-r--r--   0        0        0     1863 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
--rw-r--r--   0        0        0     1863 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/url_block_list.py
--rw-r--r--   0        0        0     1734 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/vpn.py
--rw-r--r--   0        0        0     1752 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/zone.py
--rw-r--r--   0        0        0     1726 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/security_template.py
--rw-r--r--   0        0        0     1738 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/vedge_template.py
--rw-r--r--   0        0        0     2974 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/vsmart_template.py
--rw-r--r--   0        0        0     8865 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/software_actions.py
--rw-r--r--   0        0        0     6820 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_dashboard_status.py
--rw-r--r--   0        0        0    10675 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_actions.py
--rw-r--r--   0        0        0    13973 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_inventory.py
--rw-r--r--   0        0        0      881 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_template.py
--rw-r--r--   0        0        0     5277 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_feature_profile.py
--rw-r--r--   0        0        0     6387 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_group.py
--rw-r--r--   0        0        0    27565 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_settings.py
--rw-r--r--   0        0        0    14794 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/endpoints_container.py
--rw-r--r--   0        0        0      760 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/misc.py
--rw-r--r--   0        0        0     8272 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/monitoring/device_details.py
--rw-r--r--   0        0        0      347 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/monitoring/server_info.py
--rw-r--r--   0        0        0     1929 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/monitoring/status.py
--rw-r--r--   0        0        0     1446 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/real_time_monitoring/reboot_history.py
--rw-r--r--   0        0        0     1419 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/sdavc_cloud_connector.py
--rw-r--r--   0        0        0     1047 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_backup_restore.py
--rw-r--r--   0        0        0     7648 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_management.py
--rw-r--r--   0        0        0     3649 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_migration.py
--rw-r--r--   0        0        0     3661 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
--rw-r--r--   0        0        0     6246 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/exceptions.py
--rw-r--r--   0        0        0     1340 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/base.py
--rw-r--r--   0        0        0     5165 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
--rw-r--r--   0        0        0     2364 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
--rw-r--r--   0        0        0     4587 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
--rw-r--r--   0        0        0     1834 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
--rw-r--r--   0        0        0    28479 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
--rw-r--r--   0        0        0    14507 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
--rw-r--r--   0        0        0     9901 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
--rw-r--r--   0        0        0    61890 2024-05-23 10:34:23.277722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
--rw-r--r--   0        0        0     4124 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
--rw-r--r--   0        0        0     1078 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/test_config_migration.py
--rw-r--r--   0        0        0     1902 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/integration_tests/test_find_template_values.py
--rw-r--r--   0        0        0      676 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/logging.conf
--rw-r--r--   0        0        0    16090 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/common.py
--rw-r--r--   0        0        0      194 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/common.py
--rw-r--r--   0        0        0    13622 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/config_migration.py
--rw-r--r--   0        0        0       89 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/docs/README.md
--rw-r--r--   0        0        0   142336 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/docs/diagram.png
--rw-r--r--   0        0        0    10043 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/README.md
--rw-r--r--   0        0        0      663 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/builder.py
--rw-r--r--   0        0        0    25676 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/common.py
--rw-r--r--   0        0        0     5106 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/parcel.py
--rw-r--r--   0        0        0      661 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
--rw-r--r--   0        0        0     1385 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
--rw-r--r--   0        0        0     1554 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
--rw-r--r--   0        0        0      292 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
--rw-r--r--   0        0        0      480 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
--rw-r--r--   0        0        0      275 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
--rw-r--r--   0        0        0     2787 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
--rw-r--r--   0        0        0      507 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
--rw-r--r--   0        0        0    16716 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
--rw-r--r--   0        0        0     4103 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
--rw-r--r--   0        0        0      420 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
--rw-r--r--   0        0        0     4750 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
--rw-r--r--   0        0        0     3950 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
--rw-r--r--   0        0        0     5256 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
--rw-r--r--   0        0        0     1426 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
--rw-r--r--   0        0        0     1203 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
--rw-r--r--   0        0        0      825 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
--rw-r--r--   0        0        0      653 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
--rw-r--r--   0        0        0     1244 2024-05-23 10:34:23.281722 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
--rw-r--r--   0        0        0     1034 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
--rw-r--r--   0        0        0      807 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
--rw-r--r--   0        0        0     1152 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
--rw-r--r--   0        0        0     1706 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
--rw-r--r--   0        0        0      737 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
--rw-r--r--   0        0        0     1332 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
--rw-r--r--   0        0        0     3106 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
--rw-r--r--   0        0        0     1106 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
--rw-r--r--   0        0        0     5272 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
--rw-r--r--   0        0        0     1215 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
--rw-r--r--   0        0        0     1641 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
--rw-r--r--   0        0        0     1442 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
--rw-r--r--   0        0        0     1898 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
--rw-r--r--   0        0        0     1277 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
--rw-r--r--   0        0        0      871 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
--rw-r--r--   0        0        0      830 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
--rw-r--r--   0        0        0     1288 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
--rw-r--r--   0        0        0     1398 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
--rw-r--r--   0        0        0     1604 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
--rw-r--r--   0        0        0      907 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
--rw-r--r--   0        0        0      799 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
--rw-r--r--   0        0        0     1408 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
--rw-r--r--   0        0        0     3388 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
--rw-r--r--   0        0        0     3935 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
--rw-r--r--   0        0        0     1079 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
--rw-r--r--   0        0        0     3679 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
--rw-r--r--   0        0        0     1461 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
--rw-r--r--   0        0        0     2255 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
--rw-r--r--   0        0        0    14507 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py
--rw-r--r--   0        0        0    10235 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
--rw-r--r--   0        0        0    14485 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
--rw-r--r--   0        0        0     5289 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
--rw-r--r--   0        0        0     4001 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
--rw-r--r--   0        0        0     1349 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
--rw-r--r--   0        0        0    12626 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
--rw-r--r--   0        0        0     6938 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
--rw-r--r--   0        0        0     6350 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
--rw-r--r--   0        0        0     5349 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
--rw-r--r--   0        0        0     8633 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
--rw-r--r--   0        0        0    24965 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
--rw-r--r--   0        0        0    10821 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
--rw-r--r--   0        0        0     3291 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
--rw-r--r--   0        0        0     7362 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py
--rw-r--r--   0        0        0    12770 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py
--rw-r--r--   0        0        0     9187 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
--rw-r--r--   0        0        0     6966 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
--rw-r--r--   0        0        0     5161 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
--rw-r--r--   0        0        0     3705 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
--rw-r--r--   0        0        0     5706 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
--rw-r--r--   0        0        0      297 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
--rw-r--r--   0        0        0    16817 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
--rw-r--r--   0        0        0     1058 2024-05-23 10:34:23.285723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
--rw-r--r--   0        0        0    15436 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
--rw-r--r--   0        0        0      977 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
--rw-r--r--   0        0        0    10457 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
--rw-r--r--   0        0        0     2623 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
--rw-r--r--   0        0        0     6396 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
--rw-r--r--   0        0        0     6355 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
--rw-r--r--   0        0        0     2935 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
--rw-r--r--   0        0        0     3932 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
--rw-r--r--   0        0        0     5166 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
--rw-r--r--   0        0        0     6653 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
--rw-r--r--   0        0        0     6841 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
--rw-r--r--   0        0        0      726 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
--rw-r--r--   0        0        0    12828 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
--rw-r--r--   0        0        0     2162 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
--rw-r--r--   0        0        0      799 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
--rw-r--r--   0        0        0     2530 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
--rw-r--r--   0        0        0    26093 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py
--rw-r--r--   0        0        0     2276 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
--rw-r--r--   0        0        0     2668 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
--rw-r--r--   0        0        0     1579 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
--rw-r--r--   0        0        0     5634 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py
--rw-r--r--   0        0        0     4400 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
--rw-r--r--   0        0        0    12662 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
--rw-r--r--   0        0        0     9090 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
--rw-r--r--   0        0        0    13993 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
--rw-r--r--   0        0        0     2169 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
--rw-r--r--   0        0        0     5137 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
--rw-r--r--   0        0        0    11421 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
--rw-r--r--   0        0        0    16558 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
--rw-r--r--   0        0        0     8889 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
--rw-r--r--   0        0        0      157 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/profile_type.py
--rw-r--r--   0        0        0      378 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/configuration/topology_group.py
--rw-r--r--   0        0        0     1041 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/device_inventory.py
--rw-r--r--   0        0        0      341 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/feature_profile_parcel.py
--rw-r--r--   0        0        0      785 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/misc/application_protocols.py
--rw-r--r--   0        0        0      405 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/monitoring/server_info.py
--rw-r--r--   0        0        0    10542 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/policy/__init__.py
--rw-r--r--   0        0        0     8738 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/policy/centralized.py
--rw-r--r--   0        0        0     5789 2024-05-23 10:34:23.289723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/access_control_list.py
--rw-r--r--   0        0        0     5991 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/access_control_list_ipv6.py
--rw-r--r--   0        0        0     2204 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/aip.py
--rw-r--r--   0        0        0     2598 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/amp.py
--rw-r--r--   0        0        0     3159 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/cflowd.py
--rw-r--r--   0        0        0    12117 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/control.py
--rw-r--r--   0        0        0     4134 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/device_access.py
--rw-r--r--   0        0        0     4250 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/device_access_ipv6.py
--rw-r--r--   0        0        0     4585 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/dns_security.py
--rw-r--r--   0        0        0     3251 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/hub_and_spoke.py
--rw-r--r--   0        0        0     2139 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/intrusion_prevention.py
--rw-r--r--   0        0        0     1403 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/mesh.py
--rw-r--r--   0        0        0     3520 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/qos_map.py
--rw-r--r--   0        0        0     1410 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/rewrite.py
--rw-r--r--   0        0        0     6150 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/route_policy.py
--rw-r--r--   0        0        0    12381 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/rule_set.py
--rw-r--r--   0        0        0     3147 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/security_group.py
--rw-r--r--   0        0        0     7992 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/ssl_decryption.py
--rw-r--r--   0        0        0     3539 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
--rw-r--r--   0        0        0    14018 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/traffic_data.py
--rw-r--r--   0        0        0     2684 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/url_filtering.py
--rw-r--r--   0        0        0     1329 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/vpn_membership.py
--rw-r--r--   0        0        0    10584 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/zone_based_firewall.py
--rw-r--r--   0        0        0     1094 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/app.py
--rw-r--r--   0        0        0     1295 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/app_probe.py
--rw-r--r--   0        0        0      651 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/as_path.py
--rw-r--r--   0        0        0      789 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/class_map.py
--rw-r--r--   0        0        0      661 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/color.py
--rw-r--r--   0        0        0     2634 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/communities.py
--rw-r--r--   0        0        0      918 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/data_ipv6_prefix.py
--rw-r--r--   0        0        0      860 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/data_prefix.py
--rw-r--r--   0        0        0      495 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/fqdn.py
--rw-r--r--   0        0        0     1055 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/geo_location.py
--rw-r--r--   0        0        0      817 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/ips_signature.py
--rw-r--r--   0        0        0     1111 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/ipv6_prefix.py
--rw-r--r--   0        0        0      990 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/local_app.py
--rw-r--r--   0        0        0      923 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/local_domain.py
--rw-r--r--   0        0        0      714 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/mirror.py
--rw-r--r--   0        0        0     1127 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/policer.py
--rw-r--r--   0        0        0      771 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/port.py
--rw-r--r--   0        0        0     3196 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/preferred_color_group.py
--rw-r--r--   0        0        0     1055 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/prefix.py
--rw-r--r--   0        0        0      723 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/protocol_name.py
--rw-r--r--   0        0        0     1325 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/region.py
--rw-r--r--   0        0        0      942 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/site.py
--rw-r--r--   0        0        0     6864 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/sla.py
--rw-r--r--   0        0        0      970 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/threat_grid_api_key.py
--rw-r--r--   0        0        0      960 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/tloc.py
--rw-r--r--   0        0        0     2111 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/trunkgroup.py
--rw-r--r--   0        0        0      824 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/umbrella_data.py
--rw-r--r--   0        0        0      856 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/url.py
--rw-r--r--   0        0        0     1071 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/vpn.py
--rw-r--r--   0        0        0     1405 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/list/zone.py
--rw-r--r--   0        0        0     6204 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/localized.py
--rw-r--r--   0        0        0     3752 2024-05-23 10:34:23.293723 catalystwan-0.33.7.dev1/catalystwan/models/policy/policy.py
--rw-r--r--   0        0        0    37156 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/models/policy/policy_definition.py
--rw-r--r--   0        0        0     1557 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/models/policy/policy_list.py
--rw-r--r--   0        0        0     9385 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/models/policy/security.py
--rw-r--r--   0        0        0     2437 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/models/templates.py
--rw-r--r--   0        0        0     5239 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/models/tenant.py
--rw-r--r--   0        0        0     9717 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/response.py
--rw-r--r--   0        0        0    19497 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/session.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/__init__.py
--rw-r--r--   0        0        0     1236 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_converter_chooser.py
--rw-r--r--   0        0        0      467 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
--rw-r--r--   0        0        0    10804 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
--rw-r--r--   0        0        0      519 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/malformed.py
--rw-r--r--   0        0        0     3185 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
--rw-r--r--   0        0        0     3583 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_device_template_with_info.py
--rw-r--r--   0        0        0     6139 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_merge_parcels.py
--rw-r--r--   0        0        0     4525 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_normalizer.py
--rw-r--r--   0        0        0    10765 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_transform.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/models/__init__.py
--rw-r--r--   0        0        0      401 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
--rw-r--r--   0        0        0      513 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/banner_1.json
--rw-r--r--   0        0        0      116 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/alias.json
--rw-r--r--   0        0        0      114 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/basic.json
--rw-r--r--   0        0        0      109 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/basic_no_value.json
--rw-r--r--   0        0        0      848 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children.json
--rw-r--r--   0        0        0     2348 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children_nested.json
--rw-r--r--   0        0        0     2348 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      274 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/data_path.json
--rw-r--r--   0        0        0     2973 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/cisco_bfd.json
--rw-r--r--   0        0        0    11100 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/complex_aaa.json
--rw-r--r--   0        0        0    41165 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
--rw-r--r--   0        0        0     5219 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/default_cisco_system.json
--rw-r--r--   0        0        0     5505 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/iuo.json
--rw-r--r--   0        0        0      249 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/omp_1.json
--rw-r--r--   0        0        0      875 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/omp_2.json
--rw-r--r--   0        0        0     1682 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/omp_3.json
--rw-r--r--   0        0        0      662 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/__init__.py
--rw-r--r--   0        0        0     2828 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_aaa.py
--rw-r--r--   0        0        0      303 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_banner.py
--rw-r--r--   0        0        0      587 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_bfd.py
--rw-r--r--   0        0        0      344 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_system.py
--rw-r--r--   0        0        0     8078 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_vpn.py
--rw-r--r--   0        0        0     1091 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/omp_vsmart.py
--rw-r--r--   0        0        0      605 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/alias.json
--rw-r--r--   0        0        0      574 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/basic.json
--rw-r--r--   0        0        0     1810 2024-05-23 10:34:23.297723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children.json
--rw-r--r--   0        0        0     4005 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children_nested.json
--rw-r--r--   0        0        0     4005 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
--rw-r--r--   0        0        0      731 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/data_path.json
--rw-r--r--   0        0        0    43436 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cedge_aaa.json
--rw-r--r--   0        0        0     1200 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_banner.json
--rw-r--r--   0        0        0     9495 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_bfd.json
--rw-r--r--   0        0        0    99045 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_system.json
--rw-r--r--   0        0        0    87854 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_vpn.json
--rw-r--r--   0        0        0     5939 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/omp-vsmart.json
--rw-r--r--   0        0        0     1381 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_chose_model.py
--rw-r--r--   0        0        0     2598 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_deserialize_model.py
--rw-r--r--   0        0        0     6762 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_find_template_values.py
--rw-r--r--   0        0        0     4598 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_generate_payload.py
--rw-r--r--   0        0        0     1755 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_serialize_model.py
--rw-r--r--   0        0        0     8145 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_admin_tech_api.py
--rw-r--r--   0        0        0    17792 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_administration.py
--rw-r--r--   0        0        0    11116 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_alarms_api.py
--rw-r--r--   0        0        0     8322 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_cli_template.py
--rw-r--r--   0        0        0     5494 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_creation_tools.py
--rw-r--r--   0        0        0     3981 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_device_action_api.py
--rw-r--r--   0        0        0    28159 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_devices_api.py
--rw-r--r--   0        0        0    34864 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_endpoints.py
--rw-r--r--   0        0        0    10585 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_feature_profile_api.py
--rw-r--r--   0        0        0      894 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_feature_template_field.py
--rw-r--r--   0        0        0     1545 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_logs_api.py
--rw-r--r--   0        0        0     1899 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_models_common.py
--rw-r--r--   0        0        0     1809 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_monitoring_server_info.py
--rw-r--r--   0        0        0     5489 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_monitoring_status_api.py
--rw-r--r--   0        0        0    11026 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_mtt_aaa_api.py
--rw-r--r--   0        0        0    10026 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_normalize_to_model_definition.py
--rw-r--r--   0        0        0    16472 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_omp_api.py
--rw-r--r--   0        0        0     5223 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_packet_capture.py
--rw-r--r--   0        0        0     5727 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_partition_manager_api.py
--rw-r--r--   0        0        0     7926 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_response.py
--rw-r--r--   0        0        0     6724 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_session.py
--rw-r--r--   0        0        0     7117 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_software_action_api.py
--rw-r--r--   0        0        0     6071 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_speed_test_api.py
--rw-r--r--   0        0        0    14926 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_task_status_api.py
--rw-r--r--   0        0        0    15055 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_templates.py
--rw-r--r--   0        0        0     3705 2024-05-23 10:34:23.301723 catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_backup_restore_api.py
--rw-r--r--   0        0        0     6114 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_management_api.py
--rw-r--r--   0        0        0     4506 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_migration_api.py
--rw-r--r--   0        0        0    12377 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_typed_list.py
--rw-r--r--   0        0        0     2968 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_version.py
--rw-r--r--   0        0        0    10377 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_version_utils.py
--rw-r--r--   0        0        0     3343 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/tests/test_vmanage_auth.py
--rw-r--r--   0        0        0     9379 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/typed_list.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/__init__.py
--rw-r--r--   0        0        0      266 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/alarm_status.py
--rw-r--r--   0        0        0      253 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/certificate_status.py
--rw-r--r--   0        0        0      279 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/colors.py
--rw-r--r--   0        0        0      239 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/exceptions.py
--rw-r--r--   0        0        0      320 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/__init__.py
--rw-r--r--   0        0        0     3433 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/aaa.py
--rw-r--r--   0        0        0     5810 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
--rw-r--r--   0        0        0      784 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/banner.py
--rw-r--r--   0        0        0      268 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/base.py
--rw-r--r--   0        0        0     3283 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/basic.py
--rw-r--r--   0        0        0      898 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/bfd.py
--rw-r--r--   0        0        0     4591 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/bgp.py
--rw-r--r--   0        0        0     1520 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
--rw-r--r--   0        0        0     3269 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
--rw-r--r--   0        0        0      756 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cli.py
--rw-r--r--   0        0        0     1932 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
--rw-r--r--   0        0        0     4387 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
--rw-r--r--   0        0        0     5349 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
--rw-r--r--   0        0        0     6240 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
--rw-r--r--   0        0        0      578 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/global_.py
--rw-r--r--   0        0        0     1573 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/gps.py
--rw-r--r--   0        0        0      331 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/helpers.py
--rw-r--r--   0        0        0    12974 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
--rw-r--r--   0        0        0     5619 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
--rw-r--r--   0        0        0     5331 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
--rw-r--r--   0        0        0     9349 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
--rw-r--r--   0        0        0     7411 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
--rw-r--r--   0        0        0     1963 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/logging_.py
--rw-r--r--   0        0        0     4855 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
--rw-r--r--   0        0        0    13085 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/multicast.py
--rw-r--r--   0        0        0     5329 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
--rw-r--r--   0        0        0     2295 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ntp.py
--rw-r--r--   0        0        0     1475 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/omp.py
--rw-r--r--   0        0        0     5520 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ospf.py
--rw-r--r--   0        0        0    11012 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
--rw-r--r--   0        0        0     6200 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
--rw-r--r--   0        0        0     1568 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/security.py
--rw-r--r--   0        0        0    10159 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/sig.py
--rw-r--r--   0        0        0     2240 2024-05-23 10:34:23.305723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/snmp.py
--rw-r--r--   0        0        0     9032 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/switchport.py
--rw-r--r--   0        0        0     2776 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
--rw-r--r--   0        0        0     2250 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ucse.py
--rw-r--r--   0        0        0    33006 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/vpn.py
--rw-r--r--   0        0        0     5742 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
--rw-r--r--   0        0        0    13158 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
--rw-r--r--   0        0        0     4844 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
--rw-r--r--   0        0        0     6866 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
--rw-r--r--   0        0        0    14360 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
--rw-r--r--   0        0        0    18190 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
--rw-r--r--   0        0        0     5344 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
--rw-r--r--   0        0        0     8057 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
--rw-r--r--   0        0        0     2540 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
--rw-r--r--   0        0        0     9564 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/policy/policy_lists.py
--rw-r--r--   0        0        0     6694 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/creators/config_pusher.py
--rw-r--r--   0        0        0     5570 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/creators/strategy/parcels.py
--rw-r--r--   0        0        0     1686 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/factories/feature_profile_api.py
--rw-r--r--   0        0        0     1257 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/factories/parcel_pusher.py
--rw-r--r--   0        0        0     1671 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/reverters/config_reverter.py
--rw-r--r--   0        0        0        0 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/steps/__init__.py
--rw-r--r--   0        0        0     3174 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/steps/constants.py
--rw-r--r--   0        0        0     5979 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/steps/transform.py
--rw-r--r--   0        0        0      154 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/config_status.py
--rw-r--r--   0        0        0     4778 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/creation_tools.py
--rw-r--r--   0        0        0     7281 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/dashboard.py
--rw-r--r--   0        0        0     2863 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/device_model.py
--rw-r--r--   0        0        0     2110 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/dict.py
--rw-r--r--   0        0        0      953 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/feature_template/choose_model.py
--rw-r--r--   0        0        0     4882 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/feature_template/find_template_values.py
--rw-r--r--   0        0        0      584 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/operation_status.py
--rw-r--r--   0        0        0      196 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/personality.py
--rw-r--r--   0        0        0      360 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/pydantic_field.py
--rw-r--r--   0        0        0      172 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/reachability.py
--rw-r--r--   0        0        0      407 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/session_type.py
--rw-r--r--   0        0        0      149 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/template_type.py
--rw-r--r--   0        0        0     9825 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/timezone.py
--rw-r--r--   0        0        0     3930 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/upgrades_helper.py
--rw-r--r--   0        0        0      159 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/utils/validate_status.py
--rw-r--r--   0        0        0     3032 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/version.py
--rw-r--r--   0        0        0     5415 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/vmanage_auth.py
--rw-r--r--   0        0        0    15970 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/workflows/config_migration.py
--rw-r--r--   0        0        0     9946 2024-05-23 10:34:23.309723 catalystwan-0.33.7.dev1/catalystwan/workflows/tenant_migration.py
--rw-r--r--   0        0        0      866 2024-05-23 10:34:23.313723 catalystwan-0.33.7.dev1/pyproject.toml
--rw-r--r--   0        0        0    18717 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev1/setup.py
--rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11375 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/LICENSE
+-rw-r--r--   0        0        0    13533 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/README.md
+-rw-r--r--   0        0        0     2558 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/__init__.py
+-rw-r--r--   0        0        0     1532 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/abstractions.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/__init__.py
+-rw-r--r--   0        0        0     6689 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/admin_tech_api.py
+-rw-r--r--   0        0        0    14935 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/administration.py
+-rw-r--r--   0        0        0     6314 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/alarms_api.py
+-rw-r--r--   0        0        0     3293 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/api_container.py
+-rw-r--r--   0        0        0    11636 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/basic_api.py
+-rw-r--r--   0        0        0      386 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/__init__.py
+-rw-r--r--   0        0        0     2017 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py
+-rw-r--r--   0        0        0     2679 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/cli.py
+-rw-r--r--   0        0        0     2696 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/other.py
+-rw-r--r--   0        0        0     3889 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/report.py
+-rw-r--r--   0        0        0     8611 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/service.py
+-rw-r--r--   0        0        0     2768 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/system.py
+-rw-r--r--   0        0        0     8776 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/transport.py
+-rw-r--r--   0        0        0     2053 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/config_device_inventory_api.py
+-rw-r--r--   0        0        0     4760 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/config_group_api.py
+-rw-r--r--   0        0        0     6672 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/configuration_groups/parcel.py
+-rw-r--r--   0        0        0     7315 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/dashboard_api.py
+-rw-r--r--   0        0        0     7360 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/device_action_api.py
+-rw-r--r--   0        0        0    55556 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/feature_profile_api.py
+-rw-r--r--   0        0        0     1919 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/logs_api.py
+-rw-r--r--   0        0        0     2449 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/monitoring_status_api.py
+-rw-r--r--   0        0        0     6036 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/mtt_aaa_api.py
+-rw-r--r--   0        0        0     4394 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/omp_api.py
+-rw-r--r--   0        0        0     5691 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/packet_capture_api.py
+-rw-r--r--   0        0        0     1654 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/parcel_api.py
+-rw-r--r--   0        0        0     5600 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/partition_manager_api.py
+-rw-r--r--   0        0        0    36861 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/policy_api.py
+-rw-r--r--   0        0        0     2284 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/resource_pool_api.py
+-rw-r--r--   0        0        0    11320 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/software_action_api.py
+-rw-r--r--   0        0        0     5473 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/speedtest_api.py
+-rw-r--r--   0        0        0     7149 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/task_status_api.py
+-rw-r--r--   0        0        0    30133 2024-05-27 16:09:36.226934 catalystwan-0.33.7.dev2/catalystwan/api/template_api.py
+-rw-r--r--   0        0        0     3540 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/README.md
+-rw-r--r--   0        0        0      251 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/bool_str.py
+-rw-r--r--   0        0        0     7481 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/cli_template.py
+-rw-r--r--   0        0        0     3425 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template.py
+-rw-r--r--   0        0        0      571 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2
+-rw-r--r--   0        0        0      137 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/device_variable.py
+-rw-r--r--   0        0        0     5029 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template.py
+-rw-r--r--   0        0        0     6576 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_field.py
+-rw-r--r--   0        0        0      661 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_payload.py
+-rw-r--r--   0        0        0     3244 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_aaa_model.py
+-rw-r--r--   0        0        0      667 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_banner_model.py
+-rw-r--r--   0        0        0     2180 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bfd_model.py
+-rw-r--r--   0        0        0    12522 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bgp_model.py
+-rw-r--r--   0        0        0     3436 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_logging_model.py
+-rw-r--r--   0        0        0     1584 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ntp_model.py
+-rw-r--r--   0        0        0     3835 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_omp_model.py
+-rw-r--r--   0        0        0     6749 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospf.py
+-rw-r--r--   0        0        0    13901 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospfv3.py
+-rw-r--r--   0        0        0     9589 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py
+-rw-r--r--   0        0        0     2581 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_snmp_model.py
+-rw-r--r--   0        0        0     8986 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_system.py
+-rw-r--r--   0        0        0    21665 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py
+-rw-r--r--   0        0        0    15836 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_model.py
+-rw-r--r--   0        0        0      472 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cli_template.py
+-rw-r--r--   0        0        0     1835 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/omp_vsmart_model.py
+-rw-r--r--   0        0        0      806 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/security_vsmart_model.py
+-rw-r--r--   0        0        0     1882 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/supported.py
+-rw-r--r--   0        0        0     2624 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/models/system_vsmart_model.py
+-rw-r--r--   0        0        0     2261 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py
+-rw-r--r--   0        0        0    11178 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2
+-rw-r--r--   0        0        0     1041 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2
+-rw-r--r--   0        0        0     4264 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2
+-rw-r--r--   0        0        0     3735 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2
+-rw-r--r--   0        0        0     1999 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2
+-rw-r--r--   0        0        0     2558 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py
+-rw-r--r--   0        0        0     4547 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2
+-rw-r--r--   0        0        0     1843 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2
+-rw-r--r--   0        0        0     2247 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2
+-rw-r--r--   0        0        0     2098 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2
+-rw-r--r--   0        0        0      683 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2
+-rw-r--r--   0        0        0     7113 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2
+-rw-r--r--   0        0        0     1460 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py
+-rw-r--r--   0        0        0     5013 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     4406 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_management_api.py
+-rw-r--r--   0        0        0     5090 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/tenant_migration_api.py
+-rw-r--r--   0        0        0    13729 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/api/versions_utils.py
+-rw-r--r--   0        0        0    21802 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/dataclasses.py
+-rw-r--r--   0        0        0    25624 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/__init__.py
+-rw-r--r--   0        0        0    11938 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/administration_user_and_group.py
+-rw-r--r--   0        0        0     6731 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_device.py
+-rw-r--r--   0        0        0     1476 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_vmanage.py
+-rw-r--r--   0        0        0     4035 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/client.py
+-rw-r--r--   0        0        0     2722 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/cluster_management.py
+-rw-r--r--   0        0        0      983 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/device/software_update.py
+-rw-r--r--   0        0        0     9447 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/disaster_recovery.py
+-rw-r--r--   0        0        0     3876 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py
+-rw-r--r--   0        0        0     2406 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py
+-rw-r--r--   0        0        0     3557 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py
+-rw-r--r--   0        0        0     3735 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py
+-rw-r--r--   0        0        0     2600 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py
+-rw-r--r--   0        0        0     4419 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py
+-rw-r--r--   0        0        0     3585 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py
+-rw-r--r--   0        0        0     3315 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py
+-rw-r--r--   0        0        0    10040 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py
+-rw-r--r--   0        0        0     3679 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py
+-rw-r--r--   0        0        0     7276 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py
+-rw-r--r--   0        0        0      442 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/network_hierarchy.py
+-rw-r--r--   0        0        0     1361 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/abstractions.py
+-rw-r--r--   0        0        0     1969 2024-05-27 16:09:36.230934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     2024 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2046 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/aip.py
+-rw-r--r--   0        0        0     2046 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py
+-rw-r--r--   0        0        0     1756 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/cflowd.py
+-rw-r--r--   0        0        0     2025 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/control.py
+-rw-r--r--   0        0        0     2170 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py
+-rw-r--r--   0        0        0     2239 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     1853 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     2099 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     1995 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1954 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py
+-rw-r--r--   0        0        0     1991 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     2065 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     1798 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/route_policy.py
+-rw-r--r--   0        0        0     1967 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     2092 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py
+-rw-r--r--   0        0        0     1879 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     1985 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0     2029 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     1869 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     2184 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0     2111 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1740 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app.py
+-rw-r--r--   0        0        0     1900 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py
+-rw-r--r--   0        0        0     1793 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py
+-rw-r--r--   0        0        0     1813 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py
+-rw-r--r--   0        0        0     1772 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/color.py
+-rw-r--r--   0        0        0     1854 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/community.py
+-rw-r--r--   0        0        0     1971 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0     1873 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py
+-rw-r--r--   0        0        0     2023 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py
+-rw-r--r--   0        0        0     1978 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/extended_community.py
+-rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1893 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py
+-rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1873 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0     1833 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py
+-rw-r--r--   0        0        0     1893 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py
+-rw-r--r--   0        0        0     1792 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py
+-rw-r--r--   0        0        0     1817 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/policer.py
+-rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/port.py
+-rw-r--r--   0        0        0     2065 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1852 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py
+-rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1683 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/region.py
+-rw-r--r--   0        0        0     1892 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/site.py
+-rw-r--r--   0        0        0     1782 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/sla.py
+-rw-r--r--   0        0        0     1940 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py
+-rw-r--r--   0        0        0     1872 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0     1930 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0     1863 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py
+-rw-r--r--   0        0        0     1863 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py
+-rw-r--r--   0        0        0     1734 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py
+-rw-r--r--   0        0        0     1752 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/zone.py
+-rw-r--r--   0        0        0     1726 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/security_template.py
+-rw-r--r--   0        0        0     1738 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py
+-rw-r--r--   0        0        0     2974 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py
+-rw-r--r--   0        0        0     8865 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/software_actions.py
+-rw-r--r--   0        0        0      784 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/topology_group.py
+-rw-r--r--   0        0        0     6820 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_dashboard_status.py
+-rw-r--r--   0        0        0    10675 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_actions.py
+-rw-r--r--   0        0        0    13973 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_inventory.py
+-rw-r--r--   0        0        0      881 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_template.py
+-rw-r--r--   0        0        0     5287 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_feature_profile.py
+-rw-r--r--   0        0        0     6387 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_group.py
+-rw-r--r--   0        0        0    27565 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_settings.py
+-rw-r--r--   0        0        0    15076 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/endpoints_container.py
+-rw-r--r--   0        0        0      760 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/misc.py
+-rw-r--r--   0        0        0     8272 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/device_details.py
+-rw-r--r--   0        0        0      347 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/server_info.py
+-rw-r--r--   0        0        0     1929 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/status.py
+-rw-r--r--   0        0        0     1446 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py
+-rw-r--r--   0        0        0     1419 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/sdavc_cloud_connector.py
+-rw-r--r--   0        0        0     1047 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_backup_restore.py
+-rw-r--r--   0        0        0     7648 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_management.py
+-rw-r--r--   0        0        0     3649 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_migration.py
+-rw-r--r--   0        0        0     3661 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py
+-rw-r--r--   0        0        0     6246 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/exceptions.py
+-rw-r--r--   0        0        0     1340 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py
+-rw-r--r--   0        0        0    16862 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_application_priority.py
+-rw-r--r--   0        0        0     2364 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py
+-rw-r--r--   0        0        0     4587 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py
+-rw-r--r--   0        0        0     2459 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_extended_community.py
+-rw-r--r--   0        0        0     1834 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py
+-rw-r--r--   0        0        0    30868 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py
+-rw-r--r--   0        0        0    14507 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py
+-rw-r--r--   0        0        0    12728 2024-05-27 16:09:36.234934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py
+-rw-r--r--   0        0        0    63086 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py
+-rw-r--r--   0        0        0     4124 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py
+-rw-r--r--   0        0        0      683 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/base.py
+-rw-r--r--   0        0        0     3861 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_service.py
+-rw-r--r--   0        0        0     2647 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_transport.py
+-rw-r--r--   0        0        0     1078 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_config_migration.py
+-rw-r--r--   0        0        0     3803 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_data/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_find_template_values.py
+-rw-r--r--   0        0        0      676 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/logging.conf
+-rw-r--r--   0        0        0    16233 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/common.py
+-rw-r--r--   0        0        0      194 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/common.py
+-rw-r--r--   0        0        0    20593 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/config_migration.py
+-rw-r--r--   0        0        0       89 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/README.md
+-rw-r--r--   0        0        0   142336 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/diagram.png
+-rw-r--r--   0        0        0    10043 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/README.md
+-rw-r--r--   0        0        0      663 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/builder.py
+-rw-r--r--   0        0        0    28615 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/common.py
+-rw-r--r--   0        0        0     5933 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/parcel.py
+-rw-r--r--   0        0        0      324 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/__init__.py
+-rw-r--r--   0        0        0    12853 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv4acl.py
+-rw-r--r--   0        0        0    12379 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/acl/ipv6acl.py
+-rw-r--r--   0        0        0     4708 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/__init__.py
+-rw-r--r--   0        0        0     1385 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py
+-rw-r--r--   0        0        0     1572 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py
+-rw-r--r--   0        0        0    29351 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/traffic_policy.py
+-rw-r--r--   0        0        0      292 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/cli/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/cli/config.py
+-rw-r--r--   0        0        0      275 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/__init__.py
+-rw-r--r--   0        0        0     2787 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py
+-rw-r--r--   0        0        0      507 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/__init__.py
+-rw-r--r--   0        0        0    16716 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py
+-rw-r--r--   0        0        0     4146 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py
+-rw-r--r--   0        0        0      420 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/__init__.py
+-rw-r--r--   0        0        0     4750 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py
+-rw-r--r--   0        0        0     3950 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py
+-rw-r--r--   0        0        0     5327 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py
+-rw-r--r--   0        0        0     1426 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py
+-rw-r--r--   0        0        0     1203 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py
+-rw-r--r--   0        0        0      825 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py
+-rw-r--r--   0        0        0      653 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py
+-rw-r--r--   0        0        0     1244 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py
+-rw-r--r--   0        0        0      981 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py
+-rw-r--r--   0        0        0     1305 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/extended_community.py
+-rw-r--r--   0        0        0      807 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py
+-rw-r--r--   0        0        0     1152 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py
+-rw-r--r--   0        0        0     1706 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py
+-rw-r--r--   0        0        0     1096 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py
+-rw-r--r--   0        0        0     1332 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py
+-rw-r--r--   0        0        0     3106 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py
+-rw-r--r--   0        0        0     1106 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py
+-rw-r--r--   0        0        0     5255 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py
+-rw-r--r--   0        0        0     1215 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py
+-rw-r--r--   0        0        0     1641 2024-05-27 16:09:36.238934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py
+-rw-r--r--   0        0        0     1485 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py
+-rw-r--r--   0        0        0     1898 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py
+-rw-r--r--   0        0        0     1277 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py
+-rw-r--r--   0        0        0      871 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py
+-rw-r--r--   0        0        0      830 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py
+-rw-r--r--   0        0        0     1288 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py
+-rw-r--r--   0        0        0     1398 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py
+-rw-r--r--   0        0        0     1604 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py
+-rw-r--r--   0        0        0      907 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py
+-rw-r--r--   0        0        0      799 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py
+-rw-r--r--   0        0        0     1408 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py
+-rw-r--r--   0        0        0     3388 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py
+-rw-r--r--   0        0        0     3935 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py
+-rw-r--r--   0        0        0     1079 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py
+-rw-r--r--   0        0        0     3679 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py
+-rw-r--r--   0        0        0     1461 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py
+-rw-r--r--   0        0        0      667 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/__init__.py
+-rw-r--r--   0        0        0    25515 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py
+-rw-r--r--   0        0        0     7425 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py
+-rw-r--r--   0        0        0    12993 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py
+-rw-r--r--   0        0        0     2066 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py
+-rw-r--r--   0        0        0    10235 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py
+-rw-r--r--   0        0        0    14485 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py
+-rw-r--r--   0        0        0     5289 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py
+-rw-r--r--   0        0        0     4001 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py
+-rw-r--r--   0        0        0     1349 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py
+-rw-r--r--   0        0        0    12626 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py
+-rw-r--r--   0        0        0     6938 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py
+-rw-r--r--   0        0        0     6350 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py
+-rw-r--r--   0        0        0     5347 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py
+-rw-r--r--   0        0        0     8633 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py
+-rw-r--r--   0        0        0    23869 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py
+-rw-r--r--   0        0        0    10821 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py
+-rw-r--r--   0        0        0     3291 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py
+-rw-r--r--   0        0        0     9187 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py
+-rw-r--r--   0        0        0     6966 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py
+-rw-r--r--   0        0        0     5161 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py
+-rw-r--r--   0        0        0     3705 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py
+-rw-r--r--   0        0        0     5706 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py
+-rw-r--r--   0        0        0      297 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/__init__.py
+-rw-r--r--   0        0        0    16817 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py
+-rw-r--r--   0        0        0     1287 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py
+-rw-r--r--   0        0        0    15436 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py
+-rw-r--r--   0        0        0      977 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py
+-rw-r--r--   0        0        0    10457 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py
+-rw-r--r--   0        0        0     2623 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py
+-rw-r--r--   0        0        0     6844 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access.py
+-rw-r--r--   0        0        0     6847 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/device_access_ipv6.py
+-rw-r--r--   0        0        0     6396 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py
+-rw-r--r--   0        0        0     6355 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py
+-rw-r--r--   0        0        0     2935 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py
+-rw-r--r--   0        0        0     3932 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py
+-rw-r--r--   0        0        0     5166 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py
+-rw-r--r--   0        0        0     6653 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py
+-rw-r--r--   0        0        0     6841 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py
+-rw-r--r--   0        0        0      726 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py
+-rw-r--r--   0        0        0    12828 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py
+-rw-r--r--   0        0        0     2162 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py
+-rw-r--r--   0        0        0      799 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py
+-rw-r--r--   0        0        0     2671 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py
+-rw-r--r--   0        0        0     2298 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py
+-rw-r--r--   0        0        0     2754 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py
+-rw-r--r--   0        0        0     1579 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py
+-rw-r--r--   0        0        0     5633 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py
+-rw-r--r--   0        0        0     4400 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py
+-rw-r--r--   0        0        0    10979 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py
+-rw-r--r--   0        0        0     9090 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py
+-rw-r--r--   0        0        0    13993 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py
+-rw-r--r--   0        0        0     2169 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py
+-rw-r--r--   0        0        0     5137 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py
+-rw-r--r--   0        0        0    11421 2024-05-27 16:09:36.242934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py
+-rw-r--r--   0        0        0    16558 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py
+-rw-r--r--   0        0        0     8889 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py
+-rw-r--r--   0        0        0     2788 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/network_hierarchy.py
+-rw-r--r--   0        0        0      157 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/profile_type.py
+-rw-r--r--   0        0        0     1073 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/configuration/topology_group.py
+-rw-r--r--   0        0        0     1041 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/device_inventory.py
+-rw-r--r--   0        0        0      341 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/feature_profile_parcel.py
+-rw-r--r--   0        0        0      785 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/misc/application_protocols.py
+-rw-r--r--   0        0        0      405 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/monitoring/server_info.py
+-rw-r--r--   0        0        0    10542 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/__init__.py
+-rw-r--r--   0        0        0     8738 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/centralized.py
+-rw-r--r--   0        0        0     5789 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list.py
+-rw-r--r--   0        0        0     5991 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py
+-rw-r--r--   0        0        0     2204 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/aip.py
+-rw-r--r--   0        0        0     2598 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/amp.py
+-rw-r--r--   0        0        0     3159 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/cflowd.py
+-rw-r--r--   0        0        0    12158 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/control.py
+-rw-r--r--   0        0        0     4134 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access.py
+-rw-r--r--   0        0        0     4250 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access_ipv6.py
+-rw-r--r--   0        0        0     4585 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/dns_security.py
+-rw-r--r--   0        0        0     3251 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/hub_and_spoke.py
+-rw-r--r--   0        0        0     2139 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/intrusion_prevention.py
+-rw-r--r--   0        0        0     1403 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/mesh.py
+-rw-r--r--   0        0        0     3520 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/qos_map.py
+-rw-r--r--   0        0        0     1410 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rewrite.py
+-rw-r--r--   0        0        0     6150 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/route_policy.py
+-rw-r--r--   0        0        0    12381 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rule_set.py
+-rw-r--r--   0        0        0     3147 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/security_group.py
+-rw-r--r--   0        0        0     7992 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption.py
+-rw-r--r--   0        0        0     3539 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py
+-rw-r--r--   0        0        0    14018 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/traffic_data.py
+-rw-r--r--   0        0        0     2684 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/url_filtering.py
+-rw-r--r--   0        0        0     1329 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/vpn_membership.py
+-rw-r--r--   0        0        0    10584 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/zone_based_firewall.py
+-rw-r--r--   0        0        0     1331 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app.py
+-rw-r--r--   0        0        0     1295 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app_probe.py
+-rw-r--r--   0        0        0      651 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/as_path.py
+-rw-r--r--   0        0        0      789 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/class_map.py
+-rw-r--r--   0        0        0      661 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/color.py
+-rw-r--r--   0        0        0     2634 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/communities.py
+-rw-r--r--   0        0        0      918 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py
+-rw-r--r--   0        0        0      860 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_prefix.py
+-rw-r--r--   0        0        0      495 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/fqdn.py
+-rw-r--r--   0        0        0     1055 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/geo_location.py
+-rw-r--r--   0        0        0      817 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ips_signature.py
+-rw-r--r--   0        0        0     1111 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ipv6_prefix.py
+-rw-r--r--   0        0        0      990 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_app.py
+-rw-r--r--   0        0        0      923 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_domain.py
+-rw-r--r--   0        0        0      714 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/mirror.py
+-rw-r--r--   0        0        0     1127 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/policer.py
+-rw-r--r--   0        0        0      771 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/port.py
+-rw-r--r--   0        0        0     3196 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/preferred_color_group.py
+-rw-r--r--   0        0        0     1055 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/prefix.py
+-rw-r--r--   0        0        0      723 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/protocol_name.py
+-rw-r--r--   0        0        0     1325 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/region.py
+-rw-r--r--   0        0        0      942 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/site.py
+-rw-r--r--   0        0        0     6864 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/sla.py
+-rw-r--r--   0        0        0      970 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/threat_grid_api_key.py
+-rw-r--r--   0        0        0      960 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/tloc.py
+-rw-r--r--   0        0        0     2111 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/trunkgroup.py
+-rw-r--r--   0        0        0      824 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/umbrella_data.py
+-rw-r--r--   0        0        0      856 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/url.py
+-rw-r--r--   0        0        0     1071 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/vpn.py
+-rw-r--r--   0        0        0     1405 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/list/zone.py
+-rw-r--r--   0        0        0     6204 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/localized.py
+-rw-r--r--   0        0        0     3752 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy.py
+-rw-r--r--   0        0        0    37132 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_definition.py
+-rw-r--r--   0        0        0     1557 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_list.py
+-rw-r--r--   0        0        0     9385 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/policy/security.py
+-rw-r--r--   0        0        0     2437 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/templates.py
+-rw-r--r--   0        0        0     5239 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/models/tenant.py
+-rw-r--r--   0        0        0     9717 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/response.py
+-rw-r--r--   0        0        0    19497 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/session.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/__init__.py
+-rw-r--r--   0        0        0     1236 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_converter_chooser.py
+-rw-r--r--   0        0        0      629 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/__init__.py
+-rw-r--r--   0        0        0     1710 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/dhcp.py
+-rw-r--r--   0        0        0    16810 2024-05-27 16:09:36.246934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/interface.py
+-rw-r--r--   0        0        0    11799 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/ospfv3.py
+-rw-r--r--   0        0        0     3185 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py
+-rw-r--r--   0        0        0     3583 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py
+-rw-r--r--   0        0        0     6139 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_merge_parcels.py
+-rw-r--r--   0        0        0     4782 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_normalizer.py
+-rw-r--r--   0        0        0    21196 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_transform.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/models/__init__.py
+-rw-r--r--   0        0        0      401 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/Basic_Cisco_VPN_Model.json
+-rw-r--r--   0        0        0      513 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/banner_1.json
+-rw-r--r--   0        0        0      116 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/alias.json
+-rw-r--r--   0        0        0      114 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/basic.json
+-rw-r--r--   0        0        0      109 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/basic_no_value.json
+-rw-r--r--   0        0        0      848 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children.json
+-rw-r--r--   0        0        0     2348 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json
+-rw-r--r--   0        0        0     2348 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      274 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/data_path.json
+-rw-r--r--   0        0        0     2973 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json
+-rw-r--r--   0        0        0    11100 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_aaa.json
+-rw-r--r--   0        0        0    41165 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json
+-rw-r--r--   0        0        0     5219 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json
+-rw-r--r--   0        0        0     5505 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/iuo.json
+-rw-r--r--   0        0        0      249 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_1.json
+-rw-r--r--   0        0        0      875 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_2.json
+-rw-r--r--   0        0        0     1682 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_3.json
+-rw-r--r--   0        0        0      662 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/__init__.py
+-rw-r--r--   0        0        0     2828 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_aaa.py
+-rw-r--r--   0        0        0      303 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_banner.py
+-rw-r--r--   0        0        0      587 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_bfd.py
+-rw-r--r--   0        0        0      344 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_system.py
+-rw-r--r--   0        0        0     8078 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_vpn.py
+-rw-r--r--   0        0        0     1091 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/omp_vsmart.py
+-rw-r--r--   0        0        0      605 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/alias.json
+-rw-r--r--   0        0        0      574 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/basic.json
+-rw-r--r--   0        0        0     1810 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children.json
+-rw-r--r--   0        0        0     4005 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json
+-rw-r--r--   0        0        0     4005 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json
+-rw-r--r--   0        0        0      731 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/data_path.json
+-rw-r--r--   0        0        0    43436 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json
+-rw-r--r--   0        0        0     1200 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_banner.json
+-rw-r--r--   0        0        0     9495 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json
+-rw-r--r--   0        0        0    99045 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_system.json
+-rw-r--r--   0        0        0    87854 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json
+-rw-r--r--   0        0        0     5939 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json
+-rw-r--r--   0        0        0     1381 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_chose_model.py
+-rw-r--r--   0        0        0     2598 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_deserialize_model.py
+-rw-r--r--   0        0        0     6762 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_find_template_values_2.py
+-rw-r--r--   0        0        0     4598 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_generate_payload.py
+-rw-r--r--   0        0        0     1755 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_serialize_model.py
+-rw-r--r--   0        0        0     8145 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_admin_tech_api.py
+-rw-r--r--   0        0        0    17792 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_administration.py
+-rw-r--r--   0        0        0    11116 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_alarms_api.py
+-rw-r--r--   0        0        0     8322 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_cli_template.py
+-rw-r--r--   0        0        0     5494 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_creation_tools.py
+-rw-r--r--   0        0        0     3981 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_device_action_api.py
+-rw-r--r--   0        0        0    28159 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_devices_api.py
+-rw-r--r--   0        0        0    34991 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1897 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_extended_community_converter.py
+-rw-r--r--   0        0        0    10767 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_profile_api.py
+-rw-r--r--   0        0        0      894 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_template_field.py
+-rw-r--r--   0        0        0     1545 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_logs_api.py
+-rw-r--r--   0        0        0     1007 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_mirror_converter.py
+-rw-r--r--   0        0        0     1899 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_models_common.py
+-rw-r--r--   0        0        0     1809 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_server_info.py
+-rw-r--r--   0        0        0     5489 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_status_api.py
+-rw-r--r--   0        0        0    11026 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_mtt_aaa_api.py
+-rw-r--r--   0        0        0    10026 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_normalize_to_model_definition.py
+-rw-r--r--   0        0        0    16472 2024-05-27 16:09:36.250934 catalystwan-0.33.7.dev2/catalystwan/tests/test_omp_api.py
+-rw-r--r--   0        0        0     5223 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_packet_capture.py
+-rw-r--r--   0        0        0     5727 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_partition_manager_api.py
+-rw-r--r--   0        0        0     7926 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_response.py
+-rw-r--r--   0        0        0     6724 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_session.py
+-rw-r--r--   0        0        0     7117 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_software_action_api.py
+-rw-r--r--   0        0        0     6071 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_speed_test_api.py
+-rw-r--r--   0        0        0    14926 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_task_status_api.py
+-rw-r--r--   0        0        0    15055 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_templates.py
+-rw-r--r--   0        0        0     3705 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_backup_restore_api.py
+-rw-r--r--   0        0        0     6114 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_management_api.py
+-rw-r--r--   0        0        0     4506 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_migration_api.py
+-rw-r--r--   0        0        0    12377 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_typed_list.py
+-rw-r--r--   0        0        0     2968 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_version.py
+-rw-r--r--   0        0        0    10377 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_version_utils.py
+-rw-r--r--   0        0        0     3343 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/tests/test_vmanage_auth.py
+-rw-r--r--   0        0        0     9379 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/typed_list.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/alarm_status.py
+-rw-r--r--   0        0        0      253 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/certificate_status.py
+-rw-r--r--   0        0        0      279 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/colors.py
+-rw-r--r--   0        0        0      239 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/exceptions.py
+-rw-r--r--   0        0        0      320 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/__init__.py
+-rw-r--r--   0        0        0     3433 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py
+-rw-r--r--   0        0        0     5810 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py
+-rw-r--r--   0        0        0      784 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py
+-rw-r--r--   0        0        0      268 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/base.py
+-rw-r--r--   0        0        0     3283 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py
+-rw-r--r--   0        0        0      898 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py
+-rw-r--r--   0        0        0     9266 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bgp.py
+-rw-r--r--   0        0        0     1765 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py
+-rw-r--r--   0        0        0     3269 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py
+-rw-r--r--   0        0        0      756 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cli.py
+-rw-r--r--   0        0        0     1932 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py
+-rw-r--r--   0        0        0     4566 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/dhcp.py
+-rw-r--r--   0        0        0     5349 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py
+-rw-r--r--   0        0        0     6334 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py
+-rw-r--r--   0        0        0      578 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py
+-rw-r--r--   0        0        0     1573 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/gps.py
+-rw-r--r--   0        0        0      331 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/helpers.py
+-rw-r--r--   0        0        0    13128 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py
+-rw-r--r--   0        0        0     5619 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py
+-rw-r--r--   0        0        0     5959 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py
+-rw-r--r--   0        0        0     9349 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py
+-rw-r--r--   0        0        0     7411 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py
+-rw-r--r--   0        0        0     1963 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py
+-rw-r--r--   0        0        0     4855 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py
+-rw-r--r--   0        0        0    13085 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py
+-rw-r--r--   0        0        0     5470 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py
+-rw-r--r--   0        0        0     2295 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py
+-rw-r--r--   0        0        0     1475 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py
+-rw-r--r--   0        0        0     5684 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py
+-rw-r--r--   0        0        0    11458 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py
+-rw-r--r--   0        0        0     6251 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py
+-rw-r--r--   0        0        0     1568 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py
+-rw-r--r--   0        0        0    10159 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/sig.py
+-rw-r--r--   0        0        0     2240 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py
+-rw-r--r--   0        0        0     9032 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py
+-rw-r--r--   0        0        0     2776 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py
+-rw-r--r--   0        0        0     2250 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py
+-rw-r--r--   0        0        0    31317 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py
+-rw-r--r--   0        0        0     5742 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py
+-rw-r--r--   0        0        0    13497 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py
+-rw-r--r--   0        0        0     4844 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py
+-rw-r--r--   0        0        0     6866 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py
+-rw-r--r--   0        0        0    14360 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py
+-rw-r--r--   0        0        0    18190 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py
+-rw-r--r--   0        0        0     5344 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py
+-rw-r--r--   0        0        0     8057 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py
+-rw-r--r--   0        0        0     7722 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_definitions.py
+-rw-r--r--   0        0        0    14226 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/policy/policy_lists.py
+-rw-r--r--   0        0        0      165 2024-05-27 16:09:36.254934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/utils.py
+-rw-r--r--   0        0        0    12777 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/config_pusher.py
+-rw-r--r--   0        0        0     8511 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/creators/strategy/parcels.py
+-rw-r--r--   0        0        0     1760 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py
+-rw-r--r--   0        0        0     1257 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py
+-rw-r--r--   0        0        0     3464 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/reverters/config_reverter.py
+-rw-r--r--   0        0        0        0 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/__init__.py
+-rw-r--r--   0        0        0     3767 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/constants.py
+-rw-r--r--   0        0        0     9821 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/transform.py
+-rw-r--r--   0        0        0      154 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/config_status.py
+-rw-r--r--   0        0        0     4778 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/creation_tools.py
+-rw-r--r--   0        0        0     7281 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/dashboard.py
+-rw-r--r--   0        0        0     2863 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/device_model.py
+-rw-r--r--   0        0        0     2110 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/dict.py
+-rw-r--r--   0        0        0      953 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/choose_model.py
+-rw-r--r--   0        0        0     4882 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/find_template_values.py
+-rw-r--r--   0        0        0     1173 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/model.py
+-rw-r--r--   0        0        0      584 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/operation_status.py
+-rw-r--r--   0        0        0      196 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/personality.py
+-rw-r--r--   0        0        0      360 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/pydantic_field.py
+-rw-r--r--   0        0        0      172 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/reachability.py
+-rw-r--r--   0        0        0      407 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/session_type.py
+-rw-r--r--   0        0        0      149 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/template_type.py
+-rw-r--r--   0        0        0     9825 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/timezone.py
+-rw-r--r--   0        0        0      449 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/type_check.py
+-rw-r--r--   0        0        0     3930 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/upgrades_helper.py
+-rw-r--r--   0        0        0      159 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/utils/validate_status.py
+-rw-r--r--   0        0        0     3032 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/version.py
+-rw-r--r--   0        0        0     5415 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/vmanage_auth.py
+-rw-r--r--   0        0        0    20653 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/workflows/config_migration.py
+-rw-r--r--   0        0        0     9946 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/catalystwan/workflows/tenant_migration.py
+-rw-r--r--   0        0        0      866 2024-05-27 16:09:36.258934 catalystwan-0.33.7.dev2/pyproject.toml
+-rw-r--r--   0        0        0    18941 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev2/setup.py
+-rw-r--r--   0        0        0    14665 1970-01-01 00:00:00.000000 catalystwan-0.33.7.dev2/PKG-INFO
```

### Comparing `catalystwan-0.33.7.dev1/LICENSE` & `catalystwan-0.33.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/README.md` & `catalystwan-0.33.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/abstractions.py` & `catalystwan-0.33.7.dev2/catalystwan/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/admin_tech_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/administration.py` & `catalystwan-0.33.7.dev2/catalystwan/api/administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/alarms_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/api_container.py` & `catalystwan-0.33.7.dev2/catalystwan/api/api_container.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/basic_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/basic_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/builder_factory.py` & `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/builder_factory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/cli.py` & `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/other.py` & `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/report.py` & `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/report.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 import functools
 from typing import Any, List, Optional, Tuple, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field
+from requests import Response
 
 from catalystwan.exceptions import ManagerErrorInfo, ManagerHTTPError
-from catalystwan.models.configuration.feature_profile.parcel import AnyParcel, ParcelType
-
-ParcelName = str
+from catalystwan.models.configuration.feature_profile.parcel import AnyParcel
 
 
 def handle_build_report(func):
     """Wrapper to make creating report simple and keep it DRY."""
 
     @functools.wraps(func)
     def wrapper(self, profile_uuid: UUID, parcel: AnyParcel, *args, **kwargs) -> Optional[UUID]:
@@ -33,43 +33,50 @@
 
 class FailedRequestDetails(BaseModel):
     method: str
     url: str
     headers: str
     body: str
 
+    @staticmethod
+    def from_response(response: Response):
+        request = response.request
+        FailedRequestDetails(
+            method=str(request.method), url=str(request.url), headers=str(request.headers), body=str(request.body)
+        )
+
 
 class FailedParcel(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
-    parcel_name: ParcelName = Field(serialization_alias="parcelName", validation_alias="parcelName")
-    parcel_type: ParcelType = Field(serialization_alias="parcelType", validation_alias="parcelType")
+    parcel_name: str = Field(serialization_alias="parcelName", validation_alias="parcelName")
+    parcel_type: str = Field(serialization_alias="parcelType", validation_alias="parcelType")
     error_info: Union[ManagerErrorInfo, str] = Field(serialization_alias="errorInfo", validation_alias="errorInfo")
     request_details: Optional[FailedRequestDetails] = Field(
         default=None, serialization_alias="failedRequest", validation_alias="failedRequest"
     )
 
 
 class FeatureProfileBuildReport(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     profile_name: str = Field(serialization_alias="profileName", validation_alias="profileName")
     profile_uuid: UUID = Field(serialization_alias="profileUuid", validation_alias="profileUuid")
-    created_parcels: List[Tuple[ParcelName, UUID]] = Field(
+    created_parcels: List[Tuple[str, UUID]] = Field(
         default_factory=list, serialization_alias="createdParcels", validation_alias="createdParcels"
     )
     failed_parcels: List[FailedParcel] = Field(
         default_factory=list, serialization_alias="failedParcels", validation_alias="failedParcels"
     )
 
-    def add_created_parcel(self, parcel_name: ParcelName, parcel_uuid: UUID) -> None:
+    def add_created_parcel(self, parcel_name: str, parcel_uuid: UUID) -> None:
         self.created_parcels.append((parcel_name, parcel_uuid))
 
     def add_failed_parcel(
         self,
-        parcel_name: ParcelName,
-        parcel_type: ParcelType,
+        parcel_name: str,
+        parcel_type: str,
         error_info: Union[ManagerErrorInfo, str],
         request: Optional[Any] = None,
     ) -> None:
         if request is not None:
             request = FailedRequestDetails(
                 method=str(request.method),
                 url=str(request.url),
@@ -78,7 +85,20 @@
             )
 
         self.failed_parcels.append(
             FailedParcel(
                 parcel_name=parcel_name, parcel_type=parcel_type, error_info=error_info, request_details=request
             )
         )
+
+
+def handle_build_report_for_failed_subparcel(
+    build_report: FeatureProfileBuildReport, parent: AnyParcel, subparcel: AnyParcel
+) -> None:
+    parent_failed_to_create_message = (
+        f"Parent parcel: {parent.parcel_name} failed to create. This subparcel is dependent on it."
+    )
+    build_report.add_failed_parcel(
+        parcel_name=subparcel.parcel_name,
+        parcel_type=subparcel._get_parcel_type(),
+        error_info=parent_failed_to_create_message,
+    )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/system.py` & `catalystwan-0.33.7.dev2/catalystwan/api/builders/feature_profiles/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/builders/feature_profiles/transport.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/profile_builder/test_pb_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,119 +1,78 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
-from __future__ import annotations
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
+from ipaddress import IPv4Address
 
-import logging
-from collections import defaultdict
-from typing import TYPE_CHECKING, Dict, List, Optional
-from uuid import UUID, uuid4
-
-from catalystwan.api.builders.feature_profiles.report import FeatureProfileBuildReport, handle_build_report
-from catalystwan.api.feature_profile_api import TransportFeatureProfileAPI
-from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
+from catalystwan.api.configuration_groups.parcel import Global, as_global, as_variable
+from catalystwan.integration_tests.profile_builder.base import TestFeatureProfileBuilder
+from catalystwan.integration_tests.test_data import bgp_parcel, ospf_parcel, ospfv3ipv4_parcel, ospfv3ipv6_parcel
+from catalystwan.models.common import SubnetMask
 from catalystwan.models.configuration.feature_profile.common import FeatureProfileCreationPayload
-from catalystwan.models.configuration.feature_profile.sdwan.transport import (
-    AnyTransportParcel,
-    AnyTransportSuperParcel,
-    AnyTransportVpnParcel,
-    AnyTransportVpnSubParcel,
+from catalystwan.models.configuration.feature_profile.sdwan.service.dhcp_server import (
+    AddressPool,
+    LanVpnDhcpServerParcel,
 )
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ethernet import InterfaceEthernetParcel
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import LanVpnParcel
 
-logger = logging.getLogger(__name__)
 
-if TYPE_CHECKING:
-    from catalystwan.session import ManagerSession
-
-
-class TransportAndManagementProfileBuilder:
-    """
-    A class for building system feature profiles.
-    """
-
-    def __init__(self, session: ManagerSession) -> None:
-        """
-        Initialize a new instance of the Service class.
-
-        Args:
-            session (ManagerSession): The ManagerSession object used for API communication.
-            profile_uuid (UUID): The UUID of the profile.
-        """
-        self._profile: FeatureProfileCreationPayload
-        self._api = TransportFeatureProfileAPI(session)
-        self._endpoints = TransportFeatureProfile(session)
-        self._independent_items: List[AnyTransportSuperParcel] = []
-        self._independent_items_vpns: Dict[UUID, AnyTransportVpnParcel] = {}
-        self._dependent_items_on_vpns: Dict[UUID, List[AnyTransportVpnSubParcel]] = defaultdict(list)
-
-    def add_profile_name_and_description(self, feature_profile: FeatureProfileCreationPayload) -> None:
-        """
-        Adds a name and description to the feature profile.
-
-        Args:
-            name (str): The name of the feature profile.
-            description (str): The description of the feature profile.
-
-        Returns:
-            None
-        """
-        self._profile = feature_profile
-
-    def add_parcel(self, parcel: AnyTransportSuperParcel) -> None:
-        """
-        Adds a parcel to the feature profile.
-
-        Args:
-            parcel (AnyTransportSuperParcel): The parcel to add.
-
-        Returns:
-            None
-        """
-        self._independent_items.append(parcel)
-
-    def add_parcel_vpn(self, parcel: AnyTransportVpnParcel) -> UUID:
-        """
-        Adds a VPN parcel to the builder.
-
-        Args:
-            parcel (LanVpnParcel): The VPN parcel to add.
-
-        Returns:
-            UUID: The UUID tag of the added VPN parcel.
-        """
-        vpn_tag = uuid4()
-        logger.debug(f"Adding VPN parcel {parcel.parcel_name} with tag {vpn_tag}")
-        self._independent_items_vpns[vpn_tag] = parcel
-        return vpn_tag
-
-    def add_vpn_subparcel(self, parcel: AnyTransportVpnSubParcel, vpn_tag: UUID) -> None:
-        """
-        Adds a parcel to the feature profile.
-
-        Args:
-            parcel (AnyTransportVpnSubParcel): The parcel to add.
-
-        Returns:
-            None
-        """
-        self._dependent_items_on_vpns[vpn_tag].append(parcel)
-
-    def build(self) -> FeatureProfileBuildReport:
-        """
-        Builds the feature profile.
-
-        Returns:
-            UUID: The UUID of the created feature profile.
-        """
-
-        profile_uuid = self._endpoints.create_transport_feature_profile(self._profile).id
-        self.build_report = FeatureProfileBuildReport(profile_uuid=profile_uuid, profile_name=self._profile.name)
-        for parcel in self._independent_items:
-            self._create_parcel(profile_uuid, parcel)
-        for vpn_tag, vpn_parcel in self._independent_items_vpns.items():
-            # TODO: Add subparcels to VPN
-            vpn_uuid = self._create_parcel(profile_uuid, vpn_parcel)
-            for subparcel in self._dependent_items_on_vpns[vpn_tag]:
-                self._create_parcel(profile_uuid, subparcel, vpn_uuid)
-        return self.build_report
-
-    @handle_build_report
-    def _create_parcel(self, profile_uuid: UUID, parcel: AnyTransportParcel, vpn_uuid: Optional[None] = None) -> UUID:
-        return self._api.create_parcel(profile_uuid, parcel, vpn_uuid).id
+class TestServiceFeatureProfileBuilder(TestFeatureProfileBuilder):
+    def setUp(self) -> None:
+        self.fp_name = "FeatureProfileBuilderService"
+        self.fp_description = "Transport feature profile"
+        self.builder = self.session.api.builders.feature_profiles.create_builder("service")
+        self.builder.add_profile_name_and_description(
+            feature_profile=FeatureProfileCreationPayload(name=self.fp_name, description=self.fp_description)
+        )
+        self.api = self.session.api.sdwan_feature_profiles.service
+
+    def test_when_build_profile_with_vpn_and_interface_with_dhcp_expect_success(self):
+        # Arrange
+        service_vpn_parcel = LanVpnParcel(
+            parcel_name="MinimumSpecifiedTransportVpnParcel",
+            description="Description",
+            vpn_id=as_global(50),
+        )
+        ethernet_parcel = InterfaceEthernetParcel(
+            parcel_name="TestEthernetParcel",
+            parcel_description="Test Ethernet Parcel",
+            interface_name=as_global("HundredGigE"),
+            ethernet_description=as_global("Test Ethernet Description"),
+            shutdown=as_variable("{{vpn1_gi3_lan_ip_192.168.X.1/24_}}"),
+        )
+        dhcp_server_parcel = LanVpnDhcpServerParcel(
+            parcel_name="DhcpServerDefault",
+            parcel_description="Dhcp Server Parcel",
+            address_pool=AddressPool(
+                network_address=Global[IPv4Address](value=IPv4Address("10.0.0.2")),
+                subnet_mask=Global[SubnetMask](value="255.255.255.255"),
+            ),
+        )
+        vpn_tag = self.builder.add_parcel_vpn(service_vpn_parcel)
+        self.builder.add_parcel_vpn_subparcel(vpn_tag, ethernet_parcel)
+        self.builder.add_parcel_dhcp_server(ethernet_parcel.parcel_name, dhcp_server_parcel)
+        # Act
+        report = self.builder.build()
+        # Assert
+        assert len(report.failed_parcels) == 0
+
+    def test_when_build_profile_with_vpn_and_routing_attached_expect_success(self):
+        # Arrange
+        service_vpn_parcel = LanVpnParcel(
+            parcel_name="MinimumSpecifiedServiceVpnParcel",
+            description="Description",
+            vpn_id=as_global(50),
+        )
+        vpn_tag = self.builder.add_parcel_vpn(service_vpn_parcel)
+        self.builder.add_parcel_routing_attached(vpn_tag, ospf_parcel)
+        self.builder.add_parcel_routing_attached(vpn_tag, ospfv3ipv4_parcel)
+        self.builder.add_parcel_routing_attached(vpn_tag, ospfv3ipv6_parcel)
+        self.builder.add_parcel_routing_attached(vpn_tag, bgp_parcel)
+        # Act
+        report = self.builder.build()
+        # Assert
+        assert len(report.failed_parcels) == 0
+
+    def tearDown(self) -> None:
+        target_profile = self.api.get_profiles().filter(profile_name=self.fp_name).single_or_default()
+        if target_profile:
+            # In case of a failed test, the profile might not have been created
+            self.api.delete_profile(target_profile.profile_id)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/config_device_inventory_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/config_device_inventory_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/config_group_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/config_group_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/configuration_groups/parcel.py` & `catalystwan-0.33.7.dev2/catalystwan/api/configuration_groups/parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/dashboard_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/dashboard_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/device_action_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/feature_profile_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/feature_profile_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,30 +11,51 @@
 from catalystwan.endpoints.configuration.feature_profile.sdwan.other import OtherFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.service import ServiceFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.sig_security import SIGSecurity
 from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.topology import TopologyFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
 from catalystwan.exceptions import ManagerHTTPError
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv4acl import Ipv4AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv6acl import Ipv6AclParcel
 from catalystwan.models.configuration.feature_profile.sdwan.application_priority import (
     AnyApplicationPriorityParcel,
     PolicySettingsParcel,
     QosPolicyParcel,
+    TrafficPolicyParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.other import AnyOtherParcel
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy.as_path import AsPathParcel
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy.mirror import MirrorParcel
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy.sla_class import SLAClassParcel
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.aip import (
+    AdvancedInspectionProfileParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.amp import (
+    AdvancedMalwareProtectionParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.intrusion_prevention import (
+    IntrusionPreventionParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.ssl_decryption import (
+    SslDecryptionParcel,
+)
+from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.ssl_decryption_profile import (
+    SslDecryptionProfileParcel,
+)
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object.security.url import URLParcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing import AnyRoutingParcel, RoutingBgpParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service import AnyServiceParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.multicast import MulticastParcel
 from catalystwan.models.configuration.feature_profile.sdwan.sig_security.sig_security import SIGParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology import AnyTopologyParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.custom_control import CustomControlParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.hubspoke import HubSpokeParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology.mesh import MeshParcel
 from catalystwan.models.configuration.feature_profile.sdwan.transport import AnyTransportParcel
-from catalystwan.models.configuration.feature_profile.sdwan.transport.bgp import WanRoutingBgpParcel
 from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import (
     CellularControllerParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.t1e1controller import T1E1ControllerParcel
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import ManagementVpnParcel, TransportVpnParcel
 from catalystwan.typed_list import DataSequence
 
@@ -71,14 +92,15 @@
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import (
     AnyPolicyObjectParcel,
     ApplicationListParcel,
     AppProbeParcel,
     ColorParcel,
     DataPrefixParcel,
     ExpandedCommunityParcel,
+    ExtendedCommunityParcel,
     FowardingClassParcel,
     FQDNDomainParcel,
     GeoLocationListParcel,
     IPSSignatureParcel,
     IPv6DataPrefixParcel,
     IPv6PrefixListParcel,
     LocalDomainParcel,
@@ -248,31 +270,41 @@
     def get_parcel(
         self, profile_id: UUID, parcel_type: Type[T1E1ControllerParcel], parcel_id: UUID
     ) -> Parcel[T1E1ControllerParcel]:
         ...
 
     @overload
     def get_parcel(
-        self, profile_id: UUID, parcel_type: Type[WanRoutingBgpParcel], parcel_id: UUID
-    ) -> Parcel[WanRoutingBgpParcel]:
+        self, profile_id: UUID, parcel_type: Type[RoutingBgpParcel], parcel_id: UUID
+    ) -> Parcel[RoutingBgpParcel]:
         ...
 
     @overload
     def get_parcel(
         self, profile_id: UUID, parcel_type: Type[TransportVpnParcel], parcel_id: UUID
     ) -> Parcel[TransportVpnParcel]:
         ...
 
     @overload
     def get_parcel(
         self, profile_id: UUID, parcel_type: Type[ManagementVpnParcel], parcel_id: UUID
     ) -> Parcel[ManagementVpnParcel]:
         ...
 
-    def get_parcel(self, profile_id: UUID, parcel_type: Type[AnyTransportParcel], parcel_id: UUID) -> Parcel:
+    @overload
+    def get_parcel(self, profile_id: UUID, parcel_type: Type[Ipv4AclParcel], parcel_id: UUID) -> Parcel[Ipv4AclParcel]:
+        ...
+
+    @overload
+    def get_parcel(self, profile_id: UUID, parcel_type: Type[Ipv6AclParcel], parcel_id: UUID) -> Parcel[Ipv6AclParcel]:
+        ...
+
+    def get_parcel(
+        self, profile_id: UUID, parcel_type: Type[Union[AnyTransportParcel, AnyRoutingParcel]], parcel_id: UUID
+    ) -> Parcel:
         """
         Get one Transport Parcel given profile id, parcel type and parcel id
         """
         return self.endpoint.get_transport_parcel(profile_id, parcel_type._get_parcel_type(), parcel_id)
 
 
 class OtherFeatureProfileAPI:
@@ -774,357 +806,379 @@
     SDWAN Feature Profile Policy Object APIs
     """
 
     def __init__(self, session: ManagerSession):
         self.session = session
         self.endpoint = PolicyObjectFeatureProfile(session)
 
+    def get_profiles(self) -> DataSequence[FeatureProfileInfo]:
+        return self.endpoint.get_profiles()
+
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[ApplicationListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[AdvancedInspectionProfileParcel]
+    ) -> DataSequence[Parcel[AdvancedInspectionProfileParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[AppProbeParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[AdvancedMalwareProtectionParcel]
+    ) -> DataSequence[Parcel[AdvancedMalwareProtectionParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[ColorParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[ApplicationListParcel]
+    ) -> DataSequence[Parcel[ApplicationListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[DataPrefixParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[AppProbeParcel]) -> DataSequence[Parcel[AppProbeParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[ExpandedCommunityParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[AsPathParcel]) -> DataSequence[Parcel[AsPathParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[FowardingClassParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[ColorParcel]) -> DataSequence[Parcel[ColorParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[FQDNDomainParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[DataPrefixParcel]) -> DataSequence[Parcel[DataPrefixParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[GeoLocationListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[ExpandedCommunityParcel]
+    ) -> DataSequence[Parcel[ExpandedCommunityParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[IPSSignatureParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[FowardingClassParcel]
+    ) -> DataSequence[Parcel[FowardingClassParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[IPv6DataPrefixParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[FQDNDomainParcel]) -> DataSequence[Parcel[FQDNDomainParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[IPv6PrefixListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[GeoLocationListParcel]
+    ) -> DataSequence[Parcel[GeoLocationListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[IntrusionPreventionParcel]
+    ) -> DataSequence[Parcel[IntrusionPreventionParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[IPSSignatureParcel]) -> DataSequence[Parcel[IPSSignatureParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[IPv6DataPrefixParcel]
+    ) -> DataSequence[Parcel[IPv6DataPrefixParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PrefixListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[IPv6PrefixListParcel]
+    ) -> DataSequence[Parcel[IPv6PrefixListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[ProtocolListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel]) -> DataSequence[Parcel[LocalDomainParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[SecurityApplicationListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[MirrorParcel]) -> DataSequence[Parcel[MirrorParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[SecurityDataPrefixParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel]) -> DataSequence[Parcel[PolicerParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[SecurityPortParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel]
+    ) -> DataSequence[Parcel[PreferredColorGroupParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[SecurityZoneListParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[PrefixListParcel]) -> DataSequence[Parcel[PrefixListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[StandardCommunityParcel]) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[ProtocolListParcel]) -> DataSequence[Parcel[ProtocolListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[TlocParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityApplicationListParcel]
+    ) -> DataSequence[Parcel[SecurityApplicationListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[URLParcel]) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityDataPrefixParcel]
+    ) -> DataSequence[Parcel[SecurityDataPrefixParcel]]:
         ...
 
-    # get by id
-
     @overload
-    def get(
-        self, profile_id: UUID, parcel_type: Type[ApplicationListParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[SecurityPortParcel]) -> DataSequence[Parcel[SecurityPortParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[AppProbeParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityZoneListParcel]
+    ) -> DataSequence[Parcel[SecurityZoneListParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[ColorParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[SLAClassParcel]) -> DataSequence[Parcel[SLAClassParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[DataPrefixParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SslDecryptionParcel]
+    ) -> DataSequence[Parcel[SslDecryptionParcel]]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[ExpandedCommunityParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[SslDecryptionProfileParcel]
+    ) -> DataSequence[Parcel[SslDecryptionProfileParcel]]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[FowardingClassParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[StandardCommunityParcel]
+    ) -> DataSequence[Parcel[StandardCommunityParcel]]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[FQDNDomainParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[TlocParcel]) -> DataSequence[Parcel[TlocParcel]]:
         ...
 
     @overload
-    def get(
-        self, profile_id: UUID, parcel_type: Type[GeoLocationListParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[URLParcel]) -> DataSequence[Parcel[TlocParcel]]:
         ...
 
+    # get by id
+
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[IPSSignatureParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[AdvancedInspectionProfileParcel], parcel_id: UUID
+    ) -> Parcel[AdvancedInspectionProfileParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[IPv6DataPrefixParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[AdvancedMalwareProtectionParcel], parcel_id: UUID
+    ) -> Parcel[AdvancedMalwareProtectionParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[IPv6PrefixListParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[ApplicationListParcel], parcel_id: UUID
+    ) -> Parcel[ApplicationListParcel]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[AppProbeParcel], parcel_id: UUID) -> Parcel[AppProbeParcel]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[AsPathParcel], parcel_id: UUID) -> Parcel[AsPathParcel]:
         ...
 
     @overload
-    def get(
-        self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[ColorParcel], parcel_id: UUID) -> Parcel[ColorParcel]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[PrefixListParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[DataPrefixParcel], parcel_id: UUID) -> Parcel[DataPrefixParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[ProtocolListParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[ExpandedCommunityParcel], parcel_id: UUID
+    ) -> Parcel[ExpandedCommunityParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[SecurityApplicationListParcel], parcel_id: UUID
+        self, profile_id: UUID, parcel_type: Type[ExtendedCommunityParcel], parcel_id: UUID
     ) -> DataSequence[Parcel[Any]]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[SecurityDataPrefixParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[FowardingClassParcel], parcel_id: UUID
+    ) -> Parcel[FowardingClassParcel]:
         ...
 
     @overload
-    def get(
-        self, profile_id: UUID, parcel_type: Type[SecurityPortParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+    def get(self, profile_id: UUID, parcel_type: Type[FQDNDomainParcel], parcel_id: UUID) -> Parcel[FQDNDomainParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[SecurityZoneListParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[GeoLocationListParcel], parcel_id: UUID
+    ) -> Parcel[GeoLocationListParcel]:
         ...
 
     @overload
     def get(
-        self, profile_id: UUID, parcel_type: Type[StandardCommunityParcel], parcel_id: UUID
-    ) -> DataSequence[Parcel[Any]]:
+        self, profile_id: UUID, parcel_type: Type[IntrusionPreventionParcel], parcel_id: UUID
+    ) -> Parcel[IntrusionPreventionParcel]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[TlocParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[IPSSignatureParcel], parcel_id: UUID
+    ) -> Parcel[IPSSignatureParcel]:
         ...
 
     @overload
-    def get(self, profile_id: UUID, parcel_type: Type[URLParcel], parcel_id: UUID) -> DataSequence[Parcel[Any]]:
-        ...
-
     def get(
-        self,
-        profile_id: UUID,
-        parcel_type: Type[AnyPolicyObjectParcel],
-        parcel_id: Union[UUID, None] = None,
-    ) -> DataSequence[Parcel[Any]]:
-        """
-        Get all Policy Objects for selected profile_id and selected type or get one Policy Object given parcel id
-        """
-
-        policy_object_list_type = parcel_type._get_parcel_type()
-        if not parcel_id:
-            return self.endpoint.get_all(profile_id=profile_id, policy_object_list_type=policy_object_list_type)
-        parcel = self.endpoint.get_by_id(
-            profile_id=profile_id, policy_object_list_type=policy_object_list_type, list_object_id=parcel_id
-        )
-        return DataSequence(Parcel, [parcel])
-
-    def create(self, profile_id: UUID, payload: AnyPolicyObjectParcel) -> ParcelCreationResponse:
-        """
-        Create Policy Object for selected profile_id based on payload type
-        """
-
-        policy_object_list_type = payload._get_parcel_type()
-        return self.endpoint.create(
-            profile_id=profile_id, policy_object_list_type=policy_object_list_type, payload=payload
-        )
-
-    def update(self, profile_id: UUID, payload: AnyPolicyObjectParcel, list_object_id: UUID):
-        """
-        Update Policy Object for selected profile_id based on payload type
-        """
-
-        policy_type = payload._get_parcel_type()
-        return self.endpoint.update(
-            profile_id=profile_id, policy_object_list_type=policy_type, list_object_id=list_object_id, payload=payload
-        )
-
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[ApplicationListParcel], list_object_id: UUID) -> None:
+        self, profile_id: UUID, parcel_type: Type[IPv6DataPrefixParcel], parcel_id: UUID
+    ) -> Parcel[IPv6DataPrefixParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[AppProbeParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[IPv6PrefixListParcel], parcel_id: UUID
+    ) -> Parcel[IPv6PrefixListParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[ColorParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel], parcel_id: UUID) -> Parcel[LocalDomainParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[DataPrefixParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[MirrorParcel], parcel_id: UUID) -> Parcel[MirrorParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[ExpandedCommunityParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[PolicerParcel], parcel_id: UUID) -> Parcel[PolicerParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[FowardingClassParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel], parcel_id: UUID
+    ) -> Parcel[PreferredColorGroupParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[FQDNDomainParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[PrefixListParcel], parcel_id: UUID) -> Parcel[PrefixListParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[GeoLocationListParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[ProtocolListParcel], parcel_id: UUID
+    ) -> Parcel[ProtocolListParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[IPSSignatureParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityApplicationListParcel], parcel_id: UUID
+    ) -> Parcel[SecurityApplicationListParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[IPv6DataPrefixParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityDataPrefixParcel], parcel_id: UUID
+    ) -> Parcel[SecurityDataPrefixParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[IPv6PrefixListParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityPortParcel], parcel_id: UUID
+    ) -> Parcel[SecurityPortParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[LocalDomainParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SecurityZoneListParcel], parcel_id: UUID
+    ) -> Parcel[SecurityZoneListParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[PolicerParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[SLAClassParcel], parcel_id: UUID) -> Parcel[SLAClassParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[PreferredColorGroupParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SslDecryptionParcel], parcel_id: UUID
+    ) -> Parcel[SslDecryptionParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[PrefixListParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[SslDecryptionProfileParcel], parcel_id: UUID
+    ) -> Parcel[SslDecryptionProfileParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[ProtocolListParcel], list_object_id: UUID) -> None:
+    def get(
+        self, profile_id: UUID, parcel_type: Type[StandardCommunityParcel], parcel_id: UUID
+    ) -> Parcel[StandardCommunityParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[SecurityApplicationListParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[TlocParcel], parcel_id: UUID) -> Parcel[TlocParcel]:
         ...
 
     @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[SecurityDataPrefixParcel], list_object_id: UUID) -> None:
+    def get(self, profile_id: UUID, parcel_type: Type[URLParcel], parcel_id: UUID) -> Parcel[TlocParcel]:
         ...
 
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[SecurityPortParcel], list_object_id: UUID) -> None:
-        ...
+    def get(
+        self,
+        profile_id: UUID,
+        parcel_type: Type[AnyPolicyObjectParcel],
+        parcel_id: Union[UUID, None] = None,
+    ) -> Any:
+        """
+        Get all Policy Objects for selected profile_id and selected type or get one Policy Object given parcel id
+        """
 
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[SecurityZoneListParcel], list_object_id: UUID) -> None:
-        ...
+        policy_object_list_type = parcel_type._get_parcel_type()
+        if parcel_id is None:
+            return self.endpoint.get_all(profile_id=profile_id, policy_object_list_type=policy_object_list_type)
+        return self.endpoint.get_by_id(
+            profile_id=profile_id, policy_object_list_type=policy_object_list_type, list_object_id=parcel_id
+        )
 
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[StandardCommunityParcel], list_object_id: UUID) -> None:
-        ...
+    def create(self, profile_id: UUID, payload: AnyPolicyObjectParcel) -> ParcelCreationResponse:
+        """
+        Create Policy Object for selected profile_id based on payload type
+        """
 
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[TlocParcel], list_object_id: UUID) -> None:
-        ...
+        policy_object_list_type = payload._get_parcel_type()
+        return self.endpoint.create(
+            profile_id=profile_id, policy_object_list_type=policy_object_list_type, payload=payload
+        )
 
-    @overload
-    def delete(self, profile_id: UUID, parcel_type: Type[URLParcel], list_object_id: UUID) -> None:
-        ...
+    def update(self, profile_id: UUID, payload: AnyPolicyObjectParcel, list_object_id: UUID):
+        """
+        Update Policy Object for selected profile_id based on payload type
+        """
+
+        policy_type = payload._get_parcel_type()
+        return self.endpoint.update(
+            profile_id=profile_id, policy_object_list_type=policy_type, list_object_id=list_object_id, payload=payload
+        )
 
     def delete(self, profile_id: UUID, parcel_type: Type[AnyPolicyObjectParcel], list_object_id: UUID) -> None:
         """
         Delete Policy Object for selected profile_id based on payload type
         """
 
         policy_object_list_type = parcel_type._get_parcel_type()
@@ -1461,14 +1515,22 @@
     def get_parcels(
         self,
         profile_id: UUID,
         parcel_type: Type[PolicySettingsParcel],
     ) -> DataSequence[Parcel[PolicySettingsParcel]]:
         ...
 
+    @overload
+    def get_parcels(
+        self,
+        profile_id: UUID,
+        parcel_type: Type[TrafficPolicyParcel],
+    ) -> DataSequence[Parcel[TrafficPolicyParcel]]:
+        ...
+
     def get_parcels(
         self,
         profile_id: UUID,
         parcel_type: Type[AnyApplicationPriorityParcel],
     ) -> DataSequence:
         """
         Get all Application Priority Parcels given profile id and parcel type
@@ -1484,14 +1546,23 @@
     ) -> Parcel[PolicySettingsParcel]:
         ...
 
     @overload
     def get_parcel(
         self,
         profile_id: UUID,
+        parcel_type: Type[TrafficPolicyParcel],
+        parcel_id: UUID,
+    ) -> Parcel[TrafficPolicyParcel]:
+        ...
+
+    @overload
+    def get_parcel(
+        self,
+        profile_id: UUID,
         parcel_type: Type[QosPolicyParcel],
         parcel_id: UUID,
     ) -> Parcel[QosPolicyParcel]:
         ...
 
     def get_parcel(
         self,
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/logs_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/monitoring_status_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/mtt_aaa_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/omp_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/packet_capture_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/packet_capture_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/parcel_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/parcel_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/partition_manager_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/policy_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/policy_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/resource_pool_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/resource_pool_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/software_action_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/speedtest_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/speedtest_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/task_status_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/template_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/template_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/README.md` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/cli_template.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/device_template/device_template.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/device_template/device_template_payload.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/device_template/device_template_payload.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template_field.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/feature_template_payload.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/feature_template_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_aaa_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_banner_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_banner_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_bfd_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bfd_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_bgp_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_bgp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_logging_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_logging_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ntp_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ntp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_omp_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_omp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ospf.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_ospfv3.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_ospfv3.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_secure_internet_gateway.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_secure_internet_gateway.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_snmp_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_snmp_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_system.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_vpn_interface_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_interface_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/cisco_vpn_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/omp_vsmart_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/omp_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/security_vsmart_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/security_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/supported.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/supported.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/models/system_vsmart_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/models/system_vsmart_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/aaa_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/aaa_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/aaa.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/accounting.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/radius.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/tacacs.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/aaa/feature/user.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/aaa/feature/user.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/cisco_vpn_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/cisco_vpn.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/dns.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv4route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/ipv6route.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/cisco_vpn/feature/mapping.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/tenant/tenant.json.j2` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant.json.j2`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/templates/payloads/tenant/tenant_model.py` & `catalystwan-0.33.7.dev2/catalystwan/api/templates/payloads/tenant/tenant_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/tenant_management_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/tenant_migration_api.py` & `catalystwan-0.33.7.dev2/catalystwan/api/tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/api/versions_utils.py` & `catalystwan-0.33.7.dev2/catalystwan/api/versions_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/dataclasses.py` & `catalystwan-0.33.7.dev2/catalystwan/dataclasses.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,29 +48,29 @@
     Literal,
     Mapping,
     Optional,
     Protocol,
     Sequence,
     Set,
     Tuple,
-    Type,
     TypeVar,
     Union,
     runtime_checkable,
 )
 from uuid import UUID
 
 from packaging.specifiers import SpecifierSet  # type: ignore
 from packaging.version import Version  # type: ignore
 from pydantic import BaseModel
-from typing_extensions import Annotated, get_args, get_origin
+from typing_extensions import get_args, get_origin
 
 from catalystwan.abstractions import APIEndpointClient, APIEndpointClientResponse
 from catalystwan.exceptions import APIEndpointError, APIRequestPayloadTypeError, APIVersionError, APIViewError
 from catalystwan.typed_list import DataSequence
+from catalystwan.utils.model import resolve_nested_base_model_unions
 from catalystwan.utils.session_type import SessionType
 
 BASE_PATH: Final[str] = "/dataservice"
 T = TypeVar("T")
 logger = logging.getLogger(__name__)
 
 
@@ -111,51 +111,25 @@
         return TypeSpecifier(present=True, is_json=True)
 
     @classmethod
     def model_union(cls, models: Sequence[type]) -> TypeSpecifier:
         return TypeSpecifier(present=True, payload_union_model_types=models)
 
     @classmethod
-    def resolve_nested_base_model_unions(
-        cls, annotation: Any, models_types: List[Type[BaseModel]]
-    ) -> List[Type[BaseModel]]:
-        type_origin = get_origin(annotation)
-        if isclass(annotation):
-            try:
-                if issubclass(annotation, BaseModel):
-                    return [annotation]
-                raise APIEndpointError(f"Expected: {PayloadType}")
-            except TypeError:
-                raise APIEndpointError(f"Expected: {PayloadType}")
-        # Check if Annnotated[Union[PayloadModelType, ...]], only unions of pydantic models allowed
-        elif type_origin == Annotated:
-            if annotated_origin := get_args(annotation):
-                if (len(annotated_origin) >= 1) and get_origin(annotated_origin[0]) == Union:
-                    type_args = get_args(annotated_origin[0])
-                    if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
-                        models_types.extend(list(type_args))
-                        return models_types
-                    else:
-                        non_models = [t for t in type_args if not isclass(t)]
-                        for non_model in non_models:
-                            models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
-                        return models_types
+    def resolve_nested(cls, annotation: Any, models_types: List[type]) -> List[type]:
+        try:
+            return resolve_nested_base_model_unions(annotation)
+        except TypeError:
+            raise APIEndpointError(f"Expected: {PayloadType}")
 
-        # Check if Union[PayloadModelType, ...], only unions of pydantic models allowed
-        elif type_origin == Union:
-            type_args = get_args(annotation)
-            if all(isclass(t) for t in type_args) and all(issubclass(t, BaseModel) for t in type_args):
-                models_types.extend(list(type_args))
-                return models_types
-            else:
-                non_models = [t for t in type_args if not isclass(t)]
-                for non_model in non_models:
-                    models_types.extend(cls.resolve_nested_base_model_unions(non_model, models_types))
-                return models_types
-        raise APIEndpointError(f"Expected: {PayloadType}")
+    @property
+    def payload_model_set(self) -> Optional[Set[type]]:
+        if self.payload_union_model_types is not None:
+            return set(self.payload_union_model_types)
+        return None
 
 
 @dataclass
 class APIEndpointRequestMeta:
     """Holds data for endpoints exctracted during decorating. Used for documentation"""
 
     func: Any
@@ -482,15 +456,15 @@
                     (type_args := get_args(annotation))
                     and (len(type_args) == 1)
                     and isclass(type_args[0])
                     and issubclass(type_args[0], BaseModel)
                 ):
                     return TypeSpecifier(True, type_origin, type_args[0], None, False, is_optional)
             else:
-                models = TypeSpecifier.resolve_nested_base_model_unions(annotation, [])
+                models = TypeSpecifier.resolve_nested(annotation, [])
                 return TypeSpecifier.model_union(models)
         raise APIEndpointError(f"'payload' param must be annotated with supported type: {PayloadType}")
 
     def check_params(self):
         """Checks params in decorated method definition
 
         Raises:
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/administration_user_and_group.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/administration_user_and_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/certificate_management_device.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_device.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/certificate_management_vmanage.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/certificate_management_vmanage.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/client.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/cluster_management.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/cluster_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/device/software_update.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/device/software_update.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/disaster_recovery.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/disaster_recovery.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/application_priority.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,81 +14,81 @@
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.application_priority import AnyApplicationPriorityParcel
 from catalystwan.typed_list import DataSequence
 
 
 class ApplicationPriorityFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/application-priority")
     def create_application_priority_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/application-priority")
     def get_application_priority_feature_profiles(
         self, params: GetFeatureProfilesPayload
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/application-priority/{profile_id}")
     def get_application_priority_feature_profile(
         self, profile_id: str, params: GetFeatureProfilesPayload
     ) -> FeatureProfileDetail:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/application-priority/{profile_id}")
     def edit_application_priority_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/application-priority/{profile_id}")
     def delete_application_priority_feature_profile(self, profile_id: str) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/application-priority/{profile_id}/{application_priority_list_type}")
     def create(
         self, profile_id: UUID, application_priority_list_type: str, payload: AnyApplicationPriorityParcel
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete(
         "/v1/feature-profile/sdwan/application-priority/{profile_id}/{application_priority_list_type}/{list_object_id}"
     )
     def delete(self, profile_id: UUID, application_priority_list_type: str, list_object_id: UUID) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put(
         "/v1/feature-profile/sdwan/application-priority/{profile_id}/{application_priority_list_type}/{list_object_id}"
     )
     def update(
         self,
         profile_id: UUID,
         application_priority_list_type: str,
         list_object_id: UUID,
         payload: AnyApplicationPriorityParcel,
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get(
         "/v1/feature-profile/sdwan/application-priority/{profile_id}/{application_priority_list_type}/{list_object_id}"
     )
     def get_by_id(self, profile_id: UUID, application_priority_list_type: str, list_object_id: UUID) -> Parcel:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get(
         "/v1/feature-profile/sdwan/application-priority/{profile_id}/{application_priority_list_type}",
         resp_json_key="data",
     )
     def get_all(self, profile_id: UUID, application_priority_list_type: str) -> DataSequence[Parcel]:
         ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/dns_security.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,70 +14,70 @@
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.dns_security import AnyDnsSecurityParcel
 from catalystwan.typed_list import DataSequence
 
 
 class DnsSecurityFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/dns-security")
     def create_dns_security_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security")
     def get_dns_security_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security/{profile_id}")
     def get_dns_security_feature_profile(
         self, profile_id: str, params: GetFeatureProfilesPayload
     ) -> FeatureProfileDetail:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/dns-security/{profile_id}")
     def edit_dns_security_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/dns-security/{profile_id}")
     def delete_dns_security_feature_profile(self, profile_id: str) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/dns-security/{profile_id}/{dns_security_list_type}")
     def create(
         self, profile_id: UUID, dns_security_list_type: str, payload: AnyDnsSecurityParcel
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/dns-security/{profile_id}/{dns_security_list_type}/{list_object_id}")
     def delete(self, profile_id: UUID, dns_security_list_type: str, list_object_id: UUID) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/dns-security/{profile_id}/{dns_security_list_type}/{list_object_id}")
     def update(
         self,
         profile_id: UUID,
         dns_security_list_type: str,
         list_object_id: UUID,
         payload: AnyDnsSecurityParcel,
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security/{profile_id}/{dns_security_list_type}/{list_object_id}")
     def get_by_id(self, profile_id: UUID, dns_security_list_type: str, list_object_id: UUID) -> Parcel:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/dns-security/{profile_id}/{dns_security_list_type}", resp_json_key="data")
     def get_all(self, profile_id: UUID, dns_security_list_type: str) -> DataSequence[Parcel]:
         ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/embedded_security.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,72 +17,72 @@
     AnyEmbeddedSecurityParcel,
     PolicyParcel,
 )
 from catalystwan.typed_list import DataSequence
 
 
 class EmbeddedSecurityFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/embedded-security")
     def create_embedded_security_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security")
     def get_embedded_security_feature_profiles(
         self, params: GetFeatureProfilesPayload
     ) -> DataSequence[FeatureProfileInfo]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security/{profile_id}")
     def get_embedded_security_feature_profile(
         self, profile_id: str, params: GetFeatureProfilesPayload
     ) -> FeatureProfileDetail:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/embedded-security/{profile_id}")
     def edit_embedded_security_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/embedded-security/{profile_id}")
     def delete_embedded_security_feature_profile(self, profile_id: str) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/embedded-security/{profile_id}/{embedded_security_list_type}")
     def create(
         self, profile_id: UUID, embedded_security_list_type: str, payload: PolicyParcel
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/embedded-security/{profile_id}/{embedded_security_list_type}/{list_object_id}")
     def delete(self, profile_id: UUID, embedded_security_list_type: str, list_object_id: UUID) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/embedded-security/{profile_id}/{embedded_security_list_type}/{list_object_id}")
     def update(
         self,
         profile_id: UUID,
         embedded_security_list_type: str,
         list_object_id: UUID,
         payload: AnyEmbeddedSecurityParcel,
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security/{profile_id}/{embedded_security_list_type}/{list_object_id}")
     def get_by_id(self, profile_id: UUID, embedded_security_list_type: str, list_object_id: UUID) -> Parcel:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/embedded-security/{profile_id}/{embedded_security_list_type}", resp_json_key="data")
     def get_all(self, profile_id: UUID, embedded_security_list_type: str) -> DataSequence[Parcel]:
         ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/policy_object.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,90 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from uuid import UUID
 
 from catalystwan.endpoints import APIEndpoints, delete, get, post, put, versions
+from catalystwan.models.configuration.feature_profile.common import FeatureProfileInfo, GetFeatureProfilesPayload
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
 from catalystwan.typed_list import DataSequence
 
 
 class PolicyObjectFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
+    @get("/v1/feature-profile/sdwan/policy-object")
+    def get_profiles(
+        self, params: GetFeatureProfilesPayload = GetFeatureProfilesPayload()
+    ) -> DataSequence[FeatureProfileInfo]:
+        ...
+
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}")
     def create(
         self, profile_id: UUID, policy_object_list_type: str, payload: AnyPolicyObjectParcel
     ) -> ParcelCreationResponse:
         ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @post("/v1/feature-profile/sdwan/policy-object/{policy_object_id}/unified/{security_object_list_type}")
     # def create_security_profile_parcel(self, policy_object_id: UUID, security_object_list_type: str):
     #     ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}/{list_object_id}")
     def delete(self, profile_id: UUID, policy_object_list_type: str, list_object_id: UUID) -> None:
         ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @delete(
     #     "/v1/feature-profile/sdwan/policy-object/{policy_object_id}/unified/{security_object_list_type}/{security_profile_parcel_id}"
     # )
     # def delete_security_profile_parcel1(
     #     self, policy_object_id: UUID, security_object_list_type: str, security_profile_parcel_id: UUID
     # ):
     #     ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}/{list_object_id}")
     def update(
         self, profile_id: UUID, policy_object_list_type: str, list_object_id: UUID, payload: AnyPolicyObjectParcel
     ) -> ParcelCreationResponse:
         ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @put(
     #     "/v1/feature-profile/sdwan/policy-object/{policy_object_id}/unified/{security_object_list_type}/{security_profile_parcel_id}"
     # )
     # def edit_security_profile_parcel1(
     #     self, policy_object_id: UUID, security_object_list_type: str, security_profile_parcel_id: UUID
     # ):
     #     ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}/{list_object_id}")
     def get_by_id(self, profile_id: UUID, policy_object_list_type: str, list_object_id: UUID) -> Parcel:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/policy-object/{profile_id}/{policy_object_list_type}", resp_json_key="data")
     def get_all(self, profile_id: UUID, policy_object_list_type: str) -> DataSequence[Parcel]:
         ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @get("/v1/feature-profile/sdwan/policy-object/{policy_object_list_type}/schema")
     # def get_sdwan_policy_object_data_prefix_parcel_schema_by_schema_type(self, policy_object_list_type: str):
     #     ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @get("/v1/feature-profile/sdwan/policy-object/{policy_object_id}/unified/{security_object_list_type}")
     # def get_security_profile_parcel(self, policy_object_id: UUID, security_object_list_type: str):
     #     ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @get(
     #     "/v1/feature-profile/sdwan/policy-object/{policy_object_id}/unified/{security_object_list_type}/{security_profile_parcel_id}"
     # )
     # def get_security_profile_parcel_by_parcel_id(
     #     self, policy_object_id: UUID, security_object_list_type: str, security_profile_parcel_id: UUID
     # ):
     #     ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,7 +60,30 @@
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/service/{profile_uuid}/lan/vpn/{vpn_uuid}/{parcel_type}")
     def associate_parcel_with_vpn(
         self, profile_uuid: UUID, vpn_uuid: UUID, parcel_type: str, payload: ParcelAssociationPayload
     ) -> ParcelCreationResponse:
         ...
+
+    # Ethernet, IPSec, SVI
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @post(
+        "/v1/feature-profile/sdwan/service/{profile_uuid}/lan/vpn/"
+        "{vpn_uuid}/{interface_parcel_type}/{interface_uuid}/dhcp-server"
+    )
+    def associate_dhcp_server_with_vpn_interface(
+        self,
+        profile_uuid: UUID,
+        vpn_uuid: UUID,
+        interface_parcel_type: str,
+        interface_uuid: UUID,
+        payload: ParcelAssociationPayload,
+    ) -> ParcelCreationResponse:
+        ...
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @post("/v1/feature-profile/sdwan/service/{profile_id}/lan/vpn/{vpn_id}/{parcel_type}")
+    def associate_with_vpn(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: ParcelAssociationPayload
+    ) -> ParcelCreationResponse:
+        ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/system.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/topology.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,46 +16,46 @@
 )
 from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse
 from catalystwan.models.configuration.feature_profile.sdwan.topology import AnyTopologyParcel
 from catalystwan.typed_list import DataSequence
 
 
 class TopologyFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/topology")
     def create_topology_feature_profile(self, payload: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/topology")
     def get_topology_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/topology/{profile_id}")
     def get_topology_feature_profile(self, profile_id: str, params: GetFeatureProfilesPayload) -> FeatureProfileDetail:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/topology/{profile_id}")
     def edit_topology_feature_profile(
         self, profile_id: str, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/topology/{profile_id}")
     def delete_topology_feature_profile(self, profile_id: str) -> None:
         ...
 
     #
     # Create/Delete/Get Any Topology Parcel
     #
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/topology/{profile_id}/{parcel_type}")
     def create_any_parcel(
         self, profile_id: UUID, parcel_type: str, payload: AnyTopologyParcel
     ) -> ParcelCreationResponse:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/feature_profile/sdwan/transport.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,112 +11,117 @@
     FeatureProfileCreationResponse,
     FeatureProfileDetail,
     FeatureProfileEditPayload,
     FeatureProfileInfo,
     GetFeatureProfilesPayload,
     SchemaTypeQuery,
 )
-from catalystwan.models.configuration.feature_profile.parcel import Parcel, ParcelCreationResponse, ParcelId
+from catalystwan.models.configuration.feature_profile.parcel import (
+    Parcel,
+    ParcelAssociationPayload,
+    ParcelCreationResponse,
+    ParcelId,
+)
 from catalystwan.models.configuration.feature_profile.sdwan.transport import (
     AnyTransportParcel,
     CellularControllerParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import ManagementVpnParcel
 from catalystwan.typed_list import DataSequence
 
 
 class TransportFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/transport")
     def create_transport_feature_profile(
         self, payload: FeatureProfileCreationPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_transport_feature_profiles(self, params: GetFeatureProfilesPayload) -> DataSequence[FeatureProfileInfo]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}")
     def get_transport_feature_profile(
         self, profile_id: UUID, params: GetFeatureProfilesPayload
     ) -> FeatureProfileDetail:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}")
     def edit_transport_feature_profile(
         self, profile_id: UUID, payload: FeatureProfileEditPayload
     ) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}")
     def delete_transport_feature_profile(self, profile_id: UUID) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
     def create_transport_parcel(
         self, profile_id: UUID, parcel_type: str, payload: _ParcelBase
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/wan/vpn/{vpn_id}/{parcel_type}")
     def create_transport_vpn_sub_parcel(
         self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{vpn_id}/{parcel_type}")
     def create_management_vpn_sub_parcel(
         self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: _ParcelBase
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}")
     def get_transport_parcels(self, profile_id: UUID, parcel_type: str) -> DataSequence[Parcel[AnyTransportParcel]]:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sdwan/transport/{profile_id}/{parcel_type}/{parcel_id}")
     def get_transport_parcel(self, profile_id: UUID, parcel_type: str, parcel_id: UUID) -> Parcel[AnyTransportParcel]:
         ...
 
     #
     # ManagementVPN parcel
     #
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
     def create_management_vpn_parcel(self, profile_id: UUID, payload: _ParcelBase) -> ParcelCreationResponse:
         ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn")
     # def get_management_vpn_parcels(self, profile_id: UUID) -> ParcelSequence[ManagementVPN]:
     #     ...
 
-    # @versions(supported_versions=(">=20.13"), raises=False)
+    # @versions(supported_versions=(">=20.12"), raises=False)
     # @get("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     # def get_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> Parcel[ManagementVPN]:
     #     ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     def edit_management_vpn_parcel(
         self, profile_id: UUID, parcel_id: str, payload: ManagementVpnParcel
     ) -> ParcelCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sdwan/transport/{profile_id}/management/vpn/{parcel_id}")
     def delete_management_vpn_parcel(self, profile_id: UUID, parcel_id: str) -> None:
         ...
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan/transport")
     def get_sdwan_transport_feature_profiles(
@@ -143,7 +148,29 @@
 
     @versions(supported_versions=(">=20.9"), raises=False)
     @post("/v1/feature-profile/sdwan/transport/{transport_id}/cellular-controller")
     def create_cellular_controller_profile_parcel_for_transport(
         self, transport_id: str, payload: CellularControllerParcel
     ) -> ParcelId:
         ...
+
+    #
+    # Cellular controller
+    #
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/cellular-controller/{cellular_controler_id}/{parcel_type}")
+    def associate_with_cellular_controller(
+        self, profile_id: UUID, cellular_controler_id: UUID, parcel_type: str, payload: ParcelAssociationPayload
+    ) -> ParcelId:
+        ...
+
+    #
+    # Routing
+    #
+
+    @versions(supported_versions=(">=20.9"), raises=False)
+    @post("/v1/feature-profile/sdwan/transport/{profile_id}/wan/vpn/{vpn_id}/{parcel_type}")
+    def associate_with_vpn(
+        self, profile_id: UUID, vpn_id: UUID, parcel_type: str, payload: ParcelAssociationPayload
+    ) -> ParcelCreationResponse:
+        ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/abstractions.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/abstractions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/aip.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/amp.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/cflowd.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/cflowd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/control.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/device_access.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/dns_security.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/mesh.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/qos_map.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/rewrite.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/route_policy.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/rule_set.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/security_group.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/ssl_decryption_utd_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/traffic_data.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/url_filtering.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/app.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/app_probe.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/as_path.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/class_map.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/color.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/community.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/data_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/expanded_community.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/expanded_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/extended_community.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/extended_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/fqdn.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/geo_location.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/ips_signature.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/local_app.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/local_domain.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/mirror.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/policer.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/port.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/protocol_name.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/region.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/site.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/sla.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/tloc.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/trunkgroup.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/umbrella_data.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/umbrella_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/url_allow_list.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_allow_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/url_block_list.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/url_block_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/list/zone.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/list/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/security_template.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/security_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/vedge_template.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vedge_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/policy/vsmart_template.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/policy/vsmart_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration/software_actions.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration/software_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_dashboard_status.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_dashboard_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_actions.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_actions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_inventory.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_device_template.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_device_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_feature_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_feature_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 # mypy: disable-error-code="empty-body"
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import _ParcelBase
 from catalystwan.endpoints import JSON, APIEndpoints, delete, get, post, put, versions
 from catalystwan.models.configuration.feature_profile.common import (
     FeatureProfileCreationPayload,
     FeatureProfileCreationResponse,
     FeatureProfileInfo,
 )
+from catalystwan.models.configuration.feature_profile.parcel import ParcelId
 from catalystwan.models.feature_profile_parcel import FullConfigParcel
 from catalystwan.typed_list import DataSequence
 
 
 class SchemaType(str, Enum):
     POST = "post"
     PUT = "put"
@@ -24,18 +25,14 @@
 
 class SchemaTypeQuery(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     schema_type: SchemaType = Field(alias="schemaType")
 
 
-class ParcelId(BaseModel):
-    id: str = Field(alias="parcelId")
-
-
 class GetFeatureProfilesPayload(BaseModel):
     limit: Optional[int]
     offset: Optional[int]
 
 
 class ConfigurationFeatureProfile(APIEndpoints):
     @versions(supported_versions=(">=20.9"), raises=False)
@@ -101,38 +98,38 @@
     @versions(supported_versions=(">=20.9"), raises=False)
     @get("/v1/feature-profile/sdwan")
     def get_sdwan_feature_profiles(self) -> DataSequence[FeatureProfileInfo]:
         ...
 
 
 class SDRoutingConfigurationFeatureProfile(APIEndpoints):
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sd-routing/cli")
     def create_cli_feature_profile(self, payload: FeatureProfileCreationPayload) -> FeatureProfileCreationResponse:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @post("/v1/feature-profile/sd-routing/cli/{cli_fp_id}/full-config")
     def create_cli_full_config_parcel(self, cli_fp_id: str, payload: FullConfigParcel) -> ParcelId:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sd-routing/cli/{cli_fp_id}")
     def delete_cli_feature_profile(self, cli_fp_id: str) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @delete("/v1/feature-profile/sd-routing/cli/{cli_fp_id}/full-config/{parcel_id}")
     def delete_cli_full_config_parcel(self, cli_fp_id: str, parcel_id: str) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @put("/v1/feature-profile/sd-routing/cli/{cli_fp_id}/full-config/{parcel_id}")
     def edit_cli_full_config_parcel(self, cli_fp_id: str, parcel_id: str, payload: FullConfigParcel) -> None:
         ...
 
-    @versions(supported_versions=(">=20.13"), raises=False)
+    @versions(supported_versions=(">=20.12"), raises=False)
     @get("/v1/feature-profile/sd-routing/cli")
     def get_cli_feature_profiles(
         self, payload: Optional[GetFeatureProfilesPayload]
     ) -> DataSequence[FeatureProfileInfo]:
         ...
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_group.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/configuration_settings.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/configuration_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/endpoints_container.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/endpoints_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from catalystwan.endpoints.configuration.device.software_update import ConfigurationDeviceSoftwareUpdate
 from catalystwan.endpoints.configuration.disaster_recovery import ConfigurationDisasterRecovery
 from catalystwan.endpoints.configuration.feature_profile.sdwan.cli import CliFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.sig_security import SIGSecurity
 from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.topology import TopologyFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
+from catalystwan.endpoints.configuration.network_hierarchy import NetworkHierarchy
 from catalystwan.endpoints.configuration.policy.definition.access_control_list import ConfigurationPolicyAclDefinition
 from catalystwan.endpoints.configuration.policy.definition.access_control_list_ipv6 import (
     ConfigurationPolicyAclIPv6Definition,
 )
 from catalystwan.endpoints.configuration.policy.definition.control import ConfigurationPolicyControlDefinition
 from catalystwan.endpoints.configuration.policy.definition.device_access import (
     ConfigurationPolicyDeviceAccessDefinition,
@@ -72,14 +73,15 @@
 from catalystwan.endpoints.configuration.policy.list.url_block_list import ConfigurationPolicyURLBlockList
 from catalystwan.endpoints.configuration.policy.list.vpn import ConfigurationPolicyVPNList
 from catalystwan.endpoints.configuration.policy.list.zone import ConfigurationPolicyZoneList
 from catalystwan.endpoints.configuration.policy.security_template import ConfigurationSecurityTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vedge_template import ConfigurationVEdgeTemplatePolicy
 from catalystwan.endpoints.configuration.policy.vsmart_template import ConfigurationVSmartTemplatePolicy
 from catalystwan.endpoints.configuration.software_actions import ConfigurationSoftwareActions
+from catalystwan.endpoints.configuration.topology_group import TopologyGroupEndpoints
 from catalystwan.endpoints.configuration_dashboard_status import ConfigurationDashboardStatus
 from catalystwan.endpoints.configuration_device_actions import ConfigurationDeviceActions
 from catalystwan.endpoints.configuration_device_inventory import ConfigurationDeviceInventory
 from catalystwan.endpoints.configuration_device_template import ConfigurationDeviceTemplate
 from catalystwan.endpoints.configuration_feature_profile import (
     ConfigurationFeatureProfile,
     SDRoutingConfigurationFeatureProfile,
@@ -174,15 +176,16 @@
     def __init__(self, session: ManagerSession):
         self.sdwan = ConfigurationSDWANFeatureProfileContainer(session=session)
 
 
 class ConfigurationContainer:
     def __init__(self, session: ManagerSession):
         self.policy = ConfigurationPolicyContainer(session)
-        self.feature_profile = ConfigurationFeatureProfileContainer(session=session)
+        self.feature_profile = ConfigurationFeatureProfileContainer(session)
+        self.topology_group = TopologyGroupEndpoints(session)
 
 
 class TroubleshootingToolsContainer:
     def __init__(self, session: ManagerSession):
         self.device_connectivity = TroubleshootingToolsDeviceConnectivity(session)
 
 
@@ -204,14 +207,15 @@
         self.configuration_device_template = ConfigurationDeviceTemplate(session)
         self.configuration_settings = ConfigurationSettings(session)
         self.configuration_software_actions = ConfigurationSoftwareActions(session)
         self.configuration_disaster_recovery = ConfigurationDisasterRecovery(session)
         self.monitoring_device_details = MonitoringDeviceDetails(session)
         self.monitoring_server_info = ServerInfo(session)
         self.monitoring_status = MonitoringStatus(session)
+        self.network_hierarchy = NetworkHierarchy(session)
         self.sdavc_cloud_connector = SDAVCCloudConnector(session)
         self.tenant_backup_restore = TenantBackupRestore(session)
         self.tenant_management = TenantManagement(session)
         self.tenant_migration = TenantMigration(session)
         self.configuration_feature_profile = ConfigurationFeatureProfile(session)
         self.configuration_group = ConfigurationGroup(session)
         self.sd_routing_configuration_feature_profile = SDRoutingConfigurationFeatureProfile(session)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/misc.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/monitoring/device_details.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/device_details.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/monitoring/status.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/monitoring/status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/real_time_monitoring/reboot_history.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/real_time_monitoring/reboot_history.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/sdavc_cloud_connector.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/sdavc_cloud_connector.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_backup_restore.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_backup_restore.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_management.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_management.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/tenant_migration.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py` & `catalystwan-0.33.7.dev2/catalystwan/endpoints/troubleshooting_tools/device_connectivity.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/exceptions.py` & `catalystwan-0.33.7.dev2/catalystwan/exceptions.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/base.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/base.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_other.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_other.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_service.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ipaddress import IPv4Address, IPv6Interface
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
+from ipaddress import IPv4Address, IPv4Interface, IPv6Interface
 from typing import Literal
 from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, as_global, as_variable
 from catalystwan.integration_tests.feature_profile.sdwan.base import TestFeatureProfileModels
 from catalystwan.models.common import (
     CableLengthLongValue,
@@ -21,15 +22,24 @@
     MultilinkClockSource,
     MultilinkControllerTxExList,
     MultilinkControllerType,
     MultilinkMethod,
     MultilinkNimList,
     MultilinkTxExName,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.acl import Ipv4AclParcel, Ipv6AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv4acl import Ipv4AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv6acl import Ipv6AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospf import RoutingOspfParcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospfv3 import (
+    Ospfv3InterfaceParametres,
+    Ospfv3IPv4Area,
+    Ospfv3IPv6Area,
+    RoutingOspfv3IPv4Parcel,
+    RoutingOspfv3IPv6Parcel,
+)
 from catalystwan.models.configuration.feature_profile.sdwan.service.dhcp_server import (
     AddressPool,
     LanVpnDhcpServerParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.service.eigrp import (
     AddressFamily,
     EigrpParcel,
@@ -58,22 +68,14 @@
     RPAnnounce,
     RpDiscoveryScope,
     SsmAttributes,
     SsmFlag,
     StaticJoin,
     StaticRpAddress,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospf import OspfParcel
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospfv3 import (
-    Ospfv3InterfaceParametres,
-    Ospfv3IPv4Area,
-    Ospfv3IPv4Parcel,
-    Ospfv3IPv6Area,
-    Ospfv3IPv6Parcel,
-)
 from catalystwan.models.configuration.feature_profile.sdwan.service.route_policy import RoutePolicyParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.switchport import (
     ControlDirection,
     Duplex,
     HostMode,
     PortControl,
     Speed,
@@ -127,26 +129,26 @@
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, vpn_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_default_values_ospf_parcel_expect_successful_post(self):
         # Arrange
-        ospf_parcel = OspfParcel(
-            parcel_name="TestOspfParcel",
+        ospf_parcel = RoutingOspfParcel(
+            parcel_name="TestRoutingOspfParcel",
             parcel_description="Test Ospf Parcel",
         )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, ospf_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_default_ospfv3_ipv4_expect_successful_post(self):
         # Arrange
-        ospfv3ipv4_parcel = Ospfv3IPv4Parcel(
+        ospfv3ipv4_parcel = RoutingOspfv3IPv4Parcel(
             parcel_name="TestOspfv3ipv4",
             parcel_description="Test Ospfv3ipv4 Parcel",
             area=[
                 Ospfv3IPv4Area(
                     area_number=as_global(5),
                     interfaces=[Ospfv3InterfaceParametres(name=as_global("GigabitEthernet0/0/0"))],
                 )
@@ -155,26 +157,26 @@
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, ospfv3ipv4_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_default_ospfv3_ipv6_expect_successful_post(self):
         # Arrange
-        ospfv3ipv4_parcel = Ospfv3IPv6Parcel(
+        ospfv3ipv6_parcel = RoutingOspfv3IPv6Parcel(
             parcel_name="TestOspfv3ipv6",
             parcel_description="Test Ospfv3ipv6 Parcel",
             area=[
                 Ospfv3IPv6Area(
                     area_number=as_global(7),
                     interfaces=[Ospfv3InterfaceParametres(name=as_global("GigabitEthernet0/0/0"))],
                 )
             ],
         )
         # Act
-        parcel_id = self.api.create_parcel(self.profile_uuid, ospfv3ipv4_parcel).id
+        parcel_id = self.api.create_parcel(self.profile_uuid, ospfv3ipv6_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_default_values_eigrp_parcel_expect_successful_post(self):
         eigrp_parcel = EigrpParcel(
             parcel_name="TestEigrpParcel",
             parcel_description="Test Eigrp Parcel",
@@ -202,33 +204,80 @@
             parcel_description="Test Route Policy Parcel",
         )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, route_policy_parcel).id
         # Assert
         assert parcel_id
 
+    def test_when_default_values_acl_ipv4_expect_successful_post(self):
+        # Arrange
+        acl_ipv4_parcel = Ipv4AclParcel(
+            parcel_name="TestAclIpv4Parcel",
+            parcel_description="Test Acl Ipv4 Parcel",
+        )
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv4_parcel).id
+        # Assert
+        assert parcel_id
+
+    def test_when_fully_specified_acl_ipv4_expect_successful_post(self):
+        # Arrange
+        acl_ipv4_parcel = Ipv4AclParcel(
+            parcel_name="TestAclIpv4Parcel-Full",
+            parcel_description="Test Acl Ipv4 Parcel",
+        )
+        # Arrange Sequence 1
+        seq1 = acl_ipv4_parcel.add_sequence("Sequence1", 10, "accept")
+        seq1.match_destination_data_prefix(IPv4Interface("10.0.0.0/16"))
+        seq1.match_dscp([50, 55])
+        seq1.match_icmp_msg(["dod-host-prohibited", "extended-echo", "dod-net-prohibited"])
+        seq1.match_packet_length((1000, 8000))
+        seq1.match_protocol([1])
+        seq1.match_source_data_prefix(IPv4Interface("11.0.0.0/16"))
+        # Arrange Sequence 2
+        seq2 = acl_ipv4_parcel.add_sequence("Sequence2", 20, "drop")
+        seq2.match_destination_data_prefix_variable("varDestPrefix2")
+        seq2.match_source_data_prefix_variable("varSrcPrefix2")
+        seq2.match_destination_ports([233])
+        seq2.match_source_ports([1, 3, (10, 100), (50, 200), 600])
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv4_parcel).id
+        # Assert
+        assert parcel_id
+
     def test_when_default_values_acl_ipv6_expect_successful_post(self):
         # Arrange
         acl_ipv6_parcel = Ipv6AclParcel(
             parcel_name="TestAclIpv6Parcel",
             parcel_description="Test Acl Ipv6 Parcel",
         )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv6_parcel).id
         # Assert
         assert parcel_id
 
-    def test_when_default_values_acl_ipv4_expect_successful_post(self):
+    def test_when_fully_specified_acl_ipv6_expect_successful_post(self):
         # Arrange
-        acl_ipv4_parcel = Ipv4AclParcel(
-            parcel_name="TestAclIpv4Parcel",
-            parcel_description="Test Acl Ipv4 Parcel",
+        acl_ipv6_parcel = Ipv6AclParcel(
+            parcel_name="TestAclIpv6Parcel-Full",
+            parcel_description="Test Acl Ipv6 Parcel",
         )
+        # Arrange Sequence 1
+        seq1 = acl_ipv6_parcel.add_sequence("Sequence1", 10, "accept")
+        seq1.match_destination_data_prefix(IPv6Interface("2001:db8:abcd:0012::/64"))
+        seq1.match_icmp_msg(["cp-solicitation", "ind-advertisement"])
+        seq1.match_packet_length((1000, 8000))
+        seq1.match_source_data_prefix(IPv6Interface("2001:db8:1111:0012::/64"))
+        seq1.match_traffic_class([3])
+        # Arrange Sequence 2
+        seq2 = acl_ipv6_parcel.add_sequence("Sequence2", 20, "drop")
+        seq2.match_destination_ports([233])
+        seq2.match_source_ports([1, 3, (10, 100), (50, 200), 600])
         # Act
-        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv4_parcel).id
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv6_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_correct_values_switchport_parcel_expect_successful_post(self):
         # Arrange
         switchport_default_values_parcel = SwitchportParcel(
             parcel_name="TestSwitchportParcelDefaultValues",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_system.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from catalystwan.integration_tests.feature_profile.sdwan.base import TestFeatureProfileModels
 from catalystwan.models.configuration.feature_profile.sdwan.system import (
     BannerParcel,
     BasicParcel,
     BFDParcel,
+    DeviceAccessIPv4Parcel,
+    DeviceAccessIPv6Parcel,
     GlobalParcel,
     LoggingParcel,
     MRFParcel,
     NtpParcel,
     OMPParcel,
     SecurityParcel,
     SNMPParcel,
@@ -277,7 +279,75 @@
             parcel_name="OMPDefault",
             parcel_description="OMP Parcel",
         )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, omp_parcel).id
         # Assert
         assert parcel_id
+
+    def test_when_default_values_device_access_parcel_expect_successful_post(self):
+        device_access_parcel = DeviceAccessIPv4Parcel(
+            parcel_name="DeviceAccessDefault",
+            parcel_description="DeviceAccessDefault",
+        )
+
+        parcel_id = self.api.create_parcel(self.profile_uuid, device_access_parcel).id
+
+        assert parcel_id
+
+        self.api.delete_parcel(self.profile_uuid, DeviceAccessIPv4Parcel, parcel_id)
+
+    def test_when_fully_specified_device_access_parcel_expect_successful_post(self):
+        device_access_parcel = DeviceAccessIPv4Parcel(
+            parcel_name="DeviceAccessDefault",
+            parcel_description="DeviceAccessDefault",
+        )
+        for i in range(2):
+            sequence = device_access_parcel.add_sequence(
+                sequence_id=i + 1,
+                sequence_name=f"sequence_{i+1}",
+                destination_port=22,
+                base_action="accept",
+            )
+            sequence.match_destination_data_prefix(["10.0.0.1/32", "10.0.0.0/16"])
+            sequence.match_source_data_prefix(["10.0.0.1/32", "10.0.0.0/16"])
+            sequence.match_source_ports([1, 2, 3])
+
+        parcel_id = self.api.create_parcel(self.profile_uuid, device_access_parcel).id
+
+        assert parcel_id
+
+        self.api.delete_parcel(self.profile_uuid, DeviceAccessIPv4Parcel, parcel_id)
+
+    def test_when_default_values_device_access_ipv6_parcel_expect_successful_post(self):
+        device_access_ipv6_parcel = DeviceAccessIPv6Parcel(
+            parcel_name="DeviceAccessDefault",
+            parcel_description="DeviceAccessDefault",
+        )
+
+        parcel_id = self.api.create_parcel(self.profile_uuid, device_access_ipv6_parcel).id
+
+        assert parcel_id
+
+        self.api.delete_parcel(self.profile_uuid, DeviceAccessIPv6Parcel, parcel_id)
+
+    def test_when_fully_specified_device_access_ipv6_parcel_expect_successful_post(self):
+        device_access_ipv6_parcel = DeviceAccessIPv6Parcel(
+            parcel_name="DeviceAccessDefault",
+            parcel_description="DeviceAccessDefault",
+        )
+        for i in range(2):
+            sequence = device_access_ipv6_parcel.add_sequence(
+                sequence_id=i + 1,
+                sequence_name=f"sequence_{i+1}",
+                destination_port=22,
+                base_action="accept",
+            )
+            sequence.match_destination_data_prefix(["::250/100", "::54a/64"])
+            sequence.match_source_data_prefix(["::250/100", "::54a/64"])
+            sequence.match_source_ports([1, 2, 3])
+
+        parcel_id = self.api.create_parcel(self.profile_uuid, device_access_ipv6_parcel).id
+
+        assert parcel_id
+
+        self.api.delete_parcel(self.profile_uuid, DeviceAccessIPv6Parcel, parcel_id)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/test_transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from ipaddress import IPv4Address, IPv6Address, IPv6Interface
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
+from ipaddress import IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 from typing import List, Literal
 from uuid import UUID
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, as_global
 from catalystwan.integration_tests.feature_profile.sdwan.base import TestFeatureProfileModels
+from catalystwan.integration_tests.test_data import cellular_controller_parcel, cellular_profile_parcel, gps_parcel
 from catalystwan.models.common import (
     CableLengthLongValue,
     CarrierType,
     ClockRate,
     CoreRegion,
     E1Framing,
     E1Linecode,
@@ -22,19 +24,20 @@
     T1Linecode,
     TLOCColor,
 )
 from catalystwan.models.configuration.feature_profile.common import AclQos
 from catalystwan.models.configuration.feature_profile.common import AddressWithMask as CommonPrefix
 from catalystwan.models.configuration.feature_profile.common import AdvancedGre, AllowService
 from catalystwan.models.configuration.feature_profile.common import Arp as CommonArp
-from catalystwan.models.configuration.feature_profile.common import ChannelGroup
+from catalystwan.models.configuration.feature_profile.common import ChannelGroup, DNSIPv4, DNSIPv6
 from catalystwan.models.configuration.feature_profile.common import (
     EthernetNatAttributesIpv4 as EthernetNatAttributesIpv4,
 )
 from catalystwan.models.configuration.feature_profile.common import (
+    HostMapping,
     InterfaceStaticIPv4Address,
     MultilinkAuthenticationType,
     MultilinkClockSource,
     MultilinkControllerTxExList,
     MultilinkControllerType,
     MultilinkMethod,
     MultilinkNimList,
@@ -44,26 +47,16 @@
     ShapingRateUpstreamConfig,
     SourceLoopback,
     StaticIPv4Address,
     StaticIPv4AddressConfig,
     StaticNat,
     TunnelSourceType,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import (
-    CellularControllerParcel,
-    ControllerConfig,
-)
-from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_profile import (
-    Authentication,
-    CellularProfileParcel,
-    NeedAuthentication,
-    ProfileConfig,
-    ProfileInfo,
-)
-from catalystwan.models.configuration.feature_profile.sdwan.transport.gps import GpsParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv4acl import Ipv4AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv6acl import Ipv6AclParcel
 from catalystwan.models.configuration.feature_profile.sdwan.transport.management.ethernet import (
     Advanced as ManagementEthernetAdvanced,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.management.ethernet import (
     InterfaceEthernetParcel as ManagementEthernetParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.management.ethernet import (
@@ -81,20 +74,17 @@
     E1Basic,
     Long,
     T1Basic,
     T1E1ControllerParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import (
     Address64V4PoolItem,
-    DnsIpv4,
-    DnsIpv6,
     Ipv4RouteItem,
     Ipv6RouteItem,
     ManagementVpnParcel,
-    NewHostMappingItem,
     NextHopItem,
     OneOfIpRouteNull0,
     Prefix,
     ServiceItem,
     ServiceType,
     SubnetMask,
     TransportVpnParcel,
@@ -176,26 +166,26 @@
         cls.profile_uuid = cls.api.create_profile("TestTransportService", "Description").id
 
     def test_when_fully_specified_management_vpn_parcel_expect_successful_post(self):
         # Arrange
         management_vpn_parcel = ManagementVpnParcel(
             parcel_name="FullySpecifiedManagementVpnParcel",
             description="Description",
-            dns_ipv6=DnsIpv6(
+            dns_ipv6=DNSIPv6(
                 primary_dns_address_ipv6=as_global(IPv6Address("67ca:c2df:edfe:c8ec:b6cb:f9f4:eab0:ece6")),
                 secondary_dns_address_ipv6=as_global(IPv6Address("8989:8d33:c00a:4d13:324d:8b23:8d77:a289")),
             ),
-            dns_ipv4=DnsIpv4(
+            dns_ipv4=DNSIPv4(
                 primary_dns_address_ipv4=as_global(IPv4Address("68.138.29.222")),
                 secondary_dns_address_ipv4=as_global(IPv4Address("122.89.114.112")),
             ),
             new_host_mapping=[
-                NewHostMappingItem(
+                HostMapping(
                     host_name=as_global("FullySpecifiedHost"),
-                    list_of_ip=as_global(
+                    list_of_ips=as_global(
                         [
                             "165.16.181.116",
                             "7a4c:1d87:8587:a6ec:21a6:48a7:00e8:1fef",
                         ]
                     ),
                 )
             ],
@@ -289,71 +279,101 @@
         )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, t1e1controller).id
         # Assert
         assert parcel_id
 
     def test_when_fully_specifed_gps_parcel_expect_successful_post(self):
-        # Arrange
-        gps_parcel = GpsParcel(
-            parcel_name="GpsParcel",
-            parcel_description="Description",
-            destination_address=Global[IPv4Address](value=IPv4Address("66.22.1.2")),
-            destination_port=Global[int](value=266),
-            enable=Global[bool](value=True),
-            mode=Global[Literal["ms-based", "standalone"]](value="standalone"),
-            nmea=Global[bool](value=True),
-            source_address=Global[IPv4Address](value=IPv4Address("76.22.3.9")),
-        )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, gps_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_fully_specifed_cellular_controller_expect_successful_post(self):
-        cellular_controller_parcel = CellularControllerParcel(
-            parcel_name="CellularControllerParcel",
-            description="Description",
-            controller_config=ControllerConfig(
-                id=as_global("0/2/0"),
-                slot=as_global(1),
-                max_retry=as_global(3),
-                failover_timer=as_global(4),
-                auto_sim=as_global(True),
-            ),
-        )
         # Act
         parcel_id = self.api.create_parcel(self.profile_uuid, cellular_controller_parcel).id
         # Assert
         assert parcel_id
 
     def test_when_fully_specifed_cellular_profile_expect_successful_post(self):
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, cellular_profile_parcel).id
+        # Assert
+        assert parcel_id
+
+    def test_when_default_values_acl_ipv4_expect_successful_post(self):
         # Arrange
-        cellular_profile_parcel = CellularProfileParcel(
-            parcel_name="CellularProfileParcel",
-            parcel_description="Description",
-            profile_config=ProfileConfig(
-                id=Global[int](value=2),
-                profile_info=ProfileInfo(
-                    apn=Global[str](value="KvqJrCD"),
-                    authentication=Authentication(
-                        need_authentication=NeedAuthentication(
-                            password=Global[str](value="HfBBBHZlFH"),
-                            type=Global[Literal["chap", "pap", "pap_chap"]](value="chap"),
-                            username=Global[str](value="BABBBBBBV"),
-                        )
-                    ),
-                    no_overwrite=Global[bool](value=False),
-                    pdn_type=Global[Literal["ipv4", "ipv4v6", "ipv6"]](value="ipv4"),
-                ),
-            ),
-            config_type=Default[Literal["non-eSim"]](value="non-eSim"),
+        acl_ipv4_parcel = Ipv4AclParcel(
+            parcel_name="TestAclIpv4Parcel-Defaults",
+            parcel_description="Test Acl Ipv4 Parcel",
         )
         # Act
-        parcel_id = self.api.create_parcel(self.profile_uuid, cellular_profile_parcel).id
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv4_parcel).id
+        self.api.get_parcel(self.profile_uuid, Ipv4AclParcel, parcel_id)
+        # Assert
+        assert parcel_id
+
+    def test_when_fully_specified_acl_ipv4_expect_successful_post(self):
+        # Arrange
+        acl_ipv4_parcel = Ipv4AclParcel(
+            parcel_name="TestAclIpv4Parcel-Full",
+            parcel_description="Test Acl Ipv4 Parcel",
+        )
+        # Arrange Sequence 1
+        seq1 = acl_ipv4_parcel.add_sequence("Sequence1", 10, "accept")
+        seq1.match_destination_data_prefix(IPv4Interface("10.0.0.0/16"))
+        seq1.match_dscp([50, 55])
+        seq1.match_icmp_msg(["dod-host-prohibited", "extended-echo", "dod-net-prohibited"])
+        seq1.match_packet_length((1000, 8000))
+        seq1.match_protocol([1])
+        seq1.match_source_data_prefix(IPv4Interface("11.0.0.0/16"))
+        # Arrange Sequence 2
+        seq2 = acl_ipv4_parcel.add_sequence("Sequence2", 20, "drop")
+        seq2.match_destination_data_prefix_variable("varDestPrefix2")
+        seq2.match_source_data_prefix_variable("varSrcPrefix2")
+        seq2.match_destination_ports([233])
+        seq2.match_source_ports([1, 3, (10, 100), (50, 200), 600])
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv4_parcel).id
+        self.api.get_parcel(self.profile_uuid, Ipv4AclParcel, parcel_id)
+        # Assert
+        assert parcel_id
+
+    def test_when_default_values_acl_ipv6_expect_successful_post(self):
+        # Arrange
+        acl_ipv6_parcel = Ipv6AclParcel(
+            parcel_name="TestAclIpv6Parcel-Defaults",
+            parcel_description="Test Acl Ipv6 Parcel",
+        )
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv6_parcel).id
+        self.api.get_parcel(self.profile_uuid, Ipv6AclParcel, parcel_id)
+        # Assert
+        assert parcel_id
+
+    def test_when_fully_specified_acl_ipv6_expect_successful_post(self):
+        # Arrange
+        acl_ipv6_parcel = Ipv6AclParcel(
+            parcel_name="TestAclIpv6Parcel-Full",
+            parcel_description="Test Acl Ipv6 Parcel",
+        )
+        # Arrange Sequence 1
+        seq1 = acl_ipv6_parcel.add_sequence("Sequence1", 10, "accept")
+        seq1.match_destination_data_prefix(IPv6Interface("2001:db8:abcd:0012::/64"))
+        seq1.match_icmp_msg(["cp-solicitation", "ind-advertisement"])
+        seq1.match_packet_length((1000, 8000))
+        seq1.match_source_data_prefix(IPv6Interface("2001:db8:1111:0012::/64"))
+        seq1.match_traffic_class([3])
+        # Arrange Sequence 2
+        seq2 = acl_ipv6_parcel.add_sequence("Sequence2", 20, "drop")
+        seq2.match_destination_ports([233])
+        seq2.match_source_ports([1, 3, (10, 100), (50, 200), 600])
+        # Act
+        parcel_id = self.api.create_parcel(self.profile_uuid, acl_ipv6_parcel).id
+        self.api.get_parcel(self.profile_uuid, Ipv6AclParcel, parcel_id)
         # Assert
         assert parcel_id
 
     @classmethod
     def tearDownClass(cls) -> None:
         cls.api.delete_profile(cls.profile_uuid)
         super().tearDownClass()
@@ -412,26 +432,26 @@
         assert parcel_id
 
     def test_when_fully_specifed_transport_vpn_parcel_expect_successful_post(self):
         # Arrange
         transport_vpn_parcel = TransportVpnParcel(
             parcel_name="FullySpecifiedTransportVpnParcel",
             description="Description",
-            dns_ipv6=DnsIpv6(
+            dns_ipv6=DNSIPv6(
                 primary_dns_address_ipv6=as_global(IPv6Address("67ca:c2df:edfe:c8ec:b6cb:f9f4:eab0:ece6")),
                 secondary_dns_address_ipv6=as_global(IPv6Address("8989:8d33:c00a:4d13:324d:8b23:8d77:a289")),
             ),
-            dns_ipv4=DnsIpv4(
+            dns_ipv4=DNSIPv4(
                 primary_dns_address_ipv4=as_global(IPv4Address("68.138.29.222")),
                 secondary_dns_address_ipv4=as_global(IPv4Address("122.89.114.112")),
             ),
             new_host_mapping=[
-                NewHostMappingItem(
+                HostMapping(
                     host_name=as_global("FullySpecifiedHost"),
-                    list_of_ip=as_global(
+                    list_of_ips=as_global(
                         [
                             "165.16.181.116",
                             "7a4c:1d87:8587:a6ec:21a6:48a7:00e8:1fef",
                         ]
                     ),
                 )
             ],
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/feature_profile/sdwan/topology/test_topology.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/test_config_migration.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_config_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/integration_tests/test_find_template_values.py` & `catalystwan-0.33.7.dev2/catalystwan/integration_tests/test_find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/logging.conf` & `catalystwan-0.33.7.dev2/catalystwan/logging.conf`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/common.py` & `catalystwan-0.33.7.dev2/catalystwan/models/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,22 +174,27 @@
 SpaceSeparatedPositiveIntList = Annotated[
     List[PositiveInt],
     PlainSerializer(lambda x: " ".join(map(str, x)), return_type=str, when_used="json-unless-none"),
     BeforeValidator(str_as_positive_int_list),
 ]
 
 
-def int_range_str_validator(value: Union[str, IntRange], ascending: bool = True) -> IntRange:
-    """Validates input given as string containing integer pair separated by hyphen eg: '1-3' or single number '1'"""
+def int_range_str_validator(value: Union[str, int, IntRange], ascending: bool = True) -> IntRange:
+    """
+    Validates input given as string containing integer pair separated by hyphen
+    eg: '1-3' or single number '1'
+    """
     if isinstance(value, str):
         int_list = [int(i) for i in value.strip().split("-")]
-        assert 0 < len(int_list) <= 2, "Number range must contain one or two numbers"
+        assert 0 < len(int_list) <= 2, "Number range string must contain one or two numbers"
         first = int_list[0]
         second = None if len(int_list) == 1 else int_list[1]
         int_range = (first, second)
+    elif isinstance(value, int):
+        int_range = (value, None)
     else:
         int_range = value
     if ascending and int_range[1] is not None:
         assert int_range[0] < int_range[1], "Numbers in range must be in ascending order"
     return int_range
 
 
@@ -200,14 +205,15 @@
 
 IntRangeStr = Annotated[
     IntRange,
     PlainSerializer(int_range_serializer, return_type=str, when_used="json-unless-none"),
     BeforeValidator(int_range_str_validator),
 ]
 
+BasicPolicyActionType = Literal["accept", "drop"]
 
 CarrierType = Literal[
     "default",
     "carrier1",
     "carrier2",
     "carrier3",
     "carrier4",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/docs/diagram.png` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/docs/diagram.png`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/README.md` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/README.md`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/builder.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/builder.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/common.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from datetime import datetime
-from ipaddress import IPv4Address, IPv4Interface, IPv6Interface
+from ipaddress import IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, as_default, as_global
 from catalystwan.models.common import (
@@ -23,17 +23,14 @@
     SubnetMask,
     T1Framing,
     T1Linecode,
     check_fields_exclusive,
 )
 from catalystwan.models.configuration.common import Solution
 
-IPV4Address = str
-IPv6Address = str
-
 ProfileType = Literal[
     "transport",
     "system",
     "cli",
     "service",
     "application-priority",
     "policy-object",  # automatically created default policy object feature profile
@@ -112,54 +109,74 @@
 class SchemaTypeQuery(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     schema_type: SchemaType = Field(alias="schemaType")
 
 
 class GetFeatureProfilesPayload(BaseModel):
-    limit: Optional[int]
-    offset: Optional[int]
+    limit: Optional[int] = None
+    offset: Optional[int] = None
 
 
 class GetReferenceCountFeatureProfilesPayload(GetFeatureProfilesPayload):
     model_config = ConfigDict(populate_by_name=True)
 
     reference_count: Optional[bool] = Field(serialization_alias="referenceCount", validation_alias="referenceCount")
 
 
 class DNSIPv4(BaseModel):
-    primary_dns_address_ipv4: Union[Default[None], Global[str], Variable] = Field(
-        default=Default[None](value=None), alias="primaryDnsAddressIpv4"
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    primary_dns_address_ipv4: Union[Default[None], Global[str], Global[IPv4Address], Variable] = Field(
+        default=Default[None](value=None),
+        serialization_alias="primaryDnsAddressIpv4",
+        validation_alias="primaryDnsAddressIpv4",
     )
-    secondary_dns_address_ipv4: Union[Default[None], Global[str], Variable] = Field(
-        default=Default[None](value=None), alias="secondaryDnsAddressIpv4"
+    secondary_dns_address_ipv4: Optional[Union[Default[None], Global[str], Global[IPv4Address], Variable]] = Field(
+        default=None,
+        serialization_alias="secondaryDnsAddressIpv4",
+        validation_alias="secondaryDnsAddressIpv4",
     )
 
 
 class DNSIPv6(BaseModel):
-    primary_dns_address_ipv6: Union[Default[None], Global[str], Variable] = Field(
-        default=Default[None](value=None), alias="primaryDnsAddressIpv6"
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    primary_dns_address_ipv6: Union[Default[None], Global[str], Global[IPv6Address], Variable] = Field(
+        default=Default[None](value=None),
+        serialization_alias="primaryDnsAddressIpv6",
+        validation_alias="primaryDnsAddressIpv6",
     )
-    secondary_dns_address_ipv6: Union[Default[None], Global[str], Variable] = Field(
-        default=Default[None](value=None), alias="secondaryDnsAddressIpv6"
+    secondary_dns_address_ipv6: Optional[Union[Default[None], Global[str], Global[IPv6Address], Variable]] = Field(
+        default=None,
+        serialization_alias="secondaryDnsAddressIpv6",
+        validation_alias="secondaryDnsAddressIpv6",
     )
 
 
 class HostMapping(BaseModel):
-    host_name: Union[Global[str], Variable] = Field(alias="hostName")
-    list_of_ips: Union[Global[List[str]], Variable] = Field(alias="listOfIp")
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    host_name: Union[Global[str], Variable] = Field(serialization_alias="hostName", validation_alias="hostName")
+    list_of_ips: Union[Global[List[str]], Variable] = Field(serialization_alias="listOfIp", validation_alias="listOfIp")
 
 
 class NextHop(BaseModel):
     address: Union[Global[str], Variable] = Field()
     distance: Union[Default[int], Global[int], Default[int]] = Field(default=Default[int](value=1))
 
 
 class IPv4Prefix(BaseModel):
-    ip_address: Union[Global[IPV4Address], Variable] = Field()
+    ip_address: Union[Global[IPv4Address], Variable] = Field()
     subnet_mask: Union[Global[str], Variable] = Field()
 
 
 class WANIPv4StaticRoute(BaseModel):
     prefix: IPv4Prefix = Field()
     gateway: Global[Literal["nextHop", "null0", "dhcp"]] = Field(default=Global(value="nextHop"), alias="gateway")
     next_hops: Optional[List[NextHop]] = Field(default_factory=list, alias="nextHop")
@@ -678,7 +695,109 @@
 
     if_name: Union[Variable, Global[str]] = Field(validation_alias="ifName", serialization_alias="ifName")
     bandwidth: Optional[Union[Variable, Global[int], Default[None]]] = Field(default=None)
     clock_rate: Optional[Union[Variable, Global[ClockRate], Default[None]]] = Field(
         default=None, validation_alias="clockRate", serialization_alias="clockRate"
     )
     description: Optional[Union[Variable, Global[str], Default[None]]] = Field(default=None)
+
+
+IcmpMsg = Literal[
+    "administratively-prohibited",
+    "dod-host-prohibited",
+    "dod-net-prohibited",
+    "echo",
+    "echo-reply",
+    "echo-reply-no-error",
+    "extended-echo",
+    "extended-echo-reply",
+    "general-parameter-problem",
+    "host-isolated",
+    "host-precedence-unreachable",
+    "host-redirect",
+    "host-tos-redirect",
+    "host-tos-unreachable",
+    "host-unknown",
+    "host-unreachable",
+    "interface-error",
+    "malformed-query",
+    "multiple-interface-match",
+    "net-redirect",
+    "net-tos-redirect",
+    "net-tos-unreachable",
+    "net-unreachable",
+    "network-unknown",
+    "no-room-for-option",
+    "option-missing",
+    "packet-too-big",
+    "parameter-problem",
+    "photuris",
+    "port-unreachable",
+    "precedence-unreachable",
+    "protocol-unreachable",
+    "reassembly-timeout",
+    "redirect",
+    "router-advertisement",
+    "router-solicitation",
+    "source-route-failed",
+    "table-entry-error",
+    "time-exceeded",
+    "timestamp-reply",
+    "timestamp-request",
+    "ttl-exceeded",
+    "unreachable",
+]
+
+Icmp6Msg = Literal[
+    "beyond-scope",
+    "cp-advertisement",
+    "cp-solicitation",
+    "destination-unreachable",
+    "dhaad-reply",
+    "dhaad-request",
+    "echo-reply",
+    "echo-request",
+    "header",
+    "hop-limit",
+    "ind-advertisement",
+    "ind-solicitation",
+    "mld-query",
+    "mld-reduction",
+    "mld-report",
+    "mldv2-report",
+    "mpd-advertisement",
+    "mpd-solicitation",
+    "mr-advertisement",
+    "mr-solicitation",
+    "mr-termination",
+    "nd-na",
+    "nd-ns",
+    "next-header-type",
+    "ni-query",
+    "ni-query-name",
+    "ni-query-v4-address",
+    "ni-query-v6-address",
+    "ni-response",
+    "ni-response-qtype-unknown",
+    "ni-response-refuse",
+    "ni-response-success",
+    "no-admin",
+    "no-route",
+    "packet-too-big",
+    "parameter-option",
+    "parameter-problem",
+    "port-unreachable",
+    "reassembly-timeout",
+    "redirect",
+    "reject-route",
+    "renum-command",
+    "renum-result",
+    "renum-seq-number",
+    "router-advertisement",
+    "router-renumbering",
+    "router-solicitation",
+    "rpl-control",
+    "source-policy",
+    "source-route-header",
+    "time-exceeded",
+    "unreachable",
+]
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/parcel.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/parcel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-from typing import Generic, List, Literal, TypeVar, Union
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
+from functools import lru_cache
+from typing import Generic, List, Literal, Sequence, TypeVar, Union, cast
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, model_validator
 from typing_extensions import Annotated
 
 from catalystwan.models.configuration.feature_profile.sdwan.application_priority import AnyApplicationPriorityParcel
 from catalystwan.models.configuration.feature_profile.sdwan.cli import AnyCliParcel
 from catalystwan.models.configuration.feature_profile.sdwan.dns_security import AnyDnsSecurityParcel
 from catalystwan.models.configuration.feature_profile.sdwan.embedded_security import AnyEmbeddedSecurityParcel
 from catalystwan.models.configuration.feature_profile.sdwan.other import AnyOtherParcel
 from catalystwan.models.configuration.feature_profile.sdwan.policy_object import AnyPolicyObjectParcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing import AnyRoutingParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service import AnyServiceParcel
 from catalystwan.models.configuration.feature_profile.sdwan.sig_security import AnySIGSecurityParcel
 from catalystwan.models.configuration.feature_profile.sdwan.system import AnySystemParcel
 from catalystwan.models.configuration.feature_profile.sdwan.topology import AnyTopologyParcel
 from catalystwan.models.configuration.feature_profile.sdwan.transport import AnyTransportParcel
+from catalystwan.utils.model import resolve_nested_base_model_unions
 
 ParcelType = Literal[
     "aaa",
     "app-list",
     "app-probe",
     "appqoe",
     "as-path",
@@ -26,24 +30,26 @@
     "basic",
     "bfd",
     "bgp",
     "cellular-controller",
     "class",
     "color",
     "config",
-    "config",
     "custom-control",
     "data-ipv6-prefix",
     "data-prefix",
     "dhcp-server",
     "dns",
     "expanded-community",
+    "ext-community",
     "global",
     "gps",
     "hubspoke",
+    "ipv4-acl",
+    "ipv6-acl",
     "ipv6-prefix",
     "lan/vpn",
     "lan/vpn/interface/ethernet",
     "lan/vpn/interface/gre",
     "lan/vpn/interface/ipsec",
     "lan/vpn/interface/multilink",
     "lan/vpn/interface/svi",
@@ -92,20 +98,22 @@
     "unified/ssl-decryption",
     "unified/url-filtering",
     "wan/vpn",
     "wan/vpn/interface/cellular",
     "wan/vpn/interface/dsl-ipoe",
     "wan/vpn/interface/dsl-pppoa",
     "wan/vpn/interface/dsl-pppoe",
-    "wan/vpn/interface/eth-pppoe",
     "wan/vpn/interface/ethernet",
     "wan/vpn/interface/gre",
     "wan/vpn/interface/multilink",
+    "traffic-policy",
     "wan/vpn/interface/serial",
     "wirelesslan",
+    "cellular-profile",
+    "wan/vpn/interface/ethpppoe",
 ]
 
 
 AnyParcel = Annotated[
     Union[
         AnySystemParcel,
         AnyPolicyObjectParcel,
@@ -114,23 +122,24 @@
         AnyTransportParcel,
         AnyEmbeddedSecurityParcel,
         AnyCliParcel,
         AnyDnsSecurityParcel,
         AnySIGSecurityParcel,
         AnyApplicationPriorityParcel,
         AnyTopologyParcel,
+        AnyRoutingParcel,
     ],
     Field(discriminator="type_"),
 ]
 
 T = TypeVar("T", bound=AnyParcel)
 
 
 class Parcel(BaseModel, Generic[T]):
-    parcel_id: str = Field(alias="parcelId")
+    parcel_id: Union[str, UUID] = Field(alias="parcelId")
     parcel_type: ParcelType = Field(alias="parcelType")
     created_by: str = Field(alias="createdBy")
     last_updated_by: str = Field(alias="lastUpdatedBy")
     created_on: int = Field(alias="createdOn")
     last_updated_on: int = Field(alias="lastUpdatedOn")
     payload: T
 
@@ -166,13 +175,25 @@
     model_config = ConfigDict(populate_by_name=True)
 
     id: UUID = Field(serialization_alias="parcelId", validation_alias="parcelId")
 
 
 class ParcelAssociationPayload(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
     parcel_id: UUID = Field(serialization_alias="parcelId", validation_alias="parcelId")
 
 
 class ParcelId(BaseModel):
-    id: str = Field(alias="parcelId")
+    model_config = ConfigDict(populate_by_name=True)
+    id: UUID = Field(serialization_alias="parcelId", validation_alias="parcelId")
+
+
+@lru_cache
+def list_types(any_union: T) -> Sequence[T]:
+    return cast(Sequence[T], resolve_nested_base_model_unions(any_union))
+
+
+@lru_cache
+def find_type(name: str, any_union: T) -> T:
+    parcel_types = list_types(any_union)
+    parcel_type = next(t for t in parcel_types if t._get_parcel_type() == name)
+    return cast(T, parcel_type)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/policy_settings.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/application_priority/qos_policy.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, Variable, _ParcelBase
 from catalystwan.models.configuration.feature_profile.common import RefIdItem
 
 
-class Target(BaseModel):
+class QosPolicyTarget(BaseModel):
     model_config = ConfigDict(populate_by_name=True, extra="forbid")
     interfaces: Union[Global[List[str]], Variable]
 
 
 class QosSchedulers(BaseModel):
     model_config = ConfigDict(populate_by_name=True, extra="forbid")
     bandwidth_percent: Optional[Global[str]] = Field(
@@ -29,8 +29,8 @@
     model_config = ConfigDict(populate_by_name=True, extra="forbid")
     qos_schedulers: List[QosSchedulers] = Field(validation_alias="qosSchedulers", serialization_alias="qosSchedulers")
 
 
 class QosPolicyParcel(_ParcelBase):
     type_: Literal["qos-policy"] = Field(default="qos-policy", exclude=True)
     qos_map: QosMap = Field(validation_alias=AliasPath("data", "qosMap"))
-    target: Optional[Target] = Field(default=None, validation_alias=AliasPath("data", "target"))
+    target: Optional[QosPolicyTarget] = Field(default=None, validation_alias=AliasPath("data", "target"))
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/dns_security/dns.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/ngfirewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/embedded_security/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 from typing import List, Literal, Union
 from uuid import UUID
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, Variable, _ParcelBase
-from catalystwan.models.configuration.feature_profile.sdwan.transport.bgp import RefIdItem
+from catalystwan.models.configuration.feature_profile.common import RefIdItem
 
 PredefinedZone = Literal["self", "default", "untrusted"]
 SettingOn = Literal["on"]
 FailureMode = Literal["close", "open"]
 
 
 class AppHosting(BaseModel):
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/other/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 
 from .policy.app_probe import AppProbeMapItem, AppProbeParcel
 from .policy.application_list import ApplicationFamilyListEntry, ApplicationListEntry, ApplicationListParcel
 from .policy.as_path import AsPathParcel
 from .policy.color_list import ColorEntry, ColorParcel
 from .policy.data_prefix import DataPrefixEntry, DataPrefixParcel
 from .policy.expanded_community_list import ExpandedCommunityParcel
+from .policy.extended_community import ExtendedCommunityParcel
 from .policy.fowarding_class import FowardingClassParcel, FowardingClassQueueEntry
 from .policy.ipv6_data_prefix import IPv6DataPrefixEntry, IPv6DataPrefixParcel
 from .policy.ipv6_prefix_list import IPv6PrefixListEntry, IPv6PrefixListParcel
 from .policy.mirror import MirrorParcel
 from .policy.policer import PolicerEntry, PolicerParcel
 from .policy.prefered_group_color import Preference, PreferredColorGroupEntry, PreferredColorGroupParcel
 from .policy.prefix_list import PrefixListEntry, PrefixListParcel
-from .policy.sla_class import FallbackBestTunnel, SLAAppProbeClass, SLAClassCriteria, SLAClassListEntry, SLAClassParcel
+from .policy.sla_class import SLAClassListEntry, SLAClassParcel
 from .policy.standard_community import StandardCommunityEntry, StandardCommunityParcel
 from .policy.tloc_list import TlocEntry, TlocParcel
 from .security.aip import AdvancedInspectionProfileParcel
 from .security.amp import AdvancedMalwareProtectionParcel
 from .security.application_list import (
     SecurityApplicationFamilyListEntry,
     SecurityApplicationListEntry,
@@ -41,21 +42,21 @@
 from .security.url import BaseURLListEntry, URLAllowParcel, URLBlockParcel, URLParcel
 from .security.zone import SecurityZoneListEntry, SecurityZoneListParcel
 
 AnyPolicyObjectParcel = Annotated[
     Union[
         AdvancedInspectionProfileParcel,
         AdvancedMalwareProtectionParcel,
-        URLParcel,
         ApplicationListParcel,
         AppProbeParcel,
         AsPathParcel,
         ColorParcel,
         DataPrefixParcel,
         ExpandedCommunityParcel,
+        ExtendedCommunityParcel,
         FowardingClassParcel,
         FQDNDomainParcel,
         GeoLocationListParcel,
         IntrusionPreventionParcel,
         IPSSignatureParcel,
         IPv6DataPrefixParcel,
         IPv6PrefixListParcel,
@@ -70,14 +71,15 @@
         SecurityPortParcel,
         SecurityZoneListParcel,
         SLAClassParcel,
         SslDecryptionParcel,
         SslDecryptionProfileParcel,
         StandardCommunityParcel,
         TlocParcel,
+        URLParcel,
     ],
     Field(discriminator="type_"),
 ]
 
 __all__ = (
     "AdvancedInspectionProfileParcel",
     "AdvancedMalwareProtectionParcel",
@@ -91,14 +93,15 @@
     "AsPathParcel",
     "BaseURLListEntry",
     "ColorEntry",
     "ColorParcel",
     "DataPrefixEntry",
     "DataPrefixParcel",
     "ExpandedCommunityParcel",
+    "ExtendedCommunityParcel",
     "FallbackBestTunnel",
     "FowardingClassParcel",
     "FowardingClassQueueEntry",
     "FQDNDomainParcel",
     "FQDNListEntry",
     "GeoLocationListEntry",
     "GeoLocationListParcel",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/color_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/expanded_community_list.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 
 class ExpandedCommunityParcel(_ParcelBase):
     type_: Literal["expanded-community"] = Field(default="expanded-community", exclude=True)
     model_config = ConfigDict(populate_by_name=True)
     expanded_community_list: Global[List[str]] = Field(
         default=Global[List[str]](value=list()),
-        serialization_alias="expandedCommunityList",
         validation_alias=AliasPath("data", "expandedCommunityList"),
     )
 
     def add_community(self, expanded_community: str):
         self.expanded_community_list.value.append(expanded_community)
 
     @field_validator("expanded_community_list")
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/fowarding_class.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/ipv6_prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/mirror.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import List, Literal
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
+from pydantic.networks import IPvAnyAddress
 
-from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
+from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
 
 
 class MirrorEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
     remote_dest_ip: Global[str] = Field(validation_alias="remoteDestIp", serialization_alias="remoteDestIp")
     source_ip: Global[str] = Field(validation_alias="sourceIp", serialization_alias="sourceIp")
 
 
 class MirrorParcel(_ParcelBase):
     type_: Literal["mirror"] = Field(default="mirror", exclude=True)
-    entries: List[MirrorEntry] = Field(validation_alias=AliasPath("data", "entries"), min_length=1, max_length=1)
+    entries: List[MirrorEntry] = Field(
+        default=[], validation_alias=AliasPath("data", "entries"), min_length=1, max_length=1
+    )
+
+    @classmethod
+    def create(cls, remote_dest_ip: IPvAnyAddress, source_ip: IPvAnyAddress, *args, **kwargs):
+        entry = MirrorEntry(remote_dest_ip=as_global(str(remote_dest_ip)), source_ip=as_global(str(source_ip)))
+        return cls(entries=[entry], *args, **kwargs)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefered_group_color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/prefix_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/sla_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase, as_global
+from catalystwan.models.configuration.feature_profile.common import RefIdItem
 
 SLAClassCriteria = Literal[
     "loss",
     "latency",
     "jitter",
     "loss-latency",
     "loss-jitter",
@@ -40,20 +41,14 @@
 
 def check_jitter_ms(cls, jitter: Optional[Global]):
     if jitter is not None:
         assert 1 <= jitter.value <= 1000
     return jitter
 
 
-class SLAAppProbeClass(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
-
-    ref_id: Global[UUID] = Field(serialization_alias="refId", validation_alias="refId")
-
-
 class FallbackBestTunnel(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     criteria: Global[SLAClassCriteria]
     jitter_variance: Optional[Global[int]] = Field(
         default=None,
         serialization_alias="jitterVariance",
@@ -97,16 +92,16 @@
 
 class SLAClassListEntry(BaseModel):
     model_config = ConfigDict(populate_by_name=True)
 
     latency: Optional[Global[int]] = None
     loss: Optional[Global[int]] = None
     jitter: Optional[Global[int]] = None
-    app_probe_class: Optional[SLAAppProbeClass] = Field(
-        validation_alias="appProbeClass", serialization_alias="appProbeClass"
+    app_probe_class: Optional[RefIdItem] = Field(
+        default=None, validation_alias="appProbeClass", serialization_alias="appProbeClass"
     )
     fallback_best_tunnel: Optional[FallbackBestTunnel] = Field(
         default=None, validation_alias="fallbackBestTunnel", serialization_alias="fallbackBestTunnel"
     )
 
     # validators
     _jitter_validator = field_validator("jitter")(check_jitter_ms)
@@ -116,22 +111,23 @@
 
 class SLAClassParcel(_ParcelBase):
     type_: Literal["sla-class"] = Field(default="sla-class", exclude=True)
     entries: List[SLAClassListEntry] = Field(default=[], validation_alias=AliasPath("data", "entries"))
 
     def add_entry(
         self,
-        app_probe_class_id: UUID,
+        app_probe_class_id: Optional[UUID] = None,
         loss: Optional[int] = None,
         jitter: Optional[int] = None,
         latency: Optional[int] = None,
     ):
+        ref = RefIdItem(ref_id=as_global(str(app_probe_class_id))) if app_probe_class_id is not None else None
         self.entries.append(
             SLAClassListEntry(
-                app_probe_class=SLAAppProbeClass(ref_id=as_global(app_probe_class_id)),
+                app_probe_class=ref,
                 loss=as_global(loss) if loss is not None else None,
                 jitter=as_global(jitter) if jitter is not None else None,
                 latency=as_global(latency) if latency is not None else None,
             )
         )
 
     def add_fallback(
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/standard_community.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/policy/tloc_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/aip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import Literal
 
 from pydantic import AliasPath, Field
 
 from catalystwan.api.configuration_groups.parcel import Global, _ParcelBase
-from catalystwan.models.configuration.feature_profile.sdwan.transport.bgp import RefIdItem
+from catalystwan.models.configuration.feature_profile.common import RefIdItem
 
 TlsDecryptionAction = Literal["decrypt", "neverDecrypt", "skipDecrypt"]
 
 
 class AdvancedInspectionProfileParcel(_ParcelBase):
     type_: Literal["unified/advanced-inspection-profile"] = Field(
         default="unified/advanced-inspection-profile", exclude=True
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/application_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/fqdn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/geolocation_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/protocol_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/security_port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/ssl_decryption_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/policy_object/security/zone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,90 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
+
 from typing import List, Union
 
 from pydantic import Field
 from typing_extensions import Annotated
 
-from .acl import Ipv4AclParcel, Ipv6AclParcel
-from .appqoe import AppqoeParcel
-from .dhcp_server import LanVpnDhcpServerParcel
-from .eigrp import EigrpParcel
-from .lan.ethernet import InterfaceEthernetParcel
-from .lan.gre import InterfaceGreParcel
-from .lan.ipsec import InterfaceIpsecParcel
-from .lan.multilink import InterfaceMultilinkParcel
-from .lan.svi import InterfaceSviParcel
-from .lan.vpn import LanVpnParcel
-from .multicast import MulticastParcel
-from .ospf import OspfParcel
-from .ospfv3 import Ospfv3IPv4Parcel, Ospfv3IPv6Parcel
-from .route_policy import RoutePolicyParcel
-from .switchport import SwitchportParcel
-from .wireless_lan import WirelessLanParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl import AnyAclParcel
 
-AnyTopLevelServiceParcel = Annotated[
-    Union[
-        LanVpnDhcpServerParcel,
-        AppqoeParcel,
-        LanVpnParcel,
-        OspfParcel,
-        Ospfv3IPv4Parcel,
-        Ospfv3IPv6Parcel,
-        RoutePolicyParcel,
-        EigrpParcel,
-        SwitchportParcel,
-        Ipv6AclParcel,
-        Ipv4AclParcel,
-        WirelessLanParcel,
-        MulticastParcel,
-        # TrackerGroupData,
-        # WirelessLanData,
-        # SwitchportData
-    ],
-    Field(discriminator="type_"),
-]
+from .cellular_controller import CellularControllerParcel
+from .cellular_profile import CellularProfileParcel
+from .gps import GpsParcel
+from .management.ethernet import InterfaceEthernetParcel as ManagementInterfaceEthernetParcel
+from .t1e1controller import T1E1ControllerParcel
+from .vpn import ManagementVpnParcel, TransportVpnParcel
+from .wan.interface.ethernet import InterfaceEthernetParcel
+from .wan.interface.gre import InterfaceGreParcel
+from .wan.interface.ipsec import InterfaceIpsecParcel
+from .wan.interface.multilink import InterfaceMultilinkParcel
+from .wan.interface.protocol_over import (
+    InterfaceDslIPoEParcel,
+    InterfaceDslPPPoAParcel,
+    InterfaceDslPPPoEParcel,
+    InterfaceEthPPPoEParcel,
+)
+from .wan.interface.t1e1serial import T1E1SerialParcel
 
-AnyLanVpnInterfaceParcel = Annotated[
+AnyTransportVpnSubParcel = Annotated[
     Union[
-        InterfaceEthernetParcel,
+        T1E1SerialParcel,
+        InterfaceEthPPPoEParcel,
+        InterfaceDslPPPoEParcel,
+        InterfaceDslPPPoAParcel,
+        InterfaceDslIPoEParcel,
         InterfaceGreParcel,
         InterfaceIpsecParcel,
-        InterfaceSviParcel,
+        InterfaceEthernetParcel,
         InterfaceMultilinkParcel,
+        # Add wan interfaces here
     ],
     Field(discriminator="type_"),
 ]
-
-AnyAssociatoryParcel = Annotated[
+AnyTransportVpnParcel = Annotated[Union[ManagementVpnParcel, TransportVpnParcel], Field(discriminator="type_")]
+AnyTransportSuperParcel = Annotated[
     Union[
-        MulticastParcel,
-        # DHCP
+        T1E1ControllerParcel,
+        CellularControllerParcel,
+        CellularProfileParcel,
+        T1E1ControllerParcel,
+        GpsParcel,
     ],
     Field(discriminator="type_"),
 ]
+AnyManagementVpnSubParcel = Annotated[
+    Union[ManagementInterfaceEthernetParcel],
+    Field(discriminator="type_"),
+]
 
-AnyServiceParcel = Annotated[
-    Union[AnyTopLevelServiceParcel, AnyLanVpnInterfaceParcel],
+AnyTransportParcel = Annotated[
+    Union[
+        AnyAclParcel,
+        AnyTransportSuperParcel,
+        AnyTransportVpnParcel,
+        AnyTransportVpnSubParcel,
+        AnyManagementVpnSubParcel,
+    ],
     Field(discriminator="type_"),
 ]
 
 __all__ = [
-    "LanVpnDhcpServerParcel",
-    "AppqoeParcel",
-    "LanVpnParcel",
-    "OspfParcel",
-    "RoutePolicyParcel",
-    "Ospfv3IPv4Parcel",
-    "Ospfv3IPv6Parcel",
-    "Ipv6AclParcel",
-    "Ipv4AclParcel",
-    "SwitchportParcel",
-    "InterfaceSviParcel",
-    "InterfaceGreParcel",
-    "WirelessLanParcel",
-    "MulticastParcel",
-    "AnyServiceParcel",
-    "AnyTopLevelServiceParcel",
-    "AnyLanVpnInterfaceParcel",
+    "RoutingBgpParcel",
+    "CellularControllerParcel",
+    "ManagementVpnParcel",
+    "TransportVpnParcel",
+    "AnyTransportParcel",
+    "AnyTransportSuperParcel",
+    "AnyTransportVpnSubParcel",
+    "AnyManagementVpnSubParcel",
+    "T1E1ControllerParcel",
+    "T1E1SerialParcel",
+    "InterfaceDslPPPoAParcel",
+    "InterfaceDslPPPoEParcel",
+    "InterfaceEthPPPoEParcel",
+    "InterfaceIpsecParcel",
 ]
 
 
 def __dir__() -> "List[str]":
     return list(__all__)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/acl.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospfv3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,442 +1,295 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
-from __future__ import annotations
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address, IPv6Address, IPv6Interface
+from ipaddress import IPv4Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
+from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, _ParcelBase, as_default
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
+from catalystwan.models.common import MetricType
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask
+
+NetworkType = Literal[
+    "broadcast",
+    "point-to-point",
+    "non-broadcast",
+    "point-to-multipoint",
+]
+
+NoAuthType = Literal["no-auth"]
+IpsecSha1AuthType = Literal["ipsec-sha1"]
 
-Action = Literal["drop", "accept"]
-Icmp6Msg = Literal[
-    "beyond-scope",
-    "cp-advertisement",
-    "cp-solicitation",
-    "destination-unreachable",
-    "dhaad-reply",
-    "dhaad-request",
-    "echo-reply",
-    "echo-request",
-    "header",
-    "hop-limit",
-    "ind-advertisement",
-    "ind-solicitation",
-    "mld-query",
-    "mld-reduction",
-    "mld-report",
-    "mldv2-report",
-    "mpd-advertisement",
-    "mpd-solicitation",
-    "mr-advertisement",
-    "mr-solicitation",
-    "mr-termination",
-    "nd-na",
-    "nd-ns",
-    "next-header-type",
-    "ni-query",
-    "ni-query-name",
-    "ni-query-v4-address",
-    "ni-query-v6-address",
-    "ni-response",
-    "ni-response-qtype-unknown",
-    "ni-response-refuse",
-    "ni-response-success",
-    "no-admin",
-    "no-route",
-    "packet-too-big",
-    "parameter-option",
-    "parameter-problem",
-    "port-unreachable",
-    "reassembly-timeout",
-    "redirect",
-    "reject-route",
-    "renum-command",
-    "renum-result",
-    "renum-seq-number",
-    "router-advertisement",
-    "router-renumbering",
-    "router-solicitation",
-    "rpl-control",
-    "source-policy",
-    "source-route-header",
-    "time-exceeded",
-    "unreachable",
+MaxMetricRouterLsaAction = Literal[
+    "disabled",
+    "immediately",
+    "on-startup",
 ]
-IcmpMsg = Literal[
-    "administratively-prohibited",
-    "dod-host-prohibited",
-    "dod-net-prohibited",
-    "echo",
-    "echo-reply",
-    "echo-reply-no-error",
-    "extended-echo",
-    "extended-echo-reply",
-    "general-parameter-problem",
-    "host-isolated",
-    "host-precedence-unreachable",
-    "host-redirect",
-    "host-tos-redirect",
-    "host-tos-unreachable",
-    "host-unknown",
-    "host-unreachable",
-    "interface-error",
-    "malformed-query",
-    "multiple-interface-match",
-    "net-redirect",
-    "net-tos-redirect",
-    "net-tos-unreachable",
-    "net-unreachable",
-    "network-unknown",
-    "no-room-for-option",
-    "option-missing",
-    "packet-too-big",
-    "parameter-problem",
-    "photuris",
-    "port-unreachable",
-    "precedence-unreachable",
-    "protocol-unreachable",
-    "reassembly-timeout",
-    "redirect",
-    "router-advertisement",
-    "router-solicitation",
-    "source-route-failed",
-    "table-entry-error",
-    "time-exceeded",
-    "timestamp-reply",
-    "timestamp-request",
-    "ttl-exceeded",
-    "unreachable",
+
+RedistributeProtocol = Literal[
+    "static",
+    "connected",
+    "bgp",
+    "omp",
+    "nat-route",
+    "eigrp",
 ]
-Tcp = Literal["syn"]
 
+RedistributeProtocolIPv6 = Literal[
+    "static",
+    "connected",
+    "bgp",
+    "omp",
+    "eigrp",
+]
 
-class ReferenceId(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    ref_id: Global[UUID] = Field(..., serialization_alias="refId", validation_alias="refId")
 
+class NoAuth(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class SourceDataPrefixListReference(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    source_data_prefix_list: ReferenceId = Field(
-        ...,
-        serialization_alias="sourceDataPrefixList",
-        validation_alias="sourceDataPrefixList",
-        description="Source Data Prefix Parcel",
+    auth_type: Union[Global[NoAuthType], Default[NoAuthType]] = Field(
+        serialization_alias="authType",
+        validation_alias="authType",
+        default=Default[NoAuthType](value="no-auth"),
     )
 
 
-class SourceDataPrefixIp(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    source_ip_prefix: Global[str] = Field(
-        ...,
-        serialization_alias="sourceIpPrefix",
-        validation_alias="sourceIpPrefix",
-        description="Source Data IP Prefix",
+class IpsecSha1Auth(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    auth_type: Global[IpsecSha1AuthType] = Field(
+        serialization_alias="authType",
+        validation_alias="authType",
+        default=Global[IpsecSha1AuthType](value="ipsec-sha1"),
     )
+    spi: Union[Global[int], Variable]
+    auth_key: Union[Global[str], Variable] = Field(serialization_alias="authKey", validation_alias="authKey")
 
 
-class SourcePort(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+class Ospfv3InterfaceParametres(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    name: Optional[Union[Global[str], Variable]] = Field(serialization_alias="ifName", validation_alias="ifName")
+    hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="helloInterval", validation_alias="helloInterval", default=None
     )
-    source_port: Union[Global[int], Global[str]] = Field(
-        ...,
-        serialization_alias="sourcePort",
-        validation_alias="sourcePort",
-        description="source port range or individual port number",
+    dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="deadInterval", validation_alias="deadInterval", default=None
     )
-
-
-class DestinationDataPrefixListReference(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    retransmit_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="retransmitInterval", validation_alias="retransmitInterval", default=None
     )
-    destination_data_prefix_list: ReferenceId = Field(
-        ...,
-        serialization_alias="destinationDataPrefixList",
-        validation_alias="destinationDataPrefixList",
-        description="Destination Data Prefix Parcel",
+    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
+    priority: Optional[Union[Global[int], Variable, Default[int]]] = None
+    network_type: Optional[Union[Global[NetworkType], Variable, Default[None]]] = Field(
+        serialization_alias="networkType", validation_alias="networkType", default=None
     )
-
-
-class DestinationDataPrefixIp(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    passive_interface: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="passiveInterface", validation_alias="passiveInterface", default=None
     )
-    destination_ip_prefix: Global[IPv6Interface] = Field(
-        ...,
-        serialization_alias="destinationIpPrefix",
-        validation_alias="destinationIpPrefix",
-        description="Destination Data IP Prefix",
+    authentication_config: Optional[Union[NoAuth, IpsecSha1Auth]] = Field(
+        serialization_alias="authenticationConfig", validation_alias="authenticationConfig", default=None
     )
 
 
-class DestinationPort(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    destination_port: Union[Global[int], Global[str]] = Field(
-        ...,
-        serialization_alias="destinationPort",
-        validation_alias="destinationPort",
-        description="destination port range or individual port number",
+class SummaryRouteIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    network: Union[Global[str], Global[IPv6Interface], Variable]
+    no_advertise: Union[Global[bool], Variable, Default[bool]] = Field(
+        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=Default[bool](value=False)
     )
+    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
 
 
-class Ipv4MatchEntry(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    dscp: Optional[Global[List[int]]] = Field(default=None, description="DSCP number")
-    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
-        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
-    )
-    protocol: Optional[Global[List[int]]] = Field(
-        default=None, description="protocol number list with at least one item"
-    )
-    icmp_msg: Optional[IcmpMsg] = Field(
-        default=None, serialization_alias="icmpMsg", validation_alias="icmpMsg", description="ICMP Message"
-    )
-    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
-        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
-    )
-    source_ports: Optional[List[SourcePort]] = Field(
-        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
-    )
-    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
-        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
-    )
-    destination_ports: Optional[List[DestinationPort]] = Field(
-        default=None,
-        serialization_alias="destinationPorts",
-        validation_alias="destinationPorts",
-        description="Destination Port List",
+class SummaryRoute(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    network: Optional[AddressWithMask] = None
+    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
+    no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=as_default(False)
     )
-    tcp: Optional[Tcp] = Field(default=None, description="TCP States")
 
 
-class Ipv6MatchEntry(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    next_header: Optional[Global[int]] = Field(
-        default=None, serialization_alias="nextHeader", validation_alias="nextHeader", description="next header number"
-    )
-    packet_length: Optional[Union[Global[int], Global[str]]] = Field(
-        default=None, serialization_alias="packetLength", validation_alias="packetLength", description="Packet Length"
-    )
-    source_data_prefix: Optional[Union[SourceDataPrefixListReference, SourceDataPrefixIp]] = Field(
-        default=None, serialization_alias="sourceDataPrefix", validation_alias="sourceDataPrefix"
-    )
-    source_ports: Optional[List[SourcePort]] = Field(
-        default=None, serialization_alias="sourcePorts", validation_alias="sourcePorts", description="Source Port List"
+class StubArea(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    area_type: Global[str] = Field(
+        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="stub")
     )
-    destination_data_prefix: Optional[Union[DestinationDataPrefixListReference, DestinationDataPrefixIp]] = Field(
-        default=None, serialization_alias="destinationDataPrefix", validation_alias="destinationDataPrefix"
+    no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
-    destination_ports: Optional[List[DestinationPort]] = Field(
-        default=None,
-        serialization_alias="destinationPorts",
-        validation_alias="destinationPorts",
-        description="Destination Port List",
+
+
+class NssaArea(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    area_type: Global[str] = Field(
+        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="nssa")
     )
-    tcp: Optional[Global[Tcp]] = Field(default=None, description="TCP States")
-    traffic_class: Optional[Global[List[int]]] = Field(
-        default=None,
-        serialization_alias="trafficClass",
-        validation_alias="trafficClass",
-        description="Select Traffic Class",
+    no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="noSummary", validation_alias="noSummary", default=None
     )
-    icmp6_msg: Optional[Global[List[Icmp6Msg]]] = Field(
-        default=None, serialization_alias="icmp6Msg", validation_alias="icmp6Msg", description="ICMP6 Message"
+    always_translate: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="alwaysTranslate", validation_alias="alwaysTranslate", default=None
     )
 
 
-class Ipv4AcceptAction(BaseModel):
-    """
-    Accept Action
-    """
+class NormalArea(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    area_type: Global[str] = Field(
+        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="normal")
     )
-    set_dscp: Optional[Global[int]] = Field(
-        default=None, serialization_alias="setDscp", validation_alias="setDscp", description="DSCP number"
-    )
-    counter_name: Optional[Global[str]] = Field(
-        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
+
+
+class DefaultArea(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    area_type: Default[None] = Field(
+        serialization_alias="areaType", validation_alias="areaType", default=Default[None](value=None)
     )
-    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
-    set_next_hop: Optional[Global[IPv4Address]] = Field(
-        default=None,
-        serialization_alias="setNextHop",
-        validation_alias="setNextHop",
-        description="Set Next Hop (IPV4 address)",
+
+
+class Ospfv3IPv4Area(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
+    area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
+        serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
-    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
+    ranges: Optional[List[SummaryRoute]] = None
 
 
-class Ipv6AcceptAction(BaseModel):
-    """
-    Accept Action
-    """
+class Ospfv3IPv6Area(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
+    area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
+        serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
     )
-    counter_name: Optional[Global[str]] = Field(
-        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
+    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
+    ranges: Optional[List[SummaryRouteIPv6]] = None
+
+
+class MaxMetricRouterLsa(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    action: Global[MaxMetricRouterLsaAction]
+    on_startup_time: Optional[Union[Global[int], Variable]] = Field(
+        serialization_alias="onStartUpTime", validation_alias="onStartUpTime", default=None
     )
-    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
-    set_next_hop: Optional[Global[IPv6Address]] = Field(
-        default=None,
-        serialization_alias="setNextHop",
-        validation_alias="setNextHop",
-        description="Set Next Hop (IPV6 address)",
+
+
+class RedistributedRoute(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    protocol: Union[Global[RedistributeProtocol], Variable]
+    nat_dia: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="natDia", validation_alias="natDia", default=None
     )
-    set_traffic_class: Optional[Global[int]] = Field(
-        default=None,
-        serialization_alias="setTrafficClass",
-        validation_alias="setTrafficClass",
-        description="set traffic class number",
+    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
+        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
-    mirror: Optional[ReferenceId] = Field(default=None, description="Select a Mirror Parcel UUID")
-    policer: Optional[ReferenceId] = Field(default=None, description="Select a Policer Parcel")
 
 
-class Ipv4AcceptActions(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+class RedistributedRouteIPv6(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    protocol: Union[Global[RedistributeProtocolIPv6], Variable]
+    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
+        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
-    accept: Ipv4AcceptAction = Field(..., description="Accept Action")
 
 
-class Ipv6AcceptActions(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+class DefaultOriginate(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    originate: Union[Global[bool], Default[bool]]
+    always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
+    metric: Optional[Union[Global[str], Variable, Default[None]]] = None
+    metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
+        default=None, serialization_alias="metricType", validation_alias="metricType"
     )
-    accept: Ipv6AcceptAction = Field(..., description="Accept Action")
 
 
-class DropAction(BaseModel):
-    """
-    Drop Action
-    """
+class SpfTimers(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
+    delay: Optional[Union[Global[int], Variable, Default[int]]] = None
+    initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=None, validation_alias="initialHold", serialization_alias="initialHold"
     )
-    counter_name: Optional[Global[str]] = Field(
-        default=None, serialization_alias="counterName", validation_alias="counterName", description="Counter Name"
+    max_hold: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        default=None, validation_alias="maxHold", serialization_alias="maxHold"
     )
-    log: Union[Global[bool], Default[bool]] = Field(default=as_default(False), description="Enable log")
 
 
-class DropActions(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    drop: DropAction = Field(..., description="Drop Action")
+class AdvancedOspfv3Attributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-
-class Sequences(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    sequence_id: Global[int] = Field(
-        ..., serialization_alias="sequenceId", validation_alias="sequenceId", description="Sequence Id"
+    reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
     )
-    sequence_name: Global[str] = Field(
-        ..., serialization_alias="sequenceName", validation_alias="sequenceName", description="Sequence Name"
+    compatible_rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
+        serialization_alias="compatibleRfc1583", validation_alias="compatibleRfc1583", default=None
     )
-    base_action: Optional[Union[Global[Action], Default[Action]]] = Field(
-        default=None, serialization_alias="baseAction", validation_alias="baseAction", description="Base Action"
+    default_originate: Optional[DefaultOriginate] = Field(
+        serialization_alias="defaultOriginate", validation_alias="defaultOriginate", default=None
     )
-    match_entries: Optional[List[Ipv6MatchEntry]] = Field(
-        default=None,
-        serialization_alias="matchEntries",
-        validation_alias="matchEntries",
-        description="Define match conditions",
-        max_length=1,
-        min_length=1,
+    spf_timers: Optional[SpfTimers] = Field(serialization_alias="spfTimers", validation_alias="spfTimers", default=None)
+    policy_name: Optional[Union[Default[None], Global[UUID]]] = Field(
+        serialization_alias="policyName", validation_alias="policyName", default=None
     )
+    filter: Optional[Union[Global[bool], Variable, Default[bool]]] = None
 
-    @model_validator(mode="after")
-    def check_fields_at_least_one_assigned(self):
-        """There are two Sequence models in schema,
-        one with set base_action and empty actions,
-        and one with set actions and empty base_action,
-        so we combine two models into one model with check if
-        at least one field assigned
-        """
-        if self.base_action is None and self.actions is None:
-            self.base_action = as_default("accept", Action)
 
+class BasicOspfv3Attributes(BaseModel):
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-class Ipv6Sequences(Sequences):
-    actions: Optional[List[Union[Ipv6AcceptActions, DropActions]]] = Field(
-        default=None, description="Define list of actions", max_length=1, min_length=1
+    router_id: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = Field(
+        serialization_alias="routerId", validation_alias="routerId", default=None
     )
-
-
-class Ipv4Sequences(Sequences):
-    actions: Optional[List[Union[Ipv4AcceptActions, DropActions]]] = Field(
-        default=None, description="Define list of actions", max_length=1, min_length=1
+    distance: Optional[Union[Global[int], Variable, Default[int]]] = None
+    external_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="externalDistance", validation_alias="externalDistance", default=None
+    )
+    inter_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="interAreaDistance", validation_alias="interAreaDistance", default=None
+    )
+    intra_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
+        serialization_alias="intraAreaDistance", validation_alias="intraAreaDistance", default=None
     )
 
 
-class Ipv4AclParcel(_ParcelBase):
-    type_: Literal["ipv4-acl"] = Field(default="ipv4-acl", exclude=True)
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    default_action: Union[Global[Action], Global[Action]] = Field(
-        as_default("drop", Action),
-        validation_alias=AliasPath("data", "defaultAction"),
-        description="Default Action",
+class RoutingOspfv3IPv4Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv4"] = Field(default="routing/ospfv3/ipv4", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRoute]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
     )
-    sequences: List[Union[Ipv4Sequences]] = Field(
-        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
+    max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
+    area: List[Ospfv3IPv4Area] = Field(validation_alias=AliasPath("data", "area"))
 
 
-class Ipv6AclParcel(_ParcelBase):
-    type_: Literal["ipv6-acl"] = Field(default="ipv6-acl", exclude=True)
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    default_action: Union[Global[Action], Global[Action]] = Field(
-        as_default("drop", Action),
-        validation_alias=AliasPath("data", "defaultAction"),
-        description="Default Action",
+class RoutingOspfv3IPv6Parcel(_ParcelBase):
+    type_: Literal["routing/ospfv3/ipv6"] = Field(default="routing/ospfv3/ipv6", exclude=True)
+    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+
+    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
+    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
+    redistribute: Optional[List[RedistributedRouteIPv6]] = Field(
+        default=None, validation_alias=AliasPath("data", "redistribute")
     )
-    sequences: List[Union[Ipv6Sequences]] = Field(
-        default_factory=list, validation_alias=AliasPath("data", "sequences"), description="Access Control List"
+    max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
+        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
     )
+    area: List[Ospfv3IPv6Area] = Field(validation_alias=AliasPath("data", "area"))
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/bgp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/dhcp_server.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/multilink.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
 
 class InterfaceMultilinkParcel(_ParcelBase):
     model_config = ConfigDict(
         extra="forbid",
         populate_by_name=True,
     )
-    type_: Literal["lan/vpn/interface/multilink/"] = Field(
-        default="lan/vpn/interface/multilink/", frozen=True, exclude=True
+    type_: Literal["lan/vpn/interface/multilink"] = Field(
+        default="lan/vpn/interface/multilink", frozen=True, exclude=True
     )
 
     group_number: Union[Global[int], Variable] = Field(validation_alias=AliasPath("data", "groupNumber"))
     if_name: Union[Global[str], Variable] = Field(validation_alias=AliasPath("data", "ifName"))
     method: Union[Global[MultilinkMethod], Default[None]] = Field(validation_alias=AliasPath("data", "method"))
     address_ipv4: Optional[Union[Global[IPv4Address], Default[None], Variable]] = Field(
         default=None, validation_alias=AliasPath("data", "addressIpv4")
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/lan/vpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
-from pydantic import AliasPath, BaseModel, ConfigDict, Field, IPvAnyAddress
+from pydantic import AliasPath, BaseModel, ConfigDict, Field, field_validator
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
-from catalystwan.models.configuration.feature_profile.common import AddressWithMask
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, DNSIPv4, DNSIPv6, HostMapping
 
 ProtocolIPv4 = Literal[
     "bgp",
     "ospf",
     "opsfv3",
     "connected",
     "static",
@@ -90,49 +90,14 @@
 
 RedistributeToGlobalProtocol = Literal[
     "bgp",
     "ospf",
 ]
 
 
-class DnsIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    primary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        default=Default[None](value=None),
-        serialization_alias="primaryDnsAddressIpv4",
-        validation_alias="primaryDnsAddressIpv4",
-    )
-    secondary_dns_address_ipv4: Union[Variable, Global[str], Default[None]] = Field(
-        default=Default[None](value=None),
-        serialization_alias="secondaryDnsAddressIpv4",
-        validation_alias="secondaryDnsAddressIpv4",
-    )
-
-
-class DnsIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    primary_dns_address_ipv6: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="primaryDnsAddressIpv6", validation_alias="primaryDnsAddressIpv6"
-    )
-    secondary_dns_address_ipv6: Union[Variable, Global[str], Default[None]] = Field(
-        serialization_alias="secondaryDnsAddressIpv6", validation_alias="secondaryDnsAddressIpv6"
-    )
-
-
-class HostMapping(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    host_name: Union[Variable, Global[str]] = Field(serialization_alias="hostName", validation_alias="hostName")
-    list_of_ip: Union[Variable, Global[List[IPvAnyAddress]]] = Field(
-        serialization_alias="listOfIp", validation_alias="listOfIp"
-    )
-
-
 class RoutePrefix(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     ip_address: Union[Variable, Global[str], Global[IPv4Address], Global[IPv6Address]] = Field(
         serialization_alias="ipAddress", validation_alias="ipAddress"
     )
     subnet_mask: Union[Variable, Global[str]] = Field(serialization_alias="subnetMask", validation_alias="subnetMask")
@@ -236,16 +201,14 @@
 
     next_hop_container: NextHopIPv6Container = Field(
         serialization_alias="nextHopContainer", validation_alias="nextHopContainer"
     )
 
 
 class Null0(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
     null0: Union[Global[bool], Default[bool]] = Default[bool](value=True)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
 
 
 class Null0IPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
@@ -255,23 +218,19 @@
 class NAT(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     nat: Union[Variable, Global[NATRoute]]
 
 
 class DHCP(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
     dhcp: Union[Global[bool], Default[bool]] = Default[bool](value=True)
 
 
 class StaticRouteVPN(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
-
-    vpn: Union[Global[bool], Default[bool]] = Default[bool](value=True)
+    vpn: Union[Global[bool], Default[bool]] = Field(default=Default[bool](value=True))
 
 
 class NextHopInterfaceRoute(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     address: Union[Variable, Global[str], Default[None]] = Default[None](value=None)
     distance: Union[Variable, Global[int], Default[int]] = Default[int](value=1)
@@ -333,21 +292,35 @@
 
     interface_container: InterfaceIPv6Container = Field(
         serialization_alias="interfaceContainer", validation_alias="interfaceContainer"
     )
 
 
 class StaticRouteIPv4(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
+    model_config = ConfigDict(populate_by_name=True)
 
     prefix: RoutePrefix
     one_of_ip_route: Union[NextHopRouteContainer, Null0, DHCP, StaticRouteVPN, InterfaceRouteContainer] = Field(
         serialization_alias="oneOfIpRoute", validation_alias="oneOfIpRoute"
     )
 
+    @field_validator("one_of_ip_route", mode="before")
+    @classmethod
+    def validate_one_of_ip_route(
+        cls, value: Union[dict, NextHopRouteContainer, Null0, DHCP, StaticRouteVPN, InterfaceRouteContainer]
+    ):
+        # https://github.com/pydantic/pydantic/issues/6830
+        # For some reason the Null0 is always created from dict
+        if isinstance(value, dict):
+            if value.get("vpn"):
+                return StaticRouteVPN(**value)
+            if value.get("nextHopContainer"):
+                return NextHopRouteContainer(**value)
+        return value
+
 
 class StaticRouteIPv6(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True)
 
     prefix: RoutePrefix
     one_of_ip_route: Union[NextHopRouteIPv6Container, Null0IPv6, NAT, InterfaceRouteIPv6Container] = Field(
         serialization_alias="oneOfIpRoute", validation_alias="oneOfIpRoute"
@@ -589,16 +562,16 @@
     )
     omp_admin_distance_ipv4: Optional[Union[Variable, Global[int], Default[None]]] = Field(
         validation_alias=AliasPath("data", "ompAdminDistance"), default=None
     )
     omp_admin_distance_ipv6: Optional[Union[Variable, Global[int], Default[None]]] = Field(
         validation_alias=AliasPath("data", "ompAdminDistanceIpv6"), default=None
     )
-    dns_ipv4: Optional[DnsIPv4] = Field(validation_alias=AliasPath("data", "dnsIpv4"), default=None)
-    dns_ipv6: Optional[DnsIPv6] = Field(validation_alias=AliasPath("data", "dnsIpv6"), default=None)
+    dns_ipv4: Optional[DNSIPv4] = Field(validation_alias=AliasPath("data", "dnsIpv4"), default=None)
+    dns_ipv6: Optional[DNSIPv6] = Field(validation_alias=AliasPath("data", "dnsIpv6"), default=None)
     new_host_mapping: Optional[List[HostMapping]] = Field(
         validation_alias=AliasPath("data", "newHostMapping"), default=None
     )
     omp_advertise_ipv4: Optional[List[OmpAdvertiseIPv4]] = Field(
         validation_alias=AliasPath("data", "ompAdvertiseIp4"), default=None  # API typo
     )
     omp_advertise_ipv6: Optional[List[OmpAdvertiseIPv6]] = Field(
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/object_tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospf.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/ospf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from ipaddress import IPv4Address
 from typing import List, Literal, Optional, Union
 from uuid import UUID
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
@@ -112,15 +113,15 @@
     protocol: Union[Global[RedistributeProtocolOspf], Variable]
     dia: Optional[Union[Global[bool], Variable, Default[bool]]] = None
     route_policy: Optional[Union[Default[None], Global[str], Global[UUID]]] = Field(
         serialization_alias="routePolicy", validation_alias="routePolicy", default=None
     )
 
 
-class OspfParcel(_ParcelBase):
+class RoutingOspfParcel(_ParcelBase):
     type_: Literal["routing/ospf"] = Field(default="routing/ospf", exclude=True)
     model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
     router_id: Union[Global[str], Global[IPv4Address], Variable, Default[None]] = Field(
         validation_alias=AliasPath("data", "routerId"), default=Default[None](value=None)
     )
     reference_bandwidth: Union[Global[int], Variable, Default[int]] = Field(
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/ospfv3.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/protocol_over.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,291 +1,405 @@
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
-from ipaddress import IPv4Address, IPv6Interface
-from typing import List, Literal, Optional, Union
-from uuid import UUID
+# This file is named PPPoX, because it contains different Point-To-Point Protocol Interfaces.
+
+from __future__ import annotations
+
+from typing import Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
-from catalystwan.models.common import MetricType
-from catalystwan.models.configuration.feature_profile.common import AddressWithMask
+from catalystwan.models.common import CarrierType, TLOCColor, TunnelMode
+from catalystwan.models.configuration.feature_profile.common import (
+    AclQos,
+    AddressWithMask,
+    AllowService,
+    MultiRegionFabric,
+)
 
-NetworkType = Literal[
-    "broadcast",
-    "point-to-point",
-    "non-broadcast",
-    "point-to-multipoint",
-]
 
-NoAuthType = Literal["no-auth"]
-IpsecSha1AuthType = Literal["ipsec-sha1"]
+class NatProp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    nat: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(default=None)
+    tcp_timeout: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="tcpTimeout", serialization_alias="tcpTimeout"
+    )
+    udp_timeout: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="udpTimeout", serialization_alias="udpTimeout"
+    )
 
-MaxMetricRouterLsaAction = Literal[
-    "disabled",
-    "immediately",
-    "on-startup",
-]
 
-RedistributeProtocol = Literal[
-    "static",
-    "connected",
-    "bgp",
-    "omp",
-    "nat-route",
-    "eigrp",
-]
+class Ethernet(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    if_name: Union[Variable, Global[str]] = Field(validation_alias="ifName", serialization_alias="ifName")
+    description: Optional[Union[Variable, Global[str], Default[None]]] = Field(default=None)
+    vlan_id: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="vlanId", serialization_alias="vlanId"
+    )
 
-RedistributeProtocolIPv6 = Literal[
-    "static",
-    "connected",
-    "bgp",
-    "omp",
-    "eigrp",
+
+Method = Literal[
+    "chap",
+    "pap",
+    "papandchap",
 ]
 
 
-class NoAuth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+class Chap(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    hostname: Union[Variable, Global[str]] = Field()
+    ppp_auth_password: Union[Variable, Global[str]] = Field(
+        validation_alias="pppAuthPassword", serialization_alias="pppAuthPassword"
+    )
 
-    auth_type: Union[Global[NoAuthType], Default[NoAuthType]] = Field(
-        serialization_alias="authType",
-        validation_alias="authType",
-        default=Default[NoAuthType](value="no-auth"),
+
+class Pap(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    ppp_auth_password: Union[Variable, Global[str]] = Field(
+        validation_alias="pppAuthPassword", serialization_alias="pppAuthPassword"
     )
+    username: Union[Variable, Global[str]] = Field()
 
 
-class IpsecSha1Auth(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+Callin = Literal[
+    "Bidirectional",
+    "Unidirectional",
+]
 
-    auth_type: Global[IpsecSha1AuthType] = Field(
-        serialization_alias="authType",
-        validation_alias="authType",
-        default=Global[IpsecSha1AuthType](value="ipsec-sha1"),
-    )
-    spi: Union[Global[int], Variable]
-    auth_key: Union[Global[str], Variable] = Field(serialization_alias="authKey", validation_alias="authKey")
 
+class Ppp(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    dial_pool_number: Union[Variable, Global[int]] = Field(
+        validation_alias="dialPoolNumber", serialization_alias="dialPoolNumber"
+    )
+    method: Union[Global[Method], Default[None]] = Field()
+    callin: Optional[Union[Variable, Global[Callin], Default[None]]] = Field(default=None)
+    chap: Optional[Chap] = Field(default=None, description="CHAP Attributes")
+    pap: Optional[Pap] = Field(default=None, description="PAP Attributes")
+    ppp_max_payload: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="pppMaxPayload", serialization_alias="pppMaxPayload"
+    )
 
-class Ospfv3InterfaceParametres(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    name: Optional[Union[Global[str], Variable]] = Field(serialization_alias="ifName", validation_alias="ifName")
-    hello_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="helloInterval", validation_alias="helloInterval", default=None
+class Tunnel(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    dead_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="deadInterval", validation_alias="deadInterval", default=None
+    bandwidth_percent: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="bandwidthPercent", serialization_alias="bandwidthPercent"
     )
-    retransmit_interval: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="retransmitInterval", validation_alias="retransmitInterval", default=None
+    border: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(default=None)
+    clear_dont_fragment: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="clearDontFragment", serialization_alias="clearDontFragment"
     )
-    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
-    priority: Optional[Union[Global[int], Variable, Default[int]]] = None
-    network_type: Optional[Union[Global[NetworkType], Variable, Default[None]]] = Field(
-        serialization_alias="networkType", validation_alias="networkType", default=None
+    color: Optional[Union[Global[TLOCColor], Default[Literal["default"]], Variable]] = Field(default=None)
+    exclude_controller_group_list: Optional[Union[Variable, Global[str], Default[None]]] = Field(
+        default=None, validation_alias="excludeControllerGroupList", serialization_alias="excludeControllerGroupList"
     )
-    passive_interface: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="passiveInterface", validation_alias="passiveInterface", default=None
+    group: Optional[Union[Variable, Global[str], Default[None]]] = Field(default=None)
+    low_bandwidth_link: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="lowBandwidthLink", serialization_alias="lowBandwidthLink"
     )
-    authentication_config: Optional[Union[NoAuth, IpsecSha1Auth]] = Field(
-        serialization_alias="authenticationConfig", validation_alias="authenticationConfig", default=None
+    max_control_connections: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="maxControlConnections", serialization_alias="maxControlConnections"
     )
-
-
-class SummaryRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    network: Union[Global[str], Global[IPv6Interface], Variable]
-    no_advertise: Union[Global[bool], Variable, Default[bool]] = Field(
-        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=Default[bool](value=False)
+    mode: Optional[Union[Variable, Global[TunnelMode]]] = Field(default=None)
+    network_broadcast: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="networkBroadcast", serialization_alias="networkBroadcast"
     )
-    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
-
-
-class SummaryRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    network: Optional[AddressWithMask] = None
-    cost: Optional[Union[Global[int], Variable, Default[None]]] = None
-    no_advertise: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="noAdvertise", validation_alias="noAdvertise", default=None
+    per_tunnel_qos: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="perTunnelQos", serialization_alias="perTunnelQos"
+    )
+    port_hop: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="portHop", serialization_alias="portHop"
+    )
+    restrict: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(default=None)
+    tunnel_interface: Optional[Union[Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="tunnelInterface", serialization_alias="tunnelInterface"
+    )
+    tunnel_tcp_mss_adjust: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="tunnelTcpMssAdjust", serialization_alias="tunnelTcpMssAdjust"
+    )
+    vbond_as_stun_server: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="vbondAsStunServer", serialization_alias="vbondAsStunServer"
+    )
+    vmanage_connection_preference: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="vmanageConnectionPreference", serialization_alias="vmanageConnectionPreference"
     )
 
 
-class StubArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    area_type: Global[str] = Field(
-        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="stub")
+class TunnelAdvancedOption(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="noSummary", validation_alias="noSummary", default=None
+    bind: Optional[Union[Variable, Global[str], Default[None]]] = Field(default=None)
+    carrier: Optional[Union[Variable, Default[Literal["default"]], Global[CarrierType]]] = Field(default=None)
+    gre_encap: Optional[Union[Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="greEncap", serialization_alias="greEncap"
+    )
+    gre_preference: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="grePreference", serialization_alias="grePreference"
+    )
+    gre_weight: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="greWeight", serialization_alias="greWeight"
+    )
+    hello_interval: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="helloInterval", serialization_alias="helloInterval"
+    )
+    hello_tolerance: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="helloTolerance", serialization_alias="helloTolerance"
+    )
+    ipsec_encap: Optional[Union[Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="ipsecEncap", serialization_alias="ipsecEncap"
+    )
+    ipsec_preference: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="ipsecPreference", serialization_alias="ipsecPreference"
+    )
+    ipsec_weight: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="ipsecWeight", serialization_alias="ipsecWeight"
+    )
+    last_resort_circuit: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="lastResortCircuit", serialization_alias="lastResortCircuit"
+    )
+    nat_refresh_interval: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="natRefreshInterval", serialization_alias="natRefreshInterval"
     )
 
 
-class NssaArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    area_type: Global[str] = Field(
-        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="nssa")
+class Advanced(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    no_summary: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="noSummary", validation_alias="noSummary", default=None
+    ip_directed_broadcast: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias="ipDirectedBroadcast", serialization_alias="ipDirectedBroadcast"
     )
-    always_translate: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="alwaysTranslate", validation_alias="alwaysTranslate", default=None
+    ip_mtu: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="ipMtu", serialization_alias="ipMtu"
+    )
+    tcp_mss: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias="tcpMss", serialization_alias="tcpMss"
+    )
+    tloc_extension: Optional[Union[Variable, Global[str], Default[None]]] = Field(
+        default=None, validation_alias="tlocExtension", serialization_alias="tlocExtension"
     )
 
 
-class NormalArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    area_type: Global[str] = Field(
-        serialization_alias="areaType", validation_alias="areaType", default=Global[str](value="normal")
-    )
+VdslMode = Literal[
+    "ADSL1",
+    "ADSL2",
+    "ADSL2+",
+    "ANSI",
+    "VDSL2",
+]
 
 
-class DefaultArea(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+class Vdsl(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    slot: Union[Variable, Global[str]] = Field()
+    mode: Optional[Union[Variable, Global[VdslMode], Default[Literal["auto"]]]] = Field(default=None)
+    sra: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(default=None)
 
-    area_type: Default[None] = Field(
-        serialization_alias="areaType", validation_alias="areaType", default=Default[None](value=None)
-    )
 
+AtmEncapsulation = Literal[
+    "AAL5MUX",
+    "AAL5NLPID",
+    "AAL5SNAP",
+]
 
-class Ospfv3IPv4Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
-    area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
-        serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
+class VbrNrtConfig(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
-    ranges: Optional[List[SummaryRoute]] = None
-
+    burst_cell_size: Union[Variable, Global[int]] = Field(
+        validation_alias="burstCellSize", serialization_alias="burstCellSize"
+    )
+    p_c_r: Union[Variable, Global[int]] = Field(validation_alias="pCR", serialization_alias="pCR")
+    s_c_r: Union[Variable, Global[int]] = Field(validation_alias="sCR", serialization_alias="sCR")
 
-class Ospfv3IPv6Area(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    area_number: Union[Global[int], Variable] = Field(serialization_alias="areaNum", validation_alias="areaNum")
-    area_type_config: Optional[Union[StubArea, NssaArea, NormalArea, DefaultArea]] = Field(
-        serialization_alias="areaTypeConfig", validation_alias="areaTypeConfig", default=None
+class VbrRtConfig(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    interfaces: List[Ospfv3InterfaceParametres] = Field(min_length=1)
-    ranges: Optional[List[SummaryRouteIPv6]] = None
-
+    a_c_r: Union[Variable, Global[int]] = Field(validation_alias="aCR", serialization_alias="aCR")
+    burst_cell_size: Union[Variable, Global[int]] = Field(
+        validation_alias="burstCellSize", serialization_alias="burstCellSize"
+    )
+    p_c_r: Union[Variable, Global[int]] = Field(validation_alias="pCR", serialization_alias="pCR")
 
-class MaxMetricRouterLsa(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    action: Global[MaxMetricRouterLsaAction]
-    on_startup_time: Optional[Union[Global[int], Variable]] = Field(
-        serialization_alias="onStartUpTime", validation_alias="onStartUpTime", default=None
+class AtmInterface(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    if_name: Union[Variable, Global[str]] = Field(validation_alias="ifName", serialization_alias="ifName")
+    local_vpi_vci: Union[Variable, Global[str]] = Field(
+        validation_alias="localVpiVci", serialization_alias="localVpiVci"
+    )
+    description: Optional[Union[Variable, Global[str], Default[None]]] = Field(default=None)
+    encapsulation: Optional[Union[Default[Literal["AAL5MUX"]], Global[AtmEncapsulation]]] = Field(default=None)
+    vbr_nrt_config: Optional[VbrNrtConfig] = Field(
+        default=None, validation_alias="vbrNrtConfig", serialization_alias="vbrNrtConfig", description="VBR-NRT config"
+    )
+    vbr_rt_config: Optional[VbrRtConfig] = Field(
+        default=None, validation_alias="vbrRtConfig", serialization_alias="vbrRtConfig", description="VBR-NRT config"
     )
 
 
-class RedistributedRoute(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    protocol: Union[Global[RedistributeProtocol], Variable]
-    nat_dia: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="natDia", validation_alias="natDia", default=None
+class Dynamic(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
-        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
+    dhcp_helper: Optional[Union[Variable, Global[str], Default[None]]] = Field(
+        default=None, validation_alias="dhcpHelper", serialization_alias="dhcpHelper"
+    )
+    dynamic_dhcp_distance: Optional[Union[Variable, Default[int], Global[int]]] = Field(
+        default=None, validation_alias="dynamicDhcpDistance", serialization_alias="dynamicDhcpDistance"
     )
 
 
-class RedistributedRouteIPv6(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    protocol: Union[Global[RedistributeProtocolIPv6], Variable]
-    route_policy: Optional[Union[Default[None], Global[UUID]]] = Field(
-        serialization_alias="routePolicy", validation_alias="routePolicy", default=None
+class Static(BaseModel):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    static_ip_v4: Optional[AddressWithMask] = Field(
+        default=None,
+        validation_alias="staticIpV4AddressPrimary",
+        serialization_alias="staticIpV4AddressPrimary",
+        description="Static IpV4Address Primary",
     )
 
 
-class DefaultOriginate(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+class DynamicIntfIpAddress(BaseModel):
+    dynamic: Dynamic = Field()
 
-    originate: Union[Global[bool], Default[bool]]
-    always: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-    metric: Optional[Union[Global[str], Variable, Default[None]]] = None
-    metric_type: Optional[Union[Global[MetricType], Variable, Default[None]]] = Field(
-        default=None, serialization_alias="metricType", validation_alias="metricType"
-    )
 
+class StaticIntfIpAddress(BaseModel):
+    static: Static = Field()
 
-class SpfTimers(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    delay: Optional[Union[Global[int], Variable, Default[int]]] = None
-    initial_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
-    max_hold: Optional[Union[Global[int], Variable, Default[int]]] = None
 
+class IPoEEthernet(Ethernet):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
+    )
+    intf_ip_address: Union[DynamicIntfIpAddress, StaticIntfIpAddress] = Field(
+        validation_alias="intfIpAddress", serialization_alias="intfIpAddress"
+    )
 
-class AdvancedOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    reference_bandwidth: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="referenceBandwidth", validation_alias="referenceBandwidth", default=None
+class InterfaceBase(_ParcelBase):
+    model_config = ConfigDict(
+        extra="forbid",
+        populate_by_name=True,
     )
-    compatible_rfc1583: Optional[Union[Global[bool], Variable, Default[bool]]] = Field(
-        serialization_alias="compatibleRfc1583", validation_alias="compatibleRfc1583", default=None
+    acl_qos: Optional[AclQos] = Field(default=None, validation_alias=AliasPath("data", "aclQos"), description="ACL/QOS")
+    advanced: Optional[Advanced] = Field(
+        default=None, validation_alias=AliasPath("data", "advanced"), description="Advanced Attributes"
     )
-    default_originate: Optional[DefaultOriginate] = Field(
-        serialization_alias="defaultOriginate", validation_alias="defaultOriginate", default=None
+    bandwidth_downstream: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias=AliasPath("data", "bandwidthDownstream")
     )
-    spf_timers: Optional[SpfTimers] = Field(serialization_alias="spfTimers", validation_alias="spfTimers", default=None)
-    policy_name: Optional[Union[Default[None], Global[UUID]]] = Field(
-        serialization_alias="policyName", validation_alias="policyName", default=None
+    bandwidth_upstream: Optional[Union[Variable, Global[int], Default[None]]] = Field(
+        default=None, validation_alias=AliasPath("data", "bandwidthUpstream")
     )
-    filter: Optional[Union[Global[bool], Variable, Default[bool]]] = None
-
-
-class BasicOspfv3Attributes(BaseModel):
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
-
-    router_id: Optional[Union[Global[str], Global[IPv4Address], Variable, Default[None]]] = Field(
-        serialization_alias="routerId", validation_alias="routerId", default=None
+    multi_region_fabric: Optional[MultiRegionFabric] = Field(
+        default=None, validation_alias=AliasPath("data", "multiRegionFabric"), description="Multi-Region Fabric"
+    )
+    nat_prop: Optional[NatProp] = Field(
+        default=None, validation_alias=AliasPath("data", "natProp"), description="NAT Attributes"
     )
-    distance: Optional[Union[Global[int], Variable, Default[int]]] = None
-    external_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="externalDistance", validation_alias="externalDistance", default=None
+    ppp: Optional[Ppp] = Field(default=None, validation_alias=AliasPath("data", "ppp"), description="PPP Attributes")
+    service_provider: Optional[Union[Variable, Global[str], Default[None]]] = Field(
+        default=None, validation_alias=AliasPath("data", "serviceProvider")
     )
-    inter_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="interAreaDistance", validation_alias="interAreaDistance", default=None
+    shutdown: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
+        default=None, validation_alias=AliasPath("data", "shutdown")
     )
-    intra_area_distance: Optional[Union[Global[int], Variable, Default[int]]] = Field(
-        serialization_alias="intraAreaDistance", validation_alias="intraAreaDistance", default=None
+    tunnel: Optional[Tunnel] = Field(
+        default=None, validation_alias=AliasPath("data", "tunnel"), description="Tunnel Interface Attributes"
     )
+    tunnel_advanced_option: Optional[TunnelAdvancedOption] = Field(
+        default=None, validation_alias=AliasPath("data", "tunnelAdvancedOption")
+    )
+    tunnel_allow_service: Optional[AllowService] = Field(
+        default=None,
+        validation_alias=AliasPath("data", "tunnelAllowService"),
+        description="Tunnel Interface Attributes",
+    )
+
 
+class InterfaceEthPPPoEParcel(InterfaceBase):
+    type_: Literal["wan/vpn/interface/ethpppoe"] = Field(
+        default="wan/vpn/interface/ethpppoe", frozen=True, exclude=True
+    )
+    ethernet: Optional[Ethernet] = Field(
+        default=None,
+        validation_alias=AliasPath("data", "ethernet"),
+        description="Ethernet Interface Attributes applicable for both ethppoe/ipoe",
+    )
 
-class Ospfv3IPv4Parcel(_ParcelBase):
-    type_: Literal["routing/ospfv3/ipv4"] = Field(default="routing/ospfv3/ipv4", exclude=True)
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
 
-    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
-    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
-    redistribute: Optional[List[RedistributedRoute]] = Field(
-        default=None, validation_alias=AliasPath("data", "redistribute")
+class InterfaceDslPPPoEParcel(InterfaceBase):
+    type_: Literal["wan/vpn/interface/dsl-pppoe"] = Field(
+        default="wan/vpn/interface/dsl-pppoe", frozen=True, exclude=True
     )
-    max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
+    vdsl: Optional[Vdsl] = Field(default=None, validation_alias=AliasPath("data", "vdsl"), description="vdsl")
+    ethernet: Optional[Ethernet] = Field(
+        default=None,
+        validation_alias=AliasPath("data", "ethernet"),
+        description="Ethernet Interface Attributes applicable for both ethppoe/ipoe",
     )
-    area: List[Ospfv3IPv4Area] = Field(validation_alias=AliasPath("data", "area"))
 
 
-class Ospfv3IPv6Parcel(_ParcelBase):
-    type_: Literal["routing/ospfv3/ipv6"] = Field(default="routing/ospfv3/ipv6", exclude=True)
-    model_config = ConfigDict(arbitrary_types_allowed=True, populate_by_name=True, extra="forbid")
+class InterfaceDslPPPoAParcel(InterfaceBase):
+    type_: Literal["wan/vpn/interface/dsl-pppoa"] = Field(
+        default="wan/vpn/interface/dsl-pppoa", frozen=True, exclude=True
+    )
+    atm_interface: Optional[AtmInterface] = Field(
+        default=None, validation_alias=AliasPath("data", "atmInterface"), description="ATM Interface attributes"
+    )
+    vdsl: Optional[Vdsl] = Field(default=None, validation_alias=AliasPath("data", "vdsl"), description="vdsl")
 
-    basic: Optional[BasicOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "basic"))
-    advanced: Optional[AdvancedOspfv3Attributes] = Field(default=None, validation_alias=AliasPath("data", "advanced"))
-    redistribute: Optional[List[RedistributedRouteIPv6]] = Field(
-        default=None, validation_alias=AliasPath("data", "redistribute")
+
+class InterfaceDslIPoEParcel(InterfaceBase):
+    type_: Literal["wan/vpn/interface/dsl-ipoe"] = Field(
+        default="wan/vpn/interface/dsl-ipoe", frozen=True, exclude=True
+    )
+    ethernet: Optional[IPoEEthernet] = Field(
+        default=None,
+        validation_alias=AliasPath("data", "ethernet"),
+        description="Ethernet Interface Attributes for ipoe",
     )
-    max_metric_router_lsa: Optional[MaxMetricRouterLsa] = Field(
-        validation_alias=AliasPath("data", "maxMetricRouterLsa"), default=None
+    vdsl: Optional[Vdsl] = Field(
+        default=None,
+        validation_alias=AliasPath("data", "vdsl"),
+        description="vdsl",
     )
-    area: List[Ospfv3IPv6Area] = Field(validation_alias=AliasPath("data", "area"))
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/service_insertion_attachment.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/tracker.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/service/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/sig_security/sig_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pydantic import Field
 from typing_extensions import Annotated
 
 from .aaa import AAAParcel
 from .banner import BannerParcel
 from .basic import BasicParcel
 from .bfd import BFDParcel
+from .device_access import DeviceAccessIPv4Parcel
+from .device_access_ipv6 import DeviceAccessIPv6Parcel
 from .global_parcel import GlobalParcel
 from .logging_parcel import LoggingParcel
 from .mrf import MRFParcel
 from .ntp import NtpParcel
 from .omp import OMPParcel
 from .security import SecurityParcel
 from .snmp import SNMPParcel
@@ -18,14 +20,16 @@
 AnySystemParcel = Annotated[
     Union[
         AAAParcel,
         BFDParcel,
         LoggingParcel,
         BannerParcel,
         BasicParcel,
+        DeviceAccessIPv4Parcel,
+        DeviceAccessIPv6Parcel,
         GlobalParcel,
         NtpParcel,
         MRFParcel,
         OMPParcel,
         SecurityParcel,
         SNMPParcel,
     ],
@@ -34,14 +38,16 @@
 
 __all__ = [
     "AAAParcel",
     "BFDParcel",
     "LoggingParcel",
     "BannerParcel",
     "BasicParcel",
+    "DeviceAccessIPv4Parcel",
+    "DeviceAccessIPv6Parcel",
     "GlobalParcel",
     "NtpParcel",
     "MRFParcel",
     "OMPParcel",
     "SecurityParcel",
     "SNMPParcel",
     "AnySystemParcel",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/global_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/logging_parcel.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/mrf.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/security.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/system/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/custom_control.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/hubspoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/topology/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/bgp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/routing/bgp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from __future__ import annotations
 
 from ipaddress import IPv4Address, IPv6Address
 from typing import List, Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_variable
-from catalystwan.models.common import SubnetMask
-from catalystwan.models.configuration.feature_profile.common import RefIdItem
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, RefIdItem
 
 FamilyType = Literal["ipv4-unicast", "vpnv4-unicast", "vpnv6-unicast"]
 FamilyTypeIpv6 = Literal["ipv6-unicast", "vpnv6-unicast"]
 PolicyTypeOff = Literal["off"]
 PolicyTypeRestart = Literal["restart"]
 PolicyTypeWarningDisablePeer = Literal["warning-only", "disable-peer"]
 Protocol = Literal["static", "connected", "ospf", "ospfv3", "nat"]
@@ -356,63 +356,37 @@
         serialization_alias="addressFamily",
         validation_alias="addressFamily",
         description="Set IPv6 BGP address family",
         max_length=2,
     )
 
 
-class Prefix(BaseModel):
-    """
-    Configure the IPv4 prefixes to aggregate
-    """
-
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    address: Union[Variable, Global[IPv4Address]]
-    mask: Union[Variable, Global[SubnetMask]]
-
-
 class AggregateAddres(BaseModel):
     model_config = ConfigDict(
         extra="forbid",
         populate_by_name=True,
     )
-    prefix: Prefix = Field(..., description="Configure the IPv4 prefixes to aggregate")
+    prefix: AddressWithMask = Field(..., description="Configure the IPv4 prefixes to aggregate")
     as_set: Optional[Union[Variable, Global[bool], Default[Literal[False]]]] = Field(
         default=None, serialization_alias="asSet", validation_alias="asSet", description="Set AS set path information"
     )
     summary_only: Optional[Union[Variable, Global[bool], Default[Literal[False]]]] = Field(
         default=None,
         serialization_alias="summaryOnly",
         validation_alias="summaryOnly",
         description="Variable out more specific routes from updates",
     )
 
 
-class Prefix1(BaseModel):
-    """
-    Configure the prefixes for BGP to announce
-    """
-
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    address: Union[Variable, Global[IPv4Address]]
-    mask: Union[Variable, Global[SubnetMask]]
-
-
 class NetworkItem(BaseModel):
     model_config = ConfigDict(
         extra="forbid",
         populate_by_name=True,
     )
-    prefix: Prefix1 = Field(..., description="Configure the prefixes for BGP to announce")
+    prefix: AddressWithMask = Field(..., description="Configure the prefixes for BGP to announce")
 
 
 class RedistributeItem(BaseModel):
     model_config = ConfigDict(
         extra="forbid",
         populate_by_name=True,
     )
@@ -543,22 +517,21 @@
         populate_by_name=True,
     )
     if_name: Union[Global[str], Variable] = Field(
         ..., serialization_alias="ifName", validation_alias="ifName", description="Interface Name"
     )
 
 
-class WanRoutingBgpParcel(_ParcelBase):
-    type_: Literal["bgp"] = Field(default="bgp", exclude=True)
+class RoutingBgpParcel(_ParcelBase):
+    type_: Literal["routing/bgp"] = Field(default="routing/bgp", exclude=True)
     model_config = ConfigDict(
         extra="forbid",
         populate_by_name=True,
     )
     as_num: Union[Global[int], Global[str], Variable] = Field(
-        default=as_variable("{{lbgp_1_basicConf_asNumber}}"),
         validation_alias=AliasPath("data", "asNum"),
         description="Set autonomous system number <1..4294967295> or <XX.YY>",
     )
     router_id: Optional[Union[Global[IPv4Address], Variable, Default[None]]] = Field(
         default=None,
         validation_alias=AliasPath("data", "routerId"),
         description="Configure BGP router identifier",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# Copyright 2024 Cisco Systems, Inc. and its affiliates
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 
 from typing import Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
 
 ConfigTypeValue = Literal["non-eSim"]
 
 
 class ControllerConfig(BaseModel):
     model_config = ConfigDict(extra="forbid", populate_by_name=True)
     id: Union[Variable, Global[str]] = Field(description="Cellular ID", examples=["0/2/0"])
-    slot: Optional[Union[Variable, Global[int], Default[int]]] = Field(default=None, description="Set primary SIM slot")
+    slot: Optional[Union[Variable, Global[int], Default[int]]] = Field(
+        default=None, description="Set primary SIM slot. 0 or 1"
+    )
     max_retry: Optional[Union[Variable, Global[int], Default[None]]] = Field(
         default=None,
         description="Set SIM failover retries",
         serialization_alias="maxRetry",
         validation_alias="maxRetry",
     )
     failover_timer: Optional[Union[Variable, Global[int], Default[None]]] = Field(
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/cellular_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 # Copyright 2024 Cisco Systems, Inc. and its affiliates
 
 from typing import Literal, Optional, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field, model_validator
 
-from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase
+from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
 
 AuthenticationType = Literal[
     "chap",
     "pap",
     "pap_chap",
 ]
 
@@ -62,9 +63,9 @@
 
 
 class CellularProfileParcel(_ParcelBase):
     model_config = ConfigDict(extra="forbid", populate_by_name=True)
     type_: Literal["cellular-profile"] = Field(default="cellular-profile", exclude=True, frozen=True)
     profile_config: ProfileConfig = Field(validation_alias=AliasPath("data", "profileConfig"))
     config_type: Optional[Default[Literal["non-eSim"]]] = Field(
-        default=None, validation_alias=AliasPath("data", "configType")
+        default=as_default("non-eSim"), validation_alias=AliasPath("data", "configType")
     )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/gps.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/management/ethernet.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     interface_description: Union[Variable, Global[str], Default[None]] = Field(
         default=Default[None](value=None), validation_alias=AliasPath("data", "description")
     )
     intf_ip_address: Union[InterfaceDynamicIPv4Address, InterfaceStaticIPv4Address] = Field(
         validation_alias=AliasPath("data", "intfIpAddress")
     )
     shutdown: Union[Variable, Global[bool], Default[bool]] = Field(
-        default=Default[bool](value=False), validation_alias=AliasPath("data", "shutdown")
+        default=Default[bool](value=True), validation_alias=AliasPath("data", "shutdown")
     )
     arp: Optional[List[Arp]] = Field(
         default=None, validation_alias=AliasPath("data", "arp"), description="Configure ARP entries"
     )
     auto_detect_bandwidth: Optional[Union[Variable, Global[bool], Default[bool]]] = Field(
         default=None, validation_alias=AliasPath("data", "autoDetectBandwidth")
     )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/t1e1controller.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/vpn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,27 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from ipaddress import IPv4Address, IPv6Address, IPv6Interface
 from typing import Iterator, List, Literal, Optional, Tuple, Union
 
 from pydantic import AliasPath, BaseModel, ConfigDict, Field
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, _ParcelBase, as_default
 from catalystwan.models.common import SubnetMask
+from catalystwan.models.configuration.feature_profile.common import DNSIPv4, DNSIPv6, HostMapping
 
 Gateway = Literal["nextHop", "dhcp", "null0"]
 Nat = Literal["NAT64", "NAT66"]
 ServiceType = Literal["TE"]
 
 UnitIPv4Address = Union[Variable, Global[IPv4Address]]
 UnitDistance = Union[Variable, Global[int]]
 
 RouteHop = Union[Tuple[UnitIPv4Address, UnitDistance], UnitIPv4Address]
 
 
-class DnsIpv4(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    primary_dns_address_ipv4: Optional[Union[Variable, Global[IPv4Address], Default[None]]] = Field(
-        default=None,
-        serialization_alias="primaryDnsAddressIpv4",
-        validation_alias="primaryDnsAddressIpv4",
-        description="Primary DNS Address (IPv4)",
-    )
-    secondary_dns_address_ipv4: Optional[Union[Variable, Global[IPv4Address], Default[None]]] = Field(
-        default=None,
-        serialization_alias="secondaryDnsAddressIpv4",
-        validation_alias="secondaryDnsAddressIpv4",
-        description="Secondary DNS Address (IPv4)",
-    )
-
-
-class DnsIpv6(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    primary_dns_address_ipv6: Optional[Union[Variable, Global[IPv6Address], Default[None]]] = Field(
-        default=None,
-        serialization_alias="primaryDnsAddressIpv6",
-        validation_alias="primaryDnsAddressIpv6",
-        description="Primary DNS Address (IPv6)",
-    )
-    secondary_dns_address_ipv6: Optional[Union[Variable, Global[IPv6Address], Default[None]]] = Field(
-        default=None,
-        serialization_alias="secondaryDnsAddressIpv6",
-        validation_alias="secondaryDnsAddressIpv6",
-        description="Secondary DNS Address (IPv6)",
-    )
-
-
-class NewHostMappingItem(BaseModel):
-    model_config = ConfigDict(
-        extra="forbid",
-        populate_by_name=True,
-    )
-    host_name: Union[Variable, Global[str]] = Field(
-        ..., serialization_alias="hostName", validation_alias="hostName", description="Hostname"
-    )
-    list_of_ip: Union[Variable, Global[List[str]]] = Field(
-        ..., serialization_alias="listOfIp", validation_alias="listOfIp", description="List of IP"
-    )
-
-
 class Prefix(BaseModel):
     """
     Prefix
     """
 
     model_config = ConfigDict(
         extra="forbid",
@@ -217,17 +168,17 @@
     type_: Literal["management/vpn"] = Field(default="management/vpn", exclude=True)
     vpn_id: Default[int] = Field(
         default=as_default(512),
         validation_alias=AliasPath("data", "vpnId"),
         frozen=True,
         description="Management VPN, which will always be 512",
     )
-    dns_ipv4: Optional[DnsIpv4] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv4"))
-    dns_ipv6: Optional[DnsIpv6] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv6"))
-    new_host_mapping: Optional[List[NewHostMappingItem]] = Field(
+    dns_ipv4: Optional[DNSIPv4] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv4"))
+    dns_ipv6: Optional[DNSIPv6] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv6"))
+    new_host_mapping: Optional[List[HostMapping]] = Field(
         default=None, validation_alias=AliasPath("data", "newHostMapping")
     )
     ipv4_route: List[Ipv4RouteItem] = Field(
         default_factory=list, validation_alias=AliasPath("data", "ipv4Route"), description="IPv4 Static Route"
     )
     ipv6_route: List[Ipv6RouteItem] = Field(
         default_factory=list, validation_alias=AliasPath("data", "ipv6Route"), description="IPv6 Static Route"
@@ -242,17 +193,17 @@
     type_: Literal["wan/vpn"] = Field(default="wan/vpn", exclude=True)
     vpn_id: Default[int] = Field(
         default=as_default(0),
         validation_alias=AliasPath("data", "vpnId"),
         frozen=True,
         description="Transport VPN, which will always be 0",
     )
-    dns_ipv4: Optional[DnsIpv4] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv4"))
-    dns_ipv6: Optional[DnsIpv6] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv6"))
-    new_host_mapping: Optional[List[NewHostMappingItem]] = Field(
+    dns_ipv4: Optional[DNSIPv4] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv4"))
+    dns_ipv6: Optional[DNSIPv6] = Field(default=None, validation_alias=AliasPath("data", "dnsIpv6"))
+    new_host_mapping: Optional[List[HostMapping]] = Field(
         default=None, validation_alias=AliasPath("data", "newHostMapping")
     )
     ipv4_route: List[Ipv4RouteItem] = Field(
         default_factory=list, validation_alias=AliasPath("data", "ipv4Route"), description="IPv4 Static Route"
     )
     ipv6_route: List[Ipv6RouteItem] = Field(
         default_factory=list, validation_alias=AliasPath("data", "ipv6Route"), description="IPv6 Static Route"
@@ -268,29 +219,29 @@
     nat64_v4_pool: Optional[List[Address64V4PoolItem]] = Field(
         default=None, validation_alias=AliasPath("data", "nat64V4Pool"), description="NAT64 V4 Pool"
     )
 
     def set_dns_ipv4(
         self,
         primary_ipv4: Union[Variable, Global[IPv4Address]],
-        secondary_ipv4: Optional[Union[Variable, Global[IPv4Address]]] = None,
+        secondary_ipv4: Union[Variable, Global[IPv4Address], Default[None]] = as_default(None),
     ) -> None:
         """
         Set the DNS server IP addresses for IPv4.
 
         Sets the primary and, optionally, the secondary DNS server IP addresses for the system.
         The addresses can be specified as either string representations or as IPv4Address objects.
 
         Args:
             primary (Union[Variable, Global[IPv4Address]]): The IP address of the primary DNS server.
-            secondary (Optional[Union[Variable, Global[IPv4Address]], optional): The IP address of the
+            secondary (Union[Variable, Global[IPv4Address], Default[None]]): The IP address of the
                 secondary DNS server.
                 Defaults to None, which means no secondary DNS server is set.
         """
-        self.dns_ipv4 = DnsIpv4(primary_dns_address_ipv4=primary_ipv4, secondary_dns_address_ipv4=secondary_ipv4)
+        self.dns_ipv4 = DNSIPv4(primary_dns_address_ipv4=primary_ipv4, secondary_dns_address_ipv4=secondary_ipv4)
 
     def add_ipv4_route(
         self,
         prefix_ip_address: Global[IPv4Address],
         prefix_mask_address: Global[SubnetMask],
         next_hops: List[RouteHop],
         gateway: Optional[Global[Gateway]] = None,
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/cellular.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ethernet.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py` & `catalystwan-0.33.7.dev2/catalystwan/models/configuration/feature_profile/sdwan/transport/wan/interface/t1e1serial.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/device_inventory.py` & `catalystwan-0.33.7.dev2/catalystwan/models/device_inventory.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/misc/application_protocols.py` & `catalystwan-0.33.7.dev2/catalystwan/models/misc/application_protocols.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/centralized.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/centralized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/access_control_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/access_control_list_ipv6.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/access_control_list_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/aip.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/aip.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/amp.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/amp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/cflowd.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/cflowd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/control.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,14 +309,15 @@
 AnyControlPolicySequence = Annotated[
     Union[ControlPolicyRouteSequence, ControlPolicyTLOCSequence],
     Field(discriminator="sequence_type"),
 ]
 
 
 class ControlPolicy(ControlPolicyHeader, DefinitionWithSequencesCommonBase):
+    type: Literal["control"] = "control"
     sequences: List[AnyControlPolicySequence] = []
     default_action: PolicyAcceptRejectAction = Field(
         default=PolicyAcceptRejectAction(type="reject"),
         serialization_alias="defaultAction",
         validation_alias="defaultAction",
     )
     model_config = ConfigDict(populate_by_name=True)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/device_access.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/device_access_ipv6.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/device_access_ipv6.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/dns_security.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/dns_security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/hub_and_spoke.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/hub_and_spoke.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/intrusion_prevention.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/intrusion_prevention.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/mesh.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/mesh.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/qos_map.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/qos_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/rewrite.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rewrite.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/route_policy.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/route_policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/rule_set.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/rule_set.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/security_group.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/security_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/ssl_decryption.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/ssl_decryption_utd_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/traffic_data.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/traffic_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/url_filtering.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/url_filtering.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/vpn_membership.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/vpn_membership.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/definition/zone_based_firewall.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/definition/zone_based_firewall.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/app.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/zone.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-from typing import List, Literal, Optional
+# Copyright 2022 Cisco Systems, Inc. and its affiliates
 
-from pydantic import BaseModel, ConfigDict, Field, model_validator
+from typing import List, Literal, Optional, Set
 
-from catalystwan.models.common import check_fields_exclusive
-from catalystwan.models.policy.policy_list import PolicyListBase, PolicyListId, PolicyListInfo
+from pydantic import BaseModel, Field, field_validator, model_validator
 
+from catalystwan.models.common import InterfaceType, IntRangeStr, check_fields_exclusive
+from catalystwan.models.policy.policy_list import PolicyListBase, PolicyListId, PolicyListInfo
 
-class AppListEntry(BaseModel):
-    model_config = ConfigDict(populate_by_name=True)
 
-    app_family: Optional[str] = Field(default=None, serialization_alias="appFamily", validation_alias="appFamily")
-    app: Optional[str] = None
+class ZoneListEntry(BaseModel):
+    vpn: Optional[IntRangeStr] = Field(default=None, description="0-65530 single number")
+    interface: Optional[InterfaceType] = None
+
+    @field_validator("vpn")
+    @classmethod
+    def check_vpn_range(cls, vpn: IntRangeStr):
+        for i in vpn:
+            if i is not None:
+                assert 0 <= i <= 65_530
+        return vpn
 
     @model_validator(mode="after")
-    def check_app_xor_appfamily(self):
-        check_fields_exclusive(self.__dict__, {"app", "app_family"}, True)
+    def check_vpn_xor_interface(self):
+        check_fields_exclusive(self.__dict__, {"vpn", "interface"}, True)
         return self
 
 
-class AppList(PolicyListBase):
-    type: Literal["app"] = "app"
-    entries: List[AppListEntry] = []
+class ZoneList(PolicyListBase):
+    type: Literal["zone"] = "zone"
+    entries: List[ZoneListEntry] = []
 
-    def add_app(self, app: str) -> None:
-        self._add_entry(AppListEntry(app=app))
+    def assign_vpns(self, vpns: Set[int]) -> None:
+        self.entries = [ZoneListEntry(vpn=(vpn, None)) for vpn in vpns]
 
-    def add_app_family(self, app_family: str) -> None:
-        self._add_entry(AppListEntry(app_family=app_family))
+    def assign_interfaces(self, ifs: Set[InterfaceType]) -> None:
+        self.entries = [ZoneListEntry(interface=interface) for interface in ifs]
 
 
-class AppListEditPayload(AppList, PolicyListId):
+class ZoneListEditPayload(ZoneList, PolicyListId):
     pass
 
 
-class AppListInfo(AppList, PolicyListInfo):
+class ZoneListInfo(ZoneList, PolicyListInfo):
     pass
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/app_probe.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/app_probe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/as_path.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/as_path.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/class_map.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/class_map.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/color.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/color.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/communities.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/communities.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/data_ipv6_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/data_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/data_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/geo_location.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/geo_location.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/ips_signature.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ips_signature.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/ipv6_prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/ipv6_prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/local_app.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_app.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/local_domain.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/local_domain.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/mirror.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/mirror.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/policer.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/policer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/port.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/port.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/preferred_color_group.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/preferred_color_group.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/prefix.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/prefix.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/protocol_name.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/protocol_name.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/region.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/region.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/site.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/site.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/sla.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/sla.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/threat_grid_api_key.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/threat_grid_api_key.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/tloc.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/tloc.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/trunkgroup.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/trunkgroup.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/umbrella_data.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/umbrella_data.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/url.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/url.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/list/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/list/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/localized.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/localized.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/policy.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/policy_definition.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, Dict, List, MutableSequence, Optional, Sequence, Set, Tuple, Union
 from uuid import UUID
 
 from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator, model_validator
 from typing_extensions import Annotated, Literal
 
 from catalystwan.models.common import (
+    BasicPolicyActionType,
     CarrierType,
     ControlPathType,
     EncapType,
     ICMPMessageType,
     IntStr,
     MultiRegionRole,
     OriginProtocol,
@@ -68,16 +69,14 @@
 PathType = Literal[
     "hierarchical-path",
     "direct-path",
     "transport-gateway-path",
 ]
 
 
-BasicPolicyActionType = Literal["accept", "drop"]
-
 SequenceType = Literal[
     "applicationFirewall",
     "data",
     "serviceChaining",
     "trafficEngineering",
     "qos",
     "zoneBasedFW",
@@ -1077,15 +1076,15 @@
         )
 
     def _get_match_entries_by_field(self, field: str) -> Sequence[MatchEntry]:
         return [entry for entry in self.match.entries if entry.field == field]
 
     def _remove_match(self, match_type: Any) -> None:
         if isinstance(self.match.entries, MutableSequence):
-            self.match.entries[:] = [entry for entry in self.match.entries if type(entry) != match_type]
+            self.match.entries[:] = [entry for entry in self.match.entries if type(entry) is match_type]
 
     def _insert_match(self, match: MatchEntry, insert_field_check: bool = True) -> int:
         # inserts new item or replaces item with same field name if found
         if insert_field_check:
             self._check_match_can_be_inserted(match)
         if isinstance(self.match.entries, MutableSequence):
             for index, entry in enumerate(self.match.entries):
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/policy_list.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/policy_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/policy/security.py` & `catalystwan-0.33.7.dev2/catalystwan/models/policy/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/templates.py` & `catalystwan-0.33.7.dev2/catalystwan/models/templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/models/tenant.py` & `catalystwan-0.33.7.dev2/catalystwan/models/tenant.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/response.py` & `catalystwan-0.33.7.dev2/catalystwan/response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/session.py` & `catalystwan-0.33.7.dev2/catalystwan/session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_converter_chooser.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_converter_chooser.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/interface.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from datetime import datetime
 from uuid import uuid4
 
 from catalystwan.models.templates import FeatureTemplateInformation
 
 interface_ethernet = FeatureTemplateInformation(
     last_updated_by="admin",
@@ -148,7 +149,85 @@
     '"ignore", "vipValue": "aes256-gcm", "vipVariableName": "vpn_if_ipsec_ciphersuite"},'
     '"perfect-forward-secrecy": {"vipObjectType": "object", "vipType": "ignore", "vipValue":'
     '"group-16", "vipVariableName": "vpn_if_ipsec_perfect_forward_secrecy"}}, "clear-dont-'
     'fragment": {"vipObjectType": "object", "vipType": "ignore", "vipValue": "false",'
     '"vipVariableName": "vpn_ipsec_tunnel_tunnel_clear_dont_fragment"}, "tracker":'
     '{"vipObjectType": "list", "vipType": "ignore", "vipVariableName": "tracker"}}',
 )
+
+interface_multilink = FeatureTemplateInformation(
+    last_updated_by="admin",
+    id=str(uuid4()),
+    factory_default=False,
+    name="InterfaceMultilink",
+    devices_attached=0,
+    description="HnQSYJsm",
+    last_updated_on=datetime.now(),
+    resource_group="global",
+    template_type="vpn-cedge-interface-multilink-controller",
+    device_type=["vedge-C1101-4PLTEPW"],
+    version="15.0.0",
+    template_definiton='{"if-name": {"vipObjectType": "object", "vipType":'
+    '"constant", "vipValue": "Multilink1",'
+    '"vipVariableName": "if_multilink_ctrl_if_name"}, "ppp": {"authentication": {"method":'
+    '{"vipObjectType": "object", "vipType": "constant", "vipValue": "pap"}, "pap":'
+    '{"vipObjectType": "node-only", "vipType": "constant", "vipValue": "false"}, "callin":'
+    '{"vipObjectType": "node-only", "vipType": "notIgnore", "vipValue": "callin",'
+    '"vipVariableName": "pppoa_dsl_auth-callin"}}, "pap": {"sent-username": {"username":'
+    '{"username-string": {"vipObjectType": "object", "vipType": "constant", "vipValue": "test",'
+    '"vipVariableName": "pppoa_dsl_pap_username_string"}, "password": {"vipObjectType": "node-'
+    'only", "vipType": "constant", "vipValue": "true"}, "ppp-auth-password": {"vipObjectType":'
+    '"object", "vipType": "constant", "vipValue": "test", "vipVariableName":'
+    '"pppoa_dsl_pap_auth_password"}}}}, "multilink": {"group": {"vipObjectType": "object",'
+    '"vipType": "constant", "vipValue": 1, "vipVariableName":'
+    '"if_multilink_ctrl_multilink_group"}, "fragment": {"disable": {"vipObjectType": "node-'
+    'only", "vipType": "ignore", "vipValue": "false", "vipVariableName":'
+    '"if_multilink_fragment_disable_multilink_fragment_disable"}, "delay": {"delay-value":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"if_multilink_fragment_delay_value_multilink_fragment_delay_value"}}}, "interleave":'
+    '{"vipObjectType": "node-only", "vipType": "ignore", "vipValue": "false",'
+    '"vipVariableName": "if_multilink_interleave_multilink_interleave"}}}, "description":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"if_multilink_ctrl_description"}, "ip": {"address": {"vipObjectType": "object", "vipType":'
+    '"ignore", "vipVariableName": "if_multilink_ctrl_ip_addr"}}, "ipv6": {"address":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"if_multilink_ctrl_ipv6_address"}, "access-list": {"vipType": "ignore", "vipValue": [],'
+    '"vipObjectType": "tree", "vipPrimaryKey": ["direction"]}}, "pmtu": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipValue": "false", "vipVariableName": "vpn_if_pmtu"},'
+    '"mtu": {"vipObjectType": "object", "vipType": "ignore", "vipValue": 1500,'
+    '"vipVariableName": "if_multilink_ctrl_mtu"}, "static-ingress-qos": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipVariableName": "vpn_if_static_ingress_qos"}, "tcp-mss-'
+    'adjust": {"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"vpn_if_tcp_mss_adjust"}, "tloc-extension": {"vipObjectType": "object", "vipType":'
+    '"ignore", "vipVariableName": "vpn_if_tloc_extension"}, "shutdown": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipValue": "true", "vipVariableName":'
+    '"if_multilink_ctrl_shutdown"}, "autonegotiate": {"vipObjectType": "object", "vipType":'
+    '"ignore", "vipValue": "true", "vipVariableName": "vpn_if_autonegotiate"}, "shaping-rate":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName": "qos_shaping-rate"},'
+    '"qos-map": {"vipObjectType": "object", "vipType": "ignore", "vipVariableName": "qos-map"},'
+    '"qos-map-vpn": {"vipObjectType": "object", "vipType": "ignore", "vipVariableName": "vpn-'
+    'qos_map"}, "bandwidth-upstream": {"vipObjectType": "object", "vipType": "ignore",'
+    '"vipVariableName": "if_multilink_ctrl_bandwidth_upstream"}, "bandwidth-downstream":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"if_multilink_ctrl_bandwidth_downstream"}, "rewrite-rule": {"rule-name": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipVariableName": "rewrite_rule-name"}}, "access-list":'
+    '{"vipType": "ignore", "vipValue": [], "vipObjectType": "tree", "vipPrimaryKey":'
+    '["direction"]}, "policer": {"vipType": "ignore", "vipValue": [], "vipObjectType": "tree",'
+    '"vipPrimaryKey": ["policer-name", "direction"]}, "nat64-enable": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipValue": "false"}, "qos-adaptive": {"vipObjectType":'
+    '"object", "vipType": "ignore", "vipValue": "false", "vipVariableName": "adaptive_qos"},'
+    '"ip-directed-broadcast": {"vipObjectType": "object", "vipType": "ignore", "vipValue":'
+    '"false", "vipVariableName": "vpn_if_ip-directed-broadcast"}, "service-provider":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipVariableName":'
+    '"vpn_if_service_provider"}, "clear-dont-fragment": {"vipObjectType": "object", "vipType":'
+    '"ignore", "vipValue": "false", "vipVariableName": "vpn_if_clear_dont_fragment"},'
+    '"controller": {"nim-list": {"vipType": "constant", "vipValue": [{"nim": {"vipObjectType":'
+    '"object", "vipType": "constant", "vipValue": "2t", "vipVariableName":'
+    '"nim_twot_list_nim"}, "if-name": {"vipObjectType": "object", "vipType": "constant",'
+    '"vipValue": "serial1", "vipVariableName": "nim_twot_list_if-name"}, "description":'
+    '{"vipObjectType": "object", "vipType": "ignore", "vipValue": "", "vipVariableName":'
+    '"nim_twot_list_description"}, "bandwidth": {"vipObjectType": "object", "vipType":'
+    '"ignore", "vipValue": "", "vipVariableName": "nim_twot_list_bandwidth"}, "DCE-mode-'
+    'config": {"clock-rate": {"vipObjectType": "object", "vipType": "ignore", "vipValue": "",'
+    '"vipVariableName": "nim_twot_list_clock-rate"}}}], "vipObjectType": "tree",'
+    '"vipPrimaryKey": ["nim", "if-name"]}}}',
+)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_data/feature_templates/vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_device_template_with_info.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_device_template_with_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_merge_parcels.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_merge_parcels.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/config_migration/test_normalizer.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/config_migration/test_normalizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 import unittest
 from ipaddress import IPv4Address, IPv6Address
 from typing import List, Literal
 from unittest.mock import patch
 
 from catalystwan.api.configuration_groups.parcel import Global, Variable
 from catalystwan.api.templates.device_variable import DeviceVariable
@@ -30,14 +31,15 @@
             ],
             "nested-objects": [{"next-hop": [{"distance": 1}]}],
             "ipv4-address": "10.0.0.2",
             "ipv6addr": "2000:0:2:3::",
             "ip": {
                 "address": DeviceVariable(name="lan_ip_address_2"),
             },
+            "not_correct_variable": DeviceVariable(name="vpn1_gi3_lan_ip(192.168.X.1/24)_!@#$%^&*"),
         }
         self.expected_result = {
             "key_one": Global[str](value="Simple string !@#$%^&*()-=[';/.,`~]"),
             "keyone": Global[str](value="Simplestring!@#$%^&*()-=[';/.,`~]"),
             "bool_value_as_string": Global[bool](value=True),
             "boolvalueasstring": Global[bool](value=False),
             "simple_int": Global[int](value=1),
@@ -55,14 +57,15 @@
                 {"color": Global[str](value="biz-internet")},
                 {"color": Global[str](value="public-internet")},
             ],
             "nested_objects": [{"next_hop": [{"distance": Global[int](value=1)}]}],
             "ipv4_address": Global[IPv4Address](value=IPv4Address("10.0.0.2")),
             "ipv6addr": Global[IPv6Address](value=IPv6Address("2000:0:2:3::")),
             "ip": {"address": Variable(value="{{lan_ip_address_2}}")},
+            "not_correct_variable": Variable(value="{{vpn1_gi3_lan_ip_192.168.X.1/24__________}}"),
         }
 
     def test_normalizer_handles_various_types_of_input(self):
         # Arrange
         expected_result = self.expected_result
         # Act
         returned_result = template_values_normalization(self.template_values)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/banner_1.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/banner_1.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children_nested.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/cisco_bfd.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/complex_aaa.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/complex_cisco_vpn.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/complex_cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/default_cisco_system.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/default_cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/iuo.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/iuo.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/omp_2.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_2.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/definitions/omp_3.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/definitions/omp_3.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/__init__.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/__init__.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_aaa.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_bfd.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/cisco_vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/cisco_vpn.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/models/omp_vsmart.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/models/omp_vsmart.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/alias.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/alias.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/basic.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/basic.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children_nested.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/children_nested_datapath.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/basic/data_path.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/basic/data_path.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cedge_aaa.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cedge_aaa.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_banner.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_banner.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_bfd.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_bfd.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_system.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_system.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/cisco_vpn.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/cisco_vpn.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/schemas/omp-vsmart.json` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/schemas/omp-vsmart.json`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_chose_model.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_chose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_deserialize_model.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_deserialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_find_template_values.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_find_template_values_2.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_generate_payload.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_generate_payload.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/templates/test_serialize_model.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/templates/test_serialize_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_admin_tech_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_admin_tech_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_administration.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_administration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_alarms_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_alarms_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_cli_template.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_cli_template.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_creation_tools.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_device_action_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_device_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_devices_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_devices_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_endpoints.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_endpoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # mypy: disable-error-code="annotation-unchecked"
 import json
 import tempfile
 import unittest
 from enum import Enum
 from pathlib import Path
-from typing import Dict, List, Literal, Optional, Union
+from typing import List, Literal, Optional, Union
 from unittest.mock import MagicMock
 from uuid import UUID, uuid4
 
 import pytest  # type: ignore
 from packaging.version import Version  # type: ignore
 from parameterized import parameterized  # type: ignore
 from pydantic import BaseModel, ConfigDict, Field, model_serializer
@@ -305,22 +305,14 @@
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("POST", "/v1/data")
                 def get_data(self, payload: List[str]) -> None:  # type: ignore [empty-body]
                     ...
 
-    def test_request_decorator_unsupported_payload_composite_type(self):
-        with self.assertRaises(APIEndpointError):
-
-            class TestAPI(APIEndpoints):
-                @request("POST", "/v1/data")
-                def get_data(self, payload: Dict[str, BaseModelExample]) -> None:  # type: ignore [empty-body]
-                    ...
-
     @parameterized.expand(
         [
             (BaseModelExample, False, TypeSpecifier(True, None, BaseModelExample, None, False, False)),
             (List[BaseModelExample], False, TypeSpecifier(True, list, BaseModelExample, None, False, False)),
             (Optional[BaseModelExample], False, TypeSpecifier(True, None, BaseModelExample, None, False, True)),
             (
                 Optional[List[BaseModelExample]],
@@ -348,27 +340,32 @@
                 Annotated[Union[BaseModelExample, BaseModelExample2], None],
                 False,
                 TypeSpecifier(True, None, None, [BaseModelExample, BaseModelExample2], False, False),
             ),
             (None, True, None),
         ]
     )
-    def test_request_decorator_payload_spec(self, payload_type, raises, expected_payload_spec):
+    def test_request_decorator_payload_spec(self, payload_type, raises, expected_payload_spec: Optional[TypeSpecifier]):
         # Arrange
         class TestAPI(APIEndpoints):
             def get_data(self, payload: payload_type) -> None:  # type: ignore [empty-body]
                 ...
 
         decorator = request("POST", "/v1/data")
         # Act / Assert
         if raises:
             with self.assertRaises(APIEndpointError):
                 decorator(TestAPI.get_data)
         else:
             decorator(TestAPI.get_data)
+            if expected_payload_spec is not None and expected_payload_spec.payload_union_model_types is not None:
+                # check both list contains same set and skip member list comparison below
+                assert decorator.payload_spec.payload_model_set == expected_payload_spec.payload_model_set
+                decorator.payload_spec.payload_union_model_types = None
+                expected_payload_spec.payload_union_model_types = None
             assert decorator.payload_spec == expected_payload_spec
 
     def test_request_decorator_not_annotated_params(self):
         with self.assertRaises(APIEndpointError):
 
             class TestAPI(APIEndpoints):
                 @request("POST", "/v1/data")
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_feature_profile_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_profile_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 import unittest
 from unittest.mock import Mock
 from uuid import uuid4
 
 from parameterized import parameterized  # type: ignore
 
 from catalystwan.api.feature_profile_api import (
@@ -9,33 +10,37 @@
     SystemFeatureProfileAPI,
     TransportFeatureProfileAPI,
 )
 from catalystwan.endpoints.configuration.feature_profile.sdwan.service import ServiceFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.system import SystemFeatureProfile
 from catalystwan.endpoints.configuration.feature_profile.sdwan.transport import TransportFeatureProfile
 from catalystwan.models.configuration.feature_profile.parcel import ParcelAssociationPayload, ParcelCreationResponse
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv4acl import Ipv4AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.acl.ipv6acl import Ipv6AclParcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing import (
+    RoutingOspfParcel,
+    RoutingOspfv3IPv4Parcel,
+    RoutingOspfv3IPv6Parcel,
+)
 from catalystwan.models.configuration.feature_profile.sdwan.service import AppqoeParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service import (
     InterfaceEthernetParcel as LanInterfaceEthernetParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.service import InterfaceGreParcel as LanInterfaceGreParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service import (
     InterfaceIpsecParcel as LanInterfaceIpsecParcel,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.service import InterfaceSviParcel as LanInterfaceSviParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service import (
     LanVpnDhcpServerParcel,
     LanVpnParcel,
-    OspfParcel,
     SwitchportParcel,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.acl import Ipv4AclParcel, Ipv6AclParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.eigrp import EigrpParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.multicast import MulticastParcel
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospfv3 import Ospfv3IPv4Parcel, Ospfv3IPv6Parcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.route_policy import RoutePolicyParcel
 from catalystwan.models.configuration.feature_profile.sdwan.service.wireless_lan import WirelessLanParcel
 from catalystwan.models.configuration.feature_profile.sdwan.system import (
     AAAParcel,
     BannerParcel,
     BasicParcel,
     BFDParcel,
@@ -136,17 +141,17 @@
         self.mock_endpoint.update.assert_called_once_with(self.profile_uuid, expected_path, self.parcel_uuid, parcel)
 
 
 service_endpoint_mapping = {
     LanVpnDhcpServerParcel: "dhcp-server",
     AppqoeParcel: "appqoe",
     LanVpnParcel: "lan/vpn",
-    OspfParcel: "routing/ospf",
-    Ospfv3IPv4Parcel: "routing/ospfv3/ipv4",
-    Ospfv3IPv6Parcel: "routing/ospfv3/ipv6",
+    RoutingOspfParcel: "routing/ospf",
+    RoutingOspfv3IPv4Parcel: "routing/ospfv3/ipv4",
+    RoutingOspfv3IPv6Parcel: "routing/ospfv3/ipv6",
     RoutePolicyParcel: "route-policy",
     EigrpParcel: "routing/eigrp",
     Ipv6AclParcel: "ipv6-acl",
     Ipv4AclParcel: "ipv4-acl",
     SwitchportParcel: "switchport",
     MulticastParcel: "routing/multicast",
     WirelessLanParcel: "wirelesslan",
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_feature_template_field.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_feature_template_field.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_logs_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_models_common.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_models_common.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_monitoring_server_info.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_server_info.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_monitoring_status_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_monitoring_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_mtt_aaa_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_mtt_aaa_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_normalize_to_model_definition.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_normalize_to_model_definition.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_omp_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_omp_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_packet_capture.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_packet_capture.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_partition_manager_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_partition_manager_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_response.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_session.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_software_action_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_software_action_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_speed_test_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_speed_test_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_task_status_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_task_status_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_templates.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_backup_restore_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_backup_restore_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_management_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_management_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_tenant_migration_api.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_tenant_migration_api.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_typed_list.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_version.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_version_utils.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_version_utils.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/tests/test_vmanage_auth.py` & `catalystwan-0.33.7.dev2/catalystwan/tests/test_vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/typed_list.py` & `catalystwan-0.33.7.dev2/catalystwan/typed_list.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/aaa.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/aaa.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/appqoe.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/appqoe.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/banner.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/banner.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/basic.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/basic.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/bfd.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/bfd.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_controller.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from copy import deepcopy
 from typing import Dict
 
+from catalystwan.api.configuration_groups.parcel import Global, as_global
 from catalystwan.models.configuration.feature_profile.sdwan.transport.cellular_controller import (
     CellularControllerParcel,
     ControllerConfig,
 )
 from catalystwan.utils.config_migration.converters.exceptions import CatalystwanConverterCantConvertException
 
 
@@ -27,11 +29,15 @@
         _id = data.get("id")
         if not _id:
             raise CatalystwanConverterCantConvertException("Cellular ID is required")
         lte = data.get("lte", {})
         sim = lte.get("sim", {})
         primary = sim.get("primary", {})
         slot = primary.get("slot")
+        if isinstance(slot, Global):
+            if slot.value not in (0, 1):
+                slot = as_global(0)
+
         max_retry = sim.get("max_retry")
         failovertimer = lte.get("failovertimer")
 
         return ControllerConfig(id=_id, slot=slot, max_retry=max_retry, failover_timer=failovertimer)
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cellular_profile.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cli.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cli.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/cloud_credentials.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/eigrp.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/eigrp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ethernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from ipaddress import IPv6Interface
 from typing import Dict, List, Optional, Union
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, as_default, as_global
 from catalystwan.models.common import EthernetDuplexMode, Speed
 from catalystwan.models.configuration.feature_profile.common import (
     Arp,
@@ -46,15 +47,15 @@
         return InterfaceEthernetParcel(**payload)
 
     def parse_ipv4_address(
         self, data: Dict
     ) -> Optional[Union[InterfaceDynamicIPv4Address, InterfaceStaticIPv4Address]]:
         ip_address = data.get("ip", {})
 
-        if "address" in ip_address:
+        if "address" in ip_address and ip_address["address"].value != "":
             return InterfaceStaticIPv4Address(
                 static=StaticIPv4AddressConfig(
                     primary_ip_address=self.get_static_ipv4_address(ip_address),
                     secondary_ip_address=self.get_secondary_static_ipv4_address(ip_address),
                 )
             )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/global_.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/global_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/gps.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/gps.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ethernet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from copy import deepcopy
 from typing import Dict, List, Optional
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, as_default, as_global, as_variable
-from catalystwan.models.common import EthernetDuplexMode
+from catalystwan.models.common import EthernetDuplexMode, EthernetNatType
 from catalystwan.models.configuration.feature_profile.common import (
     Arp,
     DynamicIPv6Dhcp,
     EthernetNatPool,
     StaticIPv4Address,
     StaticIPv6Address,
 )
@@ -72,17 +73,14 @@
         "static_ingress_qos",
         "flow_control",
         "address",
         "tunnel_interface",  # Not sure if this is correct. There is some data in UX1 that is not transferable to UX2
         "nat66",  # Not sure if this is correct. There is some data in UX1 that is not transferable to UX2
     )
 
-    # Default Values - Interface Name
-    basic_conf_intf_name = "{{vpn23_1_basicConf_intfName}}"
-
     # Default Values - NAT Attribute
     nat_attribute_nat_choice = "{{natAttr_natChoice}}"
 
     def create_parcel(self, name: str, description: str, template_values: dict) -> InterfaceEthernetParcel:
         values = deepcopy(template_values)
 
         self.configure_interface_name(values)
@@ -112,22 +110,21 @@
             dict: The prepared parcel values for InterfaceSviParcel to consume.
         """
         return {"parcel_name": name, "parcel_description": description, **values}
 
     def configure_interface_name(self, values: dict) -> None:
         if if_name := values.get("if_name"):
             values["interface_name"] = if_name
-        values["interface_name"] = as_variable(self.basic_conf_intf_name)
 
     def configure_ethernet_description(self, values: dict) -> None:
         values["ethernet_description"] = values.get("description")
 
     def configure_ipv4_address(self, values: dict) -> None:
         if ipv4_address_configuration := values.get("ip"):
-            if "address" in ipv4_address_configuration:
+            if "address" in ipv4_address_configuration and ipv4_address_configuration["address"].value != "":
                 values["interface_ip_address"] = InterfaceStaticIPv4Address(
                     static=StaticIPv4AddressConfig(
                         primary_ip_address=self.get_static_ipv4_address(ipv4_address_configuration),
                         secondary_ip_address=self.get_secondary_static_ipv4_address(ipv4_address_configuration),
                     )
                 )
             elif "dhcp_client" in ipv4_address_configuration:
@@ -263,17 +260,25 @@
                 vrrp_ipv6["group_id"] = vrrp_ipv6.pop("grp_id")
             values["vrrp_ipv6"] = vrrps_ipv6
 
     def configure_network_address_translation(self, values: dict) -> None:
         if nat := values.get("nat"):
             if isinstance(nat, dict):
                 # Nat can be straight up Global[bool] or a dict with more values
-                nat_type = nat.get("nat_choice", as_variable(self.nat_attribute_nat_choice))
-                if nat_type.value.lower() == "interface":
+                nat_type = nat.get("nat_choice")
+
+                if nat_type is None:
+                    nat_type = as_global("loopback", EthernetNatType)
+
+                elif nat_type.value.lower() == "interface":
                     nat_type = as_variable(self.nat_attribute_nat_choice)
+
+                elif not isinstance(nat_type, Variable):
+                    nat_type = as_global(nat_type.value, EthernetNatType)
+
                 values["nat_attributes_ipv4"] = EthernetNatAttributesIpv4(
                     nat_type=nat_type,
                     nat_pool=self.get_nat_pool(nat),
                     udp_timeout=nat.get("udp_timeout", as_default(1)),
                     tcp_timeout=nat.get("tcp_timeout", as_default(60)),
                     new_static_nat=nat.get("static"),
                 )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/ipsec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from copy import deepcopy
 from ipaddress import IPv4Address, IPv4Interface, IPv6Address
 
-from catalystwan.api.configuration_groups.parcel import Default, as_default, as_global, as_variable
+from catalystwan.api.configuration_groups.parcel import Default, Variable, as_default, as_global, as_variable
 from catalystwan.models.common import IkeGroup
 from catalystwan.models.configuration.feature_profile.common import AddressWithMask, TunnelApplication
 from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ipsec import InterfaceIpsecParcel
 from catalystwan.utils.config_migration.converters.exceptions import CatalystwanConverterCantConvertException
 from catalystwan.utils.config_migration.steps.constants import LAN_VPN_IPSEC
 
 
@@ -87,18 +88,30 @@
                     mask=as_global(str(tunnel_destination.value.network.netmask)),
                 )
             elif isinstance(tunnel_destination.value, IPv4Address):
                 values["tunnel_destination"] = AddressWithMask(
                     address=tunnel_destination,
                     mask=as_global("0.0.0.0"),
                 )
+            elif isinstance(tunnel_destination, Variable):
+                values["tunnel_destination"] = AddressWithMask(
+                    address=tunnel_destination,
+                    mask=as_global("0.0.0.0"),
+                )
 
             elif isinstance(tunnel_destination.value, IPv6Address):
-                values.pop("tunnel_destination")
-                values["tunnel_destination_v6"] = tunnel_destination
+                # 20.12, 20.13 dont have tunnel_destination_v6
+                # TODO: pass version to converter
+                values["tunnel_destination"] = AddressWithMask(
+                    address=as_variable(value="ipsec_tunnelDestination_addr"),
+                    mask=as_global("0.0.0.0"),
+                )
+
+                # values.pop("tunnel_destination")
+                # values["tunnel_destination_v6"] = tunnel_destination
 
     def configure_tunnel_source(self, values: dict) -> None:
         if tunnel_source := values.get("tunnel_source"):
             values["tunnel_source"] = AddressWithMask(
                 address=as_global(str(tunnel_source.value)),
                 mask=as_global("0.0.0.0"),
             )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/lan/svi.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/logging_.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/logging_.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/model_definition_normalizer.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/multicast.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/multicast.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/normalizer.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/normalizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2024 Cisco Systems, Inc. and its affiliates
 from ipaddress import AddressValueError, IPv4Address, IPv4Interface, IPv6Address, IPv6Interface
 from typing import List, Optional, Union, get_args
 
 from catalystwan.api.configuration_groups.parcel import Global, Variable, as_global, as_variable
 from catalystwan.api.templates.device_variable import DeviceVariable
 from catalystwan.models.common import (
     EthernetDuplexMode,
@@ -12,25 +13,25 @@
     MetricType,
     PfsGroup,
     SubnetMask,
     TLOCColor,
     VrrpTrackerAction,
 )
 from catalystwan.models.configuration.feature_profile.common import TunnelApplication
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ethernet import MediaType
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.gre import GreTunnelMode
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ipsec import IpsecTunnelMode
-from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import Direction
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospf import (
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospf import (
     AdvertiseType,
     AreaType,
     AuthenticationType,
     RedistributeProtocolOspf,
 )
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospfv3 import NetworkType
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospfv3 import NetworkType
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ethernet import MediaType
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.gre import GreTunnelMode
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.ipsec import IpsecTunnelMode
+from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import Direction
 from catalystwan.models.configuration.feature_profile.sdwan.service.switchport import (
     ControlDirection,
     Duplex,
     HostMode,
     PortControl,
     SwitchportMode,
 )
@@ -43,14 +44,15 @@
 from catalystwan.models.configuration.feature_profile.sdwan.system.logging_parcel import (
     AuthType,
     CypherSuite,
     Priority,
     TlsVersion,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.system.mrf import EnableMrfMigration, Role
+from catalystwan.utils.config_migration.converters.utils import convert_varname
 
 """List of all literals that can be casted."""
 CastableLiterals = Union[
     Priority,
     TlsVersion,
     AuthType,
     CypherSuite,
@@ -105,15 +107,15 @@
 def to_snake_case(s: str) -> str:
     """Converts a string from kebab-case to snake_case."""
     return s.replace("-", "_")
 
 
 def cast_value_to_global(value: Union[DeviceVariable, str, int, List[str], List[int]]) -> CastedTypes:
     if isinstance(value, DeviceVariable):
-        return as_variable(value.name.replace(" ", "_"))
+        return as_variable(value=convert_varname(value.name))
     if isinstance(value, list):
         value_type = Global[List[int]] if isinstance(value[0], int) else Global[List[str]]
         return value_type(value=value)  # type: ignore
     if isinstance(value, str):
         for cast_func in [try_cast_to_literal, try_cast_to_bool, try_cast_to_address]:
             if global_value := cast_func(value):
                 return global_value
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ntp.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ntp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/omp.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/omp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ospf.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from copy import deepcopy
 from typing import List, Optional
 
 from catalystwan.api.configuration_groups.parcel import Global, as_global
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospf import (
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospf import (
     AreaType,
     OspfArea,
     OspfInterfaceParametres,
-    OspfParcel,
     RouterLsa,
+    RoutingOspfParcel,
     SummaryPrefix,
     SummaryRoute,
 )
+from catalystwan.utils.config_migration.steps.constants import LAN_OSPF, WAN_OSPF
 
 
 class OspfTemplateConverter:
-    supported_template_types = ("cisco_ospf",)
+    supported_template_types = (LAN_OSPF, WAN_OSPF)
 
     delete_keys = ("max_metric", "timers", "distance", "auto_cost", "default_information", "compatible")
 
-    def create_parcel(self, name: str, description: str, template_values: dict) -> OspfParcel:
+    def create_parcel(self, name: str, description: str, template_values: dict) -> RoutingOspfParcel:
         """
         Creates a BannerParcel object based on the provided template values.
 
         Args:
             name (str): The name of the BannerParcel.
             description (str): The description of the BannerParcel.
             template_values (dict): A dictionary containing the template values.
@@ -36,15 +38,15 @@
         self.configure_distance(values)
         self.configure_reference_bandwidth(values)
         self.configure_originate(values)
         self.configure_rfc1583(values)
         self.configure_area(values)
         self.configure_route_policy(values)
         self.cleanup_keys(values)
-        return OspfParcel(parcel_name=name, parcel_description=description, **values)
+        return RoutingOspfParcel(parcel_name=name, parcel_description=description, **values)
 
     def configure_router_lsa(self, values: dict) -> None:
         if router_lsa := values.get("max_metric", {}).get("router_lsa"):
             router_lsa_list = []
             for router_lsa_value in router_lsa:
                 router_lsa_list.append(RouterLsa(**router_lsa_value))
             values["router_lsa"] = router_lsa_list
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ospfv3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,63 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from copy import deepcopy
-from typing import List, Optional, Tuple, Type, Union, cast, get_args
+from typing import List, Optional, Type, Union, get_args
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, as_global
 from catalystwan.models.configuration.feature_profile.common import AddressWithMask
-from catalystwan.models.configuration.feature_profile.sdwan.service import Ospfv3IPv4Parcel
-from catalystwan.models.configuration.feature_profile.sdwan.service.ospfv3 import (
+from catalystwan.models.configuration.feature_profile.sdwan.routing import RoutingOspfv3IPv4Parcel
+from catalystwan.models.configuration.feature_profile.sdwan.routing.ospfv3 import (
     AdvancedOspfv3Attributes,
     BasicOspfv3Attributes,
     DefaultArea,
     DefaultOriginate,
     MaxMetricRouterLsa,
     MaxMetricRouterLsaAction,
     NormalArea,
     NssaArea,
     Ospfv3InterfaceParametres,
     Ospfv3IPv4Area,
     Ospfv3IPv6Area,
-    Ospfv3IPv6Parcel,
     RedistributedRoute,
     RedistributedRouteIPv6,
     RedistributeProtocol,
     RedistributeProtocolIPv6,
+    RoutingOspfv3IPv6Parcel,
     SpfTimers,
     StubArea,
     SummaryRoute,
     SummaryRouteIPv6,
 )
 from catalystwan.utils.config_migration.converters.exceptions import CatalystwanConverterCantConvertException
+from catalystwan.utils.config_migration.steps.constants import LAN_OSPFV3, WAN_OSPFV3
 
 
 class Ospfv3TemplateConverter:
     """
-    Warning: This class returns a tuple of Ospfv3IPv4Parcel and Ospfv3IPv6Parcel objects,
+    Warning: This class returns a tuple of RoutingOspfv3IPv4Parcel and RoutingOspfv3IPv6Parcel objects,
     because the Feature Template has two definitions inside one for IPv4 and one for IPv6.
     """
 
-    supported_template_types = ("cisco_ospfv3",)
+    supported_template_types = (WAN_OSPFV3, LAN_OSPFV3)
 
     def create_parcel(
         self, name: str, description: str, template_values: dict
-    ) -> Tuple[Ospfv3IPv4Parcel, Ospfv3IPv6Parcel]:
+    ) -> List[Union[RoutingOspfv3IPv4Parcel, RoutingOspfv3IPv6Parcel]]:
         if template_values.get("ospfv3") is None:
             raise CatalystwanConverterCantConvertException("Feature Template does not contain OSPFv3 configuration")
-        ospfv3ipv4 = cast(
-            Ospfv3IPv4Parcel, Ospfv3Ipv4TemplateSubconverter().create_parcel(name, description, template_values)
-        )
-        ospfv3ipv6 = cast(
-            Ospfv3IPv6Parcel, Ospfv3Ipv6TemplateSubconverter().create_parcel(name, description, template_values)
-        )
-        return ospfv3ipv4, ospfv3ipv6
+        ospfv3ipv4 = Ospfv3Ipv4TemplateSubconverter().create_parcel(name, description, template_values)
+        ospfv3ipv6 = Ospfv3Ipv6TemplateSubconverter().create_parcel(name, description, template_values)
+        return [ospfv3ipv4, ospfv3ipv6]
 
 
 class BaseOspfv3TemplateSubconverter:
+    name_suffix: str
     key_address_family: str
     key_distance: str
-    parcel_model: Union[Type[Ospfv3IPv4Parcel], Type[Ospfv3IPv6Parcel]]
+    parcel_model: Union[Type[RoutingOspfv3IPv4Parcel], Type[RoutingOspfv3IPv6Parcel]]
     area_model: Union[Type[Ospfv3IPv4Area], Type[Ospfv3IPv6Area]]
 
     delete_keys = (
         "default_information",
         "router_id",
         "table_map",
         "max_metric",
@@ -67,15 +66,16 @@
         "distance_ipv6",
         "auto_cost",
         "compatible",
     )
 
     def create_parcel(
         self, name: str, description: str, template_values: dict
-    ) -> Union[Ospfv3IPv4Parcel, Ospfv3IPv6Parcel]:
+    ) -> Union[RoutingOspfv3IPv4Parcel, RoutingOspfv3IPv6Parcel]:
+        name = f"{name}{self.name_suffix}"
         values = self.get_values(template_values)
         self.configure_basic_ospf_v3_attributes(values)
         self.configure_advanced_ospf_v3_attributes(values)
         self.configure_max_metric_router_lsa(values)
         self.configure_area(values)
         self.configure_redistribute(values)
         self.cleanup_keys(values)
@@ -134,25 +134,33 @@
         return SpfTimers(
             delay=timers.get("delay"),
             initial_hold=timers.get("initial_hold"),
             max_hold=timers.get("max_hold"),
         )
 
     def configure_max_metric_router_lsa(self, values: dict) -> None:
-        router_lsa = values.get("max_metric", {}).get("router_lsa", [])[0]  # Payload contains only one item
-        if router_lsa == []:
+        max_metric_data = values.get("max_metric", {})
+        router_lsa_data = max_metric_data.get("router_lsa", [])
+
+        if not router_lsa_data:
+            return
+
+        router_lsa = router_lsa_data[0] if router_lsa_data else None
+        if not router_lsa:
             return
 
         action = router_lsa.get("ad_type")
-        if action is not None:
+        if action:
             action = as_global(action.value, MaxMetricRouterLsaAction)
 
+        on_startup_time = router_lsa.get("time")
+
         values["max_metric_router_lsa"] = MaxMetricRouterLsa(
             action=action,
-            on_startup_time=router_lsa.get("time"),
+            on_startup_time=on_startup_time,
         )
 
     def configure_area(self, values: dict) -> None:
         area = values.get("area")
         if area is None:
             raise CatalystwanConverterCantConvertException("Area is required for OSPFv3")
         area_list = []
@@ -197,17 +205,18 @@
 
     def cleanup_keys(self, values: dict) -> None:
         for key in self.delete_keys:
             values.pop(key, None)
 
 
 class Ospfv3Ipv4TemplateSubconverter(BaseOspfv3TemplateSubconverter):
+    name_suffix = "_IPV4"
     key_address_family = "ipv4"
     key_distance = "distance_ipv4"
-    parcel_model = Ospfv3IPv4Parcel
+    parcel_model = RoutingOspfv3IPv4Parcel
     area_model = Ospfv3IPv4Area
 
     def _set_range(self, area_value: dict) -> Optional[List[SummaryRoute]]:
         ranges = area_value.get("range")
         if ranges is None:
             return None
         range_list = []
@@ -215,15 +224,16 @@
             self._set_summary_prefix(range_)
             range_list.append(SummaryRoute(**range_))
         return range_list
 
     def _set_summary_prefix(self, range_: dict) -> None:
         if address := range_.pop("address"):
             range_["network"] = AddressWithMask(
-                address=as_global(str(address.value.network)), mask=as_global(str(address.value.netmask))
+                address=as_global(str(address.value.network.network_address)),
+                mask=as_global(str(address.value.netmask)),
             )
 
     def configure_redistribute(self, values: dict) -> None:
         redistributes = values.get("redistribute", [])
         if redistributes == []:
             return None
         redistribute_list = []
@@ -235,17 +245,18 @@
                     nat_dia=redistribute.get("dia"),
                 )
             )
         values["redistribute"] = redistribute_list
 
 
 class Ospfv3Ipv6TemplateSubconverter(BaseOspfv3TemplateSubconverter):
+    name_suffix = "_IPV6"
     key_address_family = "ipv6"
     key_distance = "distance_ipv6"
-    parcel_model = Ospfv3IPv6Parcel
+    parcel_model = RoutingOspfv3IPv6Parcel
     area_model = Ospfv3IPv6Area
 
     def _set_range(self, area_value: dict) -> Optional[List[SummaryRouteIPv6]]:
         ranges = area_value.get("range")
         if ranges is None:
             return None
         range_list = []
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/parcel_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Copyright 2023 Cisco Systems, Inc. and its affiliates
 import json
 import logging
-from typing import Any, Callable, Dict, cast
+from typing import Any, Callable, Dict, List, Union, cast
 
 from catalystwan.api.template_api import FeatureTemplateInformation
 from catalystwan.exceptions import CatalystwanException
 from catalystwan.models.configuration.feature_profile.parcel import AnyParcel
 from catalystwan.utils.config_migration.converters.feature_template.lan.multilink import LanMultilinkTemplateConverter
 from catalystwan.utils.feature_template.find_template_values import find_template_values
 
 from .aaa import AAATemplateConverter
 from .appqoe import AppqoeTemplateConverter
 from .banner import BannerTemplateConverter
 from .base import FeatureTemplateConverter
 from .basic import SystemToBasicTemplateConverter
 from .bfd import BFDTemplateConverter
-from .bgp import BGPTemplateConverter
+from .bgp import BgpRoutingTemplateConverter
 from .cellular_controller import CellularControllerTemplateConverter
 from .cellular_profile import CellularProfileTemplateConverter
 from .cli import CliTemplateConverter
 from .dhcp import DhcpTemplateConverter
 from .ethernet import ManagementInterfaceEthernetTemplateConverter
 from .global_ import GlobalTemplateConverter
 from .gps import GpsTemplateConverter
@@ -67,15 +67,15 @@
     SecurityTemplateConverter,
     SystemToBasicTemplateConverter,
     BFDTemplateConverter,
     GlobalTemplateConverter,
     LoggingTemplateConverter,
     OMPTemplateConverter,
     NtpTemplateConverter,
-    BGPTemplateConverter,
+    BgpRoutingTemplateConverter,
     ThousandEyesTemplateConverter,
     UcseTemplateConverter,
     DhcpTemplateConverter,
     SNMPTemplateConverter,
     AppqoeTemplateConverter,
     VpnTemplateConverter,
     LanInterfaceGreTemplateConverter,
@@ -132,15 +132,15 @@
         if template_type in key:
             converter = supported_parcel_converters[key]
             logger.debug(f"Choosen converter {converter} based on template type {template_type}")
             return converter
     raise CatalystwanException(f"Template type {template_type} not supported")
 
 
-def create_parcel_from_template(template: FeatureTemplateInformation) -> AnyParcel:
+def create_parcel_from_template(template: FeatureTemplateInformation) -> Union[AnyParcel, List[AnyParcel]]:
     """
     Creates a new instance of a _ParcelBase based on the given template.
 
     Args:
         template (FeatureTemplateInformation): The template to use for creating the _ParcelBase instance.
 
     Returns:
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/security.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/security.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/sig.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/sig.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/snmp.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/snmp.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/switchport.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/switchport.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/thousandeyes.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/ucse.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/ucse.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/vpn.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/vpn.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,21 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 import logging
 from copy import deepcopy
 from ipaddress import IPv4Interface, IPv6Interface
 from typing import Dict, List, Literal, Optional, Tuple, Type, Union
 
-from pydantic import BaseModel, IPvAnyAddress
+from pydantic import BaseModel
 
-from catalystwan.api.configuration_groups.parcel import (
-    Default,
-    Global,
-    OptionType,
-    Variable,
-    as_default,
-    as_global,
-    as_variable,
-)
+from catalystwan.api.configuration_groups.parcel import Default, Global, OptionType, Variable, as_default, as_global
 from catalystwan.models.common import SubnetMask
-from catalystwan.models.configuration.feature_profile.common import AddressWithMask
+from catalystwan.models.configuration.feature_profile.common import AddressWithMask, DNSIPv4, DNSIPv6, HostMapping
 from catalystwan.models.configuration.feature_profile.sdwan.service.lan.vpn import (
     DHCP,
     Direction,
-    DnsIPv4,
-    HostMapping,
     InterfaceIPv6Container,
     InterfaceRouteIPv6Container,
     IPv4Prefix,
     IPv4RouteGatewayNextHop,
     IPv4RouteGatewayNextHopWithTracker,
     IPv6Prefix,
     IPv6StaticRouteInterface,
@@ -54,21 +45,18 @@
     StaticIpsecRouteIPv4,
     StaticNat,
     StaticRouteIPv4,
     StaticRouteIPv6,
     StaticRouteVPN,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import (
-    DnsIpv4,
-    DnsIpv6,
     Gateway,
     Ipv4RouteItem,
     Ipv6RouteItem,
     ManagementVpnParcel,
-    NewHostMappingItem,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import (
     NextHopContainer as TransportNextHopContainer,
 )
 from catalystwan.models.configuration.feature_profile.sdwan.transport.vpn import (
     NextHopItem,
     NextHopItemIpv6,
@@ -97,43 +85,57 @@
 class OmpMappingItem(BaseModel):
     ux2_model_omp: Type[Union[OmpAdvertiseIPv4, OmpAdvertiseIPv6]]
     ux2_model_prefix: Type[Union[IPv4Prefix, IPv6Prefix]]
     ux2_field: Literal["omp_advertise_ipv4", "omp_advertise_ipv6"]
 
 
 class BaseTransportAndManagementTemplateConverter:
-    def configure_new_host_mapping(self, values: dict) -> Optional[List[NewHostMappingItem]]:
+    def parse_host_mapping(self, values: dict) -> Optional[List[HostMapping]]:
         hosts = values.get("host", [])
         if not hosts:
             return None
+
+        hosts_cleared = [h for h in hosts if self.is_host_mapping_parsable(h)]
+
         return [
-            NewHostMappingItem(
+            HostMapping(
                 host_name=host["hostname"],
-                list_of_ip=host["ip"],
+                list_of_ips=self.parse_list_of_ip(host),
             )
-            for host in hosts
+            for host in hosts_cleared
         ]
 
-    def configure_dns(self, values: dict) -> Tuple[DnsIpv4, DnsIpv6]:
+    def parse_list_of_ip(self, host: Dict) -> Union[Variable, Global[List[str]]]:
+        list_of_ips = host["ip"]
+        if isinstance(list_of_ips, Variable):
+            return list_of_ips
+
+        # ["34.199.1.194"," 34.204.213.179], extra space before the ip is a bug in the feature template
+        return Global[List[str]](value=[ip.strip() for ip in list_of_ips.value])
+
+    def is_host_mapping_parsable(self, host: Dict) -> bool:
+        return "ip" in host and "hostname" in host
+
+    def parse_dns(self, values: dict) -> Tuple[DNSIPv4, DNSIPv6]:
         dns = values.get("dns", [])
-        dns_ipv4 = DnsIpv4()
-        dns_ipv6 = DnsIpv6()
+        dns_ipv4 = DNSIPv4()
+        dns_ipv6 = DNSIPv6()
         for dns_entry in dns:
             dns_address = dns_entry.get("dns_addr", Default[None](value=None))
             if dns_entry["role"].value == "primary":
                 dns_ipv4.primary_dns_address_ipv4 = dns_address
             elif dns_entry["role"].value == "secondary":
                 dns_ipv4.secondary_dns_address_ipv4 = dns_address
             elif dns_entry["role"].value == "primaryv6":
                 dns_ipv6.primary_dns_address_ipv6 = dns_address
             elif dns_entry["role"].value == "secondaryv6":
                 dns_ipv6.secondary_dns_address_ipv6 = dns_address
         return dns_ipv4, dns_ipv6
 
-    def configure_route_ipv4(self, values: dict) -> Optional[List[Ipv4RouteItem]]:
+    def parse_route_ipv4(self, values: dict) -> Optional[List[Ipv4RouteItem]]:
         routes = values.get("ip", {}).get("route", [])
         if not routes:
             return None
         static_routes = []
         for route in routes:
             prefix = route.get("prefix")
             if not prefix:
@@ -163,15 +165,15 @@
                         )
                     ]
             elif "dhcp" in route:
                 ipv4route_item.gateway = as_global("dhcp", Gateway)
             static_routes.append(ipv4route_item)
         return static_routes
 
-    def configure_route_ipv6(self, values: dict) -> Optional[List[Ipv6RouteItem]]:
+    def parse_route_ipv6(self, values: dict) -> Optional[List[Ipv6RouteItem]]:
         routes = values.get("ipv6", {}).get("route", [])
         if not routes:
             return None
         static_routes = []
         for route in routes:
             one_of_ip_route: Union[OneOfIpRouteNull0, OneOfIpRouteNextHopContainer] = OneOfIpRouteNull0()
             if "null0" in route:
@@ -206,19 +208,19 @@
             template_values (dict): A dictionary containing the template values.
 
         Returns:
             VPN: The created ManagementVpnParcel.
         """
         data = deepcopy(template_values)
 
-        dns_ipv4, dns_ipv6 = self.configure_dns(data)
-        ipv4_route = self.configure_route_ipv4(data)
-        ipv6_route = self.configure_route_ipv6(data)
-        new_host_mapping = self.configure_new_host_mapping(data)
-        dns_ipv4, dns_ipv6 = self.configure_dns(data)
+        dns_ipv4, dns_ipv6 = self.parse_dns(data)
+        ipv4_route = self.parse_route_ipv4(data)
+        ipv6_route = self.parse_route_ipv6(data)
+        new_host_mapping = self.parse_host_mapping(data)
+        dns_ipv4, dns_ipv6 = self.parse_dns(data)
 
         payload = create_dict_without_none(
             dns_ipv4=dns_ipv4,
             dns_ipv6=dns_ipv6,
             new_host_mapping=new_host_mapping,
             ipv6_route=ipv6_route,
             ipv4_route=ipv4_route,
@@ -238,18 +240,18 @@
             template_values (dict): A dictionary containing the template values.
 
         Returns:
             VPN: The created TransportVpnParcel.
         """
         data = deepcopy(template_values)
 
-        ipv4_route = self.configure_route_ipv4(data)
-        ipv6_route = self.configure_route_ipv6(data)
-        new_host_mapping = self.configure_new_host_mapping(data)
-        dns_ipv4, dns_ipv6 = self.configure_dns(data)
+        ipv4_route = self.parse_route_ipv4(data)
+        ipv6_route = self.parse_route_ipv6(data)
+        new_host_mapping = self.parse_host_mapping(data)
+        dns_ipv4, dns_ipv6 = self.parse_dns(data)
         service = self.parse_service(data.get("service", []))
         enhance_ecmp_keying = data.get("enhance_ecmp_keying", {}).get("layer4")
 
         payload = create_dict_without_none(
             service=service,
             enhance_ecmp_keying=enhance_ecmp_keying,
             dns_ipv4=dns_ipv4,
@@ -273,30 +275,14 @@
 
 
 class ServiceVpnTemplateConverter:
     """
     A class for converting template values into a LanVpnParcel object.
     """
 
-    delete_keys = (
-        "ecmp_hash_key",
-        "ip",
-        "omp",
-        "nat",
-        "nat64",
-        "dns",
-        "host",
-        "ipv6",
-        "name",
-        "route_import_from",
-        "route_import",
-        "route_export",
-        "tcp_optimization",
-    )
-
     route_leaks_mapping = {
         "route_import": RouteLeakMappingItem(ux2_model=RouteLeakFromGlobal, ux2_field="route_leak_from_global"),
         "route_export": RouteLeakMappingItem(ux2_model=RouteLeakFromService, ux2_field="route_leak_from_service"),
         "route_import_from": RouteLeakMappingItem(
             ux2_model=RouteLeakBetweenServices, ux2_field="route_leak_between_services"
         ),
     }
@@ -314,316 +300,333 @@
             ux2_field="omp_advertise_ipv4",
         ),
         "ipv6_advertise": OmpMappingItem(
             ux2_model_omp=OmpAdvertiseIPv6, ux2_model_prefix=IPv6Prefix, ux2_field="omp_advertise_ipv6"
         ),
     }
 
-    # Default Values - IPv4 Route
-    ipv4_route_prefix_network_address = "{{{{lan_vpn_ipv4Route_{}_prefix_networkAddress}}}}"
-    ipv4_route_prefix_subnet_mask = "{{{{lan_vpn_ipv4Route_{}_prefix_subnetMask}}}}"
-    ipv4_route_next_hop_address = "{{{{lan_vpn_ipv4Route_{}_nextHop_{}_address}}}}"
-    ipv4_route_next_hop_administrative_distance = "{{{{lan_vpn_ipv4Route_{}_nextHop_{}_administrativeDistance}}}}"
-
-    # Default Values - Service
-    service_ipv4_addresses = "{{{{lan_vpn_service_{}_ipv4Addresses}}}}"
-
-    # Default Values - NAT
-    nat_natpool_name = "{{{{lan_vpn_nat_{}_natpoolName}}}}"
-    nat_prefix_length = "{{{{lan_vpn_nat_{}_prefixLength}}}}"
-    nat_range_start = "{{{{lan_vpn_nat_{}_rangeStart}}}}"
-    nat_range_end = "{{{{lan_vpn_nat_{}_rangeEnd}}}}"
-    nat_overload = "{{{{lan_vpn_nat_{}_overload}}}}"
-    nat_direction = "{{{{lan_vpn_nat_{}_direction}}}}"
-
-    # Default Values - Port Forwarding
-    nat_port_foward_natpool_name = "{{{{lan_vpn_natPortForward_{}_natpoolName}}}}"
-    nat_port_foward_translate_port = "{{{{lan_vpn_natPortForward_{}_translatePort}}}}"
-    nat_port_foward_translated_source_ip = "{{{{lan_vpn_natPortForward_{}_translatedSourceIp}}}}"
-    nat_port_foward_source_port = "{{{{lan_vpn_natPortForward_{}_sourcePort}}}}"
-    nat_port_foward_source_ip = "{{{{lan_vpn_natPortForward_{}_sourceIp}}}}"
-    nat_port_foward_protocol = "{{{{lan_vpn_natPortForward_{}_protocol}}}}"
-
-    # Default Values - Static NAT
-    static_nat_pool_name = "{{{{lan_vpn__staticNat_{}_poolName}}}}"
-    static_nat_source_ip = "{{{{lan_vpn_staticNat_{}_sourceIp}}}}"
-    static_nat_translated_source_ip = "{{{{lan_vpn_staticNat_{}_translatedSourceIp}}}}"
-    static_nat_direction = "{{{{lan_vpn_staticNat_{}_direction}}}}"
-
-    # Default Values - NAT64
-    nat64_v4_pool_name = "{{{{lan_vpn_nat64_{}_v4_poolName}}}}"
-    nat64_v4_pool_range_start = "{{{{lan_vpn_nat64_{}_v4_poolRangeStart}}}}"
-    nat64_v4_pool_range_end = "{{{{lan_vpn_nat64_{}_v4_poolRangeEnd}}}}"
-    nat64_v4_pool_overload = "{{{{lan_vpn_nat64_{}_v4_poolOverload}}}}"
-
     def create_parcel(self, name: str, description: str, template_values: dict) -> LanVpnParcel:
         """
         Creates a parcel from VPN family object based on the provided parameters.
 
         Args:
             name (str): The name of the parcel.
             description (str): The description of the parcel.
             template_values (dict): A dictionary containing the template values.
 
         Returns:
             VPN: The created VPN object.
         """
-        values = deepcopy(template_values)
-        self.configure_vpn_id(values)
-        self.configure_vpn_name(values)
-        self.configure_natpool(values)
-        self.configure_port_forwarding(values)
-        self.configure_static_nat(values)
-        self.configure_nat64(values)
-        self.configure_omp(values)
-        self.configure_dns(values)
-        self.configure_hostname_mapping(values)
-        self.configure_service(values)
-        self.configure_ipv4_route(values)
-        self.configure_ipv6_route(values)
-        self.configure_routes(values)
-        self.configure_route_leaks(values)
-        self.cleanup_keys(values)
-        return LanVpnParcel(**self.prepare_parcel_values(name, description, values))  # type: ignore
-
-    def prepare_parcel_values(self, name: str, description: str, values: dict) -> dict:
-        return {
-            "parcel_name": name,
-            "parcel_description": description,
-            **values,
-        }
-
-    def cleanup_keys(self, values: dict) -> None:
-        for key in self.delete_keys:
-            values.pop(key, None)
-
-    def configure_vpn_name(self, values: dict) -> None:
-        if vpn_name := values.get("name", None):
-            values["vpn_name"] = vpn_name
-
-    def configure_vpn_id(self, values: dict) -> None:
-        if vpn_id := values.get("vpn_id"):
-            vpn_id_value = int(vpn_id.value)
-            values["vpn_id"] = as_global(vpn_id_value)
-
-    def configure_dns(self, values: dict) -> None:
-        if dns := values.get("dns", []):
-            dns_ipv4 = DnsIPv4()
-            for entry in dns:
-                if entry["role"] == "primary":
-                    dns_ipv4.primary_dns_address_ipv4 = entry["dns_addr"]
-                elif entry["role"] == "secondary":
-                    dns_ipv4.secondary_dns_address_ipv4 = entry["dns_addr"]
-            values["dns"] = dns_ipv4
-
-    def configure_hostname_mapping(self, values: dict) -> None:
-        if host := values.get("host", []):
-            host_mapping_items = []
-            for entry in host:
-                host_mapping_item = HostMapping(
-                    host_name=entry["hostname"],
-                    list_of_ip=self._get_list_of_ips(entry),
-                )
-                host_mapping_items.append(host_mapping_item)
-            values["new_host_mapping"] = host_mapping_items
-
-    def _get_list_of_ips(self, entry) -> Global[List[IPvAnyAddress]]:
-        # Feature Template payload has space in ip string, so we need to strip it
-        list_of_ips = entry.get("ip", Global[List[str]](value=[])).value
-        return Global[List[IPvAnyAddress]](value=[IPvAnyAddress(ip.strip()) for ip in list_of_ips])
-
-    def configure_service(self, values: dict) -> None:
-        if service := values.get("service", []):
-            service_items = []
-            for service_i, entry in enumerate(service):
-                service_item = Service(
-                    service_type=as_global(entry["svc_type"].value, ServiceType),
-                    ipv4_addresses=entry.get("address", as_variable(self.service_ipv4_addresses.format(service_i + 1))),
-                    tracking=entry.get("track_enable", as_default(True)),
-                )
-                service_items.append(service_item)
-            values["service"] = service_items
-
-    def configure_natpool(self, values: dict) -> None:
-        if natpool := values.get("nat", {}).get("natpool", []):
-            nat_items = []
-            for nat_i, entry in enumerate(natpool):
-                direction = entry.get("direction")
-                if direction:
-                    direction = as_global(direction.value, Direction)
-                else:
-                    direction = as_variable(self.nat_direction.format(nat_i + 1))
-                nat_items.append(
-                    NatPool(
-                        nat_pool_name=entry.get("name", as_variable(self.nat_natpool_name.format(nat_i + 1))),
-                        prefix_length=entry.get("prefix_length", as_variable(self.nat_prefix_length.format(nat_i + 1))),
-                        range_start=entry.get("range_start", as_variable(self.nat_range_start.format(nat_i + 1))),
-                        range_end=entry.get("range_end", as_variable(self.nat_range_end.format(nat_i + 1))),
-                        overload=entry.get("overload", as_default(True)),
-                        direction=direction,
-                    )
+        data = deepcopy(template_values)
+
+        vpn_name = data.get("name")
+        vpn_id = data.get("vpn_id")
+        omp_admin_distance_ipv4 = data.get("omp_admin_distance_ipv4")
+        omp_admin_distance_ipv6 = data.get("omp_admin_distance_ipv6")
+        dns_ipv4, dns_ipv6 = self.parse_dns(data.get("dns", []))
+        new_host_mapping = self.parse_host_mapping(data.get("host", []))
+        net_port_forwarding = self.parse_port_forwarding(data.get("nat", {}).get("port_forward", []))
+        nat_pool = self.parse_natpool(data.get("nat", {}).get("natpool", []))
+        static_nat = self.parse_static_nat(data.get("nat", {}).get("static", []))
+        nat_64_v4_pool = self.parse_nat64_v4_pool(data.get("nat64", {}).get("v4", {}).get("pool", []))
+        service = self.parse_service(data.get("service", []))
+
+        self.parse_omp(data)
+        self.parse_ipv4_route(data)
+        self.parse_ipv6_route(data)
+        self.parse_routes(data)
+        self.parse_route_leaks(data)
+
+        omp_advertise_ipv4 = data.get("omp_advertise_ipv4")
+        omp_advertise_ipv6 = data.get("omp_advertise_ipv6")
+        route_gre = data.get("route_gre")
+        route_service = data.get("route_service")
+        ipsec_route = data.get("ipsec_route")
+        route_leak_from_global = data.get("route_leak_from_global")
+        route_leak_from_service = data.get("route_leak_from_service")
+        route_leak_between_services = data.get("route_leak_between_services")
+        mpls_vpn_ipv4_route_target = data.get("mpls_vpn_ipv4_route_target")
+        mpls_vpn_ipv6_route_target = data.get("mpls_vpn_ipv6_route_target")
+        enable_sdra = data.get("enable_sdra")
+        ipv6_route = data.get("ipv6_route")
+        ipv4_route = data.get("ipv4_route")
+
+        payload = create_dict_without_none(
+            parcel_name=name,
+            parcel_description=description,
+            vpn_name=vpn_name,
+            vpn_id=vpn_id,
+            omp_admin_distance_ipv4=omp_admin_distance_ipv4,
+            omp_admin_distance_ipv6=omp_admin_distance_ipv6,
+            dns_ipv4=dns_ipv4,
+            dns_ipv6=dns_ipv6,
+            new_host_mapping=new_host_mapping,
+            net_port_forwarding=net_port_forwarding,
+            nat_pool=nat_pool,
+            static_nat=static_nat,
+            nat_64_v4_pool=nat_64_v4_pool,
+            service=service,
+            omp_advertise_ipv4=omp_advertise_ipv4,
+            omp_advertise_ipv6=omp_advertise_ipv6,
+            route_gre=route_gre,
+            route_service=route_service,
+            ipsec_route=ipsec_route,
+            route_leak_from_global=route_leak_from_global,
+            route_leak_from_service=route_leak_from_service,
+            route_leak_between_services=route_leak_between_services,
+            mpls_vpn_ipv4_route_target=mpls_vpn_ipv4_route_target,
+            mpls_vpn_ipv6_route_target=mpls_vpn_ipv6_route_target,
+            enable_sdra=enable_sdra,
+            ipv6_route=ipv6_route,
+            ipv4_route=ipv4_route,
+        )
+
+        return LanVpnParcel(**payload)
+
+    def parse_dns(self, dns: dict) -> Tuple[DNSIPv4, DNSIPv6]:
+        dns_ipv4 = DNSIPv4()
+        dns_ipv6 = DNSIPv6()
+        for dns_entry in dns:
+            dns_address = dns_entry.get("dns_addr", Default[None](value=None))
+            if dns_entry["role"].value == "primary":
+                dns_ipv4.primary_dns_address_ipv4 = dns_address
+            elif dns_entry["role"].value == "secondary":
+                dns_ipv4.secondary_dns_address_ipv4 = dns_address
+            elif dns_entry["role"].value == "primaryv6":
+                dns_ipv6.primary_dns_address_ipv6 = dns_address
+            elif dns_entry["role"].value == "secondaryv6":
+                dns_ipv6.secondary_dns_address_ipv6 = dns_address
+        return dns_ipv4, dns_ipv6
+
+    def parse_host_mapping(self, hosts: List[Dict]) -> Optional[List[HostMapping]]:
+        if not hosts:
+            return None
+
+        hosts_cleared = [h for h in hosts if self.is_host_mapping_parsable(h)]
+
+        return [
+            HostMapping(
+                host_name=host["hostname"],
+                list_of_ips=self.parse_list_of_ip(host),
+            )
+            for host in hosts_cleared
+        ]
+
+    def parse_list_of_ip(self, host: Dict) -> Union[Variable, Global[List[str]]]:
+        list_of_ips = host["ip"]
+        if isinstance(list_of_ips, Variable):
+            return list_of_ips
+
+        # ["34.199.1.194"," 34.204.213.179], extra space before the ip is a bug in the feature template
+        return Global[List[str]](value=[ip.strip() for ip in list_of_ips.value])
+
+    def is_host_mapping_parsable(self, host: Dict) -> bool:
+        return "ip" in host and "hostname" in host
+
+    def parse_service(self, service: List[Dict]) -> Optional[List[Service]]:
+        if not service:
+            return None
+        service_items = []
+        for entry in service:
+            service_type = entry.get("svc_type")
+            if isinstance(service_type, Global):
+                service_type = as_global(service_type.value, ServiceType)
+            service_item = Service(
+                service_type=service_type,
+                ipv4_addresses=entry.get("address"),  # type: ignore
+                tracking=entry.get("track_enable", as_default(True)),
+            )
+            service_items.append(service_item)
+        return service_items
+
+    def parse_natpool(self, natpool: List[Dict]) -> Optional[List[NatPool]]:
+        if not natpool:
+            return None
+        nat_items = []
+        for entry in natpool:
+            direction = entry.get("direction")
+            nat_pool_name = entry.get("name")
+            prefix_length = entry.get("prefix_length")
+            range_start = entry.get("range_start")
+            range_end = entry.get("range_end")
+            overload = entry.get("overload", as_default(True))
+
+            if (
+                nat_pool_name is None
+                or prefix_length is None
+                or range_start is None
+                or range_end is None
+                or direction is None
+            ):
+                continue
+
+            if isinstance(direction, Global):
+                direction = as_global(str(direction.value), Direction)
+
+            nat_items.append(
+                NatPool(
+                    nat_pool_name=nat_pool_name,
+                    prefix_length=prefix_length,
+                    range_start=range_start,
+                    range_end=range_end,
+                    overload=overload,
+                    direction=direction,
                 )
-            values["nat_pool"] = nat_items
+            )
+        return nat_items
 
-    def configure_port_forwarding(self, values: dict) -> None:
-        if port_forward := values.get("nat", {}).get("port_forward", []):
-            nat_port_forwarding_items = []
-            for net_port_foward_i, entry in enumerate(port_forward):
-                protocol = entry.get("proto")
-                if protocol:
-                    protocol = as_global(protocol.value.upper(), NATPortForwardProtocol)
-                else:
-                    protocol = as_variable(self.nat_port_foward_protocol.format(net_port_foward_i + 1))
-                nat_port_forwarding_items.append(
-                    NatPortForward(
-                        nat_pool_name=entry.get(
-                            "pool_name", as_variable(self.nat_port_foward_natpool_name.format(net_port_foward_i + 1))
-                        ),
-                        source_port=entry.get(
-                            "source_port", as_variable(self.nat_port_foward_source_port.format(net_port_foward_i + 1))
-                        ),
+    def parse_port_forwarding(self, port_forward: List[Dict]) -> Optional[List[NatPortForward]]:
+        if not port_forward:
+            return None
+        nat_port_forwarding_items = []
+        for entry in port_forward:
+            protocol = entry.get("proto")
+            if isinstance(protocol, Global):
+                protocol = as_global(protocol.value.upper(), NATPortForwardProtocol)
+            nat_port_forwarding_items.append(
+                NatPortForward(
+                    **create_dict_without_none(
+                        nat_pool_name=entry.get("pool_name"),
+                        source_port=entry.get("source_port"),
                         translate_port=entry.get(
                             "translate_port",
-                            as_variable(self.nat_port_foward_translate_port.format(net_port_foward_i + 1)),
-                        ),
-                        source_ip=entry.get(
-                            "source_ip", as_variable(self.nat_port_foward_source_ip.format(net_port_foward_i + 1))
                         ),
+                        source_ip=entry.get("source_ip"),
                         translated_source_ip=entry.get(
                             "translate_ip",
-                            as_variable(self.nat_port_foward_translated_source_ip.format(net_port_foward_i + 1)),
                         ),
                         protocol=protocol,
                     )
                 )
-            values["nat_port_forwarding"] = nat_port_forwarding_items
+            )
+        return nat_port_forwarding_items
 
-    def configure_static_nat(self, values: dict) -> None:
-        if static_nat := values.get("nat", {}).get("static", []):
-            static_nat_items = []
-            for static_nat_i, entry in enumerate(static_nat):
-                static_nat_direction = entry.get("static_nat_direction")
-                if static_nat_direction:
-                    static_nat_direction = as_global(static_nat_direction.value, Direction)
-                else:
-                    static_nat_direction = as_variable(self.static_nat_direction.format(static_nat_i + 1))
-                static_nat_items.append(
-                    StaticNat(
-                        nat_pool_name=entry.get(
-                            "pool_name", as_variable(self.static_nat_pool_name.format(static_nat_i + 1))
-                        ),
-                        source_ip=entry.get(
-                            "source_ip", as_variable(self.static_nat_source_ip.format(static_nat_i + 1))
-                        ),
-                        translated_source_ip=entry.get(
-                            "translate_ip", as_variable(self.static_nat_translated_source_ip.format(static_nat_i + 1))
-                        ),
-                        static_nat_direction=static_nat_direction,
-                    )
+    def parse_static_nat(self, static_nat: List[Dict]) -> Optional[List[StaticNat]]:
+        if not static_nat:
+            return None
+        static_nat_items = []
+        for entry in static_nat:
+            static_nat_direction = entry.get("static_nat_direction")
+            nat_pool_name = entry.get("pool_name")
+            source_ip = entry.get("source_ip")
+            translated_source_ip = entry.get("translate_ip")
+
+            if (
+                static_nat_direction is None
+                or nat_pool_name is None
+                or source_ip is None
+                or translated_source_ip is None
+            ):
+                continue
+
+            if isinstance(static_nat_direction, Global):
+                static_nat_direction = as_global(static_nat_direction.value, Direction)
+
+            static_nat_items.append(
+                StaticNat(
+                    nat_pool_name=nat_pool_name,
+                    source_ip=source_ip,
+                    translated_source_ip=translated_source_ip,
+                    static_nat_direction=static_nat_direction,
+                )  # type: ignore
+            )
+        return static_nat_items
+
+    def parse_nat64_v4_pool(self, nat64pool: List[Dict]) -> Optional[List[Nat64v4Pool]]:
+        if not nat64pool:
+            return None
+        return [
+            Nat64v4Pool(
+                **create_dict_without_none(
+                    nat64_v4_pool_name=entry.get("name"),
+                    nat64_v4_pool_range_start=entry.get("start_address"),
+                    nat64_v4_pool_range_end=entry.get("end_address"),
+                    nat64_v4_pool_overload=entry.get("overload", as_default(False)),
                 )
-            values["static_nat"] = static_nat_items
+            )
+            for entry in nat64pool  # type: ignore
+        ]
 
-    def configure_nat64(self, values: dict) -> None:
-        if nat64pool := values.get("nat64", {}).get("v4", {}).get("pool", []):
-            nat64_items = []
-            for nat64pool_i, entry in enumerate(nat64pool):
-                nat64_items.append(
-                    Nat64v4Pool(
-                        nat64_v4_pool_name=entry.get(
-                            "name", as_variable(self.nat64_v4_pool_name.format(nat64pool_i + 1))
-                        ),
-                        nat64_v4_pool_range_start=entry.get(
-                            "start_address", as_variable(self.nat64_v4_pool_range_start.format(nat64pool_i + 1))
-                        ),
-                        nat64_v4_pool_range_end=entry.get(
-                            "end_address", as_variable(self.nat64_v4_pool_range_end.format(nat64pool_i + 1))
-                        ),
-                        nat64_v4_pool_overload=entry.get(
-                            "overload", as_variable(self.nat64_v4_pool_overload.format(nat64pool_i + 1))
-                        ),
-                    )
+    def parse_ipv4_route(self, values: dict) -> None:
+        ipv4_route = values.get("ip", {}).get("route", [])
+        if not ipv4_route:
+            return
+        if len(ipv4_route) == 1 and ipv4_route[0] == {}:
+            # Sometimes it parses as a list with an empty dictionary
+            return
+
+        ipv4_route_items = []
+        for route in ipv4_route:
+            prefix: Union[Global, Variable] = route.pop("prefix", None)
+            if prefix.option_type == OptionType.GLOBAL:
+                interface = IPv4Interface(prefix.value)
+                route_prefix = RoutePrefix(
+                    ip_address=as_global(interface.network.network_address),
+                    subnet_mask=as_global(str(interface.netmask)),
                 )
-            values["nat64_v4_pool"] = nat64_items
 
-    def configure_ipv4_route(self, values: dict) -> None:
-        if ipv4_route := values.get("ip", {}).get("route", []):
-            ipv4_route_items = []
-            for route_i, route in enumerate(ipv4_route):
-                prefix: Union[Global, Variable] = route.pop("prefix", None)
-                if prefix.option_type == OptionType.GLOBAL:
-                    interface = IPv4Interface(prefix.value)
-                    route_prefix = RoutePrefix(
-                        ip_address=as_global(interface.network.network_address),
-                        subnet_mask=as_global(str(interface.netmask)),
-                    )
+            elif prefix.option_type == OptionType.VARIABLE:
+                route_prefix = RoutePrefix(
+                    ip_address=prefix,
+                    subnet_mask=as_global("0.0.0.0"),
+                )
+            ip_route_item = None
+            if "next_hop" in route:
+                next_hop_items = []
+                for next_hop in route.pop("next_hop", []):
+                    address = next_hop.pop("address", None)
+                    distance = next_hop.pop("distance", as_default(1))
+                    if address is None:
+                        continue
 
-                elif prefix.option_type == OptionType.VARIABLE:
-                    route_prefix = RoutePrefix(
-                        ip_address=prefix,
-                        subnet_mask=as_global("0.0.0.0"),
-                    )
-                ip_route_item = None
-                if "next_hop" in route:
-                    next_hop_items = []
-                    for next_hop_i, next_hop in enumerate(route.pop("next_hop", [])):
-                        next_hop_items.append(
-                            IPv4RouteGatewayNextHop(
-                                address=next_hop.pop(
-                                    "address",
-                                    as_variable(self.ipv4_route_next_hop_address.format(route_i + 1, next_hop_i + 1)),
-                                ),
-                                distance=next_hop.pop(
-                                    "distance",
-                                    as_variable(
-                                        self.ipv4_route_next_hop_administrative_distance.format(
-                                            route_i + 1, next_hop_i + 1
-                                        )
-                                    ),
-                                ),
-                            )
+                    next_hop_items.append(
+                        IPv4RouteGatewayNextHop(
+                            address=address,
+                            distance=distance,
                         )
-                    ip_route_item = NextHopRouteContainer(next_hop_container=NextHopContainer(next_hop=next_hop_items))
-                elif "next_hop_with_track" in route:
-                    next_hop_with_track_items = []
-                    for next_hop_with_track in route.pop("next_hop_with_track", []):
-                        tracker = next_hop_with_track.pop("tracker")
-                        if tracker:
-                            logger.warning(
-                                f"Tracker can be any value in UX1.0, but must be UUID in UX2.0. Current value {tracker}"
-                            )
-
-                        payload = create_dict_without_none(
-                            address=next_hop_with_track.pop("address", None),
-                            distance=next_hop_with_track.pop("distance", None),
+                    )
+                ip_route_item = NextHopRouteContainer(next_hop_container=NextHopContainer(next_hop=next_hop_items))
+            elif "next_hop_with_track" in route:
+                next_hop_with_track_items = []
+                for next_hop_with_track in route.pop("next_hop_with_track", []):
+                    tracker = next_hop_with_track.pop("tracker")
+                    if tracker:
+                        logger.warning(
+                            f"Tracker can be any value in UX1.0, but must be UUID in UX2.0. Current value {tracker}"
                         )
 
-                        next_hop_with_track_items.append(IPv4RouteGatewayNextHopWithTracker(**payload))
+                    address = next_hop_with_track.pop("address", None)
+                    distance = next_hop_with_track.pop("distance", as_default(1))
+                    if address is None:
+                        continue
 
-                    ip_route_item = NextHopRouteContainer(
-                        next_hop_container=NextHopContainer(next_hop_with_tracker=next_hop_with_track_items)
-                    )
-                elif "vpn" in route:
-                    ip_route_item = StaticRouteVPN(  # type: ignore
-                        vpn=as_global(True),
-                    )
-                elif "dhcp" in route:
-                    ip_route_item = DHCP(  # type: ignore
-                        dhcp=as_global(True),
-                    )
-                else:
-                    # Let's assume it's a static route with enabled VPN
-                    ip_route_item = StaticRouteVPN(  # type: ignore
-                        vpn=as_global(True),
+                    next_hop_with_track_items.append(
+                        IPv4RouteGatewayNextHopWithTracker(address=address, distance=distance)
                     )
-                ipv4_route_items.append(
-                    StaticRouteIPv4(prefix=route_prefix, one_of_ip_route=ip_route_item)  # type: ignore
+
+                ip_route_item = NextHopRouteContainer(
+                    next_hop_container=NextHopContainer(next_hop_with_tracker=next_hop_with_track_items)
+                )
+            elif "vpn" in route:
+                ip_route_item = StaticRouteVPN(  # type: ignore
+                    vpn=as_global(True),
+                )
+            elif "dhcp" in route:
+                ip_route_item = DHCP(  # type: ignore
+                    dhcp=as_global(True),
+                )
+            else:
+                # Let's assume it's a static route with enabled VPN
+                ip_route_item = StaticRouteVPN(  # type: ignore
+                    vpn=as_global(True),
                 )
-            values["ipv4_route"] = ipv4_route_items
+            ipv4_route_items.append(StaticRouteIPv4(prefix=route_prefix, one_of_ip_route=ip_route_item))  # type: ignore
+        values["ipv4_route"] = ipv4_route_items
 
-    def configure_ipv6_route(self, values: dict) -> None:
+    def parse_ipv6_route(self, values: dict) -> None:
         if ipv6_route := values.get("ipv6", {}).get("route", []):
             ipv6_route_items = []
             for route in ipv6_route:
                 ipv6_interface = IPv6Interface(route.get("prefix").value)
                 route_prefix = RoutePrefix(
                     ip_address=as_global(ipv6_interface.network.network_address),
                     subnet_mask=as_global(str(ipv6_interface.netmask)),
@@ -632,23 +635,23 @@
                     static_route_interfaces = [IPv6StaticRouteInterface(**entry) for entry in route_interface]
                     ipv6_route_item = InterfaceRouteIPv6Container(
                         interface_container=InterfaceIPv6Container(ipv6_static_route_interface=static_route_interfaces)
                     )
                 ipv6_route_items.append(StaticRouteIPv6(prefix=route_prefix, one_of_ip_route=ipv6_route_item))
             values["ipv6_route"] = ipv6_route_items
 
-    def configure_omp(self, values: dict) -> None:
+    def parse_omp(self, values: dict) -> None:
         for omp in self.omp_mapping.keys():
             if omp_advertises := values.get("omp", {}).get(omp, []):
                 pydantic_model_omp = self.omp_mapping[omp].ux2_model_omp
                 pydantic_model_prefix = self.omp_mapping[omp].ux2_model_prefix
                 pydantic_field = self.omp_mapping[omp].ux2_field
-                self._configure_omp(values, omp_advertises, pydantic_model_omp, pydantic_model_prefix, pydantic_field)
+                self._parse_omp(values, omp_advertises, pydantic_model_omp, pydantic_model_prefix, pydantic_field)
 
-    def _configure_omp(
+    def _parse_omp(
         self, values: dict, omp_advertises: list, pydantic_model_omp, pydantic_model_prefix, pydantic_field
     ) -> None:
         omp_advertise_items = []
         for entry in omp_advertises:
             prefix_list_items = []
             for prefix_entry in entry.get("prefix_list", []):
                 prefix_list_items.append(
@@ -666,40 +669,40 @@
                 pydantic_model_omp(
                     omp_protocol=as_global(entry["protocol"].value, pydantic_model_protocol),
                     prefix_list=prefix_list_items if prefix_list_items else None,
                 )
             )
         values[pydantic_field] = omp_advertise_items
 
-    def configure_routes(self, values: dict) -> None:
+    def parse_routes(self, values: dict) -> None:
         for route in self.routes_mapping.keys():
             if routes := values.get("ip", {}).get(route, []):
                 pydantic_model = self.routes_mapping[route].ux2_model
                 pydantic_field = self.routes_mapping[route].ux2_field
-                self._configure_route(values, routes, pydantic_model, pydantic_field)
+                self._parse_route(values, routes, pydantic_model, pydantic_field)
 
-    def _configure_route(self, values: dict, routes: list, pydantic_model, pydantic_field) -> None:
+    def _parse_route(self, values: dict, routes: list, pydantic_model, pydantic_field) -> None:
         items = []
         for route in routes:
             ipv4_interface = IPv4Interface(route.get("prefix").value)
             service_prefix = AddressWithMask(
                 address=as_global(ipv4_interface.network.network_address),
                 mask=as_global(str(ipv4_interface.netmask)),
             )
             items.append(pydantic_model(prefix=service_prefix, vpn=route.get("vpn")))
         values[pydantic_field] = items
 
-    def configure_route_leaks(self, values: dict) -> None:
+    def parse_route_leaks(self, values: dict) -> None:
         for leak in self.route_leaks_mapping.keys():
             if route_leaks := values.get(leak, []):
                 pydantic_model = self.route_leaks_mapping[leak].ux2_model
                 pydantic_field = self.route_leaks_mapping[leak].ux2_field
-                self._configure_leak(values, route_leaks, pydantic_model, pydantic_field)
+                self._parse_leak(values, route_leaks, pydantic_model, pydantic_field)
 
-    def _configure_leak(self, values: dict, route_leaks: list, pydantic_model, pydantic_field) -> None:
+    def _parse_leak(self, values: dict, route_leaks: list, pydantic_model, pydantic_field) -> None:
         items = []
         for rl in route_leaks:
             redistribute_items = []
             for redistribute_item in rl.get("redistribute_to", []):
                 redistribute_items.append(
                     RedistributeToService(
                         protocol=as_global(redistribute_item["protocol"].value, RedistributeToServiceProtocol),
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/cellular.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ethernet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
+import logging
 from copy import deepcopy
 from typing import Dict, List, Optional, Union
 
 from catalystwan.api.configuration_groups.parcel import Default, Global, Variable, as_default, as_global
 from catalystwan.models.common import CarrierType, EncapType, EthernetDuplexMode, EthernetNatType, Speed
 from catalystwan.models.configuration.feature_profile.common import (
     AclQos,
@@ -26,24 +28,28 @@
     Static,
     TlocExtensionGreFrom,
     Tunnel,
 )
 from catalystwan.utils.config_migration.converters.feature_template.helpers import create_dict_without_none
 from catalystwan.utils.config_migration.steps.constants import WAN_VPN_ETHERNET
 
+logger = logging.getLogger(__name__)
+
 
 class WanInterfaceEthernetTemplateConverter:
     supported_template_types = (WAN_VPN_ETHERNET,)
 
     def create_parcel(self, name: str, description: str, template_values: dict) -> InterfaceEthernetParcel:
         data = deepcopy(template_values)
 
         encapsulation = self.parse_encapsulations(data.get("tunnel_interface", {}).get("encapsulation", []))
         interface_name = data["if_name"]
-        interface_description = data.get("description")
+        interface_description = data.get(
+            "description", as_global(description)
+        )  # Edge case where model doesn't have description but its required
         interface_ip_address = self.parse_interface_ip_address(data)
         tunnel_interface = self.parse_tunnel_interface(data)
         shutdown = data.get("shutdown")
         nat = self.parse_nat(data)
         nat_attributes_ipv4 = self.configure_network_address_translation(data)
         acl_qos = self.parse_acl_qos(data)
         advanced = self.parse_advanced(data)
@@ -56,16 +62,16 @@
         intf_ip_v6_address = self.parse_ipv6_address(data)
         block_non_source_ip = data.get("block_non_source_ip")
         service_provider = data.get("service_provider")
         dhcp_helper = data.get("dhcp_helper")
         tunnel = self.parse_tunnel(data)
 
         payload = create_dict_without_none(
-            name=name,
-            description=description,
+            parcel_name=name,
+            parcel_description=description,
             encapsulation=encapsulation,
             interface_name=interface_name,
             interface_description=interface_description,
             interface_ip_address=interface_ip_address,
             tunnel_interface=tunnel_interface,
             shutdown=shutdown,
             nat=nat,
@@ -103,23 +109,23 @@
         if data.get("tunnel_interface"):
             return as_global(True)
         return None
 
     def parse_interface_ip_address(self, data: Dict) -> Union[InterfaceDynamicIPv4Address, InterfaceStaticIPv4Address]:
         ip_address = data.get("ip", {})
 
-        if "address" in ip_address:
+        if "address" in ip_address and ip_address["address"].value != "":
             return InterfaceStaticIPv4Address(
                 static=StaticIPv4AddressConfig(
                     primary_ip_address=self.get_static_ipv4_address(ip_address),
                     secondary_ip_address=self.get_secondary_static_ipv4_address(ip_address),
                 )
             )
 
-        if "dhcp_client" in ip_address:
+        elif "dhcp_client" in ip_address:
             return InterfaceDynamicIPv4Address(
                 dynamic=DynamicDhcpDistance(dynamic_dhcp_distance=ip_address.get("dhcp_distance", as_default(1)))
             )
 
         return InterfaceDynamicIPv4Address(dynamic=DynamicDhcpDistance())
 
     def get_static_ipv4_address(self, address_configuration: dict) -> StaticIPv4Address:
@@ -159,14 +165,16 @@
         nat_type = nat.get("nat_choice")
         if not nat_type:
             if nat_pool:
                 nat_type = Global[EthernetNatType](value="pool")
             else:
                 nat_type = Global[EthernetNatType](value="loopback")
 
+        nat_type = as_global(nat_type.value, EthernetNatType)
+
         payload = create_dict_without_none(
             nat_type=nat_type,
             nat_pool=nat_pool,
             udp_timeout=nat.get("udp_timeout"),
             tcp_timeout=nat.get("tcp_timeout"),
             new_static_nat=nat.get("static"),
         )
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/gre.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/ipsec.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/multilink.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/protocol_over.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wan/t1e1serial.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/converters/feature_template/wireless_lan.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/factories/feature_profile_api.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/feature_profile_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 from catalystwan.api.feature_profile_api import (
     CliFeatureProfileAPI,
     OtherFeatureProfileAPI,
     PolicyObjectFeatureProfileAPI,
     ServiceFeatureProfileAPI,
     SystemFeatureProfileAPI,
+    TopologyFeatureProfileAPI,
     TransportFeatureProfileAPI,
 )
 from catalystwan.models.configuration.feature_profile.common import ProfileType
 from catalystwan.session import ManagerSession
 
 FEATURE_PROFILE_API_MAPPING: Mapping[ProfileType, Callable] = {
     "system": SystemFeatureProfileAPI,
     "other": OtherFeatureProfileAPI,
     "policy-object": PolicyObjectFeatureProfileAPI,
     "service": ServiceFeatureProfileAPI,
     "transport": TransportFeatureProfileAPI,
     "cli": CliFeatureProfileAPI,
+    "topology": TopologyFeatureProfileAPI,
 }
 
 FeatureProfile = Union[
     SystemFeatureProfileAPI,
     OtherFeatureProfileAPI,
     PolicyObjectFeatureProfileAPI,
     ServiceFeatureProfileAPI,
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/factories/parcel_pusher.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/factories/parcel_pusher.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/config_migration/steps/constants.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/config_migration/steps/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Copyright 2023 Cisco Systems, Inc. and its affiliates
 from typing import Dict, Union
 
 VPN_MANAGEMENT = "cisco_vpn_management"
 VPN_TRANSPORT = "cisco_vpn_transport"
 VPN_SERVICE = "cisco_vpn_service"
 
 
@@ -17,29 +18,39 @@
     "cisco_vpn_interface",
     "vpn-vedge-interface-gre",
     "vpn-vsmart-interface",
     "vpn-vedge-interface",
     "vpn-vmanage-interface",
     "vpn-vedge-interface-ipsec",
     "vpn-cedge-interface-multilink-controller",
+    "cisco_bgp",
+    "bgp",
+    "cisco_ospfv3",
+    "cisco_ospf",
 ]
 
 NO_SUBSTITUTE_ERROR = "NO_SUBSTITUTE_ERROR"
 NO_SUBSTITUTE_VPN_MANAGEMENT_SVI = (
     "NO_SUBSTITUTE_ERROR: UX1.0 -> We can attach SVI to vpn 512, UX2.0 -> There is no SVI parcel for vpn 512"
 )
 
 MANAGEMENT_VPN_ETHERNET = "management/vpn/interface/ethernet"
 
+WAN_BGP = "WAN_BGP"
+WAN_OSPF = "WAN_OSPF"
+WAN_OSPFV3 = "WAN_OSPFV3"
 WAN_VPN_GRE = "wan/vpn/interface/gre"
 WAN_VPN_IPSEC = "wan/vpn/interface/ipsec"
 WAN_VPN_SVI = "wan/vpn/interface/svi"
 WAN_VPN_ETHERNET = "wan/vpn/interface/ethernet"
 WAN_VPN_MULTILINK = "wan/vpn/interface/multilink"
 
+LAN_BGP = "LAN_BGP"
+LAN_OSPF = "LAN_OSPF"
+LAN_OSPFV3 = "LAN_OSPFV3"
 LAN_VPN_GRE = "lan/vpn/interface/gre"
 LAN_VPN_IPSEC = "lan/vpn/interface/ipsec"
 LAN_VPN_SVI = "lan/vpn/interface/svi"
 LAN_VPN_ETHERNET = "lan/vpn/interface/ethernet"
 LAN_VPN_MULTILINK = "lan/vpn/interface/multilink"
 
 VPN_TEMPLATE_MAPPINGS: Dict[str, Dict[str, Union[str, Dict[str, str]]]] = {
@@ -51,35 +62,45 @@
             "vpn-vedge-interface": MANAGEMENT_VPN_ETHERNET,
             "vpn-vmanage-interface": MANAGEMENT_VPN_ETHERNET,
         },
         "suffix": "_MANAGEMENT",
     },
     VPN_TRANSPORT: {
         "mapping": {
+            "cisco_bgp": WAN_BGP,
+            "bgp": WAN_BGP,
+            "cisco_ospf": WAN_OSPF,
+            "cisco_ospfv3": WAN_OSPFV3,
             "vpn-vedge-interface-gre": WAN_VPN_GRE,
             "cisco_vpn_interface_gre": WAN_VPN_GRE,
             "cisco_vpn_interface_ipsec": WAN_VPN_IPSEC,
             "vpn-interface-svi": WAN_VPN_SVI,
             "cisco_vpn_interface": WAN_VPN_ETHERNET,
             "vpn-vsmart-interface": WAN_VPN_ETHERNET,
             "vpn-vedge-interface": WAN_VPN_ETHERNET,
             "vpn-vmanage-interface": WAN_VPN_ETHERNET,
             "vpn-cedge-interface-multilink-controller": WAN_VPN_MULTILINK,
         },
         "suffix": "_TRANSPORT",
     },
     VPN_SERVICE: {
         "mapping": {
+            "cisco_bgp": LAN_BGP,
+            "bgp": LAN_BGP,
+            "cisco_ospf": LAN_OSPF,
+            "cisco_ospfv3": LAN_OSPFV3,
             "vpn-vedge-interface-gre": LAN_VPN_GRE,
             "cisco_vpn_interface": LAN_VPN_ETHERNET,
             "vpn-vsmart-interface": LAN_VPN_ETHERNET,
             "vpn-vedge-interface": LAN_VPN_ETHERNET,
             "vpn-vmanage-interface": LAN_VPN_ETHERNET,
             "cisco_vpn_interface_gre": LAN_VPN_GRE,
             "cisco_vpn_interface_ipsec": LAN_VPN_IPSEC,
             "vpn-interface-svi": LAN_VPN_SVI,
             "vpn-vedge-interface-ipsec": LAN_VPN_IPSEC,
             "vpn-cedge-interface-multilink-controller": LAN_VPN_MULTILINK,
         },
         "suffix": "_SERVICE",
     },
 }
+
+MULTI_PARCEL_FEATURE_TEMPLATES = [WAN_OSPFV3, LAN_OSPFV3]
```

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/creation_tools.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/creation_tools.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/dashboard.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/device_model.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/device_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/dict.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/dict.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/feature_template/choose_model.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/choose_model.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/feature_template/find_template_values.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/feature_template/find_template_values.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/operation_status.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/operation_status.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/timezone.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/timezone.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/utils/upgrades_helper.py` & `catalystwan-0.33.7.dev2/catalystwan/utils/upgrades_helper.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/version.py` & `catalystwan-0.33.7.dev2/catalystwan/version.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/vmanage_auth.py` & `catalystwan-0.33.7.dev2/catalystwan/vmanage_auth.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/catalystwan/workflows/tenant_migration.py` & `catalystwan-0.33.7.dev2/catalystwan/workflows/tenant_migration.py`

 * *Files identical despite different names*

### Comparing `catalystwan-0.33.7.dev1/pyproject.toml` & `catalystwan-0.33.7.dev2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalystwan"
-version = "0.33.7dev1"
+version = "0.33.7dev2"
 description = "Cisco Catalyst WAN SDK for Python"
 authors = ["kagorski <kagorski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/cisco-catalyst-wan-sdk"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `catalystwan-0.33.7.dev1/setup.py` & `catalystwan-0.33.7.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,29 @@
  'catalystwan.endpoints.configuration.policy.list',
  'catalystwan.endpoints.monitoring',
  'catalystwan.endpoints.real_time_monitoring',
  'catalystwan.endpoints.troubleshooting_tools',
  'catalystwan.integration_tests',
  'catalystwan.integration_tests.feature_profile.sdwan',
  'catalystwan.integration_tests.feature_profile.sdwan.topology',
+ 'catalystwan.integration_tests.profile_builder',
+ 'catalystwan.integration_tests.test_data',
  'catalystwan.models',
  'catalystwan.models.configuration',
  'catalystwan.models.configuration.feature_profile',
+ 'catalystwan.models.configuration.feature_profile.sdwan.acl',
  'catalystwan.models.configuration.feature_profile.sdwan.application_priority',
  'catalystwan.models.configuration.feature_profile.sdwan.cli',
  'catalystwan.models.configuration.feature_profile.sdwan.dns_security',
  'catalystwan.models.configuration.feature_profile.sdwan.embedded_security',
  'catalystwan.models.configuration.feature_profile.sdwan.other',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object.policy',
  'catalystwan.models.configuration.feature_profile.sdwan.policy_object.security',
+ 'catalystwan.models.configuration.feature_profile.sdwan.routing',
  'catalystwan.models.configuration.feature_profile.sdwan.service',
  'catalystwan.models.configuration.feature_profile.sdwan.service.lan',
  'catalystwan.models.configuration.feature_profile.sdwan.sig_security',
  'catalystwan.models.configuration.feature_profile.sdwan.system',
  'catalystwan.models.configuration.feature_profile.sdwan.topology',
  'catalystwan.models.configuration.feature_profile.sdwan.transport',
  'catalystwan.models.configuration.feature_profile.sdwan.transport.management',
@@ -93,15 +97,15 @@
  'requests-toolbelt>=1.0.0,<2.0.0',
  'requests>=2.27.1,<3.0.0',
  'tenacity>=8.1.0,<9.0.0',
  'typing-extensions>=4.6.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'catalystwan',
-    'version': '0.33.7.dev1',
+    'version': '0.33.7.dev2',
     'description': 'Cisco Catalyst WAN SDK for Python',
     'long_description': '<p align="center">\n  <a href="#"><img src="docs/images/catalystwan.svg" alt="Cisco Catalyst WAN SDK Logo" style="height:150px" />\n</p>\n\n[![Python-Supported](https://img.shields.io/static/v1?label=Python&logo=Python&color=3776AB&message=3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12)](https://www.python.org/)\n\nCisco Catalyst WAN SDK is a package for creating simple and parallel automatic requests via official SD-WAN Manager API. It is intended to serve as a multiple session handler (provider, provider as a tenant, tenant). The library is not dependent on environment which is being run in, you just need a connection to any SD-WAN Manager.\n\n## Important Notice: Early Beta Release\n\nWelcome to the Cisco Catalyst WAN SDK!\n\nWe are thrilled to announce that Cisco Catalyst WAN SDK is now available in early beta. This is an exciting step forward in enabling developers to harness the full potential of Cisco\'s networking solutions.  Please be aware that, as an early beta release, this version of the SDK is still undergoing development and testing. As such, it is provided "as is" and support to address any issues are limited and best effort.\n\n## Not recommend to use in production environments.\nWe encourage developers to explore and test the SDK\'s capabilities, but please exercise caution when using it in production environments.  We are dedicated to improving the Cisco Catalyst WAN SDK and we value your input. Your feedback is crucial to us-it will guide us in refining and enhancing the SDK to better meet your needs.\nTo report any issues, share your insights, or suggest improvements, please visit our Issues page on GitHub or reach out to us through the provided communication channels.\n\nThank you for being a part of our development journey!\n\n## Installation\n```console\npip install catalystwan\n```\n\n## Manager Session\nIn order to execute SDK APIs **ManagerSession** needs to be created. The fastest way to get started is to use `create_manager_session()` method which configures session, performs authentication for given credentials and returns **ManagerSession** instance in operational state. **ManagerSession** provides a collection of supported APIs in `api` instance variable.\nPlease check example below:\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    devices = session.api.devices.get()\n    print(devices)\n```\n**ManagerSession** extends [requests.Session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) so all functionality from [requests](https://requests.readthedocs.io/en/latest/) library is avaiable to user, it also implements python [contextmanager](https://docs.python.org/3.8/library/contextlib.html#contextlib.contextmanager) and automatically frees server resources on exit.\n\n<details>\n    <summary> <b>Configure Manager Session before using</b> <i>(click to expand)</i></summary>\n\nIt is possible to configure **ManagerSession** prior sending any request.\n\n```python\nfrom catalystwan.session import ManagerSession\n\nurl = "example.com"\nusername = "admin"\npassword = "password123"\n\n# configure session using constructor - nothing will be sent to target server yet\nsession = ManagerSession(url=url, username=username, password=password)\n# login and send requests\nsession.login()\nsession.get("/dataservice/device")\nsession.close()\n```\nWhen interacting with the SDWAN Manager API without using a context manager, it\'s important \nto manually execute the `close()` method to release the user session resource.\nEnsure that the `close()` method is called after you have finished using the session to maintain optimal resource management and avoid potential errors.\n\n</details>\n\n<details>\n    <summary> <b>Login as Tenant</b> <i>(click to expand)</i></summary>\n\nTenant domain needs to be provided in url together with Tenant credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "tenant.example.com"\nusername = "tenant_user"\npassword = "password123"\n\nwith create_manager_session(url=url, username=username, password=password) as session:\n    print(session.session_type)\n```\n\n</details>\n\n<details>\n    <summary> <b>Login as Provider-as-Tenant</b> <i>(click to expand)</i></summary>\n\nTenant `subdomain` needs to be provided as additional argument together with Provider credentials.\n\n```python\nfrom catalystwan.session import create_manager_session\n\nurl = "example.com"\nusername = "provider"\npassword = "password123"\nsubdomain = "tenant.example.com"\n\nwith create_manager_session(url=url, username=username, password=password, subdomain=subdomain) as session:\n    print(session.session_type)\n```\n\n</details>\n\n\n\n## API usage examples\nAll examples below assumes `session` variable contains logged-in [Manager Session](#Manager-Session) instance.\n\n<details>\n    <summary> <b>Get devices</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\n```\n\n</details>\n\n<details>\n    <summary> <b>Admin Tech</b> <i>(click to expand)</i></summary>\n\n```Python\nadmin_tech_file = session.api.admin_tech.generate("172.16.255.11")\nsession.api.admin_tech.download(admin_tech_file)\nsession.api.admin_tech.delete(admin_tech_file)\n```\n</details>\n\n<details>\n    <summary> <b>Speed test</b> <i>(click to expand)</i></summary>\n\n```python\ndevices = session.api.devices.get()\nspeedtest = session.api.speedtest.speedtest(devices[0], devices[1])\n```\n\n</details>\n\n<details>\n    <summary> <b>Upgrade device</b> <i>(click to expand)</i></summary>\n\n```python\n# Prepare devices list\ncontrollers = session.endpoints.configuration_device_inventory.get_device_details(\'controllers\')\nvsmarts = controllers.filter(personality=Personality.VSMART)\nimage = "viptela-20.7.2-x86_64.tar.gz"\n\n# Upload image\nsession.api.repository.upload_image(image)\n\n# Install software\n\ninstall_task = session.api.software.install(devices=vsmarts, image=image)\n\n# Check action status\ninstall_task.wait_for_completed()\n```\n\n</details>\n\n<details>\n    <summary> <b>Get alarms</b> <i>(click to expand)</i></summary>\nTo get all alarms:\n\n```python\nalarms = session.api.alarms.get()\n```\n\nTo get all not viewed alarms:\n\n```python\nnot_viewed_alarms = session.api.alarms.get().filter(viewed=False)\n```\n\nTo get all alarms from past `n` hours:\n\n```python\nn = 24\nalarms_from_n_hours = session.api.alarms.get(from_time=n)\n```\n\nTo get all critical alarms from past `n` hours:\n\n```python\nn = 48\ncritical_alarms = session.api.alarms.get(from_time=n).filter(severity=Severity.CRITICAL)\n```\n\n</details>\n\n<details>\n    <summary> <b>Users</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all users\nsession.api.users.get()\n\n# Create user\nnew_user = User(username="new_user", password="new_user", group=["netadmin"], description="new user")\nsession.api.users.create(new_user)\n\n# Update user data\nnew_user_update = UserUpdateRequest(username="new_user", group=["netadmin", "netops"], locale="en_US", description="updated-new_user-description")\nsession.api.users.update(new_user_update)\n\n# Update user password\nsession.api.users.update_password("new_user", "n3W-P4s$w0rd")\n\n# Reset user\nsession.api.users.reset("new_user")\n\n# Delete user\nsession.api.users.delete("new_user")\n\n# Get current user authentication type and role\nsession.api.users.get_auth_type()\nsession.api.users.get_role()\n```\n\n</details>\n\n<details>\n    <summary> <b>User Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all user groups\nsession.api.user_groups.get()\n\n# Create user group\ngroup = UserGroup("new_user_group", [])\ngroup.enable_read({"Audit Log", "Alarms"})\ngroup.enable_read_and_write({"Device Inventory"})\nsession.api.user_groups.create(group)\n\n# Update user group\ngroup.disable({"Alarms"})\nsession.api.user_groups.update(group)\n\n# Delete user group\nsession.api.user_groups.delete(group.group_name)\n```\n\n</details>\n\n</details>\n\n<details>\n    <summary> <b>Sessions</b> <i>(click to expand)</i></summary>\n\n```python\n# Get all active sessions\nactive_sessions = session.api.sessions.get()\n\n# Invalidate sessions for given user\nnew_user_sessions = active_sessions.filter(raw_username="new_user")\nsession.api.sessions.invalidate(new_user_sessions)\n```\n\n</details>\n\n<details>\n    <summary> <b>Resource Groups</b> <i>(click to expand)</i></summary>\n\n```python\n# get resource groups\nsession.api.resource_groups.get()\n\n# create resource group\nnew_resource_group = ResourceGroup(\n    name="new_resource_group",\n    desc="Custom Resource Group #1",\n    siteIds=[]\n)\nsession.api.resource_groups.create(new_resource_group)\n\n# update resource group\nresource_group = session.api.resource_groups.get().filter(name="new_resource_group").single_or_default()\nupdated_resource_group = ResourceGroupUpdateRequest(\n    id=resource_group.id,\n    name=resource_group.name,\n    desc="Custom Resource Group #1 with updated description and site ids",\n    siteIds=[200]\n)\n\n# switch to resource group view\nsession.api.resource_groups.switch("new_resource_group")\n\n# delete resource group\nsession.api.resource_groups.delete(resource_group.id)\n```\n\n</details>\n\n<details>\n    <summary> <b>Tenant management</b> <i>(click to expand)</i></summary>\n\n```python\napi = session.api.tenant_management\n# create tenants\ntenants = [\n    Tenant(\n        name="tenant1",\n        org_name="CiscoDevNet",\n        subdomain="alpha.bravo.net",\n        desc="This is tenant for unit tests",\n        edge_connector_enable=True,\n        edge_connector_system_ip="172.16.255.81",\n        edge_connector_tunnel_interface_name="GigabitEthernet1",\n        wan_edge_forecast=1,\n    )\n]\ncreate_task = api.create(tenants)\ncreate_task.wait_for_completed()\n# list all tenants\ntenants_data = api.get_all()\n# pick tenant from list by name\ntenant = tenants_data.filter(name="tenant1").single_or_default()\n# get selected tenant id\ntenant_id = tenant.tenant_id\n# get vsession id of selected tenant\nvsessionid = api.vsession_id(tenant_id)\n# delete tenant by ids\ndelete_task = api.delete([tenant_id])\ndelete_task.wait_for_completed()\n# others\napi.get_hosting_capacity_on_vsmarts()\napi.get_statuses()\napi.get_vsmart_mapping()\n```\n</details>\n\n<details>\n    <summary> <b>Tenant migration</b> <i>(click to expand)</i></summary>\n\n```python\nfrom pathlib import Path\nfrom catalystwan.session import create_manager_session\nfrom catalystwan.models.tenant import TenantExport\nfrom catalystwan.workflows.tenant_migration import migration_workflow\n\ntenant = TenantExport(\n    name="mango",\n    desc="Mango tenant description",\n    org_name="Provider Org-Mango Inc",\n    subdomain="mango.fruits.com",\n    wan_edge_forecast=100,\n    migration_key="MangoTenantMigrationKey",   # only for SDWAN Manager >= 20.13\n    is_destination_overlay_mt=True,            # only for SDWAN Manager >= 20.13\n)\n\nwith create_manager_session(url="10.0.1.15", username="st-admin", password="") as origin_session, \\\n     create_manager_session(url="10.9.0.16", username="mt-provider-admin", password="") as target_session:\n    migration_workflow(\n        origin_session=origin_session,\n        target_session=target_session,\n        workdir=Path("workdir"),\n        tenant=tenant,\n        validator="10.9.12.26"\n    )\n```\n\n`migration_workflow` performs multi-step migration procedure according to [Migrate Single-Tenant Cisco SD-WAN Overlay to Multitenant Cisco SD-WAN Deployment](https://www.cisco.com/c/en/us/td/docs/routers/sdwan/configuration/system-interface/vedge-20-x/systems-interfaces-book/sdwan-multitenancy.html#concept_sjj_jmm_z4b)\n\n\nSince 20.13 also MT to ST is supported (just provide suitable origin/target sessions, and `is_destination_overlay_mt` parameter)\n\n\nEach step of the `migration_workflow` procedure can be executed independently using api methods: `export_tenant`, `download`, `import_tenant`, `store_token`, `migrate_network`\n\n```python\norigin_api = origin_session.api.tenant_migration_api\ntarget_api = target_session.api.tenant_migration_api\ntenant_file = Path("~/tenant.tar.gz")\ntoken_file = Path("~/tenant-token.txt")\n# export\nexport_task = origin_api.export_tenant(tenant=tenant)\nremote_filename = export_task.wait_for_file()\n# download\norigin_api.download(export_path, remote_filename)\n# import\nimport_task = target_api.import_tenant(export_path, tenant.migration_key)\nimport_task.wait_for_completed()\n# get token\nmigration_id = import_task.import_info.migration_token_query_params.migration_id\ntarget_api.store_token(migration_id, token_path)\n# migrate network\nmigrate_task = origin_api.migrate_network(token_path)\nmigrate_task.wait_for_completed()\n```\n</details>\n\n### Note:\nTo remove `InsecureRequestWarning`, you can include in your scripts (warning is suppressed when `catalystwan_devel` environment variable is set):\n```Python\nimport urllib3\nurllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)\n```\n\n## Catching Exceptions\n```python\ntry:\n    session.api.users.delete("bogus-user-name")\nexcept ManagerHTTPError as error:\n    # Process an error.\n    print(error.response.status_code)\n    print(error.info.code)\n    print(error.info.message)\n    print(error.info.details)\n\n```\n\n## [Supported API endpoints](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/ENDPOINTS.md)\n\n\n## [Contributing, bug reporting and feature requests](https://github.com/cisco-open/cisco-catalyst-wan-sdk/blob/main/CONTRIBUTING.md)\n\n## Seeking support\n\nYou can contact us by submitting [issues](https://github.com/cisco-open/cisco-catalyst-wan-sdk/issues), or directly via mail on catalystwan@cisco.com.\n',
     'author': 'kagorski',
     'author_email': 'kagorski@cisco.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cisco-open/cisco-catalyst-wan-sdk',
```

### Comparing `catalystwan-0.33.7.dev1/PKG-INFO` & `catalystwan-0.33.7.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalystwan
-Version: 0.33.7.dev1
+Version: 0.33.7.dev2
 Summary: Cisco Catalyst WAN SDK for Python
 Home-page: https://github.com/cisco-open/cisco-catalyst-wan-sdk
 Author: kagorski
 Author-email: kagorski@cisco.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7.dev1 Summary: Cisco
+Metadata-Version: 2.1 Name: catalystwan Version: 0.33.7.dev2 Summary: Cisco
 Catalyst WAN SDK for Python Home-page: https://github.com/cisco-open/cisco-
 catalyst-wan-sdk Author: kagorski Author-email: kagorski@cisco.com Requires-
 Python: >=3.8.0,<4.0.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: Jinja2
 (>=3.1.2,<4.0.0) Requires-Dist: attrs (>=21.4.0,<22.0.0) Requires-Dist:
```

