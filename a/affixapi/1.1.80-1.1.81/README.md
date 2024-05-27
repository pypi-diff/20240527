# Comparing `tmp/affixapi-1.1.80.tar.gz` & `tmp/affixapi-1.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.80.tar", last modified: Sun May 26 17:51:39 2024, max compression
+gzip compressed data, was "affixapi-1.1.81.tar", last modified: Mon May 27 00:02:16 2024, max compression
```

## Comparing `affixapi-1.1.80.tar` & `affixapi-1.1.81.tar`

### file list

```diff
@@ -1,162 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.719888 affixapi-1.1.80/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-26 17:51:36.000000 affixapi-1.1.80/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-26 17:51:39.719888 affixapi-1.1.80/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21809 2024-05-26 17:51:36.000000 affixapi-1.1.80/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.719888 affixapi-1.1.80/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-26 17:51:39.000000 affixapi-1.1.80/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-26 17:51:39.000000 affixapi-1.1.80/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 17:51:39.000000 affixapi-1.1.80/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-26 17:51:39.000000 affixapi-1.1.80/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-26 17:51:39.000000 affixapi-1.1.80/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.695888 affixapi-1.1.80/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.695888 affixapi-1.1.80/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    55260 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55275 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.695888 affixapi-1.1.80/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.707888 affixapi-1.1.80/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17375 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17403 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17751 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.707888 affixapi-1.1.80/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-26 17:51:36.000000 affixapi-1.1.80/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-26 17:51:39.719888 affixapi-1.1.80/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-26 17:51:36.000000 affixapi-1.1.80/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 17:51:39.719888 affixapi-1.1.80/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_compensation_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_compensation_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employment_history_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employment_history_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employment_status_not_null_not_nullable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_policy_type_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-26 17:51:36.000000 affixapi-1.1.80/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.112760 affixapi-1.1.81/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-27 00:02:12.000000 affixapi-1.1.81/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-05-27 00:02:16.112760 affixapi-1.1.81/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21923 2024-05-27 00:02:12.000000 affixapi-1.1.81/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.112760 affixapi-1.1.81/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 2024-05-27 00:02:16.000000 affixapi-1.1.81/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6298 2024-05-27 00:02:16.000000 affixapi-1.1.81/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 00:02:16.000000 affixapi-1.1.81/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-27 00:02:16.000000 affixapi-1.1.81/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-27 00:02:16.000000 affixapi-1.1.81/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.088760 affixapi-1.1.81/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.088760 affixapi-1.1.81/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    55260 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55275 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.088760 affixapi-1.1.81/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.100760 affixapi-1.1.81/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18749 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17866 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24834 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/currency_not_null_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26128 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17375 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17403 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16709 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payrun_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16821 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.100760 affixapi-1.1.81/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-05-27 00:02:12.000000 affixapi-1.1.81/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-27 00:02:16.112760 affixapi-1.1.81/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-27 00:02:12.000000 affixapi-1.1.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 00:02:16.112760 affixapi-1.1.81/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10595 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_compensation_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_compensation_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12099 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_currency_not_null_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employment_history_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employment_history_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payrun_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10330 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_policy_type_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10485 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10471 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-05-27 00:02:12.000000 affixapi-1.1.81/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.80/LICENSE` & `affixapi-1.1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/PKG-INFO` & `affixapi-1.1.81/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.80
+Version: 1.1.81
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -361,14 +361,15 @@
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyNotNullResponse](docs/CurrencyNotNullResponse.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
@@ -387,14 +388,15 @@
  - [IntrospectResponse](docs/IntrospectResponse.md)
  - [LocationNoNonNullRequest](docs/LocationNoNonNullRequest.md)
  - [LocationResponse](docs/LocationResponse.md)
  - [MessageResponse](docs/MessageResponse.md)
  - [ModeRequest](docs/ModeRequest.md)
  - [ModeResponse](docs/ModeResponse.md)
  - [PayrunResponse](docs/PayrunResponse.md)
+ - [PayrunTypeResponse](docs/PayrunTypeResponse.md)
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
```

### Comparing `affixapi-1.1.80/README.md` & `affixapi-1.1.81/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -347,14 +347,15 @@
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyNotNullResponse](docs/CurrencyNotNullResponse.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
@@ -373,14 +374,15 @@
  - [IntrospectResponse](docs/IntrospectResponse.md)
  - [LocationNoNonNullRequest](docs/LocationNoNonNullRequest.md)
  - [LocationResponse](docs/LocationResponse.md)
  - [MessageResponse](docs/MessageResponse.md)
  - [ModeRequest](docs/ModeRequest.md)
  - [ModeResponse](docs/ModeResponse.md)
  - [PayrunResponse](docs/PayrunResponse.md)
+ - [PayrunTypeResponse](docs/PayrunTypeResponse.md)
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
```

### Comparing `affixapi-1.1.80/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.81/affixapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.80
+Version: 1.1.81
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -361,14 +361,15 @@
  - [CompensationHistoryResponse](docs/CompensationHistoryResponse.md)
  - [CreateEmployeeRequest](docs/CreateEmployeeRequest.md)
  - [CreateEmployeeRequestBankAccount](docs/CreateEmployeeRequestBankAccount.md)
  - [CreateEmployeeRequestDependents](docs/CreateEmployeeRequestDependents.md)
  - [CreateEmployeeRequestEmergencyContacts](docs/CreateEmployeeRequestEmergencyContacts.md)
  - [CreateEmployeeRequestManager](docs/CreateEmployeeRequestManager.md)
  - [CurrencyNotNullRequest](docs/CurrencyNotNullRequest.md)
+ - [CurrencyNotNullResponse](docs/CurrencyNotNullResponse.md)
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentHistoryNoNonNullRequest](docs/EmploymentHistoryNoNonNullRequest.md)
  - [EmploymentHistoryResponse](docs/EmploymentHistoryResponse.md)
@@ -387,14 +388,15 @@
  - [IntrospectResponse](docs/IntrospectResponse.md)
  - [LocationNoNonNullRequest](docs/LocationNoNonNullRequest.md)
  - [LocationResponse](docs/LocationResponse.md)
  - [MessageResponse](docs/MessageResponse.md)
  - [ModeRequest](docs/ModeRequest.md)
  - [ModeResponse](docs/ModeResponse.md)
  - [PayrunResponse](docs/PayrunResponse.md)
+ - [PayrunTypeResponse](docs/PayrunTypeResponse.md)
  - [Payruns20230301Response](docs/Payruns20230301Response.md)
  - [PayslipResponse](docs/PayslipResponse.md)
  - [PayslipResponseContributions](docs/PayslipResponseContributions.md)
  - [PayslipResponseDeductions](docs/PayslipResponseDeductions.md)
  - [PayslipResponseEarnings](docs/PayslipResponseEarnings.md)
  - [PayslipResponseTaxes](docs/PayslipResponseTaxes.md)
  - [Payslips20230301Response](docs/Payslips20230301Response.md)
```

### Comparing `affixapi-1.1.80/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.81/affixapi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 openapi_client/model/compensation_history_response.py
 openapi_client/model/create_employee_request.py
 openapi_client/model/create_employee_request_bank_account.py
 openapi_client/model/create_employee_request_dependents.py
 openapi_client/model/create_employee_request_emergency_contacts.py
 openapi_client/model/create_employee_request_manager.py
 openapi_client/model/currency_not_null_request.py
+openapi_client/model/currency_not_null_response.py
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
 openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
 openapi_client/model/employment_history_no_non_null_request.py
 openapi_client/model/employment_history_response.py
@@ -56,14 +57,15 @@
 openapi_client/model/introspect_response.py
 openapi_client/model/location_no_non_null_request.py
 openapi_client/model/location_response.py
 openapi_client/model/message_response.py
 openapi_client/model/mode_request.py
 openapi_client/model/mode_response.py
 openapi_client/model/payrun_response.py
+openapi_client/model/payrun_type_response.py
 openapi_client/model/payruns20230301_response.py
 openapi_client/model/payslip_response.py
 openapi_client/model/payslip_response_contributions.py
 openapi_client/model/payslip_response_deductions.py
 openapi_client/model/payslip_response_earnings.py
 openapi_client/model/payslip_response_taxes.py
 openapi_client/model/payslips20230301_response.py
@@ -96,14 +98,15 @@
 test/test_core_api.py
 test/test_create_employee_request.py
 test/test_create_employee_request_bank_account.py
 test/test_create_employee_request_dependents.py
 test/test_create_employee_request_emergency_contacts.py
 test/test_create_employee_request_manager.py
 test/test_currency_not_null_request.py
+test/test_currency_not_null_response.py
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
 test/test_employee_response_manager.py
 test/test_employees20230301_response.py
 test/test_employment_history_no_non_null_request.py
 test/test_employment_history_response.py
@@ -123,14 +126,15 @@
 test/test_location_no_non_null_request.py
 test/test_location_response.py
 test/test_management_api.py
 test/test_message_response.py
 test/test_mode_request.py
 test/test_mode_response.py
 test/test_payrun_response.py
+test/test_payrun_type_response.py
 test/test_payruns20230301_response.py
 test/test_payslip_response.py
 test/test_payslip_response_contributions.py
 test/test_payslip_response_deductions.py
 test/test_payslip_response_earnings.py
 test/test_payslip_response_taxes.py
 test/test_payslips20230301_response.py
```

### Comparing `affixapi-1.1.80/openapi_client/__init__.py` & `affixapi-1.1.81/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.81/openapi_client/api/2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/api/core_api.py` & `affixapi-1.1.81/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/api/management_api.py` & `affixapi-1.1.81/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.81/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/api_client.py` & `affixapi-1.1.81/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/apis/__init__.py` & `affixapi-1.1.81/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/configuration.py` & `affixapi-1.1.81/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/exceptions.py` & `affixapi-1.1.81/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.81/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/address_response.py` & `affixapi-1.1.81/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/client_request.py` & `affixapi-1.1.81/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/client_response.py` & `affixapi-1.1.81/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.81/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/company_response.py` & `affixapi-1.1.81/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/compensation_history_no_non_null_request.py` & `affixapi-1.1.81/openapi_client/model/compensation_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/compensation_history_response.py` & `affixapi-1.1.81/openapi_client/model/compensation_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/create_employee_request.py` & `affixapi-1.1.81/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.81/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.81/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.81/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.81/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.81/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/currency_response.py` & `affixapi-1.1.81/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/disconnect_response.py` & `affixapi-1.1.81/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employee_response.py` & `affixapi-1.1.81/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.81/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.81/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employment_history_no_non_null_request.py` & `affixapi-1.1.81/openapi_client/model/employment_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employment_history_response.py` & `affixapi-1.1.81/openapi_client/model/employment_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employment_status_not_null_not_nullable.py` & `affixapi-1.1.81/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.81/openapi_client/model/employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/employment_status_response.py` & `affixapi-1.1.81/openapi_client/model/employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.81/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/group_response.py` & `affixapi-1.1.81/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.81/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.81/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.81/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/identity_response.py` & `affixapi-1.1.81/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/inline_response400.py` & `affixapi-1.1.81/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/inline_response401.py` & `affixapi-1.1.81/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/inline_response409.py` & `affixapi-1.1.81/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/introspect_response.py` & `affixapi-1.1.81/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.81/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/location_response.py` & `affixapi-1.1.81/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/message_response.py` & `affixapi-1.1.81/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/mode_request.py` & `affixapi-1.1.81/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/mode_response.py` & `affixapi-1.1.81/openapi_client/model/mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payrun_response.py` & `affixapi-1.1.81/openapi_client/model/payrun_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.payrun_type_response import PayrunTypeResponse
+    globals()['PayrunTypeResponse'] = PayrunTypeResponse
+
 
 class PayrunResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
@@ -49,29 +53,20 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('run_state',): {
+        ('state',): {
             'None': None,
             'PAID': "paid",
             'PENDING': "pending",
             'NULL': "null",
         },
-        ('run_type',): {
-            'None': None,
-            'REGULAR': "regular",
-            'ONE-TIME': "one-time",
-            'OFF-CYCLE': "off-cycle",
-            'CORRECTION': "correction",
-            'REVERSAL': "reversal",
-            'NULL': "null",
-        },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
@@ -83,34 +78,35 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'remote_id': (str,),  # noqa: E501
-            'run_state': (str, none_type,),  # noqa: E501
-            'run_type': (str, none_type,),  # noqa: E501
+            'state': (str, none_type,),  # noqa: E501
+            'type': (PayrunTypeResponse,),  # noqa: E501
             'start_date': (date, none_type,),  # noqa: E501
             'end_date': (date, none_type,),  # noqa: E501
             'payment_date': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'remote_id': 'remote_id',  # noqa: E501
-        'run_state': 'run_state',  # noqa: E501
-        'run_type': 'run_type',  # noqa: E501
+        'state': 'state',  # noqa: E501
+        'type': 'type',  # noqa: E501
         'start_date': 'start_date',  # noqa: E501
         'end_date': 'end_date',  # noqa: E501
         'payment_date': 'payment_date',  # noqa: E501
     }
 
     _composed_schemas = {}
 
@@ -120,22 +116,22 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, run_state, run_type, start_date, end_date, payment_date, *args, **kwargs):  # noqa: E501
+    def __init__(self, id, remote_id, state, type, start_date, end_date, payment_date, *args, **kwargs):  # noqa: E501
         """PayrunResponse - a model defined in OpenAPI
 
         Args:
             id (str): The Affix-assigned id of the individual
             remote_id (str): the remote system-assigned id of the payrun
-            run_state (str, none_type):
-            run_type (str, none_type):
+            state (str, none_type):
+            type (PayrunTypeResponse):
             start_date (date, none_type): Payrun period start date
             end_date (date, none_type): Payrun period end date
             payment_date (date, none_type): Payment date / check date
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
@@ -190,16 +186,16 @@
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.remote_id = remote_id
-        self.run_state = run_state
-        self.run_type = run_type
+        self.state = state
+        self.type = type
         self.start_date = start_date
         self.end_date = end_date
         self.payment_date = payment_date
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
```

### Comparing `affixapi-1.1.80/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.81/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payslip_response.py` & `affixapi-1.1.81/openapi_client/model/timesheet_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,26 +23,16 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
-def lazy_import():
-    from openapi_client.model.payslip_response_contributions import PayslipResponseContributions
-    from openapi_client.model.payslip_response_deductions import PayslipResponseDeductions
-    from openapi_client.model.payslip_response_earnings import PayslipResponseEarnings
-    from openapi_client.model.payslip_response_taxes import PayslipResponseTaxes
-    globals()['PayslipResponseContributions'] = PayslipResponseContributions
-    globals()['PayslipResponseDeductions'] = PayslipResponseDeductions
-    globals()['PayslipResponseEarnings'] = PayslipResponseEarnings
-    globals()['PayslipResponseTaxes'] = PayslipResponseTaxes
 
-
-class PayslipResponse(ModelNormal):
+class TimesheetResponse(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -59,22 +49,20 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('currency',): {
-            'USD': "usd",
-            'EUR': "eur",
-            'GBP': "gbp",
-        },
     }
 
     validations = {
+        ('hours_worked',): {
+            'multiple_of': 0.1,
+        },
     }
 
     additional_properties_type = None
 
     _nullable = False
 
     @cached_property
@@ -83,84 +71,68 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'id': (str,),  # noqa: E501
             'remote_id': (str,),  # noqa: E501
             'employee_id': (str,),  # noqa: E501
-            'payrun_id': (str,),  # noqa: E501
-            'currency': (str,),  # noqa: E501
-            'gross_pay': (float, none_type,),  # noqa: E501
-            'net_pay': (float, none_type,),  # noqa: E501
-            'start_date': (date,),  # noqa: E501
-            'end_date': (date,),  # noqa: E501
-            'payment_date': (date,),  # noqa: E501
-            'earnings': ([PayslipResponseEarnings], none_type,),  # noqa: E501
-            'contributions': ([PayslipResponseContributions], none_type,),  # noqa: E501
-            'deductions': ([PayslipResponseDeductions], none_type,),  # noqa: E501
-            'taxes': ([PayslipResponseTaxes], none_type,),  # noqa: E501
+            'employee_remote_id': (str,),  # noqa: E501
+            'start_time': (datetime, none_type,),  # noqa: E501
+            'end_time': (datetime, none_type,),  # noqa: E501
+            'hours_worked': (float,),  # noqa: E501
+            'remote_created_at': (date, none_type,),  # noqa: E501
+            'remote_modified_at': (date, none_type,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'id': 'id',  # noqa: E501
         'remote_id': 'remote_id',  # noqa: E501
         'employee_id': 'employee_id',  # noqa: E501
-        'payrun_id': 'payrun_id',  # noqa: E501
-        'currency': 'currency',  # noqa: E501
-        'gross_pay': 'gross_pay',  # noqa: E501
-        'net_pay': 'net_pay',  # noqa: E501
-        'start_date': 'start_date',  # noqa: E501
-        'end_date': 'end_date',  # noqa: E501
-        'payment_date': 'payment_date',  # noqa: E501
-        'earnings': 'earnings',  # noqa: E501
-        'contributions': 'contributions',  # noqa: E501
-        'deductions': 'deductions',  # noqa: E501
-        'taxes': 'taxes',  # noqa: E501
+        'employee_remote_id': 'employee_remote_id',  # noqa: E501
+        'start_time': 'start_time',  # noqa: E501
+        'end_time': 'end_time',  # noqa: E501
+        'hours_worked': 'hours_worked',  # noqa: E501
+        'remote_created_at': 'remote_created_at',  # noqa: E501
+        'remote_modified_at': 'remote_modified_at',  # noqa: E501
     }
 
     _composed_schemas = {}
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_id, payrun_id, currency, gross_pay, net_pay, start_date, end_date, payment_date, earnings, contributions, deductions, taxes, *args, **kwargs):  # noqa: E501
-        """PayslipResponse - a model defined in OpenAPI
+    def __init__(self, id, remote_id, employee_id, employee_remote_id, start_time, end_time, hours_worked, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
+        """TimesheetResponse - a model defined in OpenAPI
 
         Args:
-            id (str): The Affix-assigned id of the payslip
-            remote_id (str): the remote system-assigned id of the payrun
-            employee_id (str):
-            payrun_id (str):
-            currency (str):
-            gross_pay (float, none_type): if USD/EUR/GBP, in cent
-            net_pay (float, none_type): if USD/EUR/GBP, in cent
-            start_date (date):
-            end_date (date):
-            payment_date (date):
-            earnings ([PayslipResponseEarnings], none_type):
-            contributions ([PayslipResponseContributions], none_type): Items paid by the employer that are not included in gross pay, such as employer-paid portion of private health insurance 
-            deductions ([PayslipResponseDeductions], none_type):
-            taxes ([PayslipResponseTaxes], none_type):
+            id (str): The Affix-assigned id of the time off entry
+            remote_id (str): the remote system-assigned id of the time off entry
+            employee_id (str): the Affix-assigned id of the individual
+            employee_remote_id (str): the remote system-assigned id of the individual
+            start_time (datetime, none_type):
+            end_time (datetime, none_type):
+            hours_worked (float):
+            remote_created_at (date, none_type):
+            remote_modified_at (date, none_type):
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -213,25 +185,20 @@
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
         self.id = id
         self.remote_id = remote_id
         self.employee_id = employee_id
-        self.payrun_id = payrun_id
-        self.currency = currency
-        self.gross_pay = gross_pay
-        self.net_pay = net_pay
-        self.start_date = start_date
-        self.end_date = end_date
-        self.payment_date = payment_date
-        self.earnings = earnings
-        self.contributions = contributions
-        self.deductions = deductions
-        self.taxes = taxes
+        self.employee_remote_id = employee_remote_id
+        self.start_time = start_time
+        self.end_time = end_time
+        self.hours_worked = hours_worked
+        self.remote_created_at = remote_created_at
+        self.remote_modified_at = remote_modified_at
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `affixapi-1.1.80/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.81/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.81/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.81/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.81/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.81/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/policy_type_response.py` & `affixapi-1.1.81/openapi_client/model/policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/provider_request.py` & `affixapi-1.1.81/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/provider_response.py` & `affixapi-1.1.81/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/providers_response.py` & `affixapi-1.1.81/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/scopes_request.py` & `affixapi-1.1.81/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/scopes_response.py` & `affixapi-1.1.81/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.81/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.81/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.81/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.81/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/timesheet_response.py` & `affixapi-1.1.81/openapi_client/model/currency_not_null_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,117 +24,93 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class TimesheetResponse(ModelNormal):
+class CurrencyNotNullResponse(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           with a capitalized key describing the allowed value and an allowed
           value. These dicts store the allowed enum values.
-      attribute_map (dict): The key is attribute name
-          and the value is json key in definition.
-      discriminator_value_class_map (dict): A dict to go from the discriminator
-          variable value to the discriminator class name.
       validations (dict): The key is the tuple path to the attribute
           and the for var_name this is (var_name,). The value is a dict
           that stores validations for max_length, min_length, max_items,
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
+        ('value',): {
+            'None': None,
+            'USD': "usd",
+            'GBP': "gbp",
+            'EUR': "eur",
+        },
     }
 
     validations = {
-        ('hours_worked',): {
-            'multiple_of': 0.1,
-        },
     }
 
     additional_properties_type = None
 
-    _nullable = False
+    _nullable = True
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'id': (str,),  # noqa: E501
-            'remote_id': (str,),  # noqa: E501
-            'employee_id': (str,),  # noqa: E501
-            'employee_remote_id': (str,),  # noqa: E501
-            'start_time': (datetime, none_type,),  # noqa: E501
-            'end_time': (datetime, none_type,),  # noqa: E501
-            'hours_worked': (float,),  # noqa: E501
-            'remote_created_at': (date, none_type,),  # noqa: E501
-            'remote_modified_at': (date, none_type,),  # noqa: E501
+            'value': (str,),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
-    attribute_map = {
-        'id': 'id',  # noqa: E501
-        'remote_id': 'remote_id',  # noqa: E501
-        'employee_id': 'employee_id',  # noqa: E501
-        'employee_remote_id': 'employee_remote_id',  # noqa: E501
-        'start_time': 'start_time',  # noqa: E501
-        'end_time': 'end_time',  # noqa: E501
-        'hours_worked': 'hours_worked',  # noqa: E501
-        'remote_created_at': 'remote_created_at',  # noqa: E501
-        'remote_modified_at': 'remote_modified_at',  # noqa: E501
-    }
+    attribute_map = {}
 
-    _composed_schemas = {}
+    _composed_schemas = None
 
     required_properties = set([
         '_data_store',
         '_check_type',
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, id, remote_id, employee_id, employee_remote_id, start_time, end_time, hours_worked, remote_created_at, remote_modified_at, *args, **kwargs):  # noqa: E501
-        """TimesheetResponse - a model defined in OpenAPI
+    def __init__(self, *args, **kwargs):
+        """CurrencyNotNullResponse - a model defined in OpenAPI
+
+        Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            id (str): The Affix-assigned id of the time off entry
-            remote_id (str): the remote system-assigned id of the time off entry
-            employee_id (str): the Affix-assigned id of the individual
-            employee_remote_id (str): the remote system-assigned id of the individual
-            start_time (datetime, none_type):
-            end_time (datetime, none_type):
-            hours_worked (float):
-            remote_created_at (date, none_type):
-            remote_modified_at (date, none_type):
+            args[0] (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
 
         Keyword Args:
+            value (str):, must be one of ["usd", "gbp", "eur", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -158,18 +134,31 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
         """
+        # required up here when default value is not given
+        _path_to_item = kwargs.pop('_path_to_item', ())
+
+        if 'value' in kwargs:
+            value = kwargs.pop('value')
+        elif args:
+            args = list(args)
+            value = args.pop(0)
+        else:
+            raise ApiTypeError(
+                "value is required, but not passed in args or kwargs and doesn't have default",
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
-        _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
 
         if args:
             raise ApiTypeError(
                 "Invalid positional arguments=%s passed to %s. Remove those invalid positional arguments." % (
                     args,
@@ -181,25 +170,17 @@
 
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
-
-        self.id = id
-        self.remote_id = remote_id
-        self.employee_id = employee_id
-        self.employee_remote_id = employee_remote_id
-        self.start_time = start_time
-        self.end_time = end_time
-        self.hours_worked = hours_worked
-        self.remote_created_at = remote_created_at
-        self.remote_modified_at = remote_modified_at
-        for var_name, var_value in kwargs.items():
-            if var_name not in self.attribute_map and \
-                        self._configuration is not None and \
-                        self._configuration.discard_unknown_keys and \
-                        self.additional_properties_type is None:
-                # discard variable.
-                continue
-            setattr(self, var_name, var_value)
+        self.value = value
+        if kwargs:
+            raise ApiTypeError(
+                "Invalid named arguments=%s passed to %s. Remove those invalid named arguments." % (
+                    kwargs,
+                    self.__class__.__name__,
+                ),
+                path_to_item=_path_to_item,
+                valid_classes=(self.__class__,),
+            )
```

### Comparing `affixapi-1.1.80/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.81/openapi_client/model/timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/token_request.py` & `affixapi-1.1.81/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/token_response.py` & `affixapi-1.1.81/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/tokens_response.py` & `affixapi-1.1.81/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model/work_locations20230301_response.py` & `affixapi-1.1.81/openapi_client/model/work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/model_utils.py` & `affixapi-1.1.81/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/openapi_client/models/__init__.py` & `affixapi-1.1.81/openapi_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from openapi_client.model.compensation_history_response import CompensationHistoryResponse
 from openapi_client.model.create_employee_request import CreateEmployeeRequest
 from openapi_client.model.create_employee_request_bank_account import CreateEmployeeRequestBankAccount
 from openapi_client.model.create_employee_request_dependents import CreateEmployeeRequestDependents
 from openapi_client.model.create_employee_request_emergency_contacts import CreateEmployeeRequestEmergencyContacts
 from openapi_client.model.create_employee_request_manager import CreateEmployeeRequestManager
 from openapi_client.model.currency_not_null_request import CurrencyNotNullRequest
+from openapi_client.model.currency_not_null_response import CurrencyNotNullResponse
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.employment_history_no_non_null_request import EmploymentHistoryNoNonNullRequest
 from openapi_client.model.employment_history_response import EmploymentHistoryResponse
@@ -45,14 +46,15 @@
 from openapi_client.model.introspect_response import IntrospectResponse
 from openapi_client.model.location_no_non_null_request import LocationNoNonNullRequest
 from openapi_client.model.location_response import LocationResponse
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.mode_request import ModeRequest
 from openapi_client.model.mode_response import ModeResponse
 from openapi_client.model.payrun_response import PayrunResponse
+from openapi_client.model.payrun_type_response import PayrunTypeResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslip_response import PayslipResponse
 from openapi_client.model.payslip_response_contributions import PayslipResponseContributions
 from openapi_client.model.payslip_response_deductions import PayslipResponseDeductions
 from openapi_client.model.payslip_response_earnings import PayslipResponseEarnings
 from openapi_client.model.payslip_response_taxes import PayslipResponseTaxes
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
```

### Comparing `affixapi-1.1.80/openapi_client/rest.py` & `affixapi-1.1.81/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/setup.py` & `affixapi-1.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.80"
+VERSION = "1.1.81"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.80/test/test_2023_03_01_api.py` & `affixapi-1.1.81/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_address_no_non_null_request.py` & `affixapi-1.1.81/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_address_response.py` & `affixapi-1.1.81/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_client_request.py` & `affixapi-1.1.81/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_client_response.py` & `affixapi-1.1.81/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_companies20230301_response.py` & `affixapi-1.1.81/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_company_response.py` & `affixapi-1.1.81/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_compensation_history_no_non_null_request.py` & `affixapi-1.1.81/test/test_compensation_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_compensation_history_response.py` & `affixapi-1.1.81/test/test_compensation_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_core_api.py` & `affixapi-1.1.81/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_create_employee_request.py` & `affixapi-1.1.81/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.81/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_create_employee_request_dependents.py` & `affixapi-1.1.81/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.81/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_create_employee_request_manager.py` & `affixapi-1.1.81/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_currency_not_null_request.py` & `affixapi-1.1.81/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_currency_response.py` & `affixapi-1.1.81/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_disconnect_response.py` & `affixapi-1.1.81/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employee_response.py` & `affixapi-1.1.81/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employee_response_manager.py` & `affixapi-1.1.81/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employees20230301_response.py` & `affixapi-1.1.81/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employment_history_no_non_null_request.py` & `affixapi-1.1.81/test/test_employment_history_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employment_history_response.py` & `affixapi-1.1.81/test/test_employment_history_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employment_status_not_null_not_nullable.py` & `affixapi-1.1.81/test/test_employment_status_not_null_not_nullable.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employment_status_not_null_request.py` & `affixapi-1.1.81/test/test_employment_status_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_employment_status_response.py` & `affixapi-1.1.81/test/test_employment_status_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_group_no_null_enum_request.py` & `affixapi-1.1.81/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_group_response.py` & `affixapi-1.1.81/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_groups20230301_response.py` & `affixapi-1.1.81/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.81/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_id_and_message_response.py` & `affixapi-1.1.81/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_identity_response.py` & `affixapi-1.1.81/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_inline_response400.py` & `affixapi-1.1.81/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_inline_response401.py` & `affixapi-1.1.81/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_inline_response409.py` & `affixapi-1.1.81/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_introspect_response.py` & `affixapi-1.1.81/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_location_no_non_null_request.py` & `affixapi-1.1.81/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_location_response.py` & `affixapi-1.1.81/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_management_api.py` & `affixapi-1.1.81/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_message_response.py` & `affixapi-1.1.81/test/test_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_mode_request.py` & `affixapi-1.1.81/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_mode_response.py` & `affixapi-1.1.81/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payrun_response.py` & `affixapi-1.1.81/test/test_payrun_type_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.payrun_response import PayrunResponse
+from openapi_client.model.payrun_type_response import PayrunTypeResponse
 
 
-class TestPayrunResponse(unittest.TestCase):
-    """PayrunResponse unit test stubs"""
+class TestPayrunTypeResponse(unittest.TestCase):
+    """PayrunTypeResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPayrunResponse(self):
-        """Test PayrunResponse"""
+    def testPayrunTypeResponse(self):
+        """Test PayrunTypeResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = PayrunResponse()  # noqa: E501
+        # model = PayrunTypeResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.80/test/test_payruns20230301_response.py` & `affixapi-1.1.81/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payslip_response.py` & `affixapi-1.1.81/test/test_payslip_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
+from openapi_client.model.currency_not_null_response import CurrencyNotNullResponse
+from openapi_client.model.payrun_type_response import PayrunTypeResponse
 from openapi_client.model.payslip_response_contributions import PayslipResponseContributions
 from openapi_client.model.payslip_response_deductions import PayslipResponseDeductions
 from openapi_client.model.payslip_response_earnings import PayslipResponseEarnings
 from openapi_client.model.payslip_response_taxes import PayslipResponseTaxes
+globals()['CurrencyNotNullResponse'] = CurrencyNotNullResponse
+globals()['PayrunTypeResponse'] = PayrunTypeResponse
 globals()['PayslipResponseContributions'] = PayslipResponseContributions
 globals()['PayslipResponseDeductions'] = PayslipResponseDeductions
 globals()['PayslipResponseEarnings'] = PayslipResponseEarnings
 globals()['PayslipResponseTaxes'] = PayslipResponseTaxes
 from openapi_client.model.payslip_response import PayslipResponse
```

### Comparing `affixapi-1.1.80/test/test_payslip_response_contributions.py` & `affixapi-1.1.81/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payslip_response_deductions.py` & `affixapi-1.1.81/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payslip_response_earnings.py` & `affixapi-1.1.81/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payslip_response_taxes.py` & `affixapi-1.1.81/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_payslips20230301_response.py` & `affixapi-1.1.81/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_policy_type_response.py` & `affixapi-1.1.81/test/test_policy_type_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_provider_request.py` & `affixapi-1.1.81/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_provider_response.py` & `affixapi-1.1.81/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_providers_response.py` & `affixapi-1.1.81/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_scopes_request.py` & `affixapi-1.1.81/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_scopes_response.py` & `affixapi-1.1.81/test/test_scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_time_off_balance_response.py` & `affixapi-1.1.81/test/test_time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.81/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.81/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_time_off_entry_response.py` & `affixapi-1.1.81/test/test_time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_timesheet_response.py` & `affixapi-1.1.81/test/test_timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_timesheets20230301_response.py` & `affixapi-1.1.81/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_token_request.py` & `affixapi-1.1.81/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_token_response.py` & `affixapi-1.1.81/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_tokens_response.py` & `affixapi-1.1.81/test/test_tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_work_locations20230301_response.py` & `affixapi-1.1.81/test/test_work_locations20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.80/test/test_xhr__vertically_integrated_api.py` & `affixapi-1.1.81/test/test_xhr__vertically_integrated_api.py`

 * *Files identical despite different names*

