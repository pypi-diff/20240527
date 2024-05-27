# Comparing `tmp/hapi_schema-0.8.7.tar.gz` & `tmp/hapi_schema-0.8.8.tar.gz`

## Comparing `hapi_schema-0.8.7.tar` & `hapi_schema-0.8.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/changelog.md
--rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/contributing.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/initialize_test_db.sh
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/coveragerc
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.config/ruff.toml
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/docker/docker-compose.yml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_conflict_event.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_currency.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_food_price.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_funding.py
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_patch.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_poverty_rate.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_refugees.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_views_as_tables.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_wfp_commodity.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/db_wfp_market.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/constraints.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/enums.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/hapi_views_code_generator.py
--rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_code_generator.py
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_definitions.toml
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/conftest.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_admin1.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_admin2.py
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_conflict_event.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_currency.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_dataset.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_food_price.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_food_security.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_funding.py
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_location.py
--rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_national_risk.py
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_operational_presence.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_org.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_org_type.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_patch.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_population.py
--rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_poverty_rate.py
--rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_refugees.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_resource.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_sector.py
--rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_views_as_tables.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_wfp_commodity.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/test_wfp_market.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_conflict_event.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_currency.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_food_price.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_funding.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_patch.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_poverty_rate.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_refugees.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_wfp_commodity.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/tests/sample_data/data_wfp_market.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/README.md
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/changelog.md
+-rw-r--r--   0        0        0     2735 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/contributing.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/initialize_test_db.sh
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/coveragerc
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.config/ruff.toml
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/docker/docker-compose.yml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0     2979 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_conflict_event.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_currency.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_food_price.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_funding.py
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_poverty_rate.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_refugees.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0    19527 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_views_as_tables.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_wfp_commodity.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/db_wfp_market.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/constraints.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/enums.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/hapi_views_code_generator.py
+-rw-r--r--   0        0        0     6259 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_code_generator.py
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_definitions.toml
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/conftest.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_admin1.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_admin2.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_conflict_event.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_currency.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_dataset.py
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_food_price.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_food_security.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_funding.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_location.py
+-rw-r--r--   0        0        0     5310 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_operational_presence.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_org.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_org_type.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_patch.py
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_population.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_poverty_rate.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_refugees.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_resource.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_sector.py
+-rw-r--r--   0        0        0    15338 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_views_as_tables.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_wfp_commodity.py
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/test_wfp_market.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_conflict_event.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_currency.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_food_price.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_funding.py
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_poverty_rate.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_refugees.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_wfp_commodity.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/tests/sample_data/data_wfp_market.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/README.md
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 hapi_schema-0.8.8/PKG-INFO
```

### Comparing `hapi_schema-0.8.7/changelog.md` & `hapi_schema-0.8.8/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 0.8.8
+
+### Changes
+
+- Rewrite enums to use values rather than variable names
+- Switch from "*" to "all" for rollup in enums
+- Add "intersectoral" to sample sector data (distinct from "all")
+- Ensure that constraint names end consistently with "\_constraint"
+
 ## 0.8.7
 
 ## Changes
 - Add unit to food\_price table primary key
 
 ## 0.8.6
```

### Comparing `hapi_schema-0.8.7/contributing.md` & `hapi_schema-0.8.8/contributing.md`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/requirements.txt` & `hapi_schema-0.8.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/.config/pre-commit-config.yaml` & `hapi_schema-0.8.8/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/.github/workflows/publish.yaml` & `hapi_schema-0.8.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.8.8/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_admin1.py` & `hapi_schema-0.8.8/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_admin2.py` & `hapi_schema-0.8.8/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_conflict_event.py` & `hapi_schema-0.8.8/src/hapi_schema/db_conflict_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """ConflictEvent table and view."""
 
 from datetime import datetime
 
 from sqlalchemy import (
     DateTime,
-    Enum,
     ForeignKey,
     Integer,
     select,
 )
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 from hapi_schema.db_admin1 import DBAdmin1, DBLocation
 from hapi_schema.db_admin2 import DBAdmin2
 from hapi_schema.utils.base import Base
 from hapi_schema.utils.constraints import (
     population_constraint,
     reference_period_constraint,
 )
-from hapi_schema.utils.enums import EventType
+from hapi_schema.utils.enums import EventType, build_enum_using_values
 from hapi_schema.utils.view_params import ViewParams
 
 
 # normalised table
 class DBConflictEvent(Base):
     __tablename__ = "conflict_event"
     __table_args__ = (
@@ -39,15 +38,15 @@
     )
     admin2_ref: Mapped[int] = mapped_column(
         ForeignKey("admin2.id", onupdate="CASCADE"),
         nullable=False,
         primary_key=True,
     )
     event_type: Mapped[EventType] = mapped_column(
-        Enum(EventType), nullable=False, primary_key=True
+        build_enum_using_values(EventType), nullable=False, primary_key=True
     )
     events: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     fatalities: Mapped[int] = mapped_column(Integer, nullable=True, index=True)
     reference_period_start: Mapped[datetime] = mapped_column(
         DateTime, primary_key=True
     )
     reference_period_end: Mapped[datetime] = mapped_column(
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_currency.py` & `hapi_schema-0.8.8/src/hapi_schema/db_currency.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_dataset.py` & `hapi_schema-0.8.8/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_food_price.py` & `hapi_schema-0.8.8/src/hapi_schema/db_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_food_security.py` & `hapi_schema-0.8.8/src/hapi_schema/db_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_funding.py` & `hapi_schema-0.8.8/src/hapi_schema/db_funding.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 
 
 class DBFunding(Base):
     __tablename__ = "funding"
     __table_args__ = (
         CheckConstraint(
             "requirements_usd >= 0.0",
-            name="requirements_usd",
+            name="requirements_usd_constraint",
         ),
         CheckConstraint(
             "funding_usd >= 0.0",
-            name="funding_usd",
+            name="funding_usd_constraint",
         ),
         CheckConstraint(
             "funding_pct >= 0.0",
-            name="funding_pct",
+            name="funding_pct_constraint",
         ),
         reference_period_constraint(),
     )
 
     resource_hdx_id = mapped_column(
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.8.8/src/hapi_schema/db_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_location.py` & `hapi_schema-0.8.8/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.8.8/src/hapi_schema/db_national_risk.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     __tablename__ = "national_risk"
     __table_args__ = (
         general_risk_constraint("overall"),
         general_risk_constraint("hazard_exposure"),
         general_risk_constraint("vulnerability"),
         general_risk_constraint("coping_capacity"),
         CheckConstraint(
-            "(global_rank >= 1) AND (global_rank <= 250)", name="global_rank"
+            "(global_rank >= 1) AND (global_rank <= 250)",
+            name="global_rank_constraint",
         ),
         CheckConstraint(
             "meta_avg_recentness_years >= 0.0",
             name="meta_avg_recentness_years",
         ),
         CheckConstraint(
             "(meta_missing_indicators_pct >= 0.0) AND (meta_missing_indicators_pct <= 100.0)",
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.8.8/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_org.py` & `hapi_schema-0.8.8/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_org_type.py` & `hapi_schema-0.8.8/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_patch.py` & `hapi_schema-0.8.8/src/hapi_schema/db_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_population.py` & `hapi_schema-0.8.8/src/hapi_schema/db_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_poverty_rate.py` & `hapi_schema-0.8.8/src/hapi_schema/db_poverty_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         percentage_constraint(var_name="headcount_ratio"),
         percentage_constraint(var_name="intensity_of_deprivation"),
         percentage_constraint(var_name="vulnerable_to_poverty"),
         percentage_constraint(var_name="in_severe_poverty"),
         reference_period_constraint(),
         CheckConstraint(
             sqltext="ABS(headcount_ratio / 100 * intensity_of_deprivation / 100  - mpi) < 0.00001",
-            name="mpi_product",
+            name="mpi_product_constraint",
         ),
     )
 
     resource_hdx_id: Mapped[str] = mapped_column(
         ForeignKey("resource.hdx_id", onupdate="CASCADE", ondelete="CASCADE"),
         nullable=False,
     )
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_refugees.py` & `hapi_schema-0.8.8/src/hapi_schema/db_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_resource.py` & `hapi_schema-0.8.8/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_sector.py` & `hapi_schema-0.8.8/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_views_as_tables.py` & `hapi_schema-0.8.8/src/hapi_schema/db_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_wfp_commodity.py` & `hapi_schema-0.8.8/src/hapi_schema/db_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/db_wfp_market.py` & `hapi_schema-0.8.8/src/hapi_schema/db_wfp_market.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/views.py` & `hapi_schema-0.8.8/src/hapi_schema/views.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/utils/constraints.py` & `hapi_schema-0.8.8/src/hapi_schema/utils/constraints.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 
 def min_age_constraint() -> CheckConstraint:
     """If the age range is rolled up, min_age should be NULL.
     Otherwise, it can be NULL for unknown, or should be an
     integer of 0 or greater."""
     sqltext = (
-        "(age_range = '*' AND min_age IS NULL) OR "
-        "(age_range != '*' AND (min_age >= 0 OR min_age is NULL))"
+        "(age_range = 'all' AND min_age IS NULL) OR "
+        "(age_range != 'all' AND min_age >= 0)"
     )
     return CheckConstraint(sqltext=sqltext, name="min_age_constraint")
 
 
 def max_age_constraint() -> CheckConstraint:
     """If min_age is NULL, max age should also be NULL.
     Otherwise, when min_age is an integer, max age should be equal to
@@ -28,48 +28,52 @@
 
 
 def population_constraint(
     population_var_name: str = "population",
 ) -> CheckConstraint:
     """Population must not be a negative number."""
     sqltext = f"{population_var_name} >= 0"
-    return CheckConstraint(sqltext=sqltext, name=f"{population_var_name}")
+    return CheckConstraint(
+        sqltext=sqltext, name=f"{population_var_name}_constraint"
+    )
 
 
 def non_negative_constraint(
     var_name: str,
 ) -> CheckConstraint:
     """Require a column to be non-negative."""
     sqltext = f"{var_name} >= 0"
-    return CheckConstraint(sqltext=sqltext, name=f"{var_name}")
+    return CheckConstraint(sqltext=sqltext, name=f"{var_name}_constraint")
 
 
 def percentage_constraint(var_name: str) -> CheckConstraint:
     sqltext = f"{var_name} >= 0. AND {var_name} <= 100."
-    return CheckConstraint(sqltext=sqltext, name=f"{var_name}")
+    return CheckConstraint(sqltext=sqltext, name=f"{var_name}_constraint")
 
 
 def reference_period_constraint() -> CheckConstraint:
     """reference_period_end should be greater than reference_period_start"""
     sqltext = "reference_period_end >= reference_period_start "
-    return CheckConstraint(sqltext=sqltext, name="reference_period")
+    return CheckConstraint(sqltext=sqltext, name="reference_period_constraint")
 
 
 def general_risk_constraint(risk_name: str) -> CheckConstraint:
     sqltext = f"({risk_name}_risk >= 0) AND ({risk_name}_risk <= 10)"
-    return CheckConstraint(sqltext=sqltext, name=f"{risk_name}_risk")
+    return CheckConstraint(
+        sqltext=sqltext, name=f"{risk_name}_risk_constraint"
+    )
 
 
 def code_and_reference_period_unique_constraint(
     admin_level: str,
 ) -> UniqueConstraint:
     return UniqueConstraint(
         "code",
         "reference_period_start",
-        name=f"{admin_level}_code_and_reference_period_unique",
+        name=f"{admin_level}_code_and_reference_period_unique_constraint",
     )
 
 
 def latlon_constraint() -> CheckConstraint:
     """Latitude and longitude must be valid"""
     sqltext = "lat <= 90.0 AND lat >= -90.0 AND lon <= 180.0 AND lon >= -180.0"
-    return CheckConstraint(sqltext=sqltext, name="latlon")
+    return CheckConstraint(sqltext=sqltext, name="latlon_constraint")
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/utils/enums.py` & `hapi_schema-0.8.8/src/hapi_schema/utils/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-import enum
+from enum import Enum as PythonEnum
+from typing import List
 
+from sqlalchemy import Enum as SQLAlchemyEnum
 
-class Gender(str, enum.Enum):
+"""The two functions below create enums using the values rather than the keys"""
+
+
+def _get_list_of_values(enum_class: PythonEnum) -> List[str]:
+    return [e.value for e in enum_class]
+
+
+def build_enum_using_values(enum_class: PythonEnum) -> SQLAlchemyEnum:
+    return SQLAlchemyEnum(enum_class, values_callable=_get_list_of_values)
+
+
+class Gender(str, PythonEnum):
     FEMALE = "f"
     MALE = "m"
     NONBINARY = "x"
     UNSPECIFIED = "u"
     OTHER = "o"
-    ALL = "*"
+    ALL = "all"
 
 
-class DisabledMarker(str, enum.Enum):
+class DisabledMarker(str, PythonEnum):
     YES = "y"
     NO = "n"
-    ALL = "*"
+    ALL = "all"
 
 
-class EventType(str, enum.Enum):
+class EventType(str, PythonEnum):
     CIVILIAN_TARGETING = "civilian_targeting"
     DEMONSTRATION = "demonstration"
     POLITICAL_VIOLENCE = "political_violence"
 
 
-class PopulationGroup(str, enum.Enum):
+class PopulationGroup(str, PythonEnum):
     REFUGEES = "REF"
     ROC = "ROC"
     ASYLUM_SEEKERS = "ASY"
     OIP = "OIP"
     IDP = "IDP"
     IOC = "IOC"
     STATELESS = "STA"
@@ -34,63 +47,63 @@
     HOST_COMMUNITY = "HST"
     RET = "RET"
     RESETTLED = "RST"
     NATURALIZED = "NAT"
     POC = "POC"
     RDP = "RDP"
     RRI = "RRI"
-    ALL = "*"
+    ALL = "all"
 
 
-class PopulationStatus(str, enum.Enum):
+class PopulationStatus(str, PythonEnum):
     POPULATION = "POP"
     AFFECTED = "AFF"
     INNEED = "INN"
     TARGETED = "TGT"
     REACHED = "REA"
-    ALL = "*"
+    ALL = "all"
 
 
-class PriceFlag(str, enum.Enum):
+class PriceFlag(str, PythonEnum):
     ACTUAL = "actual"
     AGGREGATE = "aggregate"
     ACTUAL_AGGREGATE = "actual,aggregate"
 
 
-class PriceType(str, enum.Enum):
+class PriceType(str, PythonEnum):
     FARM_GATE = "Farm Gate"
     RETAIL = "Retail"
     WHOLESALE = "Wholesale"
 
 
-class IPCPhase(str, enum.Enum):
+class IPCPhase(str, PythonEnum):
     PHASE_1 = "1"
     PHASE_2 = "2"
     PHASE_3 = "3"
     PHASE_4 = "4"
     PHASE_5 = "5"
     PHASE_3_PLUS = "3+"
-    ALL = "*"
+    ALL = "all"
 
 
-class IPCType(str, enum.Enum):
+class IPCType(str, PythonEnum):
     CURRENT = "current"
     FIRST_PROJECTION = "first projection"
     SECOND_PROJECTION = "second projection"
 
 
-class RiskClass(str, enum.Enum):
+class RiskClass(str, PythonEnum):
     VERY_LOW = "1"
     LOW = "2"
     MEDIUM = "3"
     HIGH = "4"
     VERY_HIGH = "5"
 
 
-class CommodityCategory(str, enum.Enum):
+class CommodityCategory(str, PythonEnum):
     CEREALS_TUBERS = "cereals and tubers"
     MEAT_FISH_EGGS = "meat, fish and eggs"
     MILK_DAIRY = "milk and dairy"
     MISCELLANEOUS_FOOD = "miscellaneous food"
     NON_FOOD = "non-food"
     OIL_FATS = "oil and fats"
     PULSES_NUTS = "pulses and nuts"
```

### Comparing `hapi_schema-0.8.7/src/hapi_schema/utils/hapi_views_code_generator.py` & `hapi_schema-0.8.8/src/hapi_schema/utils/hapi_views_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_code_generator.py` & `hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_code_generator.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/src/hapi_schema/utils/view_as_table_definitions.toml` & `hapi_schema-0.8.8/src/hapi_schema/utils/view_as_table_definitions.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/conftest.py` & `hapi_schema-0.8.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/test_admin1.py` & `hapi_schema-0.8.8/tests/test_admin1.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 code="FOO-003",
                 name="Province 3",
                 is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_code_date_unique(run_constraints_test):
     """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
@@ -61,9 +61,9 @@
                 location_ref=1,
                 code="FOO-003",
                 name="Province 3",
                 is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="admin1_code_and_reference_period_unique",
+        expected_constraint="admin1_code_and_reference_period_unique_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_admin2.py` & `hapi_schema-0.8.8/tests/test_admin2.py`

 * *Files 23% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 code="FOO-002-D",
                 name="District D",
                 is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_code_date_unique(run_constraints_test):
     """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
@@ -62,9 +62,9 @@
                 admin1_ref=3,
                 code="FOO-002-D",
                 name="District D",
                 is_unspecified=False,
                 reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="admin2_code_and_reference_period_unique",
+        expected_constraint="admin2_code_and_reference_period_unique_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_conflict_event.py` & `hapi_schema-0.8.8/tests/test_conflict_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -42,33 +42,33 @@
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["events"] = -1
     run_constraints_test(
         new_rows=[
             DBConflictEvent(**data),
         ],
-        expected_constraint="events",
+        expected_constraint="events_constraint",
     )
 
 
 def test_fatalities_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["fatalities"] = -1
     run_constraints_test(
         new_rows=[
             DBConflictEvent(**data),
         ],
-        expected_constraint="fatalities",
+        expected_constraint="fatalities_constraint",
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["reference_period_start"] = datetime(2025, 1, 1)
     run_constraints_test(
         new_rows=[
             DBConflictEvent(**data),
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_dataset.py` & `hapi_schema-0.8.8/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/test_food_price.py` & `hapi_schema-0.8.8/tests/test_food_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,27 @@
     """Check constraint that price is not negative"""
     data = _sample_data()
     data["price"] = -1.0
     run_constraints_test(
         new_rows=[
             DBFoodPrice(**data),
         ],
-        expected_constraint="price",
+        expected_constraint="price_constraint",
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["reference_period_start"] = datetime(2025, 1, 1)
     run_constraints_test(
         new_rows=[
             DBFoodPrice(**data),
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 # Utility functions
 
 
 def _sample_data():
```

### Comparing `hapi_schema-0.8.7/tests/test_food_security.py` & `hapi_schema-0.8.8/tests/test_food_security.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 ipc_type="current",
                 population_in_phase=1_000,
                 population_fraction_in_phase=1,
                 reference_period_start=datetime(2023, 2, 1),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_population_in_phase_positive(run_constraints_test):
     """Check that the population value is positive"""
     run_constraints_test(
         new_rows=[
@@ -55,9 +55,9 @@
                 ipc_type="current",
                 population_in_phase=-1,
                 population_fraction_in_phase=1,
                 reference_period_start=datetime(2023, 1, 1),
                 reference_period_end=datetime(2023, 1, 2),
             )
         ],
-        expected_constraint="population_in_phase",
+        expected_constraint="population_in_phase_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_funding.py` & `hapi_schema-0.8.8/tests/test_funding.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 requirements_usd=100000.0,
                 funding_usd=50000.0,
                 funding_pct=50,
                 reference_period_start=datetime(2025, 1, 1),
                 reference_period_end=datetime(2024, 12, 31),
             ),
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_requirements_usd_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
@@ -63,15 +63,15 @@
                 requirements_usd=-100000.0,
                 funding_usd=50000.0,
                 funding_pct=50,
                 reference_period_start=datetime(2024, 1, 1),
                 reference_period_end=datetime(2024, 12, 31),
             ),
         ],
-        expected_constraint="requirements_usd",
+        expected_constraint="requirements_usd_constraint",
     )
 
 
 def test_funding_usd_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
@@ -84,15 +84,15 @@
                 requirements_usd=100000.0,
                 funding_usd=-50000.0,
                 funding_pct=50,
                 reference_period_start=datetime(2024, 1, 1),
                 reference_period_end=datetime(2024, 12, 31),
             ),
         ],
-        expected_constraint="funding_usd",
+        expected_constraint="funding_usd_constraint",
     )
 
 
 def test_funding_pct_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
@@ -105,9 +105,9 @@
                 requirements_usd=100000.0,
                 funding_usd=50000.0,
                 funding_pct=-50,
                 reference_period_start=datetime(2024, 1, 1),
                 reference_period_end=datetime(2024, 12, 31),
             ),
         ],
-        expected_constraint="funding_pct",
+        expected_constraint="funding_pct_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_humanitarian_needs.py` & `hapi_schema-0.8.8/tests/test_humanitarian_needs.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,52 +73,52 @@
 def test_population_positive(run_constraints_test, base_parameters):
     """Check that the population value is positive"""
     modified_params = {**base_parameters, "population": -1}
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(**modified_params),
         ],
-        expected_constraint="population",
+        expected_constraint="population_constraint",
     )
 
 
 def test_minage(run_constraints_test, base_parameters):
     """Check that the min_age value is positive, and NULL if
-    age_range is *"""
+    age_range is all"""
     modified_params = {**base_parameters, **dict(age_range="5-10", min_age=-1)}
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="min_age_constraint",
     )
-    modified_params = {**base_parameters, **dict(age_range="*", min_age=10)}
+    modified_params = {**base_parameters, **dict(age_range="all", min_age=10)}
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="min_age_constraint",
     )
 
 
 def test_maxage(run_constraints_test, base_parameters):
     """Check that the max_age is > min_age, and NULL when min_age is NULL"""
     modified_params = {
         **base_parameters,
         **dict(age_range="5-10", min_age=5, max_age=4),
     }
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="max_age_constraint",
     )
     modified_params = {
         **base_parameters,
         **dict(age_range="unknown", min_age=None, max_age=10),
     }
     run_constraints_test(
         new_rows=[
             DBHumanitarianNeeds(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="max_age_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_location.py` & `hapi_schema-0.8.8/tests/test_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             DBLocation(
                 code="BAR",
                 name="Barlandia",
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_code_date_unique(run_constraints_test):
     """Check that reference_period_start and code must be unique together"""
     run_constraints_test(
         new_rows=[
@@ -56,9 +56,9 @@
             ),
             DBLocation(
                 code="BAR",
                 name="Barlandia",
                 reference_period_start=datetime(2023, 1, 1),
             ),
         ],
-        expected_constraint="location_code_and_reference_period_unique",
+        expected_constraint="location_code_and_reference_period_unique_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_national_risk.py` & `hapi_schema-0.8.8/tests/test_national_risk.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,44 +33,49 @@
         global_rank=4,
         overall_risk=8.1,
         hazard_exposure_risk=8.7,
         vulnerability_risk=8.5,
         coping_capacity_risk=7.1,
         meta_missing_indicators_pct=8,
         meta_avg_recentness_years=0.26,
+        reference_period_start=datetime(2023, 1, 1),
+        reference_period_end=datetime(2023, 1, 2),
     )
 
 
 def test_reference_period_constraint(run_constraints_test, base_parameters):
     """Check that reference_period_end cannot be less than start"""
+    modified_params = {
+        **base_parameters,
+        **dict(
+            reference_period_start=datetime(2023, 1, 2),
+            reference_period_end=datetime(2023, 1, 1),
+        ),
+    }
     run_constraints_test(
         new_rows=[
             DBNationalRisk(
-                **base_parameters,
-                **dict(
-                    reference_period_start=datetime(2023, 1, 2),
-                    reference_period_end=datetime(2023, 1, 1),
-                ),
+                **modified_params,
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_overall_risk_constraint(run_constraints_test, base_parameters):
     """Check that overall risk is >= 0 and <= 10"""
     modified_params = {**base_parameters, "overall_risk": -1}
     run_constraints_test(
         new_rows=[DBNationalRisk(**modified_params)],
-        expected_constraint="overall_risk",
+        expected_constraint="overall_risk_constraint",
     )
     modified_params = {**base_parameters, "overall_risk": 11}
     run_constraints_test(
         new_rows=[DBNationalRisk(**modified_params)],
-        expected_constraint="overall_risk",
+        expected_constraint="overall_risk_constraint",
     )
 
 
 def test_hazard_exposure_constraint(run_constraints_test, base_parameters):
     """Check that hazard exposure is >= 0 and <= 10"""
     modified_params = {**base_parameters, "hazard_exposure_risk": -1}
     run_constraints_test(
```

### Comparing `hapi_schema-0.8.7/tests/test_operational_presence.py` & `hapi_schema-0.8.8/tests/test_operational_presence.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,9 +41,9 @@
                 org_acronym="ORG01",
                 org_name="Organisation 1",
                 sector_code="SHL",
                 reference_period_start=datetime(2023, 1, 2),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_patch.py` & `hapi_schema-0.8.8/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/test_population.py` & `hapi_schema-0.8.8/tests/test_population.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,78 +25,85 @@
 
 @pytest.fixture
 def base_parameters():
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         gender=Gender.ALL,
+        age_range="all",
         population=1_000_000,
+        reference_period_start=datetime(2020, 1, 1),
+        reference_period_end=datetime(2020, 1, 2),
     )
 
 
 def test_reference_period_constraint(run_constraints_test, base_parameters):
     """Check that reference_period_end cannot be less than start"""
     modified_params = {
         **base_parameters,
         **dict(
             reference_period_start=datetime(2023, 1, 2),
             reference_period_end=datetime(2023, 1, 1),
         ),
     }
     run_constraints_test(
         new_rows=[DBPopulation(**modified_params)],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def test_population_positive(run_constraints_test, base_parameters):
     """Check that the population value is positive"""
     modified_params = {**base_parameters, "population": -1}
     run_constraints_test(
         new_rows=[
             DBPopulation(**modified_params),
         ],
-        expected_constraint="population",
+        expected_constraint="population_constraint",
     )
 
 
 def test_minage(run_constraints_test, base_parameters):
     """Check that the min_age value is positive, and NULL if
-    age_range is *"""
+    age_range is all"""
     modified_params = {**base_parameters, **dict(age_range="5-10", min_age=-1)}
     run_constraints_test(
         new_rows=[
             DBPopulation(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="min_age_constraint",
     )
-    modified_params = {**base_parameters, **dict(age_range="*", min_age=10)}
+    modified_params = {
+        **base_parameters,
+        **dict(age_range="all", min_age="10"),
+    }
+    print(modified_params)
     run_constraints_test(
         new_rows=[
             DBPopulation(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="min_age_constraint",
     )
 
 
 def test_maxage(run_constraints_test, base_parameters):
     """Check that the max_age is > min_age, and NULL when min_age is NULL"""
     modified_params = {
         **base_parameters,
         **dict(age_range="5-10", min_age=5, max_age=4),
     }
     run_constraints_test(
         new_rows=[
             DBPopulation(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="max_age_constraint",
     )
     modified_params = {
         **base_parameters,
         **dict(age_range="unknown", min_age=None, max_age=10),
     }
     run_constraints_test(
         new_rows=[
             DBPopulation(**modified_params),
         ],
-        expected_constraint="min_age",
+        expected_constraint="max_age_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_poverty_rate.py` & `hapi_schema-0.8.8/tests/test_poverty_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,75 +28,75 @@
     """Check that headcount ratio is between 0 and 100"""
     data = _sample_data()
     data["headcount_ratio"] = 101
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="headcount_ratio",
+        expected_constraint="headcount_ratio_constraint",
     )
 
 
 def test_intensity_of_deprivation_constraint(run_constraints_test):
     """Check that intensity of deprivation is between 0 and 100"""
     data = _sample_data()
     data["intensity_of_deprivation"] = 101
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="intensity_of_deprivation",
+        expected_constraint="intensity_of_deprivation_constraint",
     )
 
 
 def test_vulnerable_to_poverty_constraint(run_constraints_test):
     """Check that vulnerable_to_poverty is between 0 and 100"""
     data = _sample_data()
     data["vulnerable_to_poverty"] = 101
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="vulnerable_to_poverty",
+        expected_constraint="vulnerable_to_poverty_constraint",
     )
 
 
 def test_in_severe_poverty_constraint(run_constraints_test):
     """Check that in_severe_poverty is between 0 and 100"""
     data = _sample_data()
     data["in_severe_poverty"] = 101
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="in_severe_poverty",
+        expected_constraint="in_severe_poverty_constraint",
     )
 
 
 def test_mpi_product_constraint(run_constraints_test):
-    """Check that MPI is between 0.0 and 1.0"""
+    """Check that MPI is the product of headcount and intensity"""
     data = _sample_data()
-    data["mpi"] = 1.1
+    data["mpi"] = 0.5
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="mpi_product",
+        expected_constraint="mpi_product_constraint",
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     data = _sample_data()
     data["reference_period_start"] = datetime(2025, 1, 1)
     run_constraints_test(
         new_rows=[
             DBPovertyRate(**data),
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
 
 
 def _sample_data():
     # return the whole record, then tests can change as needed
     return dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
```

### Comparing `hapi_schema-0.8.7/tests/test_refugees.py` & `hapi_schema-0.8.8/tests/test_refugees.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,37 +36,37 @@
                 min_age=-5,
                 max_age=12,
                 population=2000,
                 reference_period_start=datetime(2023, 1, 1),
                 reference_period_end=datetime(2023, 12, 31),
             )
         ],
-        expected_constraint="min_age",
+        expected_constraint="min_age_constraint",
     )
 
 
 def test_max_age(run_constraints_test):
-    """Check that the minimum age is greater than 0"""
+    """Check that the max age is greater than 0"""
     run_constraints_test(
         new_rows=[
             DBRefugees(
                 resource_hdx_id="62ad6e55-5f5d-4494-854c-4110687e9e25",
                 origin_location_ref=1,
                 asylum_location_ref=2,
                 population_group="REF",
                 gender="f",
                 age_range="children",
                 min_age=5,
-                max_age=1200,
+                max_age=-1,
                 population=2000,
                 reference_period_start=datetime(2023, 1, 1),
                 reference_period_end=datetime(2023, 12, 31),
             )
         ],
-        expected_constraint="max_age",
+        expected_constraint="max_age_constraint",
     )
 
 
 def test_population_positive(run_constraints_test):
     """Check that the population value is positive"""
     run_constraints_test(
         new_rows=[
@@ -80,15 +80,15 @@
                 min_age=5,
                 max_age=12,
                 population=-2000,
                 reference_period_start=datetime(2023, 1, 1),
                 reference_period_end=datetime(2023, 12, 31),
             )
         ],
-        expected_constraint="population",
+        expected_constraint="population_constraint",
     )
 
 
 def test_reference_period_constraint(run_constraints_test):
     """Check that reference_period_end cannot be less than start"""
     run_constraints_test(
         new_rows=[
@@ -102,9 +102,9 @@
                 min_age=5,
                 max_age=12,
                 population=2000,
                 reference_period_start=datetime(2023, 2, 1),
                 reference_period_end=datetime(2023, 1, 1),
             )
         ],
-        expected_constraint="reference_period",
+        expected_constraint="reference_period_constraint",
     )
```

### Comparing `hapi_schema-0.8.7/tests/test_views_as_tables.py` & `hapi_schema-0.8.8/tests/test_views_as_tables.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/test_wfp_commodity.py` & `hapi_schema-0.8.8/tests/test_wfp_commodity.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/test_wfp_market.py` & `hapi_schema-0.8.8/tests/test_wfp_market.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """Check that latlon constraint works with latitude"""
     data = _sample_data()
     data["lat"] = 91
     run_constraints_test(
         new_rows=[
             DBWFPMarket(**data),
         ],
-        expected_constraint="latlon",
+        expected_constraint="latlon_constraint",
     )
 
 
 def test_lon_constraint(run_constraints_test):
     """Check that latlon constraint works with longitude"""
     data = _sample_data()
     data["lon"] = -181
```

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_admin2.py` & `hapi_schema-0.8.8/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_conflict_event.py` & `hapi_schema-0.8.8/tests/sample_data/data_conflict_event.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_food_price.py` & `hapi_schema-0.8.8/tests/sample_data/data_food_price.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_food_security.py` & `hapi_schema-0.8.8/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.8.8/tests/sample_data/data_humanitarian_needs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from datetime import datetime
 
 data_humanitarian_needs = [
     # total national
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
-        gender="*",
-        age_range="*",
-        disabled_marker="*",
-        sector_code="*",
-        population_group="*",
+        gender="all",
+        age_range="all",
+        disabled_marker="all",
+        sector_code="intersectoral",
+        population_group="all",
         population_status="AFF",
         population=1_000_000,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
     # national f, all ages, disabled, sector SHL
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         gender="f",
-        age_range="*",
+        age_range="all",
         disabled_marker="n",
         sector_code="SHL",
         population_group="REF",
         population_status="INN",
         population=500_000,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
@@ -45,15 +45,15 @@
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
     # admin2 ages 80+, disabled, sector HEA
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=4,
-        gender="*",
+        gender="all",
         age_range="80+",
         min_age=80,
         disabled_marker="y",
         sector_code="HEA",
         population_group="IDP",
         population_status="AFF",
         population=500,
```

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_national_risk.py` & `hapi_schema-0.8.8/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.8.8/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_patch.py` & `hapi_schema-0.8.8/tests/sample_data/data_patch.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_population.py` & `hapi_schema-0.8.8/tests/sample_data/data_population.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from datetime import datetime
 
 data_population = [
     # total national
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
-        gender="*",
-        age_range="*",
+        gender="all",
+        age_range="all",
         population=1_000_000,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
     # national f, all ages
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=1,
         gender="f",
-        age_range="*",
+        age_range="all",
         population=500_000,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
     # admin1 f, age 0-4
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
@@ -33,15 +33,15 @@
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
     # admin2 ages 80+
     dict(
         resource_hdx_id="90deb235-1bf5-4bae-b231-3393222c2d01",
         admin2_ref=4,
-        gender="*",
+        gender="all",
         age_range="80+",
         min_age=80,
         population=500,
         reference_period_start=datetime(2023, 1, 1),
         reference_period_end=datetime(2023, 6, 30),
     ),
 ]
```

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_refugees.py` & `hapi_schema-0.8.8/tests/sample_data/data_refugees.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/tests/sample_data/data_resource.py` & `hapi_schema-0.8.8/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/.gitignore` & `hapi_schema-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/LICENSE` & `hapi_schema-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/pyproject.toml` & `hapi_schema-0.8.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.8.7/PKG-INFO` & `hapi_schema-0.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.8.7
+Version: 0.8.8
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

