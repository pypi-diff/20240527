# Comparing `tmp/hapi_schema-0.8.6.tar.gz` & `tmp/hapi_schema-0.8.7.tar.gz`

## Comparing `hapi_schema-0.8.6.tar` & `hapi_schema-0.8.7.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     3706 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_currency.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_food_price.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_views_as_tables.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_wfp_commodity.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/db_wfp_market.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/hapi_views_code_generator.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/view_as_table_definitions.toml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/conftest.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_admin1.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_admin2.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_conflict_event.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_currency.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_dataset.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_food_price.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_food_security.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_funding.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_location.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_national_risk.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_operational_presence.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_org_type.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_patch.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_population.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_refugees.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_sector.py
--rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_views_as_tables.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_wfp_commodity.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/test_wfp_market.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_currency.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_food_price.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_wfp_commodity.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/tests/sample_data/data_wfp_market.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/conftest.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_admin1.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_admin2.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_dataset.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_food_price.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_food_security.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_funding.py
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_location.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_patch.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_population.py
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_sector.py
+-rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/PKG-INFO
```

### Comparing `hapi_schema-0.8.6/changelog.md` & `hapi_schema-0.8.7/changelog.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.7
+
+## Changes
+- Add unit to food\_price table primary key
+
 ## 0.8.6
 
 ## Changes
 - Added food\_price view as tables by updating the toml parameter file
 - Updated poverty\_rate view as table
 - Updated operational\_presence view as table by updating the toml parameter file
 - Made a few adhoc changes to the view as table generator code to accommodate Decimal columns
```

### Comparing `hapi_schema-0.8.6/contributing.md` & `hapi_schema-0.8.7/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/requirements.txt` & `hapi_schema-0.8.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/.config/pre-commit-config.yaml` & `hapi_schema-0.8.7/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/.github/workflows/publish.yaml` & `hapi_schema-0.8.7/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.7/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.7/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.7/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.7/src/hapi_schema/db_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_currency.py` & `hapi_schema-0.8.7/src/hapi_schema/db_currency.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.7/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_food_price.py` & `hapi_schema-0.8.7/src/hapi_schema/db_food_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         ForeignKey("wfp_commodity.code"), primary_key=True
     )
     currency_code: Mapped[str] = mapped_column(
         ForeignKey("currency.code", onupdate="CASCADE"),
         nullable=False,
         index=True,
     )
-    unit: Mapped[str] = mapped_column(String(32), nullable=False)
+    unit: Mapped[str] = mapped_column(String(32), primary_key=True)
     price_flag: Mapped[PriceFlag] = mapped_column(
         Enum(PriceFlag), primary_key=True
     )
     price_type: Mapped[PriceType] = mapped_column(
         Enum(PriceType), primary_key=True
     )
     price: Mapped[Decimal] = mapped_column(nullable=False)
```

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.7/src/hapi_schema/db_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.7/src/hapi_schema/db_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.8.7/src/hapi_schema/db_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_location.py` & `hapi_schema-0.8.7/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.7/src/hapi_schema/db_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.8.7/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_org.py` & `hapi_schema-0.8.7/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.7/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.7/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_population.py` & `hapi_schema-0.8.7/src/hapi_schema/db_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.7/src/hapi_schema/db_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.7/src/hapi_schema/db_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_resource.py` & `hapi_schema-0.8.7/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.7/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_views_as_tables.py` & `hapi_schema-0.8.7/src/hapi_schema/db_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_wfp_commodity.py` & `hapi_schema-0.8.7/src/hapi_schema/db_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/db_wfp_market.py` & `hapi_schema-0.8.7/src/hapi_schema/db_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/views.py` & `hapi_schema-0.8.7/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.7/src/hapi_schema/utils/constraints.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.7/src/hapi_schema/utils/enums.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/utils/hapi_views_code_generator.py` & `hapi_schema-0.8.7/src/hapi_schema/utils/hapi_views_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/src/hapi_schema/utils/view_as_table_definitions.toml` & `hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_definitions.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/conftest.py` & `hapi_schema-0.8.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_admin1.py` & `hapi_schema-0.8.7/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_admin2.py` & `hapi_schema-0.8.7/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_conflict_event.py` & `hapi_schema-0.8.7/tests/test_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_dataset.py` & `hapi_schema-0.8.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_food_price.py` & `hapi_schema-0.8.7/tests/test_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_food_security.py` & `hapi_schema-0.8.7/tests/test_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_funding.py` & `hapi_schema-0.8.7/tests/test_funding.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.7/tests/test_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_location.py` & `hapi_schema-0.8.7/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_national_risk.py` & `hapi_schema-0.8.7/tests/test_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_operational_presence.py` & `hapi_schema-0.8.7/tests/test_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_patch.py` & `hapi_schema-0.8.7/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_population.py` & `hapi_schema-0.8.7/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_poverty_rate.py` & `hapi_schema-0.8.7/tests/test_poverty_rate.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_refugees.py` & `hapi_schema-0.8.7/tests/test_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_views_as_tables.py` & `hapi_schema-0.8.7/tests/test_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_wfp_commodity.py` & `hapi_schema-0.8.7/tests/test_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/test_wfp_market.py` & `hapi_schema-0.8.7/tests/test_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.7/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.7/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_food_price.py` & `hapi_schema-0.8.7/tests/sample_data/data_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.7/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.8.7/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.7/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.7/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_patch.py` & `hapi_schema-0.8.7/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_population.py` & `hapi_schema-0.8.7/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.7/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/tests/sample_data/data_resource.py` & `hapi_schema-0.8.7/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/.gitignore` & `hapi_schema-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/LICENSE` & `hapi_schema-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/pyproject.toml` & `hapi_schema-0.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.6/PKG-INFO` & `hapi_schema-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.6
+Version: 0.8.7
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

