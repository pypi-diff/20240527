# Comparing `tmp/compliance-checker-5.1.0.tar.gz` & `tmp/compliance_checker-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compliance-checker-5.1.0.tar", last modified: Wed May 17 22:30:11 2023, max compression
+gzip compressed data, was "compliance_checker-5.1.1.tar", last modified: Mon May 27 16:55:29 2024, max compression
```

## Comparing `compliance-checker-5.1.0.tar` & `compliance_checker-5.1.1.tar`

### file list

```diff
@@ -1,231 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.055334 compliance-checker-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.055334 compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-checker-ugrid-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-glider-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-sgrid-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/cc-plugin-ugrid-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/default-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/deploy-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23513 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    11641 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/cchecker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/compliance_checker/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30003 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/acdd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19822 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.063334 compliance-checker-5.1.0/compliance_checker/cf/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_c.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_d.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_e.py
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/appendix_f.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf.py
--rw-r--r--   0 runner    (1001) docker     (123)   156976 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_6.py
--rw-r--r--   0 runner    (1001) docker     (123)    38843 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_7.py
--rw-r--r--   0 runner    (1001) docker     (123)    29294 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_8.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_1_9.py
--rw-r--r--   0 runner    (1001) docker     (123)    54398 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/cf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cf/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    61097 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/cfutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/data/
--rw-r--r--   0 runner    (1001) docker     (123)  3942260 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/seanames.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/data/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/templates/ccheck.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/data/templates/ccheck_wrapper.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)    71588 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/ioos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.067334 compliance-checker-5.1.0/compliance_checker/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/cdl.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/erddap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/netcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/protocols/opendap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    38029 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.071334 compliance-checker-5.1.0/compliance_checker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.071334 compliance-checker-5.1.0/compliance_checker/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/cassettes/test_erddap.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/cassettes/test_netcdf_content_type.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.083334 compliance-checker-5.1.0/compliance_checker/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2d-regular-grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2d-static-grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/2dim-grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/3d-regular-grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/3d-static-grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/point.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-single.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.nc
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.nc
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.nc
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.nc
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    13207 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    23864 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.nc
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_reference.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_reference.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.nc
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.nc
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cell_measure.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cf_example_cell_measures.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/chap2.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/climatology.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/cont_ragged.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/conv_bad.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/conv_multi.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/coordinate_types.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/coordinates_and_metadata.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/dimension_order.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/dimensionless.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/duplicate_axis.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/example-grid.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     9070 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/3mf07.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/bio_taxa.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     9443 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/fvcom.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/glcfs.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/hycom_global.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/kibesillah.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/l01-met.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    20715 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ocos.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ooi_glider.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/pr_inundation.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    29171 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/sp041.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/swan.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/examples/ww3.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/forecast_reference.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/grid-boundaries.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/grid_mapping_coordinates.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.087334 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/
--rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/illegal-aux-coords.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/illegal-vertical.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged2.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ints64.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ioos_1_1.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/line_geometry.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/mapping.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-dim-coordinates.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-incomplete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_1.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_2.cdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad2dim.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/badname.netcdf
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/empty.file
--rw-r--r--   0 runner    (1001) docker     (123)    24004 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/self_referencing.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/time_units.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/point.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/polygon_geometry.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/profile-incomplete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/profile-orthogonal.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/reduced_horizontal_grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/rhgrid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/rotated_pole_grid.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    43335 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/scalar_coordinate_variable.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/self-referencing-var.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/string_type_variable.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/taxonomy_example.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc4_file.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.nc
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-incomplete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-station.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-station.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/timeseries.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-complete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-implied.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-incomplete.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-single.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/trajectory.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/units_check.cdl
--rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/valid_coordinates.cdl
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/data/vertical_coords.cdl
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    21272 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_acdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   159694 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cf_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6835 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30458 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_feature_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_ioos_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_ioos_sos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    10610 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/compliance_checker/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.059334 compliance-checker-5.1.0/compliance_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24320 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9359 2023-05-17 22:30:11.000000 compliance-checker-5.1.0/compliance_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-17 22:30:10.000000 compliance-checker-5.1.0/compliance_checker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/_templates/versions.html
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/compliance_checker_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 22:30:11.091334 compliance-checker-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-17 22:29:54.000000 compliance-checker-5.1.0/tox.ini
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.445393 compliance_checker-5.1.1/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       76 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.coveragerc
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.305390 compliance_checker-5.1.1/.github/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.305390 compliance_checker-5.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      677 2021-08-16 20:06:40.000000 compliance_checker-5.1.1/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      310 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.github/dependabot.yml
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.305390 compliance_checker-5.1.1/.github/workflows/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      970 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.github/workflows/cc-plugin-glider-test.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      858 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.github/workflows/cc-plugin-sgrid-test.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      964 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.github/workflows/cc-plugin-ugrid-test.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1060 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.github/workflows/codecov.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      929 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.github/workflows/default-tests.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1084 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.github/workflows/deploy-docs.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      720 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.github/workflows/integration-tests.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1142 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.github/workflows/pypi.yml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1320 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/.gitignore
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      205 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.isort.cfg
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1611 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    11357 2020-07-02 17:13:22.000000 compliance_checker-5.1.1/LICENSE
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      354 2020-06-17 16:18:59.000000 compliance_checker-5.1.1/MANIFEST.in
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    25367 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    23513 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/README.md
+-rwxrwxr-x   0 filipe    (1000) filipe    (1000)    11531 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/cchecker.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.309390 compliance_checker-5.1.1/compliance_checker/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      950 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       21 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker/_version.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    29778 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/acdd.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    19758 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/base.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.313390 compliance_checker-5.1.1/compliance_checker/cf/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      367 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/__init__.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      433 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/appendix_c.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     4813 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/appendix_d.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      590 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/appendix_e.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    24133 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/appendix_f.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1202 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/cf.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)   154726 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/cf/cf_1_6.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    36953 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/cf_1_7.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    29239 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/cf/cf_1_8.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     6724 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/cf/cf_1_9.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    53439 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/cf/cf_base.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    12029 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/cf/util.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    61080 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/cfutil.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.321390 compliance_checker-5.1.1/compliance_checker/data/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)  3942260 2020-06-11 18:41:56.000000 compliance_checker-5.1.1/compliance_checker/data/cf-standard-name-table.xml
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     3976 2020-06-11 18:41:56.000000 compliance_checker-5.1.1/compliance_checker/data/seanames.csv
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.321390 compliance_checker-5.1.1/compliance_checker/data/templates/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6273 2020-07-30 15:57:44.000000 compliance_checker-5.1.1/compliance_checker/data/templates/ccheck.html.j2
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6408 2020-06-11 18:41:56.000000 compliance_checker-5.1.1/compliance_checker/data/templates/ccheck_wrapper.html.j2
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    71140 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/ioos.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.325390 compliance_checker-5.1.1/compliance_checker/protocols/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)        0 2019-04-17 09:39:36.000000 compliance_checker-5.1.1/compliance_checker/protocols/__init__.py
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      822 2020-04-17 14:56:21.000000 compliance_checker-5.1.1/compliance_checker/protocols/cdl.py
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      218 2020-06-11 20:20:09.000000 compliance_checker-5.1.1/compliance_checker/protocols/erddap.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2488 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/protocols/netcdf.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1875 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/protocols/opendap.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    10471 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/runner.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    37901 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/suite.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.333390 compliance_checker-5.1.1/compliance_checker/tests/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2000 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/__init__.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.333390 compliance_checker-5.1.1/compliance_checker/tests/cassettes/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    16222 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/cassettes/test_erddap.yaml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    16262 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/cassettes/test_netcdf_content_type.yaml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2879 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/conftest.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.429392 compliance_checker-5.1.1/compliance_checker/tests/data/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    17408 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    76161 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      977 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2d-regular-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    14178 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2d-regular-grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      373 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2d-static-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:53.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2d-static-grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      774 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2dim-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8974 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/2dim-grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      994 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/3d-regular-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    16813 2021-11-02 19:19:53.000000 compliance_checker-5.1.1/compliance_checker/tests/data/3d-regular-grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      520 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/3d-static-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6819 2021-11-02 19:19:53.000000 compliance_checker-5.1.1/compliance_checker/tests/data/3d-static-grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7621 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    38400 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.nc
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.433393 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1274 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/point.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1996 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     2271 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1454 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1766 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-single.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      657 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad-instance.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      788 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad-instance.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      784 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad-trajectory.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      828 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad-trajectory.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      812 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure1.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      992 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure1.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      820 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure2.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      992 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure2.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      841 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cf_role.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1060 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_cf_role.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1519 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_data_type.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13207 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_data_type.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1272 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_missing_data.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    23864 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_missing_data.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      332 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_reference.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      328 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_reference.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1093 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_region.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1044 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_region.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      912 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_units.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      820 2022-01-25 23:31:09.000000 compliance_checker-5.1.1/compliance_checker/tests/data/bad_units.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      745 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/cell_measure.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10859 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/cell_measure.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      735 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/cf_example_cell_measures.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      889 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/chap2.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8686 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/chap2.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      654 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/climatology.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7213 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/climatology.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1692 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/cont_ragged.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13882 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/cont_ragged.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      434 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/conv_bad.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      674 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/conv_bad.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      351 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/conv_multi.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      590 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/conv_multi.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1256 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/coordinate_types.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6995 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/coordinate_types.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      385 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/coordinates_and_metadata.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6900 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/coordinates_and_metadata.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1125 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/dimension_order.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7468 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/dimension_order.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      491 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/dimensionless.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7799 2021-11-02 19:19:50.000000 compliance_checker-5.1.1/compliance_checker/tests/data/dimensionless.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1528 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/duplicate_axis.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13844 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/duplicate_axis.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1197 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/example-grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    18294 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/example-grid.nc
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.437393 compliance_checker-5.1.1/compliance_checker/tests/data/examples/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9070 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/3mf07.cdl
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      926 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/bio_taxa.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      829 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9443 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/fvcom.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     4416 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/glcfs.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1206 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/hycom_global.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     5779 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/kibesillah.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    12628 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/l01-met.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    20715 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/ocos.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    11614 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/ooi_glider.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    11003 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/pr_inundation.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     2642 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    29171 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/sp041.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7257 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/swan.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     3751 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1242 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/examples/ww3.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      996 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/forecast_reference.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10458 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/forecast_reference.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1229 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/grid-boundaries.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    15976 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/grid-boundaries.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1820 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/grid_mapping_coordinates.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13955 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/grid_mapping_coordinates.nc
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.437393 compliance_checker-5.1.1/compliance_checker/tests/data/http_mocks/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    17660 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10033 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      748 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/illegal-aux-coords.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7836 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/illegal-aux-coords.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      384 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/illegal-vertical.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/illegal-vertical.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    15780 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    59022 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      720 2021-08-10 19:13:32.000000 compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged2.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8181 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged2.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      434 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ints64.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6224 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ints64.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     5951 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ioos_1_1.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    30161 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ioos_1_1.nc
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1430 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/data/line_geometry.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13945 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/line_geometry.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7038 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/mapping.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000) 43008441 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/mapping.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      582 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-dim-coordinates.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8012 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-dim-coordinates.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1014 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-incomplete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8502 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-incomplete.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1000 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10231 2021-11-02 19:19:51.000000 compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-orthogonal.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     6737 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_1.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    38895 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_1.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7666 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_2.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    39212 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_2.nc
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.437393 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1318 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1224 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1616 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      843 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad2dim.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      255 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/badname.netcdf
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1308 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1318 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)        4 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/empty.file
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    24004 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/self_referencing.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      373 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/time_units.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      930 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/point.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7856 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/point.nc
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1829 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/data/polygon_geometry.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    15815 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/polygon_geometry.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1020 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/profile-incomplete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8560 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/profile-incomplete.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1010 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/profile-orthogonal.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10338 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/profile-orthogonal.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      628 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/reduced_horizontal_grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8228 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/reduced_horizontal_grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      421 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/rhgrid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7232 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/rhgrid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1362 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/rotated_pole_grid.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    13237 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/rotated_pole_grid.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    43335 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)   227687 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/ru07-20130824T170228_rt0.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      390 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/scalar_coordinate_variable.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     5522 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/scalar_coordinate_variable.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      697 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/self-referencing-var.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8224 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/self-referencing-var.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      509 2020-11-29 00:41:12.000000 compliance_checker-5.1.1/compliance_checker/tests/data/string_type_variable.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/string_type_variable.nc
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1160 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/data/taxonomy_example.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     7959 2021-12-20 16:02:35.000000 compliance_checker-5.1.1/compliance_checker/tests/data/taxonomy_example.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1033 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc4_file.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    11301 2024-05-23 13:12:46.000000 compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc4_file.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc_file.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      936 2021-11-02 19:21:26.000000 compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc_file.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1033 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-incomplete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9230 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-incomplete.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1027 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10933 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1007 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-station.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    12415 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-station.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1013 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10733 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-ortho-depth.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      974 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9788 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-ortho-time.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      968 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-station.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    11536 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-station.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      924 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8922 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/timeseries.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      832 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-complete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8673 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-complete.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      880 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-implied.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8669 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-implied.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1063 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-incomplete.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9329 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-incomplete.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1038 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    10827 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-orthogonal.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1023 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-single.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     9904 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-single.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1042 2020-06-11 19:35:10.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8796 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/trajectory.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     1346 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/units_check.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8398 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/units_check.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    14798 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/valid_coordinates.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    71451 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/valid_coordinates.nc
+-rw-r--r--   0 filipe    (1000) filipe    (1000)      797 2020-06-11 18:41:48.000000 compliance_checker-5.1.1/compliance_checker/tests/data/vertical_coords.cdl
+-rw-r--r--   0 filipe    (1000) filipe    (1000)     8192 2021-11-02 19:19:52.000000 compliance_checker-5.1.1/compliance_checker/tests/data/vertical_coords.nc
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     8746 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/helpers.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     8341 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/resources.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    21264 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_acdd.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     6756 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/test_base.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)   159717 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/test_cf.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    23224 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_cf_integration.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     6829 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/test_cli.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    30364 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_feature_detection.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    49736 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_ioos_profile.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2717 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_ioos_sos.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2076 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/compliance_checker/tests/test_protocols.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    10802 2024-05-21 18:39:39.000000 compliance_checker-5.1.1/compliance_checker/tests/test_suite.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1578 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/tests/test_util.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1470 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/compliance_checker/util.py
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/compliance_checker.egg-info/
+-rw-r--r--   0 filipe    (1000) filipe    (1000)    25367 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/PKG-INFO
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)    12734 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/SOURCES.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)        1 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/dependency_links.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      509 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/entry_points.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)        1 2024-05-27 16:55:28.000000 compliance_checker-5.1.1/compliance_checker.egg-info/not-zip-safe
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      273 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/requires.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       19 2024-05-27 16:55:29.000000 compliance_checker-5.1.1/compliance_checker.egg-info/top_level.txt
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/docs/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      623 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/Makefile
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/docs/source/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/docs/source/_templates/
+drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2024-05-27 16:55:29.441393 compliance_checker-5.1.1/docs/source/_templates/autosummary/
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      190 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/_templates/autosummary/base.rst
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1050 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/_templates/autosummary/class.rst
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     1112 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/_templates/autosummary/module.rst
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      654 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/_templates/layout.html
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      260 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/_templates/versions.html
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      423 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/compliance_checker_api.rst
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     5018 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/docs/source/conf.py
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      412 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/development.md
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     2584 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/docs/source/faq.md
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      312 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/docs/source/index.rst
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)     3472 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/pyproject.toml
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      350 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/requirements.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)       38 2024-05-27 16:55:29.445393 compliance_checker-5.1.1/setup.cfg
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      222 2024-05-21 18:09:07.000000 compliance_checker-5.1.1/test_requirements.txt
+-rw-rw-r--   0 filipe    (1000) filipe    (1000)      395 2024-05-27 16:55:05.000000 compliance_checker-5.1.1/tox.ini
```

### Comparing `compliance-checker-5.1.0/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md` & `compliance_checker-5.1.1/.github/ISSUE_TEMPLATE/compliance-checker-issue-report.md`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/.github/workflows/cc-checker-ugrid-test.yml` & `compliance_checker-5.1.1/.github/workflows/cc-plugin-ugrid-test.yml`

 * *Files 19% similar despite different names*

```diff
@@ -5,30 +5,33 @@
   push:
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Setup Env
+    - name: Install compliance-checker
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
-        && micromamba activate TEST
-        && pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
-    - name: cc-plugin-glider tests
+    - name: cc-plugin-ugrid tests
       shell: bash -l {0}
       run: >
-        micromamba activate TEST
-        && git clone https://github.com/ioos/cc-checker-ugrid.git
+        git clone https://github.com/ioos/cc-checker-ugrid.git
         && cd cc-checker-ugrid
         && micromamba install --file requirements.txt --file requirements-dev.txt --channel conda-forge
-        && pip install -e . --no-deps --force-reinstall
-        && pytest -s -rxs -v cc_plugin_ugrid
+        && python -m pip install -e . --no-deps --force-reinstall
+        && python -m pytest -s -rxs -v cc_plugin_ugrid
```

### Comparing `compliance-checker-5.1.0/.github/workflows/cc-plugin-sgrid-test.yml` & `compliance_checker-5.1.1/.github/workflows/cc-plugin-glider-test.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-name: SGRID Plugin Tests
+name: Glider Plugin Tests
 
 on:
   pull_request:
   push:
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Setup Env
+    - name: Install compliance-checker
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
-        && micromamba activate TEST
-        && pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -v -e . --no-deps --force-reinstall
 
     - name: cc-plugin-glider tests
       shell: bash -l {0}
       run: >
-        micromamba activate TEST
-        && git clone https://github.com/ioos/cc-plugin-sgrid.git
-        && cd cc-plugin-sgrid
-        && pip install -e . --no-deps --force-reinstall
-        && pytest -s -rxs -v cc_plugin_sgrid
+        git clone https://github.com/ioos/cc-plugin-glider.git
+        && cd cc-plugin-glider
+        && micromamba install --file requirements.txt --file requirements-dev.txt --channel conda-forge
+        && python -m pip install -e . --no-deps --force-reinstall
+        && python -m pytest -s -rxs -v cc_plugin_glider
```

### Comparing `compliance-checker-5.1.0/.github/workflows/cc-plugin-ugrid-test.yml` & `compliance_checker-5.1.1/.github/workflows/cc-plugin-sgrid-test.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-name: UGRID Plugin Tests
+name: SGRID Plugin Tests
 
 on:
   pull_request:
   push:
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Setup Env
+    - name: Install compliance-checker
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
-        && micromamba activate TEST
-        && pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
-    - name: cc-plugin-glider tests
+    - name: cc-plugin-sgrid tests
       shell: bash -l {0}
       run: >
-        micromamba activate TEST
-        && git clone https://github.com/ioos/cc-checker-ugrid.git
-        && cd cc-checker-ugrid
-        && micromamba install --file requirements.txt --file requirements-dev.txt --channel conda-forge
-        && pip install -e . --no-deps --force-reinstall
-        && pytest -s -rxs -v cc_plugin_ugrid
+        git clone https://github.com/ioos/cc-plugin-sgrid.git
+        && cd cc-plugin-sgrid
+        && python -m pip install -e . --no-deps --force-reinstall
+        && python -m pytest -s -rxs -v cc_plugin_sgrid
```

### Comparing `compliance-checker-5.1.0/.github/workflows/codecov.yml` & `compliance_checker-5.1.1/.github/workflows/codecov.yml`

 * *Files 17% similar despite different names*

```diff
@@ -5,35 +5,38 @@
   push:
 
 jobs:
   run:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Setup Env
+    - name: Install compliance-checker
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
-        && micromamba activate TEST
-        && pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
     - name: Run tests with coverage
       shell: bash -l {0}
       run: |
-        micromamba activate TEST
-        pytest --cov=compliance_checker --cov-report=xml compliance_checker/tests
+        python -m pytest --cov=compliance_checker --cov-report=xml compliance_checker/tests
       # pass this step even if there are individual test failures, we are
       # interested in the overall level of coverage and other checks can
       # report on test failures.
       continue-on-error: true
 
     - name: Upload to codecov
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         files: coverage.xml
```

### Comparing `compliance-checker-5.1.0/.github/workflows/deploy-docs.yml` & `compliance_checker-5.1.1/.github/workflows/deploy-docs.yml`

 * *Files 13% similar despite different names*

```diff
@@ -10,39 +10,42 @@
 
 jobs:
   build-docs:
     runs-on: ubuntu-latest
 
     steps:
     - name: checkout
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
-    - name: Setup Mamba
-      uses: mamba-org/provision-with-micromamba@v15
+    - name: Setup Micromamba
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=3 pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Build environment
+    - name: Install compliance-checker
       shell: bash -l {0}
       run: |
-        micromamba create --name TEST python=3 --file requirements.txt --file test_requirements.txt --channel conda-forge
-        micromamba activate TEST
         python -m pip install -e . --no-deps --force-reinstall
 
     - name: Build documentation
       shell: bash -l {0}
       run: |
         set -e
-        micromamba activate TEST
         pushd docs
         cp  ../README.md source/quickintro.md
         make clean html linkcheck
         popd
 
     - name: Deploy
       if: success() && github.event_name == 'release'
-      uses: peaceiris/actions-gh-pages@v3
+      uses: peaceiris/actions-gh-pages@v4
       with:
         github_token: ${{ secrets.GITHUB_TOKEN }}
         publish_dir: docs/build/html
```

### Comparing `compliance-checker-5.1.0/.github/workflows/integration-tests.yml` & `compliance_checker-5.1.1/.github/workflows/default-tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,37 @@
-name: Integration Tests
+name: Default Tests
 
 on:
   pull_request:
   push:
 
 jobs:
   run:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        os: [windows-latest, ubuntu-latest, macos-latest]
+      fail-fast: false
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
-    - name: Setup Micromamba
-      uses: mamba-org/provision-with-micromamba@v15
+    - name: Setup Micromamba ${{ matrix.python-version }}
+      uses: mamba-org/setup-micromamba@v1
       with:
-        environment-file: false
+        environment-name: TEST
+        init-shell: bash
+        create-args: >-
+          python=${{ matrix.python-version }} pip
+          --file requirements.txt
+          --file test_requirements.txt
+          --channel conda-forge
 
-    - name: Setup Env
+    - name: Install compliance-checker
       shell: bash -l {0}
-      run: >
-        micromamba create --name TEST python=3 pip --file requirements.txt --file test_requirements.txt --channel conda-forge
-        && micromamba activate TEST
-        && pip install -e . --no-deps --force-reinstall
+      run: |
+        python -m pip install -e . --no-deps --force-reinstall
 
-    - name: Integration Tests
+    - name: Default Tests
       shell: bash -l {0}
-      run: |
-        micromamba activate TEST
-        pytest -m "integration" -s -rxs -v --vcr-record=none compliance_checker
+      run: python -m pytest -s -rxs -v -k "not integration" compliance_checker
```

### Comparing `compliance-checker-5.1.0/.github/workflows/pypi.yml` & `compliance_checker-5.1.1/.github/workflows/pypi.yml`

 * *Files 11% similar despite different names*

```diff
@@ -11,25 +11,25 @@
   run:
     shell: bash
 
 jobs:
   packages:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
       with:
         # Should be enough for setuptools-scm
         fetch-depth: 100
         persist-credentials: false
 
     - name: Get tags
       run: git fetch origin 'refs/tags/*:refs/tags/*'
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.11"
 
     - name: Install build tools
       run: |
         python -m pip install --upgrade pip build twine
```

### Comparing `compliance-checker-5.1.0/.gitignore` & `compliance_checker-5.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/.pre-commit-config.yaml` & `compliance_checker-5.1.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.6.0
   hooks:
     - id: trailing-whitespace
       exclude: compliance_checker/tests/data
     - id: check-ast
     - id: debug-statements
     - id: end-of-file-fixer
       exclude: compliance_checker/tests/data
@@ -15,37 +15,37 @@
     - id: check-yaml
     - id: requirements-txt-fixer
       args:
         - requirements.txt
         - test_requirements.txt
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 24.4.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/asottile/add-trailing-comma
-  rev: v2.4.0
+  rev: v3.1.0
   hooks:
     - id: add-trailing-comma
 
 
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.267
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.3.7
   hooks:
     - id: ruff
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: 0.11.2
+  rev: 1.7.0
   hooks:
     - id: pyproject-fmt
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.4
+  rev: v2.2.6
   hooks:
     - id: codespell
       args:
         - --ignore-words-list=degreeE,degreee,varn,poit,uint,sur,herat,claus,tung,messsages
       exclude: >
           (?x)^(
               .*\.xml|
```

### Comparing `compliance-checker-5.1.0/LICENSE` & `compliance_checker-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/PKG-INFO` & `compliance_checker-5.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: compliance-checker
-Version: 5.1.0
-Summary: Checks Datasets and SOS endpoints for standards compliance
-Home-page: https://github.com/ioos/compliance-checker
-Author: Dave Foster
-Author-email: dave@axiomdatascience.com
-License: Apache License 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: ~=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # IOOS Compliance Checker
 
 [![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
 [![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
 for completeness and community standard compliance of local or remote
```

### Comparing `compliance-checker-5.1.0/README.md` & `compliance_checker-5.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,54 @@
+Metadata-Version: 2.1
+Name: compliance-checker
+Version: 5.1.1
+Summary: Checks Datasets and SOS endpoints for standards compliance
+Maintainer: Benjamin Adams, Luke Campbell, Filipe Fernandes
+Maintainer-email: Dave Foster <dave@axiomdatascience.com>
+License: Apache-2.0
+Project-URL: documentation, https://ioos.github.io/compliance-checker
+Project-URL: homepage, https://compliance.ioos.us/index.html
+Project-URL: repository, https://github.com/ioos/compliance-checker
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cf-units>=2
+Requires-Dist: cftime>=1.1.0
+Requires-Dist: importlib-metadata
+Requires-Dist: importlib-resources
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: jinja2>=2.7.3
+Requires-Dist: lxml>=3.2.1
+Requires-Dist: netcdf4>=1.6.4
+Requires-Dist: owsLib>=0.8.3
+Requires-Dist: packaging
+Requires-Dist: pendulum>=1.2.4
+Requires-Dist: pygeoif>=0.6
+Requires-Dist: pyproj>=2.2.1
+Requires-Dist: regex>=2017.07.28
+Requires-Dist: requests>=2.2.1
+Requires-Dist: setuptools>=15.0
+Requires-Dist: shapely>=1.7.1
+Requires-Dist: validators>=0.14.2
+
 # IOOS Compliance Checker
 
 [![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
 [![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
 for completeness and community standard compliance of local or remote
```

### Comparing `compliance-checker-5.1.0/cchecker.py` & `compliance_checker-5.1.1/cchecker.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,16 +249,16 @@
                 for c in check_suite.checkers
                 if ":" in c and not c.endswith(":latest")
             ]
 
         for checker_name in sorted(checker_names):
             if checker_name not in check_suite.checkers:
                 print(
-                    "Cannot find checker '{}' with which to "
-                    "describe checks".format(checker_name),
+                    f"Cannot find checker '{checker_name}' with which to "
+                    "describe checks",
                     file=sys.stderr,
                 )
                 error_stat = 1
             else:
                 _print_checker_name_header(checker_name)
                 check_suite._print_checker(check_suite.checkers[checker_name])
         sys.exit(error_stat)
@@ -289,17 +289,15 @@
     # Run the compliance checker
     # 2 modes, concatenated output file or multiple output files
     return_values = []
     had_errors = []
     if output_len == 1:
         if args.format != "json":
             print(
-                "Running Compliance Checker on the datasets from: {}".format(
-                    args.dataset_location,
-                ),
+                f"Running Compliance Checker on the datasets from: {args.dataset_location}",
                 file=sys.stderr,
             )
         return_value, errors = ComplianceChecker.run_checker(
             args.dataset_location,
             args.test or ["acdd"],
             args.verbose,
             args.criteria,
@@ -311,17 +309,15 @@
         )
         return_values.append(return_value)
         had_errors.append(errors)
     else:
         for output, dataset in zip(args.output, args.dataset_location):
             if args.format != "json":
                 print(
-                    "Running Compliance Checker on the dataset from: {}".format(
-                        dataset,
-                    ),
+                    f"Running Compliance Checker on the dataset from: {dataset}",
                     file=sys.stderr,
                 )
             return_value, errors = ComplianceChecker.run_checker(
                 [dataset],
                 args.test or ["acdd"],
                 args.verbose,
                 args.criteria,
```

### Comparing `compliance-checker-5.1.0/compliance_checker/acdd.py` & `compliance_checker-5.1.1/compliance_checker/acdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,22 +245,22 @@
             lat_max = float(ds.geospatial_lat_max)
         except ValueError:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lat_extents_match",
                 [
-                    "Could not convert one of geospatial_lat_min ({}) or max ({}) to float see CF-1.6 spec chapter 4.1"
-                    "".format(ds.geospatial_lat_min, ds.geospatial_lat_max),
+                    f"Could not convert one of geospatial_lat_min ({ds.geospatial_lat_min}) or max ({ds.geospatial_lat_max}) to float see CF-1.6 spec chapter 4.1"
+                    "",
                 ],
             )
 
         # identify lat var(s) as per CF 4.1
         lat_vars = {}  # var -> number of criteria passed
-        for _name, var in ds.variables.items():
+        for var in ds.variables.values():
             # must have units
             if not hasattr(var, "units"):
                 continue
 
             lat_vars[var] = 0
 
             # units in this set
@@ -343,22 +343,22 @@
             lon_max = float(ds.geospatial_lon_max)
         except ValueError:
             return Result(
                 BaseCheck.MEDIUM,
                 False,
                 "geospatial_lon_extents_match",
                 [
-                    "Could not convert one of geospatial_lon_min ({}) or max ({}) to float see CF-1.6 spec chapter 4.1"
-                    "".format(ds.geospatial_lon_min, ds.geospatial_lon_max),
+                    f"Could not convert one of geospatial_lon_min ({ds.geospatial_lon_min}) or max ({ds.geospatial_lon_max}) to float see CF-1.6 spec chapter 4.1"
+                    "",
                 ],
             )
 
         # identify lon var(s) as per CF 4.2
         lon_vars = {}  # var -> number of criteria passed
-        for _name, var in ds.variables.items():
+        for var in ds.variables.values():
             # must have units
             if not hasattr(var, "units"):
                 continue
 
             lon_vars[var] = 0
 
             # units in this set
@@ -436,15 +436,15 @@
         except AttributeError:
             return ratable_result(
                 False,
                 "Global Attributes",  # grouped with Globals
                 [
                     (
                         "Could not parse WKT from geospatial_bounds,"
-                        ' possible bad value: "{}"'.format(ds.geospatial_bounds)
+                        f' possible bad value: "{ds.geospatial_bounds}"'
                     ),
                 ],
                 variable_name="geospatial_bounds",
             )
         # parsed OK
         else:
             return ratable_result(True, "Global Attributes", ())
@@ -633,27 +633,21 @@
         end_dt = abs(time1 - t_max)
 
         score = 2
         msgs = []
         if start_dt > timedelta(hours=1):
             msgs.append(
                 "Date time mismatch between time_coverage_start and actual "
-                "time values {} (time_coverage_start) != {} (time[0])".format(
-                    t_min.isoformat(),
-                    time0.isoformat(),
-                ),
+                f"time values {t_min.isoformat()} (time_coverage_start) != {time0.isoformat()} (time[0])",
             )
             score -= 1
         if end_dt > timedelta(hours=1):
             msgs.append(
                 "Date time mismatch between time_coverage_end and actual "
-                "time values {} (time_coverage_end) != {} (time[N])".format(
-                    t_max.isoformat(),
-                    time1.isoformat(),
-                ),
+                f"time values {t_max.isoformat()} (time_coverage_end) != {time1.isoformat()} (time[N])",
             )
             score -= 1
 
         return Result(BaseCheck.MEDIUM, (score, 2), "time_coverage_extents_match", msgs)
 
     def verify_convention_version(self, ds):
         """
@@ -672,17 +666,15 @@
 
             # if no/wrong ACDD convention, return appropriate result
             # Result will have name "Global Attributes" to group with globals
             m = [f"Conventions does not contain 'ACDD-{self._cc_spec_version}'"]
             return ratable_result((1, 2), "Global Attributes", m)
         except AttributeError:  # NetCDF attribute not found
             m = [
-                "No Conventions attribute present; must contain ACDD-{}".format(
-                    self._cc_spec_version,
-                ),
+                f"No Conventions attribute present; must contain ACDD-{self._cc_spec_version}",
             ]
             # Result will have name "Global Attributes" to group with globals
             return ratable_result((0, 2), "Global Attributes", m)
 
 
 class ACDDNCCheck(BaseNCCheck, ACDDBaseCheck):
     pass
```

### Comparing `compliance-checker-5.1.0/compliance_checker/base.py` & `compliance_checker-5.1.1/compliance_checker/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lxml import etree
 from netCDF4 import Dataset
 from owslib.namespaces import Namespaces
 from owslib.swe.observation.sos100 import SensorObservationService_1_0_0
 from owslib.swe.sensor.sml import SensorML
 
 import compliance_checker.cfutil as cfutil
-from compliance_checker import MemoizedDataset, __version__
+from compliance_checker import __version__
 from compliance_checker.util import kvp_convert
 
 # Python 3.5+ should work, also have a fallback
 try:
     from typing import Pattern
 
     re_pattern_type = Pattern
@@ -188,24 +188,25 @@
     def __del__(self):
         """
         Finalizer. Ensure any caches shared by multiple checkers
         are cleared before the next checker uses it. Some caches were
         inadvertently mutated by other functions.
         """
 
-        cfutil.get_geophysical_variables.cache_clear()
-        cfutil.get_time_variables.cache_clear()
+        if cfutil is not None:
+            cfutil.get_geophysical_variables.cache_clear()
+            cfutil.get_time_variables.cache_clear()
 
 
 class BaseNCCheck:
     """
     Base Class for NetCDF Dataset supporting Check Suites.
     """
 
-    supported_ds = {Dataset, MemoizedDataset}
+    supported_ds = [Dataset]
 
     @classmethod
     def std_check_in(cls, dataset, name, allowed_vals):
         """
         Returns 0 if attr not present, 1 if present but not in correct value, 2 if good
         """
         if name not in dataset.ncattrs():
@@ -476,18 +477,15 @@
         # redundant, we could easily do this with a hasattr
         # check instead
         res = std_check_in(base_context, name, other)
         if res == 0:
             msgs.append(f"{display_name} not present")
         elif res == 1:
             msgs.append(
-                "{} present, but not in expected value list ({})".format(
-                    display_name,
-                    sorted(other),
-                ),
+                f"{display_name} present, but not in expected value list ({sorted(other)})",
             )
 
         ret_val.append(
             Result(
                 priority,
                 (res, 2),
                 gname if gname else name,  # groups Globals if supplied
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/appendix_d.py` & `compliance_checker-5.1.1/compliance_checker/cf/appendix_d.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/appendix_e.py` & `compliance_checker-5.1.1/compliance_checker/cf/appendix_e.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/appendix_f.py` & `compliance_checker-5.1.1/compliance_checker/cf/appendix_f.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf_1_6.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf_1_6.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,15 @@
         for k, v in ds.variables.items():
             if (
                 v.dtype is not str
                 and v.dtype.kind != "S"
                 and v.dtype.type not in self._allowed_numeric_var_types
             ):
                 fails.append(
-                    "The variable {} failed because the datatype is {}".format(
-                        k,
-                        v.datatype,
-                    ),
+                    f"The variable {k} failed because the datatype is {v.datatype}",
                 )
         return Result(
             BaseCheck.HIGH,
             (total - len(fails), total),
             self.section_titles["2.2"],
             msgs=fails,
         )
@@ -105,15 +102,15 @@
         For any variables which contain any of the following attributes:
             - valid_min/valid_max
             - valid_range
             - scale_factor
             - add_offset
             - _FillValue
         the data type of the attribute must match the type of its parent variable as specified in the
-        NetCDF User Guide (NUG) https://www.unidata.ucar.edu/software/netcdf/docs/attribute_conventions.html,
+        NetCDF User Guide (NUG) https://docs.unidata.ucar.edu/netcdf-c/current/attribute_conventions.html,
         referenced in the CF Conventions in Section 2.5.2
         (http://cfconventions.org/Data/cf-conventions/cf-conventions-1.7/cf-conventions.html#missing-data)
 
         :param netCDF4.Dataset ds: open netCDF dataset object
         :rtype: compliance_checker.base.Result
         """
 
@@ -237,54 +234,54 @@
 
         rname = regex.compile("^[A-Za-z][A-Za-z0-9_]*$")
 
         # IMPLEMENTATION CONFORMANCE 2.3 REQUIRED
         for name, variable in ds.variables.items():
             variable_naming.assert_true(
                 rname.match(name) is not None,
-                "variable {} should begin with a letter and be composed of "
-                "letters, digits, and underscores".format(name),
+                f"variable {name} should begin with a letter and be composed of "
+                "letters, digits, and underscores",
             )
 
             # Keep track of all the attributes, we'll need to check them
             for attr in variable.ncattrs():
                 if attr in ignore_attributes:
                     continue
                 # Special attributes made by THREDDS
                 if attr.startswith("DODS"):
                     continue
                 # Ignore model produced attributes
                 if attr.startswith("_Coordinate"):
                     continue
                 attribute_naming.assert_true(
                     rname.match(attr) is not None,
-                    "attribute {}:{} should begin with a letter and be composed of "
-                    "letters, digits, and underscores".format(name, attr),
+                    f"attribute {name}:{attr} should begin with a letter and be composed of "
+                    "letters, digits, and underscores",
                 )
 
         ret_val.append(variable_naming.to_result())
 
         for dimension in ds.dimensions:
             dimension_naming.assert_true(
                 rname.match(dimension) is not None,
-                "dimension {} should begin with a latter and be composed of "
-                "letters, digits, and underscores".format(dimension),
+                f"dimension {dimension} should begin with a latter and be composed of "
+                "letters, digits, and underscores",
             )
         ret_val.append(dimension_naming.to_result())
 
         for global_attr in ds.ncattrs():
             # Special attributes made by THREDDS
             if global_attr.startswith("DODS"):
                 continue
             if global_attr.startswith("EXTRA_DIMENSION"):
                 continue
             attribute_naming.assert_true(
                 rname.match(global_attr) is not None,
-                "global attribute {} should begin with a letter and be composed of "
-                "letters, digits, and underscores".format(global_attr),
+                f"global attribute {global_attr} should begin with a letter and be composed of "
+                "letters, digits, and underscores",
             )
         ret_val.append(attribute_naming.to_result())
 
         return ret_val
 
     def check_names_unique(self, ds):
         """
@@ -412,61 +409,60 @@
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of Results
         """
         fails = []
         total = 0
 
-        for _name, variable in ds.variables.items():
+        for variable in ds.variables.values():
             # If the variable have a defined _FillValue a defined missing_value check it.
 
             if hasattr(variable, "_FillValue") and hasattr(variable, "missing_value"):
                 total = total + 1
                 if variable._FillValue != variable.missing_value:
                     fails.append(
-                        "For the variable {} the missing_value must be equal to the _FillValue".format(
-                            variable.name,
-                        ),
+                        f"For the variable {variable.name} the missing_value must be equal to the _FillValue",
                     )
 
         return Result(
             BaseCheck.MEDIUM,
-            (len(fails), total),
+            (total - len(fails), total),
             self.section_titles["2.5"],
             msgs=fails,
         )
 
-    def check_valid_range_or_valid_min_max_present(self, ds):
+    def check_valid_range_and_valid_min_max_present(self, ds):
         """
         The valid_range attribute must not be present if the valid_min
         and/or valid_max attributes are present. This according to 2.5.1 Requirements.
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: list
         :return: List of Results
         """
         fails = []
         total = 0
 
-        for _name, variable in ds.variables.items():
-            if hasattr(variable, "valid_max") and (
-                hasattr(variable, "valid_min") or hasattr(variable, "valid_range")
-            ):
-                total = total + 1
-
-                fails.append(
-                    "For the variable {} the valid_range attribute must not be present "
-                    "if the valid_min and/or valid_max attributes are present".format(
-                        variable.name,
-                    ),
-                )
+        for variable in ds.variables.values():
+            if hasattr(variable, "valid_max") or hasattr(variable, "valid_min"):
+                total += 1
+                # if there's also valid_range in addition to
+                # valid_min/valid_max, this is not compliant
+                if hasattr(variable, "valid_range"):
+                    fails.append(
+                        f"For the variable {variable.name} the valid_range attribute must not be present "
+                        "if the valid_min and/or valid_max attributes are present",
+                    )
+            # *Just* valid_range should be added to total as well
+            elif hasattr(variable, "valid_range"):
+                total += 1
 
         return Result(
             BaseCheck.MEDIUM,
-            (len(fails), total),
+            (total - len(fails), total),
             self.section_titles["2.5"],
             msgs=fails,
         )
 
     def check_fill_value_outside_valid_range(self, ds):
         """
         Checks each variable's _FillValue to ensure that it's in valid_range or
@@ -492,18 +488,15 @@
             attrs = variable.ncattrs()
 
             if "valid_range" in attrs:
                 if isinstance(variable.valid_range, str):
                     m = "§2.5.1 Fill Values should be outside the range specified by valid_range"  # subsection message
                     valid_fill_range.assert_true(
                         False,
-                        "{};\n\t{}:valid_range must be a numeric type not a string".format(
-                            m,
-                            name,
-                        ),
+                        f"{m};\n\t{name}:valid_range must be a numeric type not a string",
                     )
                     continue
                 rmin, rmax = variable.valid_range
                 spec_by = "valid_range"
 
             elif "valid_min" in attrs and "valid_max" in attrs:
                 if isinstance(variable.valid_min, str):
@@ -530,16 +523,16 @@
             if np.isnan(fill_value):
                 valid = True
             else:
                 valid = fill_value < rmin or fill_value > rmax
 
             valid_fill_range.assert_true(
                 valid,
-                "{}:_FillValue ({}) should be outside the range specified by {} ({}, {})"
-                "".format(name, fill_value, spec_by, rmin, rmax),
+                f"{name}:_FillValue ({fill_value}) should be outside the range specified by {spec_by} ({rmin}, {rmax})"
+                "",
             )
 
         return valid_fill_range.to_result()
 
     def check_convention_globals(self, ds):
         """
         Check the common global attributes are strings if they exist.
@@ -556,16 +549,16 @@
         valid_globals = TestCtx(BaseCheck.MEDIUM, self.section_titles["2.6"])
 
         for attr in attrs:
             dataset_attr = getattr(ds, attr, None)
             is_string = isinstance(dataset_attr, str)
             valid_globals.assert_true(
                 is_string and len(dataset_attr),
-                "§2.6.2 global attribute {} should exist and be a non-empty string"  # subsection message
-                "".format(attr),
+                f"§2.6.2 global attribute {attr} should exist and be a non-empty string"  # subsection message
+                "",
             )
         return valid_globals.to_result()
 
     # IMPLEMENTATION
     def check_coordinate_variables_strict_monotonicity(self, ds):
         """
         Checks that data in coordinate variables is either monotonically
@@ -610,28 +603,27 @@
         for name, variable in ds.variables.items():
             for attribute in variable.ncattrs():
                 varattr = getattr(variable, attribute)
                 if attribute in attrs:
                     is_string = isinstance(varattr, str)
                     valid_attributes.assert_true(
                         is_string and len(varattr) > 0,
-                        "§2.6.2 {}:{} should be a non-empty string"
-                        "".format(name, attribute),
+                        f"§2.6.2 {name}:{attribute} should be a non-empty string" "",
                     )
                     attr_bin.add(attribute)
 
         # Check all the global attributes too and mark if we've seen them
         for attribute in ds.ncattrs():
             dsattr = getattr(ds, attribute)
             if attribute in attrs:
                 is_string = isinstance(dsattr, str)
                 valid_attributes.assert_true(
                     is_string and len(dsattr) > 0,
-                    "§2.6.2 {} global attribute should be a non-empty string"
-                    "".format(attribute),
+                    f"§2.6.2 {attribute} global attribute should be a non-empty string"
+                    "",
                 )
                 attr_bin.add(attribute)
         return valid_attributes.to_result()
 
     ###############################################################################
     # Chapter 3: Description of the Data
     ###############################################################################
@@ -716,18 +708,15 @@
             ret_val.append(valid_units)
 
             units_attr_is_string = TestCtx(BaseCheck.MEDIUM, self.section_titles["3.1"])
 
             # side effects, but better than teasing out the individual result
             if units is not None and units_attr_is_string.assert_true(
                 isinstance(units, str),
-                "units ({}) attribute of '{}' must be a string compatible with UDUNITS".format(
-                    units,
-                    variable.name,
-                ),
+                f"units ({units}) attribute of '{variable.name}' must be a string compatible with UDUNITS",
             ):
                 valid_udunits = self._check_valid_udunits(ds, name)
                 ret_val.append(valid_udunits)
             ret_val.append(units_attr_is_string.to_result())
 
             if isinstance(standard_name, str):
                 # CONFORMANCE 3.1 REQUIRED
@@ -804,17 +793,15 @@
             or std_name_units_dimensionless
             or standard_name is None
         )
 
         # 1) Units must exist
         valid_units.assert_true(
             should_be_dimensionless or units is not None,
-            "units attribute is required for {} when variable is not a dimensionless quantity".format(
-                variable_name,
-            ),
+            f"units attribute is required for {variable_name} when variable is not a dimensionless quantity",
         )
 
         # Don't bother checking the rest
         if units is None and not should_be_dimensionless:
             return valid_units.to_result()
         # 2) units attribute must be a string
         valid_units.assert_true(
@@ -871,18 +858,15 @@
             or std_name_units_dimensionless
         )
 
         valid_udunits = TestCtx(BaseCheck.HIGH, self.section_titles["3.1"])
         are_udunits = units is not None and util.units_known(units)
         valid_udunits.assert_true(
             should_be_dimensionless or are_udunits or units is None,
-            'units for {}, "{}" are not recognized by UDUNITS'.format(
-                variable_name,
-                units,
-            ),
+            f'units for {variable_name}, "{units}" are not recognized by UDUNITS',
         )
         return valid_udunits.to_result()
 
     def _check_valid_standard_units(self, ds, variable_name):
         """
         Checks that the variable's units are appropriate for the standard name
         according to the CF standard name table and coordinate sections in CF
@@ -938,36 +922,36 @@
         # UDUnits accepts "s" as a unit of time but it should be <unit> since <epoch>
         # TODO: forecast_reference_time.  Include upcoming merge.
         # IMPLEMENTATION CONFORMANCE 4.4 REQUIRED 1/2
         elif standard_name == "time":
             valid_standard_units.assert_true(
                 util.units_convertible(units, "seconds since 1970-01-01"),
                 "time must be in a valid units format <unit> since <epoch> "
-                "not {}".format(units),
+                f"not {units}",
             )
 
         # UDunits can't tell the difference between east and north facing coordinates
         elif standard_name == "latitude":
             # degrees is allowed if using a transformed grid
             allowed_units = cfutil.VALID_LAT_UNITS | {"degrees"}
             valid_standard_units.assert_true(
                 (units.lower() if units is not None else None) in allowed_units,
-                'variables defining latitude ("{}") must use degrees_north '
+                f'variables defining latitude ("{variable_name}") must use degrees_north '
                 "or degrees if defining a transformed grid. Currently "
-                "{}".format(variable_name, units),
+                f"{units}",
             )
         # UDunits can't tell the difference between east and north facing coordinates
         elif standard_name == "longitude":
             # degrees is allowed if using a transformed grid
             allowed_units = cfutil.VALID_LON_UNITS | {"degrees"}
             valid_standard_units.assert_true(
                 (units.lower() if units is not None else None) in allowed_units,
-                'variables defining longitude ("{}") must use degrees_east '
+                f'variables defining longitude ("{variable_name}") must use degrees_east '
                 "or degrees if defining a transformed grid. Currently "
-                "{}".format(variable_name, units),
+                f"{units}",
             )
 
         return valid_standard_units.to_result()
 
     def check_standard_name(self, ds):
         """
         Check a variables's standard_name attribute to ensure that it meets CF
@@ -1035,17 +1019,15 @@
             # the check for this variable
             # IMPLEMENTATION CONFORMANCE 3.3 REQUIRED 1, 2, 3 / 3
             if standard_name is not None:
                 standard_name_present = True
                 valid_std_name = TestCtx(BaseCheck.HIGH, self.section_titles["3.3"])
                 valid_std_name.assert_true(
                     isinstance(standard_name, str),
-                    "Attribute standard_name for variable {} must be a string".format(
-                        name,
-                    ),
+                    f"Attribute standard_name for variable {name} must be a string",
                 )
                 valid_std_name.out_of += 1
                 if standard_name not in self._std_names:
                     err_msg = "standard_name {} is not defined in Standard Name Table v{}.".format(
                         standard_name or "undefined",
                         self._std_names._version,
                     )
@@ -1062,31 +1044,26 @@
                 ret_val.append(valid_std_name.to_result())
 
                 # 2) optional - if modifiers, should be in table
                 if standard_name_modifier is not None:
                     valid_modifier = TestCtx(BaseCheck.HIGH, self.section_titles["3.3"])
                     valid_modifier.assert_true(
                         standard_name_modifier in valid_modifiers,
-                        'Standard name modifier "{}" for variable {} is not a valid modifier '
-                        "according to CF Appendix C".format(
-                            standard_name_modifier,
-                            name,
-                        ),
+                        f'Standard name modifier "{standard_name_modifier}" for variable {name} is not a valid modifier '
+                        "according to CF Appendix C",
                     )
 
                     ret_val.append(valid_modifier.to_result())
             else:
                 standard_name_present = False
 
             # IMPLEMENTATION CONFORMANCE 3 RECOMMENDED
             long_or_std_name.assert_true(
                 long_name_present or standard_name_present,
-                "Attribute long_name or/and standard_name is highly recommended for variable {}".format(
-                    name,
-                ),
+                f"Attribute long_name or/and standard_name is highly recommended for variable {name}",
             )
             ret_val.append(long_or_std_name.to_result())
         return ret_val
 
     def check_ancillary_variables(self, ds):
         """
         Checks the ancillary_variable attribute for all variables to ensure
@@ -1111,16 +1088,15 @@
         ):
             name = ncvar.name
             valid_ancillary = TestCtx(BaseCheck.HIGH, self.section_titles["3.4"])
             ancillary_variables = ncvar.ancillary_variables
 
             valid_ancillary.assert_true(
                 isinstance(ancillary_variables, str),
-                "ancillary_variables attribute defined by {} "
-                "should be string".format(name),
+                f"ancillary_variables attribute defined by {name} " "should be string",
             )
 
             # Can't perform the second check if it's not a string
             if not isinstance(ancillary_variables, str):
                 ret_val.append(valid_ancillary.to_result())
                 continue
 
@@ -1205,17 +1181,15 @@
                     allv = False
                 else:
                     allv = np.all(vals_arr & masks_arr == vals_arr)
 
                 allvr = Result(BaseCheck.MEDIUM, allv, self.section_titles["3.5"])
                 if not allvr.value:
                     allvr.msgs = [
-                        "flag masks and flag values for '{}' combined don't equal flag values".format(
-                            name,
-                        ),
+                        f"flag masks and flag values for '{name}' combined don't equal flag values",
                     ]
 
                 ret_val.append(allvr)
 
         return ret_val
 
     def _check_flag_values(self, ds, name):
@@ -1251,16 +1225,16 @@
             f"{name}'s flag_values must be independent and can not be repeated",
         )
 
         # IMPLEMENTATION CONFORMANCE 3.5 REQUIRED 1/8
         # the data type for flag_values should be the same as the variable
         valid_values.assert_true(
             variable.dtype.type == flag_values.dtype.type,
-            "flag_values ({}) must be the same data type as {} ({})"
-            "".format(flag_values.dtype.type, name, variable.dtype.type),
+            f"flag_values ({flag_values.dtype.type}) must be the same data type as {name} ({variable.dtype.type})"
+            "",
         )
 
         # IMPLEMENTATION CONFORMANCE 3.5 REQUIRED 4/8
         if isinstance(flag_meanings, str):
             flag_meanings = flag_meanings.split()
             valid_values.assert_true(
                 len(flag_meanings) == np.array(flag_values).size,
@@ -1288,16 +1262,16 @@
         flag_masks = variable.flag_masks
         flag_meanings = getattr(variable, "flag_meanings", None)
 
         valid_masks = TestCtx(BaseCheck.HIGH, self.section_titles["3.5"])
 
         valid_masks.assert_true(
             variable.dtype.type == flag_masks.dtype.type,
-            "flag_masks ({}) must be the same data type as {} ({})"
-            "".format(flag_masks.dtype.type, name, variable.dtype.type),
+            f"flag_masks ({flag_masks.dtype.type}) must be the same data type as {name} ({variable.dtype.type})"
+            "",
         )
 
         type_ok = (
             np.issubdtype(variable.dtype, np.integer)
             or np.issubdtype(variable.dtype, "S")
             or np.issubdtype(variable.dtype, "b")
         )
@@ -1363,17 +1337,15 @@
         # IMPLEMENTATION CONFORMANCE REQUIRED 3.5 3/8
         flag_regx = regex.compile(r"^[0-9A-Za-z_\-.+@]+$")
         meanings = flag_meanings.split()
         for meaning in meanings:
             if flag_regx.match(meaning) is None:
                 valid_meanings.assert_true(
                     False,
-                    "{}'s flag_meanings attribute defined an illegal flag meaning ".format(
-                        name,
-                    )
+                    f"{name}'s flag_meanings attribute defined an illegal flag meaning "
                     + f"{meaning}",
                 )
         return valid_meanings.to_result()
 
     ###############################################################################
     # Chapter 4: Coordinate Types
     ###############################################################################
@@ -1517,48 +1489,48 @@
             allowed_units = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.1"])
             if standard_name == "grid_latitude":
                 e_n_units = cfutil.VALID_LAT_UNITS | cfutil.VALID_LON_UNITS
                 # check that the units aren't in east and north degrees units,
                 # but are convertible to angular units
                 allowed_units.assert_true(
                     units not in e_n_units and Unit(units) == Unit("degree"),
-                    "Grid latitude variable '{}' should use degree equivalent units without east or north components. "
-                    "Current units are {}".format(latitude, units),
+                    f"Grid latitude variable '{latitude}' should use degree equivalent units without east or north components. "
+                    f"Current units are {units}",
                 )
             else:
                 allowed_units.assert_true(
                     units_is_string and units.lower() in allowed_lat_units,
-                    "latitude variable '{}' should define valid units for latitude"
-                    "".format(latitude),
+                    f"latitude variable '{latitude}' should define valid units for latitude"
+                    "",
                 )
             ret_val.append(allowed_units.to_result())
 
             # Check that latitude uses degrees_north
             if standard_name == "latitude" and units != "degrees_north":
                 # This is only a recommendation and we won't penalize but we
                 # will include a recommended action.
                 msg = (
-                    "CF recommends latitude variable '{}' to use units degrees_north"
-                    "".format(latitude)
+                    f"CF recommends latitude variable '{latitude}' to use units degrees_north"
+                    ""
                 )
                 recommended_units = Result(
                     BaseCheck.LOW,
                     (1, 1),
                     self.section_titles["4.1"],
                     [msg],
                 )
                 ret_val.append(recommended_units)
 
             y_variables = ds.get_variables_by_attributes(axis="Y")
             # Check that latitude defines either standard_name or axis
             definition = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.1"])
             definition.assert_true(
                 standard_name == "latitude" or axis == "Y" or y_variables != [],
-                "latitude variable '{}' should define standard_name='latitude' or axis='Y'"
-                "".format(latitude),
+                f"latitude variable '{latitude}' should define standard_name='latitude' or axis='Y'"
+                "",
             )
             ret_val.append(definition.to_result())
 
         return ret_val
 
     def check_longitude(self, ds):
         """
@@ -1626,48 +1598,48 @@
             allowed_units = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.2"])
             if standard_name == "grid_longitude":
                 e_n_units = cfutil.VALID_LAT_UNITS | cfutil.VALID_LON_UNITS
                 # check that the units aren't in east and north degrees units,
                 # but are convertible to angular units
                 allowed_units.assert_true(
                     units not in e_n_units and Unit(units) == Unit("degree"),
-                    "Grid longitude variable '{}' should use degree equivalent units without east or north components. "
-                    "Current units are {}".format(longitude, units),
+                    f"Grid longitude variable '{longitude}' should use degree equivalent units without east or north components. "
+                    f"Current units are {units}",
                 )
             else:
                 allowed_units.assert_true(
                     units_is_string and units.lower() in allowed_lon_units,
-                    "longitude variable '{}' should define valid units for longitude"
-                    "".format(longitude),
+                    f"longitude variable '{longitude}' should define valid units for longitude"
+                    "",
                 )
             ret_val.append(allowed_units.to_result())
 
             # Check that longitude uses degrees_east
             if standard_name == "longitude" and units != "degrees_east":
                 # This is only a recommendation and we won't penalize but we
                 # will include a recommended action.
                 msg = (
-                    "CF recommends longitude variable '{}' to use units degrees_east"
-                    "".format(longitude)
+                    f"CF recommends longitude variable '{longitude}' to use units degrees_east"
+                    ""
                 )
                 recommended_units = Result(
                     BaseCheck.LOW,
                     (1, 1),
                     self.section_titles["4.2"],
                     [msg],
                 )
                 ret_val.append(recommended_units)
 
             x_variables = ds.get_variables_by_attributes(axis="X")
             # Check that longitude defines either standard_name or axis
             definition = TestCtx(BaseCheck.MEDIUM, self.section_titles["4.2"])
             definition.assert_true(
                 standard_name == "longitude" or axis == "X" or x_variables != [],
-                "longitude variable '{}' should define standard_name='longitude' or axis='X'"
-                "".format(longitude),
+                f"longitude variable '{longitude}' should define standard_name='longitude' or axis='X'"
+                "",
             )
             ret_val.append(definition.to_result())
 
         return ret_val
 
     def check_dimensional_vertical_coordinate(
         self,
@@ -1713,23 +1685,23 @@
                 or standard_name in dimless_vertical_coordinates
             ):
                 continue
 
             valid_vertical_coord = TestCtx(BaseCheck.HIGH, self.section_titles["4.3"])
             valid_vertical_coord.assert_true(
                 isinstance(units, str) and units,
-                "§4.3.1 {}'s units must be defined for vertical coordinates, "
-                "there is no default".format(name),
+                f"§4.3.1 {name}'s units must be defined for vertical coordinates, "
+                "there is no default",
             )
 
             if not util.units_convertible("bar", units):
                 valid_vertical_coord.assert_true(
                     positive in ("up", "down"),
-                    "{}: vertical coordinates not defining pressure must include "
-                    "a positive attribute that is either 'up' or 'down'".format(name),
+                    f"{name}: vertical coordinates not defining pressure must include "
+                    "a positive attribute that is either 'up' or 'down'",
                 )
 
             # _check_valid_standard_units, part of the Chapter 3 checks,
             # already verifies that this coordinate has valid units
 
             ret_val.append(valid_vertical_coord.to_result())
 
@@ -1760,16 +1732,15 @@
         if formula_terms is None and standard_name not in dim_vert_coords_dict:
             return
 
         is_not_deprecated = TestCtx(BaseCheck.LOW, self.section_titles["4.3"])
 
         is_not_deprecated.assert_true(
             units not in deprecated_units,
-            "§4.3.2: units are deprecated by CF in variable {}: {}"
-            "".format(vname, units),
+            f"§4.3.2: units are deprecated by CF in variable {vname}: {units}" "",
         )
 
         # check the vertical coordinates
         ret_val.append(is_not_deprecated.to_result())
         ret_val.append(self._check_formula_terms(ds, vname, dim_vert_coords_dict))
 
     def check_dimensionless_vertical_coordinates(self, ds):
@@ -2054,15 +2025,15 @@
                 result = Result(BaseCheck.LOW, True, self.section_titles["4.4.1"])
             ret_val.append(result)
 
         return ret_val
 
     def _check_leap_time(self, time_variable):
         """
-        Helper method to handle checking custom calendar leap time specifiations
+        Helper method to handle checking custom calendar leap time specifications
         """
         leap_time = TestCtx(BaseCheck.HIGH, self.section_titles["4.4"])
         leap_time.out_of = 1
         # IMPLEMENTATION CONFORMANCE 4.4.1 REQUIRED 2, 3 / 5
         if not hasattr(time_variable, "month_lengths") or not (
             hasattr(time_variable.month_lengths, "dtype")
             and np.issubdtype(time_variable.month_lengths.dtype, np.integer)
@@ -2164,17 +2135,17 @@
                 continue
 
             valid_aux_coords = TestCtx(BaseCheck.HIGH, self.section_titles["5"])
 
             for aux_coord in coordinates.split():
                 valid_aux_coords.assert_true(
                     aux_coord in ds.variables,
-                    "{}'s auxiliary coordinate specified by the coordinates attribute, {}, "
+                    f"{name}'s auxiliary coordinate specified by the coordinates attribute, {aux_coord}, "
                     "is not a variable in this dataset"
-                    "".format(name, aux_coord),
+                    "",
                 )
                 if aux_coord not in ds.variables:
                     continue
 
                 # TODO CONFORMANCE: Partial implementation of labels
                 # §6.1 Allows for "labels" to be referenced as coordinates
                 if (
@@ -2266,15 +2237,15 @@
             variable = ds.variables[coord]
             if variable.ndim < 2:
                 continue
             not_matching = TestCtx(BaseCheck.MEDIUM, self.section_titles["5"])
 
             not_matching.assert_true(
                 coord not in variable.dimensions,
-                "{} shares the same name as one of its dimensions" "".format(coord),
+                f"{coord} shares the same name as one of its dimensions" "",
             )
             ret_val.append(not_matching.to_result())
 
         return ret_val
 
     # NOTE **********
     # IS THIS EVEN NEEDED ANYMORE?
@@ -2396,16 +2367,15 @@
             if "C" not in axis_map:
                 continue
 
             valid_rgrid = TestCtx(BaseCheck.HIGH, self.section_titles["5.3"])
             # Make sure reduced grid features define coordinates
             valid_rgrid.assert_true(
                 isinstance(coords, str) and coords,
-                "reduced grid feature {} must define coordinates attribute"
-                "".format(name),
+                f"reduced grid feature {name} must define coordinates attribute" "",
             )
             # We can't check anything else if there are no defined coordinates
             if not isinstance(coords, str) and coords:
                 continue
 
             coord_set = set(coords.split())
 
@@ -2425,24 +2395,24 @@
             )
 
             for compressed_coord in axis_map["C"]:
                 coord = ds.variables[compressed_coord]
                 compress = getattr(coord, "compress", None)
                 valid_rgrid.assert_true(
                     isinstance(compress, str) and compress,
-                    "compress attribute for compression coordinate {} must be a non-empty string"
-                    "".format(compressed_coord),
+                    f"compress attribute for compression coordinate {compressed_coord} must be a non-empty string"
+                    "",
                 )
                 if not isinstance(compress, str):
                     continue
                 for dim in compress.split():
                     valid_rgrid.assert_true(
                         dim in ds.dimensions,
-                        "dimension {} referenced by {}:compress must exist"
-                        "".format(dim, compressed_coord),
+                        f"dimension {dim} referenced by {compressed_coord}:compress must exist"
+                        "",
                     )
             ret_val.append(valid_rgrid.to_result())
 
         return ret_val
 
     def _check_grid_mapping_attr_condition(self, attr, attr_name):
         """
@@ -2757,68 +2727,51 @@
         ).items():
             variable = ds.variables[variable_name]
             valid = True
             reasoning = []
             if boundary_variable_name not in ds.variables:
                 valid = False
                 reasoning.append(
-                    "Boundary variable {} referenced by {} not ".format(
-                        boundary_variable_name,
-                        variable.name,
-                    )
+                    f"Boundary variable {boundary_variable_name} referenced by {variable.name} not "
                     + "found in dataset variables",
                 )
             else:
                 boundary_variable = ds.variables[boundary_variable_name]
             # The number of dimensions in the bounds variable should always be
             # the number of dimensions in the referring variable + 1
             if boundary_variable.ndim < 2:
                 valid = False
                 reasoning.append(
-                    "Boundary variable {} specified by {}".format(
-                        boundary_variable.name,
-                        variable.name,
-                    )
+                    f"Boundary variable {boundary_variable.name} specified by {variable.name}"
                     + " should have at least two dimensions to enclose the base "
                     + "case of a one dimensionsal variable",
                 )
             if boundary_variable.ndim != variable.ndim + 1:
                 valid = False
                 reasoning.append(
-                    "The number of dimensions of the variable {} is {}, but the "
-                    "number of dimensions of the boundary variable {} is {}. The boundary variable "
-                    "should have {} dimensions".format(
-                        variable.name,
-                        variable.ndim,
-                        boundary_variable.name,
-                        boundary_variable.ndim,
-                        variable.ndim + 1,
-                    ),
+                    f"The number of dimensions of the variable {variable.name} is {variable.ndim}, but the "
+                    f"number of dimensions of the boundary variable {boundary_variable.name} is {boundary_variable.ndim}. The boundary variable "
+                    f"should have {variable.ndim + 1} dimensions",
                 )
             if variable.dimensions[:] != boundary_variable.dimensions[: variable.ndim]:
                 valid = False
                 reasoning.append(
-                    "Boundary variable coordinates (for {}) are in improper order: {}. Bounds-specific dimensions should be last"
-                    "".format(variable.name, boundary_variable.dimensions),
+                    f"Boundary variable coordinates (for {variable.name}) are in improper order: {boundary_variable.dimensions}. Bounds-specific dimensions should be last"
+                    "",
                 )
 
             # ensure p vertices form a valid simplex given previous a...n
             # previous auxiliary coordinates
             if (
                 ds.dimensions[boundary_variable.dimensions[-1]].size
                 < len(boundary_variable.dimensions[:-1]) + 1
             ):
                 valid = False
                 reasoning.append(
-                    "Dimension {} of boundary variable (for {}) must have at least {} elements to form a simplex/closed cell with previous dimensions {}.".format(
-                        boundary_variable.name,
-                        variable.name,
-                        len(variable.dimensions) + 1,
-                        boundary_variable.dimensions[:-1],
-                    ),
+                    f"Dimension {boundary_variable.name} of boundary variable (for {variable.name}) must have at least {len(variable.dimensions) + 1} elements to form a simplex/closed cell with previous dimensions {boundary_variable.dimensions[:-1]}.",
                 )
             result = Result(
                 BaseCheck.MEDIUM,
                 valid,
                 self.section_titles["7.1"],
                 reasoning,
             )
@@ -2831,19 +2784,19 @@
         search_str = (
             r"^(?P<measure_type>area|volume):\s+(?P<cell_measure_var_name>\w+)$"
         )
         search_res = regex.match(search_str, var.cell_measures)
         if not search_res:
             valid = False
             reasoning.append(
-                "The cell_measures attribute for variable {} "
+                f"The cell_measures attribute for variable {var.name} "
                 "is formatted incorrectly. It should take the "
                 "form of either 'area: cell_var' or "
                 "'volume: cell_var' where cell_var is an existing name of "
-                "a variable describing the cell measures.".format(var.name),
+                "a variable describing the cell measures.",
             )
         else:
             valid = True
             cell_measure_var_name = search_res.group("cell_measure_var_name")
             cell_measure_type = search_res.group("measure_type")
             # TODO: cache previous results
             if cell_measure_var_name not in set(ds.variables.keys()).union(
@@ -2868,16 +2821,16 @@
                 )
 
             else:
                 cell_measure_var = ds.variables[cell_measure_var_name]
                 if not hasattr(cell_measure_var, "units"):
                     valid = False
                     reasoning.append(
-                        "Cell measure variable {} is required "
-                        "to have units attribute defined".format(cell_measure_var_name),
+                        f"Cell measure variable {cell_measure_var_name} is required "
+                        "to have units attribute defined",
                     )
                 else:
                     # IMPLEMENTATION CONFORMANCE REQUIRED 2/2
                     # verify this combination {area: 'm2', volume: 'm3'}
 
                     # key is valid measure types, value is expected
                     # exponent
@@ -2896,20 +2849,17 @@
                     else:
                         if not cell_measure_units.is_convertible(Unit(f"m{exponent}")):
                             valid = False
                             reasoning.append(conversion_failure_msg)
                     if not set(cell_measure_var.dimensions).issubset(var.dimensions):
                         valid = False
                         reasoning.append(
-                            "Cell measure variable {} must have "
+                            f"Cell measure variable {cell_measure_var_name} must have "
                             "dimensions which are a subset of "
-                            "those defined in variable {}.".format(
-                                cell_measure_var_name,
-                                var.name,
-                            ),
+                            f"those defined in variable {var.name}.",
                         )
 
         return Result(BaseCheck.MEDIUM, valid, (self.section_titles["7.2"]), reasoning)
 
     def check_cell_measures(self, ds):
         """
         7.2 To indicate extra information about the spatial properties of a
@@ -2980,16 +2930,16 @@
 
             valid_attribute = TestCtx(
                 BaseCheck.HIGH,
                 self.section_titles["7.3"],
             )  # changed from 7.1 to 7.3
             valid_attribute.assert_true(
                 regex.match(psep, method) is not None,
-                '"{}" is not a valid format for cell_methods attribute of "{}"'
-                "".format(method, var.name),
+                f'"{method}" is not a valid format for cell_methods attribute of "{var.name}"'
+                "",
             )
             ret_val.append(valid_attribute.to_result())
 
             valid_cell_names = TestCtx(BaseCheck.MEDIUM, self.section_titles["7.3"])
 
             # check that the name is valid
             for match in regex.finditer(psep, method):
@@ -3005,16 +2955,16 @@
                     ):
                         valid = True
                     else:
                         valid = False
 
                     valid_cell_names.assert_true(
                         valid,
-                        "{}'s cell_methods name component {} does not match a dimension, "
-                        "area or auxiliary coordinate".format(var.name, var_str),
+                        f"{var.name}'s cell_methods name component {var_str} does not match a dimension, "
+                        "area or auxiliary coordinate",
                     )
 
             ret_val.append(valid_cell_names.to_result())
 
             # Checks if the method value of the 'name: method' pair is acceptable
             valid_cell_methods = TestCtx(BaseCheck.MEDIUM, self.section_titles["7.3"])
 
@@ -3069,18 +3019,15 @@
                 interval_matches = regex.match(
                     r"^\s*(?P<interval_number>\S+)\s+(?P<interval_units>\S+)\s*$",
                     val,
                 )
                 # attempt to get the number for the interval
                 if not interval_matches:
                     valid_info.messages.append(
-                        '§7.3.3 {}:cell_methods contains an interval specification that does not parse: "{}". Should be in format "interval: <number> <units>"'.format(
-                            var.name,
-                            val,
-                        ),
+                        f'§7.3.3 {var.name}:cell_methods contains an interval specification that does not parse: "{val}". Should be in format "interval: <number> <units>"',
                     )
                 else:
                     try:
                         float(interval_matches.group("interval_number"))
                     except ValueError:
                         valid_info.messages.append(
                             '§7.3.3 {}:cell_methods contains an interval value that does not parse as a numeric value: "{}".'.format(
@@ -3107,46 +3054,36 @@
                 # comments can't really be invalid, except
                 # if they come first or aren't last, and
                 # maybe if they contain colons embedded in the
                 # comment string
                 valid_info.out_of += 1
                 if len(pmatches) == 1:
                     valid_info.messages.append(
-                        "§7.3.3 If there is no standardized information, the keyword comment: should be omitted for variable {}".format(
-                            var.name,
-                        ),
+                        f"§7.3.3 If there is no standardized information, the keyword comment: should be omitted for variable {var.name}",
                     )
                 # otherwise check that the comment is the last
                 # item in the parentheses
                 elif i != len(pmatches) - 1:
                     valid_info.messages.append(
-                        '§7.3.3 The non-standard "comment:" element must come after any standard elements in cell_methods for variable {}'.format(
-                            var.name,
-                        ),
+                        f'§7.3.3 The non-standard "comment:" element must come after any standard elements in cell_methods for variable {var.name}',
                     )
                 #
                 else:
                     valid_info.score += 1
             else:
                 valid_info.out_of += 1
                 valid_info.messages.append(
-                    '§7.3.3 Invalid cell_methods keyword "{}" for variable {}. Must be one of [interval, comment]'.format(
-                        keyword,
-                        var.name,
-                    ),
+                    f'§7.3.3 Invalid cell_methods keyword "{keyword}" for variable {var.name}. Must be one of [interval, comment]',
                 )
 
         # Ensure concatenated reconstructed matches are the same as the
         # original string.  If they're not, there's likely a formatting error
         valid_info.assert_true(
             "".join(m.group(0) for m in pmatches) == paren_contents,
-            "§7.3.3 Parenthetical content inside {}:cell_methods is not well formed: {}".format(
-                var.name,
-                paren_contents,
-            ),
+            f"§7.3.3 Parenthetical content inside {var.name}:cell_methods is not well formed: {paren_contents}",
         )
 
         return valid_info
 
     def check_climatological_statistics(self, ds):
         """
         7.4 A climatological time coordinate variable does not have a bounds attribute. Instead, it has a climatology
@@ -3277,17 +3214,15 @@
                 clim_coord_var.dimensions[:]
                 != ds.variables[clim_coord_var.climatology].dimensions[
                     : clim_coord_var.ndim
                 ]
             ):
                 total_climate_count += 1
                 reasoning.append(
-                    "Climatology variable coordinates are in improper order: {}. Bounds-specific dimensions should be last".format(
-                        ds.variables[clim_coord_var.climatology].dimensions,
-                    ),
+                    f"Climatology variable coordinates are in improper order: {ds.variables[clim_coord_var.climatology].dimensions}. Bounds-specific dimensions should be last",
                 )
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
                     (self.section_titles["7.4"]),
                     reasoning,
                 )
@@ -3298,17 +3233,15 @@
             elif (
                 ds.dimensions[
                     ds.variables[clim_coord_var.climatology].dimensions[-1]
                 ].size
                 != 2
             ):
                 reasoning.append(
-                    'Climatology dimension "{}" should only contain two elements'.format(
-                        ds.variables[clim_coord_var.climatology].name,
-                    ),
+                    f'Climatology dimension "{ds.variables[clim_coord_var.climatology].name}" should only contain two elements',
                 )
                 total_climate_count += 1
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
                     (self.section_titles["7.4"]),
                     reasoning,
@@ -3327,32 +3260,30 @@
         # info, e.g.
         # "time: method1 within years time: method2 over years (sidereal years)"
 
         meth_regex = "(?:{})".format(
             "|".join(methods),
         )  # "or" comparison for the methods
         re_string = (
-            r"^time: {0} within (years|days)"  # regex string to test
-            r" time: {0} over \1(?<=days)(?: time: {0} over years)?"
-            r"(?: \([^)]+\))?$".format(meth_regex)
+            rf"^time: {meth_regex} within (years|days)"  # regex string to test
+            rf" time: {meth_regex} over \1(?<=days)(?: time: {meth_regex} over years)?"
+            r"(?: \([^)]+\))?$"
         )
 
         # find any variables with a valid climatological cell_methods
         for cell_method_var in ds.get_variables_by_attributes(
             cell_methods=lambda s: s is not None,
         ):
             if any(
                 dim in all_clim_coord_var_names for dim in cell_method_var.dimensions
             ):
                 total_climate_count += 1
                 if not regex.search(re_string, cell_method_var.cell_methods):
                     reasoning.append(
-                        'The "time: method within years/days over years/days" format is not correct in variable {}.'.format(
-                            cell_method_var.name,
-                        ),
+                        f'The "time: method within years/days over years/days" format is not correct in variable {cell_method_var.name}.',
                     )
                 else:
                     valid_climate_count += 1
 
                 result = Result(
                     BaseCheck.MEDIUM,
                     (valid_climate_count, total_climate_count),
@@ -3532,64 +3463,55 @@
             valid = True
             reasoning = []
             # puts the referenced variable being compressed into a set
             compress_set = set(compress_var.compress.split(" "))
             if compress_var.ndim != 1:
                 valid = False
                 reasoning.append(
-                    "Compression variable {} may only have one dimension".format(
-                        compress_var.name,
-                    ),
+                    f"Compression variable {compress_var.name} may only have one dimension",
                 )
             # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 1/3
             # ensure compression variable is a proper index, and thus is an
             # signed or unsigned integer type of some sort
             if (compress_var.dtype is str) or (
                 compress_var.dtype.kind not in {"i", "u"}
             ):
                 valid = False
                 reasoning.append(
-                    "Compression variable {} must be an integer type to form a proper array index".format(
-                        compress_var.name,
-                    ),
+                    f"Compression variable {compress_var.name} must be an integer type to form a proper array index",
                 )
             # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 2/3
             # make sure all the variables referred to are contained by the
             # variables.
             if not compress_set.issubset(ds.dimensions):
                 not_in_dims = sorted(compress_set.difference(ds.dimensions))
                 valid = False
                 reasoning.append(
-                    "The following dimensions referenced by the compress attribute of variable {} do not exist: {}".format(
-                        compress_var.name,
-                        not_in_dims,
-                    ),
+                    f"The following dimensions referenced by the compress attribute of variable {compress_var.name} do not exist: {not_in_dims}",
                 )
             # IMPLEMENTATION CONFORMANCE 8.2 REQUIRED 3/3
             # The values of the associated coordinate variable must be in the range
             # starting with 0 and going up to the product of the compressed dimension
             # sizes minus 1 (CDL index conventions).
 
             # Put the the values of the associated coordinate variable into a list
             coord_list_size = [
                 item.size
                 for item in ds.dimensions.values()
                 if item.name in compress_set
             ]
-            # get the upper limt of the dimenssion size
+            # get the upper limit of the dimenssion size
             upper_limit_size = np.prod(coord_list_size) - 1
 
             for coord_size in coord_list_size:
                 if coord_size not in range(0, upper_limit_size):
                     valid = False
                     reasoning.append(
-                        "The dimenssion size {} referenced by the compress attribute is not "
-                        "in the range (0, The product of the compressed dimension sizes minus 1)".format(
-                            coord_size,
-                        ),
+                        f"The dimenssion size {coord_size} referenced by the compress attribute is not "
+                        "in the range (0, The product of the compressed dimension sizes minus 1)",
                     )
             result = Result(
                 BaseCheck.MEDIUM,
                 valid,
                 self.section_titles["8.2"],
                 reasoning,
             )
@@ -3697,32 +3619,32 @@
             # If we can't figure it out, don't check it.
             if variable_feature is None:
                 continue
             feature_types_found[variable_feature].append(name)
             matching_feature = TestCtx(BaseCheck.MEDIUM, self.section_titles["9.1"])
             matching_feature.assert_true(
                 variable_feature.lower() == _feature,
-                "{} is not a {}, it is detected as a {}"
-                "".format(name, _feature, variable_feature),
+                f"{name} is not a {_feature}, it is detected as a {variable_feature}"
+                "",
             )
             ret_val.append(matching_feature.to_result())
 
         # create explanation of all of the different featureTypes
         # found in the dataset
         feature_description = ", ".join(
             [
                 "{} ({})".format(ftr, ", ".join(vrs))
                 for ftr, vrs in feature_types_found.items()
             ],
         )
         all_same_features = TestCtx(BaseCheck.HIGH, self.section_titles["9.1"])
         all_same_features.assert_true(
             len(feature_types_found) < 2,
-            "Different feature types discovered in this dataset: {}"
-            "".format(feature_description),
+            f"Different feature types discovered in this dataset: {feature_description}"
+            "",
         )
         ret_val.append(all_same_features.to_result())
 
         return ret_val
 
     def check_hints(self, ds):
         """
@@ -3748,14 +3670,14 @@
         :return: List of results
         """
         ret_val = []
         boundary_variables = cfutil.get_cell_boundary_variables(ds)
         for name in ds.variables:
             if name.endswith("_bounds") and name not in boundary_variables:
                 msg = (
-                    "{} might be a cell boundary variable but there are no variables that define it "
-                    "as a boundary using the `bounds` attribute.".format(name)
+                    f"{name} might be a cell boundary variable but there are no variables that define it "
+                    "as a boundary using the `bounds` attribute."
                 )
                 result = Result(BaseCheck.LOW, True, self.section_titles["7.1"], [msg])
                 ret_val.append(result)
 
         return ret_val
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf_1_7.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf_1_7.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,56 +163,46 @@
                     # fail.
                     out_of += 1
                     if not np.isclose(
                         variable.actual_range[0],
                         variable[:].min(),
                     ) or not np.isclose(variable.actual_range[1], variable[:].max()):
                         msgs.append(
-                            "actual_range elements of '{}' inconsistent with its min/max values".format(
-                                name,
-                            ),
+                            f"actual_range elements of '{name}' inconsistent with its min/max values",
                         )
                     else:
                         score += 1
 
                 # check that the actual range is within the valid range
                 if hasattr(variable, "valid_range"):  # check within valid_range
                     out_of += 1
                     if (variable.actual_range[0] < variable.valid_range[0]) or (
                         variable.actual_range[1] > variable.valid_range[1]
                     ):
                         msgs.append(
-                            '"{}"\'s actual_range must be within valid_range'.format(
-                                name,
-                            ),
+                            f'"{name}"\'s actual_range must be within valid_range',
                         )
                     else:
                         score += 1
 
                 # check the elements of the actual range have the appropriate
                 # relationship to the valid_min and valid_max
                 if hasattr(variable, "valid_min"):
                     out_of += 1
                     if variable.actual_range[0] < variable.valid_min:
                         msgs.append(
-                            '"{}"\'s actual_range first element must be >= valid_min ({})'.format(
-                                name,
-                                variable.valid_min,
-                            ),
+                            f'"{name}"\'s actual_range first element must be >= valid_min ({variable.valid_min})',
                         )
                     else:
                         score += 1
                 if hasattr(variable, "valid_max"):
                     out_of += 1
                     if variable.actual_range[1] > variable.valid_max:
                         msgs.append(
-                            '"{}"\'s actual_range second element must be <= valid_max ({})'.format(
-                                name,
-                                variable.valid_max,
-                            ),
+                            f'"{name}"\'s actual_range second element must be <= valid_max ({variable.valid_max})',
                         )
                     else:
                         score += 1
 
             ret_val.append(
                 Result(  # putting result into list
                     BaseCheck.HIGH,
@@ -250,116 +240,87 @@
 
             # 7.1 Required 1/5:
             # The type of the bounds attribute is a string whose value is a single variable name.
             # The specified variable must exist in the file.
             if boundary_variable_name not in ds.variables:
                 valid = False
                 reasoning.append(
-                    "Boundary variable {} referenced by {} not ".format(
-                        boundary_variable_name,
-                        variable.name,
-                    )
+                    f"Boundary variable {boundary_variable_name} referenced by {variable.name} not "
                     + "found in dataset variables",
                 )
             else:
                 boundary_variable = ds.variables[boundary_variable_name]
 
             # 7.1 Required 2/5:
             # The number of dimensions in the bounds variable should always be
             # the number of dimensions in the referring variable + 1
             if boundary_variable.ndim < 2:
                 valid = False
                 reasoning.append(
-                    "Boundary variable {} specified by {}".format(
-                        boundary_variable.name,
-                        variable.name,
-                    )
+                    f"Boundary variable {boundary_variable.name} specified by {variable.name}"
                     + " should have at least two dimensions to enclose the base "
                     + "case of a one dimensionsal variable",
                 )
             if boundary_variable.ndim != variable.ndim + 1:
                 valid = False
                 reasoning.append(
-                    "The number of dimensions of the variable {} is {}, but the "
-                    "number of dimensions of the boundary variable {} is {}. The boundary variable "
-                    "should have {} dimensions".format(
-                        variable.name,
-                        variable.ndim,
-                        boundary_variable.name,
-                        boundary_variable.ndim,
-                        variable.ndim + 1,
-                    ),
+                    f"The number of dimensions of the variable {variable.name} is {variable.ndim}, but the "
+                    f"number of dimensions of the boundary variable {boundary_variable.name} is {boundary_variable.ndim}. The boundary variable "
+                    f"should have {variable.ndim + 1} dimensions",
                 )
             if variable.dimensions[:] != boundary_variable.dimensions[: variable.ndim]:
                 valid = False
                 reasoning.append(
-                    "Boundary variable coordinates (for {}) are in improper order: {}. Bounds-specific dimensions should be last"
-                    "".format(variable.name, boundary_variable.dimensions),
+                    f"Boundary variable coordinates (for {variable.name}) are in improper order: {boundary_variable.dimensions}. Bounds-specific dimensions should be last"
+                    "",
                 )
 
             # 7.1 Required 2/5: continue
             # Ensure p vertices form a valid simplex given previous a...n
             # previous auxiliary coordinates
             if (
                 ds.dimensions[boundary_variable.dimensions[-1]].size
                 < len(boundary_variable.dimensions[:-1]) + 1
             ):
                 valid = False
                 reasoning.append(
-                    "Dimension {} of boundary variable (for {}) must have at least {} elements to form a simplex/closed cell with previous dimensions {}.".format(
-                        boundary_variable.name,
-                        variable.name,
-                        len(variable.dimensions) + 1,
-                        boundary_variable.dimensions[:-1],
-                    ),
+                    f"Dimension {boundary_variable.name} of boundary variable (for {variable.name}) must have at least {len(variable.dimensions) + 1} elements to form a simplex/closed cell with previous dimensions {boundary_variable.dimensions[:-1]}.",
                 )
 
             # 7.1 Required 3/5:
             # A boundary variable must be a numeric data type
             if boundary_variable.dtype.kind not in "biufc":
                 valid = False
                 reasoning.append(
-                    "Boundary variable {} specified by {}".format(
-                        boundary_variable.name,
-                        variable.name,
-                    )
+                    f"Boundary variable {boundary_variable.name} specified by {variable.name}"
                     + "must be a numeric data type ",
                 )
 
             # 7.1 Required 4/5:
             # If a boundary variable has units, standard_name, axis, positive, calendar, leap_month,
             # leap_year or month_lengths attributes, they must agree with those of its associated variable.
             if boundary_variable.__dict__.keys():
                 for item in boundary_variable.__dict__.keys():
                     if hasattr(variable, item):
                         if getattr(variable, item) != getattr(boundary_variable, item):
                             valid = False
                             reasoning.append(
-                                "'{}' has attr '{}' with value '{}' that does not agree "
-                                "with its associated variable ('{}')'s attr value '{}'"
-                                "".format(
-                                    boundary_variable_name,
-                                    item,
-                                    getattr(boundary_variable, item),
-                                    variable.name,
-                                    getattr(variable, item),
-                                ),
+                                f"'{boundary_variable_name}' has attr '{item}' with value '{getattr(boundary_variable, item)}' that does not agree "
+                                f"with its associated variable ('{variable.name}')'s attr value '{getattr(variable, item)}'"
+                                "",
                             )
 
             # 7.1 Required 5/5:
             # check if formula_terms is present in the var; if so,
             # the bounds variable must also have a formula_terms attr
             if hasattr(variable, "formula_terms"):
                 if not hasattr(boundary_variable, "formula_terms"):
                     valid = False
                     reasoning.append(
-                        "'{}' has 'formula_terms' attr, bounds variable '{}' must also have 'formula_terms'".format(
-                            variable_name,
-                            boundary_variable_name,
-                        ),
+                        f"'{variable_name}' has 'formula_terms' attr, bounds variable '{boundary_variable_name}' must also have 'formula_terms'",
                     )
 
             # 7.1 Recommendations 2/2
             # Boundary variables should not have the _FillValue, missing_value, units, standard_name, axis,
             # positive, calendar, leap_month, leap_year or month_lengths attributes.
             attributes_to_check = {
                 "_FillValue",
@@ -376,18 +337,15 @@
             if boundary_variable.__dict__.keys():
                 lst1 = boundary_variable.__dict__.keys()
                 lst2 = attributes_to_check
                 unwanted_attributes = [value for value in lst1 if value in lst2]
                 if unwanted_attributes:
                     valid = False
                     reasoning.append(
-                        "The Boundary variables '{}' should not have the attributes: '{}'".format(
-                            boundary_variable_name,
-                            unwanted_attributes,
-                        ),
+                        f"The Boundary variables '{boundary_variable_name}' should not have the attributes: '{unwanted_attributes}'",
                     )
 
             result = Result(
                 BaseCheck.MEDIUM,
                 valid,
                 self.section_titles["7.1"],
                 reasoning,
@@ -417,32 +375,26 @@
                 if abs(boundary_variable[ii][1]) >= abs(boundary_variable[ii][0]):
                     if not (
                         (abs(variable[ii]) >= abs(boundary_variable[ii][0]))
                         and (abs(variable[ii]) <= abs(boundary_variable[ii][1]))
                     ):
                         valid = False
                         reasoning.append(
-                            "The points specified by the coordinate variable {} ({})"
+                            f"The points specified by the coordinate variable {variable_name} ({variable[ii]})"
                             " lie outside the boundary of the cell specified by the "
-                            "associated boundary variable {} ({})".format(
-                                variable_name,
-                                variable[ii],
-                                boundary_variable_name,
-                                boundary_variable[ii],
-                            ),
+                            f"associated boundary variable {boundary_variable_name} ({boundary_variable[ii]})",
                         )
 
                 result = Result(
                     BaseCheck.MEDIUM,
                     valid,
                     self.section_titles["7.1"],
                     reasoning,
                 )
                 ret_val.append(result)
-                print(ret_val)
             return ret_val
 
     def check_cell_measures(self, ds):
         """
         A method to over-ride the CF1_6Check method. In CF 1.7, it is specified
         that variable referenced by cell_measures must be in the dataset OR
         referenced by the global attribute "external_variables", which represent
@@ -790,16 +742,14 @@
         elif val.size not in (3, 6, 7):
             return (False, msg)
 
         else:
             return (True, msg)
 
     def check_grid_mapping(self, ds):
-        # FIXME: Looks like this is not needed.
-        # super().check_grid_mapping.__doc__
         prev_return = super().check_grid_mapping(ds)
         grid_mapping_variables = cfutil.get_grid_mapping_variables(ds)
         for var_name in sorted(grid_mapping_variables):
             var = ds.variables[var_name]
             test_ctx = self.get_test_ctx(
                 BaseCheck.HIGH,
                 self.section_titles["5.6"],
@@ -816,17 +766,15 @@
                     test_ctx.messages.append("crs_wkt attribute must be a string")
                     test_ctx.out_of += 1
                 else:
                     try:
                         pyproj.CRS.from_wkt(crs_wkt)
                     except pyproj.exceptions.CRSError as crs_error:
                         test_ctx.messages.append(
-                            "Cannot parse crs_wkt attribute to CRS using Proj4. Proj4 error: {}".format(
-                                str(crs_error),
-                            ),
+                            f"Cannot parse crs_wkt attribute to CRS using Proj4. Proj4 error: {str(crs_error)}",
                         )
                     else:
                         test_ctx.score += 1
                     test_ctx.out_of += 1
 
             # existence_conditions
             exist_cond_1 = (
@@ -844,43 +792,39 @@
             # check that geoid_name and geopotential_datum_name are not both
             # present in the grid_mapping variable
             if len_vdatum_name_attrs == 2:
                 test_ctx.out_of += 1
                 test_ctx.messages.append(
                     "Cannot have both 'geoid_name' and "
                     "'geopotential_datum_name' attributes in "
-                    "grid mapping variable '{}'".format(var.name),
+                    f"grid mapping variable '{var.name}'",
                 )
             elif len_vdatum_name_attrs == 1:
                 # should be one or zero attrs
                 proj_db_path = os.path.join(pyproj.datadir.get_data_dir(), "proj.db")
                 try:
                     with sqlite3.connect(proj_db_path) as conn:
                         v_datum_attr = next(iter(vert_datum_attrs))
                         v_datum_value = getattr(var, v_datum_attr)
                         v_datum_str_valid = self._process_v_datum_str(
                             v_datum_value,
                             conn,
                         )
 
                         invalid_msg = (
-                            "Vertical datum value '{}' for "
-                            "attribute '{}' in grid mapping "
-                            "variable '{}' is not valid".format(
-                                v_datum_value,
-                                v_datum_attr,
-                                var.name,
-                            )
+                            f"Vertical datum value '{v_datum_value}' for "
+                            f"attribute '{v_datum_attr}' in grid mapping "
+                            f"variable '{var.name}' is not valid"
                         )
                         test_ctx.assert_true(v_datum_str_valid, invalid_msg)
                 except sqlite3.Error as e:
                     # if we hit an error, skip the check
                     warn(
                         "Error occurred while trying to query "
-                        "Proj4 SQLite database at {}: {}".format(proj_db_path, str(e)),
+                        f"Proj4 SQLite database at {proj_db_path}: {str(e)}",
                         stacklevel=2,
                     )
             prev_return[var.name] = test_ctx.to_result()
 
         return prev_return
 
     def check_standard_name_deprecated_modifiers(self, ds):
@@ -941,18 +885,15 @@
         if formula_terms is None and standard_name not in dim_vert_coords_dict:
             return
 
         # assert that the computed_standard_name is maps to the standard_name correctly
         _comp_std_name = dim_vert_coords_dict[standard_name][1]
         correct_computed_std_name_ctx.assert_true(
             getattr(variable, "computed_standard_name", None) in _comp_std_name,
-            "§4.3.3 The standard_name of `{}` must map to the correct computed_standard_name, `{}`".format(
-                vname,
-                sorted(_comp_std_name),
-            ),
+            f"§4.3.3 The standard_name of `{vname}` must map to the correct computed_standard_name, `{sorted(_comp_std_name)}`",
         )
         ret_val.append(correct_computed_std_name_ctx.to_result())
 
     def check_dimensionless_vertical_coordinates(self, ds):
         """
         Check the validity of dimensionless coordinates under CF
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf_1_8.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf_1_8.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 import numpy as np
 import requests
 from lxml import etree
 from netCDF4 import Dataset
 from shapely.geometry import Polygon
 
-from compliance_checker import MemoizedDataset
 from compliance_checker.base import BaseCheck, TestCtx
 from compliance_checker.cf.cf_1_7 import CF1_7Check
 from compliance_checker.cf.util import reference_attr_variables, string_from_var_type
 
 
 class CF1_8Check(CF1_7Check):
     """Implementation for CF v1.8. Inherits from CF1_7Check."""
@@ -42,15 +41,15 @@
             {
                 "2.7": "§2.7 Groups",
                 "6.1.2": "§6.1.2 Taxon Names and Identifiers",
                 "7.5": "§7.5 Geometries",
             },
         )
 
-    def check_groups(self, ds: MemoizedDataset):
+    def check_groups(self, ds: Dataset):
         """
         2.7.2. Application of attributes
 
         The following attributes are optional for non-root groups. They are allowed in order to
         provide additional provenance and description of the subsidiary data. They do not override
         attributes from parent groups.
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf_1_9.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf_1_9.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,16 +72,14 @@
                         [reasoning],
                     )
 
                     ret_val.append(result)
         return ret_val
 
     def check_time_coordinate(self, ds):
-        # FIXME: Looks like this is not needed.
-        # super().check_calendar.__doc__
         prev_return = super().check_time_coordinate(ds)
         seconds_regex = regex.compile(
             r"\w+ since \d{1,4}-\d{1,2}-\d{1,2}[ T]"
             r"\d{1,2}:\d{1,2}:(?P<seconds>\d{1,2})",
         )
         for name in cfutil.get_time_variables(ds):
             # DRY: get rid of time coordinate variable boilerplate
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/cf_base.py` & `compliance_checker-5.1.1/compliance_checker/cf/cf_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,16 +181,16 @@
             defines_grid_mapping = self.get_test_ctx(
                 BaseCheck.HIGH,
                 self.section_titles["5.6"],
                 variable.name,
             )
             defines_grid_mapping.assert_true(
                 (isinstance(grid_mapping, str) and grid_mapping),
-                "{}'s grid_mapping attribute must be a "
-                "space-separated non-empty string".format(variable.name),
+                f"{variable.name}'s grid_mapping attribute must be a "
+                "space-separated non-empty string",
             )
             if isinstance(grid_mapping, str):
                 # TODO (badams): refactor functionality to split functionality
                 #                into requisite classes
                 if ":" in grid_mapping and self._cc_spec_version >= "1.7":
                     colon_count = grid_mapping.count(":")
                     re_all = regex.findall(
@@ -202,34 +202,27 @@
                         defines_grid_mapping.messages.append(
                             "Could not consume entire grid_mapping expression, please check for well-formedness",
                         )
                     else:
                         for grid_var_name, coord_var_str in re_all:
                             defines_grid_mapping.assert_true(
                                 grid_var_name in ds.variables,
-                                "grid mapping variable {} must exist in this dataset".format(
-                                    grid_var_name,
-                                ),
+                                f"grid mapping variable {grid_var_name} must exist in this dataset",
                             )
                             for ref_var in coord_var_str.split():
                                 defines_grid_mapping.assert_true(
                                     ref_var in ds.variables,
-                                    "Coordinate-related variable {} referenced by grid_mapping variable {} must exist in this dataset".format(
-                                        ref_var,
-                                        grid_var_name,
-                                    ),
+                                    f"Coordinate-related variable {ref_var} referenced by grid_mapping variable {grid_var_name} must exist in this dataset",
                                 )
 
                 else:
                     for grid_var_name in grid_mapping.split():
                         defines_grid_mapping.assert_true(
                             grid_var_name in ds.variables,
-                            "grid mapping variable {} must exist in this dataset".format(
-                                grid_var_name,
-                            ),
+                            f"grid mapping variable {grid_var_name} must exist in this dataset",
                         )
             ret_val[variable.name] = defines_grid_mapping.to_result()
 
         # Check the grid mapping variables themselves
         for grid_var_name in grid_mapping_variables:
             valid_grid_mapping = self.get_test_ctx(
                 BaseCheck.HIGH,
@@ -260,18 +253,15 @@
 
             grid_mapping = self.grid_mapping_dict[grid_mapping_name]
             required_attrs = grid_mapping[0]
             # Make sure all the required attributes are defined
             for req in required_attrs:
                 valid_grid_mapping.assert_true(
                     hasattr(grid_var, req),
-                    "{} is a required attribute for grid mapping {}".format(
-                        req,
-                        grid_mapping_name,
-                    ),
+                    f"{req} is a required attribute for grid mapping {grid_mapping_name}",
                 )
 
             # Make sure that exactly one of the exclusive attributes exist
             if len(grid_mapping) == 4:
                 at_least_attr = grid_mapping[3]
                 number_found = 0
                 for attr in at_least_attr:
@@ -309,28 +299,25 @@
 
         :param netCDF4.Dataset ds: An open netCDF dataset
         :rtype: compliance_checker.base.Result
         """
 
         valid = False
         reasoning = []
-        correct_version_string = "{}-{}".format(
-            self._cc_spec,
-            self._cc_spec_version,
-        ).upper()
+        correct_version_string = f"{self._cc_spec}-{self._cc_spec_version}".upper()
         if hasattr(ds, "Conventions"):
             conventions = regex.split(r",|\s+", getattr(ds, "Conventions", ""))
             for convention in conventions:
                 if convention == correct_version_string:
                     valid = True
                     break
             else:
                 reasoning = [
                     "§2.6.1 Conventions global attribute does not contain "
-                    '"{}"'.format(correct_version_string),
+                    f'"{correct_version_string}"',
                 ]
         else:
             valid = False
             reasoning = ["§2.6.1 Conventions field is not present"]
         return Result(
             BaseCheck.MEDIUM,
             valid,
@@ -384,16 +371,16 @@
         variable = ds.variables[coord]
         standard_name = getattr(variable, "standard_name", None)
         formula_terms = getattr(variable, "formula_terms", None)
         valid_formula_terms = TestCtx(BaseCheck.HIGH, self.section_titles["4.3"])
 
         valid_formula_terms.assert_true(
             isinstance(formula_terms, str) and formula_terms,
-            "§4.3.2: {}'s formula_terms is a required attribute and must be a non-empty string"
-            "".format(coord),
+            f"§4.3.2: {coord}'s formula_terms is a required attribute and must be a non-empty string"
+            "",
         )
         # We can't check any more
         if not formula_terms:
             return valid_formula_terms.to_result()
 
         # check that the formula_terms are well formed and are present
         # The pattern for formula terms is always component: variable_name
@@ -426,24 +413,24 @@
         valid_formula_terms.assert_true(
             reconstructed_formula == formula_terms,
             "Attribute formula_terms is not well-formed",
         )
 
         valid_formula_terms.assert_true(
             standard_name in dimless_coords_dict,
-            "unknown standard_name '{}' for dimensionless vertical coordinate {}"
-            "".format(standard_name, coord),
+            f"unknown standard_name '{standard_name}' for dimensionless vertical coordinate {coord}"
+            "",
         )
         if standard_name not in dimless_coords_dict:
             return valid_formula_terms.to_result()
 
         valid_formula_terms.assert_true(
             no_missing_terms(standard_name, terms, dimless_coords_dict),
-            "{}'s formula_terms are invalid for {}, please see appendix D of CF 1.6"
-            "".format(coord, standard_name),
+            f"{coord}'s formula_terms are invalid for {standard_name}, please see appendix D of CF 1.6"
+            "",
         )
 
         return valid_formula_terms.to_result()
 
     def _check_grid_mapping_attr_condition(self, attr, attr_name, ret_val):
         """
         Evaluate a condition (or series of conditions) for a particular
@@ -485,21 +472,16 @@
             val_type = type(attr_val)
         else:
             val_type = attr_val.dtype.type
             type_match = val_type == var.dtype.type
 
         ctx.assert_true(
             type_match,
-            "Attribute '{}' (type: {}) and parent variable '{}' (type: {}) "
-            "must have equivalent datatypes".format(
-                attr_name,
-                val_type,
-                var.name,
-                var.dtype.type,
-            ),
+            f"Attribute '{attr_name}' (type: {val_type}) and parent variable '{var.name}' (type: {var.dtype.type}) "
+            "must have equivalent datatypes",
         )
 
     def _find_aux_coord_vars(self, ds, refresh=False):
         """
         Returns a list of auxiliary coordinate variables
 
         An auxiliary coordinate variable is any netCDF variable that contains
@@ -563,15 +545,15 @@
         # Used the cached version if it exists and is not empty
         if self._ancillary_vars.get(ds, None) and refresh is False:
             return self._ancillary_vars[ds]
 
         # Invalidate the cache at all costs
         self._ancillary_vars[ds] = []
 
-        for _name, var in ds.variables.items():
+        for var in ds.variables.values():
             if hasattr(var, "ancillary_variables"):
                 for anc_name in var.ancillary_variables.split(" "):
                     if anc_name in ds.variables:
                         self._ancillary_vars[ds].append(anc_name)
 
             if hasattr(var, "grid_mapping"):
                 gm_name = var.grid_mapping
@@ -678,18 +660,15 @@
                 util.download_cf_standard_name_table(version, location)
                 print(
                     f"Using downloaded standard name table v{version}",
                     file=sys.stderr,
                 )
             else:
                 print(
-                    "Using cached standard name table v{} from {}".format(
-                        version,
-                        location,
-                    ),
+                    f"Using cached standard name table v{version} from {location}",
                     file=sys.stderr,
                 )
 
             self._std_names = util.StandardNameTable(location)
             return True
         except Exception as e:
             # There was an error downloading the CF table. That's ok, we'll just use the packaged version
@@ -1052,24 +1031,22 @@
             # this is a fallback in case an empty att_loc is passed
             # it generally should not occur
             valid_loc = "no locations in the dataset"
             loc_sort = sorted(att_loc)
             if att_loc_len == 1:
                 valid_loc = att_loc_print_helper(loc_sort[0])
             elif att_loc_len == 2:
-                valid_loc = "{} and {}".format(
-                    att_loc_print_helper(loc_sort[0]),
-                    att_loc_print_helper(loc_sort[1]),
-                )
+                valid_loc = f"{att_loc_print_helper(loc_sort[0])} and {att_loc_print_helper(loc_sort[1])}"
             # shouldn't be reached under normal circumstances, as any attribute
             # should be either G, C, or D but if another
             # category is added, this will be useful.
             else:
-                valid_loc = ", ".join(loc_sort[:-1]) + ", and {}".format(
-                    att_loc_print_helper(loc_sort[-1]),
+                valid_loc = (
+                    ", ".join(loc_sort[:-1])
+                    + f", and {att_loc_print_helper(loc_sort[-1])}"
                 )
             return f"This attribute may only appear in {valid_loc}."
 
         for global_att_name in possible_global_atts:
             global_att = ds.getncattr(global_att_name)
             att_dict = self.appendix_a[global_att_name]
             att_loc = att_dict["attr_loc"]
@@ -1084,16 +1061,16 @@
             else:
                 section_loc = None
             test_ctx = TestCtx(BaseCheck.HIGH, section_loc)
 
             test_ctx.out_of += 1
             if "G" not in att_loc:
                 test_ctx.messages.append(
-                    '[Appendix A] Attribute "{}" should not be present in global (G) '
-                    "attributes. {}".format(global_att_name, valid_loc_warn),
+                    f'[Appendix A] Attribute "{global_att_name}" should not be present in global (G) '
+                    f"attributes. {valid_loc_warn}",
                 )
             else:
                 result = self._handle_dtype_check(global_att, global_att_name, att_dict)
                 if not result[0]:
                     test_ctx.messages.append(result[1])
                 else:
                     test_ctx.score += 1
@@ -1123,21 +1100,16 @@
                     test_ctx = TestCtx(BaseCheck.HIGH, section_loc, variable=var_name)
                     att_loc = att_dict["attr_loc"]
                     valid_loc_warn = _att_loc_msg(att_loc)
                     att = var.getncattr(att_name)
                     test_ctx.out_of += 1
                     if coord_letter not in att_loc:
                         test_ctx.messages.append(
-                            '[Appendix A] Attribute "{}" should not be present in {} '
-                            'variable "{}". {}'.format(
-                                att_name,
-                                att_loc_print_helper(coord_letter),
-                                var_name,
-                                valid_loc_warn,
-                            ),
+                            f'[Appendix A] Attribute "{att_name}" should not be present in {att_loc_print_helper(coord_letter)} '
+                            f'variable "{var_name}". {valid_loc_warn}',
                         )
                     else:
                         result = self._handle_dtype_check(att, att_name, att_dict, var)
                         if not result[0]:
                             test_ctx.messages.append(result[1])
                         else:
                             test_ctx.score += 1
@@ -1184,18 +1156,15 @@
                 # TODO: handle edge case where variable is unset here
                 temp_ctx = TestCtx()
                 self._parent_var_attr_type_check(attr_name, variable, temp_ctx)
                 var_dtype = getattr(variable, "dtype", None)
                 if temp_ctx.messages:
                     return (
                         False,
-                        "{} must be numeric and must be equivalent to {} dtype".format(
-                            attr_name,
-                            var_dtype,
-                        ),
+                        f"{attr_name} must be numeric and must be equivalent to {var_dtype} dtype",
                     )
             else:
                 # If we reached here, we fell off with an unrecognized type
                 return (
                     False,
                     f"{attr_name} has unrecognized type '{attr_type}'",
                 )
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cf/util.py` & `compliance_checker-5.1.1/compliance_checker/cf/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import itertools
 import os
 import sys
 from pkgutil import get_data
 
 import requests
 from cf_units import Unit
+from importlib_resources import files
 from lxml import etree
 from netCDF4 import Dataset
-from pkg_resources import resource_filename
 
 # copied from paegan
 # paegan may depend on these later
 _possiblet = {
     "time",
     "TIME",
     "Time",
@@ -69,15 +69,14 @@
     "x",
     "X",
     "lon",
     "LON",
     "xlon",
     "XLON",
     "lonx",
-    "lonx",
     "lon_u",
     "LON_U",
     "lon_v",
     "LON_V",
     "lonc",
     "LONC",
     "Lon",
@@ -93,15 +92,14 @@
     "y",
     "Y",
     "lat",
     "LAT",
     "ylat",
     "YLAT",
     "laty",
-    "laty",
     "lat_u",
     "LAT_U",
     "lat_v",
     "LAT_V",
     "latc",
     "LATC",
     "Lat",
@@ -165,15 +163,15 @@
     """
     Returns a value with in a nested dict structure from a dot separated
     path expression such as "system.server.host" or a list of key entries
     @retval Value if found or None
     """
     try:
         obj = dict_instance
-        keylist = keypath if type(keypath) is list else keypath.split(".")
+        keylist = keypath if isinstance(keypath, list) else keypath.split(".")
         for key in keylist:
             obj = obj[key]
         return obj
     except Exception:
         return default
 
 
@@ -282,34 +280,26 @@
     :param str version: CF standard name table version number (i.e 34)
     :param str location: Path/filename to write downloaded xml file to
     """
 
     if (
         location is None
     ):  # This case occurs when updating the packaged version from command line
-        location = resource_filename(
-            "compliance_checker",
-            "data/cf-standard-name-table.xml",
-        )
+        location = files("compliance_checker") / "data/cf-standard-name-table.xml"
 
     if version == "latest":
         url = "http://cfconventions.org/Data/cf-standard-names/current/src/cf-standard-name-table.xml"
     else:
-        url = "http://cfconventions.org/Data/cf-standard-names/{}/src/cf-standard-name-table.xml".format(
-            version,
-        )
+        url = f"http://cfconventions.org/Data/cf-standard-names/{version}/src/cf-standard-name-table.xml"
 
     r = requests.get(url, allow_redirects=True)
     r.raise_for_status()
 
     print(
-        "Downloading cf-standard-names table version {} from: {}".format(
-            version,
-            url,
-        ),
+        f"Downloading cf-standard-names table version {version} from: {url}",
         file=sys.stderr,
     )
     with open(location, "wb") as f:
         f.write(r.content)
 
 
 def create_cached_data_dir():
```

### Comparing `compliance-checker-5.1.0/compliance_checker/cfutil.py` & `compliance_checker-5.1.1/compliance_checker/cfutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import csv
 import re
 import warnings
 from collections import defaultdict
 from functools import lru_cache, partial
 
 from cf_units import Unit
-from pkg_resources import resource_filename
+from importlib_resources import files
 
 _UNITLESS_DB = None
 _SEA_NAMES = None
 
 VALID_LAT_UNITS = {
     "degrees_north",
     "degree_north",
@@ -124,15 +124,15 @@
 
     source of list: https://www.ncei.noaa.gov/resources/ocean-data-format-codes
     """
     global _SEA_NAMES
     if _SEA_NAMES is None:
         buf = {}
         with open(
-            resource_filename("compliance_checker", "data/seanames.csv"),
+            files("compliance_checker") / "data/seanames.csv",
         ) as f:
             reader = csv.reader(f)
             for code, sea_name in reader:
                 buf[sea_name] = code
         _SEA_NAMES = buf
     return _SEA_NAMES
 
@@ -273,15 +273,15 @@
     An auxiliary coordinate variable is any netCDF variable that contains
     coordinate data, but is not a coordinate variable (in the sense of the term
     defined by CF).
 
     :param netCDf4.Dataset ds: An open netCDF dataset
     """
     aux_vars = []
-    # get any variables referecned by the coordinates attribute
+    # get any variables referenced by the coordinates attribute
     for ncvar in ds.get_variables_by_attributes(
         coordinates=lambda x: isinstance(x, str),
     ):
         # split the coordinates into individual variable names
         referenced_variables = ncvar.coordinates.split(" ")
         # if the variable names exist, add them
         for referenced_variable in referenced_variables:
```

### Comparing `compliance-checker-5.1.0/compliance_checker/data/cf-standard-name-table.xml` & `compliance_checker-5.1.1/compliance_checker/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/data/seanames.csv` & `compliance_checker-5.1.1/compliance_checker/data/seanames.csv`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/data/templates/ccheck.html.j2` & `compliance_checker-5.1.1/compliance_checker/data/templates/ccheck.html.j2`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/data/templates/ccheck_wrapper.html.j2` & `compliance_checker-5.1.1/compliance_checker/data/templates/ccheck_wrapper.html.j2`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/ioos.py` & `compliance_checker-5.1.1/compliance_checker/ioos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Check for IOOS-approved attributes
 """
+
 import re
 from numbers import Number
 
 import validators
 from cf_units import Unit
 from lxml.etree import XPath
 from owslib.namespaces import Namespaces
@@ -42,48 +43,37 @@
         Checks for the existence of attr in ds, with the name/message using concept_name.
         """
         val = cls.std_check(ds, attr)
         msgs = []
 
         if not val:
             msgs.append(
-                "Attr '{}' (IOOS concept: '{}') not found in dataset".format(
-                    attr,
-                    concept_name,
-                ),
+                f"Attr '{attr}' (IOOS concept: '{concept_name}') not found in dataset",
             )
 
         return Result(priority, val, concept_name, msgs)
 
     @classmethod
     def _has_var_attr(cls, dataset, vname, attr, concept_name, priority=BaseCheck.HIGH):
         """
         Checks for the existence of an attr on variable vname in dataset, with the name/message using concept_name.
         """
         val = True
         msgs = []
         if vname not in dataset.variables:
             val = False
             msgs.append(
-                "Variable '{}' not present while checking for attr '{}' for IOOS concept: '{}'".format(
-                    vname,
-                    attr,
-                    concept_name,
-                ),
+                f"Variable '{vname}' not present while checking for attr '{attr}' for IOOS concept: '{concept_name}'",
             )
         else:
             v = dataset.variables[vname]
             if attr not in v.ncattrs():
                 val = False
                 msgs.append(
-                    "Attr '{}' not present on var '{}' while checking for IOOS concept: '{}'".format(
-                        attr,
-                        vname,
-                        concept_name,
-                    ),
+                    f"Attr '{attr}' not present on var '{vname}' while checking for IOOS concept: '{concept_name}'",
                 )
 
         return Result(priority, val, concept_name, msgs)
 
 
 class IOOSNCCheck(BaseNCCheck, IOOSBaseCheck):
     def check_time_period(self, ds):
@@ -792,17 +782,15 @@
             except TypeError:
                 vocb_results.append(
                     Result(
                         BaseCheck.MEDIUM,
                         False,
                         "contributor_role_vocabulary",
                         [
-                            "contributor_role_vocabulary '{}' must be of type 'string'".format(
-                                vocb,
-                            ),
+                            f"contributor_role_vocabulary '{vocb}' must be of type 'string'",
                         ],
                     ),
                 )
         else:
             vocb_results.append(
                 Result(
                     BaseCheck.MEDIUM,
@@ -1241,16 +1229,16 @@
             else:
                 expected_types = {"person", "group", "institution", "position"}
                 if att_value in expected_types:
                     pass_stat = True
                 else:
                     pass_stat = False
                     messages.append(
-                        "If specified, {} must be in value list "
-                        "({})".format(global_att_name, sorted(expected_types)),
+                        f"If specified, {global_att_name} must be in value list "
+                        f"({sorted(expected_types)})",
                     )
 
             result_list.append(
                 Result(BaseCheck.MEDIUM, pass_stat, global_att_name, messages),
             )
 
         return result_list
@@ -1298,17 +1286,15 @@
 
         platform_set = set()
         for v in ds.get_variables_by_attributes(platform=lambda x: x is not None):
             platform_set.add(v.getncattr("platform"))
 
         num_platforms = len(platform_set)
         if num_platforms > 1 and glb_platform:
-            msg = "A dataset may only have one platform; {} found".format(
-                len(platform_set),
-            )
+            msg = f"A dataset may only have one platform; {len(platform_set)} found"
             val = False
 
         elif (not glb_platform) and num_platforms > 0:
             msg = 'If a platform variable exists, a global attribute "platform" must also exist'
             val = False
 
         elif num_platforms == 0 and glb_platform:
@@ -1324,15 +1310,15 @@
 
         return Result(BaseCheck.HIGH, val, "platform", None if val else [msg])
 
     def check_platform_vocabulary(self, ds):
         """
         The platform_vocabulary attribute is recommended to be a URL to
         https://mmisw.org/ont/ioos/platform or
-        http://vocab.nerc.ac.uk/collection/L06/current/. However,
+        https://vocab.nerc.ac.uk/collection/L06/current/. However,
         it is required to at least be a URL.
 
         Args:
             ds (netCDF4.Dataset): open Dataset
 
         Returns:
             Result
@@ -1401,22 +1387,22 @@
                 pass_stat = units.definition in unit_def_set
             # unknown unit not convertible to UDUNITS
             except ValueError:
                 pass_stat = False
 
             valid_vertical_coord = TestCtx(BaseCheck.HIGH, "Vertical coordinates")
             units_set_msg = (
-                "{}'s units attribute {} is not equivalent to one "
-                "of {}".format(name, units_str, expected_unit_strs)
+                f"{name}'s units attribute {units_str} is not equivalent to one "
+                f"of {expected_unit_strs}"
             )
             valid_vertical_coord.assert_true(pass_stat, units_set_msg)
 
             pos_msg = (
-                "{}: vertical coordinates must include a positive "
-                "attribute that is either 'up' or 'down'".format(name)
+                f"{name}: vertical coordinates must include a positive "
+                "attribute that is either 'up' or 'down'"
             )
             valid_vertical_coord.assert_true(positive in ("up", "down"), pos_msg)
 
             ret_val.append(valid_vertical_coord.to_result())
 
         return ret_val
 
@@ -1554,20 +1540,22 @@
                 y[0] for y in filter(lambda x: not x[1], var_passed_ingest_reqs)
             )
 
         return Result(
             BaseCheck.HIGH,
             False,  # always fail
             "NDBC/GTS Ingest Requirements",
-            [var_passed_ingest_msg.format(", ".join(_var_passed))]
-            if all_passed_ingest_reqs
-            else [
-                var_passed_ingest_msg.format(", ".join(_var_passed)),
-                var_failed_ingest_msg.format(", ".join(_var_failed)),
-            ],
+            (
+                [var_passed_ingest_msg.format(", ".join(_var_passed))]
+                if all_passed_ingest_reqs
+                else [
+                    var_passed_ingest_msg.format(", ".join(_var_passed)),
+                    var_failed_ingest_msg.format(", ".join(_var_failed)),
+                ]
+            ),
         )
 
     def check_instrument_variables(self, ds):
         """
         If present, the instrument_variable is one that contains additional
         metadata about the instrument the data was collected with.
 
@@ -1582,18 +1570,15 @@
         instr_vars = get_instrument_variables(ds)
 
         # check for component, disciminant
         for instr in instr_vars:
             if instr in ds.variables:
                 compnt = getattr(ds.variables[instr], "component", None)
                 m = [
-                    "component attribute of {} ({}) must be a string".format(
-                        instr,
-                        compnt,
-                    ),
+                    f"component attribute of {instr} ({compnt}) must be a string",
                 ]
                 if compnt:
                     results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             isinstance(compnt, str),
                             "instrument_variable",
@@ -1603,18 +1588,15 @@
                 else:
                     results.append(
                         Result(BaseCheck.MEDIUM, True, "instrument_variable", m),
                     )
 
                 disct = getattr(ds.variables[instr], "discriminant", None)
                 m = [
-                    "discriminant attribute of {} ({}) must be a string".format(
-                        instr,
-                        disct,
-                    ),
+                    f"discriminant attribute of {instr} ({disct}) must be a string",
                 ]
                 if disct:
                     results.append(
                         Result(
                             BaseCheck.MEDIUM,
                             isinstance(disct, str),
                             "instrument_variable",
@@ -1702,22 +1684,20 @@
         results = []
         for v in ds.get_variables_by_attributes(
             standard_name=lambda x: x in self._qartod_std_names,
         ):
             attval = getattr(v, "references", None)
             if attval is None:
                 msg = (
-                    '"references" attribute not present for variable {}.'
+                    f'"references" attribute not present for variable {v.name}.'
                     "If present, it should be a valid URL."
-                ).format(v.name)
+                )
                 val = False
             else:
-                msg = '"references" attribute for variable "{}" must be a valid URL'.format(
-                    v.name,
-                )
+                msg = f'"references" attribute for variable "{v.name}" must be a valid URL'
                 val = bool(validators.url(attval))
 
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     val,
                     "qartod_variable:references",
@@ -1783,17 +1763,19 @@
 
             valid = isinstance(mm, str)
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     valid,
                     "instrument_variable:make_model",
-                    None
-                    if valid
-                    else [f"Attribute {v}:make_model ({mm}) should be a string"],
+                    (
+                        None
+                        if valid
+                        else [f"Attribute {v}:make_model ({mm}) should be a string"]
+                    ),
                 ),
             )
 
             # calibration_date
             cd = getattr(_v, "calibration_date", "")
             # thanks folks https://stackoverflow.com/questions/41129921/validate-an-iso-8601-datetime-string-in-python
             valid = bool(
@@ -1803,19 +1785,21 @@
                 ),
             )
             results.append(
                 Result(
                     BaseCheck.MEDIUM,
                     valid,
                     "instrument_variable:calibration_date",
-                    None
-                    if valid
-                    else [
-                        f"Attribute {v}:calibration_date ({cd}) should be an ISO-8601 string",
-                    ],
+                    (
+                        None
+                        if valid
+                        else [
+                            f"Attribute {v}:calibration_date ({cd}) should be an ISO-8601 string",
+                        ]
+                    ),
                 ),
             )
 
         return results
 
 
 class IOOSBaseSOSCheck(BaseCheck):
```

### Comparing `compliance-checker-5.1.0/compliance_checker/protocols/cdl.py` & `compliance_checker-5.1.1/compliance_checker/protocols/cdl.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/protocols/netcdf.py` & `compliance_checker-5.1.1/compliance_checker/protocols/netcdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 def is_netcdf(url):
     """
     Returns True if the URL points to a valid local netCDF file
 
     :param str url: Location of file on the file system
     """
     # Try an obvious exclusion of remote resources
+    url = str(url)
     if url.startswith("http"):
         return False
 
     # If it's a known extension, give it a shot
     if url.endswith("nc"):
         return True
 
@@ -86,10 +87,14 @@
             f"Received exception when making HEAD request to {ds_str}: {e}",
             stacklevel=2,
         )
         content_type = None
     else:
         content_type = head_req.headers.get("content-type")
 
+    if content_type is None:
+        return False
+
     # if the Content-Type header returned was "application/x-netcdf",
     # or a netCDF file (not OPeNDAP) we can open this into a Dataset
-    return content_type == "application/x-netcdf"
+    # Add support for application/x-netcdf;ver=4
+    return content_type.split(";")[0] == "application/x-netcdf"
```

### Comparing `compliance-checker-5.1.0/compliance_checker/protocols/opendap.py` & `compliance_checker-5.1.1/compliance_checker/protocols/opendap.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/runner.py` & `compliance_checker-5.1.1/compliance_checker/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,35 +103,29 @@
                 if output_filename == "-":
                     cls.stdout_output(cs, score_dict, verbose, limit)
                 # need to redirect output from stdout since print functions are
                 # presently used to generate the standard report output
                 else:
                     if len(output_format) > 1:
                         # Update file name if needed
-                        output_filename = "{}.txt".format(
-                            os.path.splitext(output_filename)[0],
-                        )
+                        output_filename = f"{os.path.splitext(output_filename)[0]}.txt"
                     with open(output_filename, "w", encoding="utf-8") as f:
                         with stdout_redirector(f):
                             cls.stdout_output(cs, score_dict, verbose, limit)
 
             elif out_fmt == "html":
                 # Update file name if needed
                 if len(output_format) > 1 and output_filename != "-":
-                    output_filename = "{}.html".format(
-                        os.path.splitext(output_filename)[0],
-                    )
+                    output_filename = f"{os.path.splitext(output_filename)[0]}.html"
                 cls.html_output(cs, score_dict, output_filename, ds_loc, limit)
 
             elif out_fmt in {"json", "json_new"}:
                 # Update file name if needed
                 if len(output_format) > 1 and output_filename != "-":
-                    output_filename = "{}.json".format(
-                        os.path.splitext(output_filename)[0],
-                    )
+                    output_filename = f"{os.path.splitext(output_filename)[0]}.json"
                 cls.json_output(cs, score_dict, output_filename, ds_loc, limit, out_fmt)
 
             else:
                 raise TypeError("Invalid format %s" % out_fmt)
 
             errors_occurred = cls.check_errors(score_groups, verbose)
```

### Comparing `compliance-checker-5.1.0/compliance_checker/suite.py` & `compliance_checker-5.1.1/compliance_checker/suite.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 import re
 import subprocess
 import sys
 import textwrap
 import warnings
 from collections import defaultdict
 from datetime import datetime, timezone
-from distutils.version import StrictVersion
 from operator import itemgetter
 from pathlib import Path
 from urllib.parse import urlparse
 
+import importlib_metadata
 import requests
 from lxml import etree as ET
 from netCDF4 import Dataset
 from owslib.sos import SensorObservationService
 from owslib.swe.sensor.sml import SensorML
-from pkg_resources import working_set
+from packaging.version import parse
 
-from compliance_checker import MemoizedDataset, __version__, tempnc
+from compliance_checker import __version__, tempnc
 from compliance_checker.base import BaseCheck, GenericFile, Result, fix_return_value
 from compliance_checker.protocols import cdl, netcdf, opendap
 
 # Ensure output is encoded as Unicode when checker output is redirected or piped
 if sys.stdout.encoding is None:
     sys.stdout = codecs.getwriter("utf8")(sys.stdout)
 if sys.stderr.encoding is None:
@@ -69,16 +69,18 @@
     def _get_generator_plugins(cls):
         """
         Return a list of classes from external plugins that are used to
         generate checker classes
         """
 
         if not hasattr(cls, "suite_generators"):
-            gens = working_set.iter_entry_points("compliance_checker.generators")
-            cls.suite_generators = [x.resolve() for x in gens]
+            gens = importlib_metadata.entry_points(
+                group="compliance_checker.generators",
+            )
+            cls.suite_generators = [x.load() for x in gens]
 
         return cls.suite_generators
 
     def _print_suites(self, verbose=0):
         """
         Prints out available check suites.  If the verbose argument is True,
         includes the internal module version number of the check and also displays
@@ -132,26 +134,28 @@
 
     @classmethod
     def load_all_available_checkers(cls):
         """
         Helper method to retrieve all sub checker classes derived from various
         base classes.
         """
-        cls._load_checkers(working_set.iter_entry_points("compliance_checker.suites"))
+        cls._load_checkers(
+            importlib_metadata.entry_points(group="compliance_checker.suites"),
+        )
 
     @classmethod
     def _load_checkers(cls, checkers):
         """
         Loads up checkers in an iterable into the class checkers dict
         :param checkers: An iterable containing the checker objects
         """
 
         for c in checkers:
             try:
-                check_obj = c.resolve()
+                check_obj = c.load()
                 if hasattr(check_obj, "_cc_spec") and hasattr(
                     check_obj,
                     "_cc_spec_version",
                 ):
                     check_version_str = ":".join(
                         (check_obj._cc_spec, check_obj._cc_spec_version),
                     )
@@ -182,17 +186,16 @@
                 print("Could not load", c, ":", e, file=sys.stderr)
         # find the latest version of versioned checkers and set that as the
         # default checker for compliance checker if no version is specified
         ver_checkers = sorted([c.split(":", 1) for c in cls.checkers if ":" in c])
         for spec, versions in itertools.groupby(ver_checkers, itemgetter(0)):
             version_nums = [v[-1] for v in versions]
             try:
-                latest_version = str(max(StrictVersion(v) for v in version_nums))
-            # if the version can't be parsed as a StrictVersion, parse
-            # according to character collation
+                latest_version = str(max(parse(v) for v in version_nums))
+            # if the version can't be parsed, do it according to character collation
             except ValueError:
                 latest_version = max(version_nums)
             cls.checkers[spec] = cls.checkers[spec + ":latest"] = cls.checkers[
                 ":".join((spec, latest_version))
             ]
 
     def _get_checks(self, checkclass, include_checks, skip_checks):
@@ -342,19 +345,16 @@
             if len(split_check_spec) < 2:
                 check_max_level = BaseCheck.HIGH
             else:
                 try:
                     check_max_level = check_lookup[split_check_spec[1]]
                 except KeyError:
                     warnings.warn(
-                        "Skip specifier '{}' on check '{}' not found,"
-                        " defaulting to skip entire check".format(
-                            split_check_spec[1],
-                            check_name,
-                        ),
+                        f"Skip specifier '{split_check_spec[1]}' on check '{check_name}' not found,"
+                        " defaulting to skip entire check",
                         stacklevel=2,
                     )
                     check_max_level = BaseCheck.HIGH
 
             check_dict[check_name] = check_max_level
 
         return check_dict
@@ -640,19 +640,15 @@
         print(f"{check_name}".center(width))
         print(f"{check_url}".center(width))
         print("-" * width)
         if issue_count > 0:
             print("Corrective Actions".center(width))
             plural = "" if issue_count == 1 else "s"
             print(
-                "{} has {} potential issue{}".format(
-                    os.path.basename(ds),
-                    issue_count,
-                    plural,
-                ),
+                f"{os.path.basename(ds)} has {issue_count} potential issue{plural}",
             )
 
         return [groups, points, out_of]
 
     def standard_output_generation(self, groups, limit, points, out_of, check):
         """
         Generates the Terminal Output
@@ -768,20 +764,17 @@
         Use ncgen to generate a netCDF file from a .cdl file
         Returns the path to the generated netcdf file. If ncgen fails, uses
         sys.exit(1) to terminate program so a long stack trace is not reported
         to the user.
 
         :param str cdl_path: Absolute path to cdl file that is used to generate netCDF file
         """
-        if (
-            ".cdl" in cdl_path
-        ):  # it's possible the filename doesn't have the .cdl extension
-            ds_str = cdl_path.replace(".cdl", ".nc")
-        else:
-            ds_str = cdl_path + ".nc"
+        if isinstance(cdl_path, str):
+            cdl_path = Path(cdl_path)
+        ds_str = cdl_path.with_suffix(".nc")
 
         # generate netCDF-4 file
         iostat = subprocess.run(
             ["ncgen", "-k", "nc4", "-o", ds_str, cdl_path],
             stderr=subprocess.PIPE,
         )
         if iostat.returncode != 0:
@@ -824,23 +817,23 @@
         else:
             return self.load_local_dataset(ds_str)
 
     def check_remote_netcdf(self, ds_str):
         if netcdf.is_remote_netcdf(ds_str):
             response = requests.get(ds_str, allow_redirects=True, timeout=60)
             try:
-                return MemoizedDataset(
+                return Dataset(
                     urlparse(response.url).path,
                     memory=response.content,
                 )
             except OSError:
                 # handle case when netCDF C libs weren't compiled with
                 # in-memory support by using tempfile
                 with tempnc(response.content) as _nc:
-                    return MemoizedDataset(_nc)
+                    return Dataset(_nc)
 
     def load_remote_dataset(self, ds_str):
         """
         Returns a dataset instance for the remote resource, either OPeNDAP or SOS
 
         :param str ds_str: URL to the remote resource
         """
@@ -874,14 +867,19 @@
         # we'll attempt to parse the response as SOS.
         # Some SOS servers don't seem to support HEAD requests.
         # Issue GET instead if we reach here and can't get the response
         response = requests.get(ds_str, allow_redirects=True, timeout=60)
         content_type = response.headers.get("content-type")
         if content_type.split(";")[0] == "text/xml":
             return self.process_doc(response.content)
+        elif content_type.split(";")[0] == "application/x-netcdf":
+            return Dataset(
+                urlparse(response.url).path,
+                memory=response.content,
+            )
         else:
             raise ValueError(
                 f"Unknown service with content-type: {content_type}",
             )
 
     def load_local_dataset(self, ds_str):
         """
@@ -889,15 +887,15 @@
 
         :param ds_str: Path to the resource
         """
         if cdl.is_cdl(ds_str):
             ds_str = self.generate_dataset(ds_str)
 
         if netcdf.is_netcdf(ds_str):
-            return MemoizedDataset(ds_str)
+            return Dataset(ds_str)
 
         # Assume this is just a Generic File if it exists
         if os.path.isfile(ds_str):
             return GenericFile(ds_str)
 
         raise ValueError("File is an unknown format")
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/__init__.py` & `compliance_checker-5.1.1/compliance_checker/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+from pathlib import Path
 
 from netCDF4 import Dataset
 
 
 class BaseTestCase(unittest.TestCase):
     """
     Base test case compliance checker unit tests
@@ -21,16 +22,16 @@
 
     __str__ = __repr__
 
     def load_dataset(self, nc_dataset):
         """
         Return a loaded NC Dataset for the given path
         """
-        if not isinstance(nc_dataset, str):
-            raise ValueError("nc_dataset should be a string")
+        if not isinstance(nc_dataset, (str, Path)):
+            raise ValueError("nc_dataset should be a valid path")
 
         nc_dataset = Dataset(nc_dataset, "r")
         self.addCleanup(nc_dataset.close)
         return nc_dataset
 
     def assert_result_is_good(self, result):
         if isinstance(result.value, bool):
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/cassettes/test_netcdf_content_type.yaml` & `compliance_checker-5.1.1/compliance_checker/tests/cassettes/test_netcdf_content_type.yaml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/conftest.py` & `compliance_checker-5.1.1/compliance_checker/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import subprocess
 from itertools import chain
-from pathlib import Path
 
 import pytest
+from importlib_resources import files
 from netCDF4 import Dataset
-from pkg_resources import resource_filename
 
 from compliance_checker.cf import util
 from compliance_checker.suite import CheckSuite
 
 
 def glob_down(pth, suffix, lvls):
     """globs down up to (lvls: int) levels of subfolders\n
@@ -23,15 +22,15 @@
 
 
 def static_files(cdl_stem):
     """
     Returns the Path to a valid nc dataset\n
     replaces the old STATIC_FILES dict
     """
-    datadir = Path(resource_filename("compliance_checker", "tests/data")).resolve()
+    datadir = files("compliance_checker").joinpath("tests/data").resolve()
     assert datadir.exists(), f"{datadir} not found"
 
     cdl_paths = glob_down(datadir, f"{cdl_stem}.cdl", 3)
     assert (
         len(cdl_paths) > 0
     ), f"No file named {cdl_stem}.cdl found in {datadir} or its subfolders"
     assert (
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/20160919092000-ABOM-L3S_GHRSST-SSTfnd-AVHRR_D-1d_dn_truncate.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/2d-regular-grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/2d-regular-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/2dim-grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/2dim-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/3d-regular-grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/3d-regular-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/3d-static-grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/3d-static-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/NCEI_profile_template_v2.0_2016-09-22_181835.151325.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/point.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/point.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-non-static.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/appendix_h/timeseries-single.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/appendix_h/timeseries-single.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad-instance.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad-instance.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad-instance.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad-trajectory.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad-trajectory.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad-trajectory.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure1.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure1.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cell_measure2.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cell_measure2.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cf_role.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_cf_role.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_cf_role.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_data_type.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_data_type.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_data_type.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_missing_data.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_missing_data.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_missing_data.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_region.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_region.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_region.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_units.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/bad_units.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/bad_units.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/cell_measure.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/cell_measure.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/cf_example_cell_measures.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/cf_example_cell_measures.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/chap2.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/chap2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/climatology.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/climatology.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/cont_ragged.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/cont_ragged.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/coordinate_types.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/coordinate_types.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/dimension_order.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/dimension_order.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/duplicate_axis.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/duplicate_axis.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/example-grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/example-grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/3mf07.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/3mf07.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/bio_taxa.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/bio_taxa.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/cf_example_cell_measures.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/fvcom.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/fvcom.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/glcfs.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/glcfs.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/hycom_global.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/hycom_global.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/kibesillah.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/kibesillah.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/l01-met.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/l01-met.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ocos.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/ocos.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ooi_glider.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/ooi_glider.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/pr_inundation.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/pr_inundation.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/sldmb_43093_agg.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/sp041.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/sp041.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/swan.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/swan.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/usgs_dem_saipan.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/examples/ww3.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/examples/ww3.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/forecast_reference.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/forecast_reference.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/grid-boundaries.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/grid-boundaries.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/grid_mapping_coordinates.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/grid_mapping_coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml` & `compliance_checker-5.1.1/compliance_checker/tests/data/http_mocks/ncsos_describesensor.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml` & `compliance_checker-5.1.1/compliance_checker/tests/data/http_mocks/ncsos_getcapabilities.xml`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/illegal-aux-coords.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/illegal-aux-coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/index_ragged2.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/index_ragged2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/ioos_1_1.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/ioos_1_1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/line_geometry.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/line_geometry.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/mapping.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/mapping.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/multi-dim-coordinates.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/multi-dim-coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-incomplete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/multi-timeseries-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_1.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_1.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/ncei_gold_point_2.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/ncei_gold_point_2.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/1d_bound_bad.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad-rhgrid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bad2dim.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bad2dim.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bounds_bad_num_coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/bounds_bad_order.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/non-comp/self_referencing.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/non-comp/self_referencing.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/point.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/point.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/polygon_geometry.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/polygon_geometry.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/profile-incomplete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/profile-orthogonal.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/profile-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/reduced_horizontal_grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/reduced_horizontal_grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/rotated_pole_grid.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/rotated_pole_grid.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/ru07-20130824T170228_rt0.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/self-referencing-var.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/self-referencing-var.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/taxonomy_example.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/taxonomy_example.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc4_file.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc4_file.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc_file.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/test_cdl_nc_file.nc` & `compliance_checker-5.1.1/compliance_checker/tests/data/test_cdl_nc_file.nc`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-incomplete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-ortho-time.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-multi-station.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-multi-station.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-ortho-depth.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-ortho-time.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries-profile-single-station.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries-profile-single-station.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/timeseries.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/timeseries.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-complete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-complete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-implied.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-implied.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-incomplete.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-incomplete.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-profile-orthogonal.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory-single.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory-single.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/trajectory.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/trajectory.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/units_check.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/units_check.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/valid_coordinates.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/valid_coordinates.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/data/vertical_coords.cdl` & `compliance_checker-5.1.1/compliance_checker/tests/data/vertical_coords.cdl`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/helpers.py` & `compliance_checker-5.1.1/compliance_checker/tests/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tempfile
 
-from netCDF4 import Dataset
+from netCDF4._netCDF4 import Dataset
 
 
 class MockNetCDF(Dataset):
     """
     Wrapper object around NetCDF Dataset to write data only to memory.
     """
 
@@ -19,14 +19,22 @@
         super().__init__(
             temp_filename,
             "w",
             diskless=True,
             persist=False,
         )
 
+    # suppress usual dealloc routine to prevent caught exception messages
+    # from printing
+    def __dealloc__(self):
+        try:
+            super().__dealloc__()
+        except AttributeError:
+            pass
+
 
 class MockTimeSeries(MockNetCDF):
     """
     Mock time series with time dimension and time, lon, lat, and depth
     variables defined
     """
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/resources.py` & `compliance_checker-5.1.1/compliance_checker/tests/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import os
 import subprocess
 
-from pkg_resources import resource_filename
+from importlib_resources import files
 
 
 def get_filename(path):
     """
     Returns the path to a valid dataset
     """
-    filename = resource_filename("compliance_checker", path)
-    nc_path = filename.replace(".cdl", ".nc")
-    if not os.path.exists(nc_path):
+    filename = files("compliance_checker") / path
+    nc_path = filename.with_suffix(".nc")
+    if not nc_path.exists():
         generate_dataset(filename, nc_path)
     return nc_path
 
 
 def generate_dataset(cdl_path, nc_path):
     subprocess.call(["ncgen", "-4", "-o", nc_path, cdl_path])
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_acdd.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_acdd.py`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,15 @@
         # and the value that was provided for easy troubleshooting
         empty_ds.geospatial_bounds = "POIT (-123.458000 38.048000)"
         results = self.acdd.check_recommended(empty_ds)
         for result in results:
             if result.variable_name == "geospatial_bounds":
                 assert (
                     "Could not parse WKT from geospatial_bounds,"
-                    ' possible bad value: "{}"'.format(empty_ds.geospatial_bounds)
+                    f' possible bad value: "{empty_ds.geospatial_bounds}"'
                     in result.msgs
                 )
 
     def test_time_extents(self):
         """
         Test that the time extents are being checked
         """
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_base.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_cf.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_cf.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         ds = MockTimeSeries()
         ds.createDimension("siglev", 20)
 
         temp = ds.createVariable(
             "temp",
             np.float64,
             dimensions=("time",),
-            fill_value=float(99999999999999999999.0),
+            fill_value=99999999999999999999.0,
         )
         temp.coordinates = "sigma noexist"
         ds.createVariable("sigma", np.float64, dimensions=("siglev",))
         self.cf.setup(ds)
         # time is a NUG coordinate variable, sigma is not, but is referred to in
         # variables, so both should show up in cf_coord_data_vars.
         # noexist does not exist in the dataset's variables, so it is not
@@ -189,15 +189,15 @@
         # delete the dataset and start over to create the variable with _FillValue at time of creation
         del ds
         ds = MockTimeSeries()
         ds.createVariable(
             "temp",
             np.float64,
             dimensions=("time",),
-            fill_value=float(99999999999999999999.0),
+            fill_value=99999999999999999999.0,
         )
 
         # give temp _FillValue as a float, expect good result
         result = self.cf.check_child_attr_data_types(ds)
         self.assert_result_is_good(result)
 
         # give temp valid_range as an array of floats, all should check out
@@ -392,15 +392,15 @@
         expected_msgs = [
             f"For the variable {v_name} the missing_value must be equal to the _FillValue"
             for v_name in ("a")
         ]
 
         assert result.msgs == expected_msgs
 
-    def test_check_valid_range_or_valid_min_max_present(self):
+    def test_check_valid_range_and_valid_min_max_present(self):
         """
         2.5.1 Missing data, valid and actual range of data
         Requirements:
         The valid_range attribute must not be present if the
         valid_min and/or valid_max attributes are present.
         """
         # TEST CONFORMANCE 2.5.1 REQUIRED
@@ -422,25 +422,25 @@
 
         # Case of valid_min and valid_max are absent and valid_range is present
         dataset.createVariable("c", "d", ("time",), fill_value=9999.9)
         dataset.variables["c"][0] = 1
         dataset.variables["c"][1] = 2
         dataset.variables["c"].setncattr("valid_range", [-10, 10])
 
-        result = self.cf.check_valid_range_or_valid_min_max_present(dataset)
+        result = self.cf.check_valid_range_and_valid_min_max_present(dataset)
 
         # check if the test fails when when variable "a" is checked.
         expected_msgs = [
             f"For the variable {v_name} the valid_range attribute must not be present "
             f"if the valid_min and/or valid_max attributes are present"
             for v_name in ("a")
         ]
 
         assert result.msgs == expected_msgs
-        assert result.value[0] == result.value[1]
+        assert result.value[0] < result.value[1]
 
     def test_check_fill_value_outside_valid_range(self):
         """
         2.5.1 The _FillValue should be outside the range specified by valid_range (if used) for a variable.
         """
         # TEST CONFORMANCE 2.5.1 REQUIRED
         dataset = self.load_dataset(STATIC_FILES["bad_data_type"])
@@ -1296,17 +1296,15 @@
         assert "time does not have correct time units" in messages
         assert (scored, out_of) == (1, 2)
         # TEST CONFORMANCE 4.4 REQUIRED 2/2, RECOMMENDED 1, 2/2
         dataset = MockTimeSeries()
         # NB: >= 60 seconds is nonstandard, but isn't actually a CF requirement
         # until CF 1.9 onwards
         dataset.variables["time"].units = "months since 0-1-1 23:00:60"
-        dataset.variables[
-            "time"
-        ].climatology = (
+        dataset.variables["time"].climatology = (
             "nonexistent_variable_reference_only_used_to_test_year_zero_failure"
         )
         results = self.cf.check_time_coordinate(dataset)
         scored, out_of, messages = get_results(results)
         assert scored < out_of
         assert (
             "Using relative time interval of months or years is not recommended for coordinate variable time"
@@ -1792,15 +1790,16 @@
         assert len([r for r in results if r.value[0] < r.value[1]]) == 2
         assert all(r.name == "§5 Coordinate Systems" for r in results)
 
     def test_64bit(self):
         dataset = self.load_dataset(STATIC_FILES["ints64"])
         suite = CheckSuite()
         suite.checkers = {"cf": CF1_6Check}
-        suite.run(dataset, "cf")
+        # suite.run(dataset, "cf")
+        suite.run_all(dataset, ["cf"], skip_checks=["cf"])
 
     def test_variable_feature_check(self):
         # non-compliant dataset -- 1/1 fail
         dataset = self.load_dataset(STATIC_FILES["bad-trajectory"])
         results = self.cf.check_variable_features(dataset)
         scored, out_of, messages = get_results(results)
         assert len(results) == 2
@@ -2812,15 +2811,15 @@
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertTrue(r[1].value)
         self.assertFalse(r[1].msgs)
 
         # set same dtype
         dataset = MockTimeSeries()  # time lat lon depth
         temp = dataset.createVariable("temp", int, dimensions=("time",))
-        temp.setncattr("scale_factor", int(5))
+        temp.setncattr("scale_factor", 5)
         r = self.cf.check_add_offset_scale_factor_type(dataset)
         self.assertTrue(r[1].value)
         self.assertFalse(r[1].msgs)
 
         # integer variable type (int8, int16, int32) compared against
         # floating point add_offset/scale_factor
         for var_bytes in ("1", "2", "4"):
@@ -2948,17 +2947,17 @@
                 text="<html><head><title>400 Bad Request</head><body><h1>Bad Request</h1><p>Unknown LSID</p></body></html>",
             )
             results = self.cf.check_taxa(dataset)
             assert len(results) == 1
             messages = results[0].msgs
             assert results[0].value[0] < results[0].value[1]
             assert len(messages) == 1
-            taxon_lsid[
-                0
-            ] = "http://www.lsid.info/urn:lsid:marinespecies.org:taxname:99999999999"
+            taxon_lsid[0] = (
+                "http://www.lsid.info/urn:lsid:marinespecies.org:taxname:99999999999"
+            )
             results = self.cf.check_taxa(dataset)
             assert messages[0].startswith(
                 "Taxon id must match one of the following forms:",
             )
             assert results[0].value[0] < results[0].value[1]
 
     def test_taxonomy_data_worms_valid(self):
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_cf_integration.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_cf_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,15 @@
     (
         "sldmb_43093_agg",
         [
             "attribute time:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "attribute lat:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "attribute lon:_CoordianteAxisType should begin with a letter and be composed of letters, digits, and underscores",
             "§2.6.2 global attribute history should exist and be a non-empty string",
-            "standard_name temperature is not defined in Standard Name Table v{}. Possible close match(es): ['air_temperature', 'soil_temperature', 'snow_temperature']".format(
-                std_names._version,
-            ),
+            f"standard_name temperature is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['air_temperature', 'soil_temperature', 'snow_temperature']",
             "temperature's auxiliary coordinate specified by the coordinates attribute, precise_lat, is not a variable in this dataset",
             "temperature's auxiliary coordinate specified by the coordinates attribute, precise_lon, is not a variable in this dataset",
         ],
     ),
     (
         "usgs_dem_saipan",
         ['§2.6.1 Conventions global attribute does not contain "CF-1.8"'],
@@ -41,38 +39,26 @@
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_gust_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.float64'>) and parent variable 'wind_speed' (type: <class 'numpy.float32'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_speed_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.float64'>) and parent variable 'wind_direction' (type: <class 'numpy.float32'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'wind_direction_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             "Attribute 'valid_range' (type: <class 'numpy.int16'>) and parent variable 'visibility_qc' (type: <class 'numpy.int8'>) must have equivalent datatypes",
             '§2.6.1 Conventions global attribute does not contain "CF-1.8"',
-            "standard_name visibility is not defined in Standard Name Table v{}. Possible close match(es): ['visibility_in_air']".format(
-                std_names._version,
-            ),
+            f"standard_name visibility is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['visibility_in_air']",
             'Standard name modifier "data_quality" for variable visibility_qc is not a valid modifier according to CF Appendix C',
-            "standard_name wind_direction is not defined in Standard Name Table v{}. Possible close match(es): ['wind_to_direction', 'wind_from_direction', 'wind_gust_from_direction']".format(
-                std_names._version,
-            ),
+            f"standard_name wind_direction is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['wind_to_direction', 'wind_from_direction', 'wind_gust_from_direction']",
             'Standard name modifier "data_quality" for variable wind_direction_qc is not a valid modifier according to CF Appendix C',
-            "standard_name wind_gust is not defined in Standard Name Table v{}. Possible close match(es): ['y_wind_gust', 'x_wind_gust', 'wind_speed_of_gust']".format(
-                std_names._version,
-            ),
+            f"standard_name wind_gust is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['y_wind_gust', 'x_wind_gust', 'wind_speed_of_gust']",
             'Standard name modifier "data_quality" for variable wind_gust_qc is not a valid modifier according to CF Appendix C',
             'Standard name modifier "data_quality" for variable air_temperature_qc is not a valid modifier according to CF Appendix C',
-            "standard_name use_wind is not defined in Standard Name Table v{}. Possible close match(es): ['y_wind', 'x_wind']".format(
-                std_names._version,
-            ),
-            "standard_name barometric_pressure is not defined in Standard Name Table v{}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']".format(
-                std_names._version,
-            ),
+            f"standard_name use_wind is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['y_wind', 'x_wind']",
+            f"standard_name barometric_pressure is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']",
             'Standard name modifier "data_quality" for variable barometric_pressure_qc is not a valid modifier according to CF Appendix C',
             'Standard name modifier "data_quality" for variable wind_speed_qc is not a valid modifier according to CF Appendix C',
-            "standard_name barometric_pressure is not defined in Standard Name Table v{}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']".format(
-                std_names._version,
-            ),
+            f"standard_name barometric_pressure is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['air_pressure', 'reference_pressure', 'barometric_altitude']",
             "CF recommends latitude variable 'lat' to use units degrees_north",
             "CF recommends longitude variable 'lon' to use units degrees_east",
         ],
     ),
     ("sp041", ["lat_qc is not a variable in this dataset"]),
     (
         "3mf07",
@@ -147,20 +133,16 @@
         ],
     ),
     (
         "glcfs",
         [
             # TODO: referenced/relative time is treated like time units
             'Units "hours since 2016-01-01T12:00:00Z" for variable time_offset must be convertible to canonical units "s"',
-            "standard_name cloud_cover is not defined in Standard Name Table v{}. Possible close match(es): ['land_cover', 'land_cover_lccs', 'cloud_albedo']".format(
-                std_names._version,
-            ),
-            "standard_name dew_point is not defined in Standard Name Table v{}. Possible close match(es): ['dew_point_depression', 'dew_point_temperature']".format(
-                std_names._version,
-            ),
+            f"standard_name cloud_cover is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['land_cover', 'land_cover_lccs', 'cloud_albedo']",
+            f"standard_name dew_point is not defined in Standard Name Table v{std_names._version}. Possible close match(es): ['dew_point_depression', 'dew_point_temperature']",
             (
                 "GRID is not a valid CF featureType. It must be one of point, timeseries, "
                 "trajectory, profile, timeseriesprofile, trajectoryprofile"
             ),
             (
                 "global attribute _CoordSysBuilder should begin with a letter and "
                 "be composed of letters, digits, and underscores"
@@ -259,15 +241,16 @@
         "loaded_dataset,expected_messages",
         dataset_stem__expected_messages,
         indirect=[
             "loaded_dataset",
         ],  # must be specified to load this param at runtime, instead of at collection
     )
     def test_cf_integration(self, loaded_dataset, expected_messages, cs):
-        check_results = cs.run(loaded_dataset, [], "cf")
+        # check_results = cs.run(loaded_dataset, [], "cf")
+        check_results = cs.run_all(loaded_dataset, ["cf"], skip_checks=[])
         scored, out_of, messages = self.get_results(check_results, cs)
 
         assert scored < out_of
 
         assert all(m in messages for m in expected_messages), mult_msgs_diff.format(
             missing_msgs="\n".join([m for m in expected_messages if m not in messages]),
             found_msgs="\n".join(messages),
@@ -284,22 +267,24 @@
         [
             ("index_ragged2", "are not a subset of dimensions for variable"),
             ("index_ragged2", "Unidentifiable feature for variable"),
         ],
         indirect=["loaded_dataset"],
     )
     def test_no_incorrect_errors(self, cs, loaded_dataset, wrong_message):
-        check_results = cs.run(loaded_dataset, [], True, "cf")
+        # check_results = cs.run(loaded_dataset, [], True, "cf")
+        check_results = cs.run_all(loaded_dataset, ["cf"], skip_checks=[])
         messages = self.get_results(check_results, cs)[-1]
 
         assert wrong_message not in "".join(messages)
 
     @pytest.mark.parametrize("loaded_dataset", ["fvcom"], indirect=True)
     def test_fvcom(self, cs, loaded_dataset):
-        check_results = cs.run(loaded_dataset, [], True, "cf")
+        # check_results = cs.run(loaded_dataset, [], True, "cf")
+        check_results = cs.run_all(loaded_dataset, ["cf"], skip_checks=[])
         scored, out_of, messages = self.get_results(check_results, cs)
         assert scored < out_of
 
         for msg in messages:
             if msg.startswith("dimensions for auxiliary coordinate variable siglay"):
                 break
         # it's not clear to me what this is supposed to be doing -- this else clause is outside of the if
@@ -319,10 +304,11 @@
         indirect=True,
     )
     def test_ncei_templates(self, cs, loaded_dataset):
         """
         Tests some of the NCEI NetCDF templates, which usually should get a
         perfect score.
         """
-        check_results = cs.run(loaded_dataset, [], "cf")
+        # check_results = cs.run(loaded_dataset, [], "cf")
+        check_results = cs.run_all(loaded_dataset, ["cf"], skip_checks=[])
         scored, out_of, messages = self.get_results(check_results, cs)
         assert scored < out_of
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_cli.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         def checker_1():
             return Namespace(name="checker_1")
 
         def checker_2():
             return Namespace(_cc_spec="checker_2", _cc_spec_version="2.2")
 
-        mock_checkers = [Namespace(resolve=checker_1), Namespace(resolve=checker_2)]
+        mock_checkers = [Namespace(load=checker_1), Namespace(load=checker_2)]
         with pytest.warns(DeprecationWarning):
             CheckSuite._load_checkers(mock_checkers)
 
         cs = CheckSuite()
         saved = sys.stdout
         try:
             # ugly!  consider refactoring to use py.test capsys
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_feature_detection.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_feature_detection.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 
     def test_timeseries(self):
         """
         Ensures timeseries detection works
         """
         with Dataset(resources.STATIC_FILES["timeseries"]) as nc:
             for variable in util.get_geophysical_variables(nc):
-                assert util.is_timeseries(nc, variable), "{} is timeseries".format(
-                    variable,
-                )
+                assert util.is_timeseries(nc, variable), f"{variable} is timeseries"
 
     def test_multi_timeseries_orthogonal(self):
         """
         Ensures multi-timeseries-orthogonal detection works
         """
         with Dataset(resources.STATIC_FILES["multi-timeseries-orthogonal"]) as nc:
             for variable in util.get_geophysical_variables(nc):
@@ -59,17 +57,15 @@
 
     def test_trajectory(self):
         """
         Ensures trajectory detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory"]) as nc:
             for variable in util.get_geophysical_variables(nc):
-                assert util.is_cf_trajectory(nc, variable), "{} is trajectory".format(
-                    variable,
-                )
+                assert util.is_cf_trajectory(nc, variable), f"{variable} is trajectory"
 
     def test_trajectory_single(self):
         """
         Ensures trajectory-single detection works
         """
         with Dataset(resources.STATIC_FILES["trajectory-single"]) as nc:
             for variable in util.get_geophysical_variables(nc):
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_ioos_profile.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_ioos_profile.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_ioos_sos.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_ioos_sos.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_protocols.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_protocols.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,41 +24,48 @@
 
 
 @pytest.mark.vcr()
 def test_erddap():
     """
     Tests that a connection can be made to ERDDAP's GridDAP
     """
-    url = "https://coastwatch.pfeg.noaa.gov/erddap/griddap/osu2ChlaAnom"
+    url = "https://www.neracoos.org/erddap/griddap/WW3_EastCoast_latest"
     cs = CheckSuite()
     ds = cs.load_dataset(url)
     assert ds is not None
 
 
 def test_hyrax():
     """
     Tests that a connection can be made to Hyrax
     """
-    url = "http://test.opendap.org:8080/opendap/ioos/mday_joinExist.ncml"
+    # Returns: error 405
+    # url = "http://test.opendap.org:8080/opendap/ioos/mday_joinExist.ncml"
+    # More direct file
+    url = "http://test.opendap.org:8080/opendap/ioos/mday_joinExist.ncml.dap.nc4"
     cs = CheckSuite()
     ds = cs.load_dataset(url)
     assert ds is not None
 
 
 def test_thredds():
     """
     Tests that a connection can be made to a remote THREDDS endpoint
     """
-    url = "http://thredds.ucar.edu/thredds/dodsC/grib/NCEP/GFS/Global_0p25deg_ana/TP"
+    # Returns: error 400
+    # url = "http://thredds.ucar.edu/thredds/dodsC/grib/NCEP/GFS/Global_0p25deg_ana/TP"
+    # Use a smaller dataset
+    url = "https://thredds.ucar.edu/thredds/ncss/grid/grib/NCEP/GFS/Global_0p25deg_ana/TP?var=Temperature_altitude_above_msl&accept=netcdf3"
 
     cs = CheckSuite()
     ds = cs.load_dataset(url)
     assert ds is not None
 
 
+@pytest.mark.skip(reason="The thredds endpoint is no longer serving SOS.")
 def test_sos():
     """
     Tests that a connection can be made to an SOS endpoint
     """
     url = "https://thredds.aoos.org/thredds/dodsC/aoos/cruises/ecofoci/2dy12.nc"
     cs = CheckSuite()
     ds = cs.load_dataset(url)
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_suite.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_suite.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 import os
 import unittest
 from pathlib import Path
 
 import numpy as np
-from pkg_resources import resource_filename
+from importlib_resources import files
 
 from compliance_checker.acdd import ACDDBaseCheck
 from compliance_checker.base import BaseCheck, GenericFile, Result
 from compliance_checker.suite import CheckSuite
 
 static_files = {
-    "2dim": resource_filename("compliance_checker", "tests/data/2dim-grid.nc"),
-    "bad_region": resource_filename("compliance_checker", "tests/data/bad_region.nc"),
-    "bad_data_type": resource_filename(
-        "compliance_checker",
-        "tests/data/bad_data_type.nc",
-    ),
-    "test_cdl": resource_filename("compliance_checker", "tests/data/test_cdl.cdl"),
-    "test_cdl_nc": resource_filename(
-        "compliance_checker",
-        "tests/data/test_cdl_nc_file.nc",
-    ),
-    "empty": resource_filename("compliance_checker", "tests/data/non-comp/empty.file"),
-    "ru07": resource_filename(
-        "compliance_checker",
-        "tests/data/ru07-20130824T170228_rt0.nc",
-    ),
-    "netCDF4": resource_filename(
-        "compliance_checker",
-        "tests/data/test_cdl_nc4_file.cdl",
-    ),
+    "2dim": files("compliance_checker") / "tests/data/2dim-grid.nc",
+    "bad_region": files("compliance_checker") / "tests/data/bad_region.nc",
+    "bad_data_type": files("compliance_checker") / "tests/data/bad_data_type.nc",
+    "test_cdl": files("compliance_checker") / "tests/data/test_cdl.cdl",
+    "test_cdl_nc": files("compliance_checker") / "tests/data/test_cdl_nc_file.nc",
+    "empty": files("compliance_checker") / "tests/data/non-comp/empty.file",
+    "ru07": files("compliance_checker") / "tests/data/ru07-20130824T170228_rt0.nc",
+    "netCDF4": files("compliance_checker") / "tests/data/test_cdl_nc4_file.cdl",
 }
 
 
 class TestSuite(unittest.TestCase):
     # @see
     # http://www.saltycrane.com/blog/2012/07/how-prevent-nose-unittest-using-docstring-when-verbosity-2/
 
@@ -59,24 +47,27 @@
 
     __str__ = __repr__
 
     def test_suite(self):
         # BWA: what's the purpose of this test?  Just to see if the suite
         # runs without errors?
         ds = self.cs.load_dataset(static_files["2dim"])
-        self.cs.run(ds, [], "acdd")
+        # self.cs.run(ds, [], "acdd")
+        self.cs.run_all(ds, ["acdd"], skip_checks=[])
 
     def test_suite_pathlib(self):
         path_obj = Path(static_files["2dim"])
         ds = self.cs.load_dataset(path_obj)
-        self.cs.run(ds, [], "acdd")
+        # self.cs.run(ds, [], "acdd")
+        self.cs.run_all(ds, ["acdd"], skip_checks=[])
 
     def test_unicode_formatting(self):
         ds = self.cs.load_dataset(static_files["bad_region"])
-        score_groups = self.cs.run(ds, [], "cf")
+        # score_groups = self.cs.run(ds, [], "cf")
+        score_groups = self.cs.run_all(ds, ["cf"], skip_checks=[])
 
         limit = 2
         for checker, rpair in score_groups.items():
             groups, errors = rpair
             score_list, points, out_of = self.cs.standard_output(
                 ds.filepath(),
                 limit,
@@ -91,17 +82,17 @@
         """
         Tests that suite.generate_dataset works with cdl file with netCDF4
         features.
         """
         # create netCDF4 file
         ds_name = self.cs.generate_dataset(static_files["netCDF4"])
         # check if correct name is return
-        assert ds_name == static_files["netCDF4"].replace(".cdl", ".nc")
+        assert ds_name == static_files["netCDF4"].with_suffix(".nc")
         # check if netCDF4 file was created
-        assert os.path.isfile(static_files["netCDF4"].replace(".cdl", ".nc"))
+        assert os.path.isfile(static_files["netCDF4"].with_suffix(".nc"))
 
     def test_include_checks(self):
         ds = self.cs.load_dataset(static_files["bad_data_type"])
         score_groups = self.cs.run_all(ds, ["cf:1.7"], ["check_standard_name"])
         checks_run = score_groups["cf:1.7"][0]
         assert len(checks_run) == 1
         first_check = checks_run[0]
@@ -142,15 +133,14 @@
         # flattened set of messages
         msg_set = {msg for sg in score_groups["cf"][0] for msg in sg.msgs}
 
         expected_excluded_names = {
             "§3.5 flag_meanings for lat",
             "§3.5 flag_meanings for lon",
             "§3.5 lat is a valid flags variable",
-            "§3.5 lat is a valid flags variable",
             "§3.5 lon is a valid flags variable",
         }
 
         self.assertTrue(len(expected_excluded_names & name_set) == 0)
 
         # should skip references
         ref_msg = "references global attribute should be a non-empty string"
@@ -160,15 +150,16 @@
         standard_name_hdr = "§3.3 Standard Name"
         self.assertTrue(standard_name_hdr in name_set)
 
     def test_group_func(self):
         # This is checking for issue #183, where group_func results in
         # IndexError: list index out of range
         ds = self.cs.load_dataset(static_files["bad_data_type"])
-        score_groups = self.cs.run(ds, [], "cf")
+        # score_groups = self.cs.run(ds, [], "cf")
+        score_groups = self.cs.run_all(ds, ["cf"], skip_checks=[])
 
         limit = 2
         for checker, rpair in score_groups.items():
             groups, errors = rpair
             score_list, points, out_of = self.cs.standard_output(
                 ds.filepath(),
                 limit,
@@ -195,15 +186,16 @@
         self.assertEqual(score[1].name, "two")
         self.assertEqual(score[1].value, (1, 2))
 
     def test_cdl_file(self):
         # Testing whether you can run compliance checker on a .cdl file
         # Load the cdl file
         ds = self.cs.load_dataset(static_files["test_cdl"])
-        vals = self.cs.run(ds, [], "cf")
+        # vals = self.cs.run(ds, [], "cf")
+        vals = self.cs.run_all(ds, ["cf"], skip_checks=[])
 
         limit = 2
         for checker, rpair in vals.items():
             groups, errors = rpair
             score_list, cdl_points, cdl_out_of = self.cs.standard_output(
                 ds.filepath(),
                 limit,
@@ -218,15 +210,16 @@
                 cdl_out_of,
                 checker,
             )
         ds.close()
 
         # Ok now load the nc file that it came from
         ds = self.cs.load_dataset(static_files["test_cdl_nc"])
-        vals = self.cs.run(ds, [], "cf")
+        # vals = self.cs.run(ds, [], "cf")
+        vals = self.cs.run_all(ds, ["cf"], skip_checks=[])
 
         limit = 2
         for checker, rpair in vals.items():
             groups, errors = rpair
             score_list, nc_points, nc_out_of = self.cs.standard_output(
                 ds.filepath(),
                 limit,
@@ -239,15 +232,15 @@
                 limit,
                 nc_points,
                 nc_out_of,
                 checker,
             )
         ds.close()
 
-        nc_file_path = static_files["test_cdl"].replace(".cdl", ".nc")
+        nc_file_path = static_files["test_cdl"].with_suffix(".nc")
         self.addCleanup(os.remove, nc_file_path)
 
         # Ok the scores should be equal!
         self.assertEqual(nc_points, cdl_points)
         self.assertEqual(nc_out_of, cdl_out_of)
 
     def test_load_local_dataset_GenericFile(self):
@@ -256,15 +249,16 @@
 
     def test_standard_output_score_header(self):
         """
         Check that the output score header only checks the number of
         of potential issues, rather than the weighted score
         """
         ds = self.cs.load_dataset(static_files["bad_region"])
-        score_groups = self.cs.run(ds, [], "cf")
+        # score_groups = self.cs.run(ds, [], "cf")
+        score_groups = self.cs.run_all(ds, ["cf"], skip_checks=[])
         limit = 2
         groups, errors = score_groups["cf"]
         score_list, all_passed, out_of = self.cs.standard_output(
             ds.filepath(),
             limit,
             "cf",
             groups,
```

### Comparing `compliance-checker-5.1.0/compliance_checker/tests/test_util.py` & `compliance_checker-5.1.1/compliance_checker/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/compliance_checker/util.py` & `compliance_checker-5.1.1/compliance_checker/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 General purpose utility functions to aid in compliance checking tasks
 """
+
 from collections import OrderedDict
 
 import isodate
 import pendulum
 
 
 def datetime_is_iso(date_str):
```

### Comparing `compliance-checker-5.1.0/compliance_checker.egg-info/PKG-INFO` & `compliance_checker-5.1.1/compliance_checker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,53 @@
 Metadata-Version: 2.1
 Name: compliance-checker
-Version: 5.1.0
+Version: 5.1.1
 Summary: Checks Datasets and SOS endpoints for standards compliance
-Home-page: https://github.com/ioos/compliance-checker
-Author: Dave Foster
-Author-email: dave@axiomdatascience.com
-License: Apache License 2.0
+Maintainer: Benjamin Adams, Luke Campbell, Filipe Fernandes
+Maintainer-email: Dave Foster <dave@axiomdatascience.com>
+License: Apache-2.0
+Project-URL: documentation, https://ioos.github.io/compliance-checker
+Project-URL: homepage, https://compliance.ioos.us/index.html
+Project-URL: repository, https://github.com/ioos/compliance-checker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: ~=3.5
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cf-units>=2
+Requires-Dist: cftime>=1.1.0
+Requires-Dist: importlib-metadata
+Requires-Dist: importlib-resources
+Requires-Dist: isodate>=0.6.1
+Requires-Dist: jinja2>=2.7.3
+Requires-Dist: lxml>=3.2.1
+Requires-Dist: netcdf4>=1.6.4
+Requires-Dist: owsLib>=0.8.3
+Requires-Dist: packaging
+Requires-Dist: pendulum>=1.2.4
+Requires-Dist: pygeoif>=0.6
+Requires-Dist: pyproj>=2.2.1
+Requires-Dist: regex>=2017.07.28
+Requires-Dist: requests>=2.2.1
+Requires-Dist: setuptools>=15.0
+Requires-Dist: shapely>=1.7.1
+Requires-Dist: validators>=0.14.2
 
 # IOOS Compliance Checker
 
 [![Tests](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml/badge.svg)](https://github.com/ioos/compliance-checker/actions/workflows/default-tests.yml)
 [![codecov](https://codecov.io/gh/ioos/compliance-checker/branch/develop/graph/badge.svg)](https://app.codecov.io/gh/ioos/compliance-checker)
 
 The IOOS Compliance Checker is a python based tool for data providers to check
```

### Comparing `compliance-checker-5.1.0/docs/Makefile` & `compliance_checker-5.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/docs/source/_templates/autosummary/class.rst` & `compliance_checker-5.1.1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/docs/source/_templates/autosummary/module.rst` & `compliance_checker-5.1.1/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/docs/source/_templates/layout.html` & `compliance_checker-5.1.1/docs/source/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `compliance-checker-5.1.0/docs/source/conf.py` & `compliance_checker-5.1.1/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,7 +161,12 @@
         "compliance_checker Documentation",
         author,
         "compliance_checker",
         "One line description of project.",
         "Miscellaneous",
     ),
 ]
+
+linkcheck_ignore = [
+    # TODO: check again in the future
+    r"https://mmisw.org/ont/ioos/platform",  # 2023-09-05 site non-responsive
+]
```

### Comparing `compliance-checker-5.1.0/docs/source/faq.md` & `compliance_checker-5.1.1/docs/source/faq.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,10 +41,12 @@
 
 ## Where can I find more information about the Compliance Checker?
 
 The Compliance Checker is completely open-source and available on [GitHub](https://github.com/ioos/compliance-checker).
 
 ## Disclaimer
 
-The objective of the IOOS Compliance Checker is to check your file against our interpretation of select dataset metadata standards to use as a guideline in generating compliant files.
-The compliance checker should not be considered the authoritative source on whether your file is 100% "compliant".
+The objective of the IOOS Compliance Checker is to check your file against
+our interpretation of select dataset metadata standards to use as a
+guideline in generating compliant files.  The compliance checker should
+not be considered the authoritative source on whether your file is 100% "compliant".
 Instead, we recommend that users use the results as a guide to work towards compliance.
```

