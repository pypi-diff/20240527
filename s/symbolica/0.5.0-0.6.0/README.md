# Comparing `tmp/symbolica-0.5.0.tar.gz` & `tmp/symbolica-0.6.0.tar.gz`

## Comparing `symbolica-0.5.0.tar` & `symbolica-0.6.0.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 symbolica-0.5.0/Cargo.toml
--rw-r--r--   0     1000     1000      747 2024-04-15 13:33:10.000000 symbolica-0.5.0/.github/workflows/coverage.yml
--rw-r--r--   0     1000     1000     1118 2024-04-15 13:33:10.000000 symbolica-0.5.0/.github/workflows/publish_pypi.yml
--rw-r--r--   0     1000     1000       19 2023-06-16 10:52:31.000000 symbolica-0.5.0/.gitignore
--rw-r--r--   0     1000     1000    35757 2024-05-13 10:09:46.000000 symbolica-0.5.0/Cargo.lock
--rw-r--r--   0     1000     1000     6428 2024-05-13 10:07:07.000000 symbolica-0.5.0/Contributing.md
--rw-r--r--   0     1000     1000      812 2023-09-07 13:11:55.000000 symbolica-0.5.0/License.md
--rw-r--r--   0     1000     1000     4118 2024-05-13 10:09:18.000000 symbolica-0.5.0/Readme.md
--rw-r--r--   0     1000     1000      422 2024-01-25 12:49:23.000000 symbolica-0.5.0/build.rs
--rw-r--r--   0     1000     1000      351 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/builder.rs
--rw-r--r--   0     1000     1000      730 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/coefficient_ring.rs
--rw-r--r--   0     1000     1000     1049 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/collect.rs
--rw-r--r--   0     1000     1000      414 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/derivative.rs
--rw-r--r--   0     1000     1000     1161 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/evaluate.rs
--rw-r--r--   0     1000     1000      170 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/expansion.rs
--rw-r--r--   0     1000     1000     3945 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/factorization.rs
--rw-r--r--   0     1000     1000     1447 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/fibonacci.rs
--rw-r--r--   0     1000     1000     2368 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/fuel_backend.rs
--rw-r--r--   0     1000     1000     1182 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/groebner_basis.rs
--rw-r--r--   0     1000     1000     1362 2024-03-18 08:47:11.000000 symbolica-0.5.0/examples/numerical_integration.rs
--rw-r--r--   0     1000     1000   191454 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/optimize.rs
--rw-r--r--   0     1000     1000   191166 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/optimize_multiple.rs
--rw-r--r--   0     1000     1000     1329 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/partial_fraction.rs
--rw-r--r--   0     1000     1000      622 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/partition.rs
--rw-r--r--   0     1000     1000     1332 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/pattern_match.rs
--rw-r--r--   0     1000     1000     2795 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/pattern_restrictions.rs
--rw-r--r--   0     1000     1000     1700 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/polynomial.rs
--rw-r--r--   0     1000     1000     1180 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/polynomial_gcd.rs
--rw-r--r--   0     1000     1000      306 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/rational_polynomial.rs
--rw-r--r--   0     1000     1000      678 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/rational_reconstruction.rs
--rw-r--r--   0     1000     1000      315 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/replace_all.rs
--rw-r--r--   0     1000     1000      796 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/replace_once.rs
--rw-r--r--   0     1000     1000      263 2024-05-13 10:07:07.000000 symbolica-0.5.0/examples/series.rs
--rw-r--r--   0     1000     1000     2402 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/solve_linear_system.rs
--rw-r--r--   0     1000     1000      711 2024-05-13 10:07:07.000000 symbolica-0.5.0/examples/streaming.rs
--rw-r--r--   0     1000     1000     1340 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/tree_replace.rs
--rw-r--r--   0     1000     1000      495 2024-04-15 13:33:10.000000 symbolica-0.5.0/examples/tree_walk.rs
--rw-r--r--   0     1000     1000    21600 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/api/cpp.rs
--rw-r--r--   0     1000     1000     7147 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/api/mathematica.rs
--rw-r--r--   0     1000     1000   191049 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/api/python.rs
--rw-r--r--   0     1000     1000      117 2023-09-07 13:11:55.000000 symbolica-0.5.0/src/api.rs
--rw-r--r--   0     1000     1000    22708 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom/coefficient.rs
--rw-r--r--   0     1000     1000    40768 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom/representation.rs
--rw-r--r--   0     1000     1000    30720 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/atom.rs
--rw-r--r--   0     1000     1000    35828 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/coefficient.rs
--rw-r--r--   0     1000     1000    17680 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/collect.rs
--rw-r--r--   0     1000     1000    10821 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/combinatorics.rs
--rw-r--r--   0     1000     1000    24367 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/derivative.rs
--rw-r--r--   0     1000     1000     8476 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/algebraic_number.rs
--rw-r--r--   0     1000     1000     3704 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/atom.rs
--rw-r--r--   0     1000     1000    34619 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/factorized_rational_polynomial.rs
--rw-r--r--   0     1000     1000    31997 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/finite_field.rs
--rw-r--r--   0     1000     1000    20789 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/float.rs
--rw-r--r--   0     1000     1000    48681 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/integer.rs
--rw-r--r--   0     1000     1000    28980 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains/rational.rs
--rw-r--r--   0     1000     1000    45363 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/domains/rational_polynomial.rs
--rw-r--r--   0     1000     1000     3148 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/domains.rs
--rw-r--r--   0     1000     1000     6653 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/evaluate.rs
--rw-r--r--   0     1000     1000    12470 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/expand.rs
--rw-r--r--   0     1000     1000    90392 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/id.rs
--rw-r--r--   0     1000     1000    17802 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/lib.rs
--rw-r--r--   0     1000     1000    49791 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/normalize.rs
--rw-r--r--   0     1000     1000    40419 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/numerical_integration.rs
--rw-r--r--   0     1000     1000    46095 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/parser.rs
--rw-r--r--   0     1000     1000    71732 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/evaluate.rs
--rw-r--r--   0     1000     1000   111965 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/factor.rs
--rwxr-xr-x   0     1000     1000   112252 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/gcd.rs
--rw-r--r--   0     1000     1000    33344 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/groebner.rs
--rwxr-xr-x   0     1000     1000   118681 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/polynomial.rs
--rw-r--r--   0     1000     1000    19317 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/resultant.rs
--rw-r--r--   0     1000     1000    30161 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly/series.rs
--rw-r--r--   0     1000     1000    30216 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/poly/univariate.rs
--rw-r--r--   0     1000     1000    61699 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/poly.rs
--rw-r--r--   0     1000     1000    45472 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/printer.rs
--rw-r--r--   0     1000     1000     5986 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/solve.rs
--rw-r--r--   0     1000     1000    23961 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/state.rs
--rw-r--r--   0     1000     1000    15822 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/streaming.rs
--rw-r--r--   0     1000     1000    26269 2024-04-15 13:33:10.000000 symbolica-0.5.0/src/tensors/matrix.rs
--rw-r--r--   0     1000     1000       16 2024-03-18 08:47:11.000000 symbolica-0.5.0/src/tensors.rs
--rw-r--r--   0     1000     1000    23774 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/transformer.rs
--rw-r--r--   0     1000     1000      641 2024-05-13 10:07:07.000000 symbolica-0.5.0/src/utils.rs
--rw-r--r--   0     1000     1000    91441 2024-05-13 10:07:07.000000 symbolica-0.5.0/symbolica.pyi
--rw-r--r--   0     1000     1000     1639 2024-05-13 10:07:07.000000 symbolica-0.5.0/tests/import_export.rs
--rw-r--r--   0     1000     1000     2298 2024-04-15 13:33:10.000000 symbolica-0.5.0/tests/pattern_matching.rs
--rw-r--r--   0     1000     1000   418688 2024-04-15 13:33:10.000000 symbolica-0.5.0/tests/rational_polynomial.rs
--rw-r--r--   0     1000     1000      755 2024-05-13 10:09:18.000000 symbolica-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 symbolica-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1900 1970-01-01 00:00:00.000000 symbolica-0.6.0/Cargo.toml
+-rw-r--r--   0     1000     1000      715 2024-05-27 14:03:09.000000 symbolica-0.6.0/.github/workflows/coverage.yml
+-rw-r--r--   0     1000     1000      714 2024-05-27 14:03:09.000000 symbolica-0.6.0/.github/workflows/publish_pypi.yml
+-rw-r--r--   0     1000     1000       55 2024-05-27 14:03:09.000000 symbolica-0.6.0/.gitignore
+-rw-r--r--   0     1000     1000    35485 2024-05-27 14:03:28.000000 symbolica-0.6.0/Cargo.lock
+-rw-r--r--   0     1000     1000     6428 2024-05-13 10:07:07.000000 symbolica-0.6.0/Contributing.md
+-rw-r--r--   0     1000     1000      812 2023-09-07 13:11:55.000000 symbolica-0.6.0/License.md
+-rw-r--r--   0     1000     1000     4118 2024-05-27 14:03:56.000000 symbolica-0.6.0/Readme.md
+-rw-r--r--   0     1000     1000      422 2024-01-25 12:49:23.000000 symbolica-0.6.0/build.rs
+-rw-r--r--   0     1000     1000      351 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/builder.rs
+-rw-r--r--   0     1000     1000      730 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/coefficient_ring.rs
+-rw-r--r--   0     1000     1000     1049 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/collect.rs
+-rw-r--r--   0     1000     1000      414 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/derivative.rs
+-rw-r--r--   0     1000     1000     1161 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/evaluate.rs
+-rw-r--r--   0     1000     1000      170 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/expansion.rs
+-rw-r--r--   0     1000     1000     3945 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/factorization.rs
+-rw-r--r--   0     1000     1000     1447 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/fibonacci.rs
+-rw-r--r--   0     1000     1000     2368 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/fuel_backend.rs
+-rw-r--r--   0     1000     1000     1182 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/groebner_basis.rs
+-rw-r--r--   0     1000     1000     1362 2024-03-18 08:47:11.000000 symbolica-0.6.0/examples/numerical_integration.rs
+-rw-r--r--   0     1000     1000   191454 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/optimize.rs
+-rw-r--r--   0     1000     1000   191166 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/optimize_multiple.rs
+-rw-r--r--   0     1000     1000     1329 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/partial_fraction.rs
+-rw-r--r--   0     1000     1000      622 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/partition.rs
+-rw-r--r--   0     1000     1000     1332 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/pattern_match.rs
+-rw-r--r--   0     1000     1000     2795 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/pattern_restrictions.rs
+-rw-r--r--   0     1000     1000     1700 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/polynomial.rs
+-rw-r--r--   0     1000     1000     1180 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/polynomial_gcd.rs
+-rw-r--r--   0     1000     1000      306 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/rational_polynomial.rs
+-rw-r--r--   0     1000     1000      678 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/rational_reconstruction.rs
+-rw-r--r--   0     1000     1000      315 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/replace_all.rs
+-rw-r--r--   0     1000     1000      796 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/replace_once.rs
+-rw-r--r--   0     1000     1000      263 2024-05-13 10:07:07.000000 symbolica-0.6.0/examples/series.rs
+-rw-r--r--   0     1000     1000     2402 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/solve_linear_system.rs
+-rw-r--r--   0     1000     1000      711 2024-05-13 10:07:07.000000 symbolica-0.6.0/examples/streaming.rs
+-rw-r--r--   0     1000     1000     1340 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/tree_replace.rs
+-rw-r--r--   0     1000     1000      495 2024-04-15 13:33:10.000000 symbolica-0.6.0/examples/tree_walk.rs
+-rw-r--r--   0     1000     1000    21600 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/api/cpp.rs
+-rw-r--r--   0     1000     1000     7147 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/api/mathematica.rs
+-rw-r--r--   0     1000     1000   203292 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/api/python.rs
+-rw-r--r--   0     1000     1000      117 2023-09-07 13:11:55.000000 symbolica-0.6.0/src/api.rs
+-rw-r--r--   0     1000     1000    22708 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/atom/coefficient.rs
+-rw-r--r--   0     1000     1000    41378 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/atom/representation.rs
+-rw-r--r--   0     1000     1000    30436 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/atom.rs
+-rw-r--r--   0     1000     1000    35828 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/coefficient.rs
+-rw-r--r--   0     1000     1000    25509 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/collect.rs
+-rw-r--r--   0     1000     1000    10870 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/combinatorics.rs
+-rw-r--r--   0     1000     1000    31379 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/derivative.rs
+-rw-r--r--   0     1000     1000     8476 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/domains/algebraic_number.rs
+-rw-r--r--   0     1000     1000     3811 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/domains/atom.rs
+-rw-r--r--   0     1000     1000    34619 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/domains/factorized_rational_polynomial.rs
+-rw-r--r--   0     1000     1000    31997 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/domains/finite_field.rs
+-rw-r--r--   0     1000     1000    22261 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/domains/float.rs
+-rw-r--r--   0     1000     1000    48681 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/domains/integer.rs
+-rw-r--r--   0     1000     1000    28980 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/domains/rational.rs
+-rw-r--r--   0     1000     1000    45363 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/domains/rational_polynomial.rs
+-rw-r--r--   0     1000     1000     3148 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/domains.rs
+-rw-r--r--   0     1000     1000     6653 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/evaluate.rs
+-rw-r--r--   0     1000     1000    12470 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/expand.rs
+-rw-r--r--   0     1000     1000    96549 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/id.rs
+-rw-r--r--   0     1000     1000    17802 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/lib.rs
+-rw-r--r--   0     1000     1000    49791 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/normalize.rs
+-rw-r--r--   0     1000     1000    40419 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/numerical_integration.rs
+-rw-r--r--   0     1000     1000    49634 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/parser.rs
+-rw-r--r--   0     1000     1000    72496 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/poly/evaluate.rs
+-rw-r--r--   0     1000     1000   111965 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/poly/factor.rs
+-rwxr-xr-x   0     1000     1000   112252 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/poly/gcd.rs
+-rw-r--r--   0     1000     1000    33344 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/poly/groebner.rs
+-rwxr-xr-x   0     1000     1000   118681 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/poly/polynomial.rs
+-rw-r--r--   0     1000     1000    19317 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/poly/resultant.rs
+-rw-r--r--   0     1000     1000    30080 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/poly/series.rs
+-rw-r--r--   0     1000     1000    30216 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/poly/univariate.rs
+-rw-r--r--   0     1000     1000    61699 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/poly.rs
+-rw-r--r--   0     1000     1000    45472 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/printer.rs
+-rw-r--r--   0     1000     1000     5986 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/solve.rs
+-rw-r--r--   0     1000     1000    24012 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/state.rs
+-rw-r--r--   0     1000     1000    16310 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/streaming.rs
+-rw-r--r--   0     1000     1000    26269 2024-04-15 13:33:10.000000 symbolica-0.6.0/src/tensors/matrix.rs
+-rw-r--r--   0     1000     1000       16 2024-03-18 08:47:11.000000 symbolica-0.6.0/src/tensors.rs
+-rw-r--r--   0     1000     1000    24684 2024-05-27 14:03:09.000000 symbolica-0.6.0/src/transformer.rs
+-rw-r--r--   0     1000     1000      641 2024-05-13 10:07:07.000000 symbolica-0.6.0/src/utils.rs
+-rw-r--r--   0     1000     1000    96741 2024-05-27 14:03:09.000000 symbolica-0.6.0/symbolica.pyi
+-rw-r--r--   0     1000     1000     1639 2024-05-13 10:07:07.000000 symbolica-0.6.0/tests/import_export.rs
+-rw-r--r--   0     1000     1000     2298 2024-04-15 13:33:10.000000 symbolica-0.6.0/tests/pattern_matching.rs
+-rw-r--r--   0     1000     1000   418688 2024-04-15 13:33:10.000000 symbolica-0.6.0/tests/rational_polynomial.rs
+-rw-r--r--   0     1000     1000      755 2024-05-27 14:03:56.000000 symbolica-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 symbolica-0.6.0/PKG-INFO
```

### Comparing `symbolica-0.5.0/Cargo.toml` & `symbolica-0.6.0/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 edition = "2021"
 keywords = ["algebra", "symbolic", "manipulation", "mathematics", "physics"]
 license-file = "License.md"
 name = "symbolica"
 readme = "Readme.md"
 repository = "https://github.com/benruijl/symbolica"
 rust-version = "1.73"
-version = "0.5.0"
+version = "0.6.0"
 
 [profile.release]
 codegen-units = 1
 lto = true
 
 [profile.dev-optim]
 inherits = "dev"
```

### Comparing `symbolica-0.5.0/.github/workflows/coverage.yml` & `symbolica-0.6.0/.github/workflows/coverage.yml`

 * *Files 16% similar despite different names*

```diff
@@ -14,12 +14,12 @@
       - name: Install cargo-llvm-cov
         uses: taiki-e/install-action@cargo-llvm-cov
       - name: Install nextest
         uses: taiki-e/install-action@nextest
       - name: Generate code coverage
         run: cargo llvm-cov --workspace --codecov --output-path codecov.json
       - name: Upload coverage to Codecov
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
-          token: ${{ secrets.CODECOV_TOKEN }} # not required for public repos
+          token: ${{ secrets.CODECOV_TOKEN }}
           files: codecov.json
           fail_ci_if_error: true
```

### Comparing `symbolica-0.5.0/Cargo.lock` & `symbolica-0.6.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,30 +15,30 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.7"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -58,29 +58,29 @@
 name = "append-only-vec"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3cb8f874ecf419dd8165d0279746de966cb8966636d028845e3bd65d519812a"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -94,71 +94,62 @@
 checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
-
-[[package]]
-name = "bitflags"
-version = "2.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "brotli"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "19483b140a7ac7174d34b5a581b406c64f84da5409d3e09cf4fff604f9270e67"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
  "brotli-decompressor",
 ]
 
 [[package]]
 name = "brotli-decompressor"
-version = "4.0.0"
+version = "4.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6221fe77a248b9117d431ad93761222e1cf8ff282d9d1d5d9f53d6299a1cf76"
+checksum = "9a45bd2e4095a8b518033b128020dd4a55aab1c0a381ba4404a472630f4bc362"
 dependencies = [
  "alloc-no-stdlib",
  "alloc-stdlib",
 ]
 
 [[package]]
 name = "bytemuck"
-version = "1.14.1"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed2490600f404f2b94c167e31d3ed1d5f3c225a0f3b80230053b3e0b7b962bd9"
+checksum = "78834c15cb5d5efe3452d58b1e8ba890dd62d21907f867f383358198e56ebca5"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -205,39 +196,39 @@
 checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "env_logger"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
@@ -245,43 +236,33 @@
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
-name = "errno"
-version = "0.3.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
-dependencies = [
- "libc",
- "windows-sys 0.52.0",
-]
-
-[[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "ghost"
 version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0e085ded9f1267c32176b40921b9754c474f7dd96f7e808d4a982e48aa1e854"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
@@ -300,129 +281,129 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.4"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "inventory"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "84344c6e0b90a9e2b6f3f9abe5cc74402684e348df7b32adca28747e0cef091a"
 dependencies = [
  "ctor",
  "ghost",
 ]
 
 [[package]]
 name = "inventory"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8573b2b1fb643a372c73b23f4da5f888677feef3305146d68a539250a9bccc7"
+checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.10"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bad00257d07be169d870ab665980b06cdb366d792ad690bf2e76876dc503455"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
- "rustix",
+ "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.155"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
+
+[[package]]
+name = "libm"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "link-cplusplus"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d240c6f7e1ba3a28b0249f774e6a9dd0175054b52dfbb61b16eb8505c3785c9"
 dependencies = [
  "cc",
 ]
 
 [[package]]
-name = "linux-raw-sys"
-version = "0.4.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
-
-[[package]]
 name = "lock_api"
-version = "0.4.11"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "matchers"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
@@ -431,17 +412,17 @@
 dependencies = [
  "overload",
  "winapi",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "object"
 version = "0.32.2"
@@ -470,52 +451,58 @@
 name = "overload"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.1"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.9"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "process_path"
 version = "0.1.4"
@@ -524,79 +511,81 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
- "inventory 0.3.14",
+ "inventory 0.3.15",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -634,17 +623,17 @@
 checksum = "6f97cdb2a36ed4183de61b2f824cc45c9f1037f28afe0a322e9fff4c108b5aaa"
 dependencies = [
  "rand_core",
 ]
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -654,114 +643,102 @@
 dependencies = [
  "crossbeam-deque",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
 ]
 
 [[package]]
 name = "ref-cast"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4846d4c50d1721b1a3bef8af76924eef20d5e723647333798c1b519b3a9473f"
+checksum = "ccf0a6f84d5f1d581da8b41b47ec8600871962f2a528115b542b362d4b744931"
 dependencies = [
  "ref-cast-impl",
 ]
 
 [[package]]
 name = "ref-cast-impl"
-version = "1.0.22"
+version = "1.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fddb4f8d99b0a2ebafc65a87a69a7b9875e4b1ae1f00db265d300ef7f28bccc"
+checksum = "bcc303e793d3734489387d205e9b186fac9c6cfacedd98cbb2e8a5943595f3e6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.4.4",
- "regex-syntax 0.8.2",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 dependencies = [
  "regex-syntax 0.6.29",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.4"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3b7fa1134405e2ec9353fd416b17f8dacd46c473d7d3fd1cf202706a14eb792a"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax 0.8.2",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rug"
-version = "1.23.0"
+version = "1.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf1855d294a2bd8f38c5a3a6dc456144aeaf15827beeb880300296923100d49"
+checksum = "a8df4099c6fa90a1a7f5ddc0c7fba50991080fa2084d5a78808a5a3cab406bb9"
 dependencies = [
  "az",
  "gmp-mpfr-sys",
  "libc",
+ "libm",
 ]
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
-
-[[package]]
-name = "rustix"
-version = "0.38.30"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
-dependencies = [
- "bitflags 2.4.2",
- "errno",
- "libc",
- "linux-raw-sys",
- "windows-sys 0.52.0",
-]
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
@@ -772,52 +749,52 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "self_cell"
-version = "1.0.3"
+version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "58bf37232d3bb9a2c4e641ca2a11d83b5062066f88df7fed36c28772046d65ba"
+checksum = "d369a96f978623eb3dc28807c4852d6cc617fed53da5d3c400feff1ef34a714a"
 
 [[package]]
 name = "serde"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.197"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "sharded-slab"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
@@ -830,15 +807,15 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "symbolica"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "ahash",
  "append-only-vec",
  "bincode",
  "brotli",
  "byteorder",
  "bytes",
@@ -871,43 +848,43 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thread_local"
-version = "1.1.7"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "tikv-jemalloc-sys"
@@ -950,15 +927,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -1024,17 +1001,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.14"
+version = "0.7.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b31891d644eba1789fb6715f27fbc322e4bdf2ecdc412ede1993246159271613"
+checksum = "cd8dc749a1b03f3c255a3064a4f5c0ee5ed09b7c6bc6d4525d31f779cd74d7fc"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1050,19 +1027,19 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+checksum = "4d4cc384e1e73b93bafa6fb4f1df8c41695c8a91cf9c4c64358067d15a7b6c6b"
 dependencies = [
- "winapi",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
@@ -1091,15 +1068,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1111,38 +1088,39 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8e92753b1c443191654ec532f14c199742964a061be25d77d7a96f09db20bf5"
 
@@ -1150,17 +1128,17 @@
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a711c68811799e017b6038e0922cb27a5e2f43a2ddb609fe0b6f3eeda9de615"
 
@@ -1168,17 +1146,23 @@
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "146c11bb1a02615db74680b32a68e2d61f553cc24c4eb5b4ca10311740e44172"
 
@@ -1186,17 +1170,17 @@
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c912b12f7454c6620635bbff3450962753834be2a594819bd5e945af18ec64bc"
 
@@ -1204,29 +1188,29 @@
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "504a2476202769977a040c6364301a3f65d0cc9e3fb08600b2bda150a0488316"
 
@@ -1234,17 +1218,17 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "wolfram-app-discovery"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fcac5bdcf7a95e6981e73b69ba9a9c360cb64d50739e3713236caaa2f026b60"
 dependencies = [
@@ -1323,24 +1307,24 @@
  "env_logger",
  "link-cplusplus",
  "wolfram-app-discovery",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.32"
+version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+checksum = "15e934569e47891f7d9411f1a451d947a60e000ab3bd24fbb970f000387d1b3b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.66",
 ]
```

### Comparing `symbolica-0.5.0/Contributing.md` & `symbolica-0.6.0/Contributing.md`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/License.md` & `symbolica-0.6.0/License.md`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/Readme.md` & `symbolica-0.6.0/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ## Rust
 
 If you want to use Symbolica as a library in Rust, simply include it in the `Cargo.toml`:
 
 ```toml
 [dependencies]
-symbolica = "0.5"
+symbolica = "0.6"
 ```
 
 # Examples
 
 Below we list some examples of the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a complete overview.
 
 ### Pattern matching
```

#### html2text {}

```diff
@@ -14,15 +14,15 @@
 (probably) already know, by using Symbolica's bindings to Python, Rust and C++:
 [A demo of Symbolica]# Installation Visit the [Get Started](https://
 symbolica.io/docs/get_started.html) page for detailed installation
 instructions. ## Python Symbolica can be installed for Python >3.5 using `pip`:
 ```sh pip install symbolica ``` The installation may take some time on Mac OS
 and Windows, as it may have to compile Symbolica. ## Rust If you want to use
 Symbolica as a library in Rust, simply include it in the `Cargo.toml`: ```toml
-[dependencies] symbolica = "0.5" ``` # Examples Below we list some examples of
+[dependencies] symbolica = "0.6" ``` # Examples Below we list some examples of
 the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a
 complete overview. ### Pattern matching Variables ending with a `_` are
 wildcards that match to any subexpression. In the following example we try to
 match the pattern `f(w1_,w2_)`: ```python from symbolica import Expression x,
 y, w1_, w2_ = Expression.vars('x','y','w1_','w2_') f = Expression.fun('f') e =
 f(3,x)*y**2+5 r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2)) print(r) ```
 which yields `y^2*f(2,x^2)+5`. ### Solving a linear system Solve a linear
```

### Comparing `symbolica-0.5.0/examples/coefficient_ring.rs` & `symbolica-0.6.0/examples/coefficient_ring.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/collect.rs` & `symbolica-0.6.0/examples/collect.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/evaluate.rs` & `symbolica-0.6.0/examples/evaluate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/factorization.rs` & `symbolica-0.6.0/examples/factorization.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/fibonacci.rs` & `symbolica-0.6.0/examples/fibonacci.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/fuel_backend.rs` & `symbolica-0.6.0/examples/fuel_backend.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/groebner_basis.rs` & `symbolica-0.6.0/examples/groebner_basis.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/numerical_integration.rs` & `symbolica-0.6.0/examples/numerical_integration.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/optimize.rs` & `symbolica-0.6.0/examples/optimize.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/optimize_multiple.rs` & `symbolica-0.6.0/examples/optimize_multiple.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/partial_fraction.rs` & `symbolica-0.6.0/examples/partial_fraction.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/partition.rs` & `symbolica-0.6.0/examples/partition.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/pattern_match.rs` & `symbolica-0.6.0/examples/pattern_match.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/pattern_restrictions.rs` & `symbolica-0.6.0/examples/pattern_restrictions.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/polynomial.rs` & `symbolica-0.6.0/examples/polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/polynomial_gcd.rs` & `symbolica-0.6.0/examples/polynomial_gcd.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/rational_reconstruction.rs` & `symbolica-0.6.0/examples/rational_reconstruction.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/replace_once.rs` & `symbolica-0.6.0/examples/replace_once.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/solve_linear_system.rs` & `symbolica-0.6.0/examples/solve_linear_system.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/streaming.rs` & `symbolica-0.6.0/examples/streaming.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/examples/tree_replace.rs` & `symbolica-0.6.0/examples/tree_replace.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/api/cpp.rs` & `symbolica-0.6.0/src/api/cpp.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/api/mathematica.rs` & `symbolica-0.6.0/src/api/mathematica.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/api/python.rs` & `symbolica-0.6.0/src/api/python.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             FromNumeratorAndDenominator, RationalPolynomial, RationalPolynomialField,
         },
         Ring,
     },
     evaluate::EvaluationFn,
     id::{
         Condition, Match, MatchSettings, MatchStack, Pattern, PatternAtomTreeIterator,
-        PatternRestriction, ReplaceIterator, WildcardAndRestriction,
+        PatternRestriction, ReplaceIterator, Replacement, WildcardAndRestriction,
     },
     numerical_integration::{ContinuousGrid, DiscreteGrid, Grid, MonteCarloRng, Sample},
     parser::Token,
     poly::{
         evaluate::{
             InstructionEvaluator, InstructionSetMode, InstructionSetModeCPPSettings,
             InstructionSetPrinter,
@@ -67,21 +67,21 @@
 fn symbolica(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PythonExpression>()?;
     m.add_class::<PythonPattern>()?;
     m.add_class::<PythonPolynomial>()?;
     m.add_class::<PythonIntegerPolynomial>()?;
     m.add_class::<PythonFiniteFieldPolynomial>()?;
     m.add_class::<PythonRationalPolynomial>()?;
-    m.add_class::<PythonRationalPolynomialSmallExponent>()?;
     m.add_class::<PythonFiniteFieldRationalPolynomial>()?;
     m.add_class::<PythonMatrix>()?;
     m.add_class::<PythonNumericalIntegrator>()?;
     m.add_class::<PythonSample>()?;
     m.add_class::<PythonAtomType>()?;
     m.add_class::<PythonAtomTree>()?;
+    m.add_class::<PythonReplacement>()?;
     m.add_class::<PythonInstructionEvaluator>()?;
     m.add_class::<PythonRandomNumberGenerator>()?;
     m.add_class::<PythonPatternRestriction>()?;
     m.add_class::<PythonTermStreamer>()?;
     m.add_class::<PythonSeries>()?;
 
     m.add_function(wrap_pyfunction!(get_version, m)?)?;
@@ -249,14 +249,29 @@
         match self {
             Self::Literal(l) => Ok(l.to_expression().expr.as_view().into_pattern().into()),
             Self::Pattern(e) => Ok(e),
         }
     }
 }
 
+#[derive(FromPyObject)]
+pub enum OneOrMultiple<T> {
+    One(T),
+    Multiple(Vec<T>),
+}
+
+impl<T> OneOrMultiple<T> {
+    pub fn to_iter(&self) -> impl Iterator<Item = &T> {
+        match self {
+            OneOrMultiple::One(a) => std::slice::from_ref(a).iter(),
+            OneOrMultiple::Multiple(m) => m.iter(),
+        }
+    }
+}
+
 /// Operations that transform an expression.
 #[pyclass(name = "Transformer", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonPattern {
     pub expr: Pattern,
 }
 
@@ -768,15 +783,14 @@
     /// Examples
     /// --------
     ///
     /// >>> x, w1_, w2_ = Expression.symbols('x','w1_','w2_')
     /// >>> f = Expression.symbol('f')
     /// >>> e = f(3,x)
     /// >>> r = e.transform().replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2), (w1_ >= 1) & w2_.is_var())
-    /// >>> print(r)
     pub fn replace_all(
         &self,
         lhs: ConvertibleToPattern,
         rhs: ConvertibleToPattern,
         cond: Option<PythonPatternRestriction>,
         non_greedy_wildcards: Option<Vec<PythonExpression>>,
         level_range: Option<(usize, Option<usize>)>,
@@ -817,14 +831,37 @@
                 rhs.to_pattern()?.expr.clone(),
                 cond.map(|r| r.condition.clone()).unwrap_or_default(),
                 settings,
             )
         );
     }
 
+    /// Create a transformer that replaces all atoms matching the patterns. See `replace_all` for more information.
+    ///
+    /// Examples
+    /// --------
+    ///
+    /// >>> x, y, f = Expression.symbols('x', 'y', 'f')
+    /// >>> e = f(x,y)
+    /// >>> r = e.transform().replace_all_multiple(Replacement(x, y), Replacement(y, x))
+    pub fn replace_all_multiple(
+        &self,
+        replacements: Vec<PythonReplacement>,
+    ) -> PyResult<PythonPattern> {
+        return append_transformer!(
+            self,
+            Transformer::ReplaceAllMultiple(
+                replacements
+                    .into_iter()
+                    .map(|r| (r.pattern, r.rhs, r.cond, r.settings))
+                    .collect()
+            )
+        );
+    }
+
     /// Create a transformer that prints the expression.
     ///
     /// Examples
     /// --------
     /// >>> Expression.parse('f(10)').transform().print(terms_on_new_line = True).execute()
     #[pyo3(signature =
         (terms_on_new_line = false,
@@ -1604,15 +1641,15 @@
         match self.expr.as_ref() {
             Atom::Num(_) => PythonAtomType::Num,
             Atom::Var(_) => PythonAtomType::Var,
             Atom::Fun(_) => PythonAtomType::Fn,
             Atom::Add(_) => PythonAtomType::Add,
             Atom::Mul(_) => PythonAtomType::Mul,
             Atom::Pow(_) => PythonAtomType::Pow,
-            Atom::Empty => unreachable!(),
+            Atom::Zero => PythonAtomType::Num,
         }
     }
 
     /// Convert the expression to a tree.
     pub fn to_atom_tree(&self) -> PyResult<PythonAtomTree> {
         self.expr.as_view().into()
     }
@@ -2347,15 +2384,15 @@
         let b = stream.to_expression();
 
         Ok(b.into())
     }
 
     /// Set the coefficient ring to contain the variables in the `vars` list.
     /// This will move all variables into a rational polynomial function.
-
+    ///
     /// Parameters
     /// ----------
     /// vars: List[Expression] A list of variables
     pub fn set_coefficient_ring(&self, vars: Vec<PythonExpression>) -> PyResult<PythonExpression> {
         let mut var_map = vec![];
         for v in vars {
             match v.expr.as_view() {
@@ -2653,14 +2690,41 @@
     /// >>> p = Expression.parse('v1^2/2+v1^3/v4*v2+v3/(1+v4)')
     /// >>> print(p.together())
     pub fn together(&self) -> PyResult<PythonExpression> {
         let poly = self.expr.to_rational_polynomial::<_, _, u32>(&Q, &Z, None);
         Ok(poly.to_expression().into())
     }
 
+    /// Cancel common factors between numerators and denominators.
+    /// Any non-canceling parts of the expression will not be rewritten.
+    ///
+    /// Examples
+    /// --------
+    ///
+    /// >>> from symbolica import Expression
+    /// >>> p = Expression.parse('1+(y+1)^10*(x+1)/(x^2+2x+1)')
+    /// >>> print(p.cancel())
+    /// 1+(y+1)**10/(x+1)
+    pub fn cancel(&self) -> PyResult<PythonExpression> {
+        Ok(self.expr.cancel().into())
+    }
+
+    /// Factor the expression over the rationals.
+    ///
+    /// Examples
+    /// --------
+    ///
+    /// >>> from symbolica import Expression
+    /// >>> p = Expression.parse('(6 + x)/(7776 + 6480*x + 2160*x^2 + 360*x^3 + 30*x^4 + x^5)')
+    /// >>> print(p.factor())
+    /// (x+6)**-4
+    pub fn factor(&self) -> PyResult<PythonExpression> {
+        Ok(self.expr.factor().into())
+    }
+
     /// Convert the expression to a polynomial, optionally, with the variables and the ordering specified in `vars`.
     /// All non-polynomial elements will be converted to new independent variables.
     pub fn to_polynomial(&self, vars: Option<Vec<PythonExpression>>) -> PyResult<PythonPolynomial> {
         let mut var_map = vec![];
         if let Some(vm) = vars {
             for v in vm {
                 match v.expr.as_view() {
@@ -2722,47 +2786,16 @@
         };
 
         Ok(PythonRationalPolynomial {
             poly: self.expr.to_rational_polynomial(&Q, &Z, var_map),
         })
     }
 
-    /// Similar to [PythonExpression::to_rational_polynomial()], but the power of each variable limited to 255.
-    pub fn to_rational_polynomial_small_exponent(
-        &self,
-        vars: Option<Vec<PythonExpression>>,
-    ) -> PyResult<PythonRationalPolynomialSmallExponent> {
-        let mut var_map = vec![];
-        if let Some(vm) = vars {
-            for v in vm {
-                match v.expr.as_view() {
-                    AtomView::Var(v) => var_map.push(v.get_symbol().into()),
-                    e => {
-                        Err(exceptions::PyValueError::new_err(format!(
-                            "Expected variable instead of {}",
-                            e
-                        )))?;
-                    }
-                }
-            }
-        }
-
-        let var_map = if var_map.is_empty() {
-            None
-        } else {
-            Some(Arc::new(var_map))
-        };
-
-        Ok(PythonRationalPolynomialSmallExponent {
-            poly: self.expr.to_rational_polynomial(&Q, &Z, var_map),
-        })
-    }
-
     /// Return an iterator over the pattern `self` matching to `lhs`.
-    /// Restrictions on pattern can be supplied through `cond`.
+    /// Restrictions on the pattern can be supplied through `cond`.
     ///
     /// Examples
     /// --------
     ///
     /// >>> x, x_ = Expression.symbols('x','x_')
     /// >>> f = Expression.symbol('f')
     /// >>> e = f(x)*f(1)*f(2)*f(3)
@@ -2794,14 +2827,47 @@
             ),
             move |(lhs, target, res, settings)| {
                 PatternAtomTreeIterator::new(lhs, target.as_view(), res, settings)
             },
         ))
     }
 
+    /// Test whether the pattern is found in the expression.
+    /// Restrictions on the pattern can be supplied through `cond`.
+    ///
+    /// Examples
+    /// --------
+    ///
+    /// >>> f = Expression.symbol('f')
+    /// >>> if f(1).matches(f(2)):
+    /// >>>    print('match')
+    pub fn matches(
+        &self,
+        lhs: ConvertibleToPattern,
+        cond: Option<PythonPatternRestriction>,
+        level_range: Option<(usize, Option<usize>)>,
+        level_is_tree_depth: Option<bool>,
+    ) -> PyResult<bool> {
+        let pat = lhs.to_pattern()?.expr;
+        let conditions = cond
+            .map(|r| r.condition.clone())
+            .unwrap_or(Condition::default());
+        let settings = MatchSettings {
+            level_range: level_range.unwrap_or((0, None)),
+            level_is_tree_depth: level_is_tree_depth.unwrap_or(false),
+            ..MatchSettings::default()
+        };
+
+        Ok(
+            PatternAtomTreeIterator::new(&pat, self.expr.as_view(), &conditions, &settings)
+                .next()
+                .is_some(),
+        )
+    }
+
     /// Return an iterator over the replacement of the pattern `self` on `lhs` by `rhs`.
     /// Restrictions on pattern can be supplied through `cond`.
     ///
     /// The `level_range` specifies the `[min,max]` level at which the pattern is allowed to match.
     /// The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree,
     /// depending on `level_is_tree_depth`.
     ///
@@ -2943,14 +3009,63 @@
             std::mem::swap(&mut out, &mut out2);
             expr_ref = out2.as_view();
         }
 
         Ok(out.into_inner().into())
     }
 
+    /// Replace all atoms matching the patterns. See `replace_all` for more information.
+    ///
+    /// The entire operation can be repeated until there are no more matches using `repeat=True`.
+    ///
+    /// Examples
+    /// --------
+    ///
+    /// >>> x, y, f = Expression.symbols('x', 'y', 'f')
+    /// >>> e = f(x,y)
+    /// >>> r = e.replace_all_multiple(Replacement(x, y), Replacement(y, x))
+    /// >>> print(r)
+    /// f(y,x)
+    ///
+    /// Parameters
+    /// ----------
+    /// replacements: Sequence[Replacement]
+    ///     The list of replacements to apply.
+    /// repeat: bool, optional
+    ///     If set to `True`, the entire operation will be repeated until there are no more matches.
+    pub fn replace_all_multiple(
+        &self,
+        replacements: Vec<PythonReplacement>,
+        repeat: Option<bool>,
+    ) -> PyResult<PythonExpression> {
+        let reps = replacements
+            .iter()
+            .map(|x| {
+                Replacement::new(&x.pattern, &x.rhs)
+                    .with_conditions(&x.cond)
+                    .with_settings(&x.settings)
+            })
+            .collect::<Vec<_>>();
+
+        let mut expr_ref = self.expr.as_view();
+
+        let mut out = RecycledAtom::new();
+        let mut out2 = RecycledAtom::new();
+        while expr_ref.replace_all_multiple_into(&reps, &mut out) {
+            if !repeat.unwrap_or(false) {
+                break;
+            }
+
+            std::mem::swap(&mut out, &mut out2);
+            expr_ref = out2.as_view();
+        }
+
+        Ok(out.into_inner().into())
+    }
+
     /// Solve a linear system in the variables `variables`, where each expression
     /// in the system is understood to yield 0.
     ///
     /// Examples
     /// --------
     /// >>> from symbolica import Expression
     /// >>> x, y, c = Expression.symbols('x', 'y', 'c')
@@ -3099,53 +3214,175 @@
             .expr
             .as_view()
             .evaluate(&constants, &functions, &mut cache);
         Ok(PyComplex::from_doubles(py, r.re, r.im))
     }
 }
 
+/// A raplacement, which is a pattern and a right-hand side, with optional conditions and settings.
+#[pyclass(name = "Replacement", module = "symbolica")]
+#[derive(Clone)]
+pub struct PythonReplacement {
+    pattern: Pattern,
+    rhs: Pattern,
+    cond: Condition<WildcardAndRestriction>,
+    settings: MatchSettings,
+}
+
+#[pymethods]
+impl PythonReplacement {
+    #[new]
+    pub fn new(
+        pattern: ConvertibleToPattern,
+        rhs: ConvertibleToPattern,
+        cond: Option<PythonPatternRestriction>,
+        non_greedy_wildcards: Option<Vec<PythonExpression>>,
+        level_range: Option<(usize, Option<usize>)>,
+        level_is_tree_depth: Option<bool>,
+    ) -> PyResult<Self> {
+        let pattern = pattern.to_pattern()?.expr;
+        let rhs = rhs.to_pattern()?.expr;
+
+        let mut settings = MatchSettings::default();
+
+        if let Some(ngw) = non_greedy_wildcards {
+            settings.non_greedy_wildcards = ngw
+                .iter()
+                .map(|x| match x.expr.as_view() {
+                    AtomView::Var(v) => {
+                        let name = v.get_symbol();
+                        if v.get_wildcard_level() == 0 {
+                            return Err(exceptions::PyTypeError::new_err(
+                                "Only wildcards can be restricted.",
+                            ));
+                        }
+                        Ok(name)
+                    }
+                    _ => Err(exceptions::PyTypeError::new_err(
+                        "Only wildcards can be restricted.",
+                    )),
+                })
+                .collect::<Result<_, _>>()?;
+        }
+        if let Some(level_range) = level_range {
+            settings.level_range = level_range;
+        }
+        if let Some(level_is_tree_depth) = level_is_tree_depth {
+            settings.level_is_tree_depth = level_is_tree_depth;
+        }
+
+        let cond = cond
+            .as_ref()
+            .map(|r| r.condition.clone())
+            .unwrap_or(Condition::default());
+
+        Ok(Self {
+            pattern,
+            rhs,
+            cond,
+            settings,
+        })
+    }
+}
+
+#[derive(FromPyObject)]
+pub enum SeriesOrExpression {
+    Series(PythonSeries),
+    Expression(PythonExpression),
+}
+
 /// A series expansion class.
 ///
 /// Supports standard arithmetic operations, such
 /// as addition and multiplication.
 ///
 /// Examples
 /// --------
 /// >>> x = Expression.symbol('x')
 /// >>> s = Expression.parse("(1-cos(x))/sin(x)").series(x, 0, 4)
 /// >>> print(s)
 #[pyclass(name = "Series", module = "symbolica")]
+#[derive(Clone)]
 pub struct PythonSeries {
     pub series: Series<AtomField>,
 }
 
 #[pymethods]
 impl PythonSeries {
-    /// Add this series to `other`, returning the result.
-    pub fn __add__(&self, rhs: &Self) -> PyResult<Self> {
+    /// Add this series to `rhs`, returning the result.
+    pub fn __add__(&self, rhs: SeriesOrExpression) -> PyResult<Self> {
+        match rhs {
+            SeriesOrExpression::Series(rhs) => Ok(Self {
+                series: &self.series + &rhs.series,
+            }),
+            SeriesOrExpression::Expression(rhs) => Ok(Self {
+                series: (&self.series + &rhs.expr)
+                    .map_err(|e| exceptions::PyValueError::new_err(e))?,
+            }),
+        }
+    }
+
+    /// Add this series to `rhs`, returning the result.
+    pub fn __radd__(&self, rhs: &PythonExpression) -> PyResult<Self> {
         Ok(Self {
-            series: &self.series + &rhs.series,
+            series: (&self.series + &rhs.expr).map_err(|e| exceptions::PyValueError::new_err(e))?,
         })
     }
 
-    pub fn __sub__(&self, rhs: &Self) -> PyResult<Self> {
+    pub fn __sub__(&self, rhs: SeriesOrExpression) -> PyResult<Self> {
+        match rhs {
+            SeriesOrExpression::Series(rhs) => Ok(Self {
+                series: &self.series - &rhs.series,
+            }),
+            SeriesOrExpression::Expression(rhs) => Ok(Self {
+                series: (&self.series - &rhs.expr)
+                    .map_err(|e| exceptions::PyValueError::new_err(e))?,
+            }),
+        }
+    }
+
+    pub fn __rsub__(&self, lhs: &PythonExpression) -> PyResult<Self> {
         Ok(Self {
-            series: &self.series - &rhs.series,
+            series: (&lhs.expr - &self.series).map_err(|e| exceptions::PyValueError::new_err(e))?,
         })
     }
 
-    pub fn __mul__(&self, rhs: &Self) -> PyResult<Self> {
+    pub fn __mul__(&self, rhs: SeriesOrExpression) -> PyResult<Self> {
+        match rhs {
+            SeriesOrExpression::Series(rhs) => Ok(Self {
+                series: &self.series * &rhs.series,
+            }),
+            SeriesOrExpression::Expression(rhs) => Ok(Self {
+                series: (&self.series * &rhs.expr)
+                    .map_err(|e| exceptions::PyValueError::new_err(e))?,
+            }),
+        }
+    }
+
+    pub fn __rmul__(&self, lhs: &PythonExpression) -> PyResult<Self> {
         Ok(Self {
-            series: &self.series * &rhs.series,
+            series: (&self.series * &lhs.expr).map_err(|e| exceptions::PyValueError::new_err(e))?,
         })
     }
 
-    pub fn __truediv__(&self, rhs: &Self) -> PyResult<Self> {
+    pub fn __truediv__(&self, rhs: SeriesOrExpression) -> PyResult<Self> {
+        match rhs {
+            SeriesOrExpression::Series(rhs) => Ok(Self {
+                series: &self.series / &rhs.series,
+            }),
+            SeriesOrExpression::Expression(rhs) => Ok(Self {
+                series: (&self.series / &rhs.expr)
+                    .map_err(|e| exceptions::PyValueError::new_err(e))?,
+            }),
+        }
+    }
+
+    pub fn __rtruediv__(&self, lhs: &PythonExpression) -> PyResult<Self> {
         Ok(Self {
-            series: &self.series / &rhs.series,
+            series: (&lhs.expr / &self.series).map_err(|e| exceptions::PyValueError::new_err(e))?,
         })
     }
 
     pub fn __pow__(&self, rhs: i64, m: Option<i64>) -> PyResult<Self> {
         if m.is_some() {
             return Err(exceptions::PyValueError::new_err(
                 "Optional number argument not supported",
@@ -3214,21 +3451,52 @@
             series: self
                 .series
                 .pow(&pow.series)
                 .map_err(|e| exceptions::PyValueError::new_err(e))?,
         })
     }
 
+    /// Shift the series by `e` units of the ramification.
+    pub fn shift(&self, e: isize) -> Self {
+        Self {
+            series: self.series.clone().mul_exp_units(e),
+        }
+    }
+
+    /// Get the ramification.
+    pub fn get_ramification(&self) -> usize {
+        self.series.get_ramification()
+    }
+
+    /// Get the trailing exponent; the exponent of the first non-zero term.
+    pub fn get_trailing_exponent(&self) -> PyResult<(i64, i64)> {
+        if let Rational::Natural(n, d) = self.series.get_trailing_exponent() {
+            Ok((n, d))
+        } else {
+            Err(exceptions::PyValueError::new_err("Order is too large"))
+        }
+    }
+
+    /// Get the absolute order.
+    pub fn get_absolute_order(&self) -> PyResult<(i64, i64)> {
+        if let Rational::Natural(n, d) = self.series.absolute_order() {
+            Ok((n, d))
+        } else {
+            Err(exceptions::PyValueError::new_err("Order is too large"))
+        }
+    }
+
     /// Convert the series into an expression.
     pub fn to_expression(&self) -> PythonExpression {
         self.series.to_atom().into()
     }
 }
 
-/// A Symbolica term streamer.
+/// A term streamer that can handle large expressions, by
+/// streaming terms to and from disk.
 #[pyclass(name = "TermStreamer", module = "symbolica")]
 pub struct PythonTermStreamer {
     pub stream: TermStreamer<CompressorWriter<BufWriter<File>>>,
 }
 
 #[pymethods]
 impl PythonTermStreamer {
@@ -3258,34 +3526,45 @@
         })
     }
 
     pub fn __iadd__(&mut self, rhs: &mut Self) {
         self.stream += &mut rhs.stream;
     }
 
+    /// Get the total number of bytes of the stream.
     pub fn get_byte_size(&self) -> usize {
         self.stream.get_byte_size()
     }
 
-    /// Add an expression to the term streamer.
+    /// Return true iff the stream fits in memory.
+    pub fn fits_in_memory(&self) -> bool {
+        self.stream.fits_in_memory()
+    }
+
+    /// Get the number of terms in the stream.
+    pub fn get_num_terms(&self) -> usize {
+        self.stream.get_num_terms()
+    }
+
+    /// Add an expression to the term stream.
     pub fn push(&mut self, expr: PythonExpression) {
         self.stream.push(expr.expr.clone());
     }
 
-    /// Sort and fuse all terms in the streamer.
+    /// Sort and fuse all terms in the stream.
     pub fn normalize(&mut self) {
         self.stream.normalize();
     }
 
     /// Convert the term stream into an expression. This may exceed the available memory.
     pub fn to_expression(&mut self) -> PythonExpression {
         self.stream.to_expression().into()
     }
 
-    /// Map the transformations to every term in the streamer.
+    /// Map the transformations to every term in the stream.
     pub fn map(&mut self, op: PythonPattern, py: Python) -> PyResult<Self> {
         let t = match &op.expr {
             Pattern::Transformer(t) => {
                 if t.0.is_some() {
                     return Err(exceptions::PyValueError::new_err(
                         "Transformer is bound to expression. Use Transformer() instead."
                             .to_string(),
@@ -3314,14 +3593,46 @@
                 });
                 out
             });
             Ok::<_, PyErr>(m)
         })
         .map(|x| PythonTermStreamer { stream: x })
     }
+
+    /// Map the transformations to every term in the stream using a single thread.
+    pub fn map_single_thread(&mut self, op: PythonPattern) -> PyResult<Self> {
+        let t = match &op.expr {
+            Pattern::Transformer(t) => {
+                if t.0.is_some() {
+                    return Err(exceptions::PyValueError::new_err(
+                        "Transformer is bound to expression. Use Transformer() instead."
+                            .to_string(),
+                    ));
+                }
+                &t.1
+            }
+            _ => {
+                return Err(exceptions::PyValueError::new_err(
+                    "Operation must of a transformer".to_string(),
+                ));
+            }
+        };
+
+        // map every term in the expression
+        let s = self.stream.map_single_thread(|x| {
+            let mut out = Atom::default();
+            Workspace::get_local().with(|ws| {
+                Transformer::execute(x.as_view(), &t, ws, &mut out)
+                    .unwrap_or_else(|e| panic!("Transformer failed during execution: {:?}", e));
+            });
+            out
+        });
+
+        Ok(PythonTermStreamer { stream: s })
+    }
 }
 
 self_cell!(
     #[pyclass(module = "symbolica")]
     pub struct PythonAtomIterator {
         owner: Atom,
         #[covariant]
@@ -4035,37 +4346,57 @@
                         "The division has a remainder: {}",
                         r
                     )))
                 }
             }
 
             /// Divide `self` by `rhs`, returning the quotient and remainder.
-            pub fn quot_rem(&self, rhs: Self) -> (Self, Self) {
-                if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
+            pub fn quot_rem(&self, rhs: Self) -> PyResult<(Self, Self)> {
+                if rhs.poly.is_zero() {
+                    Err(exceptions::PyValueError::new_err("Division by zero"))
+                } else if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     let (q, r) = self.poly.quot_rem(&rhs.poly, false);
-
-                    (Self { poly: q }, Self { poly: r })
+                    Ok((Self { poly: q }, Self { poly: r }))
                 } else {
                     let mut new_self = self.poly.clone();
                     let mut new_rhs = rhs.poly.clone();
                     new_self.unify_variables(&mut new_rhs);
 
                     let (q, r) = new_self.quot_rem(&new_rhs, false);
 
-                    (Self { poly: q }, Self { poly: r })
+                    Ok((Self { poly: q }, Self { poly: r }))
                 }
             }
 
             /// Negate the polynomial.
             pub fn __neg__(&self) -> Self {
                 Self {
                     poly: self.poly.clone().neg(),
                 }
             }
 
+            /// Compute the remainder `self % rhs.
+            pub fn __mod__(&self, rhs: Self) -> PyResult<Self> {
+                if rhs.poly.is_zero() {
+                    Err(exceptions::PyValueError::new_err("Division by zero"))
+                } else if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
+                    Ok(Self {
+                        poly: self.poly.rem(&rhs.poly),
+                    })
+                } else {
+                    let mut new_self = self.poly.clone();
+                    let mut new_rhs = rhs.poly.clone();
+                    new_self.unify_variables(&mut new_rhs);
+
+                    Ok(Self {
+                        poly: new_self.rem(&new_rhs),
+                    })
+                }
+            }
+
             /// Compute the greatest common divisor (GCD) of two polynomials.
             pub fn gcd(&self, rhs: Self) -> Self {
                 if self.poly.get_vars_ref() == rhs.poly.get_vars_ref() {
                     Self {
                         poly: self.poly.gcd(&rhs.poly),
                     }
                 } else {
@@ -4177,36 +4508,64 @@
             /// >>> from symbolica import Expression
             /// >>> p = Expression.parse('3x^2+6x+9').to_polynomial()
             /// >>> print(p.content())
             pub fn content(&self) -> PyResult<Self> {
                 Ok(Self { poly: self.poly.constant(self.poly.content())})
             }
 
-            /// Get the coefficient list in `x`.
+            /// Get the coefficient list, optionally in the variables `vars`.
             ///
             /// Examples
             /// --------
             ///
             /// >>> from symbolica import Expression
             /// >>> x = Expression.symbol('x')
             /// >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
             /// >>> for n, pp in p.coefficient_list(x):
             /// >>>     print(n, pp)
-            pub fn coefficient_list(&self, var: PythonExpression) -> PyResult<Vec<(usize, Self)>> {
-                let x = self.poly.get_vars_ref().iter().position(|v| match (v, var.expr.as_view()) {
-                    (Variable::Symbol(y), AtomView::Var(vv)) => *y == vv.get_symbol(),
-                    (Variable::Function(_, f) | Variable::Other(f), a) => f.as_view() == a,
-                    _ => false,
-                }).ok_or(exceptions::PyValueError::new_err(format!(
-                    "Variable {} not found in polynomial",
-                    var.__str__()?
-                )))?;
+            pub fn coefficient_list(&self, vars: Option<OneOrMultiple<PythonExpression>>) -> PyResult<Vec<(Vec<usize>, Self)>> {
+                if let Some(vv) = vars {
+                    let mut vars = vec![];
+
+                    for vvv in vv.to_iter() {
+                        let x = self.poly.get_vars_ref().iter().position(|v| match (v, vvv.expr.as_view()) {
+                            (Variable::Symbol(y), AtomView::Var(vv)) => *y == vv.get_symbol(),
+                            (Variable::Function(_, f) | Variable::Other(f), a) => f.as_view() == a,
+                            _ => false,
+                        }).ok_or(exceptions::PyValueError::new_err(format!(
+                            "Variable {} not found in polynomial",
+                            vvv.__str__()?
+                        )))?;
 
-                Ok(self.poly.to_univariate_polynomial_list(x).into_iter()
-                    .map(|(f, p)| (p as usize, Self { poly: f })).collect())
+                        vars.push(x);
+                    }
+
+                    if vars.is_empty() {
+                        return Ok(self.poly.into_iter().map(|t| {
+                            (t.exponents.iter().map(|x| *x as usize).collect(), Self { poly: self.poly.constant(t.coefficient.clone()) })
+                       }).collect());
+                    }
+
+                    if vars.len() == 1 {
+                        return Ok(self.poly.to_univariate_polynomial_list(vars[0]).into_iter()
+                        .map(|(f, p)| (vec![p as usize], Self { poly: f })).collect());
+                    }
+
+                    // sort the exponents wrt the var map
+                    let mut r: Vec<(Vec<_>, _)> = self.poly.to_multivariate_polynomial_list(&vars, true).into_iter()
+                        .map(|(f, p)| (vars.iter().map(|v| f[*v] as usize).collect(), Self { poly: p })).collect();
+                    r.sort_by(|a, b| a.0.cmp(&b.0));
+
+                    Ok(r)
+
+                } else {
+                    Ok(self.poly.into_iter().map(|t| {
+                         (t.exponents.iter().map(|x| *x as usize).collect(), Self { poly: self.poly.constant(t.coefficient.clone()) })
+                    }).collect())
+                }
             }
 
             /// Replace the variable `x` with a polynomial `v`.
             ///
             /// Examples
             /// --------
             ///
@@ -4291,21 +4650,14 @@
     pub fn denominator(&self) -> PythonPolynomial {
         PythonPolynomial {
             poly: (&self.poly.denominator).into(),
         }
     }
 }
 
-/// A Symbolica rational polynomial with variable powers limited to 255.
-#[pyclass(name = "RationalPolynomialSmallExponent", module = "symbolica")]
-#[derive(Clone)]
-pub struct PythonRationalPolynomialSmallExponent {
-    pub poly: RationalPolynomial<IntegerRing, u8>,
-}
-
 macro_rules! generate_rat_parse {
     ($type:ty) => {
         #[pymethods]
         impl $type {
             /// Parse a rational polynomial from a string.
             /// The list of all the variables must be provided.
             ///
@@ -4352,15 +4704,14 @@
                 Ok(self.poly.to_expression().into())
             }
         }
     };
 }
 
 generate_rat_parse!(PythonRationalPolynomial);
-generate_rat_parse!(PythonRationalPolynomialSmallExponent);
 
 /// A Symbolica rational polynomial over finite fields.
 #[pyclass(name = "FiniteFieldRationalPolynomial", module = "symbolica")]
 #[derive(Clone)]
 pub struct PythonFiniteFieldRationalPolynomial {
     pub poly: RationalPolynomial<Zp, u16>,
 }
@@ -4605,15 +4956,14 @@
                     .map(|f| Self { poly: f }).collect())
             }
         }
     };
 }
 
 generate_rat_methods!(PythonRationalPolynomial);
-generate_rat_methods!(PythonRationalPolynomialSmallExponent);
 generate_rat_methods!(PythonFiniteFieldRationalPolynomial);
 
 #[derive(FromPyObject)]
 pub enum ConvertibleToRationalPolynomial {
     Literal(PythonRationalPolynomial),
     Expression(ConvertibleToExpression),
 }
```

### Comparing `symbolica-0.5.0/src/atom/coefficient.rs` & `symbolica-0.6.0/src/atom/coefficient.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/atom/representation.rs` & `symbolica-0.6.0/src/atom/representation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 const VAR_WILDCARD_LEVEL_3: u8 = 0b00011000;
 const FUN_SYMMETRIC_FLAG: u8 = 0b00100000;
 const FUN_LINEAR_FLAG: u8 = 0b01000000;
 const VAR_ANTISYMMETRIC_FLAG: u8 = 0b10000000;
 const FUN_ANTISYMMETRIC_FLAG: u64 = 1 << 32; // stored in the function id
 const MUL_HAS_COEFF_FLAG: u8 = 0b01000000;
 
+const ZERO_DATA: [u8; 3] = [NUM_ID, 1, 0];
+
 pub type RawAtom = Vec<u8>;
 
 impl Atom {
     /// Read from a binary stream. The format is the byte-length first
     /// followed by the data.
     pub(crate) fn read<R: Read>(&mut self, mut source: R) -> Result<(), std::io::Error> {
-        let mut dest = std::mem::replace(self, Atom::Empty).into_raw();
+        let mut dest = std::mem::replace(self, Atom::Zero).into_raw();
 
         // should also set whether rat poly coefficient needs to be converted
         let mut flags_buf = [0; 1];
         let mut size_buf = [0; 8];
 
         source.read_exact(&mut flags_buf)?;
         source.read_exact(&mut size_buf)?;
@@ -513,33 +515,42 @@
 
     #[inline]
     pub fn set_from_view(&mut self, view: &MulView) {
         self.data.clear();
         self.data.extend(view.data);
     }
 
+    #[inline]
     pub(crate) fn extend(&mut self, other: AtomView<'_>) {
         self.data[0] |= NOT_NORMALIZED;
 
         // may increase size of the num of args
         let mut c = &self.data[1 + 4..];
 
         let buf_pos = 1 + 4;
 
         let mut n_args;
         (n_args, _, c) = c.get_frac_u64(); // TODO: pack size and n_args
 
         let old_size = unsafe { c.as_ptr().offset_from(self.data.as_ptr()) } as usize - 1 - 4;
 
-        let new_slice = match other {
-            AtomView::Mul(m) => m.to_slice(),
-            _ => ListSlice::from_one(other),
-        };
+        let data_start = match other {
+            AtomView::Mul(m) => {
+                let mut sd = &m.data[1 + 4..];
+                let sub_n_args;
+                (sub_n_args, _, sd) = sd.get_frac_u64();
 
-        n_args += new_slice.len() as u64;
+                n_args += sub_n_args;
+                sd
+            }
+            _ => {
+                n_args += 1;
+                &other.get_data()
+            }
+        };
 
         let new_size = (n_args, 1).get_packed_size() as usize;
 
         match new_size.cmp(&old_size) {
             Ordering::Equal => {}
             Ordering::Less => {
                 self.data.copy_within(1 + 4 + old_size.., 1 + 4 + new_size);
@@ -552,17 +563,15 @@
                     .copy_within(1 + 4 + old_size..old_len, 1 + 4 + new_size);
             }
         }
 
         // size should be ok now
         (n_args, 1).write_packed_fixed(&mut self.data[1 + 4..1 + 4 + new_size]);
 
-        for child in new_slice.iter() {
-            self.data.extend_from_slice(child.get_data());
-        }
+        self.data.extend_from_slice(data_start);
 
         let new_buf_pos = self.data.len();
 
         let mut cursor = &mut self.data[1..];
         cursor
             .write_u32::<LittleEndian>((new_buf_pos - buf_pos) as u32)
             .unwrap();
@@ -684,34 +693,39 @@
         if !normalized {
             self.data[0] |= NOT_NORMALIZED;
         } else {
             self.data[0] &= !NOT_NORMALIZED;
         }
     }
 
+    #[inline]
     pub(crate) fn extend(&mut self, other: AtomView<'_>) {
         self.data[0] |= NOT_NORMALIZED;
 
         let mut c = &self.data[1..];
 
         let mut n_args;
         (n_args, _, c) = c.get_frac_u64();
 
         let old_header_size = unsafe { c.as_ptr().offset_from(self.data.as_ptr()) } as usize;
 
-        let new_slice = match other {
-            AtomView::Add(m) => m.to_slice(),
-            _ => ListSlice::from_one(other),
-        };
-
-        for child in new_slice.iter() {
-            self.data.extend_from_slice(child.get_data());
-        }
+        match other {
+            AtomView::Add(m) => {
+                let mut sd = &m.data[1..];
+                let sub_n_args;
+                (sub_n_args, _, sd) = sd.get_frac_u64();
 
-        n_args += new_slice.len() as u64;
+                n_args += sub_n_args;
+                self.data.extend_from_slice(&sd);
+            }
+            _ => {
+                n_args += 1;
+                self.data.extend_from_slice(&other.get_data());
+            }
+        };
 
         let new_len = self.data.len() - old_header_size;
         let new_header_size = (n_args, new_len as u64).get_packed_size() as usize + 1;
 
         match new_header_size.cmp(&old_header_size) {
             Ordering::Equal => {}
             Ordering::Less => {
@@ -780,15 +794,15 @@
         buffer.extend(self.data);
         Var { data: buffer }
     }
 
     #[inline(always)]
     pub fn get_symbol(&self) -> Symbol {
         Symbol::init_fn(
-            self.data[1..].get_frac_i64().0 as u32,
+            self.data[1..].get_frac_u64().0 as u32,
             self.get_wildcard_level(),
             self.data[0] & FUN_SYMMETRIC_FLAG != 0,
             self.data[0] & VAR_ANTISYMMETRIC_FLAG != 0,
             self.data[0] & FUN_LINEAR_FLAG != 0,
         )
     }
 
@@ -903,15 +917,15 @@
     #[inline]
     pub fn iter(&self) -> ListIterator<'a> {
         let mut c = self.data;
         c.get_u8();
         c.get_u32_le(); // size
 
         let n_args;
-        (_, n_args, c) = c.get_frac_i64(); // name
+        (_, n_args, c) = c.get_frac_u64(); // name
 
         ListIterator {
             data: c,
             length: n_args as u32,
         }
     }
 
@@ -921,15 +935,15 @@
 
     pub fn to_slice(&self) -> ListSlice<'a> {
         let mut c = self.data;
         c.get_u8();
         c.get_u32_le(); // size
 
         let n_args;
-        (_, n_args, c) = c.get_frac_i64(); // name
+        (_, n_args, c) = c.get_frac_u64(); // name
 
         ListSlice {
             data: c,
             length: n_args as usize,
             slice_type: SliceType::Arg,
         }
     }
@@ -1105,25 +1119,25 @@
 
     #[inline]
     pub(crate) fn is_normalized(&self) -> bool {
         (self.data[0] & NOT_NORMALIZED) == 0
     }
 
     pub fn get_nargs(&self) -> usize {
-        self.data[1 + 4..].get_frac_i64().0 as usize
+        self.data[1 + 4..].get_frac_u64().0 as usize
     }
 
     #[inline]
     pub fn iter(&self) -> ListIterator<'a> {
         let mut c = self.data;
         c.get_u8();
         c.get_u32_le(); // size
 
         let n_args;
-        (n_args, _, c) = c.get_frac_i64();
+        (n_args, _, c) = c.get_frac_u64();
 
         ListIterator {
             data: c,
             length: n_args as u32,
         }
     }
 
@@ -1134,15 +1148,15 @@
 
     pub fn to_slice(&self) -> ListSlice<'a> {
         let mut c = self.data;
         c.get_u8();
         c.get_u32_le(); // size
 
         let n_args;
-        (n_args, _, c) = c.get_frac_i64();
+        (n_args, _, c) = c.get_frac_u64();
 
         ListSlice {
             data: c,
             length: n_args as usize,
             slice_type: SliceType::Mul,
         }
     }
@@ -1229,26 +1243,29 @@
 
     pub fn get_byte_size(&self) -> usize {
         self.data.len()
     }
 }
 
 impl<'a> AtomView<'a> {
+    pub const ZERO: Self = Self::Num(NumView { data: &ZERO_DATA });
+
     pub fn from(source: &'a [u8]) -> AtomView<'a> {
         match source[0] & TYPE_MASK {
             VAR_ID => AtomView::Var(VarView { data: source }),
             FUN_ID => AtomView::Fun(FunView { data: source }),
             NUM_ID => AtomView::Num(NumView { data: source }),
             POW_ID => AtomView::Pow(PowView { data: source }),
             MUL_ID => AtomView::Mul(MulView { data: source }),
             ADD_ID => AtomView::Add(AddView { data: source }),
             x => unreachable!("Bad id: {}", x),
         }
     }
 
+    #[inline(always)]
     pub fn get_data(&self) -> &'a [u8] {
         match self {
             AtomView::Num(n) => n.data,
             AtomView::Var(v) => v.data,
             AtomView::Fun(f) => f.data,
             AtomView::Pow(p) => p.data,
             AtomView::Mul(t) => t.data,
@@ -1348,14 +1365,21 @@
                     nm.extend(na.as_view());
                 }
             }
         }
     }
 }
 
+impl PartialEq<AtomView<'_>> for AtomView<'_> {
+    #[inline(always)]
+    fn eq(&self, other: &AtomView) -> bool {
+        self.get_data() == other.get_data()
+    }
+}
+
 #[derive(Debug, Copy, Clone)]
 pub struct ListIterator<'a> {
     data: &'a [u8],
     length: u32,
 }
 
 impl<'a> Iterator for ListIterator<'a> {
```

### Comparing `symbolica-0.5.0/src/atom.rs` & `symbolica-0.6.0/src/atom.rs`

 * *Files 2% similar despite different names*

```diff
@@ -122,28 +122,14 @@
     fn clone(&self) -> Self {
         *self
     }
 }
 
 impl Copy for AtomView<'_> {}
 
-impl PartialEq<AtomView<'_>> for AtomView<'_> {
-    fn eq(&self, other: &AtomView) -> bool {
-        match (self, other) {
-            (AtomView::Num(n1), AtomView::Num(n2)) => n1 == n2,
-            (AtomView::Var(v1), AtomView::Var(v2)) => v1 == v2,
-            (AtomView::Fun(f1), AtomView::Fun(f2)) => f1 == f2,
-            (AtomView::Pow(p1), AtomView::Pow(p2)) => p1 == p2,
-            (AtomView::Mul(m1), AtomView::Mul(m2)) => m1 == m2,
-            (AtomView::Add(a1), AtomView::Add(a2)) => a1 == a2,
-            _ => false,
-        }
-    }
-}
-
 impl Eq for AtomView<'_> {}
 
 impl PartialOrd for AtomView<'_> {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         Some(self.cmp(other))
     }
 }
@@ -372,31 +358,30 @@
             AtomView::Pow(p) => p.get_byte_size(),
             AtomView::Mul(m) => m.get_byte_size(),
             AtomView::Add(a) => a.get_byte_size(),
         }
     }
 }
 
-#[derive(Clone, PartialEq, Eq, Hash)]
+#[derive(Clone)]
 pub enum Atom {
     Num(Num),
     Var(Var),
     Fun(Fun),
     Pow(Pow),
     Mul(Mul),
     Add(Add),
-    #[doc(hidden)]
-    Empty, // for internal use
+    Zero,
 }
 
 impl Default for Atom {
     /// Create an atom that represents the number 0.
     #[inline]
     fn default() -> Self {
-        Num::zero(RawAtom::new()).into()
+        Atom::Zero
     }
 }
 
 impl std::fmt::Display for Atom {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         AtomPrinter::new(self.as_view()).fmt(f)
     }
@@ -434,14 +419,30 @@
 
 impl From<Fun> for Atom {
     fn from(n: Fun) -> Atom {
         Atom::Fun(n)
     }
 }
 
+impl PartialEq for Atom {
+    #[inline(always)]
+    fn eq(&self, other: &Self) -> bool {
+        self.as_view() == other.as_view()
+    }
+}
+
+impl Eq for Atom {}
+
+impl Hash for Atom {
+    #[inline(always)]
+    fn hash<H: std::hash::Hasher>(&self, state: &mut H) {
+        self.as_view().hash(state)
+    }
+}
+
 impl PartialOrd for Atom {
     fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
         Some(self.cmp(other))
     }
 }
 
 impl Ord for Atom {
@@ -452,97 +453,102 @@
 
 impl Atom {
     /// Create an atom that represents the number 0.
     pub fn new() -> Atom {
         Atom::default()
     }
 
-    /// Parse and atom from a string.
+    /// Parse an atom from a string.
     pub fn parse(input: &str) -> Result<Atom, String> {
         Workspace::get_local().with(|ws| Token::parse(input)?.to_atom(ws))
     }
 
     #[inline]
     pub fn new_var(id: Symbol) -> Atom {
         Var::new(id).into()
     }
 
     #[inline]
     pub fn new_num<T: Into<Coefficient>>(num: T) -> Atom {
-        Num::new(num.into()).into()
+        let c = num.into();
+        if c.is_zero() {
+            return Atom::Zero;
+        } else {
+            Num::new(c).into()
+        }
     }
 
     #[inline]
     pub fn is_zero(&self) -> bool {
         self.as_view().is_zero()
     }
 
     #[inline]
     pub fn is_one(&self) -> bool {
         self.as_view().is_one()
     }
 
     #[inline]
     pub fn to_num(&mut self, coeff: Coefficient) -> &mut Num {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Num(Num::new_into(coeff, buffer));
         if let Atom::Num(n) = self {
             n
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn to_var(&mut self, id: Symbol) -> &mut Var {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Var(Var::new_into(id, buffer));
         if let Atom::Var(n) = self {
             n
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn to_fun(&mut self, id: Symbol) -> &mut Fun {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Fun(Fun::new_into(id, buffer));
         if let Atom::Fun(n) = self {
             n
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn to_pow(&mut self, base: AtomView, exp: AtomView) -> &mut Pow {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Pow(Pow::new_into(base, exp, buffer));
         if let Atom::Pow(n) = self {
             n
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn to_mul(&mut self) -> &mut Mul {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Mul(Mul::new_into(buffer));
         if let Atom::Mul(n) = self {
             n
         } else {
             unreachable!()
         }
     }
 
     #[inline]
     pub fn to_add(&mut self) -> &mut Add {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         *self = Atom::Add(Add::new_into(buffer));
         if let Atom::Add(n) = self {
             n
         } else {
             unreachable!()
         }
     }
@@ -552,21 +558,21 @@
         match self {
             Atom::Num(n) => n.into_raw(),
             Atom::Var(v) => v.into_raw(),
             Atom::Fun(f) => f.into_raw(),
             Atom::Pow(p) => p.into_raw(),
             Atom::Mul(m) => m.into_raw(),
             Atom::Add(a) => a.into_raw(),
-            Atom::Empty => unreachable!("Empty atom"),
+            Atom::Zero => RawAtom::new(),
         }
     }
 
     #[inline(always)]
     pub fn set_from_view(&mut self, view: &AtomView) {
-        let buffer = std::mem::replace(self, Atom::Empty).into_raw();
+        let buffer = std::mem::replace(self, Atom::Zero).into_raw();
         match view {
             AtomView::Num(n) => *self = Atom::Num(Num::from_view_into(n, buffer)),
             AtomView::Var(v) => *self = Atom::Var(Var::from_view_into(v, buffer)),
             AtomView::Fun(f) => *self = Atom::Fun(Fun::from_view_into(f, buffer)),
             AtomView::Pow(p) => *self = Atom::Pow(Pow::from_view_into(p, buffer)),
             AtomView::Mul(m) => *self = Atom::Mul(Mul::from_view_into(m, buffer)),
             AtomView::Add(a) => *self = Atom::Add(Add::from_view_into(a, buffer)),
@@ -578,15 +584,15 @@
         match self {
             Atom::Num(n) => AtomView::Num(n.to_num_view()),
             Atom::Var(v) => AtomView::Var(v.to_var_view()),
             Atom::Fun(f) => AtomView::Fun(f.to_fun_view()),
             Atom::Pow(p) => AtomView::Pow(p.to_pow_view()),
             Atom::Mul(m) => AtomView::Mul(m.to_mul_view()),
             Atom::Add(a) => AtomView::Add(a.to_add_view()),
-            Atom::Empty => unreachable!("Empty atom"),
+            Atom::Zero => AtomView::ZERO,
         }
     }
 
     /// Get the symbol of a variable or function.
     #[inline(always)]
     pub fn get_symbol(&self) -> Option<Symbol> {
         match self {
@@ -601,29 +607,29 @@
         match self {
             Atom::Num(_) => {}
             Atom::Var(_) => {}
             Atom::Fun(a) => a.set_normalized(normalized),
             Atom::Pow(a) => a.set_normalized(normalized),
             Atom::Mul(a) => a.set_normalized(normalized),
             Atom::Add(a) => a.set_normalized(normalized),
-            Atom::Empty => unreachable!("Empty atom"),
+            Atom::Zero => {}
         }
     }
 }
 
 /// A constructor of a function,
 ///
 /// For example:
 /// ```
 /// # use symbolica::{
 /// #     atom::{Atom, AsAtomView, FunctionBuilder},
 /// #     state::{FunctionAttribute, State},
 /// # };
 /// # fn main() {
-/// let f_id = State::get_symbol_with_attributes("f", vec![FunctionAttribute::Symmetric]).unwrap();
+/// let f_id = State::get_symbol_with_attributes("f", &[FunctionAttribute::Symmetric]).unwrap();
 /// let fb = FunctionBuilder::new(f_id);
 /// let a = fb
 ///     .add_arg(&Atom::new_num(3))
 ///     .add_arg(&Atom::new_num(2))
 ///     .add_arg(&Atom::new_num(1))
 ///     .finish();
 ///
```

### Comparing `symbolica-0.5.0/src/coefficient.rs` & `symbolica-0.6.0/src/coefficient.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/collect.rs` & `symbolica-0.6.0/src/collect.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 use ahash::HashMap;
 
 use crate::{
     atom::{Add, AsAtomView, Atom, AtomView, Symbol},
+    coefficient::CoefficientView,
     domains::{integer::Z, rational::Q},
+    poly::{factor::Factorize, polynomial::MultivariatePolynomial},
     state::Workspace,
 };
 
 impl Atom {
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name, e.g.
     ///
     /// ```math
@@ -58,14 +60,25 @@
         self.as_view().together()
     }
 
     /// Write the expression as a sum of terms with minimal denominators.
     pub fn apart(&self, x: Symbol) -> Atom {
         self.as_view().apart(x)
     }
+
+    /// Cancel all common factors between numerators and denominators.
+    /// Any non-canceling parts of the expression will not be rewritten.
+    pub fn cancel(&self) -> Atom {
+        self.as_view().cancel()
+    }
+
+    /// Factor the expression over the rationals.
+    pub fn factor(&self) -> Atom {
+        self.as_view().factor()
+    }
 }
 
 impl<'a> AtomView<'a> {
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name, e.g.
     ///
     /// ```math
     /// collect(x + x * y + x^2, x) = x * (1+y) + x^2
@@ -155,23 +168,25 @@
             add.extend(mul_h.as_view());
         }
 
         for (key, coeff) in h {
             map_key_coeff(key.as_view(), coeff, workspace, &key_map, &coeff_map, add);
         }
 
-        if key_map.is_some() {
-            let key = workspace.new_num(1);
-            map_key_coeff(key.as_view(), rest, workspace, &key_map, &coeff_map, add);
-        } else if let Some(coeff_map) = coeff_map {
-            let mut handle = workspace.new_atom();
-            coeff_map(rest.as_view(), &mut handle);
-            add.extend(handle.as_view());
-        } else {
-            add.extend(rest.as_view());
+        if !rest.is_zero() {
+            if key_map.is_some() {
+                let key = workspace.new_num(1);
+                map_key_coeff(key.as_view(), rest, workspace, &key_map, &coeff_map, add);
+            } else if let Some(coeff_map) = coeff_map {
+                let mut handle = workspace.new_atom();
+                coeff_map(rest.as_view(), &mut handle);
+                add.extend(handle.as_view());
+            } else {
+                add.extend(rest.as_view());
+            }
         }
 
         add_h.as_view().normalize(workspace, out);
     }
 
     /// Collect terms involving the same power of `x`, where `x` is a variable or function name.
     /// Return the list of key-coefficient pairs and the remainder that matched no key.
@@ -423,14 +438,194 @@
             }
 
             add.as_view().normalize(ws, out);
         } else {
             out.set_from_view(self);
         }
     }
+
+    /// Cancel all common factors between numerators and denominators.
+    /// Any non-canceling parts of the expression will not be rewritten.
+    pub fn cancel(&self) -> Atom {
+        let mut out = Atom::new();
+        self.cancel_into(&mut out);
+        out
+    }
+
+    /// Cancel all common factors between numerators and denominators.
+    /// Any non-canceling parts of the expression will not be rewritten.
+    pub fn cancel_into(&self, out: &mut Atom) {
+        Workspace::get_local().with(|ws| {
+            self.cancel_with_ws_into(ws, out);
+        });
+    }
+
+    fn cancel_with_ws_into(&self, ws: &Workspace, out: &mut Atom) -> bool {
+        match self {
+            AtomView::Num(_) | AtomView::Var(_) | AtomView::Fun(_) | AtomView::Pow(_) => {
+                out.set_from_view(self);
+                false
+            }
+            AtomView::Mul(m) => {
+                // split between numerator, denominator and rest
+                // any numerator or denominator part that does not cancel will be kept as is
+                let mut numerators = vec![];
+                let mut denominators = vec![];
+                let mut num_changed = vec![];
+                let mut den_changed = vec![];
+                let mut rest = vec![];
+
+                for a in m.iter() {
+                    if let AtomView::Pow(p) = a {
+                        let (b, e) = p.get_base_exp();
+                        if let AtomView::Num(n) = e {
+                            if let CoefficientView::Natural(n, d) = n.get_coeff_view() {
+                                if n < 0 && d == 1 {
+                                    denominators.push(
+                                        b.to_polynomial::<_, u16>(&Q, None).pow(n.abs() as usize),
+                                    );
+                                    den_changed.push((a, false));
+                                    continue;
+                                } else if n > 0 && d == 1 {
+                                    numerators.push(a.to_polynomial::<_, u16>(&Q, None));
+                                    num_changed.push((a, false));
+                                    continue;
+                                }
+                            }
+                        }
+
+                        rest.push(a);
+                    } else {
+                        numerators.push(a.to_polynomial(&Q, None));
+                        num_changed.push((a, false));
+                    }
+                }
+
+                if numerators.is_empty() || denominators.is_empty() {
+                    out.set_from_view(self);
+                    return false;
+                }
+
+                MultivariatePolynomial::unify_variables_list(&mut numerators);
+                MultivariatePolynomial::unify_variables_list(&mut denominators);
+                numerators[0].unify_variables(&mut denominators[0]);
+                MultivariatePolynomial::unify_variables_list(&mut numerators);
+                MultivariatePolynomial::unify_variables_list(&mut denominators);
+
+                let mut changed = false;
+                for (d, ds) in denominators.iter_mut().zip(&mut den_changed) {
+                    for (n, ns) in numerators.iter_mut().zip(&mut num_changed) {
+                        let g = n.gcd(d);
+                        if !g.is_one() {
+                            changed = true;
+                            ds.1 = true;
+                            ns.1 = true;
+                            *n = &*n / &g;
+                            *d = &*d / &g;
+                        }
+                    }
+                }
+
+                if !changed {
+                    out.set_from_view(self);
+                    return false;
+                }
+
+                let mut mul = ws.new_atom();
+                let mul_view = mul.to_mul();
+
+                let mut tmp = ws.new_atom();
+                for (n, (orig, changed)) in numerators.iter().zip(num_changed) {
+                    if changed {
+                        n.to_expression_into(&mut tmp);
+                        mul_view.extend(tmp.as_view());
+                    } else {
+                        mul_view.extend(orig);
+                    }
+                }
+
+                for (d, (orig, changed)) in denominators.iter().zip(den_changed) {
+                    if changed {
+                        d.to_expression_into(&mut tmp);
+
+                        let mut pow = ws.new_atom();
+                        let exp = ws.new_num(-1);
+                        pow.to_pow(tmp.as_view(), exp.as_view());
+
+                        mul_view.extend(pow.as_view());
+                    } else {
+                        mul_view.extend(orig);
+                    }
+                }
+
+                for r in rest {
+                    mul_view.extend(r);
+                }
+
+                mul_view.as_view().normalize(ws, out);
+                true
+            }
+            AtomView::Add(a) => {
+                let mut add = ws.new_atom();
+                let add_view = add.to_add();
+
+                let mut changed = false;
+                let mut tmp = ws.new_atom();
+                for arg in a.iter() {
+                    if arg.cancel_with_ws_into(ws, &mut tmp) {
+                        changed = true;
+                        add_view.extend(tmp.as_view());
+                    } else {
+                        add_view.extend(arg);
+                    }
+                }
+
+                if changed {
+                    add_view.as_view().normalize(ws, out);
+                    true
+                } else {
+                    out.set_from_view(self);
+                    false
+                }
+            }
+        }
+    }
+
+    /// Factor the expression over the rationals.
+    pub fn factor(&self) -> Atom {
+        let r = self.to_rational_polynomial::<_, _, u16>(&Q, &Z, None);
+        let f_n = r.numerator.factor();
+        let f_d = r.denominator.factor();
+
+        let mut out = Atom::new();
+        let mul = out.to_mul();
+
+        let mut pow = Atom::new();
+        for (k, v) in f_n {
+            if v > 1 {
+                let exp = Atom::new_num(v as i64);
+                pow.to_pow(k.to_expression().as_view(), exp.as_view());
+                mul.extend(pow.as_view());
+            } else {
+                mul.extend(k.to_expression().as_view());
+            }
+        }
+
+        for (k, v) in f_d {
+            let exp = Atom::new_num(-(v as i64));
+            pow.to_pow(k.to_expression().as_view(), exp.as_view());
+            mul.extend(pow.as_view());
+        }
+
+        Workspace::get_local().with(|ws| {
+            out.as_view().normalize(ws, &mut pow);
+        });
+
+        pow
+    }
 }
 
 #[cfg(test)]
 mod test {
     use crate::{
         atom::{Atom, FunctionBuilder},
         fun,
@@ -531,8 +726,32 @@
                 .unwrap();
         let out = input.apart(State::get_symbol("v4"));
 
         let ref_out = Atom::parse("1/2*v1^2+v3*(v4+1)^-1+v1^3*v2*v4^-1").unwrap();
 
         assert_eq!(out, ref_out);
     }
+
+    #[test]
+    fn cancel() {
+        let input =
+            Atom::parse("1/(v1+1)^2 + (v1^2 - 1)*(v2+1)^10/(v1 - 1)+ 5 + (v1+1)/(v1^2+2v1+1)")
+                .unwrap();
+        let out = input.cancel();
+
+        let ref_out = Atom::parse("(v1+1)^-2+(v1+1)^-1+(v1+1)*(v2+1)^10+5").unwrap();
+
+        assert_eq!(out, ref_out);
+    }
+
+    #[test]
+    fn factor() {
+        let input =
+            Atom::parse("(6 + v1)/(7776 + 6480*v1 + 2160*v1^2 + 360*v1^3 + 30*v1^4 + v1^5)")
+                .unwrap();
+        let out = input.factor();
+
+        let ref_out = Atom::parse("(v1+6)^-4").unwrap();
+
+        assert_eq!(out, ref_out);
+    }
 }
```

### Comparing `symbolica-0.5.0/src/combinatorics.rs` & `symbolica-0.6.0/src/combinatorics.rs`

 * *Files 2% similar despite different names*

```diff
@@ -171,19 +171,20 @@
 }
 
 /// Partition the unordered list `elements` into named bins of unordered lists with a given length,
 /// returning all partitions and their multiplicity.
 ///
 /// For example:
 /// ```
+/// # use symbolica::combinatorics::partitions;
 /// partitions(&[1, 1, 1, 2, 2],
 ///     &[('f', 2), ('g', 2), ('f', 1)],
 ///     false,
 ///     false
-/// )
+/// );
 /// ```
 /// generates all possible ways to partition the elements of three sets
 /// and yields:
 /// ```plain
 /// [(3, [('g', [1]), ('f', [1, 1]), ('f', [2, 2])]), (6, [('g', [1]), ('f', [1, 2]),
 /// ('f', [1, 2])]), (6, [('g', [2]), ('f', [1, 1]), ('f', [1, 2])])]
 /// ```
```

### Comparing `symbolica-0.5.0/src/derivative.rs` & `symbolica-0.6.0/src/transformer.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,664 +1,676 @@
-use std::{ops::DerefMut, sync::Arc};
+use std::time::Instant;
 
 use crate::{
-    atom::{Atom, AtomView, FunctionBuilder, Symbol},
+    atom::{Atom, AtomView, Symbol},
     coefficient::{Coefficient, CoefficientView},
-    combinatorics::CombinationWithReplacementIterator,
-    domains::{atom::AtomField, integer::Integer, rational::Rational},
-    poly::{series::Series, Variable},
+    combinatorics::{partitions, unique_permutations},
+    domains::rational::Rational,
+    id::{Condition, MatchSettings, Pattern, Replacement, WildcardAndRestriction},
+    printer::{AtomPrinter, PrintOptions},
     state::{State, Workspace},
 };
+use ahash::HashMap;
+use colored::Colorize;
+use dyn_clone::DynClone;
+
+pub trait Map:
+    Fn(AtomView, &mut Atom) -> Result<(), TransformerError> + DynClone + Send + Sync
+{
+}
+dyn_clone::clone_trait_object!(Map);
+impl<T: Clone + Send + Sync + Fn(AtomView<'_>, &mut Atom) -> Result<(), TransformerError>> Map
+    for T
+{
+}
 
-impl Atom {
-    /// Take a derivative of the expression with respect to `x`.
-    pub fn derivative(&self, x: Symbol) -> Atom {
-        self.as_view().derivative(x)
-    }
-
-    /// Take a derivative of the expression with respect to `x` and
-    /// write the result in `out`.
-    /// Returns `true` if the derivative is non-zero.
-    pub fn derivative_into(&self, x: Symbol, out: &mut Atom) -> bool {
-        self.as_view().derivative_into(x, out)
-    }
-
-    /// Series expand in `x` around `expansion_point` to depth `depth`.
-    pub fn series(
-        &self,
-        x: Symbol,
-        expansion_point: AtomView,
-        depth: Rational,
-    ) -> Result<Series<AtomField>, &'static str> {
-        self.as_view().series(x, expansion_point, depth)
-    }
+#[derive(Clone, Debug)]
+pub struct StatsOptions {
+    pub tag: String,
+    pub color_medium_change_threshold: Option<f64>,
+    pub color_large_change_threshold: Option<f64>,
 }
 
-impl<'a> AtomView<'a> {
-    /// Take a derivative of the expression with respect to `x`.
-    pub fn derivative(&self, x: Symbol) -> Atom {
-        Workspace::get_local().with(|ws| {
-            let mut out = ws.new_atom();
-            self.derivative_with_ws_into(x, ws, &mut out);
-            out.into_inner()
-        })
-    }
-
-    /// Take a derivative of the expression with respect to `x` and
-    /// write the result in `out`.
-    /// Returns `true` if the derivative is non-zero.
-    pub fn derivative_into(&self, x: Symbol, out: &mut Atom) -> bool {
-        Workspace::get_local().with(|ws| self.derivative_with_ws_into(x, ws, out))
-    }
-
-    /// Take a derivative of the expression with respect to `x` and
-    /// write the result in `out`.
-    /// Returns `true` if the derivative is non-zero.
-    pub fn derivative_with_ws_into(
-        &self,
-        x: Symbol,
-        workspace: &Workspace,
-        out: &mut Atom,
-    ) -> bool {
-        match self {
-            AtomView::Num(_) => {
-                out.to_num(Coefficient::zero());
-                false
+impl StatsOptions {
+    pub fn format_size(&self, size: usize) -> String {
+        let mut s = size as f64;
+        let kb = 1024.;
+        let tag = [" ", "K", "M", "G", "T"];
+
+        for t in tag {
+            if s < kb {
+                return format!("{:.2}{}B", s, t);
             }
-            AtomView::Var(v) => {
-                if v.get_symbol() == x {
-                    out.to_num(1.into());
-                    true
-                } else {
-                    out.to_num(Coefficient::zero());
 
-                    false
-                }
-            }
-            AtomView::Fun(f_orig) => {
-                // detect if the function to derive is the derivative function itself
-                // if so, derive the last argument of the derivative function and set
-                // a flag to later accumulate previous derivatives
-                let (to_derive, f, is_der) = if f_orig.get_symbol() == State::DERIVATIVE {
-                    let to_derive = f_orig.iter().last().unwrap();
-                    (
-                        to_derive,
-                        match to_derive {
-                            AtomView::Fun(f) => f,
-                            _ => panic!("Last argument of der function must be a function"),
-                        },
-                        true,
-                    )
-                } else {
-                    (*self, *f_orig, false)
-                };
+            s /= kb;
+        }
 
-                // take derivative of all the arguments and store it in a list
-                let mut args_der = Vec::with_capacity(f.get_nargs());
-                for (i, arg) in f.iter().enumerate() {
-                    let mut arg_der = workspace.new_atom();
-                    if arg.derivative_with_ws_into(x, workspace, &mut arg_der) {
-                        args_der.push((i, arg_der));
-                    }
-                }
+        format!("{:.2}EB", s)
+    }
 
-                if args_der.is_empty() {
-                    out.to_num(Coefficient::zero());
-                    return false;
-                }
+    pub fn format_count(&self, count: usize) -> String {
+        format!("{}", count)
+    }
+}
 
-                // derive special functions
-                if f.get_nargs() == 1
-                    && [State::EXP, State::LOG, State::SIN, State::COS].contains(&f.get_symbol())
-                {
-                    let mut fn_der = workspace.new_atom();
-                    match f.get_symbol() {
-                        State::EXP => {
-                            fn_der.set_from_view(self);
-                        }
-                        State::LOG => {
-                            let mut n = workspace.new_atom();
-                            n.to_num((-1).into());
+#[derive(Clone, Debug)]
+pub enum TransformerError {
+    ValueError(String),
+    Interrupt,
+}
 
-                            fn_der.to_pow(f.iter().next().unwrap(), n.as_view());
-                        }
-                        State::SIN => {
-                            let p = fn_der.to_fun(State::COS);
-                            p.add_arg(f.iter().next().unwrap());
-                        }
-                        State::COS => {
-                            let mut n = workspace.new_atom();
-                            n.to_num((-1).into());
+/// Operations that take a pattern as the input and produce an expression
+#[derive(Clone)]
+pub enum Transformer {
+    /// Expand the rhs.
+    Expand(Option<Symbol>),
+    /// Derive the rhs w.r.t a variable.
+    Derivative(Symbol),
+    /// Derive the rhs w.r.t a variable.
+    Series(Symbol, Atom, Rational),
+    /// Apply find-and-replace on the lhs.
+    ReplaceAll(
+        Pattern,
+        Pattern,
+        Condition<WildcardAndRestriction>,
+        MatchSettings,
+    ),
+    /// Apply multiple find-and-replace on the lhs.
+    ReplaceAllMultiple(
+        Vec<(
+            Pattern,
+            Pattern,
+            Condition<WildcardAndRestriction>,
+            MatchSettings,
+        )>,
+    ),
+    /// Take the product of a list of arguments in the rhs.
+    Product,
+    /// Take the sum of a list of arguments in the rhs.
+    Sum,
+    /// Return the number of arguments of a function in the input.
+    /// If the argument of `ArgCount` is `true`, only the number
+    /// of arguments of `arg()` is returned and 1 is returned otherwise.
+    /// If the argument is `false`, 0 is returned for non-functions.
+    ArgCount(bool),
+    /// Map the rhs with a user-specified function.
+    Map(Box<dyn Map>),
+    /// Apply a transformation to each argument of the `arg()` function.
+    /// If the input is not `arg()`, map the current input.
+    ForEach(Vec<Transformer>),
+    /// Split a `Mul` or `Add` into a list of arguments.
+    Split,
+    Partition(Vec<(Symbol, usize)>, bool, bool),
+    Sort,
+    Deduplicate,
+    Permutations(Symbol),
+    Repeat(Vec<Transformer>),
+    Print(PrintOptions),
+    Stats(StatsOptions, Vec<Transformer>),
+    FromNumber,
+}
+
+impl std::fmt::Debug for Transformer {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        match self {
+            Transformer::Expand(s) => f.debug_tuple("Expand").field(s).finish(),
+            Transformer::Derivative(x) => f.debug_tuple("Derivative").field(x).finish(),
+            Transformer::ReplaceAll(pat, rhs, ..) => {
+                f.debug_tuple("ReplaceAll").field(pat).field(rhs).finish()
+            }
+            Transformer::ReplaceAllMultiple(pats) => {
+                f.debug_tuple("ReplaceAllMultiple").field(pats).finish()
+            }
+            Transformer::Product => f.debug_tuple("Product").finish(),
+            Transformer::Sum => f.debug_tuple("Sum").finish(),
+            Transformer::ArgCount(p) => f.debug_tuple("ArgCount").field(p).finish(),
+            Transformer::Map(_) => f.debug_tuple("Map").finish(),
+            Transformer::ForEach(t) => f.debug_tuple("ForEach").field(t).finish(),
+            Transformer::Split => f.debug_tuple("Split").finish(),
+            Transformer::Partition(g, b1, b2) => f
+                .debug_tuple("Partition")
+                .field(g)
+                .field(b1)
+                .field(b2)
+                .finish(),
+            Transformer::Sort => f.debug_tuple("Sort").finish(),
+            Transformer::Deduplicate => f.debug_tuple("Deduplicate").finish(),
+            Transformer::Permutations(i) => f.debug_tuple("Permutations").field(i).finish(),
+            Transformer::Series(x, point, d) => f
+                .debug_tuple("TaylorSeries")
+                .field(x)
+                .field(point)
+                .field(d)
+                .finish(),
+            Transformer::Repeat(r) => f.debug_tuple("Repeat").field(r).finish(),
+            Transformer::Print(p) => f.debug_tuple("Print").field(p).finish(),
+            Transformer::Stats(o, r) => f.debug_tuple("Timing").field(o).field(r).finish(),
+            Transformer::FromNumber => f.debug_tuple("FromNumber").finish(),
+        }
+    }
+}
 
-                            let mut sin = workspace.new_atom();
-                            let sin_fun = sin.to_fun(State::SIN);
-                            sin_fun.add_arg(f.iter().next().unwrap());
+impl Transformer {
+    /// Create a new partition transformer that must exactly fit the input.
+    pub fn new_partition_exact(partitions: Vec<(Symbol, usize)>) -> Transformer {
+        Transformer::Partition(partitions, false, false)
+    }
+
+    /// Create a new partition transformer that collects all left-over
+    /// atoms in the last bin.
+    pub fn new_partition_collect_in_last(
+        mut partitions: Vec<(Symbol, usize)>,
+        rest: Symbol,
+    ) -> Transformer {
+        partitions.push((rest, 0));
+        Transformer::Partition(partitions, true, false)
+    }
+
+    /// Create a new partition transformer that repeats the partitions so that it can fit
+    /// the input.
+    pub fn new_partition_repeat(partition: (Symbol, usize)) -> Transformer {
+        Transformer::Partition(vec![partition], false, true)
+    }
+
+    pub fn execute(
+        orig_input: AtomView<'_>,
+        chain: &[Transformer],
+        workspace: &Workspace,
+        out: &mut Atom,
+    ) -> Result<(), TransformerError> {
+        out.set_from_view(&orig_input);
+        let mut tmp = workspace.new_atom();
+        for t in chain {
+            std::mem::swap(out, &mut tmp);
+            let input = tmp.as_view();
+
+            match t {
+                Transformer::Map(f) => {
+                    f(input, out)?;
+                }
+                Transformer::ForEach(t) => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let mut ff = workspace.new_atom();
+                            let ff = ff.to_fun(State::ARG);
+
+                            let mut a = workspace.new_atom();
+                            for arg in f.iter() {
+                                Self::execute(arg, t, workspace, &mut a)?;
+                                ff.add_arg(a.as_view());
+                            }
 
-                            let m = fn_der.to_mul();
-                            m.extend(sin.as_view());
-                            m.extend(n.as_view());
+                            ff.as_view().normalize(workspace, out);
+                            continue;
                         }
-                        _ => unreachable!(),
                     }
 
-                    let (_, mut arg_der) = args_der.pop().unwrap();
-                    if let Atom::Mul(m) = arg_der.deref_mut() {
-                        m.extend(fn_der.as_view());
-                        arg_der.as_view().normalize(workspace, out);
-                    } else {
-                        let mut mul = workspace.new_atom();
-                        let m = mul.to_mul();
-                        m.extend(fn_der.as_view());
-                        m.extend(arg_der.as_view());
-                        mul.as_view().normalize(workspace, out);
-                    }
-
-                    return true;
-                }
-
-                // create a derivative function that tags which index was derived
-                let mut add = workspace.new_atom();
-                let a = add.to_add();
-                let mut fn_der = workspace.new_atom();
-                let mut n = workspace.new_atom();
-                let mut mul = workspace.new_atom();
-                for (index, arg_der) in args_der {
-                    let p = fn_der.to_fun(State::DERIVATIVE);
-
-                    if is_der {
-                        for (i, x_orig) in f_orig.iter().take(f.get_nargs()).enumerate() {
-                            if let AtomView::Num(nn) = x_orig {
-                                let num = nn.get_coeff_view() + (if i == index { 1 } else { 0 });
-                                n.to_num(num);
-                                p.add_arg(n.as_view());
-                            } else {
-                                panic!("Derivative function must contain numbers for all but the last position");
-                            }
-                        }
+                    Self::execute(input, t, workspace, out)?;
+                }
+                Transformer::Expand(s) => {
+                    input.expand_with_ws_into(workspace, *s, out);
+                }
+                Transformer::Derivative(x) => {
+                    input.derivative_with_ws_into(*x, workspace, out);
+                }
+                Transformer::Series(x, expansion_point, depth) => {
+                    if let Ok(s) = input.series(*x, expansion_point.as_view(), depth.clone()) {
+                        s.to_atom_into(out);
                     } else {
-                        for i in 0..f.get_nargs() {
-                            n.to_num((if i == index { 1 } else { 0 }, 1).into());
-                            p.add_arg(n.as_view());
-                        }
+                        out.set_from_view(&input);
                     }
-
-                    p.add_arg(to_derive);
-
-                    let m = mul.to_mul();
-                    m.extend(fn_der.as_view());
-                    m.extend(arg_der.as_view());
-                    mul.as_view().normalize(workspace, out);
-
-                    a.extend(mul.as_view());
                 }
+                Transformer::ReplaceAll(pat, rhs, cond, settings) => {
+                    pat.replace_all_with_ws_into(
+                        input,
+                        rhs,
+                        workspace,
+                        cond.into(),
+                        settings.into(),
+                        out,
+                    );
+                }
+                Transformer::ReplaceAllMultiple(replacements) => {
+                    let reps = replacements
+                        .iter()
+                        .map(|(pat, rhs, cond, settings)| {
+                            Replacement::new(&pat, &rhs)
+                                .with_conditions(&cond)
+                                .with_settings(&settings)
+                        })
+                        .collect::<Vec<_>>();
+                    input.replace_all_multiple_into(&reps, out);
+                }
+                Transformer::Product => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let mut mul_h = workspace.new_atom();
+                            let mul = mul_h.to_mul();
 
-                add.as_view().normalize(workspace, out);
-                true
-            }
-            AtomView::Pow(p) => {
-                let (base, exp) = p.get_base_exp();
-
-                let mut exp_der = workspace.new_atom();
-                let exp_der_non_zero = exp.derivative_with_ws_into(x, workspace, &mut exp_der);
+                            for arg in f.iter() {
+                                mul.extend(arg);
+                            }
 
-                let mut base_der = workspace.new_atom();
-                let base_der_non_zero = base.derivative_with_ws_into(x, workspace, &mut base_der);
+                            mul_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
+                    }
 
-                if !exp_der_non_zero && !base_der_non_zero {
-                    out.to_num(0.into());
-                    return false;
+                    out.set_from_view(&input);
                 }
+                Transformer::Sum => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let mut add_h = workspace.new_atom();
+                            let add = add_h.to_add();
 
-                let mut exp_der_contrib = workspace.new_atom();
-
-                if exp_der_non_zero {
-                    // create log(base)
-                    let mut log_base = workspace.new_atom();
-                    let lb = log_base.to_fun(State::LOG);
-                    lb.add_arg(base);
+                            for arg in f.iter() {
+                                add.extend(arg);
+                            }
 
-                    if let Atom::Mul(m) = exp_der.deref_mut() {
-                        m.extend(*self);
-                        m.extend(log_base.as_view());
-                        exp_der.as_view().normalize(workspace, &mut exp_der_contrib);
-                    } else {
-                        let mut mul = workspace.new_atom();
-                        let m = mul.to_mul();
-                        m.extend(*self);
-                        m.extend(exp_der.as_view());
-                        m.extend(log_base.as_view());
-                        mul.as_view().normalize(workspace, &mut exp_der_contrib);
+                            add_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
                     }
 
-                    if !base_der_non_zero {
-                        out.set_from_view(&exp_der_contrib.as_view());
-                        return true;
+                    out.set_from_view(&input);
+                }
+                Transformer::ArgCount(only_for_arg_fun) => {
+                    if let AtomView::Fun(f) = input {
+                        if !*only_for_arg_fun || f.get_symbol() == State::ARG {
+                            let n_args = f.get_nargs();
+                            out.to_num((n_args as i64).into());
+                        } else {
+                            out.to_num(1.into());
+                        }
+                    } else if !only_for_arg_fun {
+                        out.to_num(1.into());
+                    } else {
+                        out.to_num(Coefficient::zero());
                     }
                 }
+                Transformer::Split => match input {
+                    AtomView::Mul(m) => {
+                        let mut arg_h = workspace.new_atom();
+                        let arg = arg_h.to_fun(State::ARG);
 
-                let mut mul_h = workspace.new_atom();
-                let mul = mul_h.to_mul();
-                mul.extend(base_der.as_view());
+                        for factor in m.iter() {
+                            arg.add_arg(factor);
+                        }
 
-                let mut new_exp = workspace.new_atom();
-                if let AtomView::Num(n) = exp {
-                    mul.extend(exp);
+                        arg_h.as_view().normalize(workspace, out);
+                        continue;
+                    }
+                    AtomView::Add(a) => {
+                        let mut arg_h = workspace.new_atom();
+                        let arg = arg_h.to_fun(State::ARG);
 
-                    let res = n.get_coeff_view() + -1;
-                    new_exp.to_num(res);
-                } else {
-                    mul.extend(exp);
+                        for summand in a.iter() {
+                            arg.add_arg(summand);
+                        }
 
-                    let ao = new_exp.to_add();
-                    ao.extend(exp);
+                        arg_h.as_view().normalize(workspace, out);
+                        continue;
+                    }
+                    _ => {
+                        out.set_from_view(&input);
+                    }
+                },
+                Transformer::Partition(bins, fill_last, repeat) => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let args: Vec<_> = f.iter().collect();
+
+                            let mut sum_h = workspace.new_atom();
+                            let sum = sum_h.to_add();
+
+                            let partitions = partitions(&args, bins, *fill_last, *repeat);
+
+                            if partitions.is_empty() {
+                                out.set_from_view(&workspace.new_num(0).as_view());
+                                continue;
+                            }
 
-                    let mut min_one = workspace.new_atom();
-                    min_one.to_num((-1).into());
+                            for (p, args) in partitions {
+                                let mut mul_h = workspace.new_atom();
+                                let mul = mul_h.to_mul();
 
-                    ao.extend(min_one.as_view());
-                }
+                                if !p.is_one() {
+                                    mul.extend(workspace.new_num(p).as_view());
+                                }
 
-                let mut pow_h = workspace.new_atom();
-                pow_h.to_pow(base, new_exp.as_view());
+                                for (name, f_args) in args {
+                                    let mut fun_h = workspace.new_atom();
+                                    let fun = fun_h.to_fun(name);
+                                    for x in f_args {
+                                        fun.add_arg(x);
+                                    }
 
-                mul.extend(pow_h.as_view());
+                                    mul.extend(fun_h.as_view());
+                                }
 
-                if exp_der_non_zero {
-                    let mut add = workspace.new_atom();
-                    let a = add.to_add();
+                                sum.extend(mul_h.as_view());
+                            }
 
-                    a.extend(mul_h.as_view());
-                    a.extend(exp_der_contrib.as_view());
+                            sum_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
+                    }
 
-                    add.as_view().normalize(workspace, out);
-                } else {
-                    mul_h.as_view().normalize(workspace, out);
+                    out.set_from_view(&input);
                 }
+                Transformer::Sort => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let mut args: Vec<_> = f.iter().collect();
+                            args.sort();
 
-                true
-            }
-            AtomView::Mul(args) => {
-                let mut add_h = workspace.new_atom();
-                let add = add_h.to_add();
-                let mut mul_h = workspace.new_atom();
-                let mut non_zero = false;
-                for arg in args.iter() {
-                    let mut arg_der = workspace.new_atom();
-                    if arg.derivative_with_ws_into(x, workspace, &mut arg_der) {
-                        if let Atom::Mul(mm) = arg_der.deref_mut() {
-                            for other_arg in args.iter() {
-                                if other_arg != arg {
-                                    mm.extend(other_arg);
-                                }
-                            }
+                            let mut fun_h = workspace.new_atom();
+                            let fun = fun_h.to_fun(State::ARG);
 
-                            add.extend(arg_der.as_view());
-                        } else {
-                            let mm = mul_h.to_mul();
-                            mm.extend(arg_der.as_view());
-                            for other_arg in args.iter() {
-                                if other_arg != arg {
-                                    mm.extend(other_arg);
-                                }
+                            for arg in args {
+                                fun.add_arg(arg);
                             }
-                            add.extend(mul_h.as_view());
-                        }
 
-                        non_zero = true;
-                    }
-                }
-
-                if non_zero {
-                    add_h.as_view().normalize(workspace, out);
-                    true
-                } else {
-                    out.to_num(0.into());
-                    false
-                }
-            }
-            AtomView::Add(args) => {
-                let mut add_h = workspace.new_atom();
-                let add = add_h.to_add();
-                let mut arg_der = workspace.new_atom();
-                let mut non_zero = false;
-                for arg in args.iter() {
-                    if arg.derivative_with_ws_into(x, workspace, &mut arg_der) {
-                        add.extend(arg_der.as_view());
-                        non_zero = true;
+                            fun_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
                     }
-                }
 
-                if non_zero {
-                    add_h.as_view().normalize(workspace, out);
-                    true
-                } else {
-                    out.to_num(0.into());
-                    false
+                    out.set_from_view(&input);
                 }
-            }
-        }
-    }
+                Transformer::Deduplicate => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let args: Vec<_> = f.iter().collect();
+                            let mut args_dedup: Vec<_> = Vec::with_capacity(args.len());
+
+                            for a in args {
+                                // check last argument first, so that the sorted list case is fast
+                                if args_dedup.last() != Some(&a) && !args_dedup.contains(&a) {
+                                    args_dedup.push(a);
+                                }
+                            }
 
-    /// Series expand in `x` around `expansion_point` to depth `depth`.
-    pub fn series(
-        &self,
-        x: Symbol,
-        expansion_point: AtomView,
-        depth: Rational,
-    ) -> Result<Series<AtomField>, &'static str> {
-        // heuristic current depth
-        let mut current_depth = if depth.is_negative() {
-            Rational::one()
-        } else {
-            depth.clone()
-        };
-        Workspace::get_local().with(|ws| loop {
-            let info = Series::new(
-                &AtomField::new(),
-                None,
-                if expansion_point.is_zero() {
-                    Arc::new(Variable::Symbol(x))
-                } else {
-                    Arc::new(Variable::Other(Arc::new(
-                        Atom::new_var(x) - &expansion_point.to_owned(),
-                    )))
-                },
-                &current_depth + &((1.into(), current_depth.denominator())).into(),
-            );
+                            let mut fun_h = workspace.new_atom();
+                            let fun = fun_h.to_fun(State::ARG);
 
-            let mut series = self.series_with_ws(x, expansion_point, ws, &info)?;
-            if series.absolute_order() > depth {
-                series.truncate_absolute_order(&depth + &((1.into(), depth.denominator())).into());
-                break Ok(series);
-            } else {
-                // increase the expansion depth
-                // TODO: find better heuristic
-                current_depth = &current_depth * &2.into();
-            }
-        })
-    }
+                            for arg in args_dedup {
+                                fun.add_arg(arg);
+                            }
 
-    /// Series expand in `x` around `expansion_point` to depth `depth`.
-    pub fn series_with_ws(
-        &self,
-        x: Symbol,
-        expansion_point: AtomView,
-        workspace: &Workspace,
-        info: &Series<AtomField>,
-    ) -> Result<Series<AtomField>, &'static str> {
-        if !self.contains_symbol(x) {
-            return Ok(info.constant(self.to_owned().into()));
-        }
+                            fun_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
+                    }
 
-        // TODO: optimize, appending a monomial using addition is slow
-        match self {
-            AtomView::Num(n) => Ok(info.constant(n.to_owned().into())),
-            AtomView::Var(v) => {
-                if v.get_symbol() == x {
-                    Ok(info.shifted_variable(expansion_point.to_owned()))
-                } else {
-                    Ok(info.constant(v.to_owned().into()))
-                }
-            }
-            AtomView::Fun(f) => {
-                let mut args_series = Vec::with_capacity(f.get_nargs());
-                for arg in f.iter() {
-                    args_series.push(arg.series_with_ws(x, expansion_point, workspace, info)?);
+                    out.set_from_view(&input);
                 }
+                Transformer::Permutations(f_name) => {
+                    if let AtomView::Fun(f) = input {
+                        if f.get_symbol() == State::ARG {
+                            let args: Vec<_> = f.iter().collect();
 
-                match f.get_symbol() {
-                    State::COS => args_series[0].cos(),
-                    State::SIN => args_series[0].sin(),
-                    State::EXP => args_series[0].exp(),
-                    State::LOG => args_series[0].log(),
-                    State::SQRT => Ok(args_series[0].rpow((1, 2).into())),
-                    _ => {
-                        // TODO: also check for log(x)?
-                        if args_series
-                            .iter()
-                            .any(|x| x.get_trailing_exponent().is_negative())
-                        {
-                            return Err("Cannot series expand custom function with poles");
-                        }
-
-                        // TODO: depth is an overestimate
-                        let order = info.absolute_order();
-                        let depth = order.numerator().to_i64().unwrap() as u32
-                            * order.denominator().to_i64().unwrap() as u32;
-
-                        // strip the constant terms
-                        let mut constants = vec![];
-                        for x in &mut args_series {
-                            if x.get_trailing_exponent().is_zero() {
-                                let c = x.get_trailing_coefficient();
-                                *x = &*x - &x.constant(c.clone());
-                                constants.push(c);
-                            } else {
-                                constants.push(Atom::new_num(0));
-                            }
-                        }
+                            let mut sum_h = workspace.new_atom();
+                            let sum = sum_h.to_add();
 
-                        let mut f_eval = FunctionBuilder::new(f.get_symbol());
-                        for c in &constants {
-                            f_eval = f_eval.add_arg(c);
-                        }
-                        let constant = f_eval.finish();
+                            let (prefactor, permutations) = unique_permutations(&args);
 
-                        let mut result = info.constant(constant.clone());
-                        for i in 0..=depth {
-                            let mut it =
-                                CombinationWithReplacementIterator::new(args_series.len(), i);
+                            if permutations.is_empty() {
+                                out.set_from_view(&workspace.new_num(0).as_view());
+                                continue;
+                            }
 
-                            while let Some(x) = it.next() {
-                                let mut f_der = FunctionBuilder::new(State::DERIVATIVE);
-                                let mut term = info.one();
-                                for (arg, pow) in x.iter().enumerate() {
-                                    term = &term * &args_series[arg].npow(*pow as usize);
-                                    f_der = f_der.add_arg(&Atom::new_num(*pow as i64));
+                            for a in permutations {
+                                let mut fun_h = workspace.new_atom();
+                                let fun = fun_h.to_fun(*f_name);
+                                for x in a {
+                                    fun.add_arg(x);
                                 }
 
-                                f_der = f_der.add_arg(&constant);
-
-                                result = &result
-                                    + &term
-                                        .mul_coeff(&f_der.finish())
-                                        .mul_coeff(&Atom::new_num(Integer::multinom(x)))
-                                        .div_coeff(&Atom::new_num(Integer::factorial(i)));
+                                if !prefactor.is_one() {
+                                    let mut mul_h = workspace.new_atom();
+                                    let mul = mul_h.to_mul();
+                                    mul.extend(fun_h.as_view());
+                                    mul.extend(workspace.new_num(prefactor.clone()).as_view());
+                                    sum.extend(mul_h.as_view());
+                                } else {
+                                    sum.extend(fun_h.as_view());
+                                }
                             }
-                        }
 
-                        Ok(result)
+                            sum_h.as_view().normalize(workspace, out);
+                            continue;
+                        }
                     }
+
+                    out.set_from_view(&input);
                 }
-            }
-            AtomView::Pow(p) => {
-                let (base, exp) = p.get_base_exp();
+                Transformer::Repeat(r) => loop {
+                    Self::execute(tmp.as_view(), r, workspace, out)?;
+
+                    if tmp.as_view() == out.as_view() {
+                        break;
+                    }
 
-                let base_series = base.series_with_ws(x, expansion_point, workspace, info)?;
+                    std::mem::swap(out, &mut tmp);
+                },
+                Transformer::Print(o) => {
+                    println!("{}", AtomPrinter::new_with_options(input, *o));
+                    out.set_from_view(&input);
+                }
+                Transformer::Stats(o, r) => {
+                    let in_nterms = if let AtomView::Add(a) = input {
+                        a.get_nargs()
+                    } else {
+                        1
+                    };
+                    let in_size = input.get_byte_size();
+
+                    let t = Instant::now();
+                    Self::execute(input, r, workspace, out)?;
 
-                if let AtomView::Num(n) = exp {
-                    if let CoefficientView::Natural(n, d) = n.get_coeff_view() {
-                        Ok(base_series.rpow((n, d).into()))
+                    let out_nterms = if let AtomView::Add(a) = out.as_view() {
+                        a.get_nargs()
                     } else {
-                        unimplemented!("Cannot series expand with large exponents yet")
+                        1
+                    };
+                    let out_size = out.as_view().get_byte_size();
+
+                    let in_nterms_s = o.format_count(in_nterms);
+                    let out_nterms_s = o.format_count(out_nterms);
+
+                    println!(
+                        "Stats for {}:
+\tIn  │ {:>width$} │ {:>8} │
+\tOut │ {:>width$} │ {:>8} │ ⧗ {:#.2?}",
+                        o.tag.bold(),
+                        in_nterms_s,
+                        o.format_size(in_size),
+                        if out_nterms as f64 / in_nterms as f64
+                            > o.color_medium_change_threshold.unwrap_or(f64::INFINITY)
+                        {
+                            if out_nterms as f64 / in_nterms as f64
+                                > o.color_large_change_threshold.unwrap_or(f64::INFINITY)
+                            {
+                                out_nterms_s.red()
+                            } else {
+                                out_nterms_s.bright_magenta()
+                            }
+                        } else {
+                            out_nterms_s.as_str().into()
+                        },
+                        o.format_size(out_size),
+                        Instant::now().duration_since(t),
+                        width = in_nterms_s.len().max(out_nterms_s.len()).min(6),
+                    );
+                }
+                Transformer::FromNumber => {
+                    if let AtomView::Num(n) = input {
+                        if let CoefficientView::RationalPolynomial(r) = n.get_coeff_view() {
+                            r.deserialize().to_expression_with_map(
+                                workspace,
+                                &HashMap::default(),
+                                out,
+                            );
+                            continue;
+                        }
                     }
-                } else {
-                    let e = exp.series_with_ws(x, expansion_point, workspace, info)?;
-                    base_series.pow(&e)
-                }
-            }
-            AtomView::Mul(args) => {
-                let mut series = info.one();
-                for arg in args.iter() {
-                    series = &series * &arg.series_with_ws(x, expansion_point, workspace, info)?;
-                }
 
-                Ok(series)
-            }
-            AtomView::Add(args) => {
-                let mut series = info.zero();
-                for arg in args.iter() {
-                    series = &series + &arg.series_with_ws(x, expansion_point, workspace, info)?;
+                    out.set_from_view(&input);
                 }
-
-                Ok(series)
             }
         }
+
+        Ok(())
     }
 }
 
 #[cfg(test)]
 mod test {
-    use crate::{atom::Atom, state::State};
+    use crate::{
+        atom::{Atom, FunctionBuilder},
+        id::{Condition, Match, MatchSettings, Pattern, PatternRestriction},
+        printer::PrintOptions,
+        state::{State, Workspace},
+        transformer::StatsOptions,
+    };
 
-    #[test]
-    fn derivative() {
-        let v1 = State::get_symbol("v1");
-        let inputs = [
-            "(1+2*v1)^(5+v1)",
-            "log(2*v1) + exp(3*v1) + sin(4*v1) + cos(y*v1)",
-            "f(v1^2,v1)",
-            "der(0,1,f(v1,v1^3))",
-        ];
-        let r = inputs.map(|input| Atom::parse(input).unwrap().derivative(v1));
-
-        let res = [
-            "(2*v1+1)^(v1+5)*log(2*v1+1)+2*(v1+5)*(2*v1+1)^(v1+4)",
-            "2*(2*v1)^-1+3*exp(3*v1)+4*cos(4*v1)-y*sin(v1*y)",
-            "der(0,1,f(v1^2,v1))+2*v1*der(1,0,f(v1^2,v1))",
-            "der(1,1,f(v1,v1^3))+3*v1^2*der(0,2,f(v1,v1^3))",
-        ];
-        let res = res.map(|input| Atom::parse(input).unwrap());
-
-        assert_eq!(r, res);
-    }
-
-    #[test]
-    fn series() {
-        let v1 = State::get_symbol("v1");
-
-        let input = Atom::parse("exp(v1^2+1)*log(v1+3)/v1/(v1+1)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 2.into())
-            .unwrap()
-            .to_atom();
-
-        let res = Atom::parse(
-            "1/3*exp(1)+v1*(-7/18*exp(1)+2*exp(1)*log(3))+v1^2*(119/162*exp(1)-2*exp(1)*log(3))-exp(1)*log(3)+v1^-1*exp(1)*log(3)",
-        )
-        .unwrap();
-        assert_eq!(t, res);
-    }
+    use super::Transformer;
 
     #[test]
-    fn series_shift() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("1/(v1+1)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(-1).as_view(), 5.into())
-            .unwrap()
-            .to_atom();
+    fn expand_derivative() {
+        let p = Atom::parse("(1+v1)^2").unwrap();
 
-        let res = Atom::parse("1/(v1+1)").unwrap();
-        assert_eq!(t, res);
-    }
-
-    #[test]
-    fn series_spurious_pole() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("(1-cos(v1))/sin(v1)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 5.into())
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            Transformer::execute(
+                p.as_view(),
+                &[
+                    Transformer::Expand(Some(State::get_symbol("v1"))),
+                    Transformer::Derivative(State::get_symbol("v1")),
+                ],
+                ws,
+                &mut out,
+            )
             .unwrap()
-            .to_atom();
+        });
 
-        let res = Atom::parse("1/2*v1+1/24*v1^3+1/240*v1^5").unwrap();
-        assert_eq!(t, res);
+        let r = Atom::parse("2+2*v1").unwrap();
+        assert_eq!(out, r);
     }
 
     #[test]
-    fn series_logx() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("log(v1)*(1+v1)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 4.into())
-            .unwrap()
-            .to_atom();
+    fn split_argcount() {
+        let p = Atom::parse("v1+v2+v3").unwrap();
 
-        let res = Atom::parse("log(v1)+v1*log(v1)").unwrap();
-        assert_eq!(t, res);
-    }
-
-    #[test]
-    fn series_sqrt() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("(v1^3+v1+1)^(1/2)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 4.into())
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            Transformer::execute(
+                p.as_view(),
+                &[Transformer::Split, Transformer::ArgCount(true)],
+                ws,
+                &mut out,
+            )
             .unwrap()
-            .to_atom();
+        });
 
-        let res = Atom::parse("1+1/2*v1-1/8*v1^2+9/16*v1^3-37/128*v1^4").unwrap();
-        assert_eq!(t, res);
+        let r = Atom::parse("3").unwrap();
+        assert_eq!(out, r);
     }
 
     #[test]
-    fn series_fractions() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("1/v1^5").unwrap();
-
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 3.into())
-            .unwrap();
+    fn product_series() {
+        let p = Atom::parse("arg(v1,v1+1,3)").unwrap();
 
-        let t2 = t.rpow((1, 3).into());
-
-        assert_eq!(t2.absolute_order(), (22, 3).into());
-    }
-
-    #[test]
-    fn series_poles() {
-        let v1 = State::get_symbol("v1");
-        let input = Atom::parse("1/(v1^10+v1^20)").unwrap();
-
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), (-1).into())
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            Transformer::execute(
+                p.as_view(),
+                &[
+                    Transformer::Product,
+                    Transformer::Series(State::get_symbol("v1"), Atom::new_num(1), 3.into()),
+                ],
+                ws,
+                &mut out,
+            )
             .unwrap()
-            .to_atom();
-
-        println!("t={}", t);
+        });
 
-        assert_eq!(t, Atom::parse("v1^-10").unwrap())
+        let r = Atom::parse("3*(v1-1)^2+9*(v1-1)+6").unwrap();
+        assert_eq!(out, r);
     }
 
     #[test]
-    fn series_user_function() {
-        let v1 = State::get_symbol("v1");
+    fn sort_deduplicate() {
+        let p = Atom::parse("f1(3,2,1,3)").unwrap();
 
-        let input = Atom::parse("f(exp(v1),sin(v1))").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 2.into())
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            Transformer::execute(
+                p.as_view(),
+                &[
+                    Transformer::ReplaceAll(
+                        Pattern::parse("f1(x__)").unwrap(),
+                        Pattern::parse("x__").unwrap(),
+                        Condition::default(),
+                        MatchSettings::default(),
+                    ),
+                    Transformer::Sort,
+                    Transformer::Deduplicate,
+                    Transformer::Map(Box::new(|x, out| {
+                        let mut f = FunctionBuilder::new(State::get_symbol("f1"));
+                        f = f.add_arg(x);
+                        *out = f.finish();
+                        Ok(())
+                    })),
+                ],
+                ws,
+                &mut out,
+            )
             .unwrap()
-            .to_atom();
+        });
 
-        let res = Atom::parse(
-            "der(0,0,f(1,0))+f(1,0)+v1*(der(0,1,f(1,0))+der(1,0,f(1,0)))
-            +v1^2*(1/2*der(0,2,f(1,0))+1/2*der(1,0,f(1,0))+der(1,1,f(1,0))+1/2*der(2,0,f(1,0)))",
-        )
-        .unwrap();
-        assert_eq!(t, res);
+        let r = Atom::parse("f1(1,2,3)").unwrap();
+        assert_eq!(out, r);
     }
 
     #[test]
-    fn series_exp_log() {
-        let v1 = State::get_symbol("v1");
+    fn deep_nesting() {
+        let p = Atom::parse("arg(3,2,1,3)").unwrap();
 
-        let input = Atom::parse("1+2*log(v1^4)").unwrap();
-        let t = input
-            .series(v1, Atom::new_num(0).as_view(), 4.into())
+        let mut out = Atom::new();
+        Workspace::get_local().with(|ws| {
+            Transformer::execute(
+                p.as_view(),
+                &[Transformer::Repeat(vec![Transformer::Stats(
+                    StatsOptions {
+                        tag: "test".to_owned(),
+                        color_medium_change_threshold: Some(10.),
+                        color_large_change_threshold: Some(100.),
+                    },
+                    vec![Transformer::ForEach(vec![
+                        Transformer::Print(PrintOptions::default()),
+                        Transformer::ReplaceAll(
+                            Pattern::parse("x_").unwrap(),
+                            Pattern::parse("x_-1").unwrap(),
+                            (
+                                State::get_symbol("x_"),
+                                PatternRestriction::Filter(Box::new(|x| {
+                                    x != &Match::Single(Atom::new_num(0).as_view())
+                                })),
+                            )
+                                .into(),
+                            MatchSettings::default(),
+                        ),
+                    ])],
+                )])],
+                ws,
+                &mut out,
+            )
             .unwrap()
-            .exp()
-            .unwrap();
+        });
 
-        assert_eq!(t.to_atom().expand(), Atom::parse("v1^8*exp(1)",).unwrap());
+        let r = Atom::parse("arg(0,0,0,0)").unwrap();
+        assert_eq!(out, r);
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `symbolica-0.5.0/src/domains/algebraic_number.rs` & `symbolica-0.6.0/src/domains/algebraic_number.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains/atom.rs` & `symbolica-0.6.0/src/domains/atom.rs`

 * *Files 8% similar despite different names*

```diff
@@ -111,17 +111,21 @@
         true
     }
 
     fn fmt_display(
         &self,
         element: &Self::Element,
         _opts: &crate::printer::PrintOptions,
-        in_product: bool, // can be used to add parentheses
+        mut in_product: bool, // can be used to add parentheses
         f: &mut std::fmt::Formatter<'_>,
     ) -> Result<(), std::fmt::Error> {
+        if !matches!(element.as_view(), AtomView::Add(_)) {
+            in_product = false;
+        }
+
         if in_product {
             write!(f, "(")?;
         }
 
         std::fmt::Display::fmt(element, f)?;
 
         if in_product {
```

### Comparing `symbolica-0.5.0/src/domains/factorized_rational_polynomial.rs` & `symbolica-0.6.0/src/domains/factorized_rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains/finite_field.rs` & `symbolica-0.6.0/src/domains/finite_field.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains/float.rs` & `symbolica-0.6.0/src/domains/float.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 
 pub trait NumericalFloatLike:
     PartialEq
     + Clone
     + std::fmt::Debug
     + std::fmt::Display
     + std::ops::Neg<Output = Self>
-    + for<'a> Add<Self, Output = Self>
-    + for<'a> Sub<Self, Output = Self>
-    + for<'a> Mul<Self, Output = Self>
-    + for<'a> Div<Self, Output = Self>
+    + Add<Self, Output = Self>
+    + Sub<Self, Output = Self>
+    + Mul<Self, Output = Self>
+    + Div<Self, Output = Self>
     + for<'a> Add<&'a Self, Output = Self>
     + for<'a> Sub<&'a Self, Output = Self>
     + for<'a> Mul<&'a Self, Output = Self>
     + for<'a> Div<&'a Self, Output = Self>
     + for<'a> AddAssign<&'a Self>
     + for<'a> SubAssign<&'a Self>
     + for<'a> MulAssign<&'a Self>
@@ -543,14 +543,32 @@
 
     #[inline]
     fn add(self, rhs: &Self) -> Self::Output {
         Complex::new(self.re + rhs.re, self.im + rhs.im)
     }
 }
 
+impl<'a, 'b, T: Real> Add<&'a Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn add(self, rhs: &'a Complex<T>) -> Self::Output {
+        *self + *rhs
+    }
+}
+
+impl<'b, T: Real> Add<Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn add(self, rhs: Complex<T>) -> Self::Output {
+        *self + rhs
+    }
+}
+
 impl<T: Real> AddAssign for Complex<T> {
     #[inline]
     fn add_assign(&mut self, rhs: Self) {
         self.add_assign(&rhs)
     }
 }
 
@@ -576,14 +594,32 @@
 
     #[inline]
     fn sub(self, rhs: &Self) -> Self::Output {
         Complex::new(self.re - rhs.re, self.im - rhs.im)
     }
 }
 
+impl<'a, 'b, T: Real> Sub<&'a Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn sub(self, rhs: &'a Complex<T>) -> Self::Output {
+        *self - *rhs
+    }
+}
+
+impl<'b, T: Real> Sub<Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn sub(self, rhs: Complex<T>) -> Self::Output {
+        *self - rhs
+    }
+}
+
 impl<T: Real> SubAssign for Complex<T> {
     #[inline]
     fn sub_assign(&mut self, rhs: Self) {
         self.sub_assign(&rhs)
     }
 }
 
@@ -612,14 +648,32 @@
         Complex::new(
             self.re * rhs.re - self.im * rhs.im,
             self.re * rhs.im + self.im * rhs.re,
         )
     }
 }
 
+impl<'a, 'b, T: Real> Mul<&'a Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn mul(self, rhs: &'a Complex<T>) -> Self::Output {
+        *self * *rhs
+    }
+}
+
+impl<'b, T: Real> Mul<Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn mul(self, rhs: Complex<T>) -> Self::Output {
+        *self * rhs
+    }
+}
+
 impl<T: Real> MulAssign for Complex<T> {
     #[inline]
     fn mul_assign(&mut self, rhs: Self) {
         *self = self.mul(rhs);
     }
 }
 
@@ -647,14 +701,32 @@
         let n = rhs.norm_squared();
         let re = self.re * rhs.re + self.im * rhs.im;
         let im = self.im * rhs.re - self.re * rhs.im;
         Complex::new(re / n, im / n)
     }
 }
 
+impl<'a, 'b, T: Real> Div<&'a Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn div(self, rhs: &'a Complex<T>) -> Self::Output {
+        *self / *rhs
+    }
+}
+
+impl<'b, T: Real> Div<Complex<T>> for &'b Complex<T> {
+    type Output = Complex<T>;
+
+    #[inline]
+    fn div(self, rhs: Complex<T>) -> Self::Output {
+        *self / rhs
+    }
+}
+
 impl<T: Real> DivAssign for Complex<T> {
     fn div_assign(&mut self, rhs: Self) {
         *self = self.div(rhs);
     }
 }
 
 impl<T: Real> DivAssign<&Complex<T>> for Complex<T> {
@@ -909,23 +981,24 @@
             + b.tanh()
             - 0.7.asinh()
             + b.acosh() / 0.4.atanh()
             + b.powf(a);
         assert_eq!(r, 17293.219725825093);
     }
 
+
     #[test]
     fn complex() {
         let a = Complex::new(1., 2.);
         let b: Complex<f64> = Complex::new(3., 4.);
 
-        let r = a.sqrt() + b.log() - a.exp() + b.sin() - a.cos() + b.tan() - a.asin() + b.acos()
+        let r = &a.sqrt() + &b.log() - a.exp() + b.sin() - a.cos() + b.tan() - a.asin() + b.acos()
             - a.atan2(&b)
             + b.sinh()
             - a.cosh()
             + b.tanh()
             - a.asinh()
-            + b.acosh() / a.atanh()
+            + &b.acosh() / a.atanh()
             + b.powf(a);
         assert_eq!(r, Complex::new(0.1924131450685842, -39.83285329561913));
     }
 }
```

### Comparing `symbolica-0.5.0/src/domains/integer.rs` & `symbolica-0.6.0/src/domains/integer.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains/rational.rs` & `symbolica-0.6.0/src/domains/rational.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains/rational_polynomial.rs` & `symbolica-0.6.0/src/domains/rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/domains.rs` & `symbolica-0.6.0/src/domains.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/evaluate.rs` & `symbolica-0.6.0/src/evaluate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/expand.rs` & `symbolica-0.6.0/src/expand.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/id.rs` & `symbolica-0.6.0/src/id.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 use ahash::HashSet;
 use dyn_clone::DynClone;
 
 use crate::{
-    atom::{representation::ListSlice, Atom, AtomType, AtomView, Num, SliceType, Symbol},
+    atom::{
+        representation::ListSlice, AsAtomView, Atom, AtomType, AtomView, Num, SliceType, Symbol,
+    },
     state::{State, Workspace},
     transformer::{Transformer, TransformerError},
 };
 
 #[derive(Clone)]
 pub enum Pattern {
     Literal(Atom),
@@ -14,14 +16,44 @@
     Fn(Symbol, Vec<Pattern>),
     Pow(Box<[Pattern; 2]>),
     Mul(Vec<Pattern>),
     Add(Vec<Pattern>),
     Transformer(Box<(Option<Pattern>, Vec<Transformer>)>),
 }
 
+/// A replacement, specified by a pattern and the right-hand side,
+/// with optional conditions and settings.
+pub struct Replacement<'a> {
+    pat: &'a Pattern,
+    rhs: &'a Pattern,
+    conditions: Option<&'a Condition<WildcardAndRestriction>>,
+    settings: Option<&'a MatchSettings>,
+}
+
+impl<'a> Replacement<'a> {
+    pub fn new(pat: &'a Pattern, rhs: &'a Pattern) -> Self {
+        Replacement {
+            pat,
+            rhs,
+            conditions: None,
+            settings: None,
+        }
+    }
+
+    pub fn with_conditions(mut self, conditions: &'a Condition<WildcardAndRestriction>) -> Self {
+        self.conditions = Some(conditions);
+        self
+    }
+
+    pub fn with_settings(mut self, settings: &'a MatchSettings) -> Self {
+        self.settings = Some(settings);
+        self
+    }
+}
+
 impl Atom {
     pub fn into_pattern(&self) -> Pattern {
         Pattern::from_view(self.as_view(), true)
     }
 
     /// Get all symbols in the expression, optionally including function symbols.
     pub fn get_all_symbols(&self, include_function_symbols: bool) -> HashSet<Symbol> {
@@ -31,14 +63,59 @@
         out
     }
 
     /// Returns true iff `self` contains the symbol `s`.
     pub fn contains_symbol(&self, s: Symbol) -> bool {
         self.as_view().contains_symbol(s)
     }
+
+    /// Returns true iff `self` contains `a` literally.
+    pub fn contains<'a, T: AsAtomView<'a>>(&self, s: T) -> bool {
+        self.as_view().contains(s.as_atom_view())
+    }
+
+    /// Replace all occurrences of the pattern.
+    pub fn replace_all(
+        &self,
+        pattern: &Pattern,
+        rhs: &Pattern,
+        conditions: Option<&Condition<WildcardAndRestriction>>,
+        settings: Option<&MatchSettings>,
+    ) -> Atom {
+        self.as_view()
+            .replace_all(pattern, rhs, conditions, settings)
+    }
+
+    /// Replace all occurrences of the pattern.
+    pub fn replace_all_into(
+        &self,
+        pattern: &Pattern,
+        rhs: &Pattern,
+        conditions: Option<&Condition<WildcardAndRestriction>>,
+        settings: Option<&MatchSettings>,
+        out: &mut Atom,
+    ) -> bool {
+        self.as_view()
+            .replace_all_into(pattern, rhs, conditions, settings, out)
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    pub fn replace_all_multiple(&self, replacements: &[Replacement<'_>]) -> Atom {
+        self.as_view().replace_all_multiple(replacements)
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    /// Returns `true` iff a match was found.
+    pub fn replace_all_multiple_into(
+        &self,
+        replacements: &[Replacement<'_>],
+        out: &mut Atom,
+    ) -> bool {
+        self.as_view().replace_all_multiple_into(replacements, out)
+    }
 }
 
 impl<'a> AtomView<'a> {
     pub fn into_pattern(self) -> Pattern {
         Pattern::from_view(self, true)
     }
 
@@ -77,38 +154,323 @@
                 for child in a.iter() {
                     child.get_all_symbols_impl(include_function_symbols, out);
                 }
             }
         }
     }
 
+    /// Returns true iff `self` contains `a` literally.
+    pub fn contains(&self, a: AtomView) -> bool {
+        let mut stack = Vec::with_capacity(20);
+        stack.push(*self);
+
+        while let Some(c) = stack.pop() {
+            if a == c {
+                return true;
+            }
+
+            match c {
+                AtomView::Num(_) | AtomView::Var(_) => {}
+                AtomView::Fun(f) => {
+                    for arg in f.iter() {
+                        stack.push(arg);
+                    }
+                }
+                AtomView::Pow(p) => {
+                    let (base, exp) = p.get_base_exp();
+                    stack.push(base);
+                    stack.push(exp);
+                }
+                AtomView::Mul(m) => {
+                    for child in m.iter() {
+                        stack.push(child);
+                    }
+                }
+                AtomView::Add(a) => {
+                    for child in a.iter() {
+                        stack.push(child);
+                    }
+                }
+            }
+        }
+
+        false
+    }
+
     /// Returns true iff `self` contains the symbol `s`.
     pub fn contains_symbol(&self, s: Symbol) -> bool {
-        match self {
-            AtomView::Num(_) => false,
-            AtomView::Var(v) => v.get_symbol() == s,
-            AtomView::Fun(f) => {
-                if f.get_symbol() == s {
-                    return true;
+        let mut stack = Vec::with_capacity(20);
+        stack.push(*self);
+        while let Some(c) = stack.pop() {
+            match c {
+                AtomView::Num(_) => {}
+                AtomView::Var(v) => {
+                    if v.get_symbol() == s {
+                        return true;
+                    }
+                }
+                AtomView::Fun(f) => {
+                    if f.get_symbol() == s {
+                        return true;
+                    }
+                    for arg in f.iter() {
+                        stack.push(arg);
+                    }
+                }
+                AtomView::Pow(p) => {
+                    let (base, exp) = p.get_base_exp();
+                    stack.push(base);
+                    stack.push(exp);
+                }
+                AtomView::Mul(m) => {
+                    for child in m.iter() {
+                        stack.push(child);
+                    }
+                }
+                AtomView::Add(a) => {
+                    for child in a.iter() {
+                        stack.push(child);
+                    }
+                }
+            }
+        }
+
+        false
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    pub fn replace_all(
+        &self,
+        pattern: &Pattern,
+        rhs: &Pattern,
+        conditions: Option<&Condition<WildcardAndRestriction>>,
+        settings: Option<&MatchSettings>,
+    ) -> Atom {
+        pattern.replace_all(*self, rhs, conditions, settings)
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    pub fn replace_all_into(
+        &self,
+        pattern: &Pattern,
+        rhs: &Pattern,
+        conditions: Option<&Condition<WildcardAndRestriction>>,
+        settings: Option<&MatchSettings>,
+        out: &mut Atom,
+    ) -> bool {
+        pattern.replace_all_into(*self, rhs, conditions, settings, out)
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    pub fn replace_all_multiple(&self, replacements: &[Replacement<'_>]) -> Atom {
+        let mut out = Atom::new();
+        self.replace_all_multiple_into(replacements, &mut out);
+        out
+    }
+
+    /// Replace all occurrences of the patterns, where replacements are tested in the order that they are given.
+    /// Returns `true` iff a match was found.
+    pub fn replace_all_multiple_into(
+        &self,
+        replacements: &[Replacement<'_>],
+        out: &mut Atom,
+    ) -> bool {
+        Workspace::get_local().with(|ws| {
+            let matched = self.replace_all_no_norm(replacements, ws, 0, 0, out);
+
+            if matched {
+                let mut norm = ws.new_atom();
+                out.as_view().normalize(ws, &mut norm);
+                std::mem::swap(out, &mut norm);
+            }
+
+            matched
+        })
+    }
+
+    /// Replace all occurrences of the patterns in the target, without normalizing the output.
+    fn replace_all_no_norm(
+        &self,
+        replacements: &[Replacement<'_>],
+        workspace: &Workspace,
+        tree_level: usize,
+        fn_level: usize,
+        out: &mut Atom,
+    ) -> bool {
+        let mut beyond_max_level = true;
+        for r in replacements {
+            let def_c = Condition::default();
+            let def_s = MatchSettings::default();
+            let conditions = r.conditions.unwrap_or(&def_c);
+            let settings = r.settings.unwrap_or(&def_s);
+
+            if let Some(max_level) = settings.level_range.1 {
+                if settings.level_is_tree_depth && tree_level > max_level
+                    || !settings.level_is_tree_depth && fn_level > max_level
+                {
+                    continue;
                 }
+            }
 
-                for arg in f.iter() {
-                    if arg.contains_symbol(s) {
+            beyond_max_level = false;
+
+            if settings.level_is_tree_depth && tree_level < settings.level_range.0
+                || !settings.level_is_tree_depth && fn_level < settings.level_range.0
+            {
+                continue;
+            }
+
+            if r.pat.could_match(*self) {
+                let mut match_stack = MatchStack::new(conditions, settings);
+
+                let mut it = AtomMatchIterator::new(r.pat, *self);
+                if let Some((_, used_flags)) = it.next(&mut match_stack) {
+                    let mut rhs_subs = workspace.new_atom();
+                    r.rhs
+                        .substitute_wildcards(workspace, &mut rhs_subs, &match_stack)
+                        .unwrap(); // TODO: escalate?
+
+                    if used_flags.iter().all(|x| *x) {
+                        // all used, return rhs
+                        out.set_from_view(&rhs_subs.as_view());
                         return true;
                     }
+
+                    match self {
+                        AtomView::Mul(m) => {
+                            let out = out.to_mul();
+
+                            for (child, used) in m.iter().zip(used_flags) {
+                                if !used {
+                                    out.extend(child);
+                                }
+                            }
+
+                            out.extend(rhs_subs.as_view());
+                        }
+                        AtomView::Add(a) => {
+                            let out = out.to_add();
+
+                            for (child, used) in a.iter().zip(used_flags) {
+                                if !used {
+                                    out.extend(child);
+                                }
+                            }
+
+                            out.extend(rhs_subs.as_view());
+                        }
+                        _ => {
+                            out.set_from_view(&rhs_subs.as_view());
+                        }
+                    }
+
+                    return true;
                 }
-                false
+            }
+        }
+
+        if beyond_max_level {
+            out.set_from_view(self);
+            return false;
+        }
+
+        // no match found at this level, so check the children
+        let submatch = match self {
+            AtomView::Fun(f) => {
+                let out = out.to_fun(f.get_symbol());
+
+                let mut submatch = false;
+
+                let mut child_buf = workspace.new_atom();
+                for child in f.iter() {
+                    submatch |= child.replace_all_no_norm(
+                        replacements,
+                        workspace,
+                        fn_level + 1,
+                        tree_level + 1,
+                        &mut child_buf,
+                    );
+
+                    out.add_arg(child_buf.as_view());
+                }
+
+                out.set_normalized(!submatch && f.is_normalized());
+                submatch
             }
             AtomView::Pow(p) => {
                 let (base, exp) = p.get_base_exp();
-                base.contains_symbol(s) || exp.contains_symbol(s)
+
+                let mut base_out = workspace.new_atom();
+                let mut submatch = base.replace_all_no_norm(
+                    replacements,
+                    workspace,
+                    tree_level + 1,
+                    fn_level,
+                    &mut base_out,
+                );
+
+                let mut exp_out = workspace.new_atom();
+                submatch |= exp.replace_all_no_norm(
+                    replacements,
+                    workspace,
+                    tree_level + 1,
+                    fn_level,
+                    &mut exp_out,
+                );
+
+                let out = out.to_pow(base_out.as_view(), exp_out.as_view());
+                out.set_normalized(!submatch && p.is_normalized());
+                submatch
             }
-            AtomView::Mul(m) => m.iter().any(|x| x.contains_symbol(s)),
-            AtomView::Add(a) => a.iter().any(|x| x.contains_symbol(s)),
-        }
+            AtomView::Mul(m) => {
+                let mul = out.to_mul();
+
+                let mut submatch = false;
+                let mut child_buf = workspace.new_atom();
+                for child in m.iter() {
+                    submatch |= child.replace_all_no_norm(
+                        replacements,
+                        workspace,
+                        tree_level + 1,
+                        fn_level,
+                        &mut child_buf,
+                    );
+
+                    mul.extend(child_buf.as_view());
+                }
+
+                mul.set_has_coefficient(m.has_coefficient());
+                mul.set_normalized(!submatch && m.is_normalized());
+                submatch
+            }
+            AtomView::Add(a) => {
+                let out = out.to_add();
+                let mut submatch = false;
+                let mut child_buf = workspace.new_atom();
+                for child in a.iter() {
+                    submatch |= child.replace_all_no_norm(
+                        replacements,
+                        workspace,
+                        tree_level + 1,
+                        fn_level,
+                        &mut child_buf,
+                    );
+
+                    out.extend(child_buf.as_view());
+                }
+                out.set_normalized(!submatch && a.is_normalized());
+                submatch
+            }
+            _ => {
+                out.set_from_view(self); // no children
+                false
+            }
+        };
+
+        submatch
     }
 }
 
 impl Pattern {
     pub fn parse(input: &str) -> Result<Pattern, String> {
         // TODO: use workspace instead of owned atom
         Ok(Atom::parse(input)?.into_pattern())
@@ -695,224 +1057,33 @@
         target: AtomView<'_>,
         rhs: &Pattern,
         workspace: &Workspace,
         conditions: Option<&Condition<WildcardAndRestriction>>,
         settings: Option<&MatchSettings>,
         out: &mut Atom,
     ) -> bool {
-        let matched = self.replace_all_no_norm(
-            target,
-            rhs,
-            workspace,
-            conditions.unwrap_or(&Condition::default()),
-            settings.unwrap_or(&MatchSettings::default()),
-            0,
-            out,
-        );
+        let mut rep = Replacement::new(self, rhs);
+        if let Some(c) = conditions {
+            rep = rep.with_conditions(c);
+        }
+        if let Some(s) = settings {
+            rep = rep.with_settings(s);
+        }
+
+        let matched = target.replace_all_no_norm(std::slice::from_ref(&rep), workspace, 0, 0, out);
 
         if matched {
             let mut norm = workspace.new_atom();
             out.as_view().normalize(workspace, &mut norm);
             std::mem::swap(out, &mut norm);
         }
 
         matched
     }
 
-    /// Replace all occurrences of the pattern in the target, without normalizing the output.
-    fn replace_all_no_norm(
-        &self,
-        target: AtomView<'_>,
-        rhs: &Pattern,
-        workspace: &Workspace,
-        conditions: &Condition<WildcardAndRestriction>,
-        settings: &MatchSettings,
-        level: usize,
-        out: &mut Atom,
-    ) -> bool {
-        if let Some(max_level) = settings.level_range.1 {
-            if level > max_level {
-                out.set_from_view(&target);
-                return false;
-            }
-        }
-
-        if level >= settings.level_range.0 && self.could_match(target) {
-            let mut match_stack = MatchStack::new(conditions, settings);
-
-            let mut it = AtomMatchIterator::new(self, target);
-            //let mut it = SubSliceIterator::new(self, target, &match_stack, true);
-            if let Some((_, used_flags)) = it.next(&mut match_stack) {
-                let mut rhs_subs = workspace.new_atom();
-                rhs.substitute_wildcards(workspace, &mut rhs_subs, &match_stack)
-                    .unwrap(); // TODO: escalate?
-
-                if used_flags.iter().all(|x| *x) {
-                    // all used, return rhs
-                    out.set_from_view(&rhs_subs.as_view());
-                    return true;
-                }
-
-                match target {
-                    AtomView::Mul(m) => {
-                        let out = out.to_mul();
-
-                        for (child, used) in m.iter().zip(used_flags) {
-                            if !used {
-                                out.extend(child);
-                            }
-                        }
-
-                        out.extend(rhs_subs.as_view());
-                    }
-                    AtomView::Add(a) => {
-                        let out = out.to_add();
-
-                        for (child, used) in a.iter().zip(used_flags) {
-                            if !used {
-                                out.extend(child);
-                            }
-                        }
-
-                        out.extend(rhs_subs.as_view());
-                    }
-                    _ => {
-                        out.set_from_view(&rhs_subs.as_view());
-                    }
-                }
-
-                return true;
-            }
-        }
-
-        // no match found at this level, so check the children
-        let submatch = match target {
-            AtomView::Fun(f) => {
-                let out = out.to_fun(f.get_symbol());
-
-                let mut submatch = false;
-
-                for child in f.iter() {
-                    let mut child_buf = workspace.new_atom();
-
-                    submatch |= self.replace_all_no_norm(
-                        child,
-                        rhs,
-                        workspace,
-                        conditions,
-                        settings,
-                        level + 1,
-                        &mut child_buf,
-                    );
-
-                    out.add_arg(child_buf.as_view());
-                }
-
-                out.set_normalized(!submatch && f.is_normalized());
-                submatch
-            }
-            AtomView::Pow(p) => {
-                let (base, exp) = p.get_base_exp();
-
-                let mut base_out = workspace.new_atom();
-                let mut submatch = self.replace_all_no_norm(
-                    base,
-                    rhs,
-                    workspace,
-                    conditions,
-                    settings,
-                    if settings.level_is_tree_depth {
-                        level + 1
-                    } else {
-                        level
-                    },
-                    &mut base_out,
-                );
-
-                let mut exp_out = workspace.new_atom();
-                submatch |= self.replace_all_no_norm(
-                    exp,
-                    rhs,
-                    workspace,
-                    conditions,
-                    settings,
-                    if settings.level_is_tree_depth {
-                        level + 1
-                    } else {
-                        level
-                    },
-                    &mut exp_out,
-                );
-
-                let out = out.to_pow(base_out.as_view(), exp_out.as_view());
-                out.set_normalized(!submatch && p.is_normalized());
-                submatch
-            }
-            AtomView::Mul(m) => {
-                let mul = out.to_mul();
-
-                let mut submatch = false;
-                for child in m.iter() {
-                    let mut child_buf = workspace.new_atom();
-
-                    submatch |= self.replace_all_no_norm(
-                        child,
-                        rhs,
-                        workspace,
-                        conditions,
-                        settings,
-                        if settings.level_is_tree_depth {
-                            level + 1
-                        } else {
-                            level
-                        },
-                        &mut child_buf,
-                    );
-
-                    mul.extend(child_buf.as_view());
-                }
-
-                mul.set_has_coefficient(m.has_coefficient());
-                mul.set_normalized(!submatch && m.is_normalized());
-                submatch
-            }
-            AtomView::Add(a) => {
-                let out = out.to_add();
-                let mut submatch = false;
-                for child in a.iter() {
-                    let mut child_buf = workspace.new_atom();
-
-                    submatch |= self.replace_all_no_norm(
-                        child,
-                        rhs,
-                        workspace,
-                        conditions,
-                        settings,
-                        if settings.level_is_tree_depth {
-                            level + 1
-                        } else {
-                            level
-                        },
-                        &mut child_buf,
-                    );
-
-                    out.extend(child_buf.as_view());
-                }
-                out.set_normalized(!submatch && a.is_normalized());
-                submatch
-            }
-            _ => {
-                out.set_from_view(&target); // no children
-                false
-            }
-        };
-
-        submatch
-    }
-
     pub fn pattern_match<'a>(
         &'a self,
         target: AtomView<'a>,
         conditions: &'a Condition<WildcardAndRestriction>,
         settings: &'a MatchSettings,
     ) -> PatternAtomTreeIterator<'a, 'a> {
         PatternAtomTreeIterator::new(self, target, conditions, settings)
@@ -1295,15 +1466,15 @@
                 out.to_var(*n);
             }
         }
     }
 }
 
 /// Settings related to pattern matching.
-#[derive(Default, Clone)]
+#[derive(Debug, Default, Clone)]
 pub struct MatchSettings {
     /// Specifies wildcards that try to match as little as possible.
     pub non_greedy_wildcards: Vec<Symbol>,
     /// Specifies the `[min,max]` level at which the pattern is allowed to match.
     /// The first level is 0 and the level is increased when entering a function, or going one level deeper in the expression tree,
     /// depending on `level_is_tree_depth`.
     pub level_range: (usize, Option<usize>),
@@ -2426,22 +2597,38 @@
             None
         }
     }
 }
 
 #[cfg(test)]
 mod test {
-    use crate::atom::Atom;
+    use crate::{atom::Atom, id::Replacement};
 
     use super::Pattern;
 
     #[test]
     fn overlap() {
-        let a = Atom::parse("(x*(y+y^2+1)+y^2 + y)").unwrap();
-        let p = Pattern::parse("y+y^x_").unwrap();
-        let rhs = Pattern::parse("y*(1+y^(x_-1))").unwrap();
+        let a = Atom::parse("(v1*(v2+v2^2+1)+v2^2 + v2)").unwrap();
+        let p = Pattern::parse("v2+v2^v1_").unwrap();
+        let rhs = Pattern::parse("v2*(1+v2^(v1_-1))").unwrap();
 
         let r = p.replace_all(a.as_view(), &rhs, None, None);
-        let res = Atom::parse("x*(y+y^2+1)+y*(y+1)").unwrap();
+        let res = Atom::parse("v1*(v2+v2^2+1)+v2*(v2+1)").unwrap();
+        assert_eq!(r, res);
+    }
+
+    #[test]
+    fn multiple() {
+        let a = Atom::parse("f(v1,v2)").unwrap();
+        let p1 = Pattern::parse("v1").unwrap();
+        let rhs1 = Pattern::parse("v2").unwrap();
+
+        let p2 = Pattern::parse("v2").unwrap();
+        let rhs2 = Pattern::parse("v1").unwrap();
+
+        let r =
+            a.replace_all_multiple(&[Replacement::new(&p1, &rhs1), Replacement::new(&p2, &rhs2)]);
+
+        let res = Atom::parse("f(v2,v1)").unwrap();
         assert_eq!(r, res);
     }
 }
```

### Comparing `symbolica-0.5.0/src/lib.rs` & `symbolica-0.6.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/normalize.rs` & `symbolica-0.6.0/src/normalize.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/numerical_integration.rs` & `symbolica-0.6.0/src/numerical_integration.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/parser.rs` & `symbolica-0.6.0/src/parser.rs`

 * *Files 8% similar despite different names*

```diff
@@ -148,18 +148,19 @@
 
 #[derive(Debug, Clone, PartialEq, Eq, Hash)]
 pub enum Token {
     Number(SmartString<LazyCompact>),
     ID(SmartString<LazyCompact>),
     RationalPolynomial(SmartString<LazyCompact>),
     Op(bool, bool, Operator, Vec<Token>),
-    Fn(bool, Vec<Token>),
+    Fn(bool, bool, Vec<Token>),
     Start,
     OpenParenthesis,
     CloseParenthesis,
+    CloseBracket,
     EOF,
 }
 
 impl std::fmt::Display for Token {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         match self {
             Token::Number(n) => f.write_str(n),
@@ -190,15 +191,15 @@
                     }
                     first = false;
 
                     mm.fmt(f)?;
                 }
                 f.write_char(')')
             }
-            Token::Fn(_, args) => {
+            Token::Fn(_, _, args) => {
                 let mut first = true;
 
                 match &args[0] {
                     Token::ID(s) => f.write_str(s)?,
                     _ => unreachable!(),
                 };
 
@@ -212,41 +213,45 @@
                     aa.fmt(f)?;
                 }
                 f.write_char(')')
             }
             Token::Start => f.write_str("START"),
             Token::OpenParenthesis => f.write_char('('),
             Token::CloseParenthesis => f.write_char(')'),
+            Token::CloseBracket => f.write_char(']'),
             Token::EOF => f.write_str("EOF"),
         }
     }
 }
 
 impl Token {
     /// Return if the token does not require any further arguments.
     fn is_normal(&self) -> bool {
         match self {
             Token::Number(_) => true,
             Token::ID(_) => true,
             Token::RationalPolynomial(_) => true,
             Token::Op(more_left, more_right, _, _) => !more_left && !more_right,
-            Token::Fn(more_right, _) => !more_right,
+            Token::Fn(more_right, _, _) => !more_right,
             _ => false,
         }
     }
 
     /// Get the precedence of the token.
     #[inline]
     fn get_precedence(&self) -> u8 {
         match self {
             Token::Number(_) => 11,
             Token::ID(_) => 11,
             Token::RationalPolynomial(_) => 11,
             Token::Op(_, _, o, _) => o.get_precedence(),
-            Token::Fn(_, _) | Token::OpenParenthesis | Token::CloseParenthesis => 5,
+            Token::Fn(_, _, _)
+            | Token::OpenParenthesis
+            | Token::CloseParenthesis
+            | Token::CloseBracket => 5,
             Token::Start | Token::EOF => 4,
         }
     }
 
     /// Add `other` to the left side of `self`, where `self` is a binary operation.
     #[inline]
     fn add_left(&mut self, other: Token) -> Result<(), String> {
@@ -436,27 +441,31 @@
                     args[0].to_atom_with_output_no_norm(state, workspace, &mut base)?;
 
                     let num = workspace.new_num(-1);
 
                     out.to_pow(base.as_view(), num.as_view());
                 }
             },
-            Token::Fn(_, args) => {
+            Token::Fn(_, _, args) => {
                 let name = match &args[0] {
                     Token::ID(s) => s,
                     _ => unreachable!(),
                 };
 
                 let fun = out.to_fun(state.get_symbol_impl(name));
                 let mut atom = workspace.new_atom();
                 for a in args.iter().skip(1) {
                     a.to_atom_with_output_no_norm(state, workspace, &mut atom)?;
                     fun.add_arg(atom.as_view());
                 }
             }
+            Token::RationalPolynomial(_) => Err(format!(
+                "Optimized rational polynomial input cannot be parsed yet as atom: {}",
+                self
+            ))?,
             x => return Err(format!("Unexpected token {}", x)),
         }
 
         Ok(())
     }
 
     /// Parse the token into the atom `out` with pre-defined variables
@@ -572,15 +581,15 @@
                     let num = workspace.new_num(-1);
 
                     let mut pow_h = workspace.new_atom();
                     pow_h.to_pow(base.as_view(), num.as_view());
                     pow_h.as_view().normalize(workspace, out);
                 }
             },
-            Token::Fn(_, args) => {
+            Token::Fn(_, _, args) => {
                 let name = match &args[0] {
                     Token::ID(s) => s,
                     _ => unreachable!(),
                 };
 
                 let index = var_name_map
                     .iter()
@@ -660,19 +669,26 @@
                 ParseState::RationalPolynomial => {
                     let start = char_iter.clone();
                     let mut pos = 0;
 
                     let mut s = SmartString::new();
                     s.push(c);
 
-                    while c != ']' {
+                    while c != ']' && c != '\0' {
                         pos += 1;
                         c = char_iter.next().unwrap_or('\0');
                     }
 
+                    if c == '\0' {
+                        Err(format!(
+                            "Missing ] of bracket started at line {} and column {}",
+                            line_counter, column_counter
+                        ))?;
+                    }
+
                     s.push_str(&start.as_str()[..pos - 1]);
                     stack.push(Token::RationalPolynomial(s));
 
                     state = ParseState::Any;
 
                     column_counter += pos + 1;
                     c = char_iter.next().unwrap_or('\0');
@@ -695,45 +711,45 @@
 
                 match c {
                     '+' => {
                         if matches!(
                             unsafe { stack.last().unwrap_unchecked() },
                             Token::Start
                                 | Token::OpenParenthesis
-                                | Token::Fn(true, _)
+                                | Token::Fn(true, _, _)
                                 | Token::Op(_, true, _, _)
                         ) {
                             // unary + operator, can be ignored as plus is the default
                         } else {
                             stack.push(Token::Op(true, true, Operator::Add, vec![]))
                         }
                     }
                     '^' => stack.push(Token::Op(true, true, Operator::Pow, vec![])),
                     '*' => stack.push(Token::Op(true, true, Operator::Mul, vec![])),
                     '-' => {
                         if matches!(
                             unsafe { stack.last().unwrap_unchecked() },
                             Token::Start
                                 | Token::OpenParenthesis
-                                | Token::Fn(true, _)
+                                | Token::Fn(true, _, _)
                                 | Token::Op(_, true, _, _)
                         ) {
                             // unary minus only requires an argument to the right
                             stack.push(Token::Op(false, true, Operator::Neg, vec![]));
                         } else {
                             stack.push(Token::Op(true, true, Operator::Add, vec![]));
                             extra_ops.push('-'); // push a unary minus
                         }
                     }
                     '(' => {
                         // check if the opening bracket belongs to a function
                         if let Some(Token::ID(_)) = stack.last() {
                             let name = unsafe { stack.pop().unwrap_unchecked() };
                             if let Token::ID(_) = name {
-                                stack.push(Token::Fn(true, vec![name])); // serves as open paren
+                                stack.push(Token::Fn(true, false, vec![name])); // serves as open paren
                             }
                         } else if unsafe { stack.last().unwrap_unchecked() }.is_normal() {
                             // insert multiplication: x(...) -> x*(...)
                             stack.push(Token::Op(true, true, Operator::Mul, vec![]));
                             extra_ops.push(c);
                         } else {
                             stack.push(Token::OpenParenthesis)
@@ -741,35 +757,43 @@
                     }
                     ')' => stack.push(Token::CloseParenthesis),
                     '/' => {
                         if matches!(
                             stack.last().unwrap(),
                             Token::Start
                                 | Token::OpenParenthesis
-                                | Token::Fn(true, _)
+                                | Token::Fn(true, _, _)
                                 | Token::Op(_, true, _, _)
                         ) {
                             // unary inv only requires an argument to the right
                             stack.push(Token::Op(false, true, Operator::Inv, vec![]));
                         } else {
                             stack.push(Token::Op(true, true, Operator::Mul, vec![]));
                             extra_ops.push('/'); // push a (unary) inverse
                         }
                     }
                     ',' => stack.push(Token::Op(true, true, Operator::Argument, vec![])),
                     '\0' => stack.push(Token::EOF),
                     '[' => {
                         if unsafe { stack.last().unwrap_unchecked() }.is_normal() {
-                            // insert multiplication: x[3,4] -> x*[3,4]
-                            stack.push(Token::Op(true, true, Operator::Mul, vec![]));
-                            extra_ops.push(c);
+                            if let Token::ID(_) = unsafe { stack.last().unwrap_unchecked() } {
+                                let name = unsafe { stack.pop().unwrap_unchecked() };
+                                if let Token::ID(_) = name {
+                                    stack.push(Token::Fn(true, true, vec![name]));
+                                }
+                            } else {
+                                // insert multiplication: f(x)[3,4] -> f(x)*[3,4]
+                                stack.push(Token::Op(true, true, Operator::Mul, vec![]));
+                                extra_ops.push(c);
+                            }
                         } else {
                             state = ParseState::RationalPolynomial;
                         }
                     }
+                    ']' => stack.push(Token::CloseBracket),
                     _ => {
                         if unsafe { stack.last().unwrap_unchecked() }.is_normal() {
                             // insert multiplication: x y -> x*y
                             stack.push(Token::Op(true, true, Operator::Mul, vec![]));
                             extra_ops.push(c);
                         } else if c.is_ascii_digit() {
                             state = ParseState::Number;
@@ -797,24 +821,48 @@
                         Token::Op(true, _, op, _) => {
                             Err(format!(
                             "Error at line {} and position {}: operator '{}' is missing left-hand side",
                             line_counter, column_counter, op,
                         ))?;
                         }
 
-                        Token::CloseParenthesis => {
+                        x @ Token::CloseParenthesis | x @ Token::CloseBracket => {
+                            let c = x.clone();
                             let pos = stack.len() - 2;
                             // check if we have an empty function
-                            if let Token::Fn(f, _) = unsafe { stack.get_unchecked_mut(pos) } {
-                                *f = false;
-                                stack.pop();
+                            if let Token::Fn(f, bracket, _) =
+                                unsafe { stack.get_unchecked_mut(pos) }
+                            {
+                                if c == Token::CloseParenthesis && !*bracket
+                                    || c == Token::CloseBracket && *bracket
+                                {
+                                    *f = false;
+                                    stack.pop();
+                                } else {
+                                    Err(format!(
+                                        "Error at line {} and position {}: unexpected '{}'",
+                                        line_counter,
+                                        column_counter,
+                                        if c == Token::CloseParenthesis {
+                                            ")"
+                                        } else {
+                                            "]"
+                                        }
+                                    ))?;
+                                }
                             } else {
                                 Err(format!(
-                                    "Error at line {} and position {}: unexpected ')'",
-                                    line_counter, column_counter,
+                                    "Error at line {} and position {}: unexpected '{}'",
+                                    line_counter,
+                                    column_counter,
+                                    if c == Token::CloseParenthesis {
+                                        ")"
+                                    } else {
+                                        "]"
+                                    }
                                 ))?;
                             }
                         }
                         _ => {}
                     }
 
                     // no simplification, get new token
@@ -847,18 +895,37 @@
                     }
                     std::cmp::Ordering::Equal => {
                         // same degree, special merges!
                         match (&mut first, middle, last) {
                             (Token::Start, mid, Token::EOF) => {
                                 *first = mid;
                             }
-                            (Token::Fn(mr, args), mid, Token::CloseParenthesis) => {
+                            (
+                                Token::Fn(mr, bracket, args),
+                                mid,
+                                x @ Token::CloseParenthesis | x @ Token::CloseBracket,
+                            ) => {
                                 debug_assert!(*mr);
                                 *mr = false;
 
+                                if x == Token::CloseParenthesis && *bracket
+                                    || x == Token::CloseBracket && !*bracket
+                                {
+                                    Err(format!(
+                                        "Error at line {} and position {}: unexpected '{}'",
+                                        line_counter,
+                                        column_counter,
+                                        if x == Token::CloseParenthesis {
+                                            ")"
+                                        } else {
+                                            "]"
+                                        }
+                                    ))?;
+                                }
+
                                 if let Token::Op(_, _, Operator::Argument, arg2) = mid {
                                     args.extend(arg2);
                                 } else {
                                     args.push(mid);
                                 }
                             }
                             (Token::OpenParenthesis, mid, Token::CloseParenthesis) => {
@@ -930,15 +997,15 @@
                     "Unexpected end of input: missing right-hand side for operator '{}'",
                     op
                 )),
                 Some(Token::OpenParenthesis) => {
                     Err("Unexpected end of input: open parenthesis is not closed".to_string())
                 }
 
-                Some(Token::Fn(true, args)) => Err(format!(
+                Some(Token::Fn(true, _, args)) => Err(format!(
                     "Unexpected end of input: Missing closing parenthesis for function '{}'",
                     args[0]
                 )),
                 Some(Token::Start) => Err("Expression is empty".to_string()),
                 _ => Err(format!("Unknown parsing error: {:?}", stack)),
             }
         }
@@ -1186,14 +1253,21 @@
         )
         .unwrap();
         let res = Atom::parse("8923321837281*x^2*y^-1+5").unwrap();
         assert_eq!(input, res);
     }
 
     #[test]
+    fn square_bracket_function() {
+        let input = Atom::parse("v1  [v1, v2]+5 + v1[]").unwrap();
+        let res = Atom::parse("v1(v1,v2)+5+v1()").unwrap();
+        assert_eq!(input, res);
+    }
+
+    #[test]
     fn poly() {
         let var_names = ["v1".into(), "v2".into()];
         let var_map = Arc::new(vec![
             State::get_symbol("v1").into(),
             State::get_symbol("v2").into(),
         ]);
         let (rest, input) =
```

### Comparing `symbolica-0.5.0/src/poly/evaluate.rs` & `symbolica-0.6.0/src/poly/evaluate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1129,15 +1129,32 @@
                 Instruction::Add(a) | Instruction::Mul(a) => {
                     for v in &mut *a {
                         if *v >= insert_index {
                             *v += 1;
                         }
                     }
 
-                    if same_op {
+                    if !same_op {
+                        continue;
+                    }
+
+                    if idx1 == idx2 {
+                        let count = a.iter().filter(|x| *x == &idx1).count();
+                        let pairs = count / 2;
+                        if pairs > 0 {
+                            a.retain(|x| x != &idx1);
+
+                            if count % 2 == 1 {
+                                a.push(idx1);
+                            }
+
+                            a.extend(std::iter::repeat(insert_index).take(pairs));
+                            a.sort();
+                        }
+                    } else {
                         let mut idx1_count = 0;
                         let mut idx2_count = 0;
                         for v in &*a {
                             if *v == idx1 {
                                 idx1_count += 1;
                             }
                             if *v == idx2 {
@@ -1291,15 +1308,15 @@
 enum InstructionRange {
     Add(usize, usize, usize), // reg, index, len
     Mul(usize, usize, usize),
     Out(usize),
 }
 /// A fast polynomial evaluator that evaluates polynomials written
 /// in the form:
-/// ```
+/// ```text
 /// Z0 = x
 /// Z1 = y
 /// Z2 = 2.
 /// Z3 = 5.
 /// Z4 = Z0*Z2
 /// Z5 = Z3+Z1+Z0
 /// Z4 = Z4*Z3
@@ -1728,19 +1745,21 @@
     /// ```text
     /// x_0 = (p1, p2)
     /// x_1 = x_0[0] * x_0[1] + 2
     /// x_2 = x_1 + 2*x_0
     /// ```
     /// can be represented by:
     /// ```
+    /// # use symbolica::atom::Atom;
+    /// # use symbolica::state::State;
     /// vec![
-    ///       vec![(x0, vec![Atom.parse("p1"), Atom.parse("p2")])],
-    ///       vec![(x1, vec![Atom.parse("x0(0) * x0(1) + 2")])],
-    ///       vec![(x2, vec![Atom.parse("x1(0) * 2 * x0(1)")])]
-    /// ]
+    ///       vec![(State::get_symbol("x0"), vec![Atom::parse("p1"), Atom::parse("p2")])],
+    ///       vec![(State::get_symbol("x1"), vec![Atom::parse("x0(0) * x0(1) + 2")])],
+    ///       vec![(State::get_symbol("x2"), vec![Atom::parse("x1(0) * 2 * x0(1)")])]
+    /// ];
     /// ```
     ///
     /// Each expression will be converted to a polynomial and optimized by writing it in a near-optimal Horner scheme and by performing
     /// common subexpression elimination. The number of optimization iterations can be set using `n_iter`.
     ///
     pub fn new(levels: Vec<Vec<(Symbol, Vec<Atom>)>>, n_iter: usize) -> ExpressionEvaluator {
         let mut overall_ops = vec![]; // the main function that calls all levels
```

### Comparing `symbolica-0.5.0/src/poly/factor.rs` & `symbolica-0.6.0/src/poly/factor.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly/gcd.rs` & `symbolica-0.6.0/src/poly/gcd.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly/groebner.rs` & `symbolica-0.6.0/src/poly/groebner.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly/polynomial.rs` & `symbolica-0.6.0/src/poly/polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly/resultant.rs` & `symbolica-0.6.0/src/poly/resultant.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly/series.rs` & `symbolica-0.6.0/src/poly/series.rs`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 use std::{
     cmp::Ordering,
     ops::{Add, Div, Mul, Neg, Sub},
     sync::Arc,
 };
 
 use crate::{
-    atom::{Atom, AtomView, FunctionBuilder, Symbol},
+    atom::{Atom, AtomView, FunctionBuilder},
     coefficient::CoefficientView,
     domains::{
         atom::AtomField, integer::Integer, rational::Rational, EuclideanDomain, Ring, RingPrinter,
     },
     printer::PrintOptions,
     state::State,
 };
@@ -20,14 +20,15 @@
 /// A Puiseux series. The truncation order is
 /// relative to the lowest degree: i.e., a series in `x` with depth `d` is viewed as
 /// `a*x^n*(1+bx+.. + O(x^(d+1)))`.
 #[derive(Clone)]
 pub struct Series<F: Ring> {
     coefficients: Vec<F::Element>,
     variable: Arc<Variable>,
+    expansion_point: F::Element,
     field: F,
     shift: isize, // a shift in units of the ramification that indicates the starting power of the series
     order: usize, // the order of truncation in units of the ramification
     ramification: usize, // the factor that makes the exponents integer
 }
 
 impl<F: Ring + std::fmt::Debug> std::fmt::Debug for Series<F> {
@@ -90,15 +91,15 @@
             } else if self.field.is_one(c) {
                 if e.is_integer() {
                     write!(f, "{}^{}", v, e)?;
                 } else {
                     write!(f, "{}^({})", v, e)?;
                 }
             } else if e.is_integer() {
-                    write!(f, "{}*{}^{}", p, v, e)?;
+                write!(f, "{}*{}^{}", p, v, e)?;
             } else {
                 write!(f, "{}*{}^({})", p, v, e)?;
             }
         }
 
         let o = self.absolute_order();
         if o.is_integer() {
@@ -110,21 +111,28 @@
 }
 
 impl<F: Ring> Series<F> {
     /// Constructs a zero series. Instead of using this constructor,
     /// prefer to create new series from existing ones, so that the
     /// variable map and field are inherited.
     #[inline]
-    pub fn new(field: &F, cap: Option<usize>, variable: Arc<Variable>, order: Rational) -> Self {
+    pub fn new(
+        field: &F,
+        cap: Option<usize>,
+        variable: Arc<Variable>,
+        expansion_point: F::Element,
+        order: Rational,
+    ) -> Self {
         if order.is_negative() {
             panic!("The order of the series must be positive.");
         }
 
         Self {
             coefficients: Vec::with_capacity(cap.unwrap_or(0)),
+            expansion_point,
             field: field.clone(),
             variable,
             shift: 0,
             order: order.numerator().to_i64().unwrap() as usize
                 * order.denominator().to_i64().unwrap() as usize,
             ramification: order.denominator().to_i64().unwrap() as usize,
         }
@@ -133,28 +141,30 @@
     /// Constructs a zero series, inheriting the field and variable from `self`.
     #[inline]
     pub fn zero(&self) -> Self {
         Self {
             coefficients: vec![],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: 0,
             order: self.order,
             ramification: 1,
         }
     }
 
     /// Constructs a zero series with the given number of variables and capacity,
     /// inheriting the field and variable from `self`.
     #[inline]
     pub fn zero_with_capacity(&self, cap: usize) -> Self {
         Self {
             coefficients: Vec::with_capacity(cap),
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: 0,
             order: self.order,
             ramification: 1,
         }
     }
 
     /// Constructs a constant series,
@@ -165,27 +175,29 @@
             return self.zero();
         }
 
         Self {
             coefficients: vec![coeff],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: 0,
             order: self.order,
             ramification: 1,
         }
     }
 
     /// Constructs a series that is one, inheriting the field and variable map from `self`.
     #[inline]
     pub fn one(&self) -> Self {
         Self {
             coefficients: vec![self.field.one()],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: 0,
             order: self.order,
             ramification: 1,
         }
     }
 
     /// Constructs a series with a single term.
@@ -203,14 +215,15 @@
             .to_i64()
             .unwrap() as usize;
 
         Self {
             coefficients: vec![coeff],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: n * d as isize,
             order: self.order * ram / d,
             ramification: ram,
         }
     }
 
     /// Constructs a series that is `x+a`, where `a` is a constant.
@@ -220,14 +233,15 @@
             return self.monomial(self.field.one(), (1, 1).into());
         }
 
         Self {
             coefficients: vec![coeff, self.field.one()],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: 0,
             order: self.order,
             ramification: 1,
         }
     }
 
     // Map an index in the coefficient array to its power.
@@ -260,14 +274,20 @@
         (
             self.order as i64 + self.shift as i64,
             self.ramification as i64,
         )
             .into()
     }
 
+    /// Get the expansion point.
+    #[inline]
+    pub fn get_expansion_point(&self) -> F::Element {
+        self.expansion_point.clone()
+    }
+
     fn change_ramification(&mut self, ram: usize) {
         let ram = Integer::from(self.ramification as i64)
             .lcm(&Integer::from(ram as i64))
             .to_i64()
             .unwrap() as usize;
 
         if ram == self.ramification {
@@ -277,14 +297,15 @@
         let mut s = Self {
             coefficients: vec![
                 self.field.zero();
                 self.coefficients.len() * ram / self.ramification
             ],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: self.shift * (ram / self.ramification) as isize,
             order: self.order * (ram / self.ramification),
             ramification: ram,
         };
 
         for (i, c) in std::mem::take(&mut self.coefficients)
             .into_iter()
@@ -353,16 +374,21 @@
     }
 
     #[inline]
     pub fn get_trailing_exponent(&self) -> Rational {
         self.get_exponent(0)
     }
 
+    #[inline]
+    pub fn get_ramification(&self) -> usize {
+        self.ramification
+    }
+
     /// Get a copy of the variable/
-    pub fn get_vars(&self) -> Arc<Variable> {
+    pub fn get_variable(&self) -> Arc<Variable> {
         self.variable.clone()
     }
 
     /// Get a reference to the variables
     pub fn get_vars_ref(&self) -> &Variable {
         self.variable.as_ref()
     }
@@ -422,33 +448,14 @@
         }
 
         self.truncate(); // zeros may have occurred
 
         self
     }
 
-    /// Map a coefficient using the function `f`.
-    pub fn map_coeff<U: Ring, T: Fn(&F::Element) -> U::Element>(
-        &self,
-        f: T,
-        field: U,
-    ) -> Series<U> {
-        let mut r = Series {
-            coefficients: vec![],
-            field,
-            variable: self.variable.clone(),
-            shift: self.shift,
-            order: self.order,
-            ramification: self.ramification,
-        };
-        r.coefficients = self.coefficients.iter().map(f).collect::<Vec<_>>();
-        r.truncate();
-        r
-    }
-
     /// Truncate the leading and trailing non-zeroes.
     fn truncate(&mut self) {
         if self.coefficients.is_empty() {
             return;
         }
 
         let d = self
@@ -573,14 +580,15 @@
             let shift = (self.shift * r_d_s as isize).min(other.shift * r_d_o as isize);
             let order_s = (self.order * r_d_s) as isize + self.shift * r_d_s as isize;
             let order_o = (other.order * r_d_o) as isize + other.shift * r_d_o as isize;
 
             let mut s = Self {
                 coefficients: vec![],
                 variable: self.variable.clone(),
+                expansion_point: self.expansion_point.clone(),
                 field: self.field.clone(),
                 shift,
                 order: (order_s.min(order_o) - shift) as usize,
                 ramification: r,
             };
 
             s.coefficients = vec![self.field.zero(); s.order]; // TODO: tighten bound
@@ -650,14 +658,15 @@
         let r = self.joint_ramification(&rhs);
         let r_d_s = r / self.ramification;
         let r_d_o = r / rhs.ramification;
         let mut res = Series {
             coefficients: vec![],
             field: self.field.clone(),
             variable: self.variable.clone(),
+            expansion_point: self.expansion_point.clone(),
             shift: self.shift * r_d_s as isize + rhs.shift * r_d_o as isize,
             order: (self.order * r_d_s).min(rhs.order * r_d_o),
             ramification: r,
         };
 
         res.coefficients = vec![self.field.zero(); res.order as usize];
 
@@ -743,39 +752,34 @@
     pub fn make_primitive(self) -> Self {
         let c = self.content();
         self.div_coeff(&c)
     }
 }
 
 impl Series<AtomField> {
-    /// Extract x^a from an expression that comes from simplifying an exponential with logs
-    /// i.e.: exp(c + 3 Log[x^5]]) = exp(c)*x^15.
-    fn extract_exp_log(&self, e: AtomView, s: Symbol) -> Result<Self, &'static str> {
-        if !e.contains_symbol(s) {
+    /// Extract powers of `x` from an expression that comes from simplifying an exponential with logs
+    /// i.e.: `exp(c + 3 log(x^5)) = exp(c)*x^15`.
+    fn extract_exp_log(&self, e: AtomView, s: AtomView) -> Result<Self, &'static str> {
+        if !e.contains(s) {
             return Ok(self.constant(e.to_owned()));
         }
 
         match e {
             AtomView::Pow(p) => {
                 let (b, exp) = p.get_base_exp();
 
-                if let AtomView::Var(v) = b {
-                    if v.get_symbol() == s {
-                        if let AtomView::Num(n) = exp {
-                            if let CoefficientView::Natural(n, d) = n.get_coeff_view() {
-                                Ok(self.monomial(self.field.one(), (n, d).into()))
-                            } else {
-                                unimplemented!("Cannot series expand with large exponents yet")
-                            }
+                if b == s {
+                    if let AtomView::Num(n) = exp {
+                        if let CoefficientView::Natural(n, d) = n.get_coeff_view() {
+                            Ok(self.monomial(self.field.one(), (n, d).into()))
                         } else {
-                            Err("Power of variable must be rational")
+                            unimplemented!("Cannot series expand with large exponents yet")
                         }
                     } else {
-                        // s appears in the power
-                        Err("Unexpected term in exp-log simplification")
+                        Err("Power of variable must be rational")
                     }
                 } else {
                     Err("Unexpected term in exp-log simplification")
                 }
             }
             AtomView::Var(_) => Ok(self.monomial(self.field.one(), (1, 1).into())),
             AtomView::Mul(m) => {
@@ -805,19 +809,16 @@
             Atom::new()
         };
 
         // construct the constant term, log(x) in the argument will be turned into x
         let e = FunctionBuilder::new(State::EXP).add_arg(&c).finish();
 
         // split the true constant part and the x-dependent part
-        let shift_series = if let Variable::Symbol(s) = self.variable.as_ref() {
-            self.extract_exp_log(e.as_view(), *s)?
-        } else {
-            unreachable!("Expansion variable is not a variable");
-        };
+        let var = self.variable.to_atom() - &self.expansion_point;
+        let shift_series = self.extract_exp_log(e.as_view(), var.as_view())?;
 
         let p = self.clone().remove_constant();
 
         let mut r = self.one();
         let mut sp = p.clone();
         for i in 1..=self.order {
             let s = sp
@@ -834,15 +835,16 @@
 
     pub fn log(&self) -> Result<Self, &'static str> {
         if self.is_zero() {
             return Err("Log yields minus infinity");
         }
 
         // construct the log argument, which may contain x
-        let c = self.variable.to_atom().npow(self.get_exponent(0)) * &self.coefficients[0];
+        let c = (self.variable.to_atom() - &self.expansion_point).npow(self.get_exponent(0))
+            * &self.coefficients[0];
         // normalize the series to 1 + ..
         let p = self
             .clone()
             .div_coeff(&self.coefficients[0])
             .mul_exp_units(-self.shift)
             - self.one();
 
@@ -874,20 +876,18 @@
 
         let c = if self.shift == 0 {
             self.coefficients[0].clone()
         } else {
             Atom::new()
         };
 
-        if let Variable::Symbol(s) = self.variable.as_ref() {
-            if c.contains_symbol(*s) {
-                return Err(
-                    "Cannot compute the sin of a series with a constant term that depends on x",
-                );
-            }
+        if c.contains(&self.variable.to_atom()) {
+            return Err(
+                "Cannot compute the sine of a series with a constant term that depends on x",
+            );
         }
 
         let p = self.clone().remove_constant();
 
         let mut e = self.constant(FunctionBuilder::new(State::SIN).add_arg(&c).finish());
         let mut sp = p.clone();
         for i in 1..=self.order {
@@ -925,20 +925,18 @@
 
         let c = if self.shift == 0 {
             self.coefficients[0].clone()
         } else {
             Atom::new()
         };
 
-        if let Variable::Symbol(s) = self.variable.as_ref() {
-            if c.contains_symbol(*s) {
-                return Err(
-                    "Cannot compute the cosine of a series with a constant term that depends on x",
-                );
-            }
+        if c.contains(&self.variable.to_atom()) {
+            return Err(
+                "Cannot compute the cosine of a series with a constant term that depends on x",
+            );
         }
 
         let p = self.clone().remove_constant();
 
         let mut e = self.constant(FunctionBuilder::new(State::COS).add_arg(&c).finish());
         let mut sp = p.clone();
         for i in 1..=self.order {
@@ -1031,15 +1029,15 @@
     pub fn to_atom_into(&self, out: &mut Atom) {
         out.to_num(0.into());
 
         if self.is_zero() {
             return;
         }
 
-        let v = self.variable.to_atom();
+        let v = self.variable.to_atom() - &self.expansion_point;
         for (e, c) in self.coefficients.iter().enumerate() {
             let p = self.get_exponent(e);
             if !c.is_zero() {
                 *out = &*out + &(v.npow(p) * c);
             }
         }
     }
```

### Comparing `symbolica-0.5.0/src/poly/univariate.rs` & `symbolica-0.6.0/src/poly/univariate.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/poly.rs` & `symbolica-0.6.0/src/poly.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/printer.rs` & `symbolica-0.6.0/src/printer.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/solve.rs` & `symbolica-0.6.0/src/solve.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/state.rs` & `symbolica-0.6.0/src/state.rs`

 * *Files 0% similar despite different names*

```diff
@@ -156,17 +156,18 @@
     }
 
     /// Remove all user-defined symbols from the state. This will invalidate all
     /// currently existing atoms, and hence this function is unsafe.
     ///
     /// Example:
     /// ```
-    /// State::get_symbol_with_attributes("f", vec![FunctionAttribute::Symmetric]).unwrap();
+    /// # use symbolica::state::{State, FunctionAttribute};
+    /// State::get_symbol_with_attributes("f", &[FunctionAttribute::Symmetric]).unwrap();
     /// unsafe { State::reset(); }
-    /// State::get_symbol_with_attributes("f", vec![FunctionAttribute::Antisymmetric]).unwrap();
+    /// State::get_symbol_with_attributes("f", &[FunctionAttribute::Antisymmetric]).unwrap();
     /// ```
     pub unsafe fn reset() {
         let mut state = STATE.write().unwrap();
 
         state.str_to_id.clear();
         SYMBOL_OFFSET.store(ID_TO_STR.len(), Ordering::Relaxed);
 
@@ -661,15 +662,15 @@
         let mut owned = Self::new();
         owned.to_num(num.into());
         owned
     }
 
     /// Yield the atom, which will now no longer be recycled upon dropping.
     pub fn into_inner(mut self) -> Atom {
-        std::mem::replace(&mut self.0, Atom::Empty)
+        std::mem::replace(&mut self.0, Atom::Zero)
     }
 }
 
 impl Deref for RecycledAtom {
     type Target = Atom;
 
     fn deref(&self) -> &Atom {
@@ -688,24 +689,24 @@
         self.deref()
     }
 }
 
 impl Drop for RecycledAtom {
     #[inline]
     fn drop(&mut self) {
-        if let Atom::Empty = self.0 {
+        if let Atom::Zero = self.0 {
             return;
         }
 
         let _ = WORKSPACE.try_with(
             #[inline(always)]
             |ws| {
                 if let Ok(mut a) = ws.atom_buffer.try_borrow_mut() {
                     if a.len() < Workspace::ATOM_BUFFER_MAX {
-                        a.push(std::mem::replace(&mut self.0, Atom::Empty));
+                        a.push(std::mem::replace(&mut self.0, Atom::Zero));
                     }
                 }
             },
         );
     }
 }
```

### Comparing `symbolica-0.5.0/src/streaming.rs` & `symbolica-0.6.0/src/streaming.rs`

 * *Files 4% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     }
 }
 
 /// A term streamer that has terms partly in memory and partly on another storage device.
 pub struct TermStreamer<W: WriteableNamedStream> {
     mem_buf: Vec<Atom>,
     mem_size: usize,
+    num_terms: usize,
     total_size: usize,
     file_buf: Vec<W>,
     config: TermStreamerConfig,
     filename: String,
     thread_pool: Arc<rayon::ThreadPool>,
     generation: usize,
 }
@@ -174,14 +175,15 @@
                 break name;
             }
         };
 
         Self {
             mem_buf: vec![],
             mem_size: 0,
+            num_terms: 0,
             total_size: 0,
             file_buf: vec![],
             filename,
             thread_pool: Arc::new(
                 rayon::ThreadPoolBuilder::new()
                     .num_threads(config.n_cores)
                     .build()
@@ -192,23 +194,34 @@
         }
     }
 
     fn next_generation(&self) -> Self {
         Self {
             mem_buf: vec![],
             mem_size: 0,
+            num_terms: 0,
             total_size: 0,
             file_buf: vec![],
             filename: self.filename.clone(),
             config: self.config.clone(),
             thread_pool: self.thread_pool.clone(),
             generation: self.generation + 1,
         }
     }
 
+    /// Returns true iff the stream fits in memory.
+    pub fn fits_in_memory(&self) -> bool {
+        self.file_buf.is_empty()
+    }
+
+    /// Get the number of terms in the stream.
+    pub fn get_num_terms(&self) -> usize {
+        self.num_terms
+    }
+
     /// Add terms to the buffer.
     pub fn push(&mut self, a: Atom) {
         if let AtomView::Add(aa) = a.as_view() {
             for arg in aa.iter() {
                 self.push_sorted_impl(arg.to_owned());
             }
         } else {
@@ -216,14 +229,15 @@
         }
     }
 
     fn push_sorted_impl(&mut self, a: Atom) {
         let size = a.as_view().get_byte_size();
         self.mem_buf.push(a);
         self.mem_size += size;
+        self.num_terms += 1;
         self.total_size += size;
 
         if self.mem_size >= self.config.max_mem_bytes {
             self.sort();
 
             if self.mem_size * 2 > self.config.max_mem_bytes {
                 self.file_buf.push(W::create(&format!(
@@ -244,14 +258,15 @@
 
     /// Sort all the terms in the memory buffer.
     fn sort(&mut self) {
         self.mem_buf
             .par_sort_by(|a, b| a.as_view().cmp_terms(&b.as_view()));
 
         let mut out = Vec::with_capacity(self.mem_buf.len());
+        let old_size = self.mem_buf.len();
         let mut new_size = 0;
 
         if !self.mem_buf.is_empty() {
             let mut last_buf = self.mem_buf.remove(0);
 
             let mut handle: RecycledAtom = Atom::new().into();
 
@@ -282,14 +297,16 @@
             } else {
                 new_size += last_buf.as_view().get_byte_size();
                 out.push(last_buf);
             }
         }
 
         self.mem_buf = out;
+        self.num_terms += self.mem_buf.len();
+        self.num_terms -= old_size;
         self.total_size += new_size;
         self.total_size -= self.mem_size;
         self.mem_size = new_size;
     }
 
     /// Fuse sorted streams into one sorted stream.
     pub fn normalize(&mut self) {
@@ -438,17 +455,17 @@
                 });
             },
         );
 
         out_wrap.into_inner().unwrap()
     }
 
-    /// Map every term in the stream using the function `f` using a single core. The resulting terms
+    /// Map every term in the stream using the function `f` using a single thread. The resulting terms
     /// are a stream as well, which is returned by this function.
-    pub fn map_single_core(mut self, f: impl Fn(Atom) -> Atom) -> Self {
+    pub fn map_single_thread(&mut self, f: impl Fn(Atom) -> Atom) -> Self {
         let mut new_out = self.next_generation();
 
         let reader = self.reader();
 
         for x in reader {
             new_out.push(f(x));
         }
```

### Comparing `symbolica-0.5.0/src/tensors/matrix.rs` & `symbolica-0.6.0/src/tensors/matrix.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/src/utils.rs` & `symbolica-0.6.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/symbolica.pyi` & `symbolica-0.6.0/symbolica.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -762,14 +762,39 @@
         --------
 
         >>> from symbolica import Expression
         >>> p = Expression.parse('v1^2/2+v1^3/v4*v2+v3/(1+v4)')
         >>> print(p.together())
         """
 
+    def cancel(self) -> Expression:
+        """Cancel common factors between numerators and denominators.
+        Any non-canceling parts of the expression will not be rewritten.
+
+        Examples
+        --------
+
+        >>> from symbolica import Expression
+        >>> p = Expression.parse('1+(y+1)^10*(x+1)/(x^2+2x+1)')
+        >>> print(p.cancel())
+        1+(y+1)**10/(x+1)
+        """
+
+    def factor(self) -> Expression:
+        """Factor the expression over the rationals.
+
+        Examples
+        --------
+
+        >>> from symbolica import Expression
+        >>> p = Expression.parse('(6 + x)/(7776 + 6480*x + 2160*x^2 + 360*x^3 + 30*x^4 + x^5)')
+        >>> print(p.factor())
+        (x+6)**-4
+        """
+
     def to_polynomial(self, vars: Optional[Sequence[Expression]] = None) -> Polynomial:
         """Convert the expression to a polynomial, optionally, with the variable ordering specified in `vars`.
         All non-polynomial parts will be converted to new, independent variables.
         """
 
     def to_rational_polynomial(
         self,
@@ -799,15 +824,15 @@
         lhs: Transformer | Expression | int,
         cond: Optional[PatternRestriction] = None,
         level_range: Optional[Tuple[int, Optional[int]]] = None,
         level_is_tree_depth: Optional[bool] = False,
     ) -> MatchIterator:
         """
         Return an iterator over the pattern `self` matching to `lhs`.
-        Restrictions on pattern can be supplied through `cond`.
+        Restrictions on the pattern can be supplied through `cond`.
 
         The `level_range` specifies the `[min,max]` level at which the pattern is allowed to match.
         The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree,
         depending on `level_is_tree_depth`.
 
         Examples
         --------
@@ -816,14 +841,33 @@
         >>> f = Expression.symbol('f')
         >>> e = f(x)*f(1)*f(2)*f(3)
         >>> for match in e.match(f(x_)):
         >>>    for map in match:
         >>>        print(map[0],'=', map[1])
         """
 
+    def matches(
+        self,
+        lhs: Transformer | Expression | int,
+        cond: Optional[PatternRestriction] = None,
+        level_range: Optional[Tuple[int, Optional[int]]] = None,
+        level_is_tree_depth: Optional[bool] = False,
+    ) -> bool:
+        """
+        Test whether the pattern is found in the expression.
+        Restrictions on the pattern can be supplied through `cond`.
+
+        Examples
+        --------
+
+        >>> f = Expression.symbol('f')
+        >>> if f(1).matches(f(2)):
+        >>>    print('match')
+        """
+
     def replace(
         self,
         lhs: Transformer | Expression | int,
         rhs: Transformer | Expression | int,
         cond: Optional[PatternRestriction] = None,
         level_range: Optional[Tuple[int, Optional[int]]] = None,
         level_is_tree_depth: Optional[bool] = False,
@@ -888,14 +932,37 @@
         cond: Conditions on the pattern.
         non_greedy_wildcards: Wildcards that try to match as little as possible.
         level_range: Specifies the `[min,max]` level at which the pattern is allowed to match. The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree, depending on `level_is_tree_depth`.
         level_is_tree_depth: If set to `True`, the level is increased when going one level deeper in the expression tree.
         repeat: If set to `True`, the entire operation will be repeated until there are no more matches.
         """
 
+    def replace_all_multiple(self, replacements: Sequence[Replacement],  repeat: Optional[bool] = False) -> Expression:
+        """
+        Replace all atoms matching the patterns. See `replace_all` for more information.
+
+        The entire operation can be repeated until there are no more matches using `repeat=True`.
+
+        Examples
+        --------
+
+        >>> x, y, f = Expression.symbols('x', 'y', 'f')
+        >>> e = f(x,y)
+        >>> r = e.replace_all_multiple(Replacement(x, y), Replacement(y, x))
+        >>> print(r)
+        f(y,x)
+
+        Parameters
+        ----------
+        replacements: Sequence[Replacement]
+            The list of replacements to apply.
+        repeat: bool, optional
+            If set to `True`, the entire operation will be repeated until there are no more matches.
+       """
+
     @classmethod
     def solve_linear_system(
         _cls,
         system: Sequence[Expression],
         variables: Sequence[Expression],
     ) -> Sequence[Expression]:
         """Solve a linear system in the variables `variables`, where each expression
@@ -936,14 +1003,28 @@
         >>> from symbolica import Expression
         >>> x, y = Expression.symbols('x', 'y')
         >>> e = Expression.parse('sqrt(x)')*y
         >>> print(e.evaluate_complex({x: 1 + 2j, y: 4 + 3j}, {}))
         """
 
 
+class Replacement:
+    """A replacement of a pattern by a right-hand side."""
+
+    def __new__(
+            cls,
+            pattern: Transformer | Expression | int,
+            rhs: Transformer | Expression | int,
+            cond: Optional[PatternRestriction] = None,
+            non_greedy_wildcards: Optional[Sequence[Expression]] = None,
+            level_range: Optional[Tuple[int, Optional[int]]] = None,
+            level_is_tree_depth: Optional[bool] = False) -> Replacement:
+        """Create a new replacement. See `replace_all` for more information."""
+
+
 class PatternRestriction:
     """A restriction on wildcards."""
 
     def __and__(self, other: PatternRestriction) -> PatternRestriction:
         """Create a new pattern restriction that is the logical and operation between two restrictions (i.e., both should hold)."""
 
     def __or__(self, other: PatternRestriction) -> PatternRestriction:
@@ -1249,14 +1330,27 @@
         cond: Conditions on the pattern.
         non_greedy_wildcards: Wildcards that try to match as little as possible.
         level_range: Specifies the `[min,max]` level at which the pattern is allowed to match. The first level is 0 and the level is increased when going into a function or one level deeper in the expression tree, depending on `level_is_tree_depth`.
         level_is_tree_depth: If set to `True`, the level is increased when going one level deeper in the expression tree.
         repeat: If set to `True`, the entire operation will be repeated until there are no more matches.
         """
 
+    def replace_all_multiple(self, replacements: Sequence[Replacement]) -> Transformer:
+        """
+        Create a transformer that replaces all atoms matching the patterns. See `replace_all` for more information.
+
+        Examples
+        --------
+
+        >>> x, y, f = Expression.symbols('x', 'y', 'f')
+        >>> e = f(x,y)
+        >>> r = e.transform().replace_all_multiple(Replacement(x, y), Replacement(y, x))
+        >>> print(r)
+        """
+
     def print(
         self,
         terms_on_new_line: bool = False,
         color_top_level_sum: bool = True,
         color_builtin_symbols: bool = True,
         print_finite_field: bool = True,
         symmetric_representation_for_finite_field: bool = False,
@@ -1373,30 +1467,42 @@
 
     Supports standard arithmetic operations, such
     as addition and multiplication.
 
     Examples
     --------
     >>> x = Expression.symbol('x')
-    >>> s = Expression.parse("(1-cos(x))/sin(x)").series(x, 0, 4)
+    >>> s = Expression.parse("(1-cos(x))/sin(x)").series(x, 0, 4) * x
     >>> print(s)
     """
 
-    def __add__(self, other: Series) -> Series:
+    def __add__(self, other: Series | Expression) -> Series:
+        """Add another series or expression to this series, returning the result."""
+
+    def __radd__(self, other: Expression) -> Series:
         """Add two series together, returning the result."""
 
-    def __sub__(self, other: Series) -> Series:
+    def __sub__(self, other: Series | Expression) -> Series:
         """Subtract `other` from `self`, returning the result."""
 
-    def __mul__(self, other: Series) -> Series:
+    def __rsub__(self, other: Expression) -> Series:
+        """Subtract `self` from `other`, returning the result."""
+
+    def __mul__(self, other: Series | Expression) -> Series:
+        """Multiply another series or expression to this series, returning the result."""
+
+    def __rmul__(self, other: Expression) -> Series:
         """Multiply two series together, returning the result."""
 
-    def __truediv__(self, other: Series) -> Series:
+    def __truediv__(self, other: Series | Expression) -> Series:
         """Divide `self` by `other`, returning the result."""
 
+    def __rtruediv__(self, other: Expression) -> Series:
+        """Divide `other` by `self`, returning the result."""
+
     def __pow__(self, exp: int) -> Series:
         """Raise the series to the power of `exp`, returning the result."""
 
     def __neg__(self) -> Series:
         """Negate the series."""
 
     def sin(self) -> Series:
@@ -1413,46 +1519,72 @@
 
     def pow(self, num: int, den: int) -> Series:
         """Raise the series to the power of `num/den`, returning the result."""
 
     def spow(self, exp: Series) -> Series:
         """Raise the series to the power of `exp`, returning the result."""
 
+    def shift(self, e: int) -> Series:
+        """Shift the series by `e` units of the ramification."""
+
+    def get_ramification(self) -> int:
+        """Get the ramification."""
+
+    def get_trailing_exponent(self) -> Tuple[int, int]:
+        """Get the trailing exponent; the exponent of the first non-zero term."""
+
+    def get_absolute_order(self) -> Tuple[int, int]:
+        """Get the absolute order."""
+
     def to_expression(self) -> Expression:
-        """Convert the term stream into an expression. This may exceed the available memory."""
+        """Convert the series to an expression"""
 
 
 class TermStreamer:
+    """
+    A term streamer that can handle large expressions, by
+    streaming terms to and from disk.
+    """
+
     def __new__(_cls, path: Optional[str] = None,
                 max_mem_bytes: Optional[int] = None,
                 n_cores: Optional[int] = None) -> TermStreamer:
         """Create a new term streamer with a given path for its files,
            the maximum size of the memory buffer and the number of cores.
         """
 
     def __add__(self, other: TermStreamer) -> TermStreamer:
         """Add two term streamers together, returning the result."""
 
     def __iadd__(self, other: TermStreamer) -> None:
         """Add another term streamer to this one."""
 
     def get_byte_size(self) -> int:
-        """Get the byte size of the term streamer."""
+        """Get the byte size of the term stream."""
+
+    def get_num_terms(self) -> int:
+        """Get the number of terms in the stream."""
+
+    def fits_in_memory(self) -> bool:
+        """Check if the term stream fits in memory."""
 
     def push(self, expr: Expression) -> None:
-        """Push an expresssion to the term streamer."""
+        """Push an expresssion to the term stream."""
 
     def normalize(self) -> None:
-        """Sort and fuse all terms in the streamer."""
+        """Sort and fuse all terms in the stream."""
 
     def to_expression(self) -> Expression:
         """Convert the term stream into an expression. This may exceed the available memory."""
 
     def map(self, f: Transformer) -> TermStreamer:
-        """Apply a transformer to all terms in the streamer."""
+        """Apply a transformer to all terms in the stream."""
+
+    def map_single_thread(self, f: Transformer) -> TermStreamer:
+        """Apply a transformer to all terms in the stream using a single thread."""
 
 
 class MatchIterator:
     """An iterator over matches."""
 
     def __iter__(self) -> MatchIterator:
         """Create the iterator."""
@@ -1545,14 +1677,17 @@
 
     def __truediv__(self, rhs: Polynomial) -> Polynomial:
         """Divide the polynomial `self` by `rhs` if possible, returning the result."""
 
     def quot_rem(self, rhs: Polynomial) -> Tuple[Polynomial, Polynomial]:
         """Divide `self` by `rhs`, returning the quotient and remainder."""
 
+    def __mod__(self, rhs: Polynomial) -> Polynomial:
+        """Compute the remainder of the division of `self` by `rhs`."""
+
     def __neg__(self) -> Polynomial:
         """Negate the polynomial."""
 
     def gcd(self, rhs: Polynomial) -> Polynomial:
         """Compute the greatest common divisor (GCD) of two polynomials."""
 
     def resultant(self, rhs: Polynomial, var: Expression) -> Polynomial:
@@ -1629,16 +1764,16 @@
         --------
 
         >>> from symbolica import Expression
         >>> p = Expression.parse('3x^2+6x+9').to_polynomial()
         >>> print(p.content())
         """
 
-    def coefficient_list(self, x: Expression) -> list[Tuple[int, Polynomial]]:
-        """Get the coefficient list in `x`.
+    def coefficient_list(self, xs: Optional[Expression | Sequence[Expression]]) -> list[Tuple[list[int], Polynomial]]:
+        """Get the coefficient list, optionally in the variables `xs`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
         >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
@@ -1769,14 +1904,17 @@
 
     def __truediv__(self, rhs: IntegerPolynomial) -> IntegerPolynomial:
         """Divide the polynomial `self` by `rhs` if possible, returning the result."""
 
     def quot_rem(self, rhs: IntegerPolynomial) -> Tuple[IntegerPolynomial, IntegerPolynomial]:
         """Divide `self` by `rhs`, returning the quotient and remainder."""
 
+    def __mod__(self, rhs: IntegerPolynomial) -> IntegerPolynomial:
+        """Compute the remainder of the division of `self` by `rhs`."""
+
     def __neg__(self) -> IntegerPolynomial:
         """Negate the polynomial."""
 
     def gcd(self, rhs: IntegerPolynomial) -> IntegerPolynomial:
         """Compute the greatest common divisor (GCD) of two polynomials."""
 
     def resultant(self, rhs: IntegerPolynomial, var: Expression) -> IntegerPolynomial:
@@ -1829,16 +1967,16 @@
         --------
 
         >>> from symbolica import Expression
         >>> p = Expression.parse('3x^2+6x+9').to_polynomial().to_integer_polynomial()
         >>> print(p.content())
         """
 
-    def coefficient_list(self, x: Expression) -> list[Tuple[int, IntegerPolynomial]]:
-        """Get the coefficient list in `x`.
+    def coefficient_list(self, xs: Optional[Expression | Sequence[Expression]]) -> list[Tuple[list[int], IntegerPolynomial]]:
+        """Get the coefficient list, optionally in the variables `xs`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
         >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial().to_integer_polynomial()
@@ -1946,14 +2084,17 @@
 
     def __truediv__(self, rhs: FiniteFieldPolynomial) -> FiniteFieldPolynomial:
         """Divide the polynomial `self` by `rhs` if possible, returning the result."""
 
     def quot_rem(self, rhs: FiniteFieldPolynomial) -> Tuple[FiniteFieldPolynomial, FiniteFieldPolynomial]:
         """Divide `self` by `rhs`, returning the quotient and remainder."""
 
+    def __mod__(self, rhs: FiniteFieldPolynomial) -> FiniteFieldPolynomial:
+        """Compute the remainder of the division of `self` by `rhs`."""
+
     def __neg__(self) -> FiniteFieldPolynomial:
         """Negate the polynomial."""
 
     def gcd(self, rhs: FiniteFieldPolynomial) -> FiniteFieldPolynomial:
         """Compute the greatest common divisor (GCD) of two polynomials."""
 
     def resultant(self, rhs: FiniteFieldPolynomial, var: Expression) -> FiniteFieldPolynomial:
@@ -2026,16 +2167,16 @@
         --------
 
         >>> from symbolica import Expression
         >>> p = Expression.parse('3x^2+6x+9').to_polynomial()
         >>> print(p.content())
         """
 
-    def coefficient_list(self, x: Expression) -> list[Tuple[int, FiniteFieldPolynomial]]:
-        """Get the coefficient list in `x`.
+    def coefficient_list(self, xs: Optional[Expression | Sequence[Expression]]) -> list[Tuple[list[int], FiniteFieldPolynomial]]:
+        """Get the coefficient list, optionally in the variables `xs`.
 
         Examples
         --------
 
         >>> from symbolica import Expression
         >>> x = Expression.symbol('x')
         >>> p = Expression.parse('x*y+2*x+x^2').to_polynomial()
@@ -2321,14 +2462,16 @@
         >>> p = Expression.parse('1/((x+y)*(x^2+x*y+1)(x+1))').to_rational_polynomial()
         >>> for pp in p.apart(x):
         >>>     print(pp)
         """
 
 
 class Matrix:
+    """A matrix with rational polynomial coefficients."""
+
     def __new__(cls, nrows: int, ncols: int) -> Matrix:
         """Create a new zeroed matrix with `nrows` rows and `ncols` columns."""
 
     @classmethod
     def identity(cls, nrows: int) -> Matrix:
         """Create a new square matrix with `nrows` rows and ones on the main diagonal and zeroes elsewhere."""
 
@@ -2415,19 +2558,23 @@
         """Divide this matrix by scalar `rhs` and return the result."""
 
     def __neg__(self) -> Matrix:
         """Negate the matrix, returning the result."""
 
 
 class Evaluator:
+    """An optimized evaluator of an expression."""
+
     def evaluate(self, inputs: Sequence[Sequence[float]]) -> List[float]:
         """Evaluate the polynomial for multiple inputs and return the result."""
 
 
 class NumericalIntegrator:
+    """A numerical integrator for high-dimensional integrals."""
+
     @classmethod
     def continuous(
         _cls,
         n_dims: int,
         n_bins: int = 128,
         min_samples_for_update: int = 100,
         bin_number_evolution: Optional[Sequence[int]] = None,
```

### Comparing `symbolica-0.5.0/tests/import_export.rs` & `symbolica-0.6.0/tests/import_export.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/tests/pattern_matching.rs` & `symbolica-0.6.0/tests/pattern_matching.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/tests/rational_polynomial.rs` & `symbolica-0.6.0/tests/rational_polynomial.rs`

 * *Files identical despite different names*

### Comparing `symbolica-0.5.0/pyproject.toml` & `symbolica-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ]
 summary = "Symbolica is a blazing fast computer algebra system"
 description = "Symbolica is a blazing fast computer algebra system"
 keywords = ["math", "algebra", "polynomial", "expression", "manipulation"]
 license = {file = "License.md"}
 name = "symbolica"
 readme = "Readme.md"
-version = "0.5.0"
+version = "0.6.0"
 
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Rust",
   "Topic :: Scientific/Engineering :: Mathematics",
 ]
```

### Comparing `symbolica-0.5.0/PKG-INFO` & `symbolica-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: symbolica
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 License-File: License.md
 License-File: License.md
 Summary: Symbolica is a blazing fast computer algebra system
 Keywords: math,algebra,polynomial,expression,manipulation
@@ -62,15 +62,15 @@
 
 ## Rust
 
 If you want to use Symbolica as a library in Rust, simply include it in the `Cargo.toml`:
 
 ```toml
 [dependencies]
-symbolica = "0.5"
+symbolica = "0.6"
 ```
 
 # Examples
 
 Below we list some examples of the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a complete overview.
 
 ### Pattern matching
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: symbolica Version: 0.5.0 Classifier: Development
+Metadata-Version: 2.3 Name: symbolica Version: 0.6.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Programming Language :: Rust Classifier: Topic
 :: Scientific/Engineering :: Mathematics License-File: License.md License-File:
 License.md Summary: Symbolica is a blazing fast computer algebra system
 Keywords: math,algebra,polynomial,expression,manipulation Author: Ben Ruijl
 Author-email: benruyl@gmail.com Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://symbolica.io Project-
 URL: repository, https://github.com/benruijl/symbolica
@@ -22,15 +22,15 @@
 (probably) already know, by using Symbolica's bindings to Python, Rust and C++:
 [A demo of Symbolica]# Installation Visit the [Get Started](https://
 symbolica.io/docs/get_started.html) page for detailed installation
 instructions. ## Python Symbolica can be installed for Python >3.5 using `pip`:
 ```sh pip install symbolica ``` The installation may take some time on Mac OS
 and Windows, as it may have to compile Symbolica. ## Rust If you want to use
 Symbolica as a library in Rust, simply include it in the `Cargo.toml`: ```toml
-[dependencies] symbolica = "0.5" ``` # Examples Below we list some examples of
+[dependencies] symbolica = "0.6" ``` # Examples Below we list some examples of
 the features of Symbolica. Check the [guide](https://symbolica.io/docs/) for a
 complete overview. ### Pattern matching Variables ending with a `_` are
 wildcards that match to any subexpression. In the following example we try to
 match the pattern `f(w1_,w2_)`: ```python from symbolica import Expression x,
 y, w1_, w2_ = Expression.vars('x','y','w1_','w2_') f = Expression.fun('f') e =
 f(3,x)*y**2+5 r = e.replace_all(f(w1_,w2_), f(w1_ - 1, w2_**2)) print(r) ```
 which yields `y^2*f(2,x^2)+5`. ### Solving a linear system Solve a linear
```

