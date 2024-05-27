# Comparing `tmp/accounting_sh-0.0.4.tar.gz` & `tmp/accounting_sh-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accounting_sh-0.0.4.tar", last modified: Mon May 27 20:31:54 2024, max compression
+gzip compressed data, was "accounting_sh-0.0.5.tar", last modified: Mon May 27 20:33:13 2024, max compression
```

## Comparing `accounting_sh-0.0.4.tar` & `accounting_sh-0.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:54.892490 accounting_sh-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    39209 2024-05-27 20:31:54.892490 accounting_sh-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:54.880491 accounting_sh-0.0.4/accounting_sh/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/accounting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:54.884491 accounting_sh-0.0.4/accounting_sh/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/account_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/accounting_codes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/bills_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/categories_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/companies_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/company_statistics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/contacts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/countries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/credentials_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/currency_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/documents_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/expense_reports_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/invoices_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/logs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/notification_types_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/o_auth_config_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/payments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/quotes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/receipts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/revenues_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/rossum_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/tax_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/vatid_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/api/webhooks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/accounting_sh/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:54.892490 accounting_sh-0.0.4/accounting_sh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    39209 2024-05-27 20:31:54.000000 accounting_sh-0.0.4/accounting_sh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-27 20:31:54.000000 accounting_sh-0.0.4/accounting_sh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:31:54.000000 accounting_sh-0.0.4/accounting_sh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 20:31:54.000000 accounting_sh-0.0.4/accounting_sh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 20:31:54.000000 accounting_sh-0.0.4/accounting_sh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:31:54.892490 accounting_sh-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:31:54.892490 accounting_sh-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_account_connections_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_accounting_codes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_accounts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_attachments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_bills_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_categories_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_companies_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_company_statistics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_contacts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_countries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_credentials_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_currency_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_documents_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_expense_reports_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_export_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_invoices_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_logs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_notification_types_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_o_auth_config_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_payments_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_quotes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_receipts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_revenues_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_rossum_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_search_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_tax_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_transactions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_transfers_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_vatid_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-27 20:31:49.000000 accounting_sh-0.0.4/test/test_webhooks_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:33:13.086457 accounting_sh-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    39209 2024-05-27 20:33:13.086457 accounting_sh-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25003 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:33:13.074457 accounting_sh-0.0.5/accounting_sh/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/accounting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:33:13.082457 accounting_sh-0.0.5/accounting_sh/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/account_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/accounting_codes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/bills_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6713 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/company_statistics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10008 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/countries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9510 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/credentials_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/currency_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15516 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/expense_reports_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11690 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/notification_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/o_auth_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/payments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7699 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/quotes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/receipts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/revenues_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/rossum_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/tax_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6705 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/vatid_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/api/webhooks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/accounting_sh/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:33:13.086457 accounting_sh-0.0.5/accounting_sh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    39209 2024-05-27 20:33:13.000000 accounting_sh-0.0.5/accounting_sh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-27 20:33:13.000000 accounting_sh-0.0.5/accounting_sh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:33:13.000000 accounting_sh-0.0.5/accounting_sh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-27 20:33:13.000000 accounting_sh-0.0.5/accounting_sh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 20:33:13.000000 accounting_sh-0.0.5/accounting_sh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 20:33:13.086457 accounting_sh-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:33:13.086457 accounting_sh-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_account_connections_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_accounting_codes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_accounts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_attachments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_bills_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_categories_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_company_statistics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_countries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_credentials_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_currency_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_documents_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7306 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_expense_reports_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_export_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_invoices_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_logs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_notification_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_o_auth_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_payments_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_quotes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_receipts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_revenues_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_rossum_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_search_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_tax_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_transactions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_transfers_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_vatid_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-27 20:33:04.000000 accounting_sh-0.0.5/test/test_webhooks_api.py
```

### Comparing `accounting_sh-0.0.4/LICENSE` & `accounting_sh-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/PKG-INFO` & `accounting_sh-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accounting_sh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Accounting API
 Home-page: 
 Author: STAN-TAB CORP. LTD
 Author-email: "STAN-TAB CORP. LTD" <support@stantabcorp.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,15 @@
 
 # accounting-sh
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: VERSION_HERE
-- Package version: 0.0.4
+- Package version: 0.0.5
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://accounting.sh](https://accounting.sh)
 
 ## Requirements.
```

### Comparing `accounting_sh-0.0.4/README.md` & `accounting_sh-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # accounting-sh
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: VERSION_HERE
-- Package version: 0.0.4
+- Package version: 0.0.5
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://accounting.sh](https://accounting.sh)
 
 ## Requirements.
```

### Comparing `accounting_sh-0.0.4/accounting_sh/__init__.py` & `accounting_sh-0.0.5/accounting_sh/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     The version of the OpenAPI document: VERSION_HERE
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 # import ApiClient
 from accounting_sh.accounting import Accounting
 
 # import apis into sdk package
 from accounting_sh.api.account_connections_api import AccountConnectionsApi
 from accounting_sh.api.accounting_codes_api import AccountingCodesApi
```

### Comparing `accounting_sh-0.0.4/accounting_sh/accounting.py` & `accounting_sh-0.0.5/accounting_sh/accounting.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
         :param path:
         :param comment:
         :param kwargs:
         :return:
         """
         kwargs.setdefault("headers", {})
         kwargs["headers"]["Authorization"] = f"Bearer {self.token}"
-        kwargs["headers"]["User-Agent"] = "AccountingSh/0.0.4/python"
+        kwargs["headers"]["User-Agent"] = "AccountingSh/0.0.5/python"
 
         if comment is not None:
             kwargs["headers"]["X-Audit-Comment"] = comment
 
         resp = requests.request(method, urljoin(self.url, path), **kwargs)
 
         if 200 <= resp.status_code <= 300:
```

### Comparing `accounting_sh-0.0.4/accounting_sh/api/__init__.py` & `accounting_sh-0.0.5/accounting_sh/api/__init__.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/account_connections_api.py` & `accounting_sh-0.0.5/accounting_sh/api/account_connections_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/accounting_codes_api.py` & `accounting_sh-0.0.5/accounting_sh/api/accounting_codes_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/accounts_api.py` & `accounting_sh-0.0.5/accounting_sh/api/accounts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/attachments_api.py` & `accounting_sh-0.0.5/accounting_sh/api/attachments_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/bills_api.py` & `accounting_sh-0.0.5/accounting_sh/api/bills_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/categories_api.py` & `accounting_sh-0.0.5/accounting_sh/api/categories_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/companies_api.py` & `accounting_sh-0.0.5/accounting_sh/api/companies_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/company_statistics_api.py` & `accounting_sh-0.0.5/accounting_sh/api/company_statistics_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/contacts_api.py` & `accounting_sh-0.0.5/accounting_sh/api/contacts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/countries_api.py` & `accounting_sh-0.0.5/accounting_sh/api/countries_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/credentials_api.py` & `accounting_sh-0.0.5/accounting_sh/api/credentials_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/currency_api.py` & `accounting_sh-0.0.5/accounting_sh/api/currency_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/documents_api.py` & `accounting_sh-0.0.5/accounting_sh/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/expense_reports_api.py` & `accounting_sh-0.0.5/accounting_sh/api/expense_reports_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/export_api.py` & `accounting_sh-0.0.5/accounting_sh/api/export_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/invoices_api.py` & `accounting_sh-0.0.5/accounting_sh/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/logs_api.py` & `accounting_sh-0.0.5/accounting_sh/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/notification_api.py` & `accounting_sh-0.0.5/accounting_sh/api/notification_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/notification_types_api.py` & `accounting_sh-0.0.5/accounting_sh/api/notification_types_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/o_auth_config_api.py` & `accounting_sh-0.0.5/accounting_sh/api/o_auth_config_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/payments_api.py` & `accounting_sh-0.0.5/accounting_sh/api/payments_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/quotes_api.py` & `accounting_sh-0.0.5/accounting_sh/api/quotes_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/receipts_api.py` & `accounting_sh-0.0.5/accounting_sh/api/receipts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/revenues_api.py` & `accounting_sh-0.0.5/accounting_sh/api/revenues_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/rossum_api.py` & `accounting_sh-0.0.5/accounting_sh/api/rossum_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/search_api.py` & `accounting_sh-0.0.5/accounting_sh/api/search_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/settings_api.py` & `accounting_sh-0.0.5/accounting_sh/api/settings_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/tags_api.py` & `accounting_sh-0.0.5/accounting_sh/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/tax_api.py` & `accounting_sh-0.0.5/accounting_sh/api/tax_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/transactions_api.py` & `accounting_sh-0.0.5/accounting_sh/api/transactions_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/transfers_api.py` & `accounting_sh-0.0.5/accounting_sh/api/transfers_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/vatid_api.py` & `accounting_sh-0.0.5/accounting_sh/api/vatid_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh/api/webhooks_api.py` & `accounting_sh-0.0.5/accounting_sh/api/webhooks_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/accounting_sh.egg-info/PKG-INFO` & `accounting_sh-0.0.5/accounting_sh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accounting_sh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Accounting API
 Home-page: 
 Author: STAN-TAB CORP. LTD
 Author-email: "STAN-TAB CORP. LTD" <support@stantabcorp.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -232,15 +232,15 @@
 
 # accounting-sh
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: VERSION_HERE
-- Package version: 0.0.4
+- Package version: 0.0.5
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 For more information, please visit [https://accounting.sh](https://accounting.sh)
 
 ## Requirements.
```

### Comparing `accounting_sh-0.0.4/accounting_sh.egg-info/SOURCES.txt` & `accounting_sh-0.0.5/accounting_sh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/pyproject.toml` & `accounting_sh-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "accounting_sh"
-version = "0.0.4"
+version = "0.0.5"
 description = "Accounting API"
 authors = [{"name" = "STAN-TAB CORP. LTD", email="support@stantabcorp.com"}]
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["OpenAPI", "Accounting API"]
 requires-python = ">=3.10"
```

### Comparing `accounting_sh-0.0.4/setup.py` & `accounting_sh-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "accounting-sh"
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "requests >= 2.32.3",
     "typing-extensions >= 4.7.1",
 ]
 
 setup(
```

### Comparing `accounting_sh-0.0.4/test/test_account_connections_api.py` & `accounting_sh-0.0.5/test/test_account_connections_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_accounting_codes_api.py` & `accounting_sh-0.0.5/test/test_accounting_codes_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_accounts_api.py` & `accounting_sh-0.0.5/test/test_accounts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_attachments_api.py` & `accounting_sh-0.0.5/test/test_attachments_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_bills_api.py` & `accounting_sh-0.0.5/test/test_bills_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_categories_api.py` & `accounting_sh-0.0.5/test/test_categories_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_companies_api.py` & `accounting_sh-0.0.5/test/test_companies_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_company_statistics_api.py` & `accounting_sh-0.0.5/test/test_company_statistics_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_contacts_api.py` & `accounting_sh-0.0.5/test/test_contacts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_countries_api.py` & `accounting_sh-0.0.5/test/test_countries_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_credentials_api.py` & `accounting_sh-0.0.5/test/test_credentials_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_currency_api.py` & `accounting_sh-0.0.5/test/test_currency_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_documents_api.py` & `accounting_sh-0.0.5/test/test_documents_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_expense_reports_api.py` & `accounting_sh-0.0.5/test/test_expense_reports_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_export_api.py` & `accounting_sh-0.0.5/test/test_export_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_invoices_api.py` & `accounting_sh-0.0.5/test/test_invoices_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_logs_api.py` & `accounting_sh-0.0.5/test/test_logs_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_notification_api.py` & `accounting_sh-0.0.5/test/test_notification_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_notification_types_api.py` & `accounting_sh-0.0.5/test/test_notification_types_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_o_auth_config_api.py` & `accounting_sh-0.0.5/test/test_o_auth_config_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_payments_api.py` & `accounting_sh-0.0.5/test/test_payments_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_quotes_api.py` & `accounting_sh-0.0.5/test/test_quotes_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_receipts_api.py` & `accounting_sh-0.0.5/test/test_receipts_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_revenues_api.py` & `accounting_sh-0.0.5/test/test_revenues_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_rossum_api.py` & `accounting_sh-0.0.5/test/test_rossum_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_search_api.py` & `accounting_sh-0.0.5/test/test_search_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_settings_api.py` & `accounting_sh-0.0.5/test/test_settings_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_tags_api.py` & `accounting_sh-0.0.5/test/test_tags_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_tax_api.py` & `accounting_sh-0.0.5/test/test_tax_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_transactions_api.py` & `accounting_sh-0.0.5/test/test_transactions_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_transfers_api.py` & `accounting_sh-0.0.5/test/test_transfers_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_vatid_api.py` & `accounting_sh-0.0.5/test/test_vatid_api.py`

 * *Files identical despite different names*

### Comparing `accounting_sh-0.0.4/test/test_webhooks_api.py` & `accounting_sh-0.0.5/test/test_webhooks_api.py`

 * *Files identical despite different names*

