# Comparing `tmp/py_rattler-0.5.0.tar.gz` & `tmp/py_rattler-0.6.0.tar.gz`

## Comparing `py_rattler-0.5.0.tar` & `py_rattler-0.6.0.tar`

### file list

```diff
@@ -1,455 +1,493 @@
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_digest/Cargo.toml
--rw-r--r--   0     1001      127      987 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_digest/CHANGELOG.md
--rw-r--r--   0     1001      127     7607 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_digest/src/lib.rs
--rw-r--r--   0     1001      127     3521 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_digest/src/serde.rs
--rw-r--r--   0     1001      127     2155 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_digest/src/tokio.rs
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/Cargo.toml
--rw-r--r--   0     1001      127     2795 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/CHANGELOG.md
--rw-r--r--   0     1001      127     2053 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/fs.rs
--rw-r--r--   0     1001      127     1995 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/lib.rs
--rw-r--r--   0     1001      127     3671 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/read.rs
--rw-r--r--   0     1001      127       98 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
--rw-r--r--   0     1001      127     5107 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
--rw-r--r--   0     1001      127     4387 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/seek.rs
--rw-r--r--   0     1001      127     1732 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
--rw-r--r--   0     1001      127     3101 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
--rw-r--r--   0     1001      127      113 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
--rw-r--r--   0     1001      127    13544 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/write.rs
--rw-r--r--   0     1001      127     9265 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/tests/extract.rs
--rw-r--r--   0     1001      127     7880 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_package_streaming/tests/write.rs
--rw-r--r--   0        0        0     1204 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/Cargo.toml
--rw-r--r--   0     1001      127     2841 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/CHANGELOG.md
--rw-r--r--   0     1001      127     3391 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/benches/bench.rs
--rw-r--r--   0     1001      127     6204 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/lib.rs
--rw-r--r--   0     1001      127    12667 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs
--rw-r--r--   0     1001      127     1173 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
--rw-r--r--   0     1001      127     9282 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
--rw-r--r--   0     1001      127     2444 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs
--rw-r--r--   0     1001      127      561 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
--rw-r--r--   0     1001      127      864 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
--rw-r--r--   0     1001      127     1047 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
--rw-r--r--   0     1001      127    11669 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
--rw-r--r--   0     1001      127     2720 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
--rw-r--r--   0     1001      127     6299 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
--rw-r--r--   0     1001      127     3402 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
--rw-r--r--   0     1001      127     1262 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
--rw-r--r--   0     1001      127     3451 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
--rw-r--r--   0     1001      127     4718 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
--rw-r--r--   0     1001      127     5589 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
--rw-r--r--   0     1001      127     2468 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
--rw-r--r--   0     1001      127     7394 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
--rw-r--r--   0     1001      127    20180 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/src/resolvo/mod.rs
--rw-r--r--   0     1001      127    28787 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/backends.rs
--rw-r--r--   0     1001      127      165 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      738 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
--rw-r--r--   0     1001      127     1105 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3069 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
--rw-r--r--   0     1001      127     2590 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3631 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
--rw-r--r--   0     1001      127      216 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
--rw-r--r--   0     1001      127      411 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
--rw-r--r--   0     1001      127      172 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
--rw-r--r--   0     1001      127      412 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
--rw-r--r--   0     1001      127      736 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
--rw-r--r--   0     1001      127     1103 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
--rw-r--r--   0     1001      127     3067 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
--rw-r--r--   0     1001      127     2588 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
--rw-r--r--   0     1001      127     3629 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
--rw-r--r--   0     1001      127      588 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
--rw-r--r--   0     1001      127      400 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/Cargo.toml
--rw-r--r--   0     1001      127     2324 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/CHANGELOG.md
--rw-r--r--   0     1001      127    13677 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_middleware.rs
--rw-r--r--   0     1001      127     1266 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
--rw-r--r--   0     1001      127     6690 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
--rw-r--r--   0     1001      127     2852 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
--rw-r--r--   0     1001      127      103 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
--rw-r--r--   0     1001      127     5769 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
--rw-r--r--   0     1001      127      270 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
--rw-r--r--   0     1001      127      727 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
--rw-r--r--   0     1001      127     5643 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
--rw-r--r--   0     1001      127     2287 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/gcs_middleware.rs
--rw-r--r--   0     1001      127      726 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/lib.rs
--rw-r--r--   0     1001      127    10299 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/mirror_middleware.rs
--rw-r--r--   0     1001      127    10902 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/oci_middleware.rs
--rw-r--r--   0     1001      127     3489 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/redaction.rs
--rw-r--r--   0     1001      127      920 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_networking/src/retry_policies.rs
--rw-r--r--   0        0        0      747 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/Cargo.toml
--rw-r--r--   0     1001      127     2380 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md
--rw-r--r--   0     1001      127    11042 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/cuda.rs
--rw-r--r--   0     1001      127    12929 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/lib.rs
--rw-r--r--   0     1001      127     3047 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/libc.rs
--rw-r--r--   0     1001      127     3969 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/linux.rs
--rw-r--r--   0     1001      127     2381 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/osx.rs
--rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_index/Cargo.toml
--rw-r--r--   0     1001      127     2243 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_index/CHANGELOG.md
--rw-r--r--   0     1001      127     6971 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_index/src/lib.rs
--rw-r--r--   0     1001      127     2162 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_index/tests/test_index.rs
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/Cargo.toml
--rw-r--r--   0     1001      127     1011 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md
--rw-r--r--   0     1001      127     1394 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/build.rs
--rw-r--r--   0     1001      127    77341 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/src/lib.rs
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/Cargo.toml
--rw-r--r--   0     1001      127     2524 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/CHANGELOG.md
--rw-r--r--   0     1001      127     6914 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/builder.rs
--rw-r--r--   0     1001      127      871 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/channel.rs
--rw-r--r--   0     1001      127     5813 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/conda.rs
--rw-r--r--   0     1001      127     4879 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/hash.rs
--rw-r--r--   0     1001      127    23416 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/lib.rs
--rw-r--r--   0     1001      127     5861 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/deserialize.rs
--rw-r--r--   0     1001      127     2866 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/mod.rs
--rw-r--r--   0     1001      127     8928 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/serialize.rs
--rw-r--r--   0     1001      127     8432 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/v3.rs
--rw-r--r--   0     1001      127     5293 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/pypi.rs
--rw-r--r--   0     1001      127    15803 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
--rw-r--r--   0     1001      127    22538 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
--rw-r--r--   0     1001      127   487178 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
--rw-r--r--   0     1001      127    40003 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
--rw-r--r--   0     1001      127    52188 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
--rw-r--r--   0     1001      127  1811360 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
--rw-r--r--   0     1001      127   487178 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
--rw-r--r--   0     1001      127    19628 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
--rw-r--r--   0     1001      127    40003 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
--rw-r--r--   0     1001      127    52188 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
--rw-r--r--   0     1001      127  1811360 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
--rw-r--r--   0     1001      127     9470 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/url_or_path.rs
--rw-r--r--   0     1001      127       22 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/mod.rs
--rw-r--r--   0     1001      127     1693 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
--rw-r--r--   0     1001      127      372 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/mod.rs
--rw-r--r--   0     1001      127     2012 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
--rw-r--r--   0     1001      127     1571 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
--rw-r--r--   0     1001      127     7899 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
--rw-r--r--   0     1001      127     1441 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
--rw-r--r--   0     1001      127     1407 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
--rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/Cargo.toml
--rw-r--r--   0     1001      127     2231 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/CHANGELOG.md
--rw-r--r--   0     1001      127    27911 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/activation.rs
--rw-r--r--   0     1001      127      196 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/lib.rs
--rw-r--r--   0     1001      127     2232 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/run/mod.rs
--rw-r--r--   0     1001      127    28471 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/mod.rs
--rw-r--r--   0     1001      127      123 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
--rw-r--r--   0     1001      127      128 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
--rw-r--r--   0     1001      127      104 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
--rw-r--r--   0     1001      127      122 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
--rw-r--r--   0     1001      127      237 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
--rw-r--r--   0     1001      127      185 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
--rw-r--r--   0     1001      127      190 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
--rw-r--r--   0     1001      127      192 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
--rw-r--r--   0     1001      127      239 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
--rw-r--r--   0     1001      127      237 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
--rw-r--r--   0     1001      127      171 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
--rw-r--r--   0     1001      127      237 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
--rw-r--r--   0     1001      127      237 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
--rw-r--r--   0     1001      127      229 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
--rw-r--r--   0     1001      127      202 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
--rw-r--r--   0     1001      127      202 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
--rw-r--r--   0     1001      127      195 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
--rw-r--r--   0     1001      127      311 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
--rw-r--r--   0     1001      127      311 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
--rw-r--r--   0     1001      127      301 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/Cargo.toml
--rw-r--r--   0     1001      127      987 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/CHANGELOG.md
--rw-r--r--   0     1001      127     2664 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/src/lib.rs
--rw-r--r--   0     1001      127      113 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
--rw-r--r--   0     1001      127      155 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
--rw-r--r--   0     1001      127      113 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
--rw-r--r--   0     1001      127      127 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
--rw-r--r--   0     1001      127      155 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
--rw-r--r--   0     1001      127      137 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
--rw-r--r--   0     1001      127      251 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_macros/tests/tests.rs
--rw-r--r--   0        0        0     2384 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/Cargo.toml
--rw-r--r--   0     1001      127     2841 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
--rw-r--r--   0     1001      127     2806 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
--rw-r--r--   0     1001      127     7713 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
--rw-r--r--   0     1001      127      956 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
--rw-r--r--   0     1001      127      465 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
--rw-r--r--   0     1001      127      604 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
--rw-r--r--   0     1001      127    38988 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
--rw-r--r--   0     1001      127    53507 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
--rw-r--r--   0     1001      127     1919 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/lib.rs
--rw-r--r--   0     1001      127    18866 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
--rw-r--r--   0     1001      127     2718 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
--rw-r--r--   0     1001      127    13393 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
--rw-r--r--   0     1001      127     1674 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
--rw-r--r--   0     1001      127     2483 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
--rw-r--r--   0        0        0     1437 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/Cargo.toml
--rw-r--r--   0     1001      127     3084 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/CHANGELOG.md
--rw-r--r--   0     1001      127     1016 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/benches/parse.rs
--rw-r--r--   0     1001      127     3220 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
--rw-r--r--   0     1001      127     6519 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
--rw-r--r--   0     1001      127    23104 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/channel/mod.rs
--rw-r--r--   0     1001      127     4187 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/channel_data.rs
--rw-r--r--   0     1001      127    11580 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
--rw-r--r--   0     1001      127      770 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127     2206 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/lib.rs
--rw-r--r--   0     1001      127     6012 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
--rw-r--r--   0     1001      127    20136 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
--rw-r--r--   0     1001      127    28532 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
--rw-r--r--   0     1001      127      506 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
--rw-r--r--   0     1001      127      537 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
--rw-r--r--   0     1001      127     5570 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs
--rw-r--r--   0     1001      127     3206 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/about.rs
--rw-r--r--   0     1001      127     4183 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
--rw-r--r--   0     1001      127     1400 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs
--rw-r--r--   0     1001      127     3244 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs
--rw-r--r--   0     1001      127     1348 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/files.rs
--rw-r--r--   0     1001      127     6474 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
--rw-r--r--   0     1001      127     3942 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/index.rs
--rw-r--r--   0     1001      127     1977 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/link.rs
--rw-r--r--   0     1001      127     3607 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/mod.rs
--rw-r--r--   0     1001      127     1510 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/no_link.rs
--rw-r--r--   0     1001      127     1495 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
--rw-r--r--   0     1001      127      507 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
--rw-r--r--   0     1001      127    12393 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/paths.rs
--rw-r--r--   0     1001      127     2334 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs
--rw-r--r--   0     1001      127      754 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
--rw-r--r--   0     1001      127     2515 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
--rw-r--r--   0     1001      127      134 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
--rw-r--r--   0     1001      127      329 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
--rw-r--r--   0     1001      127      309 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
--rw-r--r--   0     1001      127      349 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
--rw-r--r--   0     1001      127      137 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
--rw-r--r--   0     1001      127      138 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
--rw-r--r--   0     1001      127     1171 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
--rw-r--r--   0     1001      127      776 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
--rw-r--r--   0     1001      127      601 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
--rw-r--r--   0     1001      127     6782 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
--rw-r--r--   0     1001      127      185 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
--rw-r--r--   0     1001      127     5305 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package_name.rs
--rw-r--r--   0     1001      127      233 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/parse_mode.rs
--rw-r--r--   0     1001      127    15923 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/platform.rs
--rw-r--r--   0     1001      127    12758 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/prefix_record.rs
--rw-r--r--   0     1001      127    19433 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
--rw-r--r--   0     1001      127    10542 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
--rw-r--r--   0     1001      127      181 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
--rw-r--r--   0     1001      127     2154 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
--rw-r--r--   0     1001      127     2091 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
--rw-r--r--   0     1001      127      843 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
--rw-r--r--   0     1001      127     1595 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
--rw-r--r--   0     1001      127      813 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
--rw-r--r--   0     1001      127     4832 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
--rw-r--r--   0     1001      127      232 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
--rw-r--r--   0     1001      127     6062 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
--rw-r--r--   0     1001      127     4832 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
--rw-r--r--   0     1001      127    75110 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
--rw-r--r--   0     1001      127     1080 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs
--rw-r--r--   0     1001      127      455 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/run_export.rs
--rw-r--r--   0     1001      127    53039 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
--rw-r--r--   0     1001      127      353 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
--rw-r--r--   0     1001      127      974 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
--rw-r--r--   0     1001      127     2269 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
--rw-r--r--   0     1001      127    12047 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
--rw-r--r--   0     1001      127   269415 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     4590 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
--rw-r--r--   0     1001      127    12519 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127   345345 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
--rw-r--r--   0     1001      127    23076 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     1054 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
--rw-r--r--   0     1001      127    12151 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
--rw-r--r--   0     1001      127     7102 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
--rw-r--r--   0     1001      127       22 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/utils/mod.rs
--rw-r--r--   0     1001      127     6107 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/utils/serde.rs
--rw-r--r--   0     1001      127     1531 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/bump.rs
--rw-r--r--   0     1001      127     3760 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/flags.rs
--rw-r--r--   0     1001      127    53168 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/mod.rs
--rw-r--r--   0     1001      127    18817 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/parse.rs
--rw-r--r--   0     1001      127     6410 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/segment.rs
--rw-r--r--   0     1001      127     2495 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
--rw-r--r--   0     1001      127     4834 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/with_source.rs
--rw-r--r--   0     1001      127    10418 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
--rw-r--r--   0     1001      127    18331 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
--rw-r--r--   0     1001      127    16688 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
--rw-r--r--   0     1001      127    14591 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 py_rattler-0.5.0/local_dependencies/rattler/Cargo.toml
--rw-r--r--   0     1001      127        8 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/.gitignore
--rw-r--r--   0     1001      127     4017 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/CHANGELOG.md
--rw-r--r--   0     1001      127    74752 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/resources/launcher64.exe
--rw-r--r--   0     1001      127    99068 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/resources/versions.txt
--rw-r--r--   0     1001      127     4798 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/cli/auth.rs
--rw-r--r--   0     1001      127      122 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/cli/mod.rs
--rw-r--r--   0     1001      127     1358 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/apple_codesign.rs
--rw-r--r--   0     1001      127    35157 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/clobber_registry.rs
--rw-r--r--   0     1001      127    11336 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/driver.rs
--rw-r--r--   0     1001      127     8511 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/entry_point.rs
--rw-r--r--   0     1001      127    32064 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/link.rs
--rw-r--r--   0     1001      127     9164 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/link_script.rs
--rw-r--r--   0     1001      127    32794 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/mod.rs
--rw-r--r--   0     1001      127     3839 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/python.rs
--rw-r--r--   0     1001      127      609 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
--rw-r--r--   0     1001      127      190 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
--rw-r--r--   0     1001      127      727 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
--rw-r--r--   0     1001      127      142 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
--rw-r--r--   0     1001      127      609 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
--rw-r--r--   0     1001      127      727 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
--rw-r--r--   0     1001      127      142 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
--rw-r--r--   0     1001      127      297 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
--rw-r--r--   0     1001      127      271 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
--rw-r--r--   0     1001      127      155 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
--rw-r--r--   0     1001      127     3732 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
--rw-r--r--   0     1001      127     4666 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/test_utils.rs
--rw-r--r--   0     1001      127     7975 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/transaction.rs
--rw-r--r--   0     1001      127     9414 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/install/unlink.rs
--rw-r--r--   0     1001      127     2983 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/lib.rs
--rw-r--r--   0     1001      127    19867 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/package_cache.rs
--rw-r--r--   0     1001      127    24363 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/range.rs
--rw-r--r--   0     1001      127    13477 2024-04-26 08:54:04.000000 py_rattler-0.5.0/local_dependencies/rattler/src/validation.rs
--rw-r--r--   0        0        0     2060 1970-01-01 00:00:00.000000 py_rattler-0.5.0/Cargo.toml
--rw-r--r--   0     1001      127      743 2024-04-26 08:54:04.000000 py_rattler-0.5.0/.gitignore
--rw-r--r--   0     1001      127     1502 2024-04-26 08:54:04.000000 py_rattler-0.5.0/LICENSE
--rw-r--r--   0     1001      127     6332 2024-04-26 08:54:04.000000 py_rattler-0.5.0/README.md
--rw-r--r--   0     1001      127       71 2024-04-26 08:54:04.000000 py_rattler-0.5.0/build.rs
--rw-r--r--   0     1001      127       44 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/about_json.md
--rw-r--r--   0     1001      127       45 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/activate.md
--rw-r--r--   0     1001      127       58 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/activation_error.md
--rw-r--r--   0     1001      127       61 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/activation_result.md
--rw-r--r--   0     1001      127       67 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/activation_variables.md
--rw-r--r--   0     1001      127       34 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/arch.md
--rw-r--r--   0     1001      127       62 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/authenticated_client.md
--rw-r--r--   0     1001      127       54 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/cache_dir_error.md
--rw-r--r--   0     1001      127       39 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/channel.md
--rw-r--r--   0     1001      127       52 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/channel_config.md
--rw-r--r--   0     1001      127       79 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/detect_virtual_package_error.md
--rw-r--r--   0     1001      127       44 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/environment.md
--rw-r--r--   0     1001      127       76 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/environment_creation_error.md
--rw-r--r--   0     1001      127       58 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/fetch_repo_data.md
--rw-r--r--   0     1001      127       65 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/fetch_repo_data_error.md
--rw-r--r--   0     1001      127       51 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/file_mode.md
--rw-r--r--   0     1001      127       61 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/generic_virtual_package.md
--rw-r--r--   0     1001      127     5592 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/index.md
--rw-r--r--   0     1001      127       44 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/index_json.md
--rw-r--r--   0     1001      127       67 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/invalid_channel_error.md
--rw-r--r--   0     1001      127       71 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/invalid_match_spec_error.md
--rw-r--r--   0     1001      127       75 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/invalid_package_name_error.md
--rw-r--r--   0     1001      127       59 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/invalid_url_error.md
--rw-r--r--   0     1001      127       67 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/invalid_version_error.md
--rw-r--r--   0     1001      127       43 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/io_error.md
--rw-r--r--   0     1001      127       47 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/link_error.md
--rw-r--r--   0     1001      127       34 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/linker.md
--rw-r--r--   0     1001      127       38 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/lock_file.md
--rw-r--r--   0     1001      127       48 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/locked_package.md
--rw-r--r--   0     1001      127       47 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/match_spec.md
--rw-r--r--   0     1001      127       64 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/nameless_match_spec.md
--rw-r--r--   0     1001      127       48 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/package_hashes.md
--rw-r--r--   0     1001      127       48 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/package_name.md
--rw-r--r--   0     1001      127       54 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/package_record.md
--rw-r--r--   0     1001      127       57 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/parse_arch_error.md
--rw-r--r--   0     1001      127       65 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/parse_platform_error.md
--rw-r--r--   0     1001      127       62 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/patch_instructions.md
--rw-r--r--   0     1001      127       77 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/path_modification_behavior.md
--rw-r--r--   0     1001      127       52 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/path_type.md
--rw-r--r--   0     1001      127       56 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/paths_entry.md
--rw-r--r--   0     1001      127       55 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/paths_json.md
--rw-r--r--   0     1001      127       42 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/platform.md
--rw-r--r--   0     1001      127       47 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/prefix_paths.md
--rw-r--r--   0     1001      127       69 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/prefix_placeholder.md
--rw-r--r--   0     1001      127       49 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/prefix_record.md
--rw-r--r--   0     1001      127       52 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/pypi_package_data.md
--rw-r--r--   0     1001      127       74 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/pypi_package_environment_data.md
--rw-r--r--   0     1001      127       44 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/repo_data.md
--rw-r--r--   0     1001      127       47 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/repo_data_record.md
--rw-r--r--   0     1001      127       56 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/run_exports_json.md
--rw-r--r--   0     1001      127       39 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/shell.md
--rw-r--r--   0     1001      127       35 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/solver.md
--rw-r--r--   0     1001      127       51 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/solver_error.md
--rw-r--r--   0     1001      127       47 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/sparse_repo_data.md
--rw-r--r--   0     1001      127      871 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/stylesheets/extra.css
--rw-r--r--   0     1001      127       61 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/transaction_error.md
--rw-r--r--   0     1001      127       39 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/version.md
--rw-r--r--   0     1001      127       53 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/version_with_source.md
--rw-r--r--   0     1001      127       62 2024-04-26 08:54:04.000000 py_rattler-0.5.0/docs/virtual_package.md
--rw-r--r--   0     1001      127     3847 2024-04-26 08:54:04.000000 py_rattler-0.5.0/mkdocs.yml
--rw-r--r--   0     1001      127   191576 2024-04-26 08:54:04.000000 py_rattler-0.5.0/pixi.lock
--rw-r--r--   0     1001      127     1764 2024-04-26 08:54:04.000000 py_rattler-0.5.0/pixi.toml
--rw-r--r--   0     1001      127     1863 2024-04-26 08:54:04.000000 py_rattler-0.5.0/pyproject.toml
--rw-r--r--   0     1001      127     1982 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/__init__.py
--rw-r--r--   0     1001      127      221 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/channel/__init__.py
--rw-r--r--   0     1001      127     2295 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/channel/channel.py
--rw-r--r--   0     1001      127     1532 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/channel/channel_config.py
--rw-r--r--   0     1001      127      474 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/channel/channel_priority.py
--rw-r--r--   0     1001      127     3664 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/exceptions.py
--rw-r--r--   0     1001      127       59 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/index/__init__.py
--rw-r--r--   0     1001      127     1133 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/index/index.py
--rw-r--r--   0     1001      127       59 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/linker/__init__.py
--rw-r--r--   0     1001      127     1959 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/linker/linker.py
--rw-r--r--   0     1001      127      471 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/__init__.py
--rw-r--r--   0     1001      127     1277 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/channel.py
--rw-r--r--   0     1001      127     7624 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/environment.py
--rw-r--r--   0     1001      127      805 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/hash.py
--rw-r--r--   0     1001      127     3264 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/lock_file.py
--rw-r--r--   0     1001      127     5336 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/package.py
--rw-r--r--   0     1001      127     6544 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/lock/pypi.py
--rw-r--r--   0     1001      127      167 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/match_spec/__init__.py
--rw-r--r--   0     1001      127     7953 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/match_spec/match_spec.py
--rw-r--r--   0     1001      127     4293 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/match_spec/nameless_match_spec.py
--rw-r--r--   0     1001      127      189 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/networking/__init__.py
--rw-r--r--   0     1001      127      915 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/networking/authenticated_client.py
--rw-r--r--   0     1001      127     1393 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/networking/fetch_repo_data.py
--rw-r--r--   0     1001      127      518 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/__init__.py
--rw-r--r--   0     1001      127     7060 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/about_json.py
--rw-r--r--   0     1001      127     9422 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/index_json.py
--rw-r--r--   0     1001      127     4111 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/package_name.py
--rw-r--r--   0     1001      127    14664 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/paths_json.py
--rw-r--r--   0     1001      127     6238 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/package/run_exports_json.py
--rw-r--r--   0     1001      127      118 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/platform/__init__.py
--rw-r--r--   0     1001      127     1145 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/platform/arch.py
--rw-r--r--   0     1001      127     3993 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/platform/platform.py
--rw-r--r--   0     1001      127      221 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/prefix/__init__.py
--rw-r--r--   0     1001      127     8514 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/prefix/prefix_paths.py
--rw-r--r--   0     1001      127     4514 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/prefix/prefix_record.py
--rw-r--r--   0     1001      127        0 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/py.typed
--rw-r--r--   0     1001      127      400 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/__init__.py
--rw-r--r--   0     1001      127    12456 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/package_record.py
--rw-r--r--   0     1001      127      694 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/patch_instructions.py
--rw-r--r--   0     1001      127     2660 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/record.py
--rw-r--r--   0     1001      127     2264 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/repo_data.py
--rw-r--r--   0     1001      127     6245 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/repo_data/sparse.py
--rw-r--r--   0     1001      127      179 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/shell/__init__.py
--rw-r--r--   0     1001      127     4442 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/shell/shell.py
--rw-r--r--   0     1001      127       61 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/solver/__init__.py
--rw-r--r--   0     1001      127     3342 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/solver/solver.py
--rw-r--r--   0     1001      127      526 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/utils/rattler_version.py
--rw-r--r--   0     1001      127      146 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/version/__init__.py
--rw-r--r--   0     1001      127    14442 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/version/version.py
--rw-r--r--   0     1001      127     2590 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/version/with_source.py
--rw-r--r--   0     1001      127      188 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/virtual_package/__init__.py
--rw-r--r--   0     1001      127     4411 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/virtual_package/generic.py
--rw-r--r--   0     1001      127     1509 2024-04-26 08:54:04.000000 py_rattler-0.5.0/rattler/virtual_package/virtual_package.py
--rw-r--r--   0     1001      127     4356 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/about_json.rs
--rw-r--r--   0     1001      127     2913 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/channel/mod.rs
--rw-r--r--   0     1001      127     6663 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/error.rs
--rw-r--r--   0     1001      127     1743 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/generic_virtual_package.rs
--rw-r--r--   0     1001      127      593 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/index.rs
--rw-r--r--   0     1001      127     5113 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/index_json.rs
--rw-r--r--   0     1001      127     6135 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/lib.rs
--rw-r--r--   0     1001      127     8220 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/linker.rs
--rw-r--r--   0     1001      127    15021 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/lock/mod.rs
--rw-r--r--   0     1001      127     3683 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/match_spec.rs
--rw-r--r--   0     1001      127      147 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/meta.rs
--rw-r--r--   0     1001      127     3550 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/nameless_match_spec.rs
--rw-r--r--   0     1001      127     1017 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/networking/authenticated_client.rs
--rw-r--r--   0     1001      127      804 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/networking/cached_repo_data.rs
--rw-r--r--   0     1001      127     3260 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/networking/mod.rs
--rw-r--r--   0     1001      127     2124 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/package_name.rs
--rw-r--r--   0     1001      127     9546 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/paths_json.rs
--rw-r--r--   0     1001      127     2749 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/platform.rs
--rw-r--r--   0     1001      127     5691 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/prefix_paths.rs
--rw-r--r--   0     1001      127    13111 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/record.rs
--rw-r--r--   0     1001      127     1655 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/repo_data/mod.rs
--rw-r--r--   0     1001      127      189 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/repo_data/patch_instructions.rs
--rw-r--r--   0     1001      127     2096 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/repo_data/sparse.rs
--rw-r--r--   0     1001      127     4469 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/run_exports_json.rs
--rw-r--r--   0     1001      127     3878 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/shell.rs
--rw-r--r--   0     1001      127     1972 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/solver.rs
--rw-r--r--   0     1001      127      814 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/version/component.rs
--rw-r--r--   0     1001      127     5550 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/version/mod.rs
--rw-r--r--   0     1001      127     1190 2024-04-26 08:54:04.000000 py_rattler-0.5.0/src/virtual_package.rs
--rw-r--r--   0     1001      127        0 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/__init__.py
--rw-r--r--   0     1001      127     2167 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_fetch_repo_data.py
--rw-r--r--   0     1001      127     2159 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_index.py
--rw-r--r--   0     1001      127      866 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_link.py
--rw-r--r--   0     1001      127     1559 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_prefix_record.py
--rw-r--r--   0     1001      127     1805 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_solver.py
--rw-r--r--   0     1001      127      691 2024-04-26 08:54:04.000000 py_rattler-0.5.0/tests/unit/test_version.py
--rw-r--r--   0     1001      127   105563 2024-04-26 08:54:04.000000 py_rattler-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     7318 1970-01-01 00:00:00.000000 py_rattler-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/Cargo.toml
+-rw-r--r--   0     1001      127     1011 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md
+-rw-r--r--   0     1001      127     1394 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/build.rs
+-rw-r--r--   0     1001      127    77341 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/src/lib.rs
+-rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/Cargo.toml
+-rw-r--r--   0     1001      127     4106 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/CHANGELOG.md
+-rw-r--r--   0     1001      127     2053 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/fs.rs
+-rw-r--r--   0     1001      127     2392 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/lib.rs
+-rw-r--r--   0     1001      127     3671 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/read.rs
+-rw-r--r--   0     1001      127       98 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/mod.rs
+-rw-r--r--   0     1001      127     6148 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs
+-rw-r--r--   0     1001      127     4387 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/seek.rs
+-rw-r--r--   0     1001      127     1732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs
+-rw-r--r--   0     1001      127     3101 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs
+-rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/mod.rs
+-rw-r--r--   0     1001      127    14225 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/write.rs
+-rw-r--r--   0     1001      127     9266 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/extract.rs
+-rw-r--r--   0     1001      127     7864 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/write.rs
+-rw-r--r--   0        0        0     1258 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/Cargo.toml
+-rw-r--r--   0     1001      127     3679 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/CHANGELOG.md
+-rw-r--r--   0     1001      127     8878 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/builder.rs
+-rw-r--r--   0     1001      127      871 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/channel.rs
+-rw-r--r--   0     1001      127     5792 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/conda.rs
+-rw-r--r--   0     1001      127     2006 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/file_format_version.rs
+-rw-r--r--   0     1001      127     4879 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/hash.rs
+-rw-r--r--   0     1001      127    24726 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/lib.rs
+-rw-r--r--   0     1001      127     6083 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/deserialize.rs
+-rw-r--r--   0     1001      127     2613 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/mod.rs
+-rw-r--r--   0     1001      127     9114 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/serialize.rs
+-rw-r--r--   0     1001      127     8630 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/v3.rs
+-rw-r--r--   0     1001      127     5293 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi.rs
+-rw-r--r--   0     1001      127     1480 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi_indexes.rs
+-rw-r--r--   0     1001      127    15803 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap
+-rw-r--r--   0     1001      127    22538 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap
+-rw-r--r--   0     1001      127   487177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap
+-rw-r--r--   0     1001      127   487177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap
+-rw-r--r--   0     1001      127    19608 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap
+-rw-r--r--   0     1001      127    40002 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap
+-rw-r--r--   0     1001      127    52187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap
+-rw-r--r--   0     1001      127  1811359 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap
+-rw-r--r--   0     1001      127    10278 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v5__flat-index-lock.yml.snap
+-rw-r--r--   0     1001      127   242145 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v6__always-record-purls.yml.snap
+-rw-r--r--   0     1001      127     6457 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/url_or_path.rs
+-rw-r--r--   0     1001      127       22 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1693 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs
+-rw-r--r--   0     1001      127      372 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/mod.rs
+-rw-r--r--   0     1001      127     2012 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs
+-rw-r--r--   0     1001      127     1571 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs
+-rw-r--r--   0     1001      127     7945 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs
+-rw-r--r--   0     1001      127     1441 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs
+-rw-r--r--   0     1001      127     1407 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/Cargo.toml
+-rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/src/lib.rs
+-rw-r--r--   0     1001      127      692 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/simple_spawn_blocking/src/tokio.rs
+-rw-r--r--   0        0        0     3149 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/Cargo.toml
+-rw-r--r--   0     1001      127     4303 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md
+-rw-r--r--   0     1001      127     2806 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs
+-rw-r--r--   0     1001      127     7713 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs
+-rw-r--r--   0     1001      127      956 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap
+-rw-r--r--   0     1001      127      465 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_one.snap
+-rw-r--r--   0     1001      127      604 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap
+-rw-r--r--   0     1001      127    38981 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs
+-rw-r--r--   0     1001      127    52612 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs
+-rw-r--r--   0     1001      127     3926 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/barrier_cell.rs
+-rw-r--r--   0     1001      127     3219 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/builder.rs
+-rw-r--r--   0     1001      127     1738 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/channel_config.rs
+-rw-r--r--   0     1001      127     2627 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/error.rs
+-rw-r--r--   0     1001      127     2335 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/local_subdir.rs
+-rw-r--r--   0     1001      127    18116 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/mod.rs
+-rw-r--r--   0     1001      127     8435 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/query.rs
+-rw-r--r--   0     1001      127     2409 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/remote_subdir.rs
+-rw-r--r--   0     1001      127     2377 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/repo_data.rs
+-rw-r--r--   0     1001      127    13060 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/index.rs
+-rw-r--r--   0     1001      127     8026 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/mod.rs
+-rw-r--r--   0     1001      127     5798 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/sharded_subdir/token.rs
+-rw-r--r--   0     1001      127     6178 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/gateway/subdir.rs
+-rw-r--r--   0     1001      127     2151 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/lib.rs
+-rw-r--r--   0     1001      127     3977 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/reporter.rs
+-rw-r--r--   0     1001      127    22540 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs
+-rw-r--r--   0     1001      127     2167 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/body.rs
+-rw-r--r--   0     1001      127     2718 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs
+-rw-r--r--   0     1001      127    13393 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs
+-rw-r--r--   0     1001      127     1715 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/Cargo.toml
+-rw-r--r--   0     1001      127      987 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/CHANGELOG.md
+-rw-r--r--   0     1001      127     2664 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/src/lib.rs
+-rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/01-sorted-enum.rs
+-rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/02-sorted-struct.rs
+-rw-r--r--   0     1001      127      113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.rs
+-rw-r--r--   0     1001      127      127 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/03-out-of-order-enum.stderr
+-rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.rs
+-rw-r--r--   0     1001      127      137 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/04-out-of-order-struct.stderr
+-rw-r--r--   0     1001      127      251 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_macros/tests/tests.rs
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/Cargo.toml
+-rw-r--r--   0     1001      127     3232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md
+-rw-r--r--   0     1001      127    11042 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/cuda.rs
+-rw-r--r--   0     1001      127    12929 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/lib.rs
+-rw-r--r--   0     1001      127     3047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/libc.rs
+-rw-r--r--   0     1001      127     3969 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/linux.rs
+-rw-r--r--   0     1001      127     2381 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/osx.rs
+-rw-r--r--   0        0        0      412 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/file_url/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/.gitignore
+-rw-r--r--   0     1001      127      486 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/CHANGELOG.md
+-rw-r--r--   0     1001      127     7791 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/file_url/src/lib.rs
+-rw-r--r--   0        0        0     2507 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler/Cargo.toml
+-rw-r--r--   0     1001      127        8 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/.gitignore
+-rw-r--r--   0     1001      127     5482 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/CHANGELOG.md
+-rw-r--r--   0     1001      127    74752 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/resources/launcher64.exe
+-rw-r--r--   0     1001      127    99068 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/resources/versions.txt
+-rw-r--r--   0     1001      127     4794 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/cli/auth.rs
+-rw-r--r--   0     1001      127      122 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/cli/mod.rs
+-rw-r--r--   0     1001      127     1358 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/apple_codesign.rs
+-rw-r--r--   0     1001      127    35510 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/clobber_registry.rs
+-rw-r--r--   0     1001      127     9786 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/driver.rs
+-rw-r--r--   0     1001      127     8511 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/entry_point.rs
+-rw-r--r--   0     1001      127     1666 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/error.rs
+-rw-r--r--   0     1001      127    27383 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/indicatif.rs
+-rw-r--r--   0     1001      127    20030 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/mod.rs
+-rw-r--r--   0     1001      127     4261 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/installer/reporter.rs
+-rw-r--r--   0     1001      127    33225 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/link.rs
+-rw-r--r--   0     1001      127     9691 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/link_script.rs
+-rw-r--r--   0     1001      127    33679 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/mod.rs
+-rw-r--r--   0     1001      127     3839 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/python.rs
+-rw-r--r--   0     1001      127      609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap
+-rw-r--r--   0     1001      127      190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-3.snap
+-rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap
+-rw-r--r--   0     1001      127      142 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-5.snap
+-rw-r--r--   0     1001      127      609 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap
+-rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap
+-rw-r--r--   0     1001      127      142 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber.snap
+-rw-r--r--   0     1001      127      297 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__entry_point_script.snap
+-rw-r--r--   0     1001      127      271 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__entry_point__test__windows.snap
+-rw-r--r--   0     1001      127      155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__link__test__replace_long_prefix_in_text_file.snap
+-rw-r--r--   0     1001      127     3732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap
+-rw-r--r--   0     1001      127     4688 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/test_utils.rs
+-rw-r--r--   0     1001      127     8426 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/transaction.rs
+-rw-r--r--   0     1001      127     9414 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/install/unlink.rs
+-rw-r--r--   0     1001      127     2983 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/lib.rs
+-rw-r--r--   0     1001      127    22292 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/package_cache.rs
+-rw-r--r--   0     1001      127    24363 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/range.rs
+-rw-r--r--   0     1001      127    13775 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler/src/validation.rs
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_index/Cargo.toml
+-rw-r--r--   0     1001      127     3314 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/CHANGELOG.md
+-rw-r--r--   0     1001      127     6961 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/src/lib.rs
+-rw-r--r--   0     1001      127     2162 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_index/tests/test_index.rs
+-rw-r--r--   0        0        0     1202 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/Cargo.toml
+-rw-r--r--   0     1001      127     4099 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/CHANGELOG.md
+-rw-r--r--   0     1001      127     2914 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/benches/bench.rs
+-rw-r--r--   0     1001      127     8454 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/lib.rs
+-rw-r--r--   0     1001      127    13226 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs
+-rw-r--r--   0     1001      127     1173 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs
+-rw-r--r--   0     1001      127     9630 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs
+-rw-r--r--   0     1001      127     2444 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs
+-rw-r--r--   0     1001      127      561 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs
+-rw-r--r--   0     1001      127      864 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs
+-rw-r--r--   0     1001      127     1047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs
+-rw-r--r--   0     1001      127    11669 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs
+-rw-r--r--   0     1001      127     2720 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs
+-rw-r--r--   0     1001      127     6299 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs
+-rw-r--r--   0     1001      127     3402 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs
+-rw-r--r--   0     1001      127     1262 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs
+-rw-r--r--   0     1001      127     3451 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs
+-rw-r--r--   0     1001      127     4718 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs
+-rw-r--r--   0     1001      127     5589 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs
+-rw-r--r--   0     1001      127     2468 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs
+-rw-r--r--   0     1001      127     7734 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs
+-rw-r--r--   0     1001      127    24305 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/mod.rs
+-rw-r--r--   0     1001      127    33981 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/backends.rs
+-rw-r--r--   0     1001      127      165 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      738 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap
+-rw-r--r--   0     1001      127     1105 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3069 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap
+-rw-r--r--   0     1001      127     2590 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3631 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      216 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_with_error.snap
+-rw-r--r--   0     1001      127      411 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_xtensor_xsimd.snap
+-rw-r--r--   0     1001      127      369 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__exclude_newer_error.snap
+-rw-r--r--   0     1001      127      172 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_dummy_repo_install_non_existent.snap
+-rw-r--r--   0     1001      127      412 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_locked.snap
+-rw-r--r--   0     1001      127      736 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap
+-rw-r--r--   0     1001      127     1103 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap
+-rw-r--r--   0     1001      127     3067 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap
+-rw-r--r--   0     1001      127     2588 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap
+-rw-r--r--   0     1001      127     3629 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap
+-rw-r--r--   0     1001      127      588 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap
+-rw-r--r--   0     1001      127      400 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_xtensor_xsimd.snap
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/Cargo.toml
+-rw-r--r--   0     1001      127     1233 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/CHANGELOG.md
+-rw-r--r--   0     1001      127     7607 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/lib.rs
+-rw-r--r--   0     1001      127     4014 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/serde.rs
+-rw-r--r--   0     1001      127     2155 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_digest/src/tokio.rs
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/Cargo.toml
+-rw-r--r--   0     1001      127     3627 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/CHANGELOG.md
+-rw-r--r--   0     1001      127    14736 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_middleware.rs
+-rw-r--r--   0     1001      127     1266 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs
+-rw-r--r--   0     1001      127     6690 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs
+-rw-r--r--   0     1001      127     2852 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs
+-rw-r--r--   0     1001      127      103 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/mod.rs
+-rw-r--r--   0     1001      127     5769 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs
+-rw-r--r--   0     1001      127      270 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/snapshots/rattler_networking__authentication_storage__backends__file__tests__file_storage.snap
+-rw-r--r--   0     1001      127      727 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs
+-rw-r--r--   0     1001      127     6830 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs
+-rw-r--r--   0     1001      127     2287 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/gcs_middleware.rs
+-rw-r--r--   0     1001      127      726 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/lib.rs
+-rw-r--r--   0     1001      127    10298 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/mirror_middleware.rs
+-rw-r--r--   0     1001      127    10902 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/oci_middleware.rs
+-rw-r--r--   0     1001      127     3489 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/redaction.rs
+-rw-r--r--   0     1001      127      920 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_networking/src/retry_policies.rs
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/Cargo.toml
+-rw-r--r--   0     1001      127     4351 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/CHANGELOG.md
+-rw-r--r--   0     1001      127     1016 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/benches/parse.rs
+-rw-r--r--   0     1001      127     3220 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs
+-rw-r--r--   0     1001      127     6519 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs
+-rw-r--r--   0     1001      127    23177 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel/mod.rs
+-rw-r--r--   0     1001      127     4187 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel_data.rs
+-rw-r--r--   0     1001      127    11580 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs
+-rw-r--r--   0     1001      127      770 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127     2279 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/lib.rs
+-rw-r--r--   0     1001      127     6012 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs
+-rw-r--r--   0     1001      127    20372 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs
+-rw-r--r--   0     1001      127    28532 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs
+-rw-r--r--   0     1001      127      506 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__parse__tests__parsed matchspecs.snap
+-rw-r--r--   0     1001      127      537 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap
+-rw-r--r--   0     1001      127     5728 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     3206 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/about.rs
+-rw-r--r--   0     1001      127     4183 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs
+-rw-r--r--   0     1001      127     1400 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs
+-rw-r--r--   0     1001      127     3244 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs
+-rw-r--r--   0     1001      127     1348 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/files.rs
+-rw-r--r--   0     1001      127     6460 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs
+-rw-r--r--   0     1001      127     3942 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/index.rs
+-rw-r--r--   0     1001      127     1977 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/link.rs
+-rw-r--r--   0     1001      127     3607 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/mod.rs
+-rw-r--r--   0     1001      127     1510 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_link.rs
+-rw-r--r--   0     1001      127     1495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs
+-rw-r--r--   0     1001      127      507 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/package_metadata.rs
+-rw-r--r--   0     1001      127    12387 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/paths.rs
+-rw-r--r--   0     1001      127     2334 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs
+-rw-r--r--   0     1001      127      754 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap
+-rw-r--r--   0     1001      127     2515 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap
+-rw-r--r--   0     1001      127      134 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__entry_point__test__entry_point.snap
+-rw-r--r--   0     1001      127      329 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json.snap
+-rw-r--r--   0     1001      127      309 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__index__test__reconstruct_index_json_with_symlinks.snap
+-rw-r--r--   0     1001      127      349 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__jupyterlab-link.json.snap
+-rw-r--r--   0     1001      127      137 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__setuptools-link.json.snap
+-rw-r--r--   0     1001      127      138 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__link__test__link-json__tzdata-link.json.snap
+-rw-r--r--   0     1001      127     1171 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap
+-rw-r--r--   0     1001      127      776 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap
+-rw-r--r--   0     1001      127      601 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     6782 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap
+-rw-r--r--   0     1001      127      185 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__run_exports__test__reconstruct_run_exports_json_with_symlinks.snap
+-rw-r--r--   0     1001      127     5305 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package_name.rs
+-rw-r--r--   0     1001      127      233 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/parse_mode.rs
+-rw-r--r--   0     1001      127    15923 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/platform.rs
+-rw-r--r--   0     1001      127    12758 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/prefix_record.rs
+-rw-r--r--   0     1001      127    19998 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127    11158 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs
+-rw-r--r--   0     1001      127     1554 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/sharded.rs
+-rw-r--r--   0     1001      127      181 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__null_values.snap
+-rw-r--r--   0     1001      127     2154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap
+-rw-r--r--   0     1001      127     2091 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap
+-rw-r--r--   0     1001      127      843 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap
+-rw-r--r--   0     1001      127     1595 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap
+-rw-r--r--   0     1001      127      873 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap
+-rw-r--r--   0     1001      127     4832 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap
+-rw-r--r--   0     1001      127      232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize.snap
+-rw-r--r--   0     1001      127     6461 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap
+-rw-r--r--   0     1001      127     5154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap
+-rw-r--r--   0     1001      127    77589 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs
+-rw-r--r--   0     1001      127     1063 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs
+-rw-r--r--   0     1001      127      455 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/run_export.rs
+-rw-r--r--   0     1001      127    53039 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap
+-rw-r--r--   0     1001      127      353 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__vs2015_runtime_win-64.txt.snap
+-rw-r--r--   0     1001      127      974 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap
+-rw-r--r--   0     1001      127     2269 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap
+-rw-r--r--   0     1001      127    12047 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap
+-rw-r--r--   0     1001      127   269415 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     4590 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap
+-rw-r--r--   0     1001      127    12519 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127   345345 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap
+-rw-r--r--   0     1001      127    23076 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     1054 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap
+-rw-r--r--   0     1001      127    12151 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap
+-rw-r--r--   0     1001      127     7102 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap
+-rw-r--r--   0     1001      127       22 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/mod.rs
+-rw-r--r--   0     1001      127     6107 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/serde.rs
+-rw-r--r--   0     1001      127     1531 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/bump.rs
+-rw-r--r--   0     1001      127     3760 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/flags.rs
+-rw-r--r--   0     1001      127    53146 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/mod.rs
+-rw-r--r--   0     1001      127    18817 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/parse.rs
+-rw-r--r--   0     1001      127     6410 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/segment.rs
+-rw-r--r--   0     1001      127     2495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap
+-rw-r--r--   0     1001      127     4817 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/with_source.rs
+-rw-r--r--   0     1001      127    10418 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs
+-rw-r--r--   0     1001      127    18331 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs
+-rw-r--r--   0     1001      127    16688 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs
+-rw-r--r--   0     1001      127    14591 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/Cargo.toml
+-rw-r--r--   0     1001      127     3029 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/CHANGELOG.md
+-rw-r--r--   0     1001      127    27911 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/activation.rs
+-rw-r--r--   0     1001      127      196 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/lib.rs
+-rw-r--r--   0     1001      127     2232 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/run/mod.rs
+-rw-r--r--   0     1001      127    28467 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/mod.rs
+-rw-r--r--   0     1001      127      123 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__bash.snap
+-rw-r--r--   0     1001      127      128 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__fish.snap
+-rw-r--r--   0     1001      127      104 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_bash.snap
+-rw-r--r--   0     1001      127      122 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/snapshots/rattler_shell__shell__tests__xonsh_xsh.snap
+-rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_bash.snap
+-rw-r--r--   0     1001      127      185 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_cmd.snap
+-rw-r--r--   0     1001      127      190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_fish.snap
+-rw-r--r--   0     1001      127      192 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_powershell.snap
+-rw-r--r--   0     1001      127      239 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_xonsh.snap
+-rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__activation_script_zsh.snap
+-rw-r--r--   0     1001      127      171 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__after_activation.snap
+-rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_append.snap
+-rw-r--r--   0     1001      127      237 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_prepend.snap
+-rw-r--r--   0     1001      127      229 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_bash_replace.snap
+-rw-r--r--   0     1001      127      202 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_append.snap
+-rw-r--r--   0     1001      127      202 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_prepend.snap
+-rw-r--r--   0     1001      127      195 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_cmd_replace.snap
+-rw-r--r--   0     1001      127      311 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_append.snap
+-rw-r--r--   0     1001      127      311 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_prepend.snap
+-rw-r--r--   0     1001      127      301 2024-05-27 12:39:44.000000 py_rattler-0.6.0/local_dependencies/rattler_shell/src/snapshots/rattler_shell__activation__tests__test_activation_script_powershell_replace.snap
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 py_rattler-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      127      743 2024-05-27 12:39:44.000000 py_rattler-0.6.0/.gitignore
+-rw-r--r--   0     1001      127     1502 2024-05-27 12:39:44.000000 py_rattler-0.6.0/LICENSE
+-rw-r--r--   0     1001      127     6880 2024-05-27 12:39:44.000000 py_rattler-0.6.0/README.md
+-rw-r--r--   0     1001      127       71 2024-05-27 12:39:44.000000 py_rattler-0.6.0/build.rs
+-rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/about_json.md
+-rw-r--r--   0     1001      127       45 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activate.md
+-rw-r--r--   0     1001      127       58 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_error.md
+-rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_result.md
+-rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/activation_variables.md
+-rw-r--r--   0     1001      127       34 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/arch.md
+-rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/authenticated_client.md
+-rw-r--r--   0     1001      127       54 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/cache_dir_error.md
+-rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/channel.md
+-rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/channel_config.md
+-rw-r--r--   0     1001      127       79 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/detect_virtual_package_error.md
+-rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/environment.md
+-rw-r--r--   0     1001      127       76 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/environment_creation_error.md
+-rw-r--r--   0     1001      127       58 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/fetch_repo_data.md
+-rw-r--r--   0     1001      127       65 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/fetch_repo_data_error.md
+-rw-r--r--   0     1001      127       51 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/file_mode.md
+-rw-r--r--   0     1001      127       41 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/gateway.md
+-rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/generic_virtual_package.md
+-rw-r--r--   0     1001      127     5592 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/index.md
+-rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/index_json.md
+-rw-r--r--   0     1001      127       41 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/installer.md
+-rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_channel_error.md
+-rw-r--r--   0     1001      127       71 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_match_spec_error.md
+-rw-r--r--   0     1001      127       75 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_package_name_error.md
+-rw-r--r--   0     1001      127       59 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_url_error.md
+-rw-r--r--   0     1001      127       67 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/invalid_version_error.md
+-rw-r--r--   0     1001      127       43 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/io_error.md
+-rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/link_error.md
+-rw-r--r--   0     1001      127       38 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/lock_file.md
+-rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/locked_package.md
+-rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/match_spec.md
+-rw-r--r--   0     1001      127       64 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/nameless_match_spec.md
+-rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_hashes.md
+-rw-r--r--   0     1001      127       48 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_name.md
+-rw-r--r--   0     1001      127       54 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/package_record.md
+-rw-r--r--   0     1001      127       57 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/parse_arch_error.md
+-rw-r--r--   0     1001      127       65 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/parse_platform_error.md
+-rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/patch_instructions.md
+-rw-r--r--   0     1001      127       77 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/path_modification_behavior.md
+-rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/path_type.md
+-rw-r--r--   0     1001      127       56 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/paths_entry.md
+-rw-r--r--   0     1001      127       55 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/paths_json.md
+-rw-r--r--   0     1001      127       42 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/platform.md
+-rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_paths.md
+-rw-r--r--   0     1001      127       69 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_placeholder.md
+-rw-r--r--   0     1001      127       49 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/prefix_record.md
+-rw-r--r--   0     1001      127       52 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/pypi_package_data.md
+-rw-r--r--   0     1001      127       74 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/pypi_package_environment_data.md
+-rw-r--r--   0     1001      127       44 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/repo_data.md
+-rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/repo_data_record.md
+-rw-r--r--   0     1001      127       56 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/run_exports_json.md
+-rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/shell.md
+-rw-r--r--   0     1001      127       35 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/solver.md
+-rw-r--r--   0     1001      127       51 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/solver_error.md
+-rw-r--r--   0     1001      127       47 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/sparse_repo_data.md
+-rw-r--r--   0     1001      127     2082 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/stylesheets/extra.css
+-rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/transaction_error.md
+-rw-r--r--   0     1001      127       39 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/version.md
+-rw-r--r--   0     1001      127       53 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/version_with_source.md
+-rw-r--r--   0     1001      127       62 2024-05-27 12:39:44.000000 py_rattler-0.6.0/docs/virtual_package.md
+-rw-r--r--   0     1001      127     5280 2024-05-27 12:39:44.000000 py_rattler-0.6.0/mkdocs.yml
+-rw-r--r--   0     1001      127   210327 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pixi.lock
+-rw-r--r--   0     1001      127     1898 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pixi.toml
+-rw-r--r--   0     1001      127     1863 2024-05-27 12:39:44.000000 py_rattler-0.6.0/pyproject.toml
+-rw-r--r--   0     1001      127     2070 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/__init__.py
+-rw-r--r--   0     1001      127      221 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/__init__.py
+-rw-r--r--   0     1001      127     2295 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel.py
+-rw-r--r--   0     1001      127     1532 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel_config.py
+-rw-r--r--   0     1001      127      474 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/channel/channel_priority.py
+-rw-r--r--   0     1001      127     3842 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/exceptions.py
+-rw-r--r--   0     1001      127       59 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/index/__init__.py
+-rw-r--r--   0     1001      127     1133 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/index/index.py
+-rw-r--r--   0     1001      127       69 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/install/__init__.py
+-rw-r--r--   0     1001      127     3150 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/install/installer.py
+-rw-r--r--   0     1001      127      471 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/__init__.py
+-rw-r--r--   0     1001      127     1277 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/channel.py
+-rw-r--r--   0     1001      127     7624 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/environment.py
+-rw-r--r--   0     1001      127      805 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/hash.py
+-rw-r--r--   0     1001      127     3264 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/lock_file.py
+-rw-r--r--   0     1001      127     5336 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/package.py
+-rw-r--r--   0     1001      127     6544 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/lock/pypi.py
+-rw-r--r--   0     1001      127      167 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/__init__.py
+-rw-r--r--   0     1001      127     7953 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/match_spec.py
+-rw-r--r--   0     1001      127     4293 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/match_spec/nameless_match_spec.py
+-rw-r--r--   0     1001      127      189 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/__init__.py
+-rw-r--r--   0     1001      127      915 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/authenticated_client.py
+-rw-r--r--   0     1001      127     1393 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/networking/fetch_repo_data.py
+-rw-r--r--   0     1001      127      518 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/__init__.py
+-rw-r--r--   0     1001      127     7060 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/about_json.py
+-rw-r--r--   0     1001      127     9422 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/index_json.py
+-rw-r--r--   0     1001      127     3672 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/no_arch_type.py
+-rw-r--r--   0     1001      127     4111 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/package_name.py
+-rw-r--r--   0     1001      127    15226 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/paths_json.py
+-rw-r--r--   0     1001      127     6238 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/package/run_exports_json.py
+-rw-r--r--   0     1001      127      154 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/__init__.py
+-rw-r--r--   0     1001      127     1145 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/arch.py
+-rw-r--r--   0     1001      127     3993 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/platform/platform.py
+-rw-r--r--   0     1001      127      221 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/__init__.py
+-rw-r--r--   0     1001      127     8542 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/prefix_paths.py
+-rw-r--r--   0     1001      127     4514 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/prefix/prefix_record.py
+-rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/py.typed
+-rw-r--r--   0     1001      127      495 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/__init__.py
+-rw-r--r--   0     1001      127     8268 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/gateway.py
+-rw-r--r--   0     1001      127    13342 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/package_record.py
+-rw-r--r--   0     1001      127      694 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/patch_instructions.py
+-rw-r--r--   0     1001      127     2660 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/record.py
+-rw-r--r--   0     1001      127     2264 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/repo_data.py
+-rw-r--r--   0     1001      127     6245 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/repo_data/sparse.py
+-rw-r--r--   0     1001      127      179 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/shell/__init__.py
+-rw-r--r--   0     1001      127     4442 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/shell/shell.py
+-rw-r--r--   0     1001      127       61 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/solver/__init__.py
+-rw-r--r--   0     1001      127     5197 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/solver/solver.py
+-rw-r--r--   0     1001      127      526 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/utils/rattler_version.py
+-rw-r--r--   0     1001      127      146 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/__init__.py
+-rw-r--r--   0     1001      127    14467 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/version.py
+-rw-r--r--   0     1001      127     2539 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/version/with_source.py
+-rw-r--r--   0     1001      127      188 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/__init__.py
+-rw-r--r--   0     1001      127     4411 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/generic.py
+-rw-r--r--   0     1001      127     1509 2024-05-27 12:39:44.000000 py_rattler-0.6.0/rattler/virtual_package/virtual_package.py
+-rw-r--r--   0     1001      127     4356 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/about_json.rs
+-rw-r--r--   0     1001      127     2929 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/channel/mod.rs
+-rw-r--r--   0     1001      127     7910 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/error.rs
+-rw-r--r--   0     1001      127     1743 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/generic_virtual_package.rs
+-rw-r--r--   0     1001      127      593 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/index.rs
+-rw-r--r--   0     1001      127     5113 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/index_json.rs
+-rw-r--r--   0     1001      127     2334 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/installer.rs
+-rw-r--r--   0     1001      127     6766 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      127    15021 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/lock/mod.rs
+-rw-r--r--   0     1001      127     3683 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/match_spec.rs
+-rw-r--r--   0     1001      127      147 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/meta.rs
+-rw-r--r--   0     1001      127     3550 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/nameless_match_spec.rs
+-rw-r--r--   0     1001      127     1017 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/authenticated_client.rs
+-rw-r--r--   0     1001      127      804 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/cached_repo_data.rs
+-rw-r--r--   0     1001      127     3328 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/networking/mod.rs
+-rw-r--r--   0     1001      127     1619 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/no_arch_type.rs
+-rw-r--r--   0     1001      127     2124 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/package_name.rs
+-rw-r--r--   0     1001      127     9546 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/paths_json.rs
+-rw-r--r--   0     1001      127     2521 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/platform.rs
+-rw-r--r--   0     1001      127     5691 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/prefix_paths.rs
+-rw-r--r--   0     1001      127    13360 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/record.rs
+-rw-r--r--   0     1001      127     4735 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/gateway.rs
+-rw-r--r--   0     1001      127     1672 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/mod.rs
+-rw-r--r--   0     1001      127      189 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/patch_instructions.rs
+-rw-r--r--   0     1001      127     2096 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/repo_data/sparse.rs
+-rw-r--r--   0     1001      127     4469 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/run_exports_json.rs
+-rw-r--r--   0     1001      127     3878 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/shell.rs
+-rw-r--r--   0     1001      127     3842 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/solver.rs
+-rw-r--r--   0     1001      127      814 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/version/component.rs
+-rw-r--r--   0     1001      127     5550 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/version/mod.rs
+-rw-r--r--   0     1001      127     1190 2024-05-27 12:39:44.000000 py_rattler-0.6.0/src/virtual_package.rs
+-rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/__init__.py
+-rw-r--r--   0     1001      127      696 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/__init__.py
+-rw-r--r--   0     1001      127     2129 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_fetch_repo_data.py
+-rw-r--r--   0     1001      127     2159 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_index.py
+-rw-r--r--   0     1001      127      730 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_install.py
+-rw-r--r--   0     1001      127     1732 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_prefix_record.py
+-rw-r--r--   0     1001      127     3531 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_solver.py
+-rw-r--r--   0     1001      127      892 2024-05-27 12:39:44.000000 py_rattler-0.6.0/tests/unit/test_version.py
+-rw-r--r--   0     1001      127   109244 2024-05-27 12:39:44.000000 py_rattler-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     7866 1970-01-01 00:00:00.000000 py_rattler-0.6.0/PKG-INFO
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_digest/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_digest/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rattler_digest"
-version = "0.19.3"
+version = "0.19.4"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "An simple crate used by rattler crates to compute different hashes from different sources"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
@@ -16,11 +16,12 @@
 digest = "0.10.7"
 hex = "0.4.3"
 md-5 = "0.10.6"
 serde = { version = "1.0.198" , optional = true , features = ["derive"] }
 serde_with = "3.7.0"
 sha2 = "0.10.8"
 tokio = { version = "1.37.0", default-features = false , optional = true , features = ["io-util"] }
+generic-array = "0.14.4"
 
 [features]
 tokio = ["dep:tokio"]
-serde = ["dep:serde"]
+serde = ["dep:serde", "generic-array/serde"]
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_digest/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_digest/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.4](https://github.com/mamba-org/rattler/compare/rattler_digest-v0.19.3...rattler_digest-v0.19.4) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Other
+- update README.md
+
 ## [0.19.3](https://github.com/mamba-org/rattler/compare/rattler_digest-v0.19.2...rattler_digest-v0.19.3) - 2024-04-19
 
 ### Other
 - update Cargo.toml dependencies
 
 ## [0.19.2](https://github.com/mamba-org/rattler/compare/rattler_digest-v0.19.1...rattler_digest-v0.19.2) - 2024-03-14
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_digest/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_digest/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_digest/src/serde.rs` & `py_rattler-0.6.0/local_dependencies/rattler_digest/src/serde.rs`

 * *Files 12% similar despite different names*

```diff
@@ -18,33 +18,47 @@
 use serde::de::Error;
 use serde::{Deserialize, Deserializer, Serialize, Serializer};
 use serde_with::{DeserializeAs, SerializeAs};
 use std::borrow::Cow;
 use std::fmt::LowerHex;
 use std::ops::Deref;
 
-/// Deserialize into [`Output`] of a [`Digest`]
+/// Deserialize the [`Output`] of a [`Digest`].
+///
+/// If the deserializer is human-readable, it will parse the digest from a hex
+/// string. Otherwise, it will deserialize raw bytes.
 pub fn deserialize<'de, D, Dig: Digest>(deserializer: D) -> Result<Output<Dig>, D::Error>
 where
     D: Deserializer<'de>,
 {
-    let str = Cow::<'de, str>::deserialize(deserializer)?;
-    super::parse_digest_from_hex::<Dig>(str.as_ref())
-        .ok_or_else(|| Error::custom("failed to parse digest"))
+    if deserializer.is_human_readable() {
+        let str = Cow::<'de, str>::deserialize(deserializer)?;
+        super::parse_digest_from_hex::<Dig>(str.as_ref())
+            .ok_or_else(|| Error::custom("failed to parse digest"))
+    } else {
+        Output::<Dig>::deserialize(deserializer)
+    }
 }
 
-/// Serialize into a string
+/// Serializes the [`Output`] of a [`Digest`].
+///
+/// If the serializer is human-readable, it will write the digest as a hex
+/// string. Otherwise, it will deserialize raw bytes.
 pub fn serialize<'a, S: Serializer, Dig: Digest>(
     digest: &'a Output<Dig>,
     s: S,
 ) -> Result<S::Ok, S::Error>
 where
     &'a Output<Dig>: LowerHex,
 {
-    format!("{digest:x}").serialize(s)
+    if s.is_human_readable() {
+        format!("{digest:x}").serialize(s)
+    } else {
+        digest.serialize(s)
+    }
 }
 
 /// Wrapper type for easily serializing a Hash
 pub struct SerializableHash<T: Digest>(pub Output<T>);
 
 impl<T: Digest> Serialize for SerializableHash<T>
 where
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_digest/src/tokio.rs` & `py_rattler-0.6.0/local_dependencies/rattler_digest/src/tokio.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "rattler_package_streaming"
-version = "0.20.6"
+version = "0.21.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Extract and stream of Conda package archives"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false }
-rattler_networking = { path= "../rattler_networking", version = "0.20.3", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
+rattler_networking = { path= "../rattler_networking", version = "0.20.8", default-features = false }
 bzip2 = "0.4.4"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 futures-util = "0.3.30"
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,45 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.10...rattler_package_streaming-v0.21.0) - 2024-05-27
+
+### Other
+- introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
+
+## [0.20.10](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.9...rattler_package_streaming-v0.20.10) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.20.9](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.8...rattler_package_streaming-v0.20.9) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Fixed
+- set last modified for zip archive ([#649](https://github.com/mamba-org/rattler/pull/649))
+
+### Other
+- update README.md
+
+## [0.20.8](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.7...rattler_package_streaming-v0.20.8) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_networking
+
+## [0.20.7](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.6...rattler_package_streaming-v0.20.7) - 2024-04-30
+
+### Other
+- updated the following local packages: rattler_networking
+
 ## [0.20.6](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.5...rattler_package_streaming-v0.20.6) - 2024-04-25
 
 ### Other
 - updated the following local packages: rattler_networking
 
 ## [0.20.5](https://github.com/mamba-org/rattler/compare/rattler_package_streaming-v0.20.4...rattler_package_streaming-v0.20.5) - 2024-04-25
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/fs.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/lib.rs`

 * *Files 21% similar despite different names*

```diff
@@ -74,7 +74,17 @@
 pub struct ExtractResult {
     /// The SHA256 hash of the extracted archive.
     pub sha256: Sha256Hash,
 
     /// The Md5 hash of the extracted archive.
     pub md5: Md5Hash,
 }
+
+/// A trait that can be implemented to report download progress.
+pub trait DownloadReporter: Send + Sync {
+    /// Called when the download starts.
+    fn on_download_start(&self);
+    /// Called when the download makes progress.
+    fn on_download_progress(&self, bytes_downloaded: u64, total_bytes: Option<u64>);
+    /// Called when the download finishes.
+    fn on_download_complete(&self);
+}
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/read.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/reqwest/tokio.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 //! Functionality to stream and extract packages directly from a [`reqwest::Url`] within a [`tokio`]
 //! async context.
 
-use crate::{ExtractError, ExtractResult};
+use crate::{DownloadReporter, ExtractError, ExtractResult};
 use futures_util::stream::TryStreamExt;
 use rattler_conda_types::package::ArchiveType;
 use rattler_digest::Sha256Hash;
 use reqwest::Response;
 use std::path::Path;
+use std::sync::Arc;
 use tokio::io::BufReader;
 use tokio_util::either::Either;
 use tokio_util::io::StreamReader;
 use url::Url;
 
 fn error_for_status(response: reqwest::Response) -> reqwest_middleware::Result<Response> {
     response
@@ -18,14 +19,15 @@
         .map_err(reqwest_middleware::Error::Reqwest)
 }
 
 async fn get_reader(
     url: Url,
     client: reqwest_middleware::ClientWithMiddleware,
     expected_sha256: Option<Sha256Hash>,
+    reporter: Option<Arc<dyn DownloadReporter>>,
 ) -> Result<impl tokio::io::AsyncRead, ExtractError> {
     if url.scheme() == "file" {
         let file =
             tokio::fs::File::open(url.to_file_path().expect("Could not convert to file path"))
                 .await
                 .map_err(ExtractError::IoError)?;
 
@@ -35,26 +37,37 @@
         let mut request = client.get(url.clone());
 
         if let Some(sha256) = expected_sha256 {
             // This is used by the OCI registry middleware to verify the sha256 of the response
             request = request.header("X-Expected-Sha256", format!("{sha256:x}"));
         }
 
+        if let Some(reporter) = &reporter {
+            reporter.on_download_start();
+        }
+
         let response = request
             .send()
             .await
             .and_then(error_for_status)
             .map_err(ExtractError::ReqwestError)?;
 
+        let total_bytes = response.content_length();
+        let mut bytes_received = Box::new(0);
+        let byte_stream = response.bytes_stream().inspect_ok(move |frame| {
+            *bytes_received += frame.len() as u64;
+            if let Some(reporter) = &reporter {
+                reporter.on_download_progress(*bytes_received, total_bytes);
+            }
+        });
+
         // Get the response as a stream
-        Ok(Either::Right(StreamReader::new(
-            response
-                .bytes_stream()
-                .map_err(|err| std::io::Error::new(std::io::ErrorKind::Other, err)),
-        )))
+        Ok(Either::Right(StreamReader::new(byte_stream.map_err(
+            |err| std::io::Error::new(std::io::ErrorKind::Other, err),
+        ))))
     }
 }
 
 /// Extracts the contents a `.tar.bz2` package archive from the specified remote location.
 ///
 /// ```rust,no_run
 /// # #[tokio::main]
@@ -64,28 +77,34 @@
 /// use reqwest::Client;
 /// use reqwest_middleware::ClientWithMiddleware;
 /// use rattler_package_streaming::reqwest::tokio::extract_tar_bz2;
 /// let _ = extract_tar_bz2(
 ///     ClientWithMiddleware::from(Client::new()),
 ///     Url::parse("https://conda.anaconda.org/conda-forge/win-64/python-3.11.0-hcf16a7b_0_cpython.tar.bz2").unwrap(),
 ///     Path::new("/tmp"),
+///     None,
 ///     None)
 ///     .await
 ///     .unwrap();
 /// # }
 /// ```
 pub async fn extract_tar_bz2(
     client: reqwest_middleware::ClientWithMiddleware,
     url: Url,
     destination: &Path,
     expected_sha256: Option<Sha256Hash>,
+    reporter: Option<Arc<dyn DownloadReporter>>,
 ) -> Result<ExtractResult, ExtractError> {
-    let reader = get_reader(url.clone(), client, expected_sha256).await?;
+    let reader = get_reader(url.clone(), client, expected_sha256, reporter.clone()).await?;
     // The `response` is used to stream in the package data
-    crate::tokio::async_read::extract_tar_bz2(reader, destination).await
+    let result = crate::tokio::async_read::extract_tar_bz2(reader, destination).await?;
+    if let Some(reporter) = &reporter {
+        reporter.on_download_complete();
+    }
+    Ok(result)
 }
 
 /// Extracts the contents a `.conda` package archive from the specified remote location.
 ///
 /// ```rust,no_run
 /// # #[tokio::main]
 /// # async fn main() {
@@ -94,28 +113,34 @@
 /// use reqwest::Client;
 /// use reqwest_middleware::ClientWithMiddleware;
 /// use url::Url;
 /// let _ = extract_conda(
 ///     ClientWithMiddleware::from(Client::new()),
 ///     Url::parse("https://conda.anaconda.org/conda-forge/linux-64/python-3.10.8-h4a9ceb5_0_cpython.conda").unwrap(),
 ///     Path::new("/tmp"),
+///     None,
 ///     None)
 ///     .await
 ///     .unwrap();
 /// # }
 /// ```
 pub async fn extract_conda(
     client: reqwest_middleware::ClientWithMiddleware,
     url: Url,
     destination: &Path,
     expected_sha256: Option<Sha256Hash>,
+    reporter: Option<Arc<dyn DownloadReporter>>,
 ) -> Result<ExtractResult, ExtractError> {
     // The `response` is used to stream in the package data
-    let reader = get_reader(url.clone(), client, expected_sha256).await?;
-    crate::tokio::async_read::extract_conda(reader, destination).await
+    let reader = get_reader(url.clone(), client, expected_sha256, reporter.clone()).await?;
+    let result = crate::tokio::async_read::extract_conda(reader, destination).await?;
+    if let Some(reporter) = &reporter {
+        reporter.on_download_complete();
+    }
+    Ok(result)
 }
 
 /// Extracts the contents a package archive from the specified remote location. The type of package
 /// is determined based on the path of the url.
 ///
 /// ```rust,no_run
 /// # #[tokio::main]
@@ -125,25 +150,31 @@
 /// use rattler_package_streaming::reqwest::tokio::extract;
 /// use reqwest::Client;
 /// use reqwest_middleware::ClientWithMiddleware;
 /// let _ = extract(
 ///     ClientWithMiddleware::from(Client::new()),
 ///     Url::parse("https://conda.anaconda.org/conda-forge/linux-64/python-3.10.8-h4a9ceb5_0_cpython.conda").unwrap(),
 ///     Path::new("/tmp"),
+///     None,
 ///     None)
 ///     .await
 ///     .unwrap();
 /// # }
 /// ```
 pub async fn extract(
     client: reqwest_middleware::ClientWithMiddleware,
     url: Url,
     destination: &Path,
     expected_sha256: Option<Sha256Hash>,
+    reporter: Option<Arc<dyn DownloadReporter>>,
 ) -> Result<ExtractResult, ExtractError> {
     match ArchiveType::try_from(Path::new(url.path()))
         .ok_or(ExtractError::UnsupportedArchiveType)?
     {
-        ArchiveType::TarBz2 => extract_tar_bz2(client, url, destination, expected_sha256).await,
-        ArchiveType::Conda => extract_conda(client, url, destination, expected_sha256).await,
+        ArchiveType::TarBz2 => {
+            extract_tar_bz2(client, url, destination, expected_sha256, reporter).await
+        }
+        ArchiveType::Conda => {
+            extract_conda(client, url, destination, expected_sha256, reporter).await
+        }
     }
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/seek.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/seek.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/async_read.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/tokio/fs.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/src/write.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/src/write.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 //! Functionality for writing conda packages
 use std::fs::{self, File};
 use std::io::{self, Read, Seek, Write};
 use std::path::{Path, PathBuf};
 
+use chrono::{Datelike, Timelike};
 use rattler_conda_types::package::PackageMetadata;
+use zip::DateTime;
 
 /// Trait for progress bars
 pub trait ProgressBar {
     /// Set the current progress and progress message
     fn set_progress(&mut self, progress: u64, message: &str);
     /// Set the total amount of bytes
     fn set_total(&mut self, total: u64);
@@ -285,16 +287,34 @@
     compression_num_threads: Option<u32>,
     out_name: &str,
     timestamp: Option<&chrono::DateTime<chrono::Utc>>,
     progress_bar: Option<Box<dyn ProgressBar>>,
 ) -> Result<(), std::io::Error> {
     // first create the outer zip archive that uses no compression
     let mut outer_archive = zip::ZipWriter::new(writer);
-    let options =
-        zip::write::FileOptions::default().compression_method(zip::CompressionMethod::Stored);
+
+    let last_modified_time = if let Some(time) = timestamp {
+        DateTime::from_date_and_time(
+            time.year() as u16,
+            time.month() as u8,
+            time.day() as u8,
+            time.hour() as u8,
+            time.minute() as u8,
+            time.second() as u8,
+        )
+        .expect("time should be in correct range")
+    } else {
+        // 1-1-2023 00:00:00 (Fixed date in the past for reproducible builds)
+        DateTime::from_date_and_time(2023, 1, 1, 0, 0, 0)
+            .expect("1-1-2023 00:00:00 should convert into datetime")
+    };
+
+    let options = zip::write::FileOptions::default()
+        .compression_method(zip::CompressionMethod::Stored)
+        .last_modified_time(last_modified_time);
 
     // write the metadata as first file in the zip archive
     let package_metadata = PackageMetadata::default();
     let package_metadata = serde_json::to_string(&package_metadata).unwrap();
     outer_archive.start_file("metadata.json", options)?;
     outer_archive.write_all(package_metadata.as_bytes())?;
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/tests/extract.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/extract.rs`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     let mut info_stream = rattler_package_streaming::seek::stream_conda_info(
         File::open(test_data_dir().join(file_path)).unwrap(),
     )
     .unwrap();
 
     let target_dir = temp_dir.join(format!(
         "{}-info",
-        file_path.file_stem().unwrap().to_string_lossy().as_ref()
+        &file_path.file_stem().unwrap().to_string_lossy()
     ));
 
     info_stream.unpack(target_dir).unwrap();
 }
 
 #[apply(conda_archives)]
 fn read_package_file(#[case] input: &str, #[case] _sha256: &str, #[case] _md5: &str) {
@@ -206,15 +206,15 @@
     .await
     .unwrap();
 
     assert_eq!(&format!("{:x}", result.sha256), sha256);
     assert_eq!(&format!("{:x}", result.md5), md5);
 }
 
-#[cfg(all(feature = "reqwest"))]
+#[cfg(feature = "reqwest")]
 #[apply(url_archives)]
 #[tokio::test]
 async fn test_extract_url_async(#[case] url: &str, #[case] sha256: &str, #[case] md5: &str) {
     use reqwest::Client;
     use reqwest_middleware::ClientWithMiddleware;
 
     let temp_dir = Path::new(env!("CARGO_TARGET_TMPDIR")).join("tokio");
@@ -227,14 +227,15 @@
     let target_dir = temp_dir.join(name);
     let url = url::Url::parse(url).unwrap();
     let result = rattler_package_streaming::reqwest::tokio::extract(
         ClientWithMiddleware::from(Client::new()),
         url,
         &target_dir,
         None,
+        None,
     )
     .await
     .unwrap();
 
     assert_eq!(&format!("{:x}", result.sha256), sha256);
     assert_eq!(&format!("{:x}", result.md5), md5);
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_package_streaming/tests/write.rs` & `py_rattler-0.6.0/local_dependencies/rattler_package_streaming/tests/write.rs`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
         println!("Name: {}", file_path.display());
 
         let target_dir = temp_dir.join(file_path.file_stem().unwrap());
         extract_tar_bz2(File::open(&file_path).unwrap(), &target_dir).unwrap();
 
         let new_archive = temp_dir.join(format!(
             "{}-new.tar.bz2",
-            file_path.file_stem().unwrap().to_string_lossy().as_ref()
+            &file_path.file_stem().unwrap().to_string_lossy()
         ));
 
         let writer = File::create(&new_archive).unwrap();
         let paths = find_all_package_files(&target_dir);
         write_tar_bz2_package(
             writer,
             &target_dir,
@@ -209,15 +209,15 @@
 
         let name = file_path.file_stem().unwrap().to_string_lossy();
         let target_dir = temp_dir.join(file_path.file_stem().unwrap());
         extract_conda(File::open(&file_path).unwrap(), &target_dir).unwrap();
 
         let new_archive = temp_dir.join(format!(
             "{}-new.conda",
-            file_path.file_stem().unwrap().to_string_lossy().as_ref()
+            &file_path.file_stem().unwrap().to_string_lossy()
         ));
 
         let writer = File::create(&new_archive).unwrap();
         let paths = find_all_package_files(&target_dir);
         write_conda_package(
             writer,
             &target_dir,
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_solve/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [package]
 name = "rattler_solve"
-version = "0.21.0"
+version = "0.23.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "A crate to solve conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
 rattler_libsolv_c = { path= "../rattler_libsolv_c", version = "0.19.3", default-features = false, optional = true }
 libc = { version = "0.2" , optional = true }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 thiserror = "1.0"
 tracing = "0.1.40"
 itertools = "0.12.1"
 url = { version = "2.5.0" }
 tempfile = "3.10.1"
-resolvo = { version = "0.4.0" , optional = true }
+resolvo = { version = "0.4.1" , optional = true }
 futures = { version = "0.3.30", optional = true }
 
 [features]
-default = ["libsolv_c"]
+default = ["resolvo"]
 libsolv_c = ["rattler_libsolv_c", "libc"]
 resolvo = ["dep:resolvo", "dep:futures"]
 
 [[bench]]
 name = "bench"
 harness = false
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_solve/CHANGELOG.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,45 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.23.0](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.22.0...rattler_solve-v0.23.0) - 2024-05-27
+
+### Added
+- removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
+- always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
+- add solve strategies ([#660](https://github.com/mamba-org/rattler/pull/660))
+
+### Fixed
+- result grouped by subdir instead of channel ([#666](https://github.com/mamba-org/rattler/pull/666))
+
+### Other
+- introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
+
+## [0.22.0](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.21.2...rattler_solve-v0.22.0) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.21.2](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.21.1...rattler_solve-v0.21.2) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Other
+- update README.md
+
+## [0.21.1](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.21.0...rattler_solve-v0.21.1) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.20.7...rattler_solve-v0.21.0) - 2024-04-25
 
 ### Added
 - add channel priority to solve task and expose to python solve ([#598](https://github.com/mamba-org/rattler/pull/598))
 
 ## [0.20.7](https://github.com/mamba-org/rattler/compare/rattler_solve-v0.20.6...rattler_solve-v0.20.7) - 2024-04-25
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/benches/bench.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/benches/bench.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use criterion::{black_box, criterion_group, criterion_main, Criterion, SamplingMode};
 use rattler_conda_types::ParseStrictness::Strict;
 use rattler_conda_types::{Channel, ChannelConfig, MatchSpec};
 use rattler_repodata_gateway::sparse::SparseRepoData;
-use rattler_solve::{ChannelPriority, SolverImpl, SolverTask};
+use rattler_solve::{SolverImpl, SolverTask};
 
 fn conda_json_path() -> String {
     format!(
         "{}/{}",
         env!("CARGO_MANIFEST_DIR"),
         "../../test-data/channels/conda-forge/linux-64/repodata.json"
     )
@@ -59,38 +59,28 @@
         SparseRepoData::load_records_recursive(&sparse_repo_datas, names, None).unwrap();
 
     #[cfg(feature = "libsolv_c")]
     group.bench_function("libsolv_c", |b| {
         b.iter(|| {
             rattler_solve::libsolv_c::Solver
                 .solve(black_box(SolverTask {
-                    available_packages: &available_packages,
-                    locked_packages: vec![],
-                    pinned_packages: vec![],
-                    virtual_packages: vec![],
                     specs: specs.clone(),
-                    timeout: None,
-                    channel_priority: ChannelPriority::Strict,
+                    ..SolverTask::from_iter(&available_packages)
                 }))
                 .unwrap()
         });
     });
 
     #[cfg(feature = "resolvo")]
     group.bench_function("resolvo", |b| {
         b.iter(|| {
             rattler_solve::resolvo::Solver
                 .solve(black_box(SolverTask {
-                    available_packages: &available_packages,
-                    locked_packages: vec![],
-                    pinned_packages: vec![],
-                    virtual_packages: vec![],
                     specs: specs.clone(),
-                    timeout: None,
-                    channel_priority: ChannelPriority::Strict,
+                    ..SolverTask::from_iter(&available_packages)
                 }))
                 .unwrap()
         });
     });
 
     group.finish();
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/lib.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-//! `rattler_solve` is a crate that provides functionality to solve Conda environments. It currently
-//! exposes the functionality through the [`SolverImpl::solve`] function.
+//! `rattler_solve` is a crate that provides functionality to solve Conda
+//! environments. It currently exposes the functionality through the
+//! [`SolverImpl::solve`] function.
 
 #![deny(missing_docs)]
 
 #[cfg(feature = "libsolv_c")]
 pub mod libsolv_c;
 #[cfg(feature = "resolvo")]
 pub mod resolvo;
 
-use rattler_conda_types::{GenericVirtualPackage, MatchSpec, RepoDataRecord};
 use std::fmt;
 
+use chrono::{DateTime, Utc};
+use rattler_conda_types::{GenericVirtualPackage, MatchSpec, RepoDataRecord};
+
 /// Represents a solver implementation, capable of solving [`SolverTask`]s
 pub trait SolverImpl {
     /// The repo data associated to a channel and platform combination
     type RepoData<'a>: SolverRepoData<'a>;
 
-    /// Resolve the dependencies and return the [`RepoDataRecord`]s that should be present in the
-    /// environment.
+    /// Resolve the dependencies and return the [`RepoDataRecord`]s that should
+    /// be present in the environment.
     fn solve<
         'a,
         R: IntoRepoData<'a, Self::RepoData<'a>>,
         TAvailablePackagesIterator: IntoIterator<Item = R>,
     >(
         &mut self,
         task: SolverTask<TAvailablePackagesIterator>,
@@ -31,22 +34,25 @@
 /// Represents an error when solving the dependencies for a given environment
 #[derive(thiserror::Error, Debug)]
 pub enum SolveError {
     /// There is no set of dependencies that satisfies the requirements
     Unsolvable(Vec<String>),
 
     /// The solver backend returned operations that we dont know how to install.
-    /// Each string is a somewhat user-friendly representation of which operation was not recognized
-    /// and can be used for error reporting
+    /// Each string is a somewhat user-friendly representation of which
+    /// operation was not recognized and can be used for error reporting
     UnsupportedOperations(Vec<String>),
 
     /// Error when converting matchspec
     #[error(transparent)]
     ParseMatchSpecError(#[from] rattler_conda_types::ParseMatchSpecError),
 
+    /// Encountered duplicate records in the available packages.
+    DuplicateRecords(String),
+
     /// To support Resolvo cancellation
     Cancelled,
 }
 
 impl fmt::Display for SolveError {
     fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
         match self {
@@ -62,87 +68,141 @@
             }
             SolveError::ParseMatchSpecError(e) => {
                 write!(f, "Error parsing match spec: {e}")
             }
             SolveError::Cancelled => {
                 write!(f, "Solve operation has been cancelled")
             }
+            SolveError::DuplicateRecords(filename) => {
+                write!(f, "encountered duplicate records for {filename}")
+            }
         }
     }
 }
 
 /// Represents the channel priority option to use during solves.
-#[derive(Clone, Copy, PartialEq, Eq)]
+#[derive(Clone, Copy, PartialEq, Eq, Default)]
 pub enum ChannelPriority {
-    /// The channel that the package is first found in will be used as the only channel
-    /// for that package.
+    /// The channel that the package is first found in will be used as the only
+    /// channel for that package.
+    #[default]
     Strict,
 
     // Conda also has "Flexible" as an option, where packages present in multiple channels
     // are only taken from lower-priority channels when this prevents unsatisfiable environment
     // errors, but this would need implementation in the solvers.
     // Flexible,
-    /// Packages can be retrieved from any channel as package version takes precedence.
+    /// Packages can be retrieved from any channel as package version takes
+    /// precedence.
     Disabled,
 }
 
-/// Represents a dependency resolution task, to be solved by one of the backends (currently only
-/// libsolv is supported)
+/// Represents a dependency resolution task, to be solved by one of the backends
+/// (currently only libsolv is supported)
 pub struct SolverTask<TAvailablePackagesIterator> {
     /// An iterator over all available packages
     pub available_packages: TAvailablePackagesIterator,
 
     /// Records of packages that are previously selected.
     ///
-    /// If the solver encounters multiple variants of a single package (identified by its name), it
-    /// will sort the records and select the best possible version. However, if there exists a
-    /// locked version it will prefer that variant instead. This is useful to reduce the number of
+    /// If the solver encounters multiple variants of a single package
+    /// (identified by its name), it will sort the records and select the
+    /// best possible version. However, if there exists a locked version it
+    /// will prefer that variant instead. This is useful to reduce the number of
     /// packages that are updated when installing new packages.
     ///
-    /// Usually you add the currently installed packages or packages from a lock-file here.
+    /// Usually you add the currently installed packages or packages from a
+    /// lock-file here.
     pub locked_packages: Vec<RepoDataRecord>,
 
     /// Records of packages that are previously selected and CANNOT be changed.
     ///
-    /// If the solver encounters multiple variants of a single package (identified by its name), it
-    /// will sort the records and select the best possible version. However, if there is a variant
-    /// available in the `pinned_packages` field it will always select that version no matter what
-    /// even if that means other packages have to be downgraded.
+    /// If the solver encounters multiple variants of a single package
+    /// (identified by its name), it will sort the records and select the
+    /// best possible version. However, if there is a variant available in
+    /// the `pinned_packages` field it will always select that version no matter
+    /// what even if that means other packages have to be downgraded.
     pub pinned_packages: Vec<RepoDataRecord>,
 
     /// Virtual packages considered active
     pub virtual_packages: Vec<GenericVirtualPackage>,
 
     /// The specs we want to solve
     pub specs: Vec<MatchSpec>,
 
     /// The timeout after which the solver should stop
     pub timeout: Option<std::time::Duration>,
 
-    /// The channel priority to solve with, either [`ChannelPriority::Strict`] or
-    /// [`ChannelPriority::Disabled`]
+    /// The channel priority to solve with, either [`ChannelPriority::Strict`]
+    /// or [`ChannelPriority::Disabled`]
     pub channel_priority: ChannelPriority,
+
+    /// Exclude any package that has a timestamp newer than the specified
+    /// timestamp.
+    pub exclude_newer: Option<DateTime<Utc>>,
+
+    /// The solve strategy.
+    pub strategy: SolveStrategy,
+}
+
+impl<'r, I: IntoIterator<Item = &'r RepoDataRecord>> FromIterator<I>
+    for SolverTask<Vec<RepoDataIter<I>>>
+{
+    fn from_iter<T: IntoIterator<Item = I>>(iter: T) -> Self {
+        Self {
+            available_packages: iter.into_iter().map(|iter| RepoDataIter(iter)).collect(),
+            locked_packages: Vec::new(),
+            pinned_packages: Vec::new(),
+            virtual_packages: Vec::new(),
+            specs: Vec::new(),
+            timeout: None,
+            channel_priority: ChannelPriority::default(),
+            exclude_newer: None,
+            strategy: SolveStrategy::default(),
+        }
+    }
 }
 
-/// A representation of a collection of [`RepoDataRecord`] usable by a [`SolverImpl`]
-/// implementation.
+/// Represents the strategy to use when solving dependencies
+#[derive(Debug, Clone, Copy, Default, Eq, PartialEq)]
+pub enum SolveStrategy {
+    /// Resolve the highest version of each package.
+    #[default]
+    Highest,
+
+    /// Resolve the lowest compatible version for each package.
+    ///
+    /// All candidates with the same version are still ordered the same as
+    /// with `Default`. This ensures that the candidate with the highest build
+    /// number is used and downprioritization still works.
+    LowestVersion,
+
+    /// Resolve the lowest compatible version for direct dependencies but the
+    /// highest for transitive dependencies. This is similar to `LowestVersion`
+    /// but only for direct dependencies.
+    LowestVersionDirect,
+}
+
+/// A representation of a collection of [`RepoDataRecord`] usable by a
+/// [`SolverImpl`] implementation.
 ///
-/// Some solvers might be able to cache the collection between different runs of the solver which
-/// could potentially eliminate some overhead. This trait enables creating a representation of the
-/// repodata that is most suitable for a specific backend.
+/// Some solvers might be able to cache the collection between different runs of
+/// the solver which could potentially eliminate some overhead. This trait
+/// enables creating a representation of the repodata that is most suitable for
+/// a specific backend.
 ///
-/// Some solvers may add additional functionality to their specific implementation that enables
-/// caching the repodata to disk in an efficient way (see [`crate::libsolv_c::RepoData`] for
-/// an example).
+/// Some solvers may add additional functionality to their specific
+/// implementation that enables caching the repodata to disk in an efficient way
+/// (see [`crate::libsolv_c::RepoData`] for an example).
 pub trait SolverRepoData<'a>: FromIterator<&'a RepoDataRecord> {}
 
 /// Defines the ability to convert a type into [`SolverRepoData`].
 pub trait IntoRepoData<'a, S: SolverRepoData<'a>> {
-    /// Converts this instance into an instance of [`SolverRepoData`] which is consumable by a
-    /// specific [`SolverImpl`] implementation.
+    /// Converts this instance into an instance of [`SolverRepoData`] which is
+    /// consumable by a specific [`SolverImpl`] implementation.
     fn into(self) -> S;
 }
 
 impl<'a, S: SolverRepoData<'a>> IntoRepoData<'a, S> for &'a Vec<RepoDataRecord> {
     fn into(self) -> S {
         self.iter().collect()
     }
@@ -155,7 +215,19 @@
 }
 
 impl<'a, S: SolverRepoData<'a>> IntoRepoData<'a, S> for S {
     fn into(self) -> S {
         self
     }
 }
+
+/// A helper struct that implements `IntoRepoData` for anything that can
+/// iterate over `RepoDataRecord`s.
+pub struct RepoDataIter<T>(pub T);
+
+impl<'a, T: IntoIterator<Item = &'a RepoDataRecord>, S: SolverRepoData<'a>> IntoRepoData<'a, S>
+    for RepoDataIter<T>
+{
+    fn into(self) -> S {
+        self.0.into_iter().collect()
+    }
+}
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/input.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-//! Contains business logic that loads information into libsolv in order to solve a conda
-//! environment
+//! Contains business logic that loads information into libsolv in order to
+//! solve a conda environment
+
+use std::{cmp::Ordering, collections::HashMap};
+
+use chrono::{DateTime, Utc};
+use rattler_conda_types::{package::ArchiveType, GenericVirtualPackage, RepoDataRecord};
 
 use super::{
     c_string,
     libc_byte_slice::LibcByteSlice,
     wrapper::{
         keys::{
             REPOKEY_TYPE_MD5, REPOKEY_TYPE_SHA256, SOLVABLE_BUILDFLAVOR, SOLVABLE_BUILDTIME,
@@ -12,31 +17,32 @@
         },
         pool::Pool,
         repo::Repo,
         repodata::Repodata,
         solvable::SolvableId,
     },
 };
-use rattler_conda_types::{package::ArchiveType, GenericVirtualPackage, RepoDataRecord};
-use std::{cmp::Ordering, collections::HashMap};
+use crate::SolveError;
 
 #[cfg(not(target_family = "unix"))]
 /// Adds solvables to a repo from an in-memory .solv file
 ///
-/// Note: this function relies on primitives that are only available on unix-like operating systems,
-/// and will panic if called from another platform (e.g. Windows)
+/// Note: this function relies on primitives that are only available on
+/// unix-like operating systems, and will panic if called from another platform
+/// (e.g. Windows)
 pub fn add_solv_file(_pool: &Pool, _repo: &Repo<'_>, _solv_bytes: &LibcByteSlice) {
     unimplemented!("this platform does not support in-memory .solv files");
 }
 
 #[cfg(target_family = "unix")]
 /// Adds solvables to a repo from an in-memory .solv file
 ///
-/// Note: this function relies on primitives that are only available on unix-like operating systems,
-/// and will panic if called from another platform (e.g. Windows)
+/// Note: this function relies on primitives that are only available on
+/// unix-like operating systems, and will panic if called from another platform
+/// (e.g. Windows)
 pub fn add_solv_file(pool: &Pool, repo: &Repo<'_>, solv_bytes: &LibcByteSlice) {
     // Add solv file from memory if available
     let mode = c_string("r");
     let file = unsafe { libc::fmemopen(solv_bytes.as_ptr(), solv_bytes.len(), mode.as_ptr()) };
     repo.add_solv(pool, file);
     unsafe { libc::fclose(file) };
 }
@@ -44,20 +50,21 @@
 /// Adds [`RepoDataRecord`] to `repo`
 ///
 /// Panics if the repo does not belong to the pool
 pub fn add_repodata_records<'a>(
     pool: &Pool,
     repo: &Repo<'_>,
     repo_datas: impl IntoIterator<Item = &'a RepoDataRecord>,
-) -> Vec<SolvableId> {
+    exclude_newer: Option<&DateTime<Utc>>,
+) -> Result<Vec<SolvableId>, SolveError> {
     // Sanity check
     repo.ensure_belongs_to_pool(pool);
 
-    // Get all the IDs (these strings are internal to libsolv and always present, so we can
-    // unwrap them at will)
+    // Get all the IDs (these strings are internal to libsolv and always present, so
+    // we can unwrap them at will)
     let solvable_buildflavor_id = pool.find_interned_str(SOLVABLE_BUILDFLAVOR).unwrap();
     let solvable_buildtime_id = pool.find_interned_str(SOLVABLE_BUILDTIME).unwrap();
     let solvable_buildversion_id = pool.find_interned_str(SOLVABLE_BUILDVERSION).unwrap();
     let solvable_constraints = pool.find_interned_str(SOLVABLE_CONSTRAINS).unwrap();
     let solvable_download_size_id = pool.find_interned_str(SOLVABLE_DOWNLOADSIZE).unwrap();
     let solvable_license_id = pool.find_interned_str(SOLVABLE_LICENSE).unwrap();
     let solvable_pkg_id = pool.find_interned_str(SOLVABLE_PKGID).unwrap();
@@ -68,31 +75,39 @@
 
     // Custom id
     let solvable_index_id = pool.intern_str("solvable:repodata_record_index");
 
     // Keeps a mapping from packages added to the repo to the type and solvable
     let mut package_to_type: HashMap<&str, (ArchiveType, SolvableId)> = HashMap::new();
 
-    // Through `data` we can manipulate solvables (see the `Repodata` docs for details)
+    // Through `data` we can manipulate solvables (see the `Repodata` docs for
+    // details)
     let data = repo.add_repodata();
 
     let mut solvable_ids = Vec::new();
     for (repo_data_index, repo_data) in repo_datas.into_iter().enumerate() {
+        // Skip packages that are newer than the specified timestamp
+        match (exclude_newer, repo_data.package_record.timestamp.as_ref()) {
+            (Some(exclude_newer), Some(timestamp)) if *timestamp > *exclude_newer => continue,
+            _ => {}
+        }
+
         // Create a solvable for the package
         let solvable_id =
-            match add_or_reuse_solvable(pool, repo, &data, &mut package_to_type, repo_data) {
+            match add_or_reuse_solvable(pool, repo, &data, &mut package_to_type, repo_data)? {
                 Some(id) => id,
                 None => continue,
             };
 
         // Store the current index so we can retrieve the original repo data record
         // from the final transaction
         data.set_num(solvable_id, solvable_index_id, repo_data_index as u64);
 
-        // Safe because there are no other active references to any solvable (so no aliasing)
+        // Safe because there are no other active references to any solvable (so no
+        // aliasing)
         let solvable = unsafe { solvable_id.resolve_raw(pool).as_mut() };
         let record = &repo_data.package_record;
 
         // Name and version
         solvable.name = pool.intern_str(record.name.as_normalized()).into();
         solvable.evr = pool.intern_str(record.version.to_string()).into();
         let rel_eq = pool.rel_eq(solvable.name, solvable.evr);
@@ -189,75 +204,77 @@
         }
 
         solvable_ids.push(solvable_id);
     }
 
     repo.internalize();
 
-    solvable_ids
+    Ok(solvable_ids)
 }
 
-/// When adding packages, we want to make sure that `.conda` packages have preference over `.tar.bz`
-/// packages. For that reason, when adding a solvable we check first if a `.conda` version of the
-/// package has already been added, in which case we forgo adding its `.tar.bz` version (and return
-/// `None`). If no `.conda` version has been added, we create a new solvable (replacing any existing
-/// solvable for the `.tar.bz` version of the package).
+/// When adding packages, we want to make sure that `.conda` packages have
+/// preference over `.tar.bz` packages. For that reason, when adding a solvable
+/// we check first if a `.conda` version of the package has already been added,
+/// in which case we forgo adding its `.tar.bz` version (and return `None`). If
+/// no `.conda` version has been added, we create a new solvable (replacing any
+/// existing solvable for the `.tar.bz` version of the package).
 fn add_or_reuse_solvable<'a>(
     pool: &Pool,
     repo: &Repo<'_>,
     data: &Repodata<'_>,
     package_to_type: &mut HashMap<&'a str, (ArchiveType, SolvableId)>,
     repo_data: &'a RepoDataRecord,
-) -> Option<SolvableId> {
+) -> Result<Option<SolvableId>, SolveError> {
     // Sometimes we can reuse an existing solvable
     if let Some((filename, archive_type)) = ArchiveType::split_str(&repo_data.file_name) {
         if let Some(&(other_package_type, old_solvable_id)) = package_to_type.get(filename) {
             match archive_type.cmp(&other_package_type) {
                 Ordering::Less => {
                     // A previous package that we already stored is actually a package of a better
                     // "type" so we'll just use that instead (.conda > .tar.bz)
-                    return None;
+                    return Ok(None);
                 }
                 Ordering::Greater => {
                     // A previous package has a worse package "type", we'll reuse the handle but
                     // overwrite its attributes
 
                     // Update the package to the new type mapping
                     package_to_type.insert(filename, (archive_type, old_solvable_id));
 
                     // Reset and reuse the old solvable
                     reset_solvable(pool, repo, data, old_solvable_id);
-                    return Some(old_solvable_id);
+                    return Ok(Some(old_solvable_id));
                 }
                 Ordering::Equal => {
-                    unreachable!("found a duplicate package")
+                    return Err(SolveError::DuplicateRecords(filename.to_string()));
                 }
             }
         } else {
             let solvable_id = repo.add_solvable();
             package_to_type.insert(filename, (archive_type, solvable_id));
-            return Some(solvable_id);
+            return Ok(Some(solvable_id));
         }
     } else {
         tracing::warn!("unknown package extension: {}", &repo_data.file_name);
     }
 
-    Some(repo.add_solvable())
+    Ok(Some(repo.add_solvable()))
 }
 
 pub fn add_virtual_packages(pool: &Pool, repo: &Repo<'_>, packages: &[GenericVirtualPackage]) {
     let data = repo.add_repodata();
 
     let solvable_buildflavor_id = pool.find_interned_str(SOLVABLE_BUILDFLAVOR).unwrap();
 
     for package in packages {
         // Create a solvable for the package
         let solvable_id = repo.add_solvable();
 
-        // Safe because there are no other references to this solvable_id (we just created it)
+        // Safe because there are no other references to this solvable_id (we just
+        // created it)
         let solvable = unsafe { solvable_id.resolve_raw(pool).as_mut() };
 
         // Name and version
         solvable.name = pool.intern_str(package.name.as_normalized()).into();
         solvable.evr = pool.intern_str(package.version.to_string()).into();
         let rel_eq = pool.rel_eq(solvable.name, solvable.evr);
         repo.add_provides(solvable, rel_eq);
@@ -274,50 +291,53 @@
 fn reset_solvable(pool: &Pool, repo: &Repo<'_>, data: &Repodata<'_>, solvable_id: SolvableId) {
     let blank_solvable = repo.add_solvable();
 
     // Replace the existing solvable with the blank one
     pool.swap_solvables(blank_solvable, solvable_id);
     data.swap_attrs(blank_solvable, solvable_id);
 
-    // It is safe to free the blank solvable, because there are no other references to it
-    // than in this function
+    // It is safe to free the blank solvable, because there are no other references
+    // to it than in this function
     unsafe { repo.free_solvable(blank_solvable) };
 }
 
 /// Caches the repodata as an in-memory `.solv` file
 ///
-/// Note: this function relies on primitives that are only available on unix-like operating systems,
-/// and will panic if called from another platform (e.g. Windows)
+/// Note: this function relies on primitives that are only available on
+/// unix-like operating systems, and will panic if called from another platform
+/// (e.g. Windows)
 #[cfg(not(target_family = "unix"))]
-pub fn cache_repodata(_url: String, _data: &[RepoDataRecord]) -> LibcByteSlice {
+pub fn cache_repodata(_url: String, _data: &[RepoDataRecord]) -> Result<LibcByteSlice, SolveError> {
     unimplemented!("this function is only available on unix-like operating systems")
 }
 
 /// Caches the repodata as an in-memory `.solv` file
 ///
-/// Note: this function relies on primitives that are only available on unix-like operating systems,
-/// and will panic if called from another platform (e.g. Windows)
+/// Note: this function relies on primitives that are only available on
+/// unix-like operating systems, and will panic if called from another platform
+/// (e.g. Windows)
 #[cfg(target_family = "unix")]
 pub fn cache_repodata(
     url: String,
     data: &[RepoDataRecord],
     channel_priority: Option<i32>,
-) -> LibcByteSlice {
+) -> Result<LibcByteSlice, SolveError> {
     // Add repodata to a new pool + repo
     let pool = Pool::default();
     let repo = Repo::new(&pool, url, channel_priority.unwrap_or(0));
-    add_repodata_records(&pool, &repo, data);
+    add_repodata_records(&pool, &repo, data, None)?;
 
     // Export repo to .solv in memory
     let mut stream_ptr = std::ptr::null_mut();
     let mut stream_size = 0;
     let file = unsafe { libc::open_memstream(&mut stream_ptr, &mut stream_size) };
     assert!(!file.is_null(), "unable to open memstream");
 
     repo.write(&pool, file);
     unsafe { libc::fclose(file) };
 
     let stream_ptr = std::ptr::NonNull::new(stream_ptr).expect("stream_ptr was null");
 
-    // Safe because we know `stream_ptr` points to an array of bytes of length `stream_size`
-    unsafe { LibcByteSlice::from_raw_parts(stream_ptr.cast(), stream_size) }
+    // Safe because we know `stream_ptr` points to an array of bytes of length
+    // `stream_size`
+    Ok(unsafe { LibcByteSlice::from_raw_parts(stream_ptr.cast(), stream_size) })
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/libc_byte_slice.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 //! Provides an solver implementation based on the [`rattler_libsolv_c`] crate.
 
-use crate::{ChannelPriority, IntoRepoData, SolverRepoData};
-use crate::{SolveError, SolverTask};
+use std::{
+    collections::{HashMap, HashSet},
+    ffi::CString,
+    mem::ManuallyDrop,
+};
+
 pub use input::cache_repodata;
 use input::{add_repodata_records, add_solv_file, add_virtual_packages};
 pub use libc_byte_slice::LibcByteSlice;
 use output::get_required_packages;
 use rattler_conda_types::RepoDataRecord;
-use std::collections::{HashMap, HashSet};
-use std::ffi::CString;
-use std::mem::ManuallyDrop;
 use wrapper::{
     flags::SolverFlag,
     pool::{Pool, Verbosity},
     repo::Repo,
     solve_goal::SolveGoal,
 };
 
+use crate::{ChannelPriority, IntoRepoData, SolveError, SolveStrategy, SolverRepoData, SolverTask};
+
 mod input;
 mod libc_byte_slice;
 mod output;
 mod wrapper;
 
-/// Represents the information required to load available packages into libsolv for a single channel
-/// and platform combination
+/// Represents the information required to load available packages into libsolv
+/// for a single channel and platform combination
 #[derive(Clone)]
 pub struct RepoData<'a> {
     /// The actual records after parsing `repodata.json`
     pub records: Vec<&'a RepoDataRecord>,
 
     /// The in-memory .solv file built from the records (if available)
     pub solv_file: Option<&'a LibcByteSlice>,
@@ -51,16 +54,16 @@
             solv_file: None,
         }
     }
 }
 
 impl<'a> SolverRepoData<'a> for RepoData<'a> {}
 
-/// Convenience method that converts a string reference to a `CString`, replacing NUL characters
-/// with whitespace (`b' '`)
+/// Convenience method that converts a string reference to a `CString`,
+/// replacing NUL characters with whitespace (`b' '`)
 fn c_string<T: AsRef<str>>(str: T) -> CString {
     let bytes = str.as_ref().as_bytes();
 
     let mut vec = Vec::with_capacity(bytes.len() + 1);
     vec.extend_from_slice(bytes);
 
     for byte in &mut vec {
@@ -68,15 +71,16 @@
             *byte = b' ';
         }
     }
 
     // Trailing 0
     vec.push(0);
 
-    // Safe because the string does is guaranteed to have no NUL bytes other than the trailing one
+    // Safe because the string does is guaranteed to have no NUL bytes other than
+    // the trailing one
     unsafe { CString::from_vec_with_nul_unchecked(vec) }
 }
 
 /// A [`Solver`] implemented using the `libsolv` library
 #[derive(Default)]
 pub struct Solver;
 
@@ -93,14 +97,20 @@
     ) -> Result<Vec<RepoDataRecord>, SolveError> {
         if task.timeout.is_some() {
             return Err(SolveError::UnsupportedOperations(vec![
                 "timeout".to_string()
             ]));
         }
 
+        if task.strategy != SolveStrategy::Highest {
+            return Err(SolveError::UnsupportedOperations(vec![
+                "strategy".to_string()
+            ]));
+        }
+
         // Construct a default libsolv pool
         let pool = Pool::default();
 
         // Setup proper logging for the pool
         pool.set_debug_callback(|msg, _flags| {
             tracing::event!(tracing::Level::DEBUG, "{}", msg.trim_end());
         });
@@ -108,18 +118,19 @@
 
         let repodatas: Vec<Self::RepoData<'_>> = task
             .available_packages
             .into_iter()
             .map(IntoRepoData::into)
             .collect();
 
-        // Determine the channel priority for each channel in the repodata in the order in which
-        // the repodatas are passed, where the first channel will have the highest priority value
-        // and each successive channel will descend in priority value. If not strict, the highest
-        // priority value will be 0 and the channel priority map will not be populated as it will
+        // Determine the channel priority for each channel in the repodata in the order
+        // in which the repodatas are passed, where the first channel will have
+        // the highest priority value and each successive channel will descend
+        // in priority value. If not strict, the highest priority value will be
+        // 0 and the channel priority map will not be populated as it will
         // not be used.
         let mut highest_priority: i32 = 0;
         let channel_priority: HashMap<String, i32> =
             if task.channel_priority == ChannelPriority::Strict {
                 let mut seen_channels = HashSet::new();
                 let mut channel_order: Vec<String> = Vec::new();
                 for channel in repodatas
@@ -168,33 +179,38 @@
                 0
             };
             let repo = ManuallyDrop::new(Repo::new(&pool, channel_name, priority));
 
             if let Some(solv_file) = repodata.solv_file {
                 add_solv_file(&pool, &repo, solv_file);
             } else {
-                add_repodata_records(&pool, &repo, repodata.records.iter().copied());
+                add_repodata_records(
+                    &pool,
+                    &repo,
+                    repodata.records.iter().copied(),
+                    task.exclude_newer.as_ref(),
+                )?;
             }
 
             // Keep our own info about repodata_records
             repo_mapping.insert(repo.id(), repo_mapping.len());
             all_repodata_records.push(repodata.records.clone());
         }
 
         // Create a special pool for records that are already installed or locked.
         let repo = Repo::new(&pool, "locked", highest_priority);
-        let installed_solvables = add_repodata_records(&pool, &repo, &task.locked_packages);
+        let installed_solvables = add_repodata_records(&pool, &repo, &task.locked_packages, None)?;
 
         // Also add the installed records to the repodata
         repo_mapping.insert(repo.id(), repo_mapping.len());
         all_repodata_records.push(task.locked_packages.iter().collect());
 
         // Create a special pool for records that are pinned and cannot be changed.
         let repo = Repo::new(&pool, "pinned", highest_priority);
-        let pinned_solvables = add_repodata_records(&pool, &repo, &task.pinned_packages);
+        let pinned_solvables = add_repodata_records(&pool, &repo, &task.pinned_packages, None)?;
 
         // Also add the installed records to the repodata
         repo_mapping.insert(repo.id(), repo_mapping.len());
         all_repodata_records.push(task.pinned_packages.iter().collect());
 
         // Create datastructures for solving
         pool.create_whatprovides();
@@ -246,17 +262,18 @@
 
         Ok(required_records)
     }
 }
 
 #[cfg(test)]
 mod test {
-    use super::*;
     use rstest::rstest;
 
+    use super::*;
+
     #[rstest]
     #[case("", "")]
     #[case("a\0b\0c\0d\0", "a b c d ")]
     #[case("a b c d", "a b c d")]
     #[case("😒", "😒")]
     fn test_c_string(#[case] input: &str, #[case] expected_output: &str) {
         let output = c_string(input);
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/output.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/keys.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/pool.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/queue.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repo.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/repodata.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solvable.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_goal.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solve_problem.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/solver.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/libsolv_c/wrapper/transaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/conda_util.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 use crate::resolvo::{CondaDependencyProvider, SolverMatchSpec};
 use futures::future::FutureExt;
 use rattler_conda_types::Version;
 use resolvo::{Dependencies, SolvableId, SolverCache, VersionSetId};
 use std::cmp::Ordering;
 use std::collections::HashMap;
+
+#[derive(Copy, Clone, Debug, Eq, PartialEq)]
+pub(super) enum CompareStrategy {
+    Default,
+    LowestVersion,
+}
+
 /// Returns the order of two candidates based on the order used by conda.
 #[allow(clippy::too_many_arguments)]
 pub(super) fn compare_candidates<'a>(
     a: SolvableId,
     b: SolvableId,
     solver: &SolverCache<SolverMatchSpec<'a>, String, CondaDependencyProvider<'a>>,
     match_spec_highest_version: &mut HashMap<
         VersionSetId,
         Option<(rattler_conda_types::Version, bool)>,
     >,
+    strategy: CompareStrategy,
 ) -> Ordering {
     let pool = solver.pool();
 
     let a_solvable = pool.resolve_solvable(a);
     let b_solvable = pool.resolve_solvable(b);
 
     let a_record = &a_solvable.inner();
@@ -30,18 +38,20 @@
     match a_has_tracked_features.cmp(&b_has_tracked_features) {
         Ordering::Less => return Ordering::Less,
         Ordering::Greater => return Ordering::Greater,
         Ordering::Equal => {}
     };
 
     // Otherwise, select the variant with the highest version
-    match a_record.version().cmp(b_record.version()) {
-        Ordering::Less => return Ordering::Greater,
-        Ordering::Greater => return Ordering::Less,
-        Ordering::Equal => {}
+    match (strategy, a_record.version().cmp(b_record.version())) {
+        (CompareStrategy::Default, Ordering::Greater)
+        | (CompareStrategy::LowestVersion, Ordering::Less) => return Ordering::Less,
+        (CompareStrategy::Default, Ordering::Less)
+        | (CompareStrategy::LowestVersion, Ordering::Greater) => return Ordering::Greater,
+        (_, Ordering::Equal) => {}
     };
 
     // Otherwise, select the variant with the highest build number
     match a_record.build_number().cmp(&b_record.build_number()) {
         Ordering::Less => return Ordering::Greater,
         Ordering::Greater => return Ordering::Less,
         Ordering::Equal => {}
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/src/resolvo/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/src/resolvo/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 //! Provides an solver implementation based on the [`resolvo`] crate.
 
-use crate::{ChannelPriority, IntoRepoData, SolveError, SolverRepoData, SolverTask};
-use rattler_conda_types::package::ArchiveType;
-use rattler_conda_types::{
-    GenericVirtualPackage, MatchSpec, NamelessMatchSpec, PackageRecord, ParseMatchSpecError,
-    ParseStrictness, RepoDataRecord,
-};
-use resolvo::{
-    Candidates, Dependencies, DependencyProvider, KnownDependencies, NameId, Pool, SolvableDisplay,
-    SolvableId, Solver as LibSolvRsSolver, SolverCache, UnsolvableOrCancelled, VersionSet,
-    VersionSetId,
-};
-use std::rc::Rc;
 use std::{
     cell::RefCell,
     cmp::Ordering,
-    collections::HashMap,
+    collections::{HashMap, HashSet},
     fmt::{Display, Formatter},
     marker::PhantomData,
     ops::Deref,
+    rc::Rc,
 };
 
+use chrono::{DateTime, Utc};
 use itertools::Itertools;
+use rattler_conda_types::{
+    package::ArchiveType, GenericVirtualPackage, MatchSpec, NamelessMatchSpec, PackageName,
+    PackageRecord, ParseMatchSpecError, ParseStrictness, RepoDataRecord,
+};
+use resolvo::{
+    Candidates, Dependencies, DependencyProvider, KnownDependencies, NameId, Pool, SolvableDisplay,
+    SolvableId, Solver as LibSolvRsSolver, SolverCache, UnsolvableOrCancelled, VersionSet,
+    VersionSetId,
+};
+
+use crate::{
+    resolvo::conda_util::CompareStrategy, ChannelPriority, IntoRepoData, SolveError, SolveStrategy,
+    SolverRepoData, SolverTask,
+};
 
 mod conda_util;
 
-/// Represents the information required to load available packages into libsolv for a single channel
-/// and platform combination
+/// Represents the information required to load available packages into libsolv
+/// for a single channel and platform combination
 #[derive(Clone)]
 pub struct RepoData<'a> {
     /// The actual records after parsing `repodata.json`
     pub records: Vec<&'a RepoDataRecord>,
 }
 
 impl<'a> FromIterator<&'a RepoDataRecord> for RepoData<'a> {
@@ -100,21 +104,44 @@
                 true
             }
         }
     }
 }
 
 /// Wrapper around [`PackageRecord`] so that we can use it in resolvo pool
-#[derive(Ord, PartialOrd, Eq, PartialEq)]
+#[derive(Eq, PartialEq)]
 enum SolverPackageRecord<'a> {
     Record(&'a RepoDataRecord),
     VirtualPackage(&'a GenericVirtualPackage),
 }
 
+impl<'a> PartialOrd<Self> for SolverPackageRecord<'a> {
+    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
+        Some(self.cmp(other))
+    }
+}
+
+impl<'a> Ord for SolverPackageRecord<'a> {
+    fn cmp(&self, other: &Self) -> Ordering {
+        self.name()
+            .cmp(other.name())
+            .then_with(|| self.version().cmp(other.version()))
+            .then_with(|| self.build_number().cmp(&other.build_number()))
+            .then_with(|| self.timestamp().cmp(&other.timestamp()))
+    }
+}
+
 impl<'a> SolverPackageRecord<'a> {
+    fn name(&self) -> &PackageName {
+        match self {
+            SolverPackageRecord::Record(rec) => &rec.package_record.name,
+            SolverPackageRecord::VirtualPackage(rec) => &rec.name,
+        }
+    }
+
     fn version(&self) -> &rattler_conda_types::Version {
         match self {
             SolverPackageRecord::Record(rec) => rec.package_record.version.version(),
             SolverPackageRecord::VirtualPackage(rec) => &rec.version,
         }
     }
 
@@ -163,114 +190,165 @@
 
     matchspec_to_highest_version:
         RefCell<HashMap<VersionSetId, Option<(rattler_conda_types::Version, bool)>>>,
 
     parse_match_spec_cache: RefCell<HashMap<&'a str, VersionSetId>>,
 
     stop_time: Option<std::time::SystemTime>,
+
+    strategy: SolveStrategy,
+
+    direct_dependencies: HashSet<NameId>,
 }
 
 impl<'a> CondaDependencyProvider<'a> {
+    #[allow(clippy::too_many_arguments)]
     pub fn from_solver_task(
         repodata: impl IntoIterator<Item = RepoData<'a>>,
         favored_records: &'a [RepoDataRecord],
         locked_records: &'a [RepoDataRecord],
         virtual_packages: &'a [GenericVirtualPackage],
         match_specs: &[MatchSpec],
         stop_time: Option<std::time::SystemTime>,
         channel_priority: ChannelPriority,
-    ) -> Self {
+        exclude_newer: Option<DateTime<Utc>>,
+        strategy: SolveStrategy,
+    ) -> Result<Self, SolveError> {
         let pool = Rc::new(Pool::default());
         let mut records: HashMap<NameId, Candidates> = HashMap::default();
 
         // Add virtual packages to the records
         for virtual_package in virtual_packages {
             let name = pool.intern_package_name(virtual_package.name.as_normalized());
             let solvable =
                 pool.intern_solvable(name, SolverPackageRecord::VirtualPackage(virtual_package));
             records.entry(name).or_default().candidates.push(solvable);
         }
 
+        // Compute the direct dependencies
+        let direct_dependencies = match_specs
+            .iter()
+            .filter_map(|spec| spec.name.as_ref())
+            .map(|name| pool.intern_package_name(name.as_normalized()))
+            .collect();
+
         // TODO: Normalize these channel names to urls so we can compare them correctly.
         let channel_specific_specs = match_specs
             .iter()
             .filter(|spec| spec.channel.is_some())
             .collect::<Vec<_>>();
 
         // Hashmap that maps the package name to the channel it was first found in.
         let mut package_name_found_in_channel = HashMap::<String, &String>::new();
 
         // Add additional records
         for repo_datas in repodata {
-            // Iterate over all records and dedup records that refer to the same package data but with
-            // different archive types. This can happen if you have two variants of the same package but
-            // with different extensions. We prefer `.conda` packages over `.tar.bz`.
+            // Iterate over all records and dedup records that refer to the same package
+            // data but with different archive types. This can happen if you
+            // have two variants of the same package but with different
+            // extensions. We prefer `.conda` packages over `.tar.bz`.
             //
-            // Its important to insert the records in the same same order as how they were presented to this
-            // function to ensure that each solve is deterministic. Iterating over HashMaps is not
-            // deterministic at runtime so instead we store the values in a Vec as we iterate over the
-            // records. This guarentees that the order of records remains the same over runs.
+            // Its important to insert the records in the same order as how they were
+            // presented to this function to ensure that each solve is
+            // deterministic. Iterating over HashMaps is not deterministic at
+            // runtime so instead we store the values in a Vec as we iterate over the
+            // records. This guarentees that the order of records remains the same over
+            // runs.
             let mut ordered_repodata = Vec::with_capacity(repo_datas.records.len());
-            let mut package_to_type: HashMap<&str, (ArchiveType, usize)> =
+            let mut package_to_type: HashMap<&str, (ArchiveType, usize, bool)> =
                 HashMap::with_capacity(repo_datas.records.len());
 
             for record in repo_datas.records {
+                // Determine if this record will be excluded.
+                let excluded = matches!((&exclude_newer, &record.package_record.timestamp),
+                    (Some(exclude_newer), Some(record_timestamp))
+                        if record_timestamp > exclude_newer);
+
                 let (file_name, archive_type) = ArchiveType::split_str(&record.file_name)
                     .unwrap_or((&record.file_name, ArchiveType::TarBz2));
                 match package_to_type.get_mut(file_name) {
                     None => {
                         let idx = ordered_repodata.len();
                         ordered_repodata.push(record);
-                        package_to_type.insert(file_name, (archive_type, idx));
+                        package_to_type.insert(file_name, (archive_type, idx, excluded));
                     }
-                    Some((prev_archive_type, idx)) => match archive_type.cmp(prev_archive_type) {
-                        Ordering::Greater => {
-                            // A previous package has a worse package "type", we'll use the current record
-                            // instead.
+                    Some((prev_archive_type, idx, previous_excluded)) => {
+                        if *previous_excluded && !excluded {
+                            // The previous package would have been excluded by the solver. If the
+                            // current record won't be excluded we should always use that.
                             *prev_archive_type = archive_type;
                             ordered_repodata[*idx] = record;
-                        }
-                        Ordering::Less => {
-                            // A previous package that we already stored is actually a package of a better
-                            // "type" so we'll just use that instead (.conda > .tar.bz)
-                        }
-                        Ordering::Equal => {
-                            if record != ordered_repodata[*idx] {
-                                unreachable!(
-                                    "found duplicate record with different values for {}",
-                                    &record.file_name
-                                );
+                            *previous_excluded = false;
+                        } else if excluded && !*previous_excluded {
+                            // The previous package would not have been excluded
+                            // by the solver but
+                            // this one will, so we'll keep the previous one
+                            // regardless of the type.
+                        } else {
+                            match archive_type.cmp(prev_archive_type) {
+                                Ordering::Greater => {
+                                    // A previous package has a worse package "type", we'll use the
+                                    // current record instead.
+                                    *prev_archive_type = archive_type;
+                                    ordered_repodata[*idx] = record;
+                                    *previous_excluded = excluded;
+                                }
+                                Ordering::Less => {
+                                    // A previous package that we already stored
+                                    // is actually a package of a better
+                                    // "type" so we'll just use that instead
+                                    // (.conda > .tar.bz)
+                                }
+                                Ordering::Equal => {
+                                    return Err(SolveError::DuplicateRecords(
+                                        record.file_name.clone(),
+                                    ));
+                                }
                             }
                         }
-                    },
+                    }
                 }
             }
 
             for record in ordered_repodata {
                 let package_name =
                     pool.intern_package_name(record.package_record.name.as_normalized());
                 let solvable_id =
                     pool.intern_solvable(package_name, SolverPackageRecord::Record(record));
                 let candidates = records.entry(package_name).or_default();
                 candidates.candidates.push(solvable_id);
 
+                // Filter out any records that are newer than a specific date.
+                match (&exclude_newer, &record.package_record.timestamp) {
+                    (Some(exclude_newer), Some(record_timestamp))
+                        if record_timestamp > exclude_newer =>
+                    {
+                        let reason = pool.intern_string(format!(
+                            "the package is uploaded after the cutoff date of {exclude_newer}"
+                        ));
+                        candidates.excluded.push((solvable_id, reason));
+                    }
+                    _ => {}
+                }
+
                 // Add to excluded when package is not in the specified channel.
                 if !channel_specific_specs.is_empty() {
                     if let Some(spec) = channel_specific_specs.iter().find(|&&spec| {
                         spec.name
                             .as_ref()
                             .expect("expecting a name")
                             .as_normalized()
                             == record.package_record.name.as_normalized()
                     }) {
                         // Check if the spec has a channel, and compare it to the repodata channel
                         if let Some(spec_channel) = &spec.channel {
                             if record.channel != spec_channel.base_url.to_string() {
                                 tracing::debug!("Ignoring {} from {} because it was not requested from that channel.", &record.package_record.name.as_normalized(), &record.channel);
-                                // Add record to the excluded with reason of being in the non requested channel.
+                                // Add record to the excluded with reason of being in the non
+                                // requested channel.
                                 let message = format!(
                                     "candidate not in requested channel: '{}'",
                                     spec_channel
                                         .name
                                         .clone()
                                         .unwrap_or(spec_channel.base_url.to_string())
                                 );
@@ -280,15 +358,16 @@
                                 continue;
                             }
                         }
                     }
                 }
 
                 // Enforce channel priority
-                // This function makes the assumption that the records are given in order of the channels.
+                // This function makes the assumption that the records are given in order of the
+                // channels.
                 if let (Some(first_channel), ChannelPriority::Strict) = (
                     package_name_found_in_channel
                         .get(&record.package_record.name.as_normalized().to_string()),
                     channel_priority,
                 ) {
                     // Add the record to the excluded list when it is from a different channel.
                     if first_channel != &&record.channel {
@@ -330,21 +409,23 @@
             let name = pool.intern_package_name(locked_record.package_record.name.as_normalized());
             let solvable = pool.intern_solvable(name, SolverPackageRecord::Record(locked_record));
             let candidates = records.entry(name).or_default();
             candidates.candidates.push(solvable);
             candidates.locked = Some(solvable);
         }
 
-        Self {
+        Ok(Self {
             pool,
             records,
             matchspec_to_highest_version: RefCell::default(),
             parse_match_spec_cache: RefCell::default(),
             stop_time,
-        }
+            strategy,
+            direct_dependencies,
+        })
     }
 }
 
 /// The reason why the solver was cancelled
 pub enum CancelReason {
     /// The solver was cancelled because the timeout was reached
     Timeout,
@@ -356,17 +437,37 @@
     }
 
     async fn sort_candidates(
         &self,
         solver: &SolverCache<SolverMatchSpec<'a>, String, Self>,
         solvables: &mut [SolvableId],
     ) {
+        if solvables.is_empty() {
+            // Short circuit if there are no solvables to sort
+            return;
+        }
+
         let mut highest_version_spec = self.matchspec_to_highest_version.borrow_mut();
+
+        let strategy = match self.strategy {
+            SolveStrategy::Highest => CompareStrategy::Default,
+            SolveStrategy::LowestVersion => CompareStrategy::LowestVersion,
+            SolveStrategy::LowestVersionDirect => {
+                if self
+                    .direct_dependencies
+                    .contains(&self.pool.resolve_solvable(solvables[0]).name_id())
+                {
+                    CompareStrategy::LowestVersion
+                } else {
+                    CompareStrategy::Default
+                }
+            }
+        };
         solvables.sort_by(|&p1, &p2| {
-            conda_util::compare_candidates(p1, p2, solver, &mut highest_version_spec)
+            conda_util::compare_candidates(p1, p2, solver, &mut highest_version_spec, strategy)
         });
     }
 
     async fn get_candidates(&self, name: NameId) -> Option<Candidates> {
         self.records.get(&name).cloned()
     }
 
@@ -398,15 +499,16 @@
                 return Some(Box::new(CancelReason::Timeout));
             }
         }
         None
     }
 }
 
-/// Displays the different candidates by their version and sorted by their version
+/// Displays the different candidates by their version and sorted by their
+/// version
 pub struct CondaSolvableDisplay;
 
 impl SolvableDisplay<SolverMatchSpec<'_>> for CondaSolvableDisplay {
     fn display_candidates(
         &self,
         pool: &Pool<SolverMatchSpec<'_>, String>,
         merged_candidates: &[SolvableId],
@@ -445,15 +547,17 @@
             task.available_packages.into_iter().map(|r| r.into()),
             &task.locked_packages,
             &task.pinned_packages,
             &task.virtual_packages,
             task.specs.clone().as_ref(),
             stop_time,
             task.channel_priority,
-        );
+            task.exclude_newer,
+            task.strategy,
+        )?;
         let pool = provider.pool.clone();
 
         // Construct the requirements that the solver needs to satisfy.
         let root_requirements = task
             .specs
             .iter()
             .map(|spec| {
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/backends.rs` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/backends.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+use std::{str::FromStr, time::Instant};
+
+use chrono::{DateTime, Utc};
 use once_cell::sync::Lazy;
 use rattler_conda_types::{
     Channel, ChannelConfig, GenericVirtualPackage, MatchSpec, NoArchType, PackageRecord,
     ParseStrictness, RepoData, RepoDataRecord, Version,
 };
 use rattler_repodata_gateway::sparse::SparseRepoData;
-use rattler_solve::{ChannelPriority, SolveError, SolverImpl, SolverTask};
-use std::str::FromStr;
-use std::time::Instant;
+use rattler_solve::{ChannelPriority, SolveError, SolveStrategy, SolverImpl, SolverTask};
 use url::Url;
 
 fn channel_config() -> ChannelConfig {
     ChannelConfig::default_with_root_dir(std::env::current_dir().unwrap())
 }
 
 fn conda_json_path() -> String {
@@ -102,15 +103,15 @@
             features: None,
             noarch: NoArchType::default(),
             license: None,
             license_family: None,
             timestamp: None,
             legacy_bz2_size: None,
             legacy_bz2_md5: None,
-            purls: Vec::new(),
+            purls: None,
         },
     }
 }
 
 fn solve_real_world<T: SolverImpl + Default>(specs: Vec<&str>) -> Vec<String> {
     let specs = specs
         .iter()
@@ -120,21 +121,16 @@
     let sparse_repo_datas = read_real_world_repo_data();
 
     let names = specs.iter().filter_map(|s| s.name.as_ref().cloned());
     let available_packages =
         SparseRepoData::load_records_recursive(sparse_repo_datas, names, None).unwrap();
 
     let solver_task = SolverTask {
-        available_packages: &available_packages,
         specs: specs.clone(),
-        locked_packages: Vec::default(),
-        pinned_packages: Vec::default(),
-        virtual_packages: Vec::default(),
-        timeout: None,
-        channel_priority: ChannelPriority::Strict,
+        ..SolverTask::from_iter(&available_packages)
     };
 
     let pkgs1 = match T::default().solve(solver_task) {
         Ok(result) => result,
         Err(e) => panic!("{e}"),
     };
 
@@ -147,16 +143,16 @@
                     pkg.package_record.name.as_normalized(),
                     pkg.package_record.version,
                     pkg.package_record.build
                 )
             })
             .collect::<Vec<_>>();
 
-        // The order of packages is nondeterministic, so we sort them to ensure we can compare them
-        // to a previous run
+        // The order of packages is nondeterministic, so we sort them to ensure we can
+        // compare them to a previous run
         pkgs.sort();
         pkgs
     };
 
     extract_pkgs(pkgs1)
 }
 
@@ -200,14 +196,16 @@
         )
         .unwrap()
     });
     &REPO_DATA
 }
 macro_rules! solver_backend_tests {
     ($T:path) => {
+        use chrono::{DateTime, Utc};
+
         #[test]
         fn test_solve_quetz() {
             insta::assert_yaml_snapshot!(solve_real_world::<$T>(vec!["quetz",]));
         }
 
         #[test]
         fn test_solve_xtensor_xsimd() {
@@ -241,124 +239,126 @@
             ]));
         }
 
         #[test]
         fn test_solve_favored() {
             let result = solve::<$T>(
                 dummy_channel_json_path(),
-                vec![installed_package(
-                    "conda-forge",
-                    "linux-64",
-                    "bors",
-                    "1.0",
-                    "bla_1",
-                    1,
-                )],
-                Vec::new(),
-                Vec::new(),
-                &["bors"],
+                SimpleSolveTask {
+                    specs: &["bors"],
+                    installed_packages: vec![installed_package(
+                        "conda-forge",
+                        "linux-64",
+                        "bors",
+                        "1.0",
+                        "bla_1",
+                        1,
+                    )],
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             assert_eq!(result.len(), 1);
             assert_eq!(result[0].package_record.to_string(), "bors=1.0=bla_1");
         }
 
         #[test]
         fn test_solve_with_error() {
             let result = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                Vec::new(),
-                &["foobar >=2", "bors >= 2"],
+                SimpleSolveTask {
+                    specs: &["foobar >=2", "bors >= 2"],
+                    ..SimpleSolveTask::default()
+                },
             );
 
             assert!(result.is_err());
 
             let err = result.err().unwrap();
             insta::assert_snapshot!(err);
         }
 
         #[test]
         fn test_solve_dummy_repo_install_non_existent() {
             let result = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                Vec::new(),
-                &["asdfasdf", "foo<4"],
+                SimpleSolveTask {
+                    specs: &["asdfasdf", "foo<4"],
+                    ..SimpleSolveTask::default()
+                },
             );
 
             assert!(result.is_err());
 
             let err = result.err().unwrap();
             insta::assert_debug_snapshot!(err);
         }
 
         #[test]
         fn test_solve_dummy_repo_missing_virtual_package() {
             let result = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                Vec::new(),
-                &["bar"],
+                SimpleSolveTask {
+                    specs: &["bar"],
+                    ..SimpleSolveTask::default()
+                },
             );
 
             assert!(matches!(result.err(), Some(SolveError::Unsolvable(_))));
         }
 
         #[test]
         fn test_solve_dummy_repo_with_virtual_package() {
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                vec![GenericVirtualPackage {
-                    name: rattler_conda_types::PackageName::new_unchecked("__unix"),
-                    version: Version::from_str("0").unwrap(),
-                    build_string: "0".to_string(),
-                }],
-                &["bar"],
+                SimpleSolveTask {
+                    specs: &["bar"],
+                    virtual_packages: vec![GenericVirtualPackage {
+                        name: rattler_conda_types::PackageName::new_unchecked("__unix"),
+                        version: Version::from_str("0").unwrap(),
+                        build_string: "0".to_string(),
+                    }],
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             assert_eq!(pkgs.len(), 1);
 
             let info = &pkgs[0];
             assert_eq!("bar", info.package_record.name.as_normalized());
             assert_eq!("1.2.3", &info.package_record.version.to_string());
         }
 
         #[test]
         fn test_solve_dummy_repo_install_new() {
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                Vec::new(),
-                &["foo<4"],
+                SimpleSolveTask {
+                    specs: &["foo<4"],
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             assert_eq!(1, pkgs.len());
             let info = &pkgs[0];
 
-            assert_eq!("foo-3.0.2-py36h1af98f8_1.conda", info.file_name);
+            assert_eq!("foo-3.0.2-py36h1af98f8_2.conda", info.file_name);
             assert_eq!(
-                "https://conda.anaconda.org/conda-forge/linux-64/foo-3.0.2-py36h1af98f8_1.conda",
+                "https://conda.anaconda.org/conda-forge/linux-64/foo-3.0.2-py36h1af98f8_2.conda",
                 info.url.to_string()
             );
             assert_eq!("https://conda.anaconda.org/conda-forge/", info.channel);
             assert_eq!("foo", info.package_record.name.as_normalized());
             assert_eq!("linux-64", info.package_record.subdir);
             assert_eq!("3.0.2", info.package_record.version.to_string());
-            assert_eq!("py36h1af98f8_1", info.package_record.build);
-            assert_eq!(1, info.package_record.build_number);
+            assert_eq!("py36h1af98f8_2", info.package_record.build);
+            assert_eq!(2, info.package_record.build_number);
             assert_eq!(
                 rattler_digest::parse_digest_from_hex::<rattler_digest::Sha256>(
                     "67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4"
                 )
                 .as_ref()
                 .unwrap(),
                 info.package_record.sha256.as_ref().unwrap()
@@ -376,18 +376,18 @@
         #[test]
         fn test_solve_dummy_repo_prefers_conda_package() {
             // There following package is provided as .tar.bz and as .conda in repodata.json
             let match_spec = "foo=3.0.2=py36h1af98f8_1";
 
             let operations = solve::<$T>(
                 dummy_channel_json_path(),
-                Vec::new(),
-                Vec::new(),
-                Vec::new(),
-                &[match_spec],
+                SimpleSolveTask {
+                    specs: &[match_spec],
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             // The .conda entry is selected for installing
             assert_eq!(operations.len(), 1);
             assert_eq!(operations[0].file_name, "foo-3.0.2-py36h1af98f8_1.conda");
         }
@@ -401,18 +401,19 @@
                 "3.0.2",
                 "py36h1af98f8_1",
                 1,
             )];
 
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                already_installed,
-                Vec::new(),
-                Vec::new(),
-                &["foo<4"],
+                SimpleSolveTask {
+                    specs: &["foo<4"],
+                    installed_packages: already_installed,
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             assert_eq!(1, pkgs.len());
 
             // Install
             let info = &pkgs[0];
@@ -429,18 +430,19 @@
                 "3.0.2",
                 "py36h1af98f8_1",
                 1,
             )];
 
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                already_installed,
-                Vec::new(),
-                Vec::new(),
-                &["foo>=4"],
+                SimpleSolveTask {
+                    specs: &["foo>=4"],
+                    installed_packages: already_installed,
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             // Install
             let info = &pkgs[0];
             assert_eq!("foo", info.package_record.name.as_normalized());
             assert_eq!("4.0.2", &info.package_record.version.to_string());
@@ -455,18 +457,19 @@
                 "4.0.2",
                 "py36h1af98f8_1",
                 1,
             )];
 
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                already_installed,
-                Vec::new(),
-                Vec::new(),
-                &["foo<4"],
+                SimpleSolveTask {
+                    specs: &["foo<4"],
+                    installed_packages: already_installed,
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             assert_eq!(pkgs.len(), 1);
 
             // Uninstall
             let info = &pkgs[0];
@@ -483,58 +486,101 @@
                 "3.0.2",
                 "py36h1af98f8_1",
                 1,
             )];
 
             let pkgs = solve::<$T>(
                 dummy_channel_json_path(),
-                already_installed,
-                Vec::new(),
-                Vec::new(),
-                &[],
+                SimpleSolveTask {
+                    installed_packages: already_installed,
+                    ..SimpleSolveTask::default()
+                },
             )
             .unwrap();
 
             // Should be no packages!
             assert_eq!(0, pkgs.len());
         }
+
+        #[test]
+        fn test_exclude_newer() {
+            let date = "2021-12-12T12:12:12Z".parse::<DateTime<Utc>>().unwrap();
+
+            let pkgs = solve::<$T>(
+                dummy_channel_json_path(),
+                SimpleSolveTask {
+                    specs: &["foo"],
+                    exclude_newer: Some(date),
+                    ..SimpleSolveTask::default()
+                },
+            )
+            .unwrap();
+
+            assert_eq!(1, pkgs.len());
+
+            let info = &pkgs[0];
+            assert_eq!("foo", info.package_record.name.as_normalized());
+            assert_eq!("3.0.2", &info.package_record.version.to_string(),
+                "although there is a newer version available we expect an older version of foo because we exclude the newer version based on the timestamp");
+            assert_eq!(&info.file_name, "foo-3.0.2-py36h1af98f8_1.tar.bz2", "even though there is a conda version available we expect the tar.bz2 version because we exclude the .conda version based on the timestamp");
+        }
+
+        #[test]
+        fn test_duplicate_record() {
+            use rattler_solve::SolverImpl;
+
+            let mut records = super::read_repodata(&dummy_channel_json_path());
+            records.push(records[0].clone());
+
+            let task = rattler_solve::SolverTask::from_iter([&records]);
+
+            let result = <$T>::default().solve(task);
+            match result {
+               Err(rattler_solve::SolveError::DuplicateRecords(_)) => {},
+                _ => panic!("expected a DuplicateRecord error"),
+            }
+        }
     };
 }
 
 #[cfg(feature = "libsolv_c")]
 mod libsolv_c {
+    #![allow(unused_imports)] // For some reason windows thinks this is an unused import.
+
+    use rattler_solve::{ChannelPriority, SolveStrategy};
+
     use super::{
         dummy_channel_json_path, installed_package, solve, solve_real_world, FromStr,
-        GenericVirtualPackage, SolveError, Version,
+        GenericVirtualPackage, SimpleSolveTask, SolveError, Version,
     };
-    #[allow(unused_imports)] // For some reason windows thinks this is an unused import.
-    use rattler_solve::ChannelPriority;
 
     solver_backend_tests!(rattler_solve::libsolv_c::Solver);
 
     #[test]
     #[cfg(target_family = "unix")]
     fn test_solve_with_cached_solv_file_install_new() {
-        use super::read_repodata;
         use rattler_conda_types::{Channel, ChannelConfig, MatchSpec};
         use rattler_solve::{SolverImpl, SolverTask};
 
+        use super::read_repodata;
+
         let repo_data = read_repodata(&dummy_channel_json_path());
 
         let cached_repo_data = rattler_solve::libsolv_c::cache_repodata(
             Channel::from_str(
                 "conda-forge",
                 &ChannelConfig::default_with_root_dir(std::env::current_dir().unwrap()),
             )
             .unwrap()
             .platform_url(rattler_conda_types::Platform::Linux64)
             .to_string(),
             &repo_data,
             None,
-        );
+        )
+        .unwrap();
 
         let libsolv_repodata = rattler_solve::libsolv_c::RepoData {
             records: repo_data.iter().collect(),
             solv_file: Some(&cached_repo_data),
         };
 
         let specs: Vec<MatchSpec> = vec!["foo<4".parse().unwrap()];
@@ -543,36 +589,38 @@
             .solve(SolverTask {
                 locked_packages: Vec::new(),
                 virtual_packages: Vec::new(),
                 available_packages: [libsolv_repodata],
                 specs,
                 pinned_packages: Vec::new(),
                 timeout: None,
-                channel_priority: ChannelPriority::Strict,
+                channel_priority: ChannelPriority::default(),
+                exclude_newer: None,
+                strategy: SolveStrategy::default(),
             })
             .unwrap();
 
         if pkgs.is_empty() {
             println!("No packages in the environment!");
         }
 
         assert_eq!(1, pkgs.len());
         let info = &pkgs[0];
 
-        assert_eq!("foo-3.0.2-py36h1af98f8_1.conda", info.file_name);
+        assert_eq!("foo-3.0.2-py36h1af98f8_2.conda", info.file_name);
         assert_eq!(
-            "https://conda.anaconda.org/conda-forge/linux-64/foo-3.0.2-py36h1af98f8_1.conda",
+            "https://conda.anaconda.org/conda-forge/linux-64/foo-3.0.2-py36h1af98f8_2.conda",
             info.url.to_string()
         );
         assert_eq!("https://conda.anaconda.org/conda-forge/", info.channel);
         assert_eq!("foo", info.package_record.name.as_normalized());
         assert_eq!("linux-64", info.package_record.subdir);
         assert_eq!("3.0.2", info.package_record.version.to_string());
-        assert_eq!("py36h1af98f8_1", info.package_record.build);
-        assert_eq!(1, info.package_record.build_number);
+        assert_eq!("py36h1af98f8_2", info.package_record.build);
+        assert_eq!(2, info.package_record.build_number);
         assert_eq!(
             rattler_digest::parse_digest_from_hex::<rattler_digest::Sha256>(
                 "67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4"
             )
             .as_ref()
             .unwrap(),
             info.package_record.sha256.as_ref().unwrap()
@@ -588,76 +636,188 @@
     }
 }
 
 #[cfg(feature = "resolvo")]
 mod resolvo {
     use super::{
         dummy_channel_json_path, installed_package, solve, solve_real_world, FromStr,
-        GenericVirtualPackage, SolveError, Version,
+        GenericVirtualPackage, SimpleSolveTask, SolveError, Version,
     };
 
     solver_backend_tests!(rattler_solve::resolvo::Solver);
 
     #[test]
     fn test_solve_locked() {
         let result = solve::<rattler_solve::resolvo::Solver>(
             dummy_channel_json_path(),
-            Vec::new(),
-            vec![installed_package(
-                "conda-forge",
-                "linux-64",
-                "bors",
-                "1.0",
-                "bla_1",
-                1,
-            )],
-            Vec::new(),
-            &["bors >=2"],
+            SimpleSolveTask {
+                specs: &["bors >=2"],
+                pinned_packages: vec![installed_package(
+                    "conda-forge",
+                    "linux-64",
+                    "bors",
+                    "1.0",
+                    "bla_1",
+                    1,
+                )],
+                ..SimpleSolveTask::default()
+            },
+        );
+
+        // We expect an error here. `bors` is pinnend to 1, but we try to install `>=2`.
+        insta::assert_snapshot!(result.unwrap_err());
+    }
+
+    #[test]
+    fn test_exclude_newer_error() {
+        let date = "2021-12-12T12:12:12Z".parse::<DateTime<Utc>>().unwrap();
+
+        let result = solve::<rattler_solve::resolvo::Solver>(
+            dummy_channel_json_path(),
+            SimpleSolveTask {
+                specs: &["foo>=4"],
+                exclude_newer: Some(date),
+                ..SimpleSolveTask::default()
+            },
         );
 
         // We expect an error here. `bors` is pinnend to 1, but we try to install `>=2`.
         insta::assert_snapshot!(result.unwrap_err());
     }
+
+    #[test]
+    fn test_lowest_version_strategy_highest_build_number() {
+        let result = solve::<rattler_solve::resolvo::Solver>(
+            dummy_channel_json_path(),
+            SimpleSolveTask {
+                specs: &["foo"],
+                strategy: rattler_solve::SolveStrategy::LowestVersion,
+                ..SimpleSolveTask::default()
+            },
+        )
+        .unwrap();
+
+        assert_eq!(result.len(), 1);
+        assert_eq!(
+            result[0].package_record.version,
+            Version::from_str("3.0.2").unwrap()
+        );
+        assert_eq!(
+            result[0].package_record.build_number, 2,
+            "expected the highest build number"
+        );
+    }
+
+    #[test]
+    fn test_lowest_version_strategy_all() {
+        let result = solve::<rattler_solve::resolvo::Solver>(
+            dummy_channel_json_path(),
+            SimpleSolveTask {
+                specs: &["foobar"],
+                strategy: rattler_solve::SolveStrategy::LowestVersion,
+                ..SimpleSolveTask::default()
+            },
+        )
+        .unwrap();
+
+        assert_eq!(result.len(), 2);
+        assert_eq!(result[0].package_record.name.as_normalized(), "foobar");
+        assert_eq!(
+            result[0].package_record.version,
+            Version::from_str("2.0").unwrap(),
+            "expected lowest version of foobar"
+        );
+
+        assert_eq!(result[1].package_record.name.as_normalized(), "bors");
+        assert_eq!(
+            result[1].package_record.version,
+            Version::from_str("1.0").unwrap(),
+            "expected lowest version of bors"
+        );
+    }
+
+    #[test]
+    fn test_lowest_direct_version_strategy() {
+        let result = solve::<rattler_solve::resolvo::Solver>(
+            dummy_channel_json_path(),
+            SimpleSolveTask {
+                specs: &["foobar"],
+                strategy: rattler_solve::SolveStrategy::LowestVersionDirect,
+                ..SimpleSolveTask::default()
+            },
+        )
+        .unwrap();
+
+        assert_eq!(result.len(), 2);
+        assert_eq!(result[0].package_record.name.as_normalized(), "foobar");
+        assert_eq!(
+            result[0].package_record.version,
+            Version::from_str("2.0").unwrap(),
+            "expected lowest version of foobar"
+        );
+
+        assert_eq!(result[1].package_record.name.as_normalized(), "bors");
+        assert_eq!(
+            result[1].package_record.version,
+            Version::from_str("1.2.1").unwrap(),
+            "expected highest compatible version of bors"
+        );
+    }
 }
 
-fn solve<T: SolverImpl + Default>(
-    repo_path: String,
+#[derive(Default)]
+struct SimpleSolveTask<'a> {
+    specs: &'a [&'a str],
     installed_packages: Vec<RepoDataRecord>,
     pinned_packages: Vec<RepoDataRecord>,
     virtual_packages: Vec<GenericVirtualPackage>,
-    match_specs: &[&str],
+    exclude_newer: Option<DateTime<Utc>>,
+    strategy: SolveStrategy,
+}
+
+fn solve<T: SolverImpl + Default>(
+    repo_path: String,
+    task: SimpleSolveTask<'_>,
 ) -> Result<Vec<RepoDataRecord>, SolveError> {
     let repo_data = read_repodata(&repo_path);
 
-    let specs: Vec<_> = match_specs
+    let specs: Vec<_> = task
+        .specs
         .iter()
         .map(|m| MatchSpec::from_str(m, ParseStrictness::Lenient).unwrap())
         .collect();
 
     let task = SolverTask {
-        locked_packages: installed_packages,
-        virtual_packages,
-        available_packages: [&repo_data],
+        locked_packages: task.installed_packages,
+        virtual_packages: task.virtual_packages,
         specs,
-        pinned_packages,
-        timeout: None,
-        channel_priority: ChannelPriority::Strict,
+        pinned_packages: task.pinned_packages,
+        exclude_newer: task.exclude_newer,
+        strategy: task.strategy,
+        ..SolverTask::from_iter([&repo_data])
     };
 
     let pkgs = T::default().solve(task)?;
 
     if pkgs.is_empty() {
         println!("No packages in the environment!");
     }
 
     Ok(pkgs)
 }
 
-fn compare_solve(specs: Vec<&str>) {
-    let specs = specs
+#[derive(Default)]
+struct CompareTask<'a> {
+    specs: Vec<&'a str>,
+    exclude_newer: Option<DateTime<Utc>>,
+}
+
+fn compare_solve(task: CompareTask<'_>) {
+    let specs = task
+        .specs
         .iter()
         .map(|s| MatchSpec::from_str(s, ParseStrictness::Lenient).unwrap())
         .collect::<Vec<_>>();
 
     let sparse_repo_datas = read_real_world_repo_data();
 
     let names = specs.iter().filter_map(|s| s.name.as_ref().cloned());
@@ -673,37 +833,33 @@
                     pkg.package_record.name.as_normalized(),
                     pkg.package_record.version,
                     pkg.package_record.build
                 )
             })
             .collect::<Vec<_>>();
 
-        // The order of packages is nondeterministic, so we sort them to ensure we can compare them
-        // to a previous run
+        // The order of packages is nondeterministic, so we sort them to ensure we can
+        // compare them to a previous run
         pkgs.sort();
         pkgs
     };
 
     let mut results = Vec::new();
 
     #[cfg(feature = "libsolv_c")]
     {
         let start_solve = Instant::now();
         results.push((
             "libsolv_c",
             extract_pkgs(
                 rattler_solve::libsolv_c::Solver
                     .solve(SolverTask {
-                        available_packages: &available_packages,
                         specs: specs.clone(),
-                        locked_packages: Vec::default(),
-                        pinned_packages: Vec::default(),
-                        virtual_packages: Vec::default(),
-                        timeout: None,
-                        channel_priority: ChannelPriority::Strict,
+                        exclude_newer: task.exclude_newer,
+                        ..SolverTask::from_iter(&available_packages)
                     })
                     .unwrap(),
             ),
         ));
         let end_solve = Instant::now();
         println!("libsolv_c took {}ms", (end_solve - start_solve).as_millis());
     }
@@ -712,21 +868,17 @@
     {
         let start_solve = Instant::now();
         results.push((
             "resolvo",
             extract_pkgs(
                 rattler_solve::resolvo::Solver
                     .solve(SolverTask {
-                        available_packages: &available_packages,
                         specs: specs.clone(),
-                        locked_packages: Vec::default(),
-                        pinned_packages: Vec::default(),
-                        virtual_packages: Vec::default(),
-                        timeout: None,
-                        channel_priority: ChannelPriority::Strict,
+                        exclude_newer: task.exclude_newer,
+                        ..SolverTask::from_iter(&available_packages)
                     })
                     .unwrap(),
             ),
         ));
         let end_solve = Instant::now();
         println!("resolvo took {}ms", (end_solve - start_solve).as_millis());
     }
@@ -747,35 +899,50 @@
 
         Some(current)
     });
 }
 
 #[test]
 fn compare_solve_tensorboard() {
-    compare_solve(vec!["tensorboard=2.1.1", "grpc-cpp=1.39.1"]);
+    compare_solve(CompareTask {
+        specs: vec!["tensorboard=2.1.1", "grpc-cpp=1.39.1"],
+        ..CompareTask::default()
+    });
 }
 
 #[test]
 fn compare_solve_python() {
-    compare_solve(vec!["python=3.9"]);
+    compare_solve(CompareTask {
+        specs: vec!["python=3.9"],
+        ..CompareTask::default()
+    });
 }
 
 #[test]
 fn compare_solve_tensorflow() {
-    compare_solve(vec!["tensorflow"]);
+    compare_solve(CompareTask {
+        specs: vec!["tensorflow"],
+        ..CompareTask::default()
+    });
 }
 
 #[test]
 fn compare_solve_quetz() {
-    compare_solve(vec!["quetz"]);
+    compare_solve(CompareTask {
+        specs: vec!["quetz"],
+        ..CompareTask::default()
+    });
 }
 
 #[test]
 fn compare_solve_xtensor_xsimd() {
-    compare_solve(vec!["xtensor", "xsimd"]);
+    compare_solve(CompareTask {
+        specs: vec!["xtensor", "xsimd"],
+        ..CompareTask::default()
+    });
 }
 
 fn solve_to_get_channel_of_spec(
     spec_str: &str,
     expected_channel: &str,
     repo_data: Vec<&SparseRepoData>,
     channel_priority: ChannelPriority,
@@ -784,38 +951,24 @@
     let spec = MatchSpec::from_str(spec_str, ParseStrictness::Lenient).unwrap();
     let specs = vec![spec.clone()];
     let names = specs.iter().filter_map(|s| s.name.as_ref().cloned());
 
     let available_packages =
         SparseRepoData::load_records_recursive(repo_data, names, None).unwrap();
 
+    let task = SolverTask {
+        specs: specs.clone(),
+        channel_priority,
+        ..SolverTask::from_iter(&available_packages)
+    };
+
     let result = if use_resolvo {
-        rattler_solve::resolvo::Solver
-            .solve(SolverTask {
-                available_packages: &available_packages,
-                specs: specs.clone(),
-                locked_packages: Vec::default(),
-                pinned_packages: Vec::default(),
-                virtual_packages: Vec::default(),
-                timeout: None,
-                channel_priority,
-            })
-            .unwrap()
+        rattler_solve::resolvo::Solver.solve(task).unwrap()
     } else {
-        rattler_solve::libsolv_c::Solver
-            .solve(SolverTask {
-                available_packages: &available_packages,
-                specs: specs.clone(),
-                locked_packages: Vec::default(),
-                pinned_packages: Vec::default(),
-                virtual_packages: Vec::default(),
-                timeout: None,
-                channel_priority,
-            })
-            .unwrap()
+        rattler_solve::libsolv_c::Solver.solve(task).unwrap()
     };
 
     let record = result.iter().find(|record| {
         record.package_record.name.as_normalized() == spec.name.as_ref().unwrap().as_normalized()
     });
     assert_eq!(record.unwrap().channel, expected_channel.to_string());
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__libsolv_c__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_python_numpy.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_quetz.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorboard.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_tensorflow.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap` & `py_rattler-0.6.0/local_dependencies/rattler_solve/tests/snapshots/backends__resolvo__solve_with_error.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_networking/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "rattler_networking"
-version = "0.20.3"
+version = "0.20.8"
 edition= "2021"
 authors = ["Wolf Vollprecht <w.vollprecht@gmail.com>"]
 description = "Authenticated requests in the conda ecosystem"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
@@ -16,30 +16,33 @@
 native-tls = ['reqwest/native-tls', "google-cloud-auth?/default-tls"]
 rustls-tls = ['reqwest/rustls-tls', "google-cloud-auth?/rustls-tls"]
 
 [dependencies]
 anyhow = "1.0.82"
 async-trait = "0.1.80"
 base64 = "0.22.0"
+bytes = "1.6.0"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 dirs = "5.0.1"
 fslock = "0.2.1"
+futures = "0.3.30"
+google-cloud-auth = { version = "0.13.2", default-features = false , optional = true }
 http = "1.1"
 itertools = "0.12.1"
 keyring = "2.3.2"
 netrc-rs = "0.1.2"
+pin-project-lite = "0.2.14"
 reqwest = { version = "0.12.3", default-features = false , features = ["json"] }
 reqwest-middleware = "0.3.0"
 retry-policies = { version = "0.3.0", default-features = false }
 serde = { version = "1.0.198" , features = ["derive"] }
 serde_json = { version = "1.0.116" }
 thiserror = "1.0"
 tracing = "0.1.40"
 url = { version = "2.5.0" }
-google-cloud-auth = { version = "0.13.2", default-features = false, optional = true }
 
 [target.'cfg( target_arch = "wasm32" )'.dependencies]
 getrandom = { version = "0.2.14", default-features = false , features = ["js"] }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_networking/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,43 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.8](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.7...rattler_networking-v0.20.8) - 2024-05-27
+
+### Other
+- introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
+
+## [0.20.7](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.6...rattler_networking-v0.20.7) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.20.6](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.5...rattler_networking-v0.20.6) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+- add AuthenticationStorage::from_file() ([#645](https://github.com/mamba-org/rattler/pull/645))
+
+### Other
+- update README.md
+
+## [0.20.5](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.4...rattler_networking-v0.20.5) - 2024-05-06
+
+### Added
+- respect `RATTLER_AUTH_FILE` when using AuthenticationStorage::default() ([#636](https://github.com/mamba-org/rattler/pull/636))
+
+## [0.20.4](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.3...rattler_networking-v0.20.4) - 2024-04-30
+
+### Other
+- bump py-rattler 0.5.0 ([#629](https://github.com/mamba-org/rattler/pull/629))
+
 ## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.2...rattler_networking-v0.20.3) - 2024-04-25
 
 ### Added
 - Add GCS support for rattler auth ([#605](https://github.com/mamba-org/rattler/pull/605))
 
 ## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_networking-v0.20.1...rattler_networking-v0.20.2) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_middleware.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_middleware.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 use base64::prelude::BASE64_STANDARD;
 use base64::Engine;
 use reqwest::{Request, Response};
 use reqwest_middleware::{Middleware, Next};
 use std::path::{Path, PathBuf};
 use std::sync::OnceLock;
 use url::Url;
+
 /// `reqwest` middleware to authenticate requests
 #[derive(Clone, Default)]
 pub struct AuthenticationMiddleware {
     auth_storage: AuthenticationStorage,
 }
 
 #[async_trait]
 impl Middleware for AuthenticationMiddleware {
     async fn handle(
         &self,
         req: Request,
         extensions: &mut http::Extensions,
         next: Next<'_>,
     ) -> reqwest_middleware::Result<Response> {
-        let url = req.url().clone();
+        // If an `Authorization` header is already present, don't authenticate
+        if req.headers().get(reqwest::header::AUTHORIZATION).is_some() {
+            return next.run(req, extensions).await;
+        }
 
+        let url = req.url().clone();
         match self.auth_storage.get_by_url(url) {
             Err(_) => {
                 // Forward error to caller (invalid URL)
                 next.run(req, extensions).await
             }
             Ok((url, auth)) => {
                 let url = Self::authenticate_url(url, &auth);
@@ -395,8 +400,37 @@
             } else {
                 assert_eq!(retrieved.1, None);
             }
         }
 
         Ok(())
     }
+
+    #[test]
+    fn test_rattler_auth_file_env_var_handling() -> anyhow::Result<()> {
+        let tdir = tempdir()?;
+
+        let storage = temp_env::with_var(
+            "RATTLER_AUTH_FILE",
+            Some(
+                tdir.path()
+                    .to_path_buf()
+                    .join("auth.json")
+                    .to_str()
+                    .unwrap(),
+            ),
+            || AuthenticationStorage::from_env().unwrap(),
+        );
+
+        let host = "test.example.com";
+        let authentication = Authentication::CondaToken("testtoken".to_string());
+        storage.store(host, &authentication)?;
+
+        let file = tdir.path().join("auth.json");
+        assert_eq!(
+            std::fs::read_to_string(file)?,
+            "{\"test.example.com\":{\"CondaToken\":\"testtoken\"}}"
+        );
+
+        Ok(())
+    }
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/authentication.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/file.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/keyring.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/backends/netrc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/authentication_storage/storage.rs`

 * *Files 14% similar despite different names*

```diff
@@ -47,14 +47,48 @@
     pub fn new() -> Self {
         Self {
             backends: vec![],
             cache: Arc::new(Mutex::new(HashMap::new())),
         }
     }
 
+    /// Create a new authentication storage with the default backends
+    /// respecting the `RATTLER_AUTH_FILE` environment variable.
+    /// If the variable is set, the file storage backend will be used
+    /// with the path specified in the variable
+    pub fn from_env() -> Result<Self> {
+        if let Ok(auth_file) = std::env::var("RATTLER_AUTH_FILE") {
+            let path = std::path::Path::new(&auth_file);
+
+            tracing::info!(
+                "\"RATTLER_AUTH_FILE\" environment variable set, using file storage at {}",
+                auth_file
+            );
+
+            Ok(Self::from_file(path)?)
+        } else {
+            Ok(Self::default())
+        }
+    }
+
+    /// Create a new authentication storage with just a file storage backend
+    pub fn from_file(path: &std::path::Path) -> Result<Self> {
+        let mut storage = Self::new();
+        let backend = FileStorage::new(path.to_path_buf()).map_err(|e| {
+            anyhow!(
+                "Error creating file storage backend from file ({}): {}",
+                path.display(),
+                e
+            )
+        })?;
+
+        storage.add_backend(Arc::from(backend));
+        Ok(storage)
+    }
+
     /// Add a new storage backend to the authentication storage
     /// (backends are tried in the order they are added)
     pub fn add_backend(&mut self, backend: Arc<dyn StorageBackend + Send + Sync>) {
         self.backends.push(backend);
     }
 
     /// Store the given authentication information for the given host
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/gcs_middleware.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/gcs_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/mirror_middleware.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/mirror_middleware.rs`

 * *Files 0% similar despite different names*

```diff
@@ -195,18 +195,18 @@
         StatusCode::INTERNAL_SERVER_ERROR
     }
 
     async fn test_server(name: &str, broken: bool) -> Url {
         let state = String::from(name);
 
         // Construct a router that returns data from the static dir but fails the first try.
-        let router = if !broken {
-            Router::new().route("/count", get(count)).with_state(state)
-        } else {
+        let router = if broken {
             Router::new().route("/count", get(broken_return))
+        } else {
+            Router::new().route("/count", get(count)).with_state(state)
         };
 
         let addr = SocketAddr::new([127, 0, 0, 1].into(), 0);
         let listener = tokio::net::TcpListener::bind(&addr).await.unwrap();
         let addr = listener.local_addr().unwrap();
 
         let service = router.into_make_service();
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/oci_middleware.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/oci_middleware.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/redaction.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/redaction.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_networking/src/retry_policies.rs` & `py_rattler-0.6.0/local_dependencies/rattler_networking/src/retry_policies.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_virtual_packages"
-version = "0.19.8"
+version = "0.19.12"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
 description = "Library to work with and detect Conda virtual packages"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
 libloading = "0.8.3"
 nom = "7.1.3"
 once_cell = "1.19.0"
 regex = "1.10.4"
 serde = { version = "1.0.198" , features = ["derive"] }
 thiserror = "1.0"
 tracing = "0.1.40"
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.12](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.11...rattler_virtual_packages-v0.19.12) - 2024-05-27
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.19.11](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.10...rattler_virtual_packages-v0.19.11) - 2024-05-14
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.19.10](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.9...rattler_virtual_packages-v0.19.10) - 2024-05-13
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.19.9](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.8...rattler_virtual_packages-v0.19.9) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.19.8](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.7...rattler_virtual_packages-v0.19.8) - 2024-04-25
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.19.7](https://github.com/mamba-org/rattler/compare/rattler_virtual_packages-v0.19.6...rattler_virtual_packages-v0.19.7) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/cuda.rs` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/cuda.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/libc.rs` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/libc.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/linux.rs` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/linux.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_virtual_packages/src/osx.rs` & `py_rattler-0.6.0/local_dependencies/rattler_virtual_packages/src/osx.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_index/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_index/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "rattler_index"
-version = "0.19.8"
+version = "0.19.13"
 edition= "2021"
 authors = []
 description = "A crate that indexes directories containing conda packages to create local conda channels"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false }
-rattler_package_streaming = { path= "../rattler_package_streaming", version = "0.20.6", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_digest = { path= "../rattler_digest", version = "0.19.4", default-features = false }
+rattler_package_streaming = { path= "../rattler_package_streaming", version = "0.21.0", default-features = false }
 fs-err = "2.11.0"
 serde_json = { version = "1.0.116" }
 tracing = "0.1.40"
 walkdir = "2.5.0"
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_index/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_index/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,39 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.19.13](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.12...rattler_index-v0.19.13) - 2024-05-27
+
+### Added
+- always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
+
+## [0.19.12](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.11...rattler_index-v0.19.12) - 2024-05-14
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_package_streaming
+
+## [0.19.11](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.10...rattler_index-v0.19.11) - 2024-05-13
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_digest, rattler_package_streaming
+
+## [0.19.10](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.9...rattler_index-v0.19.10) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.19.9](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.8...rattler_index-v0.19.9) - 2024-04-30
+
+### Other
+- release ([#625](https://github.com/mamba-org/rattler/pull/625))
+
 ## [0.19.8](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.7...rattler_index-v0.19.8) - 2024-04-25
 
 ### Other
 - updated the following local packages: rattler_conda_types
 
 ## [0.19.7](https://github.com/mamba-org/rattler/compare/rattler_index-v0.19.6...rattler_index-v0.19.7) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_index/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_index/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         features: index.features,
         noarch: index.noarch,
         license: index.license,
         license_family: index.license_family,
         timestamp: index.timestamp,
         legacy_bz2_md5: None,
         legacy_bz2_size: None,
-        purls: Vec::default(),
+        purls: None,
     };
     Ok(package_record)
 }
 
 fn package_record_from_tar_bz2(file: &Path) -> Result<PackageRecord, std::io::Error> {
     let reader = std::fs::File::open(file)?;
     let mut archive = read::stream_tar_bz2(reader);
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_index/tests/test_index.rs` & `py_rattler-0.6.0/local_dependencies/rattler_index/tests/test_index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/build.rs` & `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/build.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_libsolv_c/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_libsolv_c/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 [package]
-name = "rattler_lock"
-version = "0.22.3"
+name = "rattler_conda_types"
+version = "0.24.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
-description = "Rust data types for conda lock"
+description = "Rust data types for common types used within the Conda ecosystem"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false }
+file_url = { path = "../file_url", version = "0.1.1" }
+rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false, features = ["serde"] }
+rattler_macros = { path = "../rattler_macros", version = "0.19.3", default-features = false }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 fxhash = "0.2.1"
-indexmap = { version = "2.2.6", features = ["serde"] }
+glob = "0.3.1"
+hex = "0.4.3"
 itertools = "0.12.1"
-pep508_rs = { version = "0.4.2" , features = ["serde"] }
-pep440_rs = { version = "0.5.0" , features = ["serde"] }
-serde = { version = "1.0.198" , features = ["derive"] }
+lazy-regex = "3.1.0"
+nom = "7.1.3"
+purl = { version = "0.1.2", features = ["serde","serde"] }
+regex = "1.10.4"
+serde = { version = "1.0.198" , features = ["derive", "rc"] }
 serde_json = { version = "1.0.116" }
-serde_yaml = "0.9.34"
+serde_repr = "0.1"
 serde_with = { version = "3.7.0", features = ["indexmap_2"] }
+smallvec = { version = "1.13.2", features = [
+    "serde",
+    "const_new",
+    "const_generics",
+    "union","serde", "const_new", "const_generics", "union",
+] }
+strum = { version = "0.26.2", features = ["derive","derive"] }
 thiserror = "1.0"
+tracing = "0.1.40"
+typed-path = { version = "0.8.0" }
 url = { version = "2.5.0" , features = ["serde"] }
-purl = { version = "0.1.2", features = ["serde","serde"] }
-percent-encoding = "2.3.1"
+
+[[bench]]
+name = "parse"
+harness = false
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_lock/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,43 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.22.8](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.7...rattler_lock-v0.22.8) - 2024-05-27
+
+### Added
+- removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
+- always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
+
+## [0.22.7](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.6...rattler_lock-v0.22.7) - 2024-05-14
+
+### Other
+- bump pep crates ([#661](https://github.com/mamba-org/rattler/pull/661))
+
+## [0.22.6](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.5...rattler_lock-v0.22.6) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Other
+- update README.md
+
+## [0.22.5](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.4...rattler_lock-v0.22.5) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.22.4](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.3...rattler_lock-v0.22.4) - 2024-04-30
+
+### Added
+- adds pypi indexes to the lock-file ([#626](https://github.com/mamba-org/rattler/pull/626))
+
 ## [0.22.3](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.2...rattler_lock-v0.22.3) - 2024-04-25
 
 ### Fixed
 - compare `UrlOrPath` ([#618](https://github.com/mamba-org/rattler/pull/618))
 - parse absolute paths on Windows correctly in lockfiles ([#616](https://github.com/mamba-org/rattler/pull/616))
 
 ## [0.22.2](https://github.com/mamba-org/rattler/compare/rattler_lock-v0.22.1...rattler_lock-v0.22.2) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/builder.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/builder.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 //! Builder for the creation of lock files.
 
-use crate::{
-    Channel, CondaPackageData, EnvironmentData, EnvironmentPackageData, LockFile, LockFileInner,
-    PypiPackageData, PypiPackageEnvironmentData,
+use std::{
+    collections::{BTreeSet, HashMap},
+    sync::Arc,
 };
+
 use fxhash::FxHashMap;
 use indexmap::{IndexMap, IndexSet};
 use pep508_rs::ExtraName;
 use rattler_conda_types::Platform;
-use std::{
-    collections::{BTreeSet, HashMap},
-    sync::Arc,
+
+use crate::{
+    file_format_version::FileFormatVersion, Channel, CondaPackageData, EnvironmentData,
+    EnvironmentPackageData, LockFile, LockFileInner, Package, PypiIndexes, PypiPackageData,
+    PypiPackageEnvironmentData,
 };
 
 /// A struct to incrementally build a lock-file.
 #[derive(Default)]
 pub struct LockFileBuilder {
     /// Metadata about the different environments stored in the lock file.
     environments: IndexMap<String, EnvironmentData>,
@@ -27,48 +30,67 @@
 
 impl LockFileBuilder {
     /// Generate a new lock file using the builder pattern
     pub fn new() -> Self {
         Self::default()
     }
 
+    /// Sets the pypi indexes for an environment.
+    pub fn set_pypi_indexes(
+        &mut self,
+        environment_data: impl Into<String>,
+        indexes: PypiIndexes,
+    ) -> &mut Self {
+        self.environments
+            .entry(environment_data.into())
+            .or_insert_with(|| EnvironmentData {
+                channels: vec![],
+                packages: FxHashMap::default(),
+                indexes: None,
+            })
+            .indexes = Some(indexes);
+        self
+    }
+
     /// Sets the metadata for an environment.
     pub fn set_channels(
         &mut self,
         environment: impl Into<String>,
         channels: impl IntoIterator<Item = impl Into<Channel>>,
     ) -> &mut Self {
         self.environments
             .entry(environment.into())
             .or_insert_with(|| EnvironmentData {
                 channels: vec![],
                 packages: FxHashMap::default(),
+                indexes: None,
             })
             .channels = channels.into_iter().map(Into::into).collect();
         self
     }
 
     /// Adds a conda locked package to a specific environment and platform.
     ///
-    /// This function is similar to [`Self::with_conda_package`] but differs in that it takes a
-    /// mutable reference to self instead of consuming it. This allows for a more fluent with
-    /// chaining calls.
+    /// This function is similar to [`Self::with_conda_package`] but differs in
+    /// that it takes a mutable reference to self instead of consuming it.
+    /// This allows for a more fluent with chaining calls.
     pub fn add_conda_package(
         &mut self,
         environment: impl Into<String>,
         platform: Platform,
         locked_package: CondaPackageData,
     ) -> &mut Self {
         // Get the environment
         let environment = self
             .environments
             .entry(environment.into())
             .or_insert_with(|| EnvironmentData {
                 channels: vec![],
                 packages: HashMap::default(),
+                indexes: None,
             });
 
         // Add the package to the list of packages.
         let package_idx = self.conda_packages.insert_full(locked_package).0;
 
         // Add the package to the environment that it is intended for.
         environment
@@ -78,31 +100,32 @@
             .push(EnvironmentPackageData::Conda(package_idx));
 
         self
     }
 
     /// Adds a pypi locked package to a specific environment and platform.
     ///
-    /// This function is similar to [`Self::with_pypi_package`] but differs in that it takes a
-    /// mutable reference to self instead of consuming it. This allows for a more fluent with
-    /// chaining calls.
+    /// This function is similar to [`Self::with_pypi_package`] but differs in
+    /// that it takes a mutable reference to self instead of consuming it.
+    /// This allows for a more fluent with chaining calls.
     pub fn add_pypi_package(
         &mut self,
         environment: impl Into<String>,
         platform: Platform,
         locked_package: PypiPackageData,
         environment_data: PypiPackageEnvironmentData,
     ) -> &mut Self {
         // Get the environment
         let environment = self
             .environments
             .entry(environment.into())
             .or_insert_with(|| EnvironmentData {
                 channels: vec![],
                 packages: HashMap::default(),
+                indexes: None,
             });
 
         // Add the package to the list of packages.
         let package_idx = self.pypi_packages.insert_full(locked_package).0;
         let runtime_idx = self
             .pypi_runtime_configurations
             .insert_full(environment_data.into())
@@ -116,32 +139,65 @@
             .push(EnvironmentPackageData::Pypi(package_idx, runtime_idx));
 
         self
     }
 
     /// Adds a conda locked package to a specific environment and platform.
     ///
-    /// This function is similar to [`Self::add_conda_package`] but differs in that it consumes
-    /// `self` instead of taking a mutable reference. This allows for a better interface when
-    /// modifying an existing instance.
+    /// This function is similar to [`Self::add_conda_package`] but differs in
+    /// that it consumes `self` instead of taking a mutable reference. This
+    /// allows for a better interface when modifying an existing instance.
     pub fn with_conda_package(
         mut self,
         environment: impl Into<String>,
         platform: Platform,
         locked_package: CondaPackageData,
     ) -> Self {
         self.add_conda_package(environment, platform, locked_package);
         self
     }
 
+    /// Adds a package from another environment to a specific environment and
+    /// platform.
+    pub fn with_package(
+        mut self,
+        environment: impl Into<String>,
+        platform: Platform,
+        locked_package: Package,
+    ) -> Self {
+        self.add_package(environment, platform, locked_package);
+        self
+    }
+
+    /// Adds a package from another environment to a specific environment and
+    /// platform.
+    pub fn add_package(
+        &mut self,
+        environment: impl Into<String>,
+        platform: Platform,
+        locked_package: Package,
+    ) -> &mut Self {
+        match locked_package {
+            Package::Conda(p) => {
+                self.add_conda_package(environment, platform, p.package_data().clone())
+            }
+            Package::Pypi(p) => self.add_pypi_package(
+                environment,
+                platform,
+                p.package_data().clone(),
+                p.environment_data().clone(),
+            ),
+        }
+    }
+
     /// Adds a pypi locked package to a specific environment and platform.
     ///
-    /// This function is similar to [`Self::add_pypi_package`] but differs in that it consumes
-    /// `self` instead of taking a mutable reference. This allows for a better interface when
-    /// modifying an existing instance.
+    /// This function is similar to [`Self::add_pypi_package`] but differs in
+    /// that it consumes `self` instead of taking a mutable reference. This
+    /// allows for a better interface when modifying an existing instance.
     pub fn with_pypi_package(
         mut self,
         environment: impl Into<String>,
         platform: Platform,
         locked_package: PypiPackageData,
         environment_data: PypiPackageEnvironmentData,
     ) -> Self {
@@ -155,25 +211,36 @@
         environment: impl Into<String>,
         channels: impl IntoIterator<Item = impl Into<Channel>>,
     ) -> Self {
         self.set_channels(environment, channels);
         self
     }
 
+    /// Sets the channels of an environment.
+    pub fn with_pypi_indexes(
+        mut self,
+        environment: impl Into<String>,
+        indexes: PypiIndexes,
+    ) -> Self {
+        self.set_pypi_indexes(environment, indexes);
+        self
+    }
+
     /// Build a [`LockFile`]
     pub fn finish(self) -> LockFile {
         let (environment_lookup, environments) = self
             .environments
             .into_iter()
             .enumerate()
             .map(|(idx, (name, env))| ((name, idx), env))
             .unzip();
 
         LockFile {
             inner: Arc::new(LockFileInner {
+                version: FileFormatVersion::LATEST,
                 conda_packages: self.conda_packages.into_iter().collect(),
                 pypi_packages: self.pypi_packages.into_iter().collect(),
                 pypi_environment_package_datas: self
                     .pypi_runtime_configurations
                     .into_iter()
                     .map(Into::into)
                     .collect(),
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/channel.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/channel.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/conda.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/conda.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 use rattler_conda_types::{PackageRecord, RepoDataRecord};
 use serde::{Deserialize, Serialize};
 use serde_with::{serde_as, skip_serializing_none};
 use std::cmp::Ordering;
-use std::hash::Hash;
 use url::Url;
 
 /// A locked conda dependency is just a [`PackageRecord`] with some additional information on where
 /// it came from. It is very similar to a [`RepoDataRecord`], but it does not explicitly contain the
 /// channel name.
 #[serde_as]
 #[skip_serializing_none]
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/hash.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/hash.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,155 +1,182 @@
 #![deny(missing_docs, dead_code)]
 
-//! Definitions for a lock-file format that stores information about pinned dependencies from both
-//! the Conda and Pypi ecosystem.
+//! Definitions for a lock-file format that stores information about pinned
+//! dependencies from both the Conda and Pypi ecosystem.
 //!
 //! The crate is structured in two API levels.
 //!
-//! 1. The top level API accessible through the [`LockFile`] type that exposes high level access to
-//!    the lock-file. This API is intended to be relatively stable and is the preferred way to
-//!    interact with the lock-file.
-//! 2. The `*Data` types. These are lower level types that expose more of the internal data
-//!    structures used in the crate. These types are not intended to be stable and are subject to
-//!    change over time. These types are used internally by the top level API. Also note that only
-//!    a subset of the `*Data` types are exposed. See `[crate::PyPiPackageData]`,
+//! 1. The top level API accessible through the [`LockFile`] type that exposes
+//!    high level access to the lock-file. This API is intended to be relatively
+//!    stable and is the preferred way to interact with the lock-file.
+//! 2. The `*Data` types. These are lower level types that expose more of the
+//!    internal data structures used in the crate. These types are not intended
+//!    to be stable and are subject to change over time. These types are used
+//!    internally by the top level API. Also note that only a subset of the
+//!    `*Data` types are exposed. See `[crate::PyPiPackageData]`,
 //!    `[crate::CondaPackageData]` for examples.
 //!
 //! ## Design goals
 //!
 //! The goal of the lock-file format is:
 //!
-//! * To be complete. The lock-file should contain all the information needed to recreate
-//!   environments even years after it was created. As long as the package data persists that a
-//!   lock-file refers to, it should be possible to recreate the environment.
-//! * To be human readable. Although lock-files are not intended to be edited by hand, they should
-//!   be relatively easy to read and understand. So that when a lock-file is checked into version
-//!   control and someone looks at the diff, they can understand what changed.
-//! * To be easily parsable. It should be fairly straightforward to create a parser for the format
-//!   so that it can be used in other tools.
-//! * To reduce diff size when the content changes. The order of content in the serialized lock-file
-//!   should be fixed to ensure that the diff size is minimized when the content changes.
-//! * To be reproducible. Recreating the lock-file with the exact same input (including externally
-//!   fetched data) should yield the same lock-file byte-for-byte.
-//! * To be statically verifiable. Given the specifications of the packages that went into a
-//!   lock-file it should be possible to cheaply verify whether or not the specifications are still
-//!   satisfied by the packages stored in the lock-file.
-//! * Backward compatible. Older version of lock-files should still be readable by never versions of
-//!   this crate.
+//! * To be complete. The lock-file should contain all the information needed to
+//!   recreate environments even years after it was created. As long as the
+//!   package data persists that a lock-file refers to, it should be possible to
+//!   recreate the environment.
+//! * To be human readable. Although lock-files are not intended to be edited by
+//!   hand, they should be relatively easy to read and understand. So that when
+//!   a lock-file is checked into version control and someone looks at the diff,
+//!   they can understand what changed.
+//! * To be easily parsable. It should be fairly straightforward to create a
+//!   parser for the format so that it can be used in other tools.
+//! * To reduce diff size when the content changes. The order of content in the
+//!   serialized lock-file should be fixed to ensure that the diff size is
+//!   minimized when the content changes.
+//! * To be reproducible. Recreating the lock-file with the exact same input
+//!   (including externally fetched data) should yield the same lock-file
+//!   byte-for-byte.
+//! * To be statically verifiable. Given the specifications of the packages that
+//!   went into a lock-file it should be possible to cheaply verify whether or
+//!   not the specifications are still satisfied by the packages stored in the
+//!   lock-file.
+//! * Backward compatible. Older version of lock-files should still be readable
+//!   by never versions of this crate.
 //!
 //! ## Relation to conda-lock
 //!
 //! Initially the lock-file format was based on [`conda-lock`](https://github.com/conda/conda-lock)
-//! but over time significant changes have been made compared to the original conda-lock format.
-//! Conda-lock files (e.g. `conda-lock.yml` files) can still be parsed by this crate but the
-//! serialization format changed significantly. This means files created by this crate are not
-//! compatible with conda-lock.
+//! but over time significant changes have been made compared to the original
+//! conda-lock format. Conda-lock files (e.g. `conda-lock.yml` files) can still
+//! be parsed by this crate but the serialization format changed significantly.
+//! This means files created by this crate are not compatible with conda-lock.
 //!
-//! Conda-lock stores a lot of metadata to be able to verify if the lock-file is still valid given
-//! the sources/inputs. For example conda-lock contains a `content-hash` which is a hash of all the
-//! input data of the lock-file.
-//! This crate approaches this differently by storing enough information in the lock-file to be able
-//! to verify if the lock-file still satisfies an input/source without requiring additional input
-//! (e.g. network requests) or expensive solves. We call this static satisfiability verification.
+//! Conda-lock stores a lot of metadata to be able to verify if the lock-file is
+//! still valid given the sources/inputs. For example conda-lock contains a
+//! `content-hash` which is a hash of all the input data of the lock-file.
+//! This crate approaches this differently by storing enough information in the
+//! lock-file to be able to verify if the lock-file still satisfies an
+//! input/source without requiring additional input (e.g. network requests) or
+//! expensive solves. We call this static satisfiability verification.
 //!
-//! Conda-lock stores a custom __partial__ representation of a [`rattler_conda_types::RepoDataRecord`]
-//! in the lock-file. This poses a problem when incrementally updating an environment. To only
-//! partially update packages in the lock-file without completely recreating it, the records stored
-//! in the lock-file need to be passed to the solver as "preferred" packages. Since
-//! [`rattler_conda_types::MatchSpec`] can match on any field present in a
-//! [`rattler_conda_types::PackageRecord`] we need to store all fields in the lock-file not just a
-//! subset.
-//! To that end this crate stores the full [`rattler_conda_types::PackageRecord`] in the lock-file.
-//! This allows completely recreating the record that was read from repodata when the lock-file was
-//! created which will allow a correct incremental update.
+//! Conda-lock stores a custom __partial__ representation of a
+//! [`rattler_conda_types::RepoDataRecord`] in the lock-file. This poses a
+//! problem when incrementally updating an environment. To only partially update
+//! packages in the lock-file without completely recreating it, the records
+//! stored in the lock-file need to be passed to the solver as "preferred"
+//! packages. Since [`rattler_conda_types::MatchSpec`] can match on any field
+//! present in a [`rattler_conda_types::PackageRecord`] we need to store all
+//! fields in the lock-file not just a subset.
+//! To that end this crate stores the full
+//! [`rattler_conda_types::PackageRecord`] in the lock-file. This allows
+//! completely recreating the record that was read from repodata when the
+//! lock-file was created which will allow a correct incremental update.
 //!
-//! Conda-lock requires users to create multiple lock-files when they want to store multiple
-//! environments. This crate allows storing multiple environments for different platforms and with
-//! different channels in a single lock-file. This allows storing production- and test environments
-//! in a single file.
+//! Conda-lock requires users to create multiple lock-files when they want to
+//! store multiple environments. This crate allows storing multiple environments
+//! for different platforms and with different channels in a single lock-file.
+//! This allows storing production- and test environments in a single file.
+
+use std::{
+    borrow::Cow,
+    collections::{BTreeSet, HashMap},
+    io::Read,
+    path::Path,
+    str::FromStr,
+    sync::Arc,
+};
 
 use fxhash::FxHashMap;
 use pep508_rs::{ExtraName, Requirement};
 use rattler_conda_types::{MatchSpec, PackageRecord, Platform, RepoDataRecord};
-use std::collections::{BTreeSet, HashMap};
-use std::sync::Arc;
-use std::{borrow::Cow, io::Read, path::Path, str::FromStr};
 use url::Url;
 
 mod builder;
 mod channel;
 mod conda;
+mod file_format_version;
 mod hash;
 mod parse;
 mod pypi;
+mod pypi_indexes;
 mod url_or_path;
 mod utils;
 
 pub use builder::LockFileBuilder;
 pub use channel::Channel;
 pub use conda::{CondaPackageData, ConversionError};
+pub use file_format_version::FileFormatVersion;
 pub use hash::PackageHashes;
 pub use parse::ParseCondaLockError;
 pub use pypi::{PypiPackageData, PypiPackageEnvironmentData, PypiSourceTreeHashable};
+pub use pypi_indexes::{FindLinksUrlOrPath, PypiIndexes};
 pub use url_or_path::UrlOrPath;
 
-/// The name of the default environment in a [`LockFile`]. This is the environment name that is used
-/// when no explicit environment name is specified.
+/// The name of the default environment in a [`LockFile`]. This is the
+/// environment name that is used when no explicit environment name is
+/// specified.
 pub const DEFAULT_ENVIRONMENT_NAME: &str = "default";
 
 /// Represents a lock-file for both Conda packages and Pypi packages.
 ///
-/// Lock-files can store information for multiple platforms and for multiple environments.
+/// Lock-files can store information for multiple platforms and for multiple
+/// environments.
 ///
-/// The high-level API provided by this type holds internal references to the data. Its is therefore
-/// cheap to clone this type and any type derived from it (e.g. [`Environment`] or [`Package`]).
+/// The high-level API provided by this type holds internal references to the
+/// data. Its is therefore cheap to clone this type and any type derived from it
+/// (e.g. [`Environment`] or [`Package`]).
 #[derive(Clone, Default)]
 pub struct LockFile {
     inner: Arc<LockFileInner>,
 }
 
 /// Internal data structure that stores the lock-file data.
 #[derive(Default)]
 struct LockFileInner {
+    version: FileFormatVersion,
     environments: Vec<EnvironmentData>,
     conda_packages: Vec<CondaPackageData>,
     pypi_packages: Vec<PypiPackageData>,
     pypi_environment_package_datas: Vec<PypiPackageEnvironmentData>,
 
     environment_lookup: FxHashMap<String, usize>,
 }
 
-/// An package used in an environment. Selects a type of package based on the enum and might contain
-/// additional data that is specific to the environment. For instance different environments might
-/// select the same Pypi package but with different extras.
+/// An package used in an environment. Selects a type of package based on the
+/// enum and might contain additional data that is specific to the environment.
+/// For instance different environments might select the same Pypi package but
+/// with different extras.
 #[derive(Clone, Copy, Debug)]
 enum EnvironmentPackageData {
     Conda(usize),
     Pypi(usize, usize),
 }
 
 /// Information about a specific environment in the lock file.
 ///
-/// This only needs to store information about an environment that cannot be derived from the
-/// packages itself.
+/// This only needs to store information about an environment that cannot be
+/// derived from the packages itself.
 ///
 /// The default environment is called "default".
 #[derive(Clone, Debug)]
 struct EnvironmentData {
     /// The channels used to solve the environment. Note that the order matters.
     channels: Vec<Channel>,
 
-    /// For each individual platform this environment supports we store the package identifiers
-    /// associated with the environment.
+    /// The pypi indexes used to solve the environment.
+    indexes: Option<PypiIndexes>,
+
+    /// For each individual platform this environment supports we store the
+    /// package identifiers associated with the environment.
     packages: FxHashMap<Platform, Vec<EnvironmentPackageData>>,
 }
 
 impl LockFile {
-    /// Constructs a new lock-file builder. This is the preferred way to constructs a lock-file
-    /// programmatically.
+    /// Constructs a new lock-file builder. This is the preferred way to
+    /// constructs a lock-file programmatically.
     pub fn builder() -> LockFileBuilder {
         LockFileBuilder::new()
     }
 
     /// Parses an conda-lock file from a reader.
     pub fn from_reader(mut reader: impl Read) -> Result<Self, ParseCondaLockError> {
         let mut str = String::new();
@@ -175,15 +202,16 @@
         let index = *self.inner.environment_lookup.get(name)?;
         Some(Environment {
             inner: self.inner.clone(),
             index,
         })
     }
 
-    /// Returns the environment with the default name as defined by [`DEFAULT_ENVIRONMENT_NAME`].
+    /// Returns the environment with the default name as defined by
+    /// [`DEFAULT_ENVIRONMENT_NAME`].
     pub fn default_environment(&self) -> Option<Environment> {
         self.environment(DEFAULT_ENVIRONMENT_NAME)
     }
 
     /// Returns an iterator over all environments defined in the lock-file.
     pub fn environments(
         &self,
@@ -197,14 +225,19 @@
                     Environment {
                         inner: self.inner.clone(),
                         index: *index,
                     },
                 )
             })
     }
+
+    /// Returns the version of the lock-file.
+    pub fn version(&self) -> FileFormatVersion {
+        self.inner.version
+    }
 }
 
 /// Information about a specific environment in the lock-file.
 #[derive(Clone)]
 pub struct Environment {
     inner: Arc<LockFileInner>,
     index: usize,
@@ -219,34 +252,44 @@
     /// Returns all the platforms for which we have a locked-down environment.
     pub fn platforms(&self) -> impl Iterator<Item = Platform> + ExactSizeIterator + '_ {
         self.data().packages.keys().copied()
     }
 
     /// Returns the channels that are used by this environment.
     ///
-    /// Note that the order of the channels is significant. The first channel is the highest
-    /// priority channel.
+    /// Note that the order of the channels is significant. The first channel is
+    /// the highest priority channel.
     pub fn channels(&self) -> &[Channel] {
         &self.data().channels
     }
 
+    /// Returns the Pypi indexes that were used to solve this environment.
+    ///
+    /// If there are no pypi packages in the lock-file this will return `None`.
+    ///
+    /// Starting with version `5` of the format this should not be optional.
+    pub fn pypi_indexes(&self) -> Option<&PypiIndexes> {
+        self.data().indexes.as_ref()
+    }
+
     /// Returns all the packages for a specific platform in this environment.
     pub fn packages(
         &self,
         platform: Platform,
     ) -> Option<impl Iterator<Item = Package> + ExactSizeIterator + DoubleEndedIterator + '_> {
         let packages = self.data().packages.get(&platform)?;
         Some(
             packages
                 .iter()
                 .map(move |package| Package::from_env_package(*package, self.inner.clone())),
         )
     }
 
-    /// Returns an iterator over all packages and platforms defined for this environment
+    /// Returns an iterator over all packages and platforms defined for this
+    /// environment
     pub fn packages_by_platform(
         &self,
     ) -> impl Iterator<
         Item = (
             Platform,
             impl Iterator<Item = Package> + ExactSizeIterator + DoubleEndedIterator + '_,
         ),
@@ -283,15 +326,16 @@
                     })
                     .collect();
                 (*platform, records)
             })
             .collect()
     }
 
-    /// Returns all conda packages for all platforms and converts them to [`RepoDataRecord`].
+    /// Returns all conda packages for all platforms and converts them to
+    /// [`RepoDataRecord`].
     pub fn conda_repodata_records(
         &self,
     ) -> Result<HashMap<Platform, Vec<RepoDataRecord>>, ConversionError> {
         let env_data = self.data();
         env_data
             .packages
             .iter()
@@ -306,17 +350,18 @@
                     })
                     .collect::<Result<_, _>>()
                     .map(|records| (*platform, records))
             })
             .collect()
     }
 
-    /// Takes all the conda packages, converts them to [`RepoDataRecord`] and returns them or
-    /// returns an error if the conversion failed. Returns `None` if the specified platform is not
-    /// defined for this environment.
+    /// Takes all the conda packages, converts them to [`RepoDataRecord`] and
+    /// returns them or returns an error if the conversion failed. Returns
+    /// `None` if the specified platform is not defined for this
+    /// environment.
     pub fn conda_repodata_records_for_platform(
         &self,
         platform: Platform,
     ) -> Result<Option<Vec<RepoDataRecord>>, ConversionError> {
         let Some(packages) = self.data().packages.get(&platform) else {
             return Ok(None);
         };
@@ -329,16 +374,17 @@
                 }
                 EnvironmentPackageData::Pypi(_, _) => None,
             })
             .collect::<Result<_, _>>()
             .map(Some)
     }
 
-    /// Returns all the pypi packages and their associated environment data for the specified
-    /// platform. Returns `None` if the platform is not defined for this environment.
+    /// Returns all the pypi packages and their associated environment data for
+    /// the specified platform. Returns `None` if the platform is not
+    /// defined for this environment.
     pub fn pypi_packages_for_platform(
         &self,
         platform: Platform,
     ) -> Option<Vec<(PypiPackageData, PypiPackageEnvironmentData)>> {
         let Some(packages) = self.data().packages.get(&platform) else {
             return None;
         };
@@ -352,29 +398,46 @@
                         self.inner.pypi_packages[*package_idx].clone(),
                         self.inner.pypi_environment_package_datas[*env_idx].clone(),
                     )),
                 })
                 .collect(),
         )
     }
+
+    /// Returns the version of the lock-file that contained this environment.
+    pub fn version(&self) -> FileFormatVersion {
+        self.inner.version
+    }
 }
 
 /// Data related to a single locked package in an [`Environment`].
 #[derive(Clone)]
 pub enum Package {
     /// A conda package
     Conda(CondaPackage),
 
     /// A pypi package
     Pypi(PypiPackage),
 }
 
+impl From<CondaPackage> for Package {
+    fn from(value: CondaPackage) -> Self {
+        Package::Conda(value)
+    }
+}
+
+impl From<PypiPackage> for Package {
+    fn from(value: PypiPackage) -> Self {
+        Package::Pypi(value)
+    }
+}
+
 impl Package {
-    /// Constructs a new instance from a [`EnvironmentPackageData`] and a reference to the internal
-    /// data structure.
+    /// Constructs a new instance from a [`EnvironmentPackageData`] and a
+    /// reference to the internal data structure.
     fn from_env_package(data: EnvironmentPackageData, inner: Arc<LockFileInner>) -> Self {
         match data {
             EnvironmentPackageData::Conda(idx) => {
                 Package::Conda(CondaPackage { inner, index: idx })
             }
             EnvironmentPackageData::Pypi(idx, runtime) => Package::Pypi(PypiPackage {
                 inner,
@@ -390,43 +453,43 @@
     }
 
     /// Returns true if this package represents a pypi package.
     pub fn is_pypi(&self) -> bool {
         matches!(self, Self::Pypi(_))
     }
 
-    /// Returns this instance as a [`CondaPackage`] if this instance represents a conda
-    /// package.
+    /// Returns this instance as a [`CondaPackage`] if this instance represents
+    /// a conda package.
     pub fn as_conda(&self) -> Option<&CondaPackage> {
         match self {
             Self::Conda(value) => Some(value),
             Self::Pypi(_) => None,
         }
     }
 
-    /// Returns this instance as a [`PypiPackage`] if this instance represents a pypi
-    /// package.
+    /// Returns this instance as a [`PypiPackage`] if this instance represents a
+    /// pypi package.
     pub fn as_pypi(&self) -> Option<&PypiPackage> {
         match self {
             Self::Conda(_) => None,
             Self::Pypi(value) => Some(value),
         }
     }
 
-    /// Returns this instance as a [`CondaPackage`] if this instance represents a conda
-    /// package.
+    /// Returns this instance as a [`CondaPackage`] if this instance represents
+    /// a conda package.
     pub fn into_conda(self) -> Option<CondaPackage> {
         match self {
             Self::Conda(value) => Some(value),
             Self::Pypi(_) => None,
         }
     }
 
-    /// Returns this instance as a [`PypiPackage`] if this instance represents a pypi
-    /// package.
+    /// Returns this instance as a [`PypiPackage`] if this instance represents a
+    /// pypi package.
     pub fn into_pypi(self) -> Option<PypiPackage> {
         match self {
             Self::Conda(_) => None,
             Self::Pypi(value) => Some(value),
         }
     }
 
@@ -569,35 +632,39 @@
 
 /// A helper struct to group package and environment data together.
 #[derive(Copy, Clone)]
 pub struct PypiPackageDataRef<'p> {
     /// The package data. This information is deduplicated between environments.
     pub package: &'p PypiPackageData,
 
-    /// Environment specific data for the package. This information is specific to the environment.
+    /// Environment specific data for the package. This information is specific
+    /// to the environment.
     pub environment: &'p PypiPackageEnvironmentData,
 }
 
 #[cfg(test)]
 mod test {
-    use super::{LockFile, DEFAULT_ENVIRONMENT_NAME};
+    use std::path::Path;
+
     use rattler_conda_types::Platform;
     use rstest::*;
-    use std::path::Path;
+
+    use super::{LockFile, DEFAULT_ENVIRONMENT_NAME};
 
     #[rstest]
     #[case("v0/numpy-conda-lock.yml")]
     #[case("v0/python-conda-lock.yml")]
     #[case("v0/pypi-matplotlib-conda-lock.yml")]
     #[case("v3/robostack-turtlesim-conda-lock.yml")]
     #[case("v4/numpy-lock.yml")]
     #[case("v4/python-lock.yml")]
     #[case("v4/pypi-matplotlib-lock.yml")]
     #[case("v4/turtlesim-lock.yml")]
     #[case("v4/path-based-lock.yml")]
+    #[case("v5/flat-index-lock.yml")]
     fn test_parse(#[case] file_name: &str) {
         let path = Path::new(env!("CARGO_MANIFEST_DIR"))
             .join("../../test-data/conda-lock")
             .join(file_name);
         let conda_lock = LockFile::from_path(&path).unwrap();
         insta::assert_yaml_snapshot!(file_name, conda_lock);
     }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/deserialize.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/deserialize.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+use crate::file_format_version::FileFormatVersion;
 use crate::utils::serde::RawCondaPackageData;
 use crate::{
     Channel, CondaPackageData, EnvironmentData, EnvironmentPackageData, LockFile, LockFileInner,
-    ParseCondaLockError, PypiPackageData, PypiPackageEnvironmentData, UrlOrPath,
+    ParseCondaLockError, PypiIndexes, PypiPackageData, PypiPackageEnvironmentData, UrlOrPath,
 };
 use fxhash::FxHashMap;
 use indexmap::IndexSet;
 use itertools::{Either, Itertools};
 use pep508_rs::ExtraName;
 use rattler_conda_types::Platform;
 use serde::Deserialize;
@@ -19,14 +20,16 @@
     environments: BTreeMap<String, DeserializableEnvironment>,
     packages: Vec<DeserializablePackageData<'d>>,
 }
 
 #[derive(Deserialize)]
 struct DeserializableEnvironment {
     channels: Vec<Channel>,
+    #[serde(flatten)]
+    indexes: Option<PypiIndexes>,
     packages: BTreeMap<Platform, Vec<DeserializablePackageSelector>>,
 }
 
 #[derive(Deserialize)]
 #[serde(tag = "kind", rename_all = "snake_case")]
 enum DeserializablePackageData<'d> {
     Conda(Box<RawCondaPackageData<'d>>),
@@ -57,15 +60,18 @@
         Self {
             extras: config.extras.into_iter().collect(),
         }
     }
 }
 
 /// Parses a [`LockFile`] from a [`serde_yaml::Value`].
-pub fn parse_from_document(document: Value) -> Result<LockFile, ParseCondaLockError> {
+pub fn parse_from_document(
+    document: Value,
+    version: FileFormatVersion,
+) -> Result<LockFile, ParseCondaLockError> {
     let raw: DeserializableLockFile<'_> =
         serde_yaml::from_value(document).map_err(ParseCondaLockError::ParseError)?;
 
     // Split the packages into conda and pypi packages.
     let (conda_packages, pypi_packages): (Vec<_>, Vec<_>) =
         raw.packages.into_iter().partition_map(|p| match p {
             DeserializablePackageData::Conda(p) => Either::Left(CondaPackageData::from(*p)),
@@ -89,14 +95,15 @@
         .environments
         .into_iter()
         .map(|(name, env)| {
             Ok((
                 name.clone(),
                 EnvironmentData {
                     channels: env.channels,
+                    indexes: env.indexes,
                     packages: env
                         .packages
                         .into_iter()
                         .map(|(platform, packages)| {
                             let packages = packages
                                 .into_iter()
                                 .map(|p| {
@@ -140,14 +147,15 @@
         .into_iter()
         .enumerate()
         .map(|(idx, (name, env))| ((name, idx), env))
         .unzip();
 
     Ok(LockFile {
         inner: Arc::new(LockFileInner {
+            version,
             environments,
             environment_lookup,
             conda_packages,
             pypi_packages,
             pypi_environment_package_datas: pypi_runtime_lookup
                 .into_iter()
                 .map(Into::into)
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/serialize.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/serialize.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-use super::FILE_VERSION;
+use crate::file_format_version::FileFormatVersion;
 use crate::utils::serde::RawCondaPackageData;
-use crate::{Channel, EnvironmentPackageData, LockFile, PypiPackageData, UrlOrPath};
+use crate::{Channel, EnvironmentPackageData, LockFile, PypiIndexes, PypiPackageData, UrlOrPath};
 use itertools::Itertools;
 use pep508_rs::ExtraName;
 use rattler_conda_types::Platform;
 use serde::{Serialize, Serializer};
 use std::borrow::Cow;
 use std::collections::{BTreeSet, HashSet};
 use std::{cmp::Ordering, collections::BTreeMap};
 use url::Url;
 
 #[derive(Serialize)]
 struct SerializableLockFile<'a> {
-    version: u64,
+    version: FileFormatVersion,
     environments: BTreeMap<&'a String, SerializableEnvironment<'a>>,
     packages: Vec<SerializablePackageData<'a>>,
 }
 
 #[derive(Serialize)]
 struct SerializableEnvironment<'a> {
     channels: &'a [Channel],
+    #[serde(flatten)]
+    indexes: Option<&'a PypiIndexes>,
     packages: BTreeMap<Platform, Vec<SerializablePackageSelector<'a>>>,
 }
 
 #[allow(clippy::large_enum_variant)]
 #[derive(Serialize, Eq, PartialEq)]
 #[serde(tag = "kind", rename_all = "snake_case")]
 enum SerializablePackageData<'a> {
@@ -182,14 +184,15 @@
             .iter()
             .map(|(name, env_idx)| {
                 let env_data = &inner.environments[*env_idx];
                 (
                     name,
                     SerializableEnvironment {
                         channels: &env_data.channels,
+                        indexes: env_data.indexes.as_ref(),
                         packages: env_data
                             .packages
                             .iter()
                             .map(|(platform, packages)| {
                                 (
                                     *platform,
                                     packages
@@ -238,15 +241,15 @@
         packages.retain(|p| used_urls_in_envs.contains(&p.url()));
 
         // Sort the packages in a deterministic order. See [`SerializablePackageData`] for more
         // information.
         packages.sort();
 
         let raw = SerializableLockFile {
-            version: FILE_VERSION,
+            version: FileFormatVersion::LATEST,
             environments,
             packages,
         };
 
         raw.serialize(serializer)
     }
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/parse/v3.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/parse/v3.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 //! A module that enables parsing of lock files version 3 or lower.
 
 use super::ParseCondaLockError;
+use crate::file_format_version::FileFormatVersion;
 use crate::{
     Channel, CondaPackageData, EnvironmentData, EnvironmentPackageData, LockFile, LockFileInner,
     PackageHashes, PypiPackageData, PypiPackageEnvironmentData, UrlOrPath,
     DEFAULT_ENVIRONMENT_NAME,
 };
 use fxhash::FxHashMap;
 use indexmap::IndexSet;
 use pep440_rs::VersionSpecifiers;
 use pep508_rs::{ExtraName, Requirement};
 use rattler_conda_types::{
     NoArchType, PackageName, PackageRecord, PackageUrl, Platform, VersionWithSource,
 };
 use serde::Deserialize;
 use serde_with::{serde_as, skip_serializing_none, OneOrMany};
+use std::ops::Not;
 use std::{collections::BTreeSet, sync::Arc};
 use url::Url;
 
 #[derive(Deserialize)]
 struct LockFileV3 {
     metadata: LockMetaV3,
     package: Vec<LockedPackageV3>,
@@ -109,19 +111,22 @@
     pub license_family: Option<String>,
     #[serde(skip_serializing_if = "NoArchType::is_none")]
     pub noarch: NoArchType,
     pub size: Option<u64>,
     #[serde_as(as = "Option<crate::utils::serde::Timestamp>")]
     pub timestamp: Option<chrono::DateTime<chrono::Utc>>,
     #[serde(default, skip_serializing_if = "Vec::is_empty")]
-    pub purls: Vec<PackageUrl>,
+    pub purls: BTreeSet<PackageUrl>,
 }
 
 /// A function that enables parsing of lock files version 3 or lower.
-pub fn parse_v3_or_lower(document: serde_yaml::Value) -> Result<LockFile, ParseCondaLockError> {
+pub fn parse_v3_or_lower(
+    document: serde_yaml::Value,
+    version: FileFormatVersion,
+) -> Result<LockFile, ParseCondaLockError> {
     let lock_file: LockFileV3 =
         serde_yaml::from_value(document).map_err(ParseCondaLockError::ParseError)?;
 
     // Iterate over all packages, deduplicate them and store the list of packages per platform.
     // There might be duplicates for noarch packages.
     let mut conda_packages = IndexSet::with_capacity(lock_file.package.len());
     let mut pypi_packages = IndexSet::with_capacity(lock_file.package.len());
@@ -162,15 +167,15 @@
                             platform: platform.only_platform().map(ToString::to_string),
                             sha256,
                             size: value.size,
                             subdir: value.subdir.unwrap_or(platform.to_string()),
                             timestamp: value.timestamp,
                             track_features: value.track_features,
                             version: value.version,
-                            purls: value.purls,
+                            purls: value.purls.is_empty().not().then_some(value.purls),
                         },
                         url: value.url,
                         file_name: None,
                         channel: None,
                     })
                     .0;
 
@@ -197,19 +202,21 @@
 
         per_platform.entry(package.platform).or_default().push(pkg);
     }
 
     // Construct the default environment
     let default_environment = EnvironmentData {
         channels: lock_file.metadata.channels,
+        indexes: None,
         packages: per_platform,
     };
 
     Ok(LockFile {
         inner: Arc::new(LockFileInner {
+            version,
             conda_packages: conda_packages.into_iter().collect(),
             pypi_packages: pypi_packages.into_iter().collect(),
             pypi_environment_package_datas: pypi_runtime_configs
                 .into_iter()
                 .map(Into::into)
                 .collect(),
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/pypi.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/pypi.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__packages_for_platform.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__numpy-conda-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -12188,8 +12188,7 @@
     url: "https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.2-hf913c23_6.conda"
     sha256: 018989ba028e76abc332c246002e8f5975ff123c68f6116a30da8009b14ea88d
     md5: 8f346953ef63bf5fb482488a659adcf3
     depends:
       - libcxx >=14.0.6
       - "libzlib >=1.2.13,<1.3.0a0"
     platform: osx
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__pypi-matplotlib-conda-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -855,8 +855,7 @@
     subdir: osx-64
     url: "https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.11-h9173be1_1013.tar.bz2"
     sha256: 9102c5f89c78c56b0bb0766a074f509d67362cf97aa66d706d4e95e9061bb03c
     md5: cf985617d679990418c380099620b01a
     depends:
       - libzlib ==1.2.11 h9173be1_1013
     platform: osx
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v0__python-conda-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -1285,8 +1285,7 @@
     url: "https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2"
     sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
     md5: 515d77642eaa3639413c6b1bc3f94219
     depends:
       - "vc >=14.1,<15"
       - vs2015_runtime >=14.16.27033
     platform: win
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v3__robostack-turtlesim-conda-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: "https://conda.anaconda.org/conda-forge/"
       - url: "https://repo.prefix.dev/robostack-staging/"
     packages:
       linux-64:
@@ -51032,8 +51032,7 @@
       - "zlib >=1.2.11,<1.3.0a0"
     arch: aarch64
     platform: osx
     license: GPL-2.0
     license_family: GPL
     size: 95357
     timestamp: 1617437173697
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__numpy-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -12188,8 +12188,7 @@
     url: "https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.2-hf913c23_6.conda"
     sha256: 018989ba028e76abc332c246002e8f5975ff123c68f6116a30da8009b14ea88d
     md5: 8f346953ef63bf5fb482488a659adcf3
     depends:
       - libcxx >=14.0.6
       - "libzlib >=1.2.13,<1.3.0a0"
     platform: osx
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__path-based-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
-assertion_line: 602
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: "https://conda.anaconda.org/conda-forge/"
     packages:
       win-64:
         - conda: "https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda"
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__pypi-matplotlib-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -855,8 +855,7 @@
     subdir: osx-64
     url: "https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.11-h9173be1_1013.tar.bz2"
     sha256: 9102c5f89c78c56b0bb0766a074f509d67362cf97aa66d706d4e95e9061bb03c
     md5: cf985617d679990418c380099620b01a
     depends:
       - libzlib ==1.2.11 h9173be1_1013
     platform: osx
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__python-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: conda-forge
     packages:
       linux-64:
         - conda: "https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2"
@@ -1285,8 +1285,7 @@
     url: "https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2"
     sha256: 54d9778f75a02723784dc63aff4126ff6e6749ba21d11a6d03c1f4775f269fe0
     md5: 515d77642eaa3639413c6b1bc3f94219
     depends:
       - "vc >=14.1,<15"
       - vs2015_runtime >=14.16.27033
     platform: win
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/snapshots/rattler_lock__test__v4__turtlesim-lock.yml.snap`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 source: crates/rattler_lock/src/lib.rs
 expression: conda_lock
 ---
-version: 4
+version: 5
 environments:
   default:
     channels:
       - url: "https://conda.anaconda.org/conda-forge/"
       - url: "https://repo.prefix.dev/robostack-staging/"
     packages:
       linux-64:
@@ -51032,8 +51032,7 @@
       - "zlib >=1.2.11,<1.3.0a0"
     arch: aarch64
     platform: osx
     license: GPL-2.0
     license_family: GPL
     size: 95357
     timestamp: 1617437173697
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/url_or_path.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/url_or_path.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+use file_url::url_to_path;
 use itertools::Itertools;
-use percent_encoding::percent_decode;
 use serde_with::{DeserializeFromStr, SerializeDisplay};
 use std::borrow::Cow;
 use std::hash::Hash;
 use std::path::Path;
 use std::{
     fmt::{Display, Formatter},
     path::PathBuf,
     str::FromStr,
 };
 use thiserror::Error;
-use url::{Host, Url};
+use url::Url;
 
 /// Represents either a URL or a path.
 ///
 /// URLs have stricter requirements on their format, they must be absolute and they with the
 /// [`url`] we can only create urls for absolute file paths for the current os.
 ///
 /// This also looks better when looking at the lockfile.
@@ -23,81 +23,14 @@
     /// A URL.
     Url(Url),
 
     /// A local (or networked) path.
     Path(PathBuf),
 }
 
-/// Returns true if the specified segment is considered to be a Windows drive letter segment.
-/// E.g. the segment `C:` or `C%3A` would be considered a drive letter segment.
-fn is_windows_drive_letter_segment(segment: &str) -> Option<String> {
-    // Segment is a simple drive letter: X:
-    if let Some((drive_letter, ':')) = segment.chars().collect_tuple() {
-        if drive_letter.is_ascii_alphabetic() {
-            return Some(format!("{drive_letter}:\\"));
-        }
-    }
-
-    // Segment is a simple drive letter but the colon is percent escaped: E.g. X%3A
-    if let Some((drive_letter, '%', '3', 'a' | 'A')) = segment.chars().collect_tuple() {
-        if drive_letter.is_ascii_alphabetic() {
-            return Some(format!("{drive_letter}:\\"));
-        }
-    }
-
-    None
-}
-
-/// Tries to convert a `file://` based URL to a path.
-///
-/// We assume that any passed URL that represents a path is an absolute path.
-///
-/// [`Url::to_file_path`] has a different code path for Windows and other operating systems, this
-/// can cause URLs to parse perfectly fine on Windows, but fail to parse on Linux. This function
-/// tries to parse the URL as a path on all operating systems.
-fn url_to_path(url: &Url) -> Option<PathBuf> {
-    if url.scheme() != "file" {
-        return None;
-    }
-
-    let mut segments = url.path_segments()?;
-    let host = match url.host() {
-        None | Some(Host::Domain("localhost")) => None,
-        Some(host) => Some(host),
-    };
-
-    let (mut path, seperator) = if let Some(host) = host {
-        // A host is only present for Windows UNC paths
-        (format!("\\\\{host}\\"), "\\")
-    } else {
-        let first = segments.next()?;
-        if first.starts_with('.') {
-            // Relative file paths are not supported
-            return None;
-        }
-
-        match is_windows_drive_letter_segment(first) {
-            Some(drive_letter) => (drive_letter, "\\"),
-            None => (format!("/{first}/"), "/"),
-        }
-    };
-
-    for (idx, segment) in segments.enumerate() {
-        if idx > 0 {
-            path.push_str(seperator);
-        }
-        match String::from_utf8(percent_decode(segment.as_bytes()).collect()) {
-            Ok(s) => path.push_str(&s),
-            _ => return None,
-        }
-    }
-
-    Some(PathBuf::from(path))
-}
-
 impl PartialEq for UrlOrPath {
     fn eq(&self, other: &Self) -> bool {
         match (self.canonicalize().as_ref(), other.canonicalize().as_ref()) {
             (UrlOrPath::Path(a), UrlOrPath::Path(b)) => a == b,
             (UrlOrPath::Url(a), UrlOrPath::Url(b)) => a == b,
             _ => false,
         }
@@ -206,34 +139,14 @@
 
 #[cfg(test)]
 mod test {
     use super::*;
     use std::str::FromStr;
 
     #[test]
-    fn test_url_to_path() {
-        let urls = [
-            ("file:///home/bob/test-file.txt", "/home/bob/test-file.txt"),
-            ("file:///C:/Test/Foo.txt", "C:\\Test\\Foo.txt"),
-            ("file:///c:/temp/test-file.txt", "c:\\temp\\test-file.txt"),
-            ("file:///c:\\temp\\test-file.txt", "c:\\temp\\test-file.txt"),
-            // Percent encoding
-            ("file:///foo/ba%20r", "/foo/ba r"),
-            ("file:///C%3A/Test/Foo.txt", "C:\\Test\\Foo.txt"),
-        ];
-
-        for (url, path) in urls {
-            assert_eq!(
-                url_to_path(&Url::from_str(url).unwrap()).unwrap(),
-                PathBuf::from(path)
-            );
-        }
-    }
-
-    #[test]
     fn test_equality() {
         let tests = [
             // Same urls
             (UrlOrPath::Url("https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2".parse().unwrap()),
              UrlOrPath::Url("https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2".parse().unwrap())),
 
             // Absolute paths as file and direct path
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/match_spec_map_or_vec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/ordered.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/pep440_map_or_vec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/raw_conda_package_data.rs`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
     BuildNumber, NoArchType, PackageName, PackageRecord, PackageUrl, VersionWithSource,
 };
 use rattler_digest::{serde::SerializableHash, Md5Hash, Sha256Hash};
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use std::borrow::Cow;
 use std::cmp::Ordering;
+use std::collections::BTreeSet;
 use url::Url;
 
 fn is_default<T: Default + Eq>(value: &T) -> bool {
     value == &T::default()
 }
 
 /// A helper struct that wraps all fields of a [`CondaPackageData`] and allows for easy conversion
@@ -81,17 +82,16 @@
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub file_name: Cow<'a, Option<String>>,
 
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub license: Cow<'a, Option<String>>,
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub license_family: Cow<'a, Option<String>>,
-
-    #[serde(default, skip_serializing_if = "Vec::is_empty")]
-    pub purls: Cow<'a, Vec<PackageUrl>>,
+    #[serde(default, skip_serializing_if = "Option::is_none")]
+    pub purls: Cow<'a, Option<BTreeSet<PackageUrl>>>,
 
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub size: Cow<'a, Option<u64>>,
     #[serde(default, skip_serializing_if = "Option::is_none")]
     pub legacy_bz2_size: Cow<'a, Option<u64>>,
 
     #[serde(default, skip_serializing_if = "Option::is_none")]
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/timestamp.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs` & `py_rattler-0.6.0/local_dependencies/rattler_lock/src/utils/serde/url_or_path.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_shell/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_shell/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [package]
 name = "rattler_shell"
-version = "0.20.1"
+version = "0.20.5"
 edition= "2021"
 authors = ["Wolf Vollprecht <w.vollprecht@gmail.com>"]
 description = "A crate to help with activation and deactivation of a conda environment"
 categories = ["conda", "mamba", "package_management", "virtual_environment"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false }
+rattler_conda_types = { path= "../rattler_conda_types", version = "0.24.0", default-features = false }
 enum_dispatch = "0.3.13"
 indexmap = "2.2.6"
 itertools = "0.12.1"
 serde_json = { version = "1.0.116" , features = ["preserve_order"] }
 shlex = "1.3.0"
 sysinfo = { version = "0.30.10", optional = true }
 tempfile = "3.10.1"
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_shell/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_shell/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,34 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.5](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.4...rattler_shell-v0.20.5) - 2024-05-27
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.20.4](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.3...rattler_shell-v0.20.4) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.20.3](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.2...rattler_shell-v0.20.3) - 2024-05-13
+
+### Other
+- updated the following local packages: rattler_conda_types
+
+## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.1...rattler_shell-v0.20.2) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types
+
 ## [0.20.1](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.20.0...rattler_shell-v0.20.1) - 2024-04-25
 
 ### Fixed
 - compare `UrlOrPath` ([#618](https://github.com/mamba-org/rattler/pull/618))
 
 ## [0.20.0](https://github.com/mamba-org/rattler/compare/rattler_shell-v0.19.6...rattler_shell-v0.20.0) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_shell/src/activation.rs` & `py_rattler-0.6.0/local_dependencies/rattler_shell/src/activation.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_shell/src/run/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_shell/src/run/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_shell/src/shell/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_shell/src/shell/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -627,15 +627,15 @@
 
         // Get current process information
         let mut current_pid = get_current_pid().ok()?;
         system_info.refresh_process(current_pid);
 
         while let Some(parent_process_id) = system_info
             .process(current_pid)
-            .and_then(|process| process.parent())
+            .and_then(sysinfo::Process::parent)
         {
             // Get the name of the parent process
             system_info.refresh_process(parent_process_id);
             let parent_process = system_info.process(parent_process_id)?;
             let parent_process_name = parent_process.name().to_lowercase();
 
             let shell: Option<ShellEnum> = if parent_process_name.contains("bash") {
@@ -869,15 +869,15 @@
         insta::assert_snapshot!(script.contents);
     }
 
     #[cfg(feature = "sysinfo")]
     #[test]
     fn test_from_parent_process_doenst_crash() {
         let shell = ShellEnum::from_parent_process();
-        println!("Detected shell: {:?}", shell);
+        println!("Detected shell: {shell:?}");
     }
 
     #[test]
     fn test_from_env() {
         let shell = ShellEnum::from_env();
         println!("Detected shell: {shell:?}");
     }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_macros/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_macros/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_macros/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_macros/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 [package]
-name = "rattler_repodata_gateway"
-version = "0.19.9"
+name = "rattler"
+version = "0.26.0"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
-description = "A crate to interact with Conda repodata"
+description = "Rust library to install conda environments"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
+[features]
+default = ['native-tls']
+native-tls = ['reqwest/native-tls', 'rattler_package_streaming/native-tls']
+rustls-tls = ['reqwest/rustls-tls', 'rattler_package_streaming/rustls-tls']
+cli-tools = ['dep:clap']
+indicatif = ['dep:indicatif', 'dep:console']
+
 [dependencies]
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false, features = ["tokio", "serde"] }
-rattler_conda_types = { path= "../rattler_conda_types", version = "0.22.0", default-features = false, optional = true }
-rattler_networking = { path= "../rattler_networking", version = "0.20.3", default-features = false }
-async-compression = { version = "0.4.8", features = [
-    "gzip",
-    "tokio",
-    "bzip2",
-    "zstd","gzip", "tokio", "bzip2", "zstd",
-] }
-blake2 = "0.10.6"
-cache_control = "0.2.0"
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
+rattler_networking = { path = "../rattler_networking", version = "0.20.8", default-features = false }
+rattler_shell = { path = "../rattler_shell", version = "0.20.5", default-features = false }
+rattler_package_streaming = { path = "../rattler_package_streaming", version = "0.21.0", default-features = false, features = ["reqwest"] }
+simple_spawn_blocking = { path = "../simple_spawn_blocking", version = "1.0", default-features = false, features = ["tokio"] }
+anyhow = "1.0.82"
+bytes = "1.6.0"
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
-    "alloc","std", "serde", "alloc", "clock",
+    "alloc",
 ] }
-humansize = "2.1.3"
-humantime = "2.1.0"
+clap = { version = "4.5.4", features = ["derive"] , optional = true }
+digest = "0.10.7"
+dirs = "5.0.1"
+fs-err = "2.11.0"
 futures = "0.3.30"
-reqwest = { version = "0.12.3", default-features = false , features = ["stream"] }
+fxhash = "0.2.1"
+humantime = "2.1.0"
+indexmap = "2.2.6"
+indicatif = { version = "0.17.8", optional = true }
+itertools = "0.12.1"
+memchr = "2.7.2"
+memmap2 = "0.9.4"
+once_cell = "1.19.0"
+parking_lot = "0.12.1"
+reflink-copy = "0.1.16"
+regex = "1.10.4"
+reqwest = { version = "0.12.3", default-features = false , features = ["stream", "json", "gzip"] }
 reqwest-middleware = "0.3.0"
-tokio-util = { version = "0.7.10", features = ["codec", "io"] }
+smallvec = { version = "1.13.2", features = [
+    "serde",
+    "const_new",
+    "const_generics",
+    "union",
+] }
 tempfile = "3.10.1"
-tracing = "0.1.40"
 thiserror = "1.0"
+tokio = { version = "1.37.0", default-features = false , features = ["rt", "io-util", "macros"] }
+tokio-stream = { version = "0.1.15", features = ["sync"] }
+tracing = "0.1.40"
 url = { version = "2.5.0" , features = ["serde"] }
-tokio = { version = "1.37.0", default-features = false , features = ["rt", "io-util"] }
-anyhow = "1.0.82"
-serde = { version = "1.0.198" , features = ["derive"] }
-serde_json = { version = "1.0.116" }
-pin-project-lite = "0.2.14"
-memmap2 = { version = "0.9.4", optional = true }
-ouroboros = { version = "0.18.3", optional = true }
-serde_with = "3.7.0"
-superslice = { version = "1.0.0", optional = true }
-itertools = { version = "0.12.1", optional = true }
-json-patch = "1.2.0"
-hex = { version = "0.4.3", features = ["serde"] }
-
-[target.'cfg(unix)'.dependencies]
-libc = { version = "0.2" }
-
-[target.'cfg(windows)'.dependencies]
-windows-sys = { version = "0.52.0", default-features = false , features = ["Win32_Storage_FileSystem", "Win32_Foundation", "Win32_System_IO"] }
-
-[features]
-default = ['native-tls']
-native-tls = ['reqwest/native-tls']
-rustls-tls = ['reqwest/rustls-tls']
-sparse = ["rattler_conda_types", "memmap2", "ouroboros", "superslice", "itertools", "serde_json/raw_value"]
+uuid = { version = "1.8.0", default-features = false , features = ["v4", "fast-rng"] }
+console = { version = "0.15.8", features = ["windows-console-colors"] , optional = true }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,46 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.20.2](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.1...rattler_repodata_gateway-v0.20.2) - 2024-05-27
+
+### Fixed
+- result grouped by subdir instead of channel ([#666](https://github.com/mamba-org/rattler/pull/666))
+
+### Other
+- introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
+
+## [0.20.1](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.20.0...rattler_repodata_gateway-v0.20.1) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.20.0](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.19.11...rattler_repodata_gateway-v0.20.0) - 2024-05-13
+
+### Added
+- add clear subdir cache function to repodata gateway ([#650](https://github.com/mamba-org/rattler/pull/650))
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Other
+- update README.md
+
+## [0.19.11](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.19.10...rattler_repodata_gateway-v0.19.11) - 2024-05-06
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_networking
+
+## [0.19.10](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.19.9...rattler_repodata_gateway-v0.19.10) - 2024-04-30
+
+### Added
+- create SparseRepoData from byte slices ([#624](https://github.com/mamba-org/rattler/pull/624))
+
 ## [0.19.9](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.19.8...rattler_repodata_gateway-v0.19.9) - 2024-04-25
 
 ### Other
 - updated the following local packages: rattler_networking
 
 ## [0.19.8](https://github.com/mamba-org/rattler/compare/rattler_repodata_gateway-v0.19.7...rattler_repodata_gateway-v0.19.8) - 2024-04-25
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/cache_headers.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/cache/snapshots/rattler_repodata_gateway__fetch__cache__test__parse_repo_data_state_two.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/jlap/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,16 @@
 //!      }"#).unwrap();
 //!
 //!     // Patches `current_repo_data` and returns an updated JLAP state object
 //!     let updated_jlap_state = patch_repo_data(
 //!         &client,
 //!         subdir_url,
 //!         repo_data_state,
-//!         &current_repo_data
+//!         &current_repo_data,
+//!         None
 //!     ).await.unwrap();
 //!
 //!     // Now we can use the `updated_jlap_state` object to update our `.info.json` file
 //! }
 //! ```
 //!
 
@@ -86,27 +87,29 @@
 use rattler_networking::Redact;
 use reqwest::{
     header::{HeaderMap, HeaderValue},
     Response, StatusCode,
 };
 use reqwest_middleware::ClientWithMiddleware;
 use serde::{Deserialize, Serialize};
+use serde_json::Value;
 use serde_with::serde_as;
-use std::collections::{BTreeMap, HashMap};
 use std::io::Write;
 use std::iter::Iterator;
 use std::path::Path;
 use std::str;
 use std::str::FromStr;
 use std::sync::Arc;
 use tempfile::NamedTempFile;
-use tokio::task::JoinError;
 use url::Url;
 
 pub use crate::fetch::cache::{JLAPFooter, JLAPState, RepoDataState};
+use crate::reporter::ResponseReporterExt;
+use crate::Reporter;
+use simple_spawn_blocking::{tokio::run_blocking_task, Cancelled};
 
 /// File suffix for JLAP file
 pub const JLAP_FILE_SUFFIX: &str = "jlap";
 
 /// File name of JLAP file
 pub const JLAP_FILE_NAME: &str = "repodata.jlap";
 
@@ -160,14 +163,20 @@
     InvalidResponse,
 
     /// The operation was cancelled
     #[error("the operation was cancelled")]
     Cancelled,
 }
 
+impl From<Cancelled> for JLAPError {
+    fn from(_: Cancelled) -> Self {
+        JLAPError::Cancelled
+    }
+}
+
 impl From<reqwest_middleware::Error> for JLAPError {
     fn from(value: reqwest_middleware::Error) -> Self {
         Self::HTTP(value.redact())
     }
 }
 
 impl From<reqwest::Error> for JLAPError {
@@ -300,35 +309,30 @@
 
     /// Applies patches to a `repo_data_json_path` file provided using the `hash` value to
     /// find the correct ones to apply.
     pub async fn apply(
         &self,
         repo_data_json_path: &Path,
         hash: Output<Blake2b256>,
+        reporter: Option<Arc<dyn Reporter>>,
     ) -> Result<Blake2b256Hash, JLAPError> {
         // We use the current hash to find which patches we need to apply
         let current_idx = self.patches.iter().position(|patch| patch.from == hash);
         let Some(idx) = current_idx else {
             return Err(JLAPError::NoHashFound);
         };
 
         // Apply the patches on a blocking thread. Applying the patches is a relatively CPU intense
         // operation and we don't want to block the tokio runtime.
-        let patches = self.patches.clone();
+        let repo_data_path = self.patches.clone();
         let repo_data_json_path = repo_data_json_path.to_path_buf();
-        match tokio::task::spawn_blocking(move || {
-            apply_jlap_patches(patches, idx, &repo_data_json_path)
+        run_blocking_task(move || {
+            apply_jlap_patches(repo_data_path, idx, &repo_data_json_path, reporter)
         })
         .await
-        .map_err(JoinError::try_into_panic)
-        {
-            Ok(hash) => hash,
-            Err(Ok(reason)) => std::panic::resume_unwind(reason),
-            Err(_) => Err(JLAPError::Cancelled),
-        }
     }
 
     /// Returns a new [`JLAPState`] based on values in [`JLAPResponse`] struct
     ///
     /// We accept `position` as an argument because it is not derived from the JLAP response.
     ///
     /// The `initialization_vector` value is optionally passed in because we may wish
@@ -406,28 +410,36 @@
 ///
 /// The return value is the updated [`JLAPState`] and the Blake2b256 hash of the new file.
 pub async fn patch_repo_data(
     client: &ClientWithMiddleware,
     subdir_url: Url,
     repo_data_state: RepoDataState,
     repo_data_json_path: &Path,
+    reporter: Option<Arc<dyn Reporter>>,
 ) -> Result<(JLAPState, Blake2b256Hash), JLAPError> {
     // Determine what we should use as our starting state
     let mut jlap_state = get_jlap_state(repo_data_state.jlap);
 
     let jlap_url = subdir_url
         .join(JLAP_FILE_NAME)
         .expect("Valid URLs should always be join-able with this constant value");
 
+    let download_report = reporter
+        .as_deref()
+        .map(|reporter| (reporter, reporter.on_download_start(&jlap_url)));
     let (response, position) =
-        fetch_jlap_with_retry(jlap_url.as_str(), client, jlap_state.position).await?;
-    let response_text = match response.text().await {
+        fetch_jlap_with_retry(&jlap_url, client, jlap_state.position).await?;
+    let jlap_response_url = response.url().clone();
+    let response_text = match response.text_with_progress(download_report).await {
         Ok(value) => value,
         Err(error) => return Err(error.into()),
     };
+    if let Some((reporter, index)) = download_report {
+        reporter.on_download_complete(&jlap_response_url, index);
+    }
 
     // Update position as it may have changed
     jlap_state.position = position;
 
     let jlap = JLAPResponse::new(&response_text, &jlap_state)?;
     let hash = repo_data_state.blake2_hash_nominal.unwrap_or_default();
     let latest_hash = jlap.footer.latest;
@@ -441,27 +453,27 @@
         return Ok((
             jlap.get_state(jlap.new_position, new_iv),
             repo_data_state.blake2_hash.unwrap_or_default(),
         ));
     }
 
     // Applies patches and returns early if an error is encountered
-    let hash = jlap.apply(repo_data_json_path, hash).await?;
+    let hash = jlap.apply(repo_data_json_path, hash, reporter).await?;
 
     // Patches were applied successfully, so we need to update the position
     Ok((jlap.get_state(jlap.new_position, new_iv), hash))
 }
 
 /// Fetches a JLAP response from server
 async fn fetch_jlap(
-    url: &str,
+    url: &Url,
     client: &ClientWithMiddleware,
     range: &str,
 ) -> reqwest_middleware::Result<Response> {
-    let request_builder = client.get(url);
+    let request_builder = client.get(url.clone());
     let mut headers = HeaderMap::default();
 
     headers.insert(
         reqwest::header::RANGE,
         HeaderValue::from_str(range).unwrap(),
     );
 
@@ -473,15 +485,15 @@
 /// When a JLAP file is updated on the server, it may cause new requests to trigger a
 /// `RANGE_NOT_SATISFIABLE` error because the local cache is now out of sync. In this case, we
 /// try the request once more from the beginning.
 ///
 /// We return a new value for position if this was triggered so that we can update the
 /// `JLAPState` accordingly.
 async fn fetch_jlap_with_retry(
-    url: &str,
+    url: &Url,
     client: &ClientWithMiddleware,
     position: u64,
 ) -> Result<(Response, u64), JLAPError> {
     tracing::info!("fetching JLAP state from {url} (bytes={position}-)");
     let range = format!("bytes={position}-");
 
     match fetch_jlap(url, client, &range).await {
@@ -498,90 +510,71 @@
             }
             Ok((response, position))
         }
         Err(error) => Err(error.into()),
     }
 }
 
-#[derive(Serialize, Deserialize, Default)]
-struct OrderedRepoData {
-    info: Option<HashMap<String, String>>,
-
-    #[serde(serialize_with = "ordered_map")]
-    packages: Option<HashMap<String, HashMap<String, serde_json::Value>>>,
-
-    #[serde(serialize_with = "ordered_map", rename = "packages.conda")]
-    packages_conda: Option<HashMap<String, HashMap<String, serde_json::Value>>>,
-
-    removed: Option<Vec<String>>,
-
-    repodata_version: Option<u64>,
-}
-
-fn ordered_map<S>(
-    value: &Option<HashMap<String, HashMap<String, serde_json::Value>>>,
-    serializer: S,
-) -> Result<S::Ok, S::Error>
-where
-    S: serde::Serializer,
-{
-    match value {
-        Some(value) => {
-            let ordered: BTreeMap<_, _> = value
-                .iter()
-                .map(|(key, packages)| (key, packages.iter().collect::<BTreeMap<_, _>>()))
-                .collect();
-            ordered.serialize(serializer)
-        }
-        None => serializer.serialize_none(),
-    }
-}
-
 /// Applies JLAP patches to a `repodata.json` file
 ///
 /// This is a multi-step process that involves:
 ///
 /// 1. Opening and parsing the current repodata file
 /// 2. Applying patches to this repodata file
 /// 3. Re-ordering the repo data
 /// 4. Saving this repodata file to disk
 fn apply_jlap_patches(
     patches: Arc<[Patch]>,
     start_index: usize,
     repo_data_path: &Path,
+    reporter: Option<Arc<dyn Reporter>>,
 ) -> Result<Blake2b256Hash, JLAPError> {
+    let report = reporter
+        .as_deref()
+        .map(|reporter| (reporter, reporter.on_jlap_start()));
+
+    if let Some((reporter, index)) = report {
+        reporter.on_jlap_decode_start(index);
+    }
+
     // Read the contents of the current repodata to a string
     let repo_data_contents =
         std::fs::read_to_string(repo_data_path).map_err(JLAPError::FileSystem)?;
 
     // Parse the JSON so we can manipulate it
     tracing::info!("parsing cached repodata.json as JSON");
-    let mut doc = serde_json::from_str(&repo_data_contents).map_err(JLAPError::JSONParse)?;
+    let mut repo_data =
+        serde_json::from_str::<Value>(&repo_data_contents).map_err(JLAPError::JSONParse)?;
+
+    if let Some((reporter, index)) = report {
+        reporter.on_jlap_decode_completed(index);
+    }
 
     // Apply any patches that we have not already applied
     tracing::info!(
         "applying patches #{} through #{}",
         start_index + 1,
         patches.len()
     );
-    for patch in patches[start_index..].iter() {
-        if let Err(error) = json_patch::patch_unsafe(&mut doc, &patch.patch) {
+    for (patch_index, patch) in patches[start_index..].iter().enumerate() {
+        if let Some((reporter, index)) = report {
+            reporter.on_jlap_apply_patch(index, patch_index, patches.len());
+        }
+        if let Err(error) = json_patch::patch_unsafe(&mut repo_data, &patch.patch) {
             return Err(JLAPError::JSONPatch(error));
         }
     }
 
-    // Order the json
-    tracing::info!("converting patched JSON back to repodata");
-    let ordered_doc: OrderedRepoData = serde_json::from_value(doc).map_err(JLAPError::JSONParse)?;
+    if let Some((reporter, index)) = report {
+        reporter.on_jlap_apply_patches_completed(index);
+        reporter.on_jlap_encode_start(index);
+    }
 
     // Convert the json to bytes, but we don't really care about formatting.
-    let mut updated_json = serde_json::to_string(&ordered_doc).map_err(JLAPError::JSONParse)?;
-
-    // We need to add an extra newline character to the end of our string so the hashes match
-    updated_json.insert(updated_json.len(), '\n');
+    let updated_json = serde_json::to_string(&repo_data).map_err(JLAPError::JSONParse)?;
 
     // Write the content to disk and immediately compute the hash of the file contents.
     tracing::info!("writing patched repodata to disk");
     let mut hashing_writer = NamedTempFile::new_in(
         repo_data_path
             .parent()
             .expect("the repodata.json file must reside in a directory"),
@@ -591,14 +584,19 @@
     hashing_writer
         .write_all(&updated_json.into_bytes())
         .map_err(JLAPError::FileSystem)?;
     let (file, hash) = hashing_writer.finalize();
     file.persist(repo_data_path)
         .map_err(|e| JLAPError::FileSystem(e.error))?;
 
+    if let Some((reporter, index)) = report {
+        reporter.on_jlap_encode_completed(index);
+        reporter.on_jlap_completed(index);
+    }
+
     Ok(hash)
 }
 
 /// Retrieves the correct values for `position` and `initialization_vector` from a `JLAPState` object
 ///
 /// If we cannot find the correct values, we provide defaults from this module.
 /// When we can correctly parse a hex string (the `initialization_vector` should always be a
@@ -775,20 +773,19 @@
       "subdir": "osx-64",
       "timestamp": 1680034665911,
       "version": "1.5.4"
     }
   },
   "removed": [],
   "repodata_version": 1
-}
-"#;
+}"#;
 
-    const FAKE_REPO_DATA_UPDATE_ONE: &str = "{\"info\":{\"subdir\":\"osx-64\"},\"packages\":{},\"packages.conda\":{\"zstd-1.5.4-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"f284fea068c51b1a0eaea3ac58c300c0\",\"name\":\"zstd\",\"sha256\":\"0af4513ef7ad7fa8854fa714130c25079f3744471fc106f47df80eb10c34429d\",\"size\":605550,\"subdir\":\"osx-64\",\"timestamp\":1680034665911,\"version\":\"1.5.4\"},\"zstd-1.5.5-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"5e0b7ddb1b7dc6b630e1f9a03499c19c\",\"name\":\"zstd\",\"sha256\":\"5b192501744907b841de036bb89f5a2776b4cac5795ccc25dcaebeac784db038\",\"size\":622467,\"subdir\":\"osx-64\",\"timestamp\":1681304595869,\"version\":\"1.5.5\"}},\"removed\":[],\"repodata_version\":1}\n";
+    const FAKE_REPO_DATA_UPDATE_ONE: &str = "{\"info\":{\"subdir\":\"osx-64\"},\"packages\":{},\"packages.conda\":{\"zstd-1.5.4-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"f284fea068c51b1a0eaea3ac58c300c0\",\"name\":\"zstd\",\"sha256\":\"0af4513ef7ad7fa8854fa714130c25079f3744471fc106f47df80eb10c34429d\",\"size\":605550,\"subdir\":\"osx-64\",\"timestamp\":1680034665911,\"version\":\"1.5.4\"},\"zstd-1.5.5-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"5e0b7ddb1b7dc6b630e1f9a03499c19c\",\"name\":\"zstd\",\"sha256\":\"5b192501744907b841de036bb89f5a2776b4cac5795ccc25dcaebeac784db038\",\"size\":622467,\"subdir\":\"osx-64\",\"timestamp\":1681304595869,\"version\":\"1.5.5\"}},\"removed\":[],\"repodata_version\":1}";
 
-    const FAKE_REPO_DATA_UPDATE_TWO: &str = "{\"info\":{\"subdir\":\"osx-64\"},\"packages\":{},\"packages.conda\":{\"zstd-1.5.4-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"f284fea068c51b1a0eaea3ac58c300c0\",\"name\":\"zstd\",\"sha256\":\"0af4513ef7ad7fa8854fa714130c25079f3744471fc106f47df80eb10c34429d\",\"size\":605550,\"subdir\":\"osx-64\",\"timestamp\":1680034665911,\"version\":\"1.5.4\"},\"zstd-1.5.5-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"5e0b7ddb1b7dc6b630e1f9a03499c19c\",\"name\":\"zstd\",\"sha256\":\"5b192501744907b841de036bb89f5a2776b4cac5795ccc25dcaebeac784db038\",\"size\":622467,\"subdir\":\"osx-64\",\"timestamp\":1681304595869,\"version\":\"1.5.5\"},\"zstd-static-1.4.5-hb1e8313_0.conda\":{\"build\":\"hb1e8313_0\",\"build_number\":0,\"depends\":[\"libcxx >=10.0.0\",\"zstd 1.4.5 h41d2c2f_0\"],\"license\":\"BSD 3-Clause\",\"md5\":\"5447986040e0b73d6c681a4d8f615d6c\",\"name\":\"zstd-static\",\"sha256\":\"3759ab53ff8320d35c6db00d34059ba99058eeec1cbdd0da968c5e12f73f7658\",\"size\":13930,\"subdir\":\"osx-64\",\"timestamp\":1595965109852,\"version\":\"1.4.5\"}},\"removed\":[],\"repodata_version\":1}\n";
+    const FAKE_REPO_DATA_UPDATE_TWO: &str = "{\"info\":{\"subdir\":\"osx-64\"},\"packages\":{},\"packages.conda\":{\"zstd-1.5.4-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"f284fea068c51b1a0eaea3ac58c300c0\",\"name\":\"zstd\",\"sha256\":\"0af4513ef7ad7fa8854fa714130c25079f3744471fc106f47df80eb10c34429d\",\"size\":605550,\"subdir\":\"osx-64\",\"timestamp\":1680034665911,\"version\":\"1.5.4\"},\"zstd-1.5.5-hc035e20_0.conda\":{\"build\":\"hc035e20_0\",\"build_number\":0,\"depends\":[\"libcxx >=14.0.6\",\"lz4-c >=1.9.4,<1.10.0a0\",\"xz >=5.2.10,<6.0a0\",\"zlib >=1.2.13,<1.3.0a0\"],\"license\":\"BSD-3-Clause AND GPL-2.0-or-later\",\"license_family\":\"BSD\",\"md5\":\"5e0b7ddb1b7dc6b630e1f9a03499c19c\",\"name\":\"zstd\",\"sha256\":\"5b192501744907b841de036bb89f5a2776b4cac5795ccc25dcaebeac784db038\",\"size\":622467,\"subdir\":\"osx-64\",\"timestamp\":1681304595869,\"version\":\"1.5.5\"},\"zstd-static-1.4.5-hb1e8313_0.conda\":{\"build\":\"hb1e8313_0\",\"build_number\":0,\"depends\":[\"libcxx >=10.0.0\",\"zstd 1.4.5 h41d2c2f_0\"],\"license\":\"BSD 3-Clause\",\"md5\":\"5447986040e0b73d6c681a4d8f615d6c\",\"name\":\"zstd-static\",\"sha256\":\"3759ab53ff8320d35c6db00d34059ba99058eeec1cbdd0da968c5e12f73f7658\",\"size\":13930,\"subdir\":\"osx-64\",\"timestamp\":1595965109852,\"version\":\"1.4.5\"}},\"removed\":[],\"repodata_version\":1}";
 
     const FAKE_REPO_DATA_UPDATE_ONE_HASH: &str =
         "9b76165ba998f77b2f50342006192bf28817dad474d78d760ab12cc0260e3ed9";
 
     const FAKE_REPO_DATA_UPDATE_TWO_HASH: &str =
         "160b529c5f72b9755f951c1b282705d49d319a5f2f80b33fb1a670d02ddeacf9";
 
@@ -947,14 +944,15 @@
         let test_env = TestEnvironment::new(repo_data, jlap_data, repo_data_state).await;
 
         let (updated_jlap_state, _hash) = patch_repo_data(
             &test_env.client,
             test_env.server_url,
             test_env.repo_data_state,
             &test_env.cache_repo_data,
+            None,
         )
         .await
         .unwrap();
 
         // Make assertions
         let repo_data = tokio::fs::read_to_string(test_env.cache_repo_data)
             .await
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/fetch/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 //! This module provides functionality to download and cache `repodata.json` from a remote location.
 
+use crate::reporter::ResponseReporterExt;
 use crate::utils::{AsyncEncoding, Encoding, LockedFile};
+use crate::Reporter;
 use cache::{CacheHeaders, Expiring, RepoDataState};
 use cache_control::{Cachability, CacheControl};
 use futures::{future::ready, FutureExt, TryStreamExt};
 use humansize::{SizeFormatter, DECIMAL};
 use rattler_digest::{compute_file_digest, Blake2b256, HashingWriter};
 use rattler_networking::Redact;
 use reqwest::{
     header::{HeaderMap, HeaderValue},
     Response, StatusCode,
 };
+use std::sync::Arc;
 use std::{
     io::ErrorKind,
     path::{Path, PathBuf},
     time::SystemTime,
 };
 use tempfile::NamedTempFile;
 use tokio_util::io::StreamReader;
 use tracing::instrument;
 use url::Url;
 
 mod cache;
 pub mod jlap;
 
-/// Type alias for function to report progress while downloading repodata
-pub type ProgressFunc = Box<dyn FnMut(DownloadProgress) + Send + Sync>;
-
 /// `RepoData` could not be found for given channel and platform
 #[derive(Debug, thiserror::Error)]
 pub enum RepoDataNotFoundError {
     /// There was an error on the Http request
     #[error(transparent)]
-    HttpError(reqwest_middleware::Error),
+    HttpError(reqwest::Error),
 
     /// There was a file system error
     #[error(transparent)]
-    FileSystemError(std::io::Error),
+    FileSystemError(#[from] std::io::Error),
 }
 
 #[allow(missing_docs)]
 #[derive(Debug, thiserror::Error)]
 pub enum FetchRepoDataError {
     #[error("failed to acquire a lock on the repodata cache")]
     FailedToAcquireLock(#[source] anyhow::Error),
@@ -84,23 +84,17 @@
 
 impl From<reqwest::Error> for FetchRepoDataError {
     fn from(err: reqwest::Error) -> Self {
         Self::HttpError(err.redact().into())
     }
 }
 
-impl From<reqwest_middleware::Error> for RepoDataNotFoundError {
-    fn from(err: reqwest_middleware::Error) -> Self {
-        Self::HttpError(err.redact())
-    }
-}
-
 impl From<reqwest::Error> for RepoDataNotFoundError {
     fn from(err: reqwest::Error) -> Self {
-        Self::HttpError(err.redact().into())
+        Self::HttpError(err.redact())
     }
 }
 
 impl From<tokio::task::JoinError> for FetchRepoDataError {
     fn from(err: tokio::task::JoinError) -> Self {
         // Rethrow any panic
         if let Ok(panic) = err.try_into_panic() {
@@ -193,25 +187,14 @@
             jlap_enabled: true,
             zstd_enabled: true,
             bz2_enabled: true,
         }
     }
 }
 
-/// A struct that provides information about download progress.
-#[derive(Debug, Clone)]
-pub struct DownloadProgress {
-    /// The number of bytes already downloaded
-    pub bytes: u64,
-
-    /// The total number of bytes to download. Or `None` if this is not known. This can happen
-    /// if the server does not supply a `Content-Length` header.
-    pub total: Option<u64>,
-}
-
 /// The result of [`fetch_repo_data`].
 #[derive(Debug)]
 pub struct CachedRepoData {
     /// A lockfile that guards access to any of the repodata.json file or its cache.
     pub lock_file: LockedFile,
 
     /// The path to the uncompressed repodata.json file.
@@ -317,15 +300,15 @@
 /// the respective URLs. The result of these are cached.
 #[instrument(err, skip_all, fields(subdir_url, cache_path = % cache_path.display()))]
 pub async fn fetch_repo_data(
     subdir_url: Url,
     client: reqwest_middleware::ClientWithMiddleware,
     cache_path: PathBuf,
     options: FetchRepoDataOptions,
-    progress: Option<ProgressFunc>,
+    reporter: Option<Arc<dyn Reporter>>,
 ) -> Result<CachedRepoData, FetchRepoDataError> {
     let subdir_url = normalize_subdir_url(subdir_url);
 
     // Compute the cache key from the url
     let cache_key = crate::utils::url_to_cache_filename(
         &subdir_url
             .join(options.variant.file_name())
@@ -425,14 +408,15 @@
     let jlap_state = if has_jlap && cache_state.is_some() {
         let repo_data_state = cache_state.as_ref().unwrap();
         match jlap::patch_repo_data(
             &client,
             subdir_url.clone(),
             repo_data_state.clone(),
             &repo_data_json_path,
+            reporter.clone(),
         )
         .await
         {
             Ok((state, disk_hash)) => {
                 tracing::info!("fetched JLAP patches successfully");
                 let cache_state = RepoDataState {
                     blake2_hash: Some(disk_hash),
@@ -501,14 +485,17 @@
     );
 
     // Add previous cache headers if we have them
     if let Some(cache_headers) = cache_state.as_ref().map(|state| &state.cache_headers) {
         cache_headers.add_to_request(&mut headers);
     }
     // Send the request and wait for a reply
+    let download_reporter = reporter
+        .as_deref()
+        .map(|r| (r, r.on_download_start(&repo_data_url)));
     let response = match request_builder.headers(headers).send().await {
         Ok(response) if response.status() == StatusCode::NOT_FOUND => {
             return Err(FetchRepoDataError::NotFound(RepoDataNotFoundError::from(
                 response.error_for_status().unwrap_err(),
             )));
         }
         Ok(response) => response.error_for_status()?,
@@ -547,29 +534,34 @@
         });
     }
 
     // Get cache headers from the response
     let cache_headers = CacheHeaders::from(&response);
 
     // Stream the content to a temporary file
+    let response_url = response.url().clone();
     let (temp_file, blake2_hash) = stream_and_decode_to_file(
         repo_data_url.clone(),
         response,
         if has_zst {
             Encoding::Zst
         } else if has_bz2 {
             Encoding::Bz2
         } else {
             Encoding::Passthrough
         },
         &cache_path,
-        progress,
+        download_reporter,
     )
     .await?;
 
+    if let Some((reporter, index)) = download_reporter {
+        reporter.on_download_complete(&response_url, index);
+    }
+
     // Persist the file to its final destination
     let repo_data_destination_path = repo_data_json_path.clone();
     let repo_data_json_metadata = tokio::task::spawn_blocking(move || {
         let file = temp_file
             .persist(repo_data_destination_path)
             .map_err(FetchRepoDataError::FailedToPersistTemporaryFile)?;
 
@@ -621,49 +613,28 @@
 /// to disk it also computes the BLAKE2 hash of the file.
 #[instrument(skip_all)]
 async fn stream_and_decode_to_file(
     url: Url,
     response: Response,
     content_encoding: Encoding,
     temp_dir: &Path,
-    mut progress_func: Option<ProgressFunc>,
+    reporter: Option<(&dyn Reporter, usize)>,
 ) -> Result<(NamedTempFile, blake2::digest::Output<Blake2b256>), FetchRepoDataError> {
-    // Determine the length of the response in bytes and notify the listener that a download is
-    // starting. The response may be compressed. Decompression happens below.
-    let content_size = response.content_length();
-    if let Some(progress_func) = progress_func.as_mut() {
-        progress_func(DownloadProgress {
-            bytes: 0,
-            total: content_size,
-        });
-    }
-
     // Determine the encoding of the response
     let transfer_encoding = Encoding::from(&response);
 
     // Convert the response into a byte stream
+    let mut total_bytes = 0;
     let bytes_stream = response
-        .bytes_stream()
+        .byte_stream_with_progress(reporter)
+        .inspect_ok(|bytes| {
+            total_bytes += bytes.len();
+        })
         .map_err(|e| std::io::Error::new(ErrorKind::Other, e));
 
-    // Listen in on the bytes as they come from the response. Progress is tracked here instead of
-    // after decoding because that doesnt properly represent the number of bytes that are being
-    // transferred over the network.
-    let mut total_bytes = 0;
-    let total_bytes_mut = &mut total_bytes;
-    let bytes_stream = bytes_stream.inspect_ok(move |bytes| {
-        *total_bytes_mut += bytes.len() as u64;
-        if let Some(progress_func) = progress_func.as_mut() {
-            progress_func(DownloadProgress {
-                bytes: *total_bytes_mut,
-                total: content_size,
-            });
-        }
-    });
-
     // Create a new stream from the byte stream that decodes the bytes using the transfer encoding
     // on the fly.
     let decoded_byte_stream = StreamReader::new(bytes_stream).decode(transfer_encoding);
 
     // Create yet another stream that decodes the bytes yet again but this time using the content
     // encoding.
     let mut decoded_repo_data_json_bytes =
@@ -1034,27 +1005,26 @@
 
     // Well then! If we get here, it means the cache must be up to date!
     ValidatedCacheState::UpToDate(cache_state)
 }
 
 #[cfg(test)]
 mod test {
-    use super::{
-        fetch_repo_data, CacheResult, CachedRepoData, DownloadProgress, FetchRepoDataOptions,
-    };
+    use super::{fetch_repo_data, CacheResult, CachedRepoData, FetchRepoDataOptions};
     use crate::fetch::{FetchRepoDataError, RepoDataNotFoundError};
     use crate::utils::simple_channel_server::SimpleChannelServer;
     use crate::utils::Encoding;
+    use crate::Reporter;
     use assert_matches::assert_matches;
     use hex_literal::hex;
     use rattler_networking::AuthenticationMiddleware;
     use reqwest::Client;
     use reqwest_middleware::ClientWithMiddleware;
     use std::path::Path;
-    use std::sync::atomic::{AtomicU64, Ordering};
+    use std::sync::atomic::{AtomicUsize, Ordering};
     use std::sync::Arc;
     use tempfile::TempDir;
     use tokio::io::AsyncWriteExt;
     use url::Url;
 
     async fn write_encoded(
         mut input: &[u8],
@@ -1401,34 +1371,49 @@
     #[tokio::test]
     pub async fn test_progress() {
         // Create a directory with some repodata.
         let subdir_path = TempDir::new().unwrap();
         std::fs::write(subdir_path.path().join("repodata.json"), FAKE_REPO_DATA).unwrap();
         let server = SimpleChannelServer::new(subdir_path.path()).await;
 
-        let last_download_progress = Arc::new(AtomicU64::new(0));
-        let last_download_progress_captured = last_download_progress.clone();
-        let download_progress = move |progress: DownloadProgress| {
-            last_download_progress_captured.store(progress.bytes, Ordering::SeqCst);
-            assert_eq!(progress.total, Some(1110));
-        };
+        struct BasicReporter {
+            last_download_progress: AtomicUsize,
+        }
+
+        impl Reporter for BasicReporter {
+            fn on_download_progress(
+                &self,
+                _url: &Url,
+                _index: usize,
+                bytes_downloaded: usize,
+                total_bytes: Option<usize>,
+            ) {
+                self.last_download_progress
+                    .store(bytes_downloaded, Ordering::SeqCst);
+                assert_eq!(total_bytes, Some(1110));
+            }
+        }
+
+        let reporter = Arc::new(BasicReporter {
+            last_download_progress: AtomicUsize::new(0),
+        });
 
         // Download the data from the channel with an empty cache.
         let cache_dir = TempDir::new().unwrap();
         let _result = fetch_repo_data(
             server.url(),
             ClientWithMiddleware::from(Client::new()),
             cache_dir.into_path(),
             FetchRepoDataOptions::default(),
-            Some(Box::new(download_progress)),
+            Some(reporter.clone()),
         )
         .await
         .unwrap();
 
-        assert_eq!(last_download_progress.load(Ordering::SeqCst), 1110);
+        assert_eq!(reporter.last_download_progress.load(Ordering::SeqCst), 1110);
     }
 
     #[tracing_test::traced_test]
     #[tokio::test]
     pub async fn test_repodata_not_found() {
         // Create a directory with some repodata.
         let subdir_path = TempDir::new().unwrap();
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/lib.rs`

 * *Files 11% similar despite different names*

```diff
@@ -45,23 +45,32 @@
 //!         fetch::FetchRepoDataOptions { ..Default::default() },
 //!         None,
 //!     ).await;
 //!
 //!     let result = match result {
 //!         Err(err) => {
 //!             panic!("{:?}", err);
-//!         },
+//!         }
 //!         Ok(result) => result
 //!     };
 //!
 //!     println!("{:?}", result.cache_state);
 //!     println!("{:?}", result.cache_result);
 //!     println!("{:?}", result.lock_file);
 //!     println!("{:?}", result.repo_data_json_path);
 //! }
 //! ```
 
 pub mod fetch;
+mod reporter;
 #[cfg(feature = "sparse")]
 pub mod sparse;
-
 mod utils;
+pub use reporter::Reporter;
+
+#[cfg(feature = "gateway")]
+mod gateway;
+
+#[cfg(feature = "gateway")]
+pub use gateway::{
+    ChannelConfig, Gateway, GatewayBuilder, GatewayError, RepoData, SourceConfig, SubdirSelection,
+};
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/sparse/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 //! This module provides the [`SparseRepoData`] which is a struct to enable only sparsely loading records
 //! from a `repodata.json` file.
 
 #![allow(clippy::mem_forget)]
 
+use bytes::Bytes;
 use futures::{stream, StreamExt, TryFutureExt, TryStreamExt};
 use itertools::Itertools;
 use rattler_conda_types::{
     compute_package_url, Channel, ChannelInfo, PackageName, PackageRecord, RepoDataRecord,
 };
 use serde::{
     de::{Error, MapAccess, Visitor},
@@ -20,68 +21,123 @@
     path::Path,
 };
 use superslice::Ext;
 
 /// A struct to enable loading records from a `repodata.json` file on demand. Since most of the time you
 /// don't need all the records from the `repodata.json` this can help provide some significant speedups.
 pub struct SparseRepoData {
-    /// Data structure that holds a memory mapped repodata.json file and an index into the the records
-    /// store in that data.
+    /// Data structure that holds an index into the the records stored in a repo data.
     inner: SparseRepoDataInner,
 
     /// The channel from which this data was downloaded.
     channel: Channel,
 
     /// The subdirectory from where the repodata is downloaded
     subdir: String,
 
     /// A function that can be used to patch the package record after it has been parsed.
     /// This is mainly used to add `pip` to `python` if desired
     patch_record_fn: Option<fn(&mut PackageRecord)>,
 }
 
+enum SparseRepoDataInner {
+    /// The repo data is stored as a memory mapped file
+    Memmapped(MemmappedSparseRepoDataInner),
+    /// The repo data is stored as `Bytes`
+    Bytes(BytesSparseRepoDataInner),
+}
+
+impl SparseRepoDataInner {
+    fn borrow_repo_data(&self) -> &LazyRepoData<'_> {
+        match self {
+            SparseRepoDataInner::Memmapped(inner) => inner.borrow_repo_data(),
+            SparseRepoDataInner::Bytes(inner) => inner.borrow_repo_data(),
+        }
+    }
+}
+
 /// A struct that holds a memory map of a `repodata.json` file and also a self-referential field which
 /// indexes the data in the memory map with a sparsely parsed json struct. See [`LazyRepoData`].
-
 #[ouroboros::self_referencing]
-struct SparseRepoDataInner {
+struct MemmappedSparseRepoDataInner {
     /// Memory map of the `repodata.json` file
     memory_map: memmap2::Mmap,
 
     /// Sparsely parsed json content of the memory map. This data struct holds references into the memory
     /// map so we have to use ouroboros to make this legal.
     #[borrows(memory_map)]
     #[covariant]
     repo_data: LazyRepoData<'this>,
 }
 
+/// A struct that holds a reference to the bytes of a `repodata.json` file and also a self-referential
+/// field which indexes the data in the `bytes` with a sparsely parsed json struct. See [`LazyRepoData`].
+#[ouroboros::self_referencing]
+struct BytesSparseRepoDataInner {
+    /// Bytes of the `repodata.json` file
+    bytes: Bytes,
+
+    /// Sparsely parsed json content of the file's bytes. This data struct holds references into the
+    /// bytes so we have to use ouroboros to make this legal.
+    #[borrows(bytes)]
+    #[covariant]
+    repo_data: LazyRepoData<'this>,
+}
+
 impl SparseRepoData {
     /// Construct an instance of self from a file on disk and a [`Channel`].
+    ///
     /// The `patch_function` can be used to patch the package record after it has been parsed
     /// (e.g. to add `pip` to `python`).
     pub fn new(
         channel: Channel,
         subdir: impl Into<String>,
         path: impl AsRef<Path>,
         patch_function: Option<fn(&mut PackageRecord)>,
     ) -> Result<Self, io::Error> {
         let file = std::fs::File::open(path)?;
         let memory_map = unsafe { memmap2::Mmap::map(&file) }?;
         Ok(SparseRepoData {
-            inner: SparseRepoDataInnerTryBuilder {
-                memory_map,
-                repo_data_builder: |memory_map| serde_json::from_slice(memory_map.as_ref()),
-            }
-            .try_build()?,
+            inner: SparseRepoDataInner::Memmapped(
+                MemmappedSparseRepoDataInnerTryBuilder {
+                    memory_map,
+                    repo_data_builder: |memory_map| serde_json::from_slice(memory_map.as_ref()),
+                }
+                .try_build()?,
+            ),
             subdir: subdir.into(),
             channel,
             patch_record_fn: patch_function,
         })
     }
 
+    /// Construct an instance of self from a bytes and a [`Channel`].
+    ///
+    /// The `patch_function` can be used to patch the package record after it has been parsed
+    /// (e.g. to add `pip` to `python`).
+    pub fn from_bytes(
+        channel: Channel,
+        subdir: impl Into<String>,
+        bytes: Bytes,
+        patch_function: Option<fn(&mut PackageRecord)>,
+    ) -> Result<Self, serde_json::Error> {
+        Ok(Self {
+            inner: SparseRepoDataInner::Bytes(
+                BytesSparseRepoDataInnerTryBuilder {
+                    bytes,
+                    repo_data_builder: |bytes| serde_json::from_slice(bytes),
+                }
+                .try_build()?,
+            ),
+            channel,
+            subdir: subdir.into(),
+            patch_record_fn: patch_function,
+        })
+    }
+
     /// Returns an iterator over all package names in this repodata file.
     ///
     /// This works by iterating over all elements in the `packages` and `conda_packages` fields of
     /// the repodata and returning the unique package names.
     pub fn package_names(&self) -> impl Iterator<Item = &'_ str> + '_ {
         let repo_data = self.inner.borrow_repo_data();
         repo_data
@@ -346,15 +402,15 @@
     // - clang-format-13.0.0-default_he082bbe_0.tar.bz2 (package name: clang-format)
     //
     // Because most use-cases involve finding filenames by package name we reorder the entries here
     // by package name. This enables use the binary search for the packages we need.
     //
     // Since (in most cases) the repodata is already ordered by filename which does closely resemble
     // ordering by package name this sort operation will most likely be very fast.
-    entries.sort_by(|(a, _), (b, _)| a.package.cmp(b.package));
+    entries.sort_unstable_by(|(a, _), (b, _)| a.package.cmp(b.package));
 
     Ok(entries)
 }
 
 /// A struct that holds both a filename and the part of the filename thats just the package name.
 struct PackageFilename<'i> {
     package: &'i str,
@@ -382,40 +438,72 @@
             filename: s,
         })
     }
 }
 
 #[cfg(test)]
 mod test {
-    use super::{load_repo_data_recursively, PackageFilename};
+    use super::{load_repo_data_recursively, PackageFilename, SparseRepoData};
+    use bytes::Bytes;
     use rattler_conda_types::{Channel, ChannelConfig, PackageName, RepoData, RepoDataRecord};
     use rstest::rstest;
     use std::path::{Path, PathBuf};
 
     fn test_dir() -> PathBuf {
         Path::new(env!("CARGO_MANIFEST_DIR")).join("../../test-data")
     }
 
+    fn default_repo_datas() -> Vec<(Channel, &'static str, PathBuf)> {
+        let channel_config = ChannelConfig::default_with_root_dir(std::env::current_dir().unwrap());
+        vec![
+            (
+                Channel::from_str("conda-forge", &channel_config).unwrap(),
+                "noarch",
+                test_dir().join("channels/conda-forge/noarch/repodata.json"),
+            ),
+            (
+                Channel::from_str("conda-forge", &channel_config).unwrap(),
+                "linux-64",
+                test_dir().join("channels/conda-forge/linux-64/repodata.json"),
+            ),
+        ]
+    }
+
+    fn default_repo_data_bytes() -> Vec<(Channel, &'static str, Bytes)> {
+        default_repo_datas()
+            .into_iter()
+            .map(|(channel, subdir, path)| {
+                let bytes = std::fs::read(path).unwrap();
+                (channel, subdir, bytes.into())
+            })
+            .collect()
+    }
+
+    fn load_sparse_from_bytes(
+        repo_datas: &[(Channel, &'static str, Bytes)],
+        package_names: impl IntoIterator<Item = impl AsRef<str>>,
+    ) -> Vec<Vec<RepoDataRecord>> {
+        let sparse: Vec<_> = repo_datas
+            .iter()
+            .map(|(channel, subdir, bytes)| {
+                SparseRepoData::from_bytes(channel.clone(), *subdir, bytes.clone(), None).unwrap()
+            })
+            .collect();
+
+        let package_names = package_names
+            .into_iter()
+            .map(|name| PackageName::try_from(name.as_ref()).unwrap());
+        SparseRepoData::load_records_recursive(&sparse, package_names, None).unwrap()
+    }
+
     async fn load_sparse(
         package_names: impl IntoIterator<Item = impl AsRef<str>>,
     ) -> Vec<Vec<RepoDataRecord>> {
-        let channel_config = ChannelConfig::default_with_root_dir(std::env::current_dir().unwrap());
         load_repo_data_recursively(
-            [
-                (
-                    Channel::from_str("conda-forge", &channel_config).unwrap(),
-                    "noarch",
-                    test_dir().join("channels/conda-forge/noarch/repodata.json"),
-                ),
-                (
-                    Channel::from_str("conda-forge", &channel_config).unwrap(),
-                    "linux-64",
-                    test_dir().join("channels/conda-forge/linux-64/repodata.json"),
-                ),
-            ],
+            default_repo_datas(),
             package_names
                 .into_iter()
                 .map(|name| PackageName::try_from(name.as_ref()).unwrap()),
             None,
         )
         .await
         .unwrap()
@@ -459,16 +547,28 @@
             .map(std::vec::Vec::len)
             .sum::<usize>();
 
         assert_eq!(total_records, 21732);
     }
 
     #[tokio::test]
+    async fn test_sparse_rubin_env() {
+        let sparse_empty_data = load_sparse(["rubin-env"]).await;
+
+        let total_records = sparse_empty_data
+            .iter()
+            .map(std::vec::Vec::len)
+            .sum::<usize>();
+
+        assert_eq!(total_records, 45060);
+    }
+
+    #[tokio::test]
     async fn test_sparse_numpy_dev() {
-        let sparse_empty_data = load_sparse([
+        let package_names = vec![
             "python",
             "cython",
             "compilers",
             "openblas",
             "nomkl",
             "pytest",
             "pytest-cov",
@@ -483,21 +583,28 @@
             "pandas",
             "matplotlib",
             "pydata-sphinx-theme",
             "pycodestyle",
             "gitpython",
             "cffi",
             "pytz",
-        ])
-        .await;
+        ];
 
-        let total_records = sparse_empty_data
-            .iter()
-            .map(std::vec::Vec::len)
-            .sum::<usize>();
+        // Memmapped
+        let sparse_empty_data = load_sparse(package_names.clone()).await;
+
+        let total_records = sparse_empty_data.iter().map(Vec::len).sum::<usize>();
+
+        assert_eq!(total_records, 16065);
+
+        // Bytes
+        let repo_datas = default_repo_data_bytes();
+        let sparse_empty_data = load_sparse_from_bytes(&repo_datas, package_names);
+
+        let total_records = sparse_empty_data.iter().map(Vec::len).sum::<usize>();
 
         assert_eq!(total_records, 16065);
     }
 
     #[test]
     fn load_complete_records() {
         let mut records = Vec::new();
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/encoding.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/flock.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+use ::url::Url;
+pub use body::BodyStreamExt;
 pub use encoding::{AsyncEncoding, Encoding};
 pub use flock::LockedFile;
 use std::fmt::Write;
-use url::Url;
 
 mod encoding;
 
 #[cfg(test)]
 pub(crate) mod simple_channel_server;
 
+mod body;
 mod flock;
 
 /// Convert a URL to a cache filename
 pub(crate) fn url_to_cache_filename(url: &Url) -> String {
     // Start Rant:
     // This function mimics behavior from Mamba which itself mimics this behavior from Conda.
     // However, I find this function absolutely ridiculous, it contains all sort of weird edge
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs` & `py_rattler-0.6.0/local_dependencies/rattler_repodata_gateway/src/utils/simple_channel_server.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 use axum::routing::get_service;
-use std::future::IntoFuture;
-use std::net::SocketAddr;
-use std::path::Path;
+use rattler_conda_types::Channel;
+use std::{future::IntoFuture, net::SocketAddr, path::Path};
 use tokio::sync::oneshot;
 use tower_http::services::ServeDir;
 use url::Url;
 
 pub struct SimpleChannelServer {
     local_addr: SocketAddr,
     shutdown_sender: Option<oneshot::Sender<()>>,
 }
 
 impl SimpleChannelServer {
     /// Returns the root `Url` to the server.
     pub fn url(&self) -> Url {
         Url::parse(&format!("http://localhost:{}", self.local_addr.port())).unwrap()
     }
+
+    #[allow(dead_code)]
+    pub fn channel(&self) -> Channel {
+        Channel::from_url(self.url())
+    }
 }
 
 impl SimpleChannelServer {
     pub async fn new(path: impl AsRef<Path>) -> Self {
         // Define a service to serve the contents of the folder. The `precompressed_gzip` method
         // adds the behavior that a file gzip compressed file called `<path>.gz` is preferred over
         // the original file. This is very useful because we can store gzipped compressed files in
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/Cargo.toml` & `py_rattler-0.6.0/local_dependencies/rattler_lock/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 [package]
-name = "rattler_conda_types"
-version = "0.22.0"
+name = "rattler_lock"
+version = "0.22.8"
 edition= "2021"
 authors = ["Bas Zalmstra <zalmstra.bas@gmail.com>"]
-description = "Rust data types for common types used within the Conda ecosystem"
+description = "Rust data types for conda lock"
 categories= ["conda"]
 homepage= "https://github.com/mamba-org/rattler"
 repository= "https://github.com/mamba-org/rattler"
 license= "BSD-3-Clause"
 readme= "README.md"
 resolver = "2"
 
 [dependencies]
-rattler_digest = { path= "../rattler_digest", version = "0.19.3", default-features = false, features = ["serde"] }
-rattler_macros = { path= "../rattler_macros", version = "0.19.3", default-features = false }
+rattler_conda_types = { path = "../rattler_conda_types", version = "0.24.0", default-features = false }
+rattler_digest = { path = "../rattler_digest", version = "0.19.4", default-features = false }
+file_url = { path = "../file_url", version = "0.1.1" }
 chrono = { version = "0.4.38", default-features = false, features = [
     "std",
     "serde",
     "alloc",
 ] }
 fxhash = "0.2.1"
-glob = "0.3.1"
-hex = "0.4.3"
+indexmap = { version = "2.2.6", features = ["serde"] }
 itertools = "0.12.1"
-lazy-regex = "3.1.0"
-nom = "7.1.3"
-purl = { version = "0.1.2", features = ["serde","serde"] }
-regex = "1.10.4"
-serde = { version = "1.0.198" , features = ["derive", "rc"] }
+pep508_rs = { version = "0.4.2" , features = ["serde"] }
+pep440_rs = { version = "0.5.0" , features = ["serde"] }
+serde = { version = "1.0.198" , features = ["derive"] }
 serde_json = { version = "1.0.116" }
-serde_repr = "0.1"
+serde_yaml = "0.9.34"
 serde_with = { version = "3.7.0", features = ["indexmap_2"] }
-smallvec = { version = "1.13.2", features = [
-    "serde",
-    "const_new",
-    "const_generics",
-    "union","serde", "const_new", "const_generics", "union",
-] }
-strum = { version = "0.26.2", features = ["derive","derive"] }
+serde_repr = "0.1"
 thiserror = "1.0"
-tracing = "0.1.40"
 url = { version = "2.5.0" , features = ["serde"] }
-
-[[bench]]
-name = "parse"
-harness = false
+purl = { version = "0.1.2", features = ["serde","serde"] }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,42 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.24.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.23.1...rattler_conda_types-v0.24.0) - 2024-05-27
+
+### Added
+- removed Ord and more ([#673](https://github.com/mamba-org/rattler/pull/673))
+- always store purls as a key in lock file ([#669](https://github.com/mamba-org/rattler/pull/669))
+- add solve strategies ([#660](https://github.com/mamba-org/rattler/pull/660))
+
+### Fixed
+- make topological sorting support fully cyclic dependencies ([#678](https://github.com/mamba-org/rattler/pull/678))
+
+## [0.23.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.23.0...rattler_conda_types-v0.23.1) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+## [0.23.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.22.1...rattler_conda_types-v0.23.0) - 2024-05-13
+
+### Added
+- high level repodata access ([#560](https://github.com/mamba-org/rattler/pull/560))
+
+### Other
+- update README.md
+
+## [0.22.1](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.22.0...rattler_conda_types-v0.22.1) - 2024-05-06
+
+### Added
+- expose `*Record.noarch` in Python bindings ([#635](https://github.com/mamba-org/rattler/pull/635))
+
 ## [0.22.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.21.0...rattler_conda_types-v0.22.0) - 2024-04-25
 
 ### Added
 - add support for extracting prefix placeholder data to PathsEntry ([#614](https://github.com/mamba-org/rattler/pull/614))
 
 ## [0.21.0](https://github.com/mamba-org/rattler/compare/rattler_conda_types-v0.20.5...rattler_conda_types-v0.21.0) - 2024-04-19
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/benches/parse.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/benches/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/build_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/channel/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel/mod.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 use itertools::Itertools;
 use std::borrow::Cow;
 use std::fmt::{Display, Formatter};
-use std::path::{Component, Path, PathBuf};
+use std::path::{Path, PathBuf};
 use std::str::FromStr;
 
+use file_url::directory_path_to_url;
 use serde::{Deserialize, Serialize};
-use smallvec::SmallVec;
 use thiserror::Error;
+use typed_path::{Utf8NativePathBuf, Utf8TypedPath, Utf8TypedPathBuf};
 use url::Url;
 
 use super::{ParsePlatformError, Platform};
 
 const DEFAULT_CHANNEL_ALIAS: &str = "https://conda.anaconda.org";
 
 /// The `ChannelConfig` describes properties that are required to resolve "simple" channel names to
@@ -117,15 +118,15 @@
 
 /// `Channel`s are the primary source of package information.
 #[derive(Debug, Clone, Serialize, Eq, PartialEq, Hash)]
 pub struct Channel {
     /// The platforms supported by this channel, or None if no explicit platforms have been
     /// specified.
     #[serde(skip_serializing_if = "Option::is_none")]
-    pub platforms: Option<SmallVec<[Platform; 2]>>,
+    pub platforms: Option<Vec<Platform>>,
 
     /// Base URL of the channel, everything is relative to this url.
     pub base_url: Url,
 
     /// The name of the channel
     pub name: Option<String>,
 }
@@ -137,45 +138,53 @@
         config: &ChannelConfig,
     ) -> Result<Self, ParseChannelError> {
         let str = str.as_ref();
         let (platforms, channel) = parse_platforms(str)?;
 
         let channel = if parse_scheme(channel).is_some() {
             let url = Url::parse(channel)?;
-            Channel::from_url(url, platforms, config)
+            Channel {
+                platforms,
+                ..Channel::from_url(url)
+            }
         } else if is_path(channel) {
-            let path = PathBuf::from(channel);
-
             #[cfg(target_arch = "wasm32")]
             return Err(ParseChannelError::InvalidPath(path));
 
             #[cfg(not(target_arch = "wasm32"))]
             {
-                let absolute_path = absolute_path(&path, &config.root_dir);
-                let url = Url::from_directory_path(absolute_path)
-                    .map_err(|_err| ParseChannelError::InvalidPath(path))?;
+                let absolute_path = absolute_path(channel, &config.root_dir)?;
+                let url = directory_path_to_url(absolute_path.to_path())
+                    .map_err(|_err| ParseChannelError::InvalidPath(channel.to_owned()))?;
                 Self {
                     platforms,
                     base_url: url,
                     name: Some(channel.to_owned()),
                 }
             }
         } else {
-            Channel::from_name(channel, platforms, config)
+            Channel {
+                platforms,
+                ..Channel::from_name(channel, config)
+            }
         };
 
         Ok(channel)
     }
 
+    /// Set the explicit platforms of the channel.
+    pub fn with_explicit_platforms(self, platforms: impl IntoIterator<Item = Platform>) -> Self {
+        Self {
+            platforms: Some(platforms.into_iter().collect()),
+            ..self
+        }
+    }
+
     /// Constructs a new [`Channel`] from a `Url` and associated platforms.
-    pub fn from_url(
-        url: Url,
-        platforms: Option<impl Into<SmallVec<[Platform; 2]>>>,
-        _config: &ChannelConfig,
-    ) -> Self {
+    pub fn from_url(url: Url) -> Self {
         // Get the path part of the URL but trim the directory suffix
         let path = url.path().trim_end_matches('/');
 
         // Ensure that the base_url does always ends in a `/`
         let base_url = if url.path().ends_with('/') {
             url.clone()
         } else {
@@ -191,56 +200,75 @@
         // Case 4: custom_channels matches
         // Case 5: channel_alias match
 
         if base_url.has_host() {
             // Case 7: Fallback
             let name = path.trim_start_matches('/');
             Self {
-                platforms: platforms.map(Into::into),
+                platforms: None,
                 name: (!name.is_empty()).then_some(name).map(str::to_owned),
                 base_url,
             }
         } else {
             // Case 6: non-otherwise-specified file://-type urls
             let name = path
                 .rsplit_once('/')
                 .map_or_else(|| base_url.path(), |(_, path_part)| path_part);
             Self {
-                platforms: platforms.map(Into::into),
+                platforms: None,
                 name: (!name.is_empty()).then_some(name).map(str::to_owned),
                 base_url,
             }
         }
     }
 
     /// Construct a channel from a name, platform and configuration.
-    pub fn from_name(
-        name: &str,
-        platforms: Option<SmallVec<[Platform; 2]>>,
-        config: &ChannelConfig,
-    ) -> Self {
+    pub fn from_name(name: &str, config: &ChannelConfig) -> Self {
         // TODO: custom channels
 
         let dir_name = if name.ends_with('/') {
             Cow::Borrowed(name)
         } else {
             Cow::Owned(format!("{name}/"))
         };
 
         let name = name.trim_end_matches('/');
         Self {
-            platforms,
+            platforms: None,
             base_url: config
                 .channel_alias
                 .join(dir_name.as_ref())
                 .expect("name is not a valid Url"),
             name: (!name.is_empty()).then_some(name).map(str::to_owned),
         }
     }
 
+    /// Constructs a channel from a directory path.
+    ///
+    /// # Panics
+    ///
+    /// Panics if the path is not an absolute path or could not be canonicalized.
+    pub fn from_directory(path: &Path) -> Self {
+        let path = if path.is_absolute() {
+            Cow::Borrowed(path)
+        } else {
+            Cow::Owned(
+                path.canonicalize()
+                    .expect("path is a not a valid absolute path"),
+            )
+        };
+
+        let url = Url::from_directory_path(path).expect("path is a valid url");
+        Self {
+            platforms: None,
+            base_url: url,
+            name: None,
+        }
+    }
+
     /// Returns the name of the channel
     pub fn name(&self) -> &str {
         match self.base_url().scheme() {
             // The name of the channel is only defined for http and https channels.
             // If the name is not defined we return the base url.
             "https" | "http" => self
                 .name
@@ -294,16 +322,24 @@
     ParsePlatformError(#[source] ParsePlatformError),
 
     /// Error when the url could not be parsed.
     #[error("could not parse url")]
     ParseUrlError(#[source] url::ParseError),
 
     /// Error when the path is invalid.
-    #[error("invalid path '{0}")]
-    InvalidPath(PathBuf),
+    #[error("invalid path '{0}'")]
+    InvalidPath(String),
+
+    /// The root directory is not an absolute path
+    #[error("root directory from channel config is not an absolute path")]
+    NonAbsoluteRootDir(PathBuf),
+
+    /// The root directory is not UTF-8 encoded.
+    #[error("root directory of channel config is not utf8 encoded")]
+    NotUtf8RootDir(PathBuf),
 }
 
 impl From<ParsePlatformError> for ParseChannelError {
     fn from(err: ParsePlatformError) -> Self {
         ParseChannelError::ParsePlatformError(err)
     }
 }
@@ -312,26 +348,24 @@
     fn from(err: url::ParseError) -> Self {
         ParseChannelError::ParseUrlError(err)
     }
 }
 
 /// Extract the platforms from the given human readable channel.
 #[allow(clippy::type_complexity)]
-fn parse_platforms(
-    channel: &str,
-) -> Result<(Option<SmallVec<[Platform; 2]>>, &str), ParsePlatformError> {
+fn parse_platforms(channel: &str) -> Result<(Option<Vec<Platform>>, &str), ParsePlatformError> {
     if channel.rfind(']').is_some() {
         if let Some(start_platform_idx) = channel.find('[') {
             let platform_part = &channel[start_platform_idx + 1..channel.len() - 1];
-            let platforms: SmallVec<_> = platform_part
+            let platforms = platform_part
                 .split(',')
                 .map(str::trim)
                 .filter(|s| !s.is_empty())
                 .map(FromStr::from_str)
-                .collect::<Result<_, _>>()?;
+                .collect::<Result<Vec<_>, _>>()?;
             let platforms = if platforms.is_empty() {
                 None
             } else {
                 Some(platforms)
             };
             return Ok((platforms, &channel[0..start_platform_idx]));
         }
@@ -390,129 +424,84 @@
     }
 
     // A drive letter followed by a colon and a (backward or forward) slash
     matches!(path.chars().take(3).collect_tuple(),
         Some((letter, ':', '/' | '\\')) if letter.is_alphabetic())
 }
 
-/// Normalizes a file path by eliminating `..` and `.`.
-fn normalize_path(path: &Path) -> PathBuf {
-    let mut components = path.components().peekable();
-    let mut ret = if let Some(c @ Component::Prefix(..)) = components.peek().cloned() {
-        components.next();
-        PathBuf::from(c.as_os_str())
-    } else {
-        PathBuf::new()
-    };
-
-    for component in components {
-        match component {
-            Component::Prefix(..) => unreachable!(),
-            Component::RootDir => {
-                ret.push(component.as_os_str());
-            }
-            Component::CurDir => {}
-            Component::ParentDir => {
-                ret.pop();
-            }
-            Component::Normal(c) => {
-                ret.push(c);
-            }
-        }
-    }
-    ret
-}
-
 /// Returns the specified path as an absolute path
-fn absolute_path<'a>(path: &'a Path, root_dir: &Path) -> Cow<'a, Path> {
+fn absolute_path(path: &str, root_dir: &Path) -> Result<Utf8TypedPathBuf, ParseChannelError> {
+    let path = Utf8TypedPath::from(path);
     if path.is_absolute() {
-        return Cow::Borrowed(path);
+        return Ok(path.normalize());
+    }
+
+    let root_dir_str = root_dir
+        .to_str()
+        .ok_or_else(|| ParseChannelError::NotUtf8RootDir(root_dir.to_path_buf()))?;
+    let native_root_dir = Utf8NativePathBuf::from(root_dir_str);
+
+    if !native_root_dir.is_absolute() {
+        return Err(ParseChannelError::NonAbsoluteRootDir(
+            root_dir.to_path_buf(),
+        ));
     }
 
-    let absolute_dir = root_dir.join(path);
-    Cow::Owned(normalize_path(&absolute_dir))
+    Ok(native_root_dir.to_typed_path().join(path).normalize())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
-    use smallvec::smallvec;
-    use std::{
-        path::{Path, PathBuf},
-        str::FromStr,
-    };
+    use std::str::FromStr;
     use url::Url;
 
     #[test]
     fn test_parse_platforms() {
         assert_eq!(
             parse_platforms("[noarch, linux-64]"),
-            Ok((Some(smallvec![Platform::NoArch, Platform::Linux64]), ""))
+            Ok((Some(vec![Platform::NoArch, Platform::Linux64]), ""))
         );
         assert_eq!(
             parse_platforms("sometext[noarch]"),
-            Ok((Some(smallvec![Platform::NoArch]), "sometext"))
+            Ok((Some(vec![Platform::NoArch]), "sometext"))
         );
         assert_eq!(
             parse_platforms("sometext[noarch,]"),
-            Ok((Some(smallvec![Platform::NoArch]), "sometext"))
+            Ok((Some(vec![Platform::NoArch]), "sometext"))
         );
         assert_eq!(parse_platforms("sometext[]"), Ok((None, "sometext")));
         assert!(matches!(
             parse_platforms("[notaplatform]"),
             Err(ParsePlatformError { .. })
         ));
     }
 
     #[test]
-    fn test_normalize_path() {
-        assert_eq!(
-            normalize_path(Path::new("foo/bar")),
-            PathBuf::from("foo/bar")
-        );
-        assert_eq!(
-            normalize_path(Path::new("foo/bar/")),
-            PathBuf::from("foo/bar/")
-        );
-        assert_eq!(
-            normalize_path(Path::new("./foo/bar")),
-            PathBuf::from("foo/bar")
-        );
-        assert_eq!(
-            normalize_path(Path::new("./foo/../bar")),
-            PathBuf::from("bar")
-        );
-        assert_eq!(
-            normalize_path(Path::new("./foo/../bar/..")),
-            PathBuf::from("")
-        );
-    }
-
-    #[test]
     fn test_absolute_path() {
         let current_dir = std::env::current_dir().expect("no current dir?");
+        let native_current_dir = typed_path::utils::utf8_current_dir()
+            .expect("")
+            .to_typed_path_buf();
         assert_eq!(
-            absolute_path(Path::new("."), &current_dir).as_ref(),
-            &current_dir
+            absolute_path(".", &current_dir).as_ref(),
+            Ok(&native_current_dir)
         );
         assert_eq!(
-            absolute_path(Path::new("foo"), &current_dir).as_ref(),
-            &current_dir.join("foo")
+            absolute_path("foo", &current_dir).as_ref(),
+            Ok(&native_current_dir.join("foo"))
         );
 
-        let mut parent_dir = current_dir.clone();
+        let mut parent_dir = native_current_dir.clone();
         assert!(parent_dir.pop());
 
+        assert_eq!(absolute_path("..", &current_dir).as_ref(), Ok(&parent_dir));
         assert_eq!(
-            absolute_path(Path::new(".."), &current_dir).as_ref(),
-            &parent_dir
-        );
-        assert_eq!(
-            absolute_path(Path::new("../foo"), &current_dir).as_ref(),
-            &parent_dir.join("foo")
+            absolute_path("../foo", &current_dir).as_ref(),
+            Ok(&parent_dir.join("foo"))
         );
     }
 
     #[test]
     fn test_parse_scheme() {
         assert_eq!(parse_scheme("https://google.com"), Some("https"));
         assert_eq!(parse_scheme("http://google.com"), Some("http"));
@@ -535,15 +524,15 @@
             channel.base_url,
             Url::from_str("https://conda.anaconda.org/conda-forge/").unwrap()
         );
         assert_eq!(channel.name.as_deref(), Some("conda-forge"));
         assert_eq!(channel.name(), "conda-forge");
         assert_eq!(channel.platforms, None);
 
-        assert_eq!(channel, Channel::from_name("conda-forge/", None, &config));
+        assert_eq!(channel, Channel::from_name("conda-forge/", &config));
     }
 
     #[test]
     fn parse_from_url() {
         let config = ChannelConfig::default_with_root_dir(std::env::current_dir().unwrap());
 
         let channel =
@@ -577,22 +566,20 @@
             channel.base_url().to_string(),
             "file:///var/channels/conda-forge/"
         );
 
         let current_dir = std::env::current_dir().expect("no current dir?");
         let channel = Channel::from_str("./dir/does/not_exist", &config).unwrap();
         assert_eq!(channel.name.as_deref(), Some("./dir/does/not_exist"));
+        let expected = absolute_path("./dir/does/not_exist", &current_dir).unwrap();
         assert_eq!(
             channel.name(),
-            Url::from_directory_path(absolute_path(
-                Path::new("./dir/does/not_exist"),
-                &current_dir
-            ))
-            .unwrap()
-            .as_str()
+            file_url::directory_path_to_url(expected.to_path())
+                .unwrap()
+                .as_str()
         );
         assert_eq!(channel.platforms, None);
         assert_eq!(
             channel.base_url().to_file_path().unwrap(),
             current_dir.join("dir/does/not_exist")
         );
     }
@@ -630,27 +617,27 @@
         )
         .unwrap();
         assert_eq!(
             channel.base_url,
             Url::from_str("https://conda.anaconda.org/conda-forge/").unwrap()
         );
         assert_eq!(channel.name.as_deref(), Some("conda-forge"));
-        assert_eq!(channel.platforms, Some(smallvec![platform]));
+        assert_eq!(channel.platforms, Some(vec![platform]));
 
         let channel = Channel::from_str(
             format!("https://conda.anaconda.org/pkgs/main[{platform}]"),
             &config,
         )
         .unwrap();
         assert_eq!(
             channel.base_url,
             Url::from_str("https://conda.anaconda.org/pkgs/main/").unwrap()
         );
         assert_eq!(channel.name.as_deref(), Some("pkgs/main"));
-        assert_eq!(channel.platforms, Some(smallvec![platform]));
+        assert_eq!(channel.platforms, Some(vec![platform]));
 
         let channel = Channel::from_str("conda-forge/label/rust_dev", &config).unwrap();
         assert_eq!(
             channel.base_url,
             Url::from_str("https://conda.anaconda.org/conda-forge/label/rust_dev/").unwrap()
         );
         assert_eq!(channel.name.as_deref(), Some("conda-forge/label/rust_dev"));
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/channel_data.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/channel_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/explicit_environment_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 pub use match_spec::{MatchSpec, NamelessMatchSpec};
 pub use no_arch_type::{NoArchKind, NoArchType};
 pub use package_name::{InvalidPackageNameError, PackageName};
 pub use parse_mode::ParseStrictness;
 pub use platform::{Arch, ParseArchError, ParsePlatformError, Platform};
 pub use prefix_record::PrefixRecord;
 pub use repo_data::patches::{PackageRecordPatch, PatchInstructions, RepoDataPatch};
+pub use repo_data::sharded::{Shard, ShardedRepodata, ShardedSubdirInfo};
 pub use repo_data::{
     compute_package_url, ChannelInfo, ConvertSubdirError, PackageRecord, RepoData,
 };
 pub use repo_data_record::RepoDataRecord;
 pub use run_export::RunExportKind;
 pub use version::{
     Component, ParseVersionError, ParseVersionErrorKind, StrictVersion, Version, VersionBumpError,
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/matcher.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -249,14 +249,24 @@
                 md5: self.md5,
                 sha256: self.sha256,
             },
         )
     }
 }
 
+// Enable constructing a match spec from a package name.
+impl From<PackageName> for MatchSpec {
+    fn from(value: PackageName) -> Self {
+        Self {
+            name: Some(value),
+            ..Default::default()
+        }
+    }
+}
+
 /// Similar to a [`MatchSpec`] but does not include the package name. This is useful in places
 /// where the package name is already known (e.g. `foo = "3.4.1 *cuda"`)
 #[serde_as]
 #[skip_serializing_none]
 #[derive(Debug, Default, Clone, Serialize, Deserialize, Eq, PartialEq, Hash)]
 pub struct NamelessMatchSpec {
     /// The version spec of the package (e.g. `1.2.3`, `>=1.2.3`, `1.2.*`)
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/match_spec/snapshots/rattler_conda_types__match_spec__tests__serialize_matchspec.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/no_arch_type.rs`

 * *Files 8% similar despite different names*

```diff
@@ -47,14 +47,19 @@
     }
 
     /// Returns true if this instance is a Python noarch type
     pub fn is_python(&self) -> bool {
         self.kind() == Some(NoArchKind::Python)
     }
 
+    /// Returns true if this instance is a Generic noarch type
+    pub fn is_generic(&self) -> bool {
+        self.kind() == Some(NoArchKind::Generic)
+    }
+
     /// Constructs a Python noarch instance.
     pub fn python() -> Self {
         Self(Some(RawNoArchType::Python))
     }
 
     /// Constructs a Generic noarch instance.
     pub fn generic() -> Self {
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/about.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/about.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_identifier.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/archive_type.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/files.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/files.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/has_prefix.rs`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,25 @@
                     file_mode,
                     multispace1,
                     possibly_quoted_string,
                 )),
                 |(prefix, _, file_mode, _, path)| HasPrefixEntry {
                     prefix: Cow::Owned(prefix.into_owned()),
                     file_mode,
-                    relative_path: PathBuf::from(path.as_ref()),
+                    relative_path: PathBuf::from(&*path),
                 },
             ))(buf)
         }
 
         /// Parses "<path>" and fails if there is more input.
         fn only_path(buf: &str) -> IResult<&str, HasPrefixEntry> {
             all_consuming(map(possibly_quoted_string, |path| HasPrefixEntry {
                 prefix: Cow::Borrowed(placeholder_string()),
                 file_mode: FileMode::Text,
-                relative_path: PathBuf::from(path.as_ref()),
+                relative_path: PathBuf::from(&*path),
             }))(buf)
         }
 
         /// Parses "text|binary" as a [`FileMode`]
         fn file_mode(buf: &str) -> IResult<&str, FileMode> {
             alt((
                 value(FileMode::Text, tag_no_case("text")),
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/index.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/link.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/no_link.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_link.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/no_softlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/paths.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/paths.rs`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                     let path_type = path_type(&path);
 
                     match path_type {
                         Ok(path_type) => Ok(PathsEntry {
                             path_type,
                             prefix_placeholder: prefix.map(|entry| PrefixPlaceholder {
                                 file_mode: entry.file_mode,
-                                placeholder: entry.prefix.as_ref().to_owned(),
+                                placeholder: (*entry.prefix).to_owned(),
                             }),
                             no_link: no_link.contains(&path),
                             sha256: None,
                             size_in_bytes: None,
                             relative_path: path,
                         }),
                         Err(e) => Err(e),
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/run_exports.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__about__test__reconstruct_about_json_mamba.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__paths_sorted.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__reconstruct_paths_json_with_symlinks.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package/snapshots/rattler_conda_types__package__paths__test__roundtrip_paths_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/package_name.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/platform.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/platform.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/prefix_record.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/prefix_record.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-//! Defines [`RepoData`]. `RepoData` stores information of all packages present in a subdirectory
-//! of a channel. It provides indexing functionality.
+//! Defines [`RepoData`]. `RepoData` stores information of all packages present
+//! in a subdirectory of a channel. It provides indexing functionality.
 
 pub mod patches;
+pub mod sharded;
 mod topological_sort;
 
-use std::borrow::Cow;
-use std::collections::{BTreeMap, BTreeSet};
-use std::fmt::{Display, Formatter};
-use std::path::Path;
+use std::{
+    borrow::Cow,
+    collections::{BTreeMap, BTreeSet},
+    fmt::{Display, Formatter},
+    path::Path,
+};
 
 use fxhash::{FxHashMap, FxHashSet};
-
 use rattler_digest::{serde::SerializableHash, Md5Hash, Sha256Hash};
+use rattler_macros::sorted;
 use serde::{Deserialize, Serialize};
 use serde_with::{serde_as, skip_serializing_none, OneOrMany};
 use thiserror::Error;
 use url::Url;
 
-use rattler_macros::sorted;
-
 use crate::{
     build_spec::BuildNumber, package::IndexJson, utils::serde::DeserializeFromStrUnchecked,
     Channel, NoArchType, PackageName, PackageUrl, Platform, RepoDataRecord, VersionWithSource,
 };
 
-/// [`RepoData`] is an index of package binaries available on in a subdirectory of a Conda channel.
+/// [`RepoData`] is an index of package binaries available on in a subdirectory
+/// of a Conda channel.
 // Note: we cannot use the sorted macro here, because the `packages` and `conda_packages` fields are
 // serialized in a special way. Therefore we do it manually.
 #[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Clone)]
 pub struct RepoData {
     /// The channel information contained in the repodata.json file
     pub info: Option<ChannelInfo>,
 
     /// The tar.bz2 packages contained in the repodata.json file
     #[serde(serialize_with = "sort_map_alphabetically")]
     pub packages: FxHashMap<String, PackageRecord>,
 
-    /// The conda packages contained in the repodata.json file (under a different key for
-    /// backwards compatibility with previous conda versions)
+    /// The conda packages contained in the repodata.json file (under a
+    /// different key for backwards compatibility with previous conda
+    /// versions)
     #[serde(
         default,
         rename = "packages.conda",
         serialize_with = "sort_map_alphabetically"
     )]
     pub conda_packages: FxHashMap<String, PackageRecord>,
 
-    /// removed packages (files are still accessible, but they are not installable like regular packages)
+    /// removed packages (files are still accessible, but they are not
+    /// installable like regular packages)
     #[serde(
         default,
         serialize_with = "sort_set_alphabetically",
         skip_serializing_if = "FxHashSet::is_empty"
     )]
     pub removed: FxHashSet<String>,
 
@@ -65,43 +69,45 @@
     pub subdir: String,
 
     /// The base_url for all package urls. Can be an absolute or relative url.
     #[serde(skip_serializing_if = "Option::is_none")]
     pub base_url: Option<String>,
 }
 
-/// A single record in the Conda repodata. A single record refers to a single binary distribution
-/// of a package on a Conda channel.
+/// A single record in the Conda repodata. A single record refers to a single
+/// binary distribution of a package on a Conda channel.
 #[serde_as]
 #[skip_serializing_none]
 #[sorted]
-#[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Ord, PartialOrd, Clone, Hash)]
+#[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Clone, Hash)]
 pub struct PackageRecord {
     /// Optionally the architecture the package supports
     pub arch: Option<String>,
 
     /// The build string of the package
     pub build: String,
 
     /// The build number of the package
     pub build_number: BuildNumber,
 
-    /// Additional constraints on packages. `constrains` are different from `depends` in that packages
-    /// specified in `depends` must be installed next to this package, whereas packages specified in
-    /// `constrains` are not required to be installed, but if they are installed they must follow these
-    /// constraints.
+    /// Additional constraints on packages. `constrains` are different from
+    /// `depends` in that packages specified in `depends` must be installed
+    /// next to this package, whereas packages specified in `constrains` are
+    /// not required to be installed, but if they are installed they must follow
+    /// these constraints.
     #[serde(default, skip_serializing_if = "Vec::is_empty")]
     pub constrains: Vec<String>,
 
     /// Specification of packages this package depends on
     #[serde(default)]
     pub depends: Vec<String>,
 
-    /// Features are a deprecated way to specify different feature sets for the conda solver. This is not
-    /// supported anymore and should not be used. Instead, `mutex` packages should be used to specify
+    /// Features are a deprecated way to specify different feature sets for the
+    /// conda solver. This is not supported anymore and should not be used.
+    /// Instead, `mutex` packages should be used to specify
     /// mutually exclusive features.
     pub features: Option<String>,
 
     /// A deprecated md5 hash
     pub legacy_bz2_md5: Option<String>,
 
     /// A deprecated package archive size.
@@ -117,26 +123,33 @@
     #[serde_as(as = "Option<SerializableHash::<rattler_digest::Md5>>")]
     pub md5: Option<Md5Hash>,
 
     /// The name of the package
     #[serde_as(deserialize_as = "DeserializeFromStrUnchecked")]
     pub name: PackageName,
 
-    /// If this package is independent of architecture this field specifies in what way. See
-    /// [`NoArchType`] for more information.
+    /// If this package is independent of architecture this field specifies in
+    /// what way. See [`NoArchType`] for more information.
     #[serde(skip_serializing_if = "NoArchType::is_none")]
     pub noarch: NoArchType,
 
     /// Optionally the platform the package supports
     pub platform: Option<String>, // Note that this does not match the [`Platform`] enum..
 
-    /// Package identifiers of packages that are equivalent to this package but from other
-    /// ecosystems.
-    #[serde(default, skip_serializing_if = "Vec::is_empty")]
-    pub purls: Vec<PackageUrl>,
+    /// Package identifiers of packages that are equivalent to this package but
+    /// from other ecosystems.
+    /// starting from 0.23.2, this field became [`Option<Vec<PackageUrl>>`].
+    /// This was done to support older lockfiles,
+    /// where we didn't differentiate between empty purl and missing one.
+    /// Now, None:: means that the purl is missing, and it will be tried to
+    /// filled in. So later it can be one of the following:
+    /// [`Some(vec![])`] means that the purl is empty and package is not pypi
+    /// one. [`Some([`PackageUrl`])`] means that it is a pypi package.
+    #[serde(default, skip_serializing_if = "Option::is_none")]
+    pub purls: Option<BTreeSet<PackageUrl>>,
 
     /// Optionally a SHA256 hash of the package archive
     #[serde_as(as = "Option<SerializableHash::<rattler_digest::Sha256>>")]
     pub sha256: Option<Sha256Hash>,
 
     /// Optionally the size of the package archive in bytes
     pub size: Option<u64>,
@@ -145,16 +158,17 @@
     #[serde(default)]
     pub subdir: String,
 
     /// The date this entry was created.
     #[serde_as(as = "Option<crate::utils::serde::Timestamp>")]
     pub timestamp: Option<chrono::DateTime<chrono::Utc>>,
 
-    /// Track features are nowadays only used to downweight packages (ie. give them less priority). To
-    /// that effect, the number of track features is counted (number of commas) and the package is downweighted
+    /// Track features are nowadays only used to downweight packages (ie. give
+    /// them less priority). To that effect, the number of track features is
+    /// counted (number of commas) and the package is downweighted
     /// by the number of track_features.
     #[serde(default, skip_serializing_if = "Vec::is_empty")]
     #[serde_as(as = "OneOrMany<_>")]
     pub track_features: Vec<String>,
 
     /// The version of the package
     pub version: VersionWithSource,
@@ -189,16 +203,16 @@
     }
 
     /// Returns the `base_url` specified in the repodata.
     pub fn base_url(&self) -> Option<&str> {
         self.info.as_ref().and_then(|i| i.base_url.as_deref())
     }
 
-    /// Builds a [`Vec<RepoDataRecord>`] from the packages in a [`RepoData`] given the source of the
-    /// data.
+    /// Builds a [`Vec<RepoDataRecord>`] from the packages in a [`RepoData`]
+    /// given the source of the data.
     pub fn into_repo_data_records(self, channel: &Channel) -> Vec<RepoDataRecord> {
         let mut records = Vec::with_capacity(self.packages.len() + self.conda_packages.len());
         let channel_name = channel.canonical_name();
         let base_url = self.base_url().map(ToOwned::to_owned);
 
         // Determine the base_url of the channel
         for (filename, package_record) in self.packages.into_iter().chain(self.conda_packages) {
@@ -261,15 +275,16 @@
         let mut url = url.clone();
         url.set_path(&format!("{path}/"));
         Cow::Owned(url)
     }
 }
 
 impl PackageRecord {
-    /// A simple helper method that constructs a `PackageRecord` with the bare minimum values.
+    /// A simple helper method that constructs a `PackageRecord` with the bare
+    /// minimum values.
     pub fn new(name: PackageName, version: impl Into<VersionWithSource>, build: String) -> Self {
         Self {
             arch: None,
             build,
             build_number: 0,
             constrains: vec![],
             depends: vec![],
@@ -284,22 +299,23 @@
             platform: None,
             sha256: None,
             size: None,
             subdir: Platform::current().to_string(),
             timestamp: None,
             track_features: vec![],
             version: version.into(),
-            purls: vec![],
+            purls: None,
         }
     }
 
     /// Sorts the records topologically.
     ///
-    /// This function is deterministic, meaning that it will return the same result regardless of
-    /// the order of `records` and of the `depends` vector inside the records.
+    /// This function is deterministic, meaning that it will return the same
+    /// result regardless of the order of `records` and of the `depends`
+    /// vector inside the records.
     ///
     /// Note that this function only works for packages with unique names.
     pub fn sort_topologically<T: AsRef<PackageRecord> + Clone>(records: Vec<T>) -> Vec<T> {
         topological_sort::sort_topologically(records)
     }
 }
 
@@ -326,16 +342,16 @@
 /// database
 /// These were the combinations that have been found in the database.
 /// and have been represented in the function.
 ///
 /// # Why can we not use `Platform::FromStr`?
 ///
 /// We cannot use the [`Platform`] `FromStr` directly because `x86` and `x86_64`
-/// are different architecture strings. Also some combinations have been removed,
-/// because they have not been found.
+/// are different architecture strings. Also some combinations have been
+/// removed, because they have not been found.
 fn determine_subdir(
     platform: Option<String>,
     arch: Option<String>,
 ) -> Result<String, ConvertSubdirError> {
     let platform = platform.ok_or(ConvertSubdirError::PlatformEmpty)?;
     let arch = arch.ok_or(ConvertSubdirError::ArchEmpty)?;
 
@@ -365,15 +381,16 @@
         _ => Err(ConvertSubdirError::NoKnownCombination { platform, arch }),
     }?;
     // Convert back to Platform string which should correspond to known subdirs
     Ok(plat.to_string())
 }
 
 impl PackageRecord {
-    /// Builds a [`PackageRecord`] from a [`IndexJson`] and optionally a size, sha256 and md5 hash.
+    /// Builds a [`PackageRecord`] from a [`IndexJson`] and optionally a size,
+    /// sha256 and md5 hash.
     pub fn from_index_json(
         index: IndexJson,
         size: Option<u64>,
         sha256: Option<Sha256Hash>,
         md5: Option<Md5Hash>,
     ) -> Result<PackageRecord, ConvertSubdirError> {
         // Determine the subdir if it can't be found
@@ -399,15 +416,15 @@
             platform: index.platform,
             sha256,
             size,
             subdir,
             timestamp: index.timestamp,
             track_features: index.track_features,
             version: index.version,
-            purls: vec![],
+            purls: None,
         })
     }
 }
 
 fn sort_map_alphabetically<T: Serialize, S: serde::Serializer>(
     value: &FxHashMap<String, T>,
     serializer: S,
@@ -423,18 +440,20 @@
     serializer: S,
 ) -> Result<S::Ok, S::Error> {
     value.iter().collect::<BTreeSet<_>>().serialize(serializer)
 }
 
 #[cfg(test)]
 mod test {
-    use crate::repo_data::{compute_package_url, determine_subdir};
     use fxhash::FxHashMap;
 
-    use crate::{Channel, ChannelConfig, RepoData};
+    use crate::{
+        repo_data::{compute_package_url, determine_subdir},
+        Channel, ChannelConfig, RepoData,
+    };
 
     // isl-0.12.2-1.tar.bz2
     // gmp-5.1.2-6.tar.bz2
     // Are both package variants in the osx-64 subdir
     // Will just test for this case
     #[test]
     fn test_determine_subdir() {
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/patches.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #![allow(clippy::option_option)]
 
 use fxhash::{FxHashMap, FxHashSet};
 use serde::{Deserialize, Serialize};
 use serde_with::{serde_as, skip_serializing_none, OneOrMany};
+use std::collections::BTreeSet;
 use std::io;
 use std::path::Path;
 
-use crate::{package::ArchiveType, PackageRecord, PackageUrl, RepoData};
+use crate::{package::ArchiveType, PackageRecord, PackageUrl, RepoData, Shard};
 
 /// Represents a Conda repodata patch.
 ///
 /// This struct contains information about a patch to a Conda repodata file,
 /// which is used to update the metadata for Conda packages. The patch contains
 /// information about changes to the repodata, such as removed (yanked) packages and updated package
 /// metadata.
@@ -93,15 +94,15 @@
         skip_serializing_if = "Option::is_none",
         with = "::serde_with::rust::double_option"
     )]
     pub license_family: Option<Option<String>>,
 
     /// Package identifiers of packages that are equivalent to this package but from other
     /// ecosystems.
-    pub purls: Option<Vec<PackageUrl>>,
+    pub purls: Option<BTreeSet<PackageUrl>>,
 }
 
 /// Repodata patch instructions for a single subdirectory. See [`RepoDataPatch`] for more
 /// information.
 #[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Clone)]
 pub struct PatchInstructions {
     /// Filenames that have been removed from the subdirectory
@@ -139,69 +140,95 @@
         if let Some(license) = &patch.license {
             self.license = license.clone();
         }
         if let Some(license_family) = &patch.license_family {
             self.license_family = license_family.clone();
         }
         if let Some(package_urls) = &patch.purls {
-            self.purls = package_urls.clone();
+            self.purls = Some(package_urls.clone());
         }
     }
 }
 
-impl RepoData {
-    /// Apply a patch to a repodata file
-    /// Note that we currently do not handle `revoked` instructions
-    pub fn apply_patches(&mut self, instructions: &PatchInstructions) {
-        for (pkg, patch) in instructions.packages.iter() {
-            if let Some(record) = self.packages.get_mut(pkg) {
+/// Apply a patch to a repodata file
+/// Note that we currently do not handle `revoked` instructions
+pub fn apply_patches_impl(
+    packages: &mut FxHashMap<String, PackageRecord>,
+    conda_packages: &mut FxHashMap<String, PackageRecord>,
+    removed: &mut FxHashSet<String>,
+    instructions: &PatchInstructions,
+) {
+    for (pkg, patch) in instructions.packages.iter() {
+        if let Some(record) = packages.get_mut(pkg) {
+            record.apply_patch(patch);
+        }
+
+        // also apply the patch to the conda packages
+        if let Some((pkg_name, archive_type)) = ArchiveType::split_str(pkg) {
+            assert!(archive_type == ArchiveType::TarBz2);
+            if let Some(record) = conda_packages.get_mut(&format!("{pkg_name}.conda")) {
                 record.apply_patch(patch);
             }
-
-            // also apply the patch to the conda packages
-            if let Some((pkg_name, archive_type)) = ArchiveType::split_str(pkg) {
-                assert!(archive_type == ArchiveType::TarBz2);
-                if let Some(record) = self.conda_packages.get_mut(&format!("{pkg_name}.conda")) {
-                    record.apply_patch(patch);
-                }
-            }
         }
+    }
 
-        for (pkg, patch) in instructions.conda_packages.iter() {
-            if let Some(record) = self.conda_packages.get_mut(pkg) {
-                record.apply_patch(patch);
-            }
+    for (pkg, patch) in instructions.conda_packages.iter() {
+        if let Some(record) = conda_packages.get_mut(pkg) {
+            record.apply_patch(patch);
         }
+    }
 
-        let mut removed = FxHashSet::<String>::default();
-        // remove packages that have been removed
-        for pkg in instructions.remove.iter() {
-            if let Some((pkg_name, archive_type)) = ArchiveType::split_str(pkg) {
-                match archive_type {
-                    ArchiveType::TarBz2 => {
-                        if self.packages.remove_entry(pkg).is_some() {
-                            removed.insert(pkg.clone());
-                        }
-
-                        // also remove equivalent .conda package if it exists
-                        let conda_pkg_name = format!("{pkg_name}.conda");
-                        if self.conda_packages.remove_entry(&conda_pkg_name).is_some() {
-                            removed.insert(conda_pkg_name);
-                        }
+    // remove packages that have been removed
+    for pkg in instructions.remove.iter() {
+        if let Some((pkg_name, archive_type)) = ArchiveType::split_str(pkg) {
+            match archive_type {
+                ArchiveType::TarBz2 => {
+                    if packages.remove_entry(pkg).is_some() {
+                        removed.insert(pkg.clone());
                     }
-                    ArchiveType::Conda => {
-                        if self.conda_packages.remove_entry(pkg).is_some() {
-                            removed.insert(pkg.clone());
-                        }
+
+                    // also remove equivalent .conda package if it exists
+                    let conda_pkg_name = format!("{pkg_name}.conda");
+                    if conda_packages.remove_entry(&conda_pkg_name).is_some() {
+                        removed.insert(conda_pkg_name);
+                    }
+                }
+                ArchiveType::Conda => {
+                    if conda_packages.remove_entry(pkg).is_some() {
+                        removed.insert(pkg.clone());
                     }
                 }
             }
         }
+    }
+}
+
+impl RepoData {
+    /// Apply a patch to a repodata file
+    /// Note that we currently do not handle `revoked` instructions
+    pub fn apply_patches(&mut self, instructions: &PatchInstructions) {
+        apply_patches_impl(
+            &mut self.packages,
+            &mut self.conda_packages,
+            &mut self.removed,
+            instructions,
+        );
+    }
+}
 
-        self.removed.extend(removed);
+impl Shard {
+    /// Apply a patch to a shard
+    /// Note that we currently do not handle `revoked` instructions
+    pub fn apply_patches(&mut self, instructions: &PatchInstructions) {
+        apply_patches_impl(
+            &mut self.packages,
+            &mut self.conda_packages,
+            &mut self.removed,
+            instructions,
+        );
     }
 }
 
 #[cfg(test)]
 mod test {
     use crate::{PatchInstructions, RepoData};
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patch_purl.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__patching.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_1.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__patches__test__removing_2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__base_url_packages.snap`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ---
 source: crates/rattler_conda_types/src/repo_data/mod.rs
+assertion_line: 511
 expression: file_urls
 ---
-- "channels/dummy/linux-64/baz-2.0-unix_py36h1af98f8_2\u0000.tar.bz2"
-- "channels/dummy/linux-64/baz-1.0-unix_py36h1af98f8_2\u0000.tar.bz2"
+- channels/dummy/linux-64/foobar-2.1-bla_1.tar.bz2
 - channels/dummy/linux-64/bors-2.1-bla_1.tar.bz2
+- channels/dummy/linux-64/foo-3.0.2-py36h1af98f8_2.conda
 - channels/dummy/linux-64/bar-1.0-unix_py36h1af98f8_2.tar.bz2
 - channels/dummy/linux-64/bors-1.0-bla_1.tar.bz2
 - channels/dummy/linux-64/foo-3.0.2-py36h1af98f8_1.conda
 - channels/dummy/linux-64/foo-3.0.2-py36h1af98f8_1.tar.bz2
-- channels/dummy/linux-64/bors-1.1-bla_1.tar.bz2
+- channels/dummy/linux-64/baz-2.0-unix_py36h1af98f8_2.tar.bz2
 - channels/dummy/linux-64/foo-4.0.2-py36h1af98f8_2.tar.bz2
+- channels/dummy/linux-64/bors-1.1-bla_1.tar.bz2
 - channels/dummy/linux-64/bors-2.0-bla_1.tar.bz2
 - channels/dummy/linux-64/foobar-2.0-bla_1.tar.bz2
-- channels/dummy/linux-64/foobar-2.1-bla_1.tar.bz2
 - channels/dummy/linux-64/bors-1.2.1-bla_1.tar.bz2
-
+- channels/dummy/linux-64/baz-1.0-unix_py36h1af98f8_2.tar.bz2
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__deserialize_no_packages_conda.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages-2.snap`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ---
 source: crates/rattler_conda_types/src/repo_data/mod.rs
-assertion_line: 460
+assertion_line: 470
 expression: json
 ---
 {
   "info": {
     "subdir": "linux-64",
     "base_url": "../linux-64"
   },
@@ -21,42 +21,42 @@
       "name": "bar",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
       "timestamp": 1605110689658,
       "version": "1.2.3"
     },
-    "baz-1.0-unix_py36h1af98f8_2\u0000.tar.bz2": {
-      "build": "unix_py36h1af98f8_2\u0000",
+    "baz-1.0-unix_py36h1af98f8_2.tar.bz2": {
+      "build": "unix_py36h1af98f8_2",
       "build_number": 1,
       "depends": [
         "__unix"
       ],
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "baz",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
       "timestamp": 1605110689658,
       "version": "1.2.3"
     },
-    "baz-2.0-unix_py36h1af98f8_2\u0000.tar.bz2": {
-      "build": "unix_py36h1af98f8_2\u0000",
+    "baz-2.0-unix_py36h1af98f8_2.tar.bz2": {
+      "build": "unix_py36h1af98f8_2",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "baz",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "2.0"
     },
     "bors-1.0-bla_1.tar.bz2": {
       "build": "bla_1",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
@@ -104,43 +104,43 @@
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "bors",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "2.0"
     },
     "bors-2.1-bla_1.tar.bz2": {
       "build": "bla_1",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "bors",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "2.1"
     },
     "foo-3.0.2-py36h1af98f8_1.conda": {
       "build": "py36h1af98f8_1",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
       "license_family": "MIT",
       "md5": "fb731d9290f0bcbf3a054665f33ec94f",
       "name": "foo",
       "sha256": "67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "3.0.2"
     },
     "foo-3.0.2-py36h1af98f8_1.tar.bz2": {
       "build": "py36h1af98f8_1",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
@@ -149,26 +149,40 @@
       "name": "foo",
       "sha256": "1154fceeb5c4ee9bb97d245713ac21eb1910237c724d2b7103747215663273c2",
       "size": 414494,
       "subdir": "linux-64",
       "timestamp": 1605110689658,
       "version": "3.0.2"
     },
+    "foo-3.0.2-py36h1af98f8_2.conda": {
+      "build": "py36h1af98f8_2",
+      "build_number": 2,
+      "depends": [],
+      "license": "MIT",
+      "license_family": "MIT",
+      "md5": "fb731d9290f0bcbf3a054665f33ec94f",
+      "name": "foo",
+      "sha256": "67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4",
+      "size": 414494,
+      "subdir": "linux-64",
+      "timestamp": 1715610974,
+      "version": "3.0.2"
+    },
     "foo-4.0.2-py36h1af98f8_2.tar.bz2": {
       "build": "py36h1af98f8_2",
       "build_number": 1,
       "depends": [],
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "foo",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "4.0.2"
     },
     "foobar-2.0-bla_1.tar.bz2": {
       "build": "bla_1",
       "build_number": 1,
       "depends": [
         "bors <2.0"
@@ -192,14 +206,14 @@
       "license": "MIT",
       "license_family": "MIT",
       "md5": "bc13aa58e2092bcb0b97c561373d3905",
       "name": "foobar",
       "sha256": "97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a",
       "size": 414494,
       "subdir": "linux-64",
-      "timestamp": 1605110689658,
+      "timestamp": 1715610974,
       "version": "2.1"
     }
   },
   "packages.conda": {},
   "repodata_version": 2
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/snapshots/rattler_conda_types__repo_data__test__serialize_packages.snap`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ---
 source: crates/rattler_conda_types/src/repo_data/mod.rs
+assertion_line: 466
 expression: repodata
 ---
 info:
   subdir: linux-64
   base_url: "../linux-64"
 packages:
   bar-1.0-unix_py36h1af98f8_2.tar.bz2:
@@ -16,40 +17,40 @@
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: bar
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
     timestamp: 1605110689658
     version: 1.2.3
-  "baz-1.0-unix_py36h1af98f8_2\u0000.tar.bz2":
-    build: "unix_py36h1af98f8_2\u0000"
+  baz-1.0-unix_py36h1af98f8_2.tar.bz2:
+    build: unix_py36h1af98f8_2
     build_number: 1
     depends:
       - __unix
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: baz
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
     timestamp: 1605110689658
     version: 1.2.3
-  "baz-2.0-unix_py36h1af98f8_2\u0000.tar.bz2":
-    build: "unix_py36h1af98f8_2\u0000"
+  baz-2.0-unix_py36h1af98f8_2.tar.bz2:
+    build: unix_py36h1af98f8_2
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: baz
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: "2.0"
   bors-1.0-bla_1.tar.bz2:
     build: bla_1
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
@@ -93,67 +94,80 @@
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: bors
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: "2.0"
   bors-2.1-bla_1.tar.bz2:
     build: bla_1
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: bors
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: "2.1"
   foo-3.0.2-py36h1af98f8_1.conda:
     build: py36h1af98f8_1
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
     md5: fb731d9290f0bcbf3a054665f33ec94f
     name: foo
     sha256: 67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: 3.0.2
   foo-3.0.2-py36h1af98f8_1.tar.bz2:
     build: py36h1af98f8_1
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
     md5: d65ab674acf3b7294ebacaec05fc5b54
     name: foo
     sha256: 1154fceeb5c4ee9bb97d245713ac21eb1910237c724d2b7103747215663273c2
     size: 414494
     subdir: linux-64
     timestamp: 1605110689658
     version: 3.0.2
+  foo-3.0.2-py36h1af98f8_2.conda:
+    build: py36h1af98f8_2
+    build_number: 2
+    depends: []
+    license: MIT
+    license_family: MIT
+    md5: fb731d9290f0bcbf3a054665f33ec94f
+    name: foo
+    sha256: 67a63bec3fd3205170eaad532d487595b8aaceb9814d13c6858d7bac3ef24cd4
+    size: 414494
+    subdir: linux-64
+    timestamp: 1715610974
+    version: 3.0.2
   foo-4.0.2-py36h1af98f8_2.tar.bz2:
     build: py36h1af98f8_2
     build_number: 1
     depends: []
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: foo
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: 4.0.2
   foobar-2.0-bla_1.tar.bz2:
     build: bla_1
     build_number: 1
     depends:
       - bors <2.0
     license: MIT
@@ -173,12 +187,11 @@
     license: MIT
     license_family: MIT
     md5: bc13aa58e2092bcb0b97c561373d3905
     name: foobar
     sha256: 97ec377d2ad83dfef1194b7aa31b0c9076194e10d995a6e696c9d07dd782b14a
     size: 414494
     subdir: linux-64
-    timestamp: 1605110689658
+    timestamp: 1715610974
     version: "2.1"
 packages.conda: {}
 repodata_version: 2
-
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data/topological_sort.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,28 @@
         .collect();
 
     // Detect cycles
     let mut visited = FxHashSet::default();
     let mut stack = Vec::new();
     let mut cycles = Vec::new();
 
-    for root in &roots {
-        if !visited.contains(root) {
-            if let Some(cycle) = find_cycles(root, &all_packages, &mut visited, &mut stack) {
+    // We must start from the roots, unless all packages are in a cycle, in which case we can start from any package
+    let starting_points_for_root_finding = if roots.is_empty() {
+        packages.first().map_or_else(Vec::new, |package| {
+            vec![package.as_ref().name.as_normalized().to_string()]
+        })
+    } else {
+        roots
+    };
+
+    for starting_point in &starting_points_for_root_finding {
+        if !visited.contains(starting_point) {
+            if let Some(cycle) =
+                find_cycles(starting_point, &all_packages, &mut visited, &mut stack)
+            {
                 cycles.push(cycle);
             }
         }
     }
 
     // print all cycles
     for cycle in &cycles {
@@ -335,14 +346,15 @@
         assert_eq!(roots.as_slice(), expected_roots);
     }
 
     #[rstest]
     #[case(get_resolved_packages_for_python(), "python", &[("libzlib", "libgcc-ng")])]
     #[case(get_resolved_packages_for_numpy(), "numpy", &[("llvm-openmp", "libzlib")])]
     #[case(get_resolved_packages_for_two_roots(), "4ti2", &[("libzlib", "libgcc-ng")])]
+    #[case(get_resolved_packages_for_rootless_graph(), "pip", &[("python", "pip")])]
     #[case(get_resolved_packages_for_python_pip(), "pip", &[("pip", "python"), ("libzlib", "libgcc-ng")])]
     fn test_topological_sort(
         #[case] packages: Vec<RepoDataRecord>,
         #[case] expected_last_package: &str,
         #[case] circular_deps: &[(&str, &str)],
     ) {
         let sorted_packages = sort_topologically(packages.clone());
@@ -1743,14 +1755,64 @@
               "channel": "https://conda.anaconda.org/conda-forge/"
             }
           ]"#;
 
         serde_json::from_str(repodata_json).unwrap()
     }
 
+    fn get_resolved_packages_for_rootless_graph() -> Vec<RepoDataRecord> {
+        // Pip depends on Python and Python depends on Pip since Python 3.12
+        // Below is a simplified version of their repodata.
+        let repodata_json = r#"[
+          {
+              "build": "pyhd8ed1ab_0",
+              "build_number": 0,
+              "depends": [
+                  "python >=3.7"
+              ],
+              "license": "MIT",
+              "license_family": "MIT",
+              "md5": "f586ac1e56c8638b64f9c8122a7b8a67",
+              "name": "pip",
+              "noarch": "python",
+              "sha256": "b7c1c5d8f13e8cb491c4bd1d0d1896a4cf80fc47de01059ad77509112b664a4a",
+              "size": 1398245,
+              "subdir": "noarch",
+              "timestamp": 1706960660581,
+              "version": "24.0",
+              "fn": "pip-24.0-pyhd8ed1ab_0.conda",
+              "url": "https://conda.anaconda.org/conda-forge/noarch/pip-24.0-pyhd8ed1ab_0.conda",
+              "channel": "https://conda.anaconda.org/conda-forge/"
+          },
+          {
+            "build": "h1411813_0_cpython",
+            "build_number": 0,
+            "constrains": [
+                "python_abi 3.12.* *_cp312"
+            ],
+            "depends": [
+                "pip"
+            ],
+            "license": "Python-2.0",
+            "md5": "df1448ec6cbf8eceb03d29003cf72ae6",
+            "name": "python",
+            "sha256": "3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a",
+            "size": 14557341,
+            "subdir": "osx-64",
+            "timestamp": 1713208068012,
+            "version": "3.12.3",
+            "fn": "python-3.12.3-h1411813_0_cpython.conda",
+            "url": "https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda",
+            "channel": "https://conda.anaconda.org/conda-forge/"
+        }
+      ]"#;
+
+        serde_json::from_str(repodata_json).unwrap()
+    }
+
     fn get_resolved_packages_for_python_pip() -> Vec<RepoDataRecord> {
         let pip = r#"
         [
           {
             "arch": null,
             "build": "pyhd8ed1ab_0",
             "build_number": 0,
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/repo_data_record.rs`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 use crate::PackageRecord;
 use serde::{Deserialize, Serialize};
 use url::Url;
 
 /// Information about a package from repodata. It includes a [`crate::PackageRecord`] but it also stores
 /// the source of the data (like the url and the channel).
-#[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Ord, PartialOrd, Clone, Hash)]
+#[derive(Debug, Deserialize, Serialize, Eq, PartialEq, Clone, Hash)]
 pub struct RepoDataRecord {
     /// The data stored in the repodata.json.
     #[serde(flatten)]
     pub package_record: PackageRecord,
 
     /// The filename of the package
     #[serde(rename = "fn")]
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__ros-noetic_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__explicit_environment_spec__test__explicit-envs__xtensor_linux-64.txt.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__libsqlite-3_40_0-hcfcfb64_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__menuinst-1_4_19-py311h1ea47a8_1_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pip-23_0-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__pysocks-1_7_1-pyh0701188_6_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__requests-2_28_2-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__tk-8_6_12-h8ffe710_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__urllib3-1_26_14-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__vc-14_3-hb6edc58_10_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__wheel-0_38_4-pyhd8ed1ab_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/snapshots/rattler_conda_types__prefix_record__test__xz-5_2_6-h8d14728_0_json.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/utils/serde.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/utils/serde.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/bump.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/bump.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/flags.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/flags.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -947,15 +947,14 @@
 
 impl<'de> Deserialize<'de> for Version {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
     where
         D: Deserializer<'de>,
     {
         Cow::<'de, str>::deserialize(deserializer)?
-            .as_ref()
             .parse()
             .map_err(D::Error::custom)
     }
 }
 
 pub struct SegmentIter<'v> {
     /// Information about the segment we are iterating.
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/parse.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/segment.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/segment.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/snapshots/rattler_conda_types__version__parse__test__parse.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version/with_source.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version/with_source.rs`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 }
 
 impl Ord for VersionWithSource {
     fn cmp(&self, other: &Self) -> Ordering {
         // First order by version then by string representation
         self.version
             .cmp(&other.version)
-            .then_with(|| self.as_str().as_ref().cmp(other.as_str().as_ref()))
+            .then_with(|| self.as_str().cmp(&other.as_str()))
     }
 }
 
 impl VersionWithSource {
     /// Constructs a new instance from a [`Version`] and a source representation.
     pub fn new(version: Version, source: impl ToString) -> Self {
         Self {
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/constraint.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/parse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs` & `py_rattler-0.6.0/local_dependencies/rattler_conda_types/src/version_spec/version_tree.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/CHANGELOG.md` & `py_rattler-0.6.0/local_dependencies/rattler/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,47 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.26.0](https://github.com/mamba-org/rattler/compare/rattler-v0.25.0...rattler-v0.26.0) - 2024-05-27
+
+### Fixed
+- improve progress bar duration display ([#680](https://github.com/mamba-org/rattler/pull/680))
+
+### Other
+- introducing the installer ([#664](https://github.com/mamba-org/rattler/pull/664))
+- create directories up front ([#533](https://github.com/mamba-org/rattler/pull/533))
+
+## [0.25.0](https://github.com/mamba-org/rattler/compare/rattler-v0.24.1...rattler-v0.25.0) - 2024-05-14
+
+### Added
+- exclude repodata records based on timestamp ([#654](https://github.com/mamba-org/rattler/pull/654))
+
+### Other
+- use semaphore for install driver ([#653](https://github.com/mamba-org/rattler/pull/653))
+
+## [0.24.1](https://github.com/mamba-org/rattler/compare/rattler-v0.24.0...rattler-v0.24.1) - 2024-05-13
+
+### Other
+- updated the following local packages: rattler_conda_types, rattler_digest, rattler_package_streaming, rattler_networking
+
+## [0.24.0](https://github.com/mamba-org/rattler/compare/rattler-v0.23.2...rattler-v0.24.0) - 2024-05-06
+
+### Fixed
+- use the output of `readlink` as hash for softlinks ([#643](https://github.com/mamba-org/rattler/pull/643))
+- sha computation of symlinks was failing sometimes ([#641](https://github.com/mamba-org/rattler/pull/641))
+
+## [0.23.2](https://github.com/mamba-org/rattler/compare/rattler-v0.23.1...rattler-v0.23.2) - 2024-04-30
+
+### Other
+- updated the following local packages: rattler_networking
+
 ## [0.23.1](https://github.com/mamba-org/rattler/compare/rattler-v0.23.0...rattler-v0.23.1) - 2024-04-25
 
 ### Other
 - updated the following local packages: rattler_networking
 
 ## [0.23.0](https://github.com/mamba-org/rattler/compare/rattler-v0.22.0...rattler-v0.23.0) - 2024-04-25
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/resources/launcher64.exe` & `py_rattler-0.6.0/local_dependencies/rattler/resources/launcher64.exe`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/resources/versions.txt` & `py_rattler-0.6.0/local_dependencies/rattler/resources/versions.txt`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/cli/auth.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/cli/auth.rs`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 /// Login to prefix.dev or anaconda.org servers to access private channels
 #[derive(Parser, Debug)]
 pub struct Args {
     #[clap(subcommand)]
     subcommand: Subcommand,
 }
 
-/// Authentication errors that can be returned by the AuthenticationCLIError
+/// Authentication errors that can be returned by the `AuthenticationCLIError`
 #[derive(thiserror::Error, Debug)]
 pub enum AuthenticationCLIError {
     /// An error occured when the input repository URL is parsed
     #[error("Failed to parse the URL")]
     ParseUrlError(#[from] url::ParseError),
 
     /// Basic authentication needs a username and a password. The password is
@@ -83,25 +83,25 @@
         url::Url::parse(url)?.host_str().unwrap().to_string()
     } else {
         url.to_string()
     };
 
     let host = if host.matches('.').count() == 1 {
         // use wildcard for top-level domains
-        format!("*.{}", host)
+        format!("*.{host}")
     } else {
         host
     };
 
     Ok(host)
 }
 
 fn login(args: LoginArgs, storage: AuthenticationStorage) -> Result<(), AuthenticationCLIError> {
     let host = get_url(&args.host)?;
-    println!("Authenticating with {}", host);
+    println!("Authenticating with {host}");
 
     let auth = if let Some(conda_token) = args.conda_token {
         Authentication::CondaToken(conda_token)
     } else if let Some(username) = args.username {
         if args.password.is_none() {
             return Err(AuthenticationCLIError::MissingPassword);
         } else {
@@ -127,15 +127,15 @@
         .map_err(AuthenticationCLIError::StorageError)?;
     Ok(())
 }
 
 fn logout(args: LogoutArgs, storage: AuthenticationStorage) -> Result<(), AuthenticationCLIError> {
     let host = get_url(&args.host)?;
 
-    println!("Removing authentication for {}", host);
+    println!("Removing authentication for {host}");
 
     storage
         .delete(&host)
         .map_err(AuthenticationCLIError::StorageError)?;
     Ok(())
 }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/apple_codesign.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/apple_codesign.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/clobber_registry.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/clobber_registry.rs`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 fn clobber_template(package_name: &PackageName) -> String {
     format!("{CLOBBER_TEMPLATE}{}", package_name.as_normalized())
 }
 
 impl ClobberRegistry {
     /// Create a new clobber registry that is initialized with the given prefix records.
-    pub fn from_prefix_records(prefix_records: &[PrefixRecord]) -> Self {
+    pub fn from_prefix_records<'i>(
+        prefix_records: impl IntoIterator<Item = &'i PrefixRecord>,
+    ) -> Self {
         let mut registry = Self::default();
 
         let mut temp_clobbers = Vec::new();
         for prefix_record in prefix_records {
             let package_name = prefix_record.repodata_record.package_record.name.clone();
             registry.package_names.push(package_name.clone());
 
@@ -420,15 +422,18 @@
                 prefix_record_clobber_1.clone(),
             )],
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
-        let install_driver = InstallDriver::new(100, Some(&prefix_records), true);
+        let install_driver = InstallDriver::builder()
+            .with_prefix_records(&prefix_records)
+            .execute_link_scripts(true)
+            .finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
             &install_driver,
@@ -622,15 +627,17 @@
                     prefix_record_clobber_2.clone(),
                 )],
                 python_info: None,
                 current_python_info: None,
                 platform: Platform::current(),
             };
 
-            let install_driver = InstallDriver::new(100, Some(&prefix_records), false);
+            let install_driver = InstallDriver::builder()
+                .with_prefix_records(&prefix_records)
+                .finish();
 
             execute_transaction(
                 transaction,
                 target_prefix.path(),
                 &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
                 &cache,
                 &install_driver,
@@ -719,15 +726,17 @@
                 new: update_ops[0].clone(),
             }],
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
-        let install_driver = InstallDriver::new(100, Some(&prefix_records), false);
+        let install_driver = InstallDriver::builder()
+            .with_prefix_records(&prefix_records)
+            .finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
             &install_driver,
@@ -817,15 +826,17 @@
             ],
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
         let prefix_records = PrefixRecord::collect_from_prefix(target_prefix.path()).unwrap();
-        let install_driver = InstallDriver::new(100, Some(&prefix_records), false);
+        let install_driver = InstallDriver::builder()
+            .with_prefix_records(&prefix_records)
+            .finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
             &install_driver,
@@ -848,15 +859,17 @@
             operations: vec![TransactionOperation::Install(update_ops[0].clone())],
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
         let prefix_records = PrefixRecord::collect_from_prefix(target_prefix.path()).unwrap();
-        let install_driver = InstallDriver::new(100, Some(&prefix_records), false);
+        let install_driver = InstallDriver::builder()
+            .with_prefix_records(&prefix_records)
+            .finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
             &install_driver,
@@ -963,15 +976,17 @@
                 .map(|r| TransactionOperation::Remove(r.clone()))
                 .collect(),
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
-        let install_driver = InstallDriver::new(100, Some(&prefix_records), false);
+        let install_driver = InstallDriver::builder()
+            .with_prefix_records(&prefix_records)
+            .finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
             &install_driver,
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/entry_point.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/entry_point.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/link.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/link.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 //! This module contains the logic to link a give file from the package cache into the target directory.
 //! See [`link_file`] for more information.
 use memmap2::Mmap;
 use once_cell::sync::Lazy;
 use rattler_conda_types::package::{FileMode, PathType, PathsEntry, PrefixPlaceholder};
 use rattler_conda_types::Platform;
-use rattler_digest::HashingWriter;
 use rattler_digest::Sha256;
+use rattler_digest::{HashingWriter, Sha256Hash};
 use reflink_copy::reflink;
 use regex::Regex;
 use std::borrow::Cow;
 use std::fmt;
 use std::fmt::Formatter;
 use std::fs::Permissions;
 use std::io::{ErrorKind, Read, Seek, Write};
@@ -58,18 +58,14 @@
 /// Errors that can occur when calling [`link_file`].
 #[derive(Debug, thiserror::Error)]
 pub enum LinkFileError {
     /// An IO error occurred.
     #[error("unexpected io operation while {0}")]
     IoError(String, #[source] std::io::Error),
 
-    /// The parent directory of the destination file could not be created.
-    #[error("failed to create parent directory")]
-    FailedToCreateParentDirectory(#[source] std::io::Error),
-
     /// The source file could not be opened.
     #[error("could not open source file for reading")]
     FailedToOpenSourceFile(#[source] std::io::Error),
 
     /// The source file could not be opened.
     #[error("failed to read the source file")]
     FailedToReadSourceFile(#[source] std::io::Error),
@@ -98,14 +94,18 @@
     /// macOS ARM64 (Apple Silicon).
     #[error("failed to sign Apple binary")]
     FailedToSignAppleBinary,
 
     /// No Python version was specified when installing a noarch package.
     #[error("cannot install noarch python files because there is no python version specified ")]
     MissingPythonInfo,
+
+    /// The hash of the file could not be computed.
+    #[error("failed to compute the sha256 hash of the file")]
+    FailedToComputeSha(#[source] std::io::Error),
 }
 
 /// The successful result of calling [`link_file`].
 pub struct LinkedFile {
     /// True if an existing file already existed and linking overwrote the original file.
     pub clobbered: bool,
 
@@ -146,19 +146,14 @@
     target_platform: Platform,
     apple_codesign_behavior: AppleCodeSignBehavior,
 ) -> Result<LinkedFile, LinkFileError> {
     let source_path = package_dir.join(&path_json_entry.relative_path);
 
     let destination_path = target_dir.join(&destination_relative_path);
 
-    // Ensure that all directories up to the path exist.
-    if let Some(parent) = destination_path.parent() {
-        std::fs::create_dir_all(parent).map_err(LinkFileError::FailedToCreateParentDirectory)?;
-    }
-
     // Temporary variables to store intermediate computations in. If we already computed the file
     // size or the sha hash we dont have to recompute them at the end of the function.
     let mut sha256 = None;
     let mut file_size = path_json_entry.size_in_bytes;
 
     let link_method = if let Some(PrefixPlaceholder {
         file_mode,
@@ -242,17 +237,24 @@
                         if apple_codesign_behavior == AppleCodeSignBehavior::Fail {
                             return Err(e);
                         }
                     }
                 }
 
                 // The file on disk changed from the original file so the hash and file size
-                // also became invalid.
-                sha256 = None;
-                file_size = None;
+                // also became invalid. Let's recompute them.
+                sha256 = Some(
+                    rattler_digest::compute_file_digest::<Sha256>(&destination_path)
+                        .map_err(LinkFileError::FailedToComputeSha)?,
+                );
+                file_size = Some(
+                    std::fs::symlink_metadata(&destination_path)
+                        .map_err(LinkFileError::FailedToOpenDestinationFile)?
+                        .len(),
+                );
             }
         }
         LinkMethod::Patched(*file_mode)
     } else if path_json_entry.path_type == PathType::HardLink && allow_ref_links {
         reflink_to_destination(&source_path, &destination_path, allow_hard_links)?
     } else if path_json_entry.path_type == PathType::HardLink && allow_hard_links {
         hardlink_to_destination(&source_path, &destination_path)?
@@ -261,19 +263,36 @@
     } else {
         copy_to_destination(&source_path, &destination_path)?
     };
 
     // Compute the final SHA256 if we didnt already or if its not stored in the paths.json entry.
     let sha256 = if let Some(sha256) = sha256 {
         sha256
+    } else if link_method == LinkMethod::Softlink {
+        // we hash the content of the symlink file. Note that this behavior is different from
+        // conda or mamba (where the target of the symlink is hashed). However, hashing the target
+        // of the symlink is more tricky in our case as we link everything in parallel and would have to
+        // potentially "wait" for dependencies to be available.
+        // This needs to be taken into account when verifying an installation.
+        let linked_path = destination_path
+            .read_link()
+            .map_err(LinkFileError::FailedToReadSymlink)?;
+        rattler_digest::compute_bytes_digest::<Sha256>(
+            linked_path.as_os_str().to_string_lossy().as_bytes(),
+        )
     } else if let Some(sha256) = path_json_entry.sha256 {
         sha256
-    } else {
+    } else if path_json_entry.path_type == PathType::HardLink {
         rattler_digest::compute_file_digest::<Sha256>(&destination_path)
-            .map_err(LinkFileError::FailedToOpenDestinationFile)?
+            .map_err(LinkFileError::FailedToComputeSha)?
+    } else {
+        // This is either a softlink or a directory.
+        // Computing the hash for a directory is not possible.
+        // This hash is `0000...0000`
+        Sha256Hash::default()
     };
 
     // Compute the final file size if we didnt already.
     let file_size = if let Some(file_size) = file_size {
         file_size
     } else if let Some(size_in_bytes) = path_json_entry.size_in_bytes {
         size_in_bytes
@@ -366,25 +385,25 @@
             }
             Err(e) if e.kind() == ErrorKind::AlreadyExists => {
                 std::fs::remove_file(destination_path).map_err(|err| {
                     LinkFileError::IoError(String::from("removing clobbered file"), err)
                 })?;
             }
             Err(e) if e.kind() == ErrorKind::Unsupported && allow_hard_links => {
-                return hardlink_to_destination(source_path, destination_path)
+                return hardlink_to_destination(source_path, destination_path);
             }
             Err(e) if e.kind() == ErrorKind::Unsupported && !allow_hard_links => {
-                return copy_to_destination(source_path, destination_path)
+                return copy_to_destination(source_path, destination_path);
             }
             Err(_) => {
                 return if allow_hard_links {
                     hardlink_to_destination(source_path, destination_path)
                 } else {
                     copy_to_destination(source_path, destination_path)
-                }
+                };
             }
         }
     }
 }
 
 /// Hard link the specified file from the source (or cached) directory. If the file already exists
 /// it is removed and the operation is retried.
@@ -416,15 +435,14 @@
 fn symlink_to_destination(
     source_path: &Path,
     destination_path: &Path,
 ) -> Result<LinkMethod, LinkFileError> {
     let linked_path = source_path
         .read_link()
         .map_err(LinkFileError::FailedToReadSymlink)?;
-
     loop {
         match symlink(&linked_path, destination_path) {
             Ok(_) => return Ok(LinkMethod::Softlink),
             Err(e) if e.kind() == ErrorKind::AlreadyExists => {
                 std::fs::remove_file(destination_path).map_err(|err| {
                     LinkFileError::IoError(String::from("removing clobbered file"), err)
                 })?;
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/link_script.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/link_script.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 //! Functions for running link scripts (pre-unlink and post-link) for a package
+use std::borrow::Borrow;
 use std::{
     collections::{HashMap, HashSet},
     path::Path,
 };
+use thiserror::Error;
 
-use rattler_conda_types::{PackageName, PackageRecord, Platform, PrefixRecord, RepoDataRecord};
+use rattler_conda_types::{PackageName, PackageRecord, Platform, PrefixRecord};
 use rattler_shell::shell::{Bash, CmdExe, ShellEnum};
 
 use super::{InstallDriver, Transaction};
 
 /// Error type for link script errors
 #[derive(Debug, thiserror::Error)]
 pub enum LinkScriptError {
@@ -59,21 +61,30 @@
             LinkScriptType::PreUnlink => "pre-unlink".to_string(),
             LinkScriptType::PostLink => "post-link".to_string(),
         }
     }
 }
 
 /// Records the results of running pre/post link scripts
+#[derive(Debug, Clone)]
 pub struct PrePostLinkResult {
     /// Messages from the link scripts
     pub messages: HashMap<PackageName, String>,
     /// Packages that failed to run the link scripts
     pub failed_packages: Vec<PackageName>,
 }
 
+/// An error that can occur during pre-, post-link script execution.
+#[derive(Debug, Error)]
+pub enum PrePostLinkError {
+    /// Failed to determine the currently installed packages.
+    #[error("failed to determine the installed packages")]
+    FailedToDetectInstalledPackages(#[source] std::io::Error),
+}
+
 /// Run the link scripts for a given package
 pub fn run_link_scripts<'a>(
     link_script_type: LinkScriptType,
     prefix_records: impl Iterator<Item = &'a PrefixRecord>,
     target_prefix: &Path,
     platform: &Platform,
 ) -> Result<PrePostLinkResult, LinkScriptError> {
@@ -147,23 +158,27 @@
         messages,
         failed_packages,
     })
 }
 
 impl InstallDriver {
     /// Run any post-link scripts that are part of the packages that are being installed.
-    pub fn run_post_link_scripts(
+    pub fn run_post_link_scripts<Old, New>(
         &self,
-        transaction: &Transaction<PrefixRecord, RepoDataRecord>,
+        transaction: &Transaction<Old, New>,
         prefix_records: &[&PrefixRecord],
         target_prefix: &Path,
-    ) -> Result<PrePostLinkResult, LinkScriptError> {
+    ) -> Result<PrePostLinkResult, LinkScriptError>
+    where
+        Old: AsRef<New>,
+        New: AsRef<PackageRecord>,
+    {
         let to_install = transaction
             .installed_packages()
-            .map(|r| &r.package_record.name)
+            .map(|r| &r.as_ref().name)
             .collect::<HashSet<_>>();
 
         let filter_iter = prefix_records
             .iter()
             .filter(|r| to_install.contains(&r.repodata_record.package_record.name))
             .cloned();
 
@@ -172,22 +187,25 @@
             filter_iter,
             target_prefix,
             &transaction.platform,
         )
     }
 
     /// Run any post-link scripts that are part of the packages that are being installed.
-    pub fn run_pre_unlink_scripts(
+    pub fn run_pre_unlink_scripts<Old, New>(
         &self,
-        transaction: &Transaction<PrefixRecord, RepoDataRecord>,
+        transaction: &Transaction<Old, New>,
         target_prefix: &Path,
-    ) -> Result<PrePostLinkResult, LinkScriptError> {
+    ) -> Result<PrePostLinkResult, LinkScriptError>
+    where
+        Old: Borrow<PrefixRecord>,
+    {
         run_link_scripts(
             LinkScriptType::PreUnlink,
-            transaction.removed_packages(),
+            transaction.removed_packages().map(Borrow::borrow),
             target_prefix,
             &transaction.platform,
         )
     }
 }
 
 #[cfg(test)]
@@ -221,21 +239,22 @@
             python_info: None,
             current_python_info: None,
             platform: Platform::current(),
         };
 
         let packages_dir = tempfile::tempdir().unwrap();
         let cache = PackageCache::new(packages_dir.path());
+        let driver = InstallDriver::builder().execute_link_scripts(true).finish();
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
-            &InstallDriver::default(),
+            &driver,
             &InstallOptions::default(),
         )
         .await;
 
         // check that the post-link script was run
         assert!(target_prefix.path().join("i-was-post-linked").exists());
 
@@ -249,15 +268,15 @@
         };
 
         execute_transaction(
             transaction,
             target_prefix.path(),
             &reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new()),
             &cache,
-            &InstallDriver::default(),
+            &driver,
             &InstallOptions::default(),
         )
         .await;
 
         // check that the pre-unlink script was run
         assert!(!target_prefix.path().join("i-was-post-linked").exists());
     }
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/mod.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,75 @@
-//! This module contains the logic to install a package into a prefix. The main entry point is the
-//! [`link_package`] function.
+//! This module contains the logic to install a package into a prefix. The main
+//! entry point is the [`link_package`] function.
 //!
-//! The [`link_package`] function takes a package directory and a target directory. The package
-//! directory is the directory that contains the extracted package archive. The target directory is
-//! the directory into which the package should be installed. The target directory is also called
+//! The [`link_package`] function takes a package directory and a target
+//! directory. The package directory is the directory that contains the
+//! extracted package archive. The target directory is the directory into which
+//! the package should be installed. The target directory is also called
 //! the "prefix".
 //!
-//! The [`link_package`] function will read the `paths.json` file from the package directory and
-//! link all files specified in that file into the target directory. The `paths.json` file contains
-//! a list of files that should be installed and how they should be installed. For example, the
-//! `paths.json` file might contain a file that should be copied into the target directory. Or it
-//! might contain a file that should be linked into the target directory. The `paths.json` file
-//! also contains a SHA256 hash for each file. This hash is used to verify that the file was not
-//! tampered with.
+//! The [`link_package`] function will read the `paths.json` file from the
+//! package directory and link all files specified in that file into the target
+//! directory. The `paths.json` file contains a list of files that should be
+//! installed and how they should be installed. For example, the `paths.json`
+//! file might contain a file that should be copied into the target directory.
+//! Or it might contain a file that should be linked into the target directory.
+//! The `paths.json` file also contains a SHA256 hash for each file. This hash
+//! is used to verify that the file was not tampered with.
 pub mod apple_codesign;
 mod clobber_registry;
 mod driver;
 mod entry_point;
 pub mod link;
 pub mod link_script;
 mod python;
 mod transaction;
 pub mod unlink;
 
+mod installer;
 #[cfg(test)]
 mod test_utils;
 
-pub use crate::install::entry_point::{get_windows_launcher, python_entry_point_template};
+use std::{
+    cmp::Ordering,
+    collections::{binary_heap::PeekMut, BinaryHeap, HashSet},
+    fs,
+    future::ready,
+    io::ErrorKind,
+    path::{Path, PathBuf},
+    sync::Arc,
+};
+
+pub use apple_codesign::AppleCodeSignBehavior;
 pub use driver::InstallDriver;
+use futures::{stream::FuturesUnordered, FutureExt, StreamExt};
+#[cfg(feature = "indicatif")]
+pub use installer::{
+    DefaultProgressFormatter, IndicatifReporter, IndicatifReporterBuilder, Placement,
+    ProgressFormatter,
+};
+pub use installer::{Installer, InstallerError, Reporter};
+use itertools::Itertools;
 pub use link::{link_file, LinkFileError, LinkMethod};
-use rattler_conda_types::prefix_record::PathsEntry;
+pub use python::PythonInfo;
+use rattler_conda_types::{
+    package::{IndexJson, LinkJson, NoArchLinks, PackageFile, PathsJson},
+    prefix_record::PathsEntry,
+    Platform,
+};
+use simple_spawn_blocking::Cancelled;
+use tokio::task::JoinError;
+use tracing::instrument;
 pub use transaction::{Transaction, TransactionError, TransactionOperation};
 pub use unlink::unlink_package;
 
 use crate::install::entry_point::{
     create_unix_python_entry_point, create_windows_python_entry_point,
 };
-pub use apple_codesign::AppleCodeSignBehavior;
-use futures::FutureExt;
-pub use python::PythonInfo;
-use rattler_conda_types::package::{IndexJson, LinkJson, NoArchLinks, PackageFile};
-
-use rattler_conda_types::{package::PathsJson, Platform};
-use std::cmp::Ordering;
-use std::collections::binary_heap::PeekMut;
-use std::collections::BinaryHeap;
-use std::io::ErrorKind;
-use std::sync::Arc;
-use std::{
-    future::ready,
-    path::{Path, PathBuf},
-};
-use tokio::task::JoinError;
-use tracing::instrument;
+pub use crate::install::entry_point::{get_windows_launcher, python_entry_point_template};
 
 /// An error that might occur when installing a package.
 #[derive(Debug, thiserror::Error)]
 pub enum InstallError {
     /// The operation was cancelled.
     #[error("the operation was cancelled")]
     Cancelled,
@@ -73,147 +86,173 @@
     #[error("failed to read 'link.json'")]
     FailedToReadLinkJson(#[source] std::io::Error),
 
     /// A file could not be linked.
     #[error("failed to link '{0}'")]
     FailedToLink(PathBuf, #[source] LinkFileError),
 
+    /// A directory could not be created.
+    #[error("failed to create directory '{0}")]
+    FailedToCreateDirectory(PathBuf, #[source] std::io::Error),
+
     /// The target prefix is not UTF-8.
     #[error("target prefix is not UTF-8")]
     TargetPrefixIsNotUtf8,
 
     /// Failed to create the target directory.
     #[error("failed to create target directory")]
     FailedToCreateTargetDirectory(#[source] std::io::Error),
 
-    /// A noarch package could not be installed because no python version was specified.
+    /// A noarch package could not be installed because no python version was
+    /// specified.
     #[error("cannot install noarch python package because there is no python version specified")]
     MissingPythonInfo,
 
     /// Failed to create a python entry point for a noarch package.
     #[error("failed to create Python entry point")]
     FailedToCreatePythonEntryPoint(#[source] std::io::Error),
 
     /// When post-processing of the environment fails.
     /// Post-processing involves removing clobbered paths.
     #[error("failed to post process the environment (unclobbering)")]
     PostProcessFailed(#[source] std::io::Error),
 }
 
+impl From<Cancelled> for InstallError {
+    fn from(_: Cancelled) -> Self {
+        InstallError::Cancelled
+    }
+}
+
 impl From<JoinError> for InstallError {
     fn from(err: JoinError) -> Self {
         if let Ok(panic) = err.try_into_panic() {
             std::panic::resume_unwind(panic)
         } else {
             InstallError::Cancelled
         }
     }
 }
 
-/// Additional options to pass to [`link_package`] to modify the installation process. Using
-/// [`InstallOptions::default`] works in most cases unless you want specific control over the
-/// installation process.
+/// Additional options to pass to [`link_package`] to modify the installation
+/// process. Using [`InstallOptions::default`] works in most cases unless you
+/// want specific control over the installation process.
 #[derive(Default, Clone)]
 pub struct InstallOptions {
-    /// When files are copied/linked to the target directory hardcoded paths in these files are
-    /// "patched". The hardcoded paths are replaced with the full path of the target directory, also
-    /// called the "prefix".
-    ///
-    /// However, in exceptional cases you might want to use a different prefix than the one that is
-    /// being installed to. This field allows you to do that. When its set this is used instead of
-    /// the target directory.
+    /// When files are copied/linked to the target directory hardcoded paths in
+    /// these files are "patched". The hardcoded paths are replaced with the
+    /// full path of the target directory, also called the "prefix".
+    ///
+    /// However, in exceptional cases you might want to use a different prefix
+    /// than the one that is being installed to. This field allows you to do
+    /// that. When its set this is used instead of the target directory.
     pub target_prefix: Option<PathBuf>,
 
-    /// Instead of reading the `paths.json` file from the package directory itself, use the data
-    /// specified here.
+    /// Instead of reading the `paths.json` file from the package directory
+    /// itself, use the data specified here.
     ///
-    /// This is sometimes useful to avoid reading the file twice or when you want to modify
-    /// installation process externally.
+    /// This is sometimes useful to avoid reading the file twice or when you
+    /// want to modify installation process externally.
     pub paths_json: Option<PathsJson>,
 
-    /// Instead of reading the `index.json` file from the package directory itself, use the data
-    /// specified here.
+    /// Instead of reading the `index.json` file from the package directory
+    /// itself, use the data specified here.
     ///
-    /// This is sometimes useful to avoid reading the file twice or when you want to modify
-    /// installation process externally.
+    /// This is sometimes useful to avoid reading the file twice or when you
+    /// want to modify installation process externally.
     pub index_json: Option<IndexJson>,
 
-    /// Instead of reading the `link.json` file from the package directory itself, use the data
-    /// specified here.
+    /// Instead of reading the `link.json` file from the package directory
+    /// itself, use the data specified here.
     ///
-    /// This is sometimes useful to avoid reading the file twice or when you want to modify
-    /// installation process externally.
+    /// This is sometimes useful to avoid reading the file twice or when you
+    /// want to modify installation process externally.
     ///
-    /// Because the the `link.json` file is optional this fields is using a doubly wrapped Option.
-    /// The first `Option` is to indicate whether or not this value is set. The second Option is the
-    /// [`LinkJson`] to use or `None` if you want to force that there is no [`LinkJson`].
+    /// Because the the `link.json` file is optional this fields is using a
+    /// doubly wrapped Option. The first `Option` is to indicate whether or
+    /// not this value is set. The second Option is the [`LinkJson`] to use
+    /// or `None` if you want to force that there is no [`LinkJson`].
     ///
-    /// This struct is only used if the package to be linked is a noarch Python package.
+    /// This struct is only used if the package to be linked is a noarch Python
+    /// package.
     pub link_json: Option<Option<LinkJson>>,
 
-    /// Whether or not to use symbolic links where possible. If this is set to `Some(false)`
-    /// symlinks are disabled, if set to `Some(true)` symbolic links are alwas used when specified
-    /// in the [`info/paths.json`] file even if this is not supported. If the value is set to `None`
+    /// Whether or not to use symbolic links where possible. If this is set to
+    /// `Some(false)` symlinks are disabled, if set to `Some(true)` symbolic
+    /// links are alwas used when specified in the [`info/paths.json`] file
+    /// even if this is not supported. If the value is set to `None`
     /// symbolic links are only used if they are supported.
     ///
     /// Windows only supports symbolic links in specific cases.
     pub allow_symbolic_links: Option<bool>,
 
-    /// Whether or not to use hard links where possible. If this is set to `Some(false)` the use of
-    /// hard links is disabled, if set to `Some(true)` hard links are always used when specified
-    /// in the [`info/paths.json`] file even if this is not supported. If the value is set to `None`
-    /// hard links are only used if they are supported. A dummy hardlink is created to determine
-    /// support.
+    /// Whether or not to use hard links where possible. If this is set to
+    /// `Some(false)` the use of hard links is disabled, if set to
+    /// `Some(true)` hard links are always used when specified
+    /// in the [`info/paths.json`] file even if this is not supported. If the
+    /// value is set to `None` hard links are only used if they are
+    /// supported. A dummy hardlink is created to determine support.
     ///
-    /// Hard links are supported by most OSes but often require that the hard link and its content
-    /// are on the same filesystem.
+    /// Hard links are supported by most OSes but often require that the hard
+    /// link and its content are on the same filesystem.
     pub allow_hard_links: Option<bool>,
 
-    /// Whether or not to use ref links where possible. If this is set to `Some(false)` the use of
-    /// hard links is disabled, if set to `Some(true)` ref links are always used when hard links are
-    /// specified in the [`info/paths.json`] file even if this is not supported. If the value is set
-    /// to `None` ref links are only used if they are supported.
-    ///
-    /// Ref links are only support by a small number of OSes and filesystems. If reflinking fails
-    /// for whatever reason the files are hardlinked instead (if allowed).
+    /// Whether or not to use ref links where possible. If this is set to
+    /// `Some(false)` the use of hard links is disabled, if set to
+    /// `Some(true)` ref links are always used when hard links are specified
+    /// in the [`info/paths.json`] file even if this is not supported. If the
+    /// value is set to `None` ref links are only used if they are
+    /// supported.
+    ///
+    /// Ref links are only support by a small number of OSes and filesystems. If
+    /// reflinking fails for whatever reason the files are hardlinked
+    /// instead (if allowed).
     pub allow_ref_links: Option<bool>,
 
-    /// The platform for which the package is installed. Some operations like signing require
-    /// different behavior depending on the platform. If the field is set to `None` the current
-    /// platform is used.
+    /// The platform for which the package is installed. Some operations like
+    /// signing require different behavior depending on the platform. If the
+    /// field is set to `None` the current platform is used.
     pub platform: Option<Platform>,
 
-    /// Python version information of the python distribution installed within the environment. This
-    /// is only used when installing noarch Python packages. Noarch python packages are python
-    /// packages that contain python source code that has to be installed in the correct
-    /// site-packages directory based on the version of python. This site-packages directory depends
-    /// on the version of python, therefor it must be provided when linking.
-    ///
-    /// If you're installing a noarch python package and do not provide this field, the
-    /// [`link_package`] function will return [`InstallError::MissingPythonInfo`].
+    /// Python version information of the python distribution installed within
+    /// the environment. This is only used when installing noarch Python
+    /// packages. Noarch python packages are python packages that contain
+    /// python source code that has to be installed in the correct
+    /// site-packages directory based on the version of python. This
+    /// site-packages directory depends on the version of python, therefor
+    /// it must be provided when linking.
+    ///
+    /// If you're installing a noarch python package and do not provide this
+    /// field, the [`link_package`] function will return
+    /// [`InstallError::MissingPythonInfo`].
     pub python_info: Option<PythonInfo>,
 
-    /// For binaries on macOS ARM64 (Apple Silicon), binaries need to be signed with an ad-hoc
-    /// certificate to properly work. This field controls wether or not to do that.
-    /// Code signing is only executed when the target platform is macOS ARM64. By default,
-    /// codesigning will fail the installation if it fails. This behavior can be changed by setting
-    /// this field to `AppleCodeSignBehavior::Ignore` or `AppleCodeSignBehavior::DoNothing`.
-    ///
-    /// To sign the binaries, the `/usr/bin/codesign` executable is called with `--force` and
-    /// `--sign -` arguments. The `--force` argument is used to overwrite existing signatures, and
-    /// the `--sign -` argument is used to sign with an ad-hoc certificate.
-    /// Ad-hoc signing does not use an identity at all, and identifies exactly one instance of code.
+    /// For binaries on macOS ARM64 (Apple Silicon), binaries need to be signed
+    /// with an ad-hoc certificate to properly work. This field controls
+    /// wether or not to do that. Code signing is only executed when the
+    /// target platform is macOS ARM64. By default, codesigning will fail
+    /// the installation if it fails. This behavior can be changed by setting
+    /// this field to `AppleCodeSignBehavior::Ignore` or
+    /// `AppleCodeSignBehavior::DoNothing`.
+    ///
+    /// To sign the binaries, the `/usr/bin/codesign` executable is called with
+    /// `--force` and `--sign -` arguments. The `--force` argument is used
+    /// to overwrite existing signatures, and the `--sign -` argument is
+    /// used to sign with an ad-hoc certificate. Ad-hoc signing does not use
+    /// an identity at all, and identifies exactly one instance of code.
     pub apple_codesign_behavior: AppleCodeSignBehavior,
 }
 
-/// Given an extracted package archive (`package_dir`), installs its files to the `target_dir`.
+/// Given an extracted package archive (`package_dir`), installs its files to
+/// the `target_dir`.
 ///
-/// Returns a [`PathsEntry`] for every file that was linked into the target directory. The entries
-/// are ordered in the same order as they appear in the `paths.json` file of the package.
-#[instrument(skip_all, fields(package_dir = %package_dir.display()))]
+/// Returns a [`PathsEntry`] for every file that was linked into the target
+/// directory. The entries are ordered in the same order as they appear in the
+/// `paths.json` file of the package.
+#[instrument(skip_all, fields(package_dir = % package_dir.display()))]
 pub async fn link_package(
     package_dir: &Path,
     target_dir: &Path,
     driver: &InstallDriver,
     options: InstallOptions,
 ) -> Result<Vec<PathsEntry>, InstallError> {
     // Determine the target prefix for linking
@@ -226,20 +265,22 @@
         .to_owned();
 
     // Ensure target directory exists
     tokio::fs::create_dir_all(&target_dir)
         .await
         .map_err(InstallError::FailedToCreateTargetDirectory)?;
 
-    // Reuse or read the `paths.json` and `index.json` files from the package directory
+    // Reuse or read the `paths.json` and `index.json` files from the package
+    // directory
     let paths_json = read_paths_json(package_dir, driver, options.paths_json);
     let index_json = read_index_json(package_dir, driver, options.index_json);
     let (paths_json, index_json) = tokio::try_join!(paths_json, index_json)?;
 
-    // Error out if this is a noarch python package but the python information is missing.
+    // Error out if this is a noarch python package but the python information is
+    // missing.
     if index_json.noarch.is_python() && options.python_info.is_none() {
         return Err(InstallError::MissingPythonInfo);
     }
 
     // Parse the `link.json` file and extract entry points from it.
     let link_json = if index_json.noarch.is_python() {
         read_link_json(package_dir, driver, options.link_json.flatten()).await?
@@ -261,17 +302,14 @@
         }
     );
     let allow_ref_links = options.allow_ref_links.unwrap_or(allow_hard_links);
 
     // Determine the platform to use
     let platform = options.platform.unwrap_or(Platform::current());
 
-    // Construct a channel to will hold the results of the different linking stages
-    let (tx, mut rx) = tokio::sync::mpsc::channel(driver.concurrency_limit());
-
     // compute all path renames
     let mut final_paths = compute_paths(&index_json, &paths_json, options.python_info.as_ref());
 
     // register all paths in the install driver path registry
     let clobber_paths = Arc::new(
         driver
             .clobber_registry()
@@ -280,198 +318,217 @@
 
     for (_, computed_path) in final_paths.iter_mut() {
         if let Some(clobber_rename) = clobber_paths.get(computed_path) {
             *computed_path = clobber_rename.clone();
         }
     }
 
-    // Wrap the python info in an `Arc` so we can more easily share it with async tasks.
+    // Figure out all the directories that we are going to need
+    let mut directories_to_construct = HashSet::new();
+    for (_, computed_path) in final_paths.iter() {
+        let mut current_path = computed_path.parent();
+        while let Some(path) = current_path {
+            if !path.as_os_str().is_empty() && directories_to_construct.insert(path.to_path_buf()) {
+                current_path = path.parent();
+            } else {
+                break;
+            }
+        }
+    }
+
+    let directories_target_dir = target_dir.to_path_buf();
+    driver
+        .run_blocking_io_task(move || {
+            for directory in directories_to_construct.into_iter().sorted() {
+                let full_path = directories_target_dir.join(directory);
+                match fs::create_dir(&full_path) {
+                    Ok(_) => (),
+                    Err(e) if e.kind() == ErrorKind::AlreadyExists => (),
+                    Err(e) => return Err(InstallError::FailedToCreateDirectory(full_path, e)),
+                }
+            }
+            Ok(())
+        })
+        .await?;
+
+    // Wrap the python info in an `Arc` so we can more easily share it with async
+    // tasks.
     let python_info = options.python_info.map(Arc::new);
 
     // Start linking all package files in parallel
+    let mut pending_futures = FuturesUnordered::new();
     let mut number_of_paths_entries = 0;
     for (entry, computed_path) in final_paths {
         let package_dir = package_dir.to_owned();
         let target_dir = target_dir.to_owned();
         let target_prefix = target_prefix.clone();
 
         let clobber_rename = clobber_paths.get(&entry.relative_path).cloned();
-        // Spawn a task to link the specific file. Note that these tasks are throttled by the
-        // driver. So even though we might spawn thousands of tasks they might not all run
-        // parallel because the driver dictates that only N tasks can run in parallel at the same
-        // time.
-        let tx = tx.clone();
-        driver.spawn_throttled_and_forget(move || {
-            // Return immediately if the receiver was closed. This can happen if a previous step
-            // failed. In that case we do not want to continue the installation.
-            if tx.is_closed() {
-                return;
-            }
+        let install_future = async move {
+            let _permit = driver.acquire_io_permit().await;
 
-            let linked_file_result = match link_file(
-                &entry,
-                computed_path,
-                &package_dir,
-                &target_dir,
-                &target_prefix,
-                allow_symbolic_links && !entry.no_link,
-                allow_hard_links && !entry.no_link,
-                allow_ref_links && !entry.no_link,
-                platform,
-                options.apple_codesign_behavior,
-            ) {
-                Ok(result) => Ok((
-                    number_of_paths_entries,
-                    PathsEntry {
-                        relative_path: result.relative_path,
-                        original_path: if clobber_rename.is_some() {
-                            Some(entry.relative_path)
-                        } else {
-                            None
-                        },
-                        path_type: entry.path_type.into(),
-                        no_link: entry.no_link,
-                        sha256: entry.sha256,
-                        sha256_in_prefix: Some(result.sha256),
-                        size_in_bytes: Some(result.file_size),
-                        file_mode: match result.method {
-                            LinkMethod::Patched(file_mode) => Some(file_mode),
-                            _ => None,
-                        },
-                        prefix_placeholder: entry
-                            .prefix_placeholder
-                            .as_ref()
-                            .map(|p| p.placeholder.clone()),
-                    },
-                )),
-                Err(e) => Err(InstallError::FailedToLink(entry.relative_path.clone(), e)),
+            // Spawn a blocking task to link the specific file. We use a blocking task here
+            // because filesystem access is blocking anyway so its more
+            // efficient to group them together in a single blocking call.
+            let cloned_entry = entry.clone();
+            let result = match tokio::task::spawn_blocking(move || {
+                link_file(
+                    &cloned_entry,
+                    computed_path,
+                    &package_dir,
+                    &target_dir,
+                    &target_prefix,
+                    allow_symbolic_links && !cloned_entry.no_link,
+                    allow_hard_links && !cloned_entry.no_link,
+                    allow_ref_links && !cloned_entry.no_link,
+                    platform,
+                    options.apple_codesign_behavior,
+                )
+            })
+            .await
+            .map_err(JoinError::try_into_panic)
+            {
+                Ok(Ok(linked_file)) => linked_file,
+                Ok(Err(e)) => {
+                    return Err(InstallError::FailedToLink(entry.relative_path.clone(), e))
+                }
+                Err(Ok(payload)) => std::panic::resume_unwind(payload),
+                Err(Err(_err)) => return Err(InstallError::Cancelled),
+            };
+
+            // Construct a `PathsEntry` from the result of the linking operation
+            let paths_entry = PathsEntry {
+                relative_path: result.relative_path,
+                original_path: if clobber_rename.is_some() {
+                    Some(entry.relative_path)
+                } else {
+                    None
+                },
+                path_type: entry.path_type.into(),
+                no_link: entry.no_link,
+                sha256: entry.sha256,
+                sha256_in_prefix: Some(result.sha256),
+                size_in_bytes: Some(result.file_size),
+                file_mode: match result.method {
+                    LinkMethod::Patched(file_mode) => Some(file_mode),
+                    _ => None,
+                },
+                prefix_placeholder: entry
+                    .prefix_placeholder
+                    .as_ref()
+                    .map(|p| p.placeholder.clone()),
             };
 
-            // Send the result to the main task for further processing.
-            let _ = tx.blocking_send(linked_file_result);
-        });
+            Ok(vec![(number_of_paths_entries, paths_entry)])
+        };
 
+        pending_futures.push(install_future.boxed());
         number_of_paths_entries += 1;
     }
 
-    // If this package is a noarch python package we also have to create entry points.
+    // If this package is a noarch python package we also have to create entry
+    // points.
     //
-    // Be careful with the fact that this code is currently running in parallel with the linking of
-    // individual files.
+    // Be careful with the fact that this code is currently running in parallel with
+    // the linking of individual files.
     if let Some(link_json) = link_json {
         // Parse the `link.json` file and extract entry points from it.
         let entry_points = match link_json.noarch {
             NoArchLinks::Python(entry_points) => entry_points.entry_points,
             NoArchLinks::Generic => {
                 unreachable!("we only use link.json for noarch: python packages")
             }
         };
 
         // Get python info
         let python_info = python_info
             .clone()
             .expect("should be safe because its checked above that this contains a value");
 
-        // Create entry points for each listed item. This is different between Windows and unix
-        // because on Windows, two PathEntry's are created whereas on Linux only one is created.
+        // Create entry points for each listed item. This is different between Windows
+        // and unix because on Windows, two PathEntry's are created whereas on
+        // Linux only one is created.
         for entry_point in entry_points {
-            let tx = tx.clone();
             let python_info = python_info.clone();
             let target_dir = target_dir.to_owned();
             let target_prefix = target_prefix.clone();
 
-            if platform.is_windows() {
-                driver.spawn_throttled_and_forget(move || {
-                    // Return immediately if the receiver was closed. This can happen if a previous step
-                    // failed. In that case we do not want to continue the installation.
-                    if tx.is_closed() {
-                        return;
-                    }
+            let entry_point_fut = async move {
+                // Acquire an IO permit
+                let _permit = driver.acquire_io_permit().await;
 
+                let entries = if platform.is_windows() {
                     match create_windows_python_entry_point(
                         &target_dir,
                         &target_prefix,
                         &entry_point,
                         &python_info,
                         &platform,
                     ) {
-                        Ok([a, b]) => {
-                            let _ = tx.blocking_send(Ok((number_of_paths_entries, a)));
-                            let _ = tx.blocking_send(Ok((number_of_paths_entries + 1, b)));
-                        }
-                        Err(e) => {
-                            let _ = tx.blocking_send(Err(
-                                InstallError::FailedToCreatePythonEntryPoint(e),
-                            ));
-                        }
+                        Ok([a, b]) => vec![
+                            (number_of_paths_entries, a),
+                            (number_of_paths_entries + 1, b),
+                        ],
+                        Err(e) => return Err(InstallError::FailedToCreatePythonEntryPoint(e)),
                     }
-                });
-                number_of_paths_entries += 2;
-            } else {
-                driver.spawn_throttled_and_forget(move || {
-                    // Return immediately if the receiver was closed. This can happen if a previous step
-                    // failed. In that case we do not want to continue the installation.
-                    if tx.is_closed() {
-                        return;
-                    }
-
-                    let result = match create_unix_python_entry_point(
+                } else {
+                    match create_unix_python_entry_point(
                         &target_dir,
                         &target_prefix,
                         &entry_point,
                         &python_info,
                     ) {
-                        Ok(a) => Ok((number_of_paths_entries, a)),
-                        Err(e) => Err(InstallError::FailedToCreatePythonEntryPoint(e)),
-                    };
-
-                    let _ = tx.blocking_send(result);
-                });
-                number_of_paths_entries += 1;
-            }
+                        Ok(a) => vec![(number_of_paths_entries, a)],
+                        Err(e) => return Err(InstallError::FailedToCreatePythonEntryPoint(e)),
+                    }
+                };
+
+                Ok(entries)
+            };
+
+            pending_futures.push(entry_point_fut.boxed());
+            number_of_paths_entries += if platform.is_windows() { 2 } else { 1 };
         }
     }
 
-    // Drop the transmitter on the current task. This ensures that the only alive transmitters are
-    // owned by tasks that are running in the background. When we try to receive stuff over the
-    // channel we can then know that all tasks are done if all senders are dropped.
-    drop(tx);
-
-    // Await the result of all the background tasks. The background tasks are scheduled in order,
-    // however, they can complete in any order. This means we have to reorder them back into
-    // their original order. This is achieved by waiting to add finished results to the result Vec,
-    // if the result before it has not yet finished. To that end we use a `BinaryHeap` as a priority
-    // queue which will buffer up finished results that finished before their predecessor.
+    // Await the result of all the background tasks. The background tasks are
+    // scheduled in order, however, they can complete in any order. This means
+    // we have to reorder them back into their original order. This is achieved
+    // by waiting to add finished results to the result Vec, if the result
+    // before it has not yet finished. To that end we use a `BinaryHeap` as a
+    // priority queue which will buffer up finished results that finished before
+    // their predecessor.
     //
-    // What makes this loop special is that it also aborts if any of the returned results indicate
-    // a failure.
+    // What makes this loop special is that it also aborts if any of the returned
+    // results indicate a failure.
     let mut paths = Vec::with_capacity(number_of_paths_entries);
-    let mut out_of_order_queue =
-        BinaryHeap::<OrderWrapper<PathsEntry>>::with_capacity(driver.concurrency_limit());
-    while let Some(link_result) = rx.recv().await {
-        let (index, data) = link_result?;
-
-        if index == paths.len() {
-            // If this is the next element expected in the sorted list, add it immediately. This
-            // basically means the future finished in order.
-            paths.push(data);
-
-            // By adding a finished future we have to check if there might also be another future
-            // that finished earlier and should also now be added to the result Vec.
-            while let Some(next_output) = out_of_order_queue.peek_mut() {
-                if next_output.index == paths.len() {
-                    paths.push(PeekMut::pop(next_output).data);
-                } else {
-                    break;
+    let mut out_of_order_queue = BinaryHeap::<OrderWrapper<PathsEntry>>::with_capacity(100);
+    while let Some(link_result) = pending_futures.next().await {
+        for (index, data) in link_result? {
+            if index == paths.len() {
+                // If this is the next element expected in the sorted list, add it immediately.
+                // This basically means the future finished in order.
+                paths.push(data);
+
+                // By adding a finished future we have to check if there might also be another
+                // future that finished earlier and should also now be added to
+                // the result Vec.
+                while let Some(next_output) = out_of_order_queue.peek_mut() {
+                    if next_output.index == paths.len() {
+                        paths.push(PeekMut::pop(next_output).data);
+                    } else {
+                        break;
+                    }
                 }
+            } else {
+                // Otherwise add it to the out-of-order queue. This means that we still have to
+                // wait for another element before we can add the result to the
+                // ordered list.
+                out_of_order_queue.push(OrderWrapper { index, data });
             }
-        } else {
-            // Otherwise add it to the out of order queue. This means that we still have to wait for
-            // an another element before we can add the result to the ordered list.
-            out_of_order_queue.push(OrderWrapper { index, data });
         }
     }
     debug_assert_eq!(
         paths.len(),
         paths.capacity(),
         "some futures where not added to the result"
     );
@@ -496,67 +553,67 @@
         };
 
         final_paths.push((entry.clone(), path));
     }
     final_paths
 }
 
-/// A helper function that reads the `paths.json` file from a package unless it has already been
-/// provided, in which case it is returned immediately.
+/// A helper function that reads the `paths.json` file from a package unless it
+/// has already been provided, in which case it is returned immediately.
 async fn read_paths_json(
     package_dir: &Path,
     driver: &InstallDriver,
     paths_json: Option<PathsJson>,
 ) -> Result<PathsJson, InstallError> {
     if let Some(paths_json) = paths_json {
         Ok(paths_json)
     } else {
         let package_dir = package_dir.to_owned();
         driver
-            .spawn_throttled(move || {
+            .run_blocking_io_task(move || {
                 PathsJson::from_package_directory_with_deprecated_fallback(&package_dir)
                     .map_err(InstallError::FailedToReadPathsJson)
             })
             .await
     }
 }
 
-/// A helper function that reads the `index.json` file from a package unless it has already been
-/// provided, in which case it is returned immediately.
+/// A helper function that reads the `index.json` file from a package unless it
+/// has already been provided, in which case it is returned immediately.
 async fn read_index_json(
     package_dir: &Path,
     driver: &InstallDriver,
     index_json: Option<IndexJson>,
 ) -> Result<IndexJson, InstallError> {
     if let Some(index) = index_json {
         Ok(index)
     } else {
         let package_dir = package_dir.to_owned();
         driver
-            .spawn_throttled(move || {
+            .run_blocking_io_task(move || {
                 IndexJson::from_package_directory(package_dir)
                     .map_err(InstallError::FailedToReadIndexJson)
             })
             .await
     }
 }
 
-/// A helper function that reads the `link.json` file from a package unless it has already been
-/// provided, in which case it is returned immediately.
+/// A helper function that reads the `link.json` file from a package unless it
+/// has already been provided, in which case it is returned immediately.
 async fn read_link_json(
     package_dir: &Path,
     driver: &InstallDriver,
     index_json: Option<LinkJson>,
 ) -> Result<Option<LinkJson>, InstallError> {
     if let Some(index) = index_json {
         Ok(Some(index))
     } else {
         let package_dir = package_dir.to_owned();
         driver
-            .spawn_throttled(move || {
+            .run_blocking_io_task(move || {
                 LinkJson::from_package_directory(package_dir)
                     .map_or_else(
                         |e| {
                             // Its ok if the file is not present.
                             if e.kind() == ErrorKind::NotFound {
                                 Ok(None)
                             } else {
@@ -567,15 +624,16 @@
                     )
                     .map_err(InstallError::FailedToReadLinkJson)
             })
             .await
     }
 }
 
-/// A helper struct for a `BinaryHeap` to provides ordering to items that are otherwise unordered.
+/// A helper struct for a `BinaryHeap` to provides ordering to items that are
+/// otherwise unordered.
 struct OrderWrapper<T> {
     index: usize,
     data: T,
 }
 
 impl<T> PartialEq for OrderWrapper<T> {
     fn eq(&self, other: &Self) -> bool {
@@ -621,16 +679,16 @@
                 "failed to create symlink in target directory: {e}. Disabling use of symlinks."
             );
             false
         }
     }
 }
 
-/// Returns true if it is possible to create hard links from the target directory to the package
-/// cache directory.
+/// Returns true if it is possible to create hard links from the target
+/// directory to the package cache directory.
 async fn can_create_hardlinks(target_dir: &Path, package_dir: &Path) -> bool {
     paths_have_same_filesystem(target_dir, package_dir).await
 }
 
 /// Returns true if two paths share the same filesystem
 #[cfg(unix)]
 async fn paths_have_same_filesystem(a: &Path, b: &Path) -> bool {
@@ -648,31 +706,30 @@
         (Ok(a), Ok(b)) => a.components().next() == b.components().next(),
         _ => false,
     }
 }
 
 #[cfg(test)]
 mod test {
-    use crate::install::{InstallDriver, PythonInfo};
-    use crate::{
-        get_test_data_dir,
-        install::{link_package, InstallOptions},
-        package_cache::PackageCache,
-    };
+    use std::{env::temp_dir, process::Command, str::FromStr};
+
     use futures::{stream, StreamExt};
-    use rattler_conda_types::package::ArchiveIdentifier;
-    use rattler_conda_types::{ExplicitEnvironmentSpec, Platform, Version};
+    use rattler_conda_types::{
+        package::ArchiveIdentifier, ExplicitEnvironmentSpec, Platform, Version,
+    };
     use rattler_lock::LockFile;
-
-    use std::env::temp_dir;
-    use std::process::Command;
-    use std::str::FromStr;
     use tempfile::tempdir;
     use url::Url;
 
+    use crate::{
+        get_test_data_dir,
+        install::{link_package, InstallDriver, InstallOptions, PythonInfo},
+        package_cache::PackageCache,
+    };
+
     #[tracing_test::traced_test]
     #[tokio::test]
     pub async fn test_explicit_lock() {
         // Load a prepared explicit environment file for the current platform.
         let current_platform = Platform::current();
         let explicit_env_path =
             get_test_data_dir().join(format!("python/explicit-env-{current_platform}.txt"));
@@ -713,17 +770,17 @@
     }
 
     pub async fn test_install_python(
         urls: impl Iterator<Item = Url>,
         cache_name: &str,
         platform: Platform,
     ) {
-        // Open a package cache in the systems temporary directory with a specific name. This allows
-        // us to reuse a package cache across multiple invocations of this test. Useful if you're
-        // debugging.
+        // Open a package cache in the systems temporary directory with a specific name.
+        // This allows us to reuse a package cache across multiple invocations
+        // of this test. Useful if you're debugging.
         let package_cache = PackageCache::new(temp_dir().join("rattler").join(cache_name));
 
         // Create an HTTP client we can use to download packages
         let client = reqwest_middleware::ClientWithMiddleware::from(reqwest::Client::new());
 
         // Specify python version
         let python_version =
@@ -739,15 +796,20 @@
                 let package_cache = &package_cache;
                 let install_driver = &install_driver;
                 let python_version = &python_version;
                 async move {
                     // Populate the cache
                     let package_info = ArchiveIdentifier::try_from_url(&package_url).unwrap();
                     let package_dir = package_cache
-                        .get_or_fetch_from_url(package_info, package_url.clone(), client.clone())
+                        .get_or_fetch_from_url(
+                            package_info,
+                            package_url.clone(),
+                            client.clone(),
+                            None,
+                        )
                         .await
                         .unwrap();
 
                     // Install the package to the prefix
                     link_package(
                         &package_dir,
                         prefix_path,
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/python.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/python.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-2.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-4.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-6.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__clobber_registry__tests__transaction_with_clobber-7.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/snapshots/rattler__install__test__prefix_paths.snap`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/test_utils.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/test_utils.rs`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
         // Make sure the package is available in the package cache.
         package_cache
             .get_or_fetch_from_url_with_retry(
                 &install_record.package_record,
                 install_record.url.clone(),
                 download_client.clone(),
                 default_retry_policy(),
+                None,
             )
             .map_ok(|cache_dir| Some((install_record.clone(), cache_dir)))
             .map_err(anyhow::Error::from)
             .await
             .unwrap()
     } else {
         None
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/transaction.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/transaction.rs`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 
 /// Error that occurred during creation of a Transaction
 #[derive(Debug, thiserror::Error)]
 pub enum TransactionError {
     /// An error that happens if the python version could not be parsed.
     #[error(transparent)]
     PythonInfoError(#[from] PythonInfoError),
+
+    /// The operation was cancelled
+    #[error("the operation was cancelled")]
+    Cancelled,
 }
 
 /// Describes an operation to perform
 #[derive(Debug, Clone, PartialEq, Eq)]
 pub enum TransactionOperation<Old, New> {
     /// The given package record should be installed
     Install(New),
@@ -58,14 +62,15 @@
             | TransactionOperation::Reinstall(old)
             | TransactionOperation::Remove(old) => Some(old),
         }
     }
 }
 
 /// Describes the operations to perform to bring an environment from one state into another.
+#[derive(Debug)]
 pub struct Transaction<Old, New> {
     /// A list of operations to update an environment
     pub operations: Vec<TransactionOperation<Old, New>>,
 
     /// The python version of the target state, or None if python doesnt exist in the environment.
     pub python_info: Option<PythonInfo>,
 
@@ -80,23 +85,33 @@
 impl<Old, New> Transaction<Old, New> {
     /// Return an iterator over the prefix records of all packages that are going to be removed.
     pub fn removed_packages(&self) -> impl Iterator<Item = &Old> + '_ {
         self.operations
             .iter()
             .filter_map(TransactionOperation::record_to_remove)
     }
+
+    /// Returns the number of records to install.
+    pub fn packages_to_uninstall(&self) -> usize {
+        self.removed_packages().count()
+    }
 }
 
 impl<Old: AsRef<New>, New> Transaction<Old, New> {
     /// Return an iterator over the prefix records of all packages that are going to be installed.
     pub fn installed_packages(&self) -> impl Iterator<Item = &New> + '_ {
         self.operations
             .iter()
             .filter_map(TransactionOperation::record_to_install)
     }
+
+    /// Returns the number of records to install.
+    pub fn packages_to_install(&self) -> usize {
+        self.installed_packages().count()
+    }
 }
 
 impl<Old: AsRef<PackageRecord>, New: AsRef<PackageRecord>> Transaction<Old, New> {
     /// Constructs a [`Transaction`] by taking the current situation and diffing that against the
     /// desired situation.
     pub fn from_current_and_desired<
         CurIter: IntoIterator<Item = Old>,
@@ -151,15 +166,15 @@
             if let Some(old_record) = old_record {
                 if !describe_same_content(record.as_ref(), old_record.as_ref()) {
                     // if the content changed, we need to reinstall (remove and install)
                     operations.push(TransactionOperation::Change {
                         old: old_record,
                         new: record,
                     });
-                } else if needs_python_relink {
+                } else if needs_python_relink && old_record.as_ref().noarch.is_python() {
                     // when the python version changed, we need to relink all noarch packages
                     // to recompile the bytecode
                     operations.push(TransactionOperation::Reinstall(old_record));
                 }
                 // if the content is the same, we dont need to do anything
             } else {
                 operations.push(TransactionOperation::Install(record));
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/install/unlink.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/install/unlink.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/lib.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/lib.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/package_cache.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/package_cache.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,55 @@
-//! This module provides functionality to cache extracted Conda packages. See [`PackageCache`].
+//! This module provides functionality to cache extracted Conda packages. See
+//! [`PackageCache`].
+
+use std::{
+    error::Error,
+    fmt::{Display, Formatter},
+    future::Future,
+    path::PathBuf,
+    sync::Arc,
+};
 
-use crate::validation::validate_package_directory;
 use chrono::Utc;
 use fxhash::FxHashMap;
 use itertools::Itertools;
+use parking_lot::Mutex;
 use rattler_conda_types::{package::ArchiveIdentifier, PackageRecord};
 use rattler_digest::Sha256Hash;
 use rattler_networking::retry_policies::{DoNotRetryPolicy, RetryDecision, RetryPolicy};
-use rattler_package_streaming::ExtractError;
+use rattler_package_streaming::{DownloadReporter, ExtractError};
 use reqwest::StatusCode;
-use std::error::Error;
-use std::{
-    fmt::{Display, Formatter},
-    future::Future,
-    path::PathBuf,
-    sync::{Arc, Mutex},
-};
 use tokio::sync::broadcast;
 use tracing::Instrument;
 use url::Url;
 
+use crate::validation::validate_package_directory;
+
+/// A trait that can be implemented to report progress of the download and
+/// validation process.
+pub trait CacheReporter: Send + Sync {
+    /// Called when validation starts
+    fn on_validate_start(&self) -> usize;
+    /// Called when validation completex
+    fn on_validate_complete(&self, index: usize);
+    /// Called when a download starts
+    fn on_download_start(&self) -> usize;
+    /// Called with regular updates on the download progress
+    fn on_download_progress(&self, index: usize, progress: u64, total: Option<u64>);
+    /// Called when a download completes
+    fn on_download_completed(&self, index: usize);
+}
+
 /// A [`PackageCache`] manages a cache of extracted Conda packages on disk.
 ///
-/// The store does not provide an implementation to get the data into the store. Instead this is
-/// left up to the user when the package is requested. If the package is found in the cache it is
-/// returned immediately. However, if the cache is stale a user defined function is called to
-/// populate the cache. This separates the corners between caching and fetching of the content.
+/// The store does not provide an implementation to get the data into the store.
+/// Instead this is left up to the user when the package is requested. If the
+/// package is found in the cache it is returned immediately. However, if the
+/// cache is stale a user defined function is called to populate the cache. This
+/// separates the corners between caching and fetching of the content.
 #[derive(Clone)]
 pub struct PackageCache {
     inner: Arc<Mutex<PackageCacheInner>>,
 }
 
 /// Provides a unique identifier for packages in the cache.
 /// TODO: This could not be unique over multiple subdir. How to handle?
@@ -85,15 +105,16 @@
 
 #[derive(Default)]
 struct Package {
     path: Option<PathBuf>,
     inflight: Option<broadcast::Sender<Result<PathBuf, PackageCacheError>>>,
 }
 
-/// An error that might be returned from one of the caching function of the [`PackageCache`].
+/// An error that might be returned from one of the caching function of the
+/// [`PackageCache`].
 #[derive(Debug, Clone, thiserror::Error)]
 pub enum PackageCacheError {
     /// An error occurred while fetching the package.
     #[error(transparent)]
     FetchError(#[from] Arc<dyn std::error::Error + Send + Sync + 'static>),
 }
 
@@ -106,44 +127,46 @@
                 packages: FxHashMap::default(),
             })),
         }
     }
 
     /// Returns the directory that contains the specified package.
     ///
-    /// If the package was previously successfully fetched and stored in the cache the directory
-    /// containing the data is returned immediately. If the package was not previously fetch the
-    /// filesystem is checked to see if a directory with valid package content exists. Otherwise,
-    /// the user provided `fetch` function is called to populate the cache.
+    /// If the package was previously successfully fetched and stored in the
+    /// cache the directory containing the data is returned immediately. If
+    /// the package was not previously fetch the filesystem is checked to
+    /// see if a directory with valid package content exists. Otherwise, the
+    /// user provided `fetch` function is called to populate the cache.
     ///
-    /// If the package is already being fetched by another task/thread the request is coalesced. No
-    /// duplicate fetch is performed.
+    /// If the package is already being fetched by another task/thread the
+    /// request is coalesced. No duplicate fetch is performed.
     pub async fn get_or_fetch<F, Fut, E>(
         &self,
         pkg: impl Into<CacheKey>,
         fetch: F,
+        reporter: Option<Arc<dyn CacheReporter>>,
     ) -> Result<PathBuf, PackageCacheError>
     where
         F: (FnOnce(PathBuf) -> Fut) + Send + 'static,
         Fut: Future<Output = Result<(), E>> + Send + 'static,
         E: std::error::Error + Send + Sync + 'static,
     {
         let cache_key = pkg.into();
 
         // Get the package entry
         let (package, pkg_cache_dir) = {
-            let mut inner = self.inner.lock().unwrap();
+            let mut inner = self.inner.lock();
             let destination = inner.path.join(cache_key.to_string());
             let package = inner.packages.entry(cache_key).or_default().clone();
             (package, destination)
         };
 
         let mut rx = {
             // Only sync code in this block
-            let mut inner = package.lock().unwrap();
+            let mut inner = package.lock();
 
             // If there exists an existing value in our cache, we can return that.
             if let Some(path) = inner.path.as_ref() {
                 return Ok(path.clone());
             }
 
             // Is there an in-flight requests for the package?
@@ -152,23 +175,23 @@
             } else {
                 // There is no in-flight requests so we start one!
                 let (tx, rx) = broadcast::channel(1);
                 inner.inflight = Some(tx.clone());
 
                 let package = package.clone();
                 tokio::spawn(async move {
-                    let result = validate_or_fetch_to_cache(pkg_cache_dir.clone(), fetch)
+                    let result = validate_or_fetch_to_cache(pkg_cache_dir.clone(), fetch, reporter)
                         .instrument(
                             tracing::debug_span!("validating", path = %pkg_cache_dir.display()),
                         )
                         .await;
 
                     {
                         // only sync code in this block
-                        let mut package = package.lock().unwrap();
+                        let mut package = package.lock();
                         package.inflight = None;
 
                         match result {
                             Ok(_) => {
                                 package.path.replace(pkg_cache_dir.clone());
                                 let _ = tx.send(Ok(pkg_cache_dir));
                             }
@@ -184,50 +207,60 @@
         };
 
         rx.recv().await.expect("in-flight request has died")
     }
 
     /// Returns the directory that contains the specified package.
     ///
-    /// This is a convenience wrapper around `get_or_fetch` which fetches the package from the given
-    /// URL if the package could not be found in the cache.
+    /// This is a convenience wrapper around `get_or_fetch` which fetches the
+    /// package from the given URL if the package could not be found in the
+    /// cache.
     pub async fn get_or_fetch_from_url(
         &self,
         pkg: impl Into<CacheKey>,
         url: Url,
         client: reqwest_middleware::ClientWithMiddleware,
+        reporter: Option<Arc<dyn CacheReporter>>,
     ) -> Result<PathBuf, PackageCacheError> {
-        self.get_or_fetch_from_url_with_retry(pkg, url, client, DoNotRetryPolicy)
+        self.get_or_fetch_from_url_with_retry(pkg, url, client, DoNotRetryPolicy, reporter)
             .await
     }
 
     /// Returns the directory that contains the specified package.
     ///
-    /// This is a convenience wrapper around `get_or_fetch` which fetches the package from the given
-    /// URL if the package could not be found in the cache.
+    /// This is a convenience wrapper around `get_or_fetch` which fetches the
+    /// package from the given URL if the package could not be found in the
+    /// cache.
     pub async fn get_or_fetch_from_url_with_retry(
         &self,
         pkg: impl Into<CacheKey>,
         url: Url,
         client: reqwest_middleware::ClientWithMiddleware,
         retry_policy: impl RetryPolicy + Send + 'static,
+        reporter: Option<Arc<dyn CacheReporter>>,
     ) -> Result<PathBuf, PackageCacheError> {
         let request_start = Utc::now();
         let cache_key = pkg.into();
         let sha256 = cache_key.sha256();
+        let download_reporter = reporter.clone();
         self.get_or_fetch(cache_key, move |destination| async move {
             let mut current_try = 0;
             loop {
                 current_try += 1;
                 tracing::debug!("downloading {} to {}", &url, destination.display());
+
                 let result = rattler_package_streaming::reqwest::tokio::extract(
                     client.clone(),
                     url.clone(),
                     &destination,
                     sha256,
+                    download_reporter.clone().map(|reporter| Arc::new(PassthroughReporter {
+                        reporter,
+                        index: Mutex::new(None),
+                    }) as Arc::<dyn DownloadReporter>)
                 )
                 .await;
 
                 // Extract any potential error
                 let Err(err) = result else { return Ok(()); };
 
                 // Only retry on certain errors.
@@ -259,34 +292,45 @@
                     destination.display(),
                     err,
                     current_try,
                     duration
                 );
                 tokio::time::sleep(duration).await;
             }
-        })
+        }, reporter)
         .await
     }
 }
 
-/// Validates that the package that is currently stored is a valid package and otherwise calls the
-/// `fetch` method to populate the cache.
+/// Validates that the package that is currently stored is a valid package and
+/// otherwise calls the `fetch` method to populate the cache.
 async fn validate_or_fetch_to_cache<F, Fut, E>(
     path: PathBuf,
     fetch: F,
+    reporter: Option<Arc<dyn CacheReporter>>,
 ) -> Result<(), PackageCacheError>
 where
     F: FnOnce(PathBuf) -> Fut + Send,
     Fut: Future<Output = Result<(), E>> + 'static,
     E: std::error::Error + Send + Sync + 'static,
 {
     // If the directory already exists validate the contents of the package
     if path.is_dir() {
         let path_inner = path.clone();
-        match tokio::task::spawn_blocking(move || validate_package_directory(&path_inner)).await {
+
+        let reporter = reporter.as_deref().map(|r| (r, r.on_validate_start()));
+
+        let validation_result =
+            tokio::task::spawn_blocking(move || validate_package_directory(&path_inner)).await;
+
+        if let Some((reporter, index)) = reporter {
+            reporter.on_validate_complete(index);
+        }
+
+        match validation_result {
             Ok(Ok(_)) => {
                 tracing::debug!("validation succeeded");
                 return Ok(());
             }
             Ok(Err(e)) => {
                 tracing::warn!("validation for {path:?} failed: {e}");
                 if let Some(cause) = e.source() {
@@ -307,18 +351,50 @@
 
     // Otherwise, defer to populate method to fill our cache.
     fetch(path)
         .await
         .map_err(|e| PackageCacheError::FetchError(Arc::new(e)))
 }
 
+struct PassthroughReporter {
+    reporter: Arc<dyn CacheReporter>,
+    index: Mutex<Option<usize>>,
+}
+
+impl DownloadReporter for PassthroughReporter {
+    fn on_download_start(&self) {
+        let index = self.reporter.on_download_start();
+        assert!(
+            self.index.lock().replace(index).is_none(),
+            "on_download_start was called multiple times"
+        );
+    }
+
+    fn on_download_progress(&self, bytes_downloaded: u64, total_bytes: Option<u64>) {
+        let index = self.index.lock().expect("on_download_start was not called");
+        self.reporter
+            .on_download_progress(index, bytes_downloaded, total_bytes);
+    }
+
+    fn on_download_complete(&self) {
+        let index = self
+            .index
+            .lock()
+            .take()
+            .expect("on_download_start was not called");
+        self.reporter.on_download_completed(index);
+    }
+}
+
 #[cfg(test)]
 mod test {
-    use super::PackageCache;
-    use crate::{get_test_data_dir, validation::validate_package_directory};
+    use std::{
+        convert::Infallible, fs::File, future::IntoFuture, net::SocketAddr, path::Path, sync::Arc,
+    };
+
     use assert_matches::assert_matches;
     use axum::{
         body::Body,
         extract::State,
         http::{Request, StatusCode},
         middleware,
         middleware::Next,
@@ -326,23 +402,23 @@
         routing::get_service,
         Router,
     };
     use bytes::Bytes;
     use futures::stream;
     use rattler_conda_types::package::{ArchiveIdentifier, PackageFile, PathsJson};
     use rattler_networking::retry_policies::{DoNotRetryPolicy, ExponentialBackoffBuilder};
-    use std::{
-        convert::Infallible, fs::File, future::IntoFuture, net::SocketAddr, path::Path, sync::Arc,
-    };
     use tempfile::tempdir;
     use tokio::sync::Mutex;
     use tokio_stream::StreamExt;
     use tower_http::services::ServeDir;
     use url::Url;
 
+    use super::PackageCache;
+    use crate::{get_test_data_dir, validation::validate_package_directory};
+
     #[tokio::test]
     pub async fn test_package_cache() {
         let tar_archive_path =
             get_test_data_dir().join("ros-noetic-rosbridge-suite-0.11.14-py39h6fdeb60_14.tar.bz2");
 
         // Read the paths.json file straight from the tar file.
         let paths = {
@@ -364,23 +440,24 @@
             .get_or_fetch(
                 ArchiveIdentifier::try_from_path(&tar_archive_path).unwrap(),
                 move |destination| async move {
                     rattler_package_streaming::tokio::fs::extract(&tar_archive_path, &destination)
                         .await
                         .map(|_| ())
                 },
+                None,
             )
             .await
             .unwrap();
 
         // Validate the contents of the package
         let (_, current_paths) = validate_package_directory(&package_dir).unwrap();
 
-        // Make sure that the paths are the same as what we would expect from the original tar
-        // archive.
+        // Make sure that the paths are the same as what we would expect from the
+        // original tar archive.
         assert_eq!(current_paths, paths);
     }
 
     /// A helper middleware function that fails the first two requests.
     async fn fail_the_first_two_requests(
         State(count): State<Arc<Mutex<i32>>>,
         req: Request<Body>,
@@ -447,32 +524,34 @@
 
     async fn test_flaky_package_cache(archive_name: &str, middleware: Middleware) {
         let static_dir = get_test_data_dir();
         println!("Serving files from {}", static_dir.display());
         // Construct a service that serves raw files from the test directory
         let service = get_service(ServeDir::new(static_dir));
 
-        // Construct a router that returns data from the static dir but fails the first try.
+        // Construct a router that returns data from the static dir but fails the first
+        // try.
         let request_count = Arc::new(Mutex::new(0));
         let router = Router::new().route_service("/*key", service);
 
         let router = match middleware {
             Middleware::FailTheFirstTwoRequests => router.layer(middleware::from_fn_with_state(
                 request_count.clone(),
                 fail_the_first_two_requests,
             )),
             Middleware::FailAfterBytes(size) => router.layer(middleware::from_fn_with_state(
                 (request_count.clone(), Arc::new(Mutex::new(size))),
                 fail_with_half_package,
             )),
         };
 
-        // Construct the server that will listen on localhost but with a *random port*. The random
-        // port is very important because it enables creating multiple instances at the same time.
-        // We need this to be able to run tests in parallel.
+        // Construct the server that will listen on localhost but with a *random port*.
+        // The random port is very important because it enables creating
+        // multiple instances at the same time. We need this to be able to run
+        // tests in parallel.
         let addr = SocketAddr::new([127, 0, 0, 1].into(), 0);
         let listener = tokio::net::TcpListener::bind(&addr).await.unwrap();
         let addr = listener.local_addr().unwrap();
 
         let service = router.into_make_service();
         tokio::spawn(axum::serve(listener, service).into_future());
 
@@ -484,14 +563,15 @@
         // Do the first request without
         let result = cache
             .get_or_fetch_from_url_with_retry(
                 ArchiveIdentifier::try_from_filename(archive_name).unwrap(),
                 server_url.join(archive_name).unwrap(),
                 reqwest::Client::default().into(),
                 DoNotRetryPolicy,
+                None,
             )
             .await;
 
         // First request without retry policy should fail
         assert_matches!(result, Err(_));
         {
             let request_count_lock = request_count.lock().await;
@@ -501,14 +581,15 @@
         // The second one should fail after the 2nd try
         let result = cache
             .get_or_fetch_from_url_with_retry(
                 ArchiveIdentifier::try_from_filename(archive_name).unwrap(),
                 server_url.join(archive_name).unwrap(),
                 reqwest::Client::default().into(),
                 ExponentialBackoffBuilder::default().build_with_max_retries(3),
+                None,
             )
             .await;
 
         assert!(result.is_ok());
         {
             let request_count_lock = request_count.lock().await;
             assert_eq!(*request_count_lock, 3, "Expected there to be 3 requests");
```

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/range.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/range.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/local_dependencies/rattler/src/validation.rs` & `py_rattler-0.6.0/local_dependencies/rattler/src/validation.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 //! `paths.json` file.
 //!
 //! Very old Conda packages do not contain a `paths.json` file. These packages contain a
 //! (deprecated) `files` file as well as optionally a `has_prefix` and some other files. If the
 //! `paths.json` file is missing these deprecated files are used instead to reconstruct a
 //! [`PathsJson`] object. See [`PathsJson::from_deprecated_package_directory`] for more information.
 
+use digest::Digest;
 use rattler_conda_types::package::{IndexJson, PackageFile, PathType, PathsEntry, PathsJson};
-use rattler_digest::compute_file_digest;
+use rattler_digest::Sha256;
 use std::{
-    fs::Metadata,
     io::ErrorKind,
     path::{Path, PathBuf},
 };
 
 /// An error that is returned by [`validate_package_directory`] if the contents of the directory seems to be
 /// corrupted.
 #[derive(Debug, thiserror::Error)]
@@ -131,53 +131,66 @@
 /// Determine whether the information in the [`PathsEntry`] matches the file in the package directory.
 fn validate_package_entry(
     package_dir: &Path,
     entry: &PathsEntry,
 ) -> Result<(), PackageEntryValidationError> {
     let path = package_dir.join(&entry.relative_path);
 
-    // Get the metadata for the entry
-    let metadata = match std::fs::symlink_metadata(&path) {
-        Ok(metadata) => metadata,
-        Err(e) if e.kind() == ErrorKind::NotFound => {
-            return Err(PackageEntryValidationError::NotFound);
-        }
-        Err(e) => return Err(PackageEntryValidationError::GetMetadataFailed(e)),
-    };
-
     // Validate based on the type of path
     match entry.path_type {
-        PathType::HardLink => validate_package_hard_link_entry(path, entry, metadata),
-        PathType::SoftLink => validate_package_soft_link_entry(path, entry, metadata),
-        PathType::Directory => validate_package_directory_entry(path, entry, metadata),
+        PathType::HardLink => validate_package_hard_link_entry(path, entry),
+        PathType::SoftLink => validate_package_soft_link_entry(path, entry),
+        PathType::Directory => validate_package_directory_entry(path, entry),
     }
 }
 
 /// Determine whether the information in the [`PathsEntry`] matches the file at the specified path.
 fn validate_package_hard_link_entry(
     path: PathBuf,
     entry: &PathsEntry,
-    metadata: Metadata,
 ) -> Result<(), PackageEntryValidationError> {
     debug_assert!(entry.path_type == PathType::HardLink);
 
+    // Short-circuit if we have no validation reference
+    if entry.sha256.is_none() && entry.size_in_bytes.is_none() {
+        if !path.is_file() {
+            return Err(PackageEntryValidationError::NotFound);
+        }
+        return Ok(());
+    }
+
+    // Open the file for reading
+    let mut file = match std::fs::File::open(&path) {
+        Ok(file) => file,
+        Err(e) if e.kind() == ErrorKind::NotFound => {
+            return Err(PackageEntryValidationError::NotFound);
+        }
+        Err(e) => return Err(PackageEntryValidationError::IoError(e)),
+    };
+
     // Validate the size of the file
     if let Some(size_in_bytes) = entry.size_in_bytes {
-        if size_in_bytes != metadata.len() {
+        let actual_file_len = file
+            .metadata()
+            .map_err(PackageEntryValidationError::IoError)?
+            .len();
+        if size_in_bytes != actual_file_len {
             return Err(PackageEntryValidationError::IncorrectSize(
                 size_in_bytes,
-                metadata.len(),
+                actual_file_len,
             ));
         }
     }
 
     // Check the SHA256 hash of the file
     if let Some(expected_hash) = &entry.sha256 {
         // Determine the hash of the file on disk
-        let hash = compute_file_digest::<rattler_digest::Sha256>(&path)?;
+        let mut hasher = Sha256::default();
+        std::io::copy(&mut file, &mut hasher)?;
+        let hash = hasher.finalize();
 
         // Compare the two hashes
         if expected_hash != &hash {
             return Err(PackageEntryValidationError::HashMismatch(
                 format!("{expected_hash:x}"),
                 format!("{hash:x}"),
             ));
@@ -186,41 +199,39 @@
 
     Ok(())
 }
 
 /// Determine whether the information in the [`PathsEntry`] matches the symbolic link at the specified
 /// path.
 fn validate_package_soft_link_entry(
-    _path: PathBuf,
+    path: PathBuf,
     entry: &PathsEntry,
-    metadata: Metadata,
 ) -> Result<(), PackageEntryValidationError> {
     debug_assert!(entry.path_type == PathType::SoftLink);
 
-    if !metadata.is_symlink() {
+    if !path.is_symlink() {
         return Err(PackageEntryValidationError::ExpectedSymlink);
     }
 
     // TODO: Validate symlink content. Dont validate the SHA256 hash of the file because since a
     // symlink will most likely point to another file added as a hardlink by the package this is
     // double work. Instead check that the symlink is correct e.g. `../a` points to the same file as
     // `b/../../a` but they are different.
 
     Ok(())
 }
 
 /// Determine whether the information in the [`PathsEntry`] matches the directory at the specified path.
 fn validate_package_directory_entry(
-    _path: PathBuf,
+    path: PathBuf,
     entry: &PathsEntry,
-    metadata: Metadata,
 ) -> Result<(), PackageEntryValidationError> {
     debug_assert!(entry.path_type == PathType::Directory);
 
-    if metadata.is_dir() {
+    if path.is_dir() {
         Ok(())
     } else {
         Err(PackageEntryValidationError::ExpectedDirectory)
     }
 }
 
 #[cfg(test)]
```

### Comparing `py_rattler-0.5.0/Cargo.toml` & `py_rattler-0.6.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-rattler"
-version = "0.5.0"
+version = "0.6.0"
 edition = "2021"
 license = "BSD-3-Clause"
 publish = false
 
 [lib]
 name = "rattler"
 crate-type = ["cdylib"]
@@ -13,44 +13,46 @@
 default = ["native-tls"]
 native-tls = ["rattler_networking/native-tls", "rattler_repodata_gateway/native-tls"]
 rustls-tls = ["rattler_networking/rustls-tls", "rattler_repodata_gateway/rustls-tls"]
 vendored-openssl = ["openssl", "openssl/vendored"]
 
 [dependencies]
 anyhow = "1.0.82"
+chrono = { version = "0.4" }
 futures = "0.3.30"
 
-rattler = { path = "local_dependencies/rattler", default-features = false }
+rattler = { path = "local_dependencies/rattler", default-features = false, features = ["indicatif"] }
 rattler_repodata_gateway = { path = "local_dependencies/rattler_repodata_gateway", default-features = false, features = [
     "sparse",
+    "gateway",
 ] }
 rattler_conda_types = { path = "local_dependencies/rattler_conda_types", default-features = false }
 rattler_digest = { path = "local_dependencies/rattler_digest" }
 rattler_networking = { path = "local_dependencies/rattler_networking", default-features = false }
 rattler_shell = { path = "local_dependencies/rattler_shell", default-features = false }
 rattler_virtual_packages = { path = "local_dependencies/rattler_virtual_packages", default-features = false }
 rattler_solve = { path = "local_dependencies/rattler_solve", default-features = false, features = [
     "resolvo",
 ] }
 rattler_index = { path = "local_dependencies/rattler_index" }
 rattler_lock = { path = "local_dependencies/rattler_lock", default-features = false }
 rattler_package_streaming = { path = "local_dependencies/rattler_package_streaming", default-features = false }
-
 pyo3 = { version = "0.20", features = [
     "abi3-py38",
     "extension-module",
     "multiple-pymethods",
+    "chrono"
 ] }
 pyo3-asyncio = { version = "0.20", features = ["tokio-runtime"] }
 tokio = { version = "1.37" }
 
 reqwest = { version = "0.12.3", default-features = false }
 reqwest-middleware = "0.3.0"
 
-thiserror = "1.0.58"
+thiserror = "1.0.61"
 url = "2.5.0"
 
 openssl = { version = "0.10", optional = true }
 pep508_rs = "0.4.2"
 
 [build-dependencies]
 pyo3-build-config = "0.21"
```

### Comparing `py_rattler-0.5.0/.gitignore` & `py_rattler-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/LICENSE` & `py_rattler-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/README.md` & `py_rattler-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,41 +30,37 @@
 Rattler is a library that provides common functionality used within the conda ecosystem ([what is conda & conda-forge?](#what-is-conda--conda-forge)).
 The goal of the library is to enable programs and other libraries to easily interact with the conda ecosystem without being dependent on Python.
 Its primary use case is as a library that you can use to provide conda related workflows in your own tools.
 
 Rattler is written in Rust and tries to provide a clean API to its functionalities (see: [Components](#components)). 
 With the primary goal in mind we aim to provide bindings to different languages to make it easy to integrate Rattler in non-rust projects.
 
-Rattler is actively used within the https://prefix.dev backend.
+Rattler is actively used by [pixi](https://github.com/prefix-dev/pixi), [rattler-build](https://github.com/prefix-dev/rattler-build), and the https://prefix.dev backend.
 
 ## Showcase
 
 This repository also contains a binary (use `cargo run` to try) that shows some of the capabilities of the library.
 This is an example of installing an environment containing `cowpy` and all its dependencies _from scratch_ (including Python!):
 
 ![Installing an environment](https://github.com/mamba-org/rattler/assets/4995967/c7946f6e-28a9-41ef-8836-ef4b4c94d273)
 
 ## Give it a try!
 
 Before you begin, make sure you have the following prerequisites:
 - A recent version of [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
-- A recent version of [micromamba](https://github.com/mamba-org/micromamba-releases)
+- A recent version of [pixi](https://github.com/prefix-dev/pixi)
 
 Follow these steps to clone, compile, and run the rattler project:
 ```shell
 # Clone the rattler repository along with its submodules:
 git clone --recursive https://github.com/mamba-org/rattler.git
 cd rattler
 
-# Set up an environment with the required dependencies for compiling rattler and libsolv:
-micromamba create -f environment.yml
-micromamba activate rattler-env
-
 # Compile and execute rattler to create a JupyterLab instance:
-cargo run --release --bin rattler create jupyterlab
+pixi run rattler create jupyterlab
 ```
 
 The above command will execute the `rattler` executable in release mode.
 It will download and install an environment into the `.prefix` folder that contains [`jupyterlab`](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) and all the dependencies required to run it (like `python`)
 
 Run the following command to start jupyterlab:
 
@@ -94,19 +90,26 @@
 
 * **rattler_conda_types**: foundational types for all datastructures used withing the conda eco-system.
 * **rattler_package_streaming**: provides functionality to download, extract and create conda package archives.  
 * **rattler_repodata_gateway**: downloads, reads and processes information about existing conda packages from an index.
 * **rattler_shell**: code to activate an existing environment and run programs in it.
 * **rattler_solve**: a backend agnostic library to solve the package satisfiability problem.
 * **rattler_virtual_packages**: a crate to detect system capabilities.
+* **rattler_index**: create local conda channels from local packages.
 * **rattler**: functionality to create complete environments from scratch using the crates above.
+* **rattler-lock**: a library to create and parse lockfiles for conda environments.
+* **rattler-networking**: common functionality for networking, like authentication, mirroring and more.
 * **rattler-bin**: an example of a package manager using all the crates above (see: [showcase](#showcase))
 
 You can find these crates in the `crates` folder.
 
+Additionally, we provide Python bindings for most of the functionalities provided by the above crates.
+A python package `py-rattler` is available on [conda-forge](https://prefix.dev/channels/conda-forge/packages/py-rattler) and [PyPI](https://pypi.org/project/py-rattler/).
+Documatation for the python bindings can be found [here](https://mamba-org.github.io/rattler/py-rattler).
+
 ## What is conda & conda-forge?
 
 The conda ecosystem provides **cross-platform**, **binary** packages that you can use with **any programming language**.
 `conda` is an open-source package management system and environment management system that can install and manage multiple versions of software packages and their dependencies.
 `conda` is written in Python.
 The aim of Rattler is to provide all functionality required to work with the conda ecosystem from Rust.
 Rattler is not a reimplementation of `conda`.
```

#### html2text {}

```diff
@@ -19,32 +19,31 @@
 conda-forge?](#what-is-conda--conda-forge)). The goal of the library is to
 enable programs and other libraries to easily interact with the conda ecosystem
 without being dependent on Python. Its primary use case is as a library that
 you can use to provide conda related workflows in your own tools. Rattler is
 written in Rust and tries to provide a clean API to its functionalities (see:
 [Components](#components)). With the primary goal in mind we aim to provide
 bindings to different languages to make it easy to integrate Rattler in non-
-rust projects. Rattler is actively used within the https://prefix.dev backend.
-## Showcase This repository also contains a binary (use `cargo run` to try)
-that shows some of the capabilities of the library. This is an example of
-installing an environment containing `cowpy` and all its dependencies _from
-scratch_ (including Python!): ![Installing an environment](https://github.com/
-mamba-org/rattler/assets/4995967/c7946f6e-28a9-41ef-8836-ef4b4c94d273) ## Give
-it a try! Before you begin, make sure you have the following prerequisites: - A
-recent version of [git](https://git-scm.com/book/en/v2/Getting-Started-
-Installing-Git) - A recent version of [micromamba](https://github.com/mamba-
-org/micromamba-releases) Follow these steps to clone, compile, and run the
+rust projects. Rattler is actively used by [pixi](https://github.com/prefix-
+dev/pixi), [rattler-build](https://github.com/prefix-dev/rattler-build), and
+the https://prefix.dev backend. ## Showcase This repository also contains a
+binary (use `cargo run` to try) that shows some of the capabilities of the
+library. This is an example of installing an environment containing `cowpy` and
+all its dependencies _from scratch_ (including Python!): ![Installing an
+environment](https://github.com/mamba-org/rattler/assets/4995967/c7946f6e-28a9-
+41ef-8836-ef4b4c94d273) ## Give it a try! Before you begin, make sure you have
+the following prerequisites: - A recent version of [git](https://git-scm.com/
+book/en/v2/Getting-Started-Installing-Git) - A recent version of [pixi](https:/
+/github.com/prefix-dev/pixi) Follow these steps to clone, compile, and run the
 rattler project: ```shell # Clone the rattler repository along with its
 submodules: git clone --recursive https://github.com/mamba-org/rattler.git cd
-rattler # Set up an environment with the required dependencies for compiling
-rattler and libsolv: micromamba create -f environment.yml micromamba activate
-rattler-env # Compile and execute rattler to create a JupyterLab instance:
-cargo run --release --bin rattler create jupyterlab ``` The above command will
-execute the `rattler` executable in release mode. It will download and install
-an environment into the `.prefix` folder that contains [`jupyterlab`](https://
+rattler # Compile and execute rattler to create a JupyterLab instance: pixi run
+rattler create jupyterlab ``` The above command will execute the `rattler`
+executable in release mode. It will download and install an environment into
+the `.prefix` folder that contains [`jupyterlab`](https://
 jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) and all the
 dependencies required to run it (like `python`) Run the following command to
 start jupyterlab: ```shell # on windows .\.prefix\Scripts\jupyter-lab.exe # on
 linux or macOS ./.prefix/bin/jupyter-lab ``` Voila! You have a working
 installation of jupyterlab installed on your system! You can of course install
 any package you want this way. Try it! ## Contributing ð We would love to
 have you contribute! See the CONTRIBUTION.md for more info. For questions,
@@ -55,23 +54,32 @@
 the conda eco-system. * **rattler_package_streaming**: provides functionality
 to download, extract and create conda package archives. *
 **rattler_repodata_gateway**: downloads, reads and processes information about
 existing conda packages from an index. * **rattler_shell**: code to activate an
 existing environment and run programs in it. * **rattler_solve**: a backend
 agnostic library to solve the package satisfiability problem. *
 **rattler_virtual_packages**: a crate to detect system capabilities. *
+**rattler_index**: create local conda channels from local packages. *
 **rattler**: functionality to create complete environments from scratch using
-the crates above. * **rattler-bin**: an example of a package manager using all
-the crates above (see: [showcase](#showcase)) You can find these crates in the
-`crates` folder. ## What is conda & conda-forge? The conda ecosystem provides
-**cross-platform**, **binary** packages that you can use with **any programming
-language**. `conda` is an open-source package management system and environment
-management system that can install and manage multiple versions of software
-packages and their dependencies. `conda` is written in Python. The aim of
-Rattler is to provide all functionality required to work with the conda
-ecosystem from Rust. Rattler is not a reimplementation of `conda`. `conda` is a
-package management tool. Rattler is a _library_ to work with the conda
-ecosystem from different languages and applications. For example, it powers the
-backend of https://prefix.dev. `conda-forge` is a community-driven effort to
-bring new and existing software into the conda ecosystem. It provides _tens-of-
-thousands of up-to-date_ packages that are maintained by a community of
-contributors. For an overview of available packages see https://prefix.dev.
+the crates above. * **rattler-lock**: a library to create and parse lockfiles
+for conda environments. * **rattler-networking**: common functionality for
+networking, like authentication, mirroring and more. * **rattler-bin**: an
+example of a package manager using all the crates above (see: [showcase]
+(#showcase)) You can find these crates in the `crates` folder. Additionally, we
+provide Python bindings for most of the functionalities provided by the above
+crates. A python package `py-rattler` is available on [conda-forge](https://
+prefix.dev/channels/conda-forge/packages/py-rattler) and [PyPI](https://
+pypi.org/project/py-rattler/). Documatation for the python bindings can be
+found [here](https://mamba-org.github.io/rattler/py-rattler). ## What is conda
+& conda-forge? The conda ecosystem provides **cross-platform**, **binary**
+packages that you can use with **any programming language**. `conda` is an
+open-source package management system and environment management system that
+can install and manage multiple versions of software packages and their
+dependencies. `conda` is written in Python. The aim of Rattler is to provide
+all functionality required to work with the conda ecosystem from Rust. Rattler
+is not a reimplementation of `conda`. `conda` is a package management tool.
+Rattler is a _library_ to work with the conda ecosystem from different
+languages and applications. For example, it powers the backend of https://
+prefix.dev. `conda-forge` is a community-driven effort to bring new and
+existing software into the conda ecosystem. It provides _tens-of-thousands of
+up-to-date_ packages that are maintained by a community of contributors. For an
+overview of available packages see https://prefix.dev.
```

### Comparing `py_rattler-0.5.0/docs/index.md` & `py_rattler-0.6.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/pixi.lock` & `py_rattler-0.6.0/pixi.lock`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,43 @@
   build:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h9eb54c0_6.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/kernel-headers_linux-64-2.6.32-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-hceb6213_106.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h6ddb7a1_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/maturin-1.2.3-py38hcdda232_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/patchelf-0.17.2-h58526e2_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.8.19-hd12c33a_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/rust-1.77.2-h70c747d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-unknown-linux-gnu-1.77.2-h2c6d0dc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
@@ -41,14 +49,16 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/maturin-1.2.3-py38h196e9ca_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.8.19-h5ba8234_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/rust-1.77.2-h7e1429e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-apple-darwin-1.77.2-h38e4360_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
@@ -59,14 +69,16 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/maturin-1.2.3-py38h92a0862_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.8.19-h2469fbe_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/rust-1.77.2-h4ff7c5d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-aarch64-apple-darwin-1.77.2-hf6ec828_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
@@ -81,14 +93,16 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/maturin-1.2.3-py38hf90c7e5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.8.19-h4de0772_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-4_cp38.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/rust-1.77.2-hf8d6059_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-pc-windows-msvc-1.77.2-h17fc481_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
@@ -103,22 +117,22 @@
     - url: https://conda.anaconda.org/conda-forge/
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/astunparse-1.6.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py38h17151c0_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py312h30efb56_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/cairo-1.18.0-h3faef2a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairocffi-1.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairosvg-2.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py38h6d47a40_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/cssselect2-0.2.1-pyh9f0ad1d_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/expat-2.6.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -153,54 +167,56 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libtiff-4.6.0-h1dd3fc0_3.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libwebp-base-1.4.0-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcb-1.15-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py38h01eb140_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mdx_truly_sane_lists-1.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.5.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-autorefs-1.0.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.18-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.20-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-extensions-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-0.24.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-python-1.9.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openjpeg-2.5.2-h488ebb8_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/paginate-0.5.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py38h9e66945_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py312hdcec9eb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pixman-0.43.2-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pthread-stubs-0.4-h36c2ea0_1001.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.8.19-hd12c33a_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-4_cp38.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py38h01eb140_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/regex-2024.4.16-py38h01eb140_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/regex-2024.4.28-py312h9a8786e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py38h578d9bd_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-kbproto-1.0.7-h7f98852_1002.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-libice-1.1.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-libsm-1.2.4-h7391055_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-libx11-1.8.9-h8ee46fc_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-libxau-1.0.11-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xorg-libxdmcp-1.1.3-h7f98852_0.tar.bz2
@@ -213,22 +229,22 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/astunparse-1.6.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py38h940360d_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py312heafc425_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/cairo-1.18.0-h99e66fa_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairocffi-1.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairosvg-2.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py38h082e395_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py312h38bf5a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/cssselect2-0.2.1-pyh9f0ad1d_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/expat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -258,73 +274,75 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libpng-1.6.43-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libtiff-4.6.0-h129831d_3.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libwebp-base-1.4.0-h10d778d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libxcb-1.15-hb7f2c08_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py38hae2e43d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py312h41838bb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mdx_truly_sane_lists-1.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.5.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-autorefs-1.0.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.18-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.20-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-extensions-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-0.24.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-python-1.9.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openjpeg-2.5.2-h7310d3a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/paginate-0.5.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pcre2-10.43-h0ad2156_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py38h85abd47_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py312h0c923fa_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pixman-0.43.4-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pthread-stubs-0.4-hc929b4f_1001.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.8.19-h5ba8234_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-4_cp38.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py38hcafd530_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/regex-2024.4.16-py38hae2e43d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/regex-2024.4.28-py312h5fa3f64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py38h2bea1e5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xorg-libxau-1.0.11-h0dc2134_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xorg-libxdmcp-1.1.3-h35c211d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/astunparse-1.6.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py38he333c0f_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py312h9f69965_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cairo-1.18.0-hd1e100b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairocffi-1.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairosvg-2.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py38h73f40f7_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py312h8e38eb3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/cssselect2-0.2.1-pyh9f0ad1d_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/expat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -354,73 +372,75 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libpng-1.6.43-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libtiff-4.6.0-h07db509_3.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libwebp-base-1.4.0-h93a5062_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libxcb-1.15-hf346824_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py38h336bac9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py312he37b823_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mdx_truly_sane_lists-1.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.5.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-autorefs-1.0.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.18-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.20-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-extensions-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-0.24.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-python-1.9.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openjpeg-2.5.2-h9f1df11_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/paginate-0.5.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pcre2-10.43-h26f9a81_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pillow-10.3.0-py38h9ef4633_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pillow-10.3.0-py312h8a801b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pixman-0.43.4-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pthread-stubs-0.4-h27ca646_1001.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.8.19-h2469fbe_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.8-4_cp38.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py38hb192615_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/regex-2024.4.16-py38h336bac9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/regex-2024.4.28-py312h4a164c9_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py38h336bac9_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xorg-libxau-1.0.11-hb547adb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xorg-libxdmcp-1.1.3-h27ca646_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/noarch/astunparse-1.6.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/babel-2.14.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py38hd3f51b4_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py312h53d5487_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/cairo-1.18.0-h1fef639_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairocffi-1.6.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cairosvg-2.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py38h91455d4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/cssselect2-0.2.1-pyh9f0ad1d_1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/expat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/font-ttf-dejavu-sans-mono-2.37-hab24e00_0.tar.bz2
@@ -454,57 +474,59 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-3.6-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py38h91455d4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mdx_truly_sane_lists-1.3-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.5.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-autorefs-1.0.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.18-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.20-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-extensions-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-0.24.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocstrings-python-1.9.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/openjpeg-2.5.2-h3d672ee_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/paginate-0.5.6-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pcre2-10.43-h17e33f8_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py38h894f861_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py312h6f6a607_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pixman-0.43.4-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pthread-stubs-0.4-hcd874cb_1001.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.17.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pymdown-extensions-10.8-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.8.19-h4de0772_0_cpython.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-4_cp38.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py38h91455d4_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/regex-2024.4.16-py38h91455d4_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/regex-2024.4.28-py312h4389bb4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py38haa244fe_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py312h2e8e312_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/xorg-libxau-1.0.11-hcd874cb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xorg-libxdmcp-1.1.3-hcd874cb_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/yaml-0.2.5-h8ffe710_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
@@ -513,131 +535,168 @@
   test:
     channels:
     - url: https://conda.anaconda.org/conda-forge/
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h9eb54c0_6.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/kernel-headers_linux-64-2.6.32-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h55db66e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-hceb6213_106.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-hc881cc4_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h6ddb7a1_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.2.0-h95c4c6d_6.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/maturin-1.2.3-py38hcdda232_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/mypy-1.5.1-py38h01eb140_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4.20240210-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.2.1-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/patchelf-0.17.2-h58526e2_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py38h01eb140_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xprocess-0.23.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.8.19-hd12c33a_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.3.7-py38h18b4745_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/rust-1.77.2-h70c747d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-unknown-linux-gnu-1.77.2-h2c6d0dc_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libcxx-16.0.6-hd57cbcb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/maturin-1.2.3-py38h196e9ca_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/mypy-1.5.1-py38hcafd530_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.4.20240210-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.2.1-hd75f5a5_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py38hae2e43d_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xprocess-0.23.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.8.19-h5ba8234_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.3.7-py38h1916ca8_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/rust-1.77.2-h7e1429e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-apple-darwin-1.77.2-h38e4360_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libcxx-16.0.6-h4653b0c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/maturin-1.2.3-py38h92a0862_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/mypy-1.5.1-py38hb192615_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.4.20240210-h078ce10_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.2.1-h0d3ecfb_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py38h336bac9_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xprocess-0.23.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.8.19-h2469fbe_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.3.7-py38h5477e86_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/rust-1.77.2-h4ff7c5d_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-aarch64-apple-darwin-1.77.2-hf6ec828_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.2.0-pyhd8ed1ab_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/iniconfig-2.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libgfortran-5.3.0-6.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-5.3.0-7.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gcc-libs-core-5.3.0-7.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-gmp-6.1.0-2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/m2w64-libwinpthread-git-5.0.0.4634.697f757-2.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/win-64/maturin-1.2.3-py38hf90c7e5_1.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/msys2-conda-epoch-20160418-1.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/mypy-1.5.1-py38h91455d4_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mypy_extensions-1.0.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.2.1-hcfcfb64_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py38h91455d4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-7.4.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-asyncio-0.21.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xprocess-0.23.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.8.19-h4de0772_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.8-4_cp38.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.3.7-py38h5e48be7_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/rust-1.77.2-hf8d6059_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-pc-windows-msvc-1.77.2-h17fc481_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-hcf57466_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33130-h82b7239_18.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33130-hcb4865c_18.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/wheel-0.43.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
 packages:
 - kind: conda
   name: _libgcc_mutex
   version: '0.1'
   build: conda_forge
   subdir: linux-64
@@ -694,93 +753,108 @@
   - pytz
   - setuptools
   license: BSD-3-Clause
   license_family: BSD
   size: 7609750
   timestamp: 1702422720584
 - kind: conda
+  name: binutils_impl_linux-64
+  version: '2.40'
+  build: ha885e6a_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/binutils_impl_linux-64-2.40-ha885e6a_0.conda
+  sha256: 180b268f207d1481beb9de5c173751d14c429a7226fa9a85941e4a54cf6be1b4
+  md5: 800a4c872b5bc06fa83888d112fe6c4f
+  depends:
+  - ld_impl_linux-64 2.40 h55db66e_0
+  - sysroot_linux-64
+  license: GPL-3.0-only
+  license_family: GPL
+  size: 5797310
+  timestamp: 1713651250214
+- kind: conda
   name: brotli-python
   version: 1.1.0
-  build: py38h17151c0_1
+  build: py312h30efb56_1
   build_number: 1
   subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py38h17151c0_1.conda
-  sha256: f932ae77f10885dd991b0e1f56f6effea9f19b169e8606dab0bdafd0e44db3c9
-  md5: 7a5a699c8992fc51ef25e980f4502c2a
+  url: https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py312h30efb56_1.conda
+  sha256: b68706698b6ac0d31196a8bcb061f0d1f35264bcd967ea45e03e108149a74c6f
+  md5: 45801a89533d3336a365284d93298e36
   depends:
   - libgcc-ng >=12
   - libstdcxx-ng >=12
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   constrains:
   - libbrotlicommon 1.1.0 hd590300_1
   license: MIT
   license_family: MIT
-  size: 350830
-  timestamp: 1695990250755
+  size: 350604
+  timestamp: 1695990206327
 - kind: conda
   name: brotli-python
   version: 1.1.0
-  build: py38h940360d_1
+  build: py312h53d5487_1
   build_number: 1
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py38h940360d_1.conda
-  sha256: 0a088bff62ddd2e505bdc80cc16da009c134b9ccfa6352b0cfe9d4eeed27d8c2
-  md5: ad8d4ae4e8351a2fc0fe92f13bd266d8
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py312h53d5487_1.conda
+  sha256: 769e276ecdebf86f097786cbde1ebd11e018cd6cd838800995954fe6360e0797
+  md5: d01a6667b99f0e8ad4097af66c938e62
   depends:
-  - libcxx >=15.0.7
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   constrains:
-  - libbrotlicommon 1.1.0 h0dc2134_1
+  - libbrotlicommon 1.1.0 hcfcfb64_1
   license: MIT
   license_family: MIT
-  size: 366343
-  timestamp: 1695990788245
+  size: 322514
+  timestamp: 1695991054894
 - kind: conda
   name: brotli-python
   version: 1.1.0
-  build: py38hd3f51b4_1
+  build: py312h9f69965_1
   build_number: 1
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py38hd3f51b4_1.conda
-  sha256: a292d6b3118ef284cc03a99a6efe5e08ca3a6d0e37eff78eb8d87cfca3830d7b
-  md5: 72708ea626a2530148ea49eb743576f4
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py312h9f69965_1.conda
+  sha256: 3418b1738243abba99e931c017b952771eeaa1f353c07f7d45b55e83bb74fcb3
+  md5: 1bc01b9ffdf42beb1a9fe4e9222e0567
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  - libcxx >=15.0.7
+  - python >=3.12.0rc3,<3.13.0a0
+  - python >=3.12.0rc3,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   constrains:
-  - libbrotlicommon 1.1.0 hcfcfb64_1
+  - libbrotlicommon 1.1.0 hb547adb_1
   license: MIT
   license_family: MIT
-  size: 321650
-  timestamp: 1695990817828
+  size: 343435
+  timestamp: 1695990731924
 - kind: conda
   name: brotli-python
   version: 1.1.0
-  build: py38he333c0f_1
+  build: py312heafc425_1
   build_number: 1
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py38he333c0f_1.conda
-  sha256: 3fd1e0a4b7ea1b20f69bbc2d74c798f3eebd775ccbcdee170f68b1871f8bbb74
-  md5: 29160c74d5977b1c5ecd654b00d576f0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py312heafc425_1.conda
+  sha256: fc55988f9bc05a938ea4b8c20d6545bed6e9c6c10aa5147695f981136ca894c1
+  md5: a288b88f06b8bfe0dedaf5c4b6ac6b7a
   depends:
   - libcxx >=15.0.7
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   constrains:
-  - libbrotlicommon 1.1.0 hb547adb_1
+  - libbrotlicommon 1.1.0 h0dc2134_1
   license: MIT
   license_family: MIT
-  size: 343036
-  timestamp: 1695990970956
+  size: 366883
+  timestamp: 1695990710194
 - kind: conda
   name: bzip2
   version: 1.0.8
   build: h10d778d_5
   build_number: 5
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
@@ -1028,83 +1102,83 @@
   - python >=3.7
   license: ISC
   size: 160559
   timestamp: 1707022289175
 - kind: conda
   name: cffi
   version: 1.16.0
-  build: py38h082e395_0
+  build: py312h38bf5a0_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py38h082e395_0.conda
-  sha256: c79e5074c663670f75258f6fce8ebd0e65042bd22ecbb4979294c57ff4fa8fc5
-  md5: 046fe2a8edb11f1b8a7d3bd8e2fd1de7
+  url: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py312h38bf5a0_0.conda
+  sha256: 8b856583b56fc30f064a7cb286f85e4b5725f2bd4fda8ba0c4e94bffe258741e
+  md5: a45759c013ab20b9017ef9539d234dd7
   depends:
   - libffi >=3.4,<4.0a0
   - pycparser
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
-  size: 228367
-  timestamp: 1696002058694
+  size: 282370
+  timestamp: 1696002004433
 - kind: conda
   name: cffi
   version: 1.16.0
-  build: py38h6d47a40_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py38h6d47a40_0.conda
-  sha256: ec0a62d4836d3ec2321d07cffa5aeef37c6818c6cce6383dc6be7205d09551b3
-  md5: fc010dfb8ce6540d289436fbba499ee7
+  build: py312h8e38eb3_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py312h8e38eb3_0.conda
+  sha256: 1544403cb1a5ca2aeabf0dac86d9ce6066d6fb4363493643b33ffd1b78038d18
+  md5: 960ecbd65860d3b1de5e30373e1bffb1
   depends:
   - libffi >=3.4,<4.0a0
-  - libgcc-ng >=12
   - pycparser
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python >=3.12.0rc3,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
-  size: 239127
-  timestamp: 1696001978654
+  size: 284245
+  timestamp: 1696002181644
 - kind: conda
   name: cffi
   version: 1.16.0
-  build: py38h73f40f7_0
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py38h73f40f7_0.conda
-  sha256: 375e0be4068f4b00facfa569aa26c92ed87858f45be875f2c4bf90f33733f4de
-  md5: 02911ce6163d7a3e8fe9d9398fb9986d
+  build: py312he70551f_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py312he70551f_0.conda
+  sha256: dd39e594f5c6bca52dfed343de2af9326a99700ce2ba3404bd89706926fc0137
+  md5: 5a51096925d52332c62bfd8904899055
   depends:
-  - libffi >=3.4,<4.0a0
   - pycparser
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
-  size: 230759
-  timestamp: 1696002169830
+  size: 287805
+  timestamp: 1696002408940
 - kind: conda
   name: cffi
   version: 1.16.0
-  build: py38h91455d4_0
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py38h91455d4_0.conda
-  sha256: 0704377274cfe0b3a5c308facecdeaaf2207303ee847842a4bbd3f70b7331ddc
-  md5: e9b2ac14b9c3d3eaeb2f69745e021e49
+  build: py312hf06ca03_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda
+  sha256: 5a36e2c254603c367d26378fa3a205bd92263e30acf195f488749562b4c44251
+  md5: 56b0ca764ce23cc54f3f7e2a7b970f6d
   depends:
+  - libffi >=3.4,<4.0a0
+  - libgcc-ng >=12
   - pycparser
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   license: MIT
   license_family: MIT
-  size: 234905
-  timestamp: 1696002150251
+  size: 294523
+  timestamp: 1696001868949
 - kind: conda
   name: charset-normalizer
   version: 3.3.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.3.2-pyhd8ed1ab_0.conda
@@ -1485,14 +1559,35 @@
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: GPL-2.0-only OR FTL
   size: 510306
   timestamp: 1694616398888
 - kind: conda
+  name: gcc_impl_linux-64
+  version: 13.2.0
+  build: h9eb54c0_6
+  build_number: 6
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/gcc_impl_linux-64-13.2.0-h9eb54c0_6.conda
+  sha256: 67d16151d316f04ea2779ff3a4f5fcf4a5454e89bc21dabc1a4f7c08cf5ea821
+  md5: 36ca2a36806ab26c2daf20d5b62280d7
+  depends:
+  - binutils_impl_linux-64 >=2.40
+  - libgcc-devel_linux-64 13.2.0 hceb6213_106
+  - libgcc-ng >=13.2.0
+  - libgomp >=13.2.0
+  - libsanitizer 13.2.0 h6ddb7a1_6
+  - libstdcxx-ng >=13.2.0
+  - sysroot_linux-64
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
+  size: 53360656
+  timestamp: 1714581875812
+- kind: conda
   name: ghp-import
   version: 2.1.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/ghp-import-2.1.0-pyhd8ed1ab_0.tar.bz2
   sha256: 097d9b4c946b195800bc68f68393370049238509b08ef828c06fbf481bbc139c
@@ -1634,14 +1729,30 @@
   - markupsafe >=2.0
   - python >=3.7
   license: BSD-3-Clause
   license_family: BSD
   size: 111589
   timestamp: 1704967140287
 - kind: conda
+  name: kernel-headers_linux-64
+  version: 2.6.32
+  build: he073ed8_17
+  build_number: 17
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/kernel-headers_linux-64-2.6.32-he073ed8_17.conda
+  sha256: fb39d64b48f3d9d1acc3df208911a41f25b6a00bd54935d5973b4739a9edd5b6
+  md5: d731b543793afc0433c4fd593e693fce
+  constrains:
+  - sysroot_linux-64 ==2.12
+  license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
+  license_family: GPL
+  size: 710627
+  timestamp: 1708000830116
+- kind: conda
   name: lcms2
   version: '2.16'
   build: h67d730c_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/lcms2-2.16-h67d730c_0.conda
   sha256: f9fd9e80e46358a57d9bb97b1e37a03da4022143b019aa3c4476d8a7795de290
   md5: d3592435917b62a8becff3a60db674f6
@@ -1963,14 +2074,28 @@
   - vc >=14.1,<15.0a0
   - vs2015_runtime >=14.16.27012
   license: MIT
   license_family: MIT
   size: 42063
   timestamp: 1636489106777
 - kind: conda
+  name: libgcc-devel_linux-64
+  version: 13.2.0
+  build: hceb6213_106
+  build_number: 106
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/libgcc-devel_linux-64-13.2.0-hceb6213_106.conda
+  sha256: f5af7a346ba0a2c322028a7fa8ba99f5094911439d5aab2c6bc42a4e9022bc68
+  md5: b85d6b583f498b4ddc9150aefb492f7f
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
+  size: 2575829
+  timestamp: 1714581666472
+- kind: conda
   name: libgcc-ng
   version: 13.2.0
   build: hc881cc4_6
   build_number: 6
   subdir: linux-64
   url: https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.2.0-hc881cc4_6.conda
   sha256: 836a0057525f1414de43642d357d0ab21ac7f85e24800b010dbc17d132e6efec
@@ -2307,14 +2432,29 @@
   md5: 65dcddb15965c9de2c0365cb14910532
   depends:
   - libzlib >=1.2.13,<1.3.0a0
   license: zlib-acknowledgement
   size: 268524
   timestamp: 1708780496420
 - kind: conda
+  name: libsanitizer
+  version: 13.2.0
+  build: h6ddb7a1_6
+  build_number: 6
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/libsanitizer-13.2.0-h6ddb7a1_6.conda
+  sha256: 06f3695963ee86badbfe006f13fa9fe600539acb77f19c5c972d498a14e9b53d
+  md5: 95b48df99634d9e706a0bf7e30ae91c8
+  depends:
+  - libgcc-ng >=13.2.0
+  license: GPL-3.0-only WITH GCC-exception-3.1
+  license_family: GPL
+  size: 4188343
+  timestamp: 1714581787957
+- kind: conda
   name: libsqlite
   version: 3.45.3
   build: h091b4b1_0
   subdir: osx-arm64
   url: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
   sha256: 4337f466eb55bbdc74e168b52ec8c38f598e3664244ec7a2536009036e2066cc
   md5: c8c1186c7f3351f6ffddb97b1f54fc58
@@ -2779,84 +2919,84 @@
   license: BSD-3-Clause
   license_family: BSD
   size: 78331
   timestamp: 1710435316163
 - kind: conda
   name: markupsafe
   version: 2.1.5
-  build: py38h01eb140_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py38h01eb140_0.conda
-  sha256: 384a193d11c89463533e6fc5d94a6c67c16c598b32747a8f86f9ad227f0aed17
-  md5: aeeb09febb02542e020c3ba7084ead01
+  build: py312h41838bb_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py312h41838bb_0.conda
+  sha256: 8dc8f31f78d00713300da000b6ebaa1943a17c112f267de310d5c3d82950079c
+  md5: c4a9c25c09cef3901789ca818d9beb10
   depends:
-  - libgcc-ng >=12
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   constrains:
   - jinja2 >=3.0.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 24274
-  timestamp: 1706900087252
+  size: 25742
+  timestamp: 1706900456837
 - kind: conda
   name: markupsafe
   version: 2.1.5
-  build: py38h336bac9_0
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py38h336bac9_0.conda
-  sha256: f1b1b405c5246c499d66658e754e920529866826b247111cd481e15d0571f702
-  md5: 76e1802508a91e5970f42f6558f5064e
+  build: py312h98912ed_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda
+  sha256: 273d8efd6c089c534ccbede566394c0ac1e265bfe5d89fe76e80332f3d75a636
+  md5: 6ff0b9582da2d4a74a1f9ae1f9ce2af6
   depends:
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - libgcc-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   constrains:
   - jinja2 >=3.0.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 23719
-  timestamp: 1706900313162
+  size: 26685
+  timestamp: 1706900070330
 - kind: conda
   name: markupsafe
   version: 2.1.5
-  build: py38h91455d4_0
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py38h91455d4_0.conda
-  sha256: a0753407d33dbeebf3ee3118cc4bd3559af81e3de497b15f01a52b2702314c73
-  md5: 0b3eb104f5c37ba2e7ec675b6a8ea453
-  depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  build: py312he37b823_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py312he37b823_0.conda
+  sha256: 61480b725490f68856dd14e646f51ffc34f77f2c985bd33e3b77c04b2856d97d
+  md5: ba3a8f8cf8bbdb81394275b1e1d271da
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   constrains:
   - jinja2 >=3.0.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 26598
-  timestamp: 1706900643364
+  size: 26382
+  timestamp: 1706900495057
 - kind: conda
   name: markupsafe
   version: 2.1.5
-  build: py38hae2e43d_0
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py38hae2e43d_0.conda
-  sha256: ef6eaa455d99e40df64131d23f4b52bc3601f95a48f255cb9917f2d4eb760a36
-  md5: 5107dae4aa6cbcb0cb73718cdd951c29
+  build: py312he70551f_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda
+  sha256: f8690a3c87e2e96cebd434a829bb95cac43afe6c439530b336dc3452fe4ce4af
+  md5: 4950a739b19edaac1ed29ca9474e49ac
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   constrains:
   - jinja2 >=3.0.0
   license: BSD-3-Clause
   license_family: BSD
-  size: 23167
-  timestamp: 1706900242727
+  size: 29060
+  timestamp: 1706900374745
 - kind: conda
   name: maturin
   version: 1.2.3
   build: py38h196e9ca_1
   build_number: 1
   subdir: osx-64
   url: https://conda.anaconda.org/conda-forge/osx-64/maturin-1.2.3-py38h196e9ca_1.conda
@@ -2925,14 +3065,30 @@
   - python_abi 3.8.* *_cp38
   - tomli >=1.1.0
   license: MIT
   license_family: MIT
   size: 4675089
   timestamp: 1695301899264
 - kind: conda
+  name: mdx_truly_sane_lists
+  version: '1.3'
+  build: pyhd8ed1ab_0
+  subdir: noarch
+  noarch: python
+  url: https://conda.anaconda.org/conda-forge/noarch/mdx_truly_sane_lists-1.3-pyhd8ed1ab_0.tar.bz2
+  sha256: 2a00cd521d63ae8a20b52de590ff2f1f63ea4ba569f7e66ae629330f0e69cf43
+  md5: 3c4c4f9b8ae968cb20823351d81d12b5
+  depends:
+  - markdown >=2.6
+  - python >=3.6
+  license: MIT
+  license_family: MIT
+  size: 10480
+  timestamp: 1658251565870
+- kind: conda
   name: mergedeep
   version: 1.3.4
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
   sha256: 41ad8c16876820981adfc6e17a62935c950214bd9a9bb092e6aaefdc89a33f0b
@@ -2991,21 +3147,21 @@
   - pymdown-extensions
   - python >=3.8,<4.0
   license: ISC
   size: 21614
   timestamp: 1709500020733
 - kind: conda
   name: mkdocs-material
-  version: 9.5.18
+  version: 9.5.20
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.18-pyhd8ed1ab_0.conda
-  sha256: 47f3d939ade648d8288705f1dd95c9a1f80b10772b1fdbd8a81a6fe92689c395
-  md5: d5d4bb5f8a501e9ce4bc73a5baa3553b
+  url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-9.5.20-pyhd8ed1ab_0.conda
+  sha256: 38f61b17fa334d20a60c5a37eefa836e05c4e4b0a3cff763591c941be90de348
+  md5: 5f09758905bfaf7d5c748196f63aba35
   depends:
   - babel ~=2.10
   - colorama ~=0.4
   - jinja2 ~=3.0
   - markdown ~=3.2
   - mkdocs ~=1.5,>=1.5.3
   - mkdocs-material-extensions ~=1.3
@@ -3013,16 +3169,16 @@
   - pygments ~=2.16
   - pymdown-extensions ~=10.2
   - python >=3.8
   - regex >=2022.4
   - requests ~=2.26
   license: MIT
   license_family: MIT
-  size: 5002352
-  timestamp: 1713278417020
+  size: 5007228
+  timestamp: 1714393800216
 - kind: conda
   name: mkdocs-material-extensions
   version: 1.3.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/mkdocs-material-extensions-1.3.1-pyhd8ed1ab_0.conda
@@ -3490,108 +3646,108 @@
   license: BSD-3-Clause
   license_family: BSD
   size: 950847
   timestamp: 1708118050286
 - kind: conda
   name: pillow
   version: 10.3.0
-  build: py38h85abd47_0
+  build: py312h0c923fa_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py38h85abd47_0.conda
-  sha256: b3f85b5c20ab9d2614e81816adb0a88769ae5b3392e02b802d470b3e4805e0bf
-  md5: 785f9ef8a330dcf8d6619c127b13f21d
+  url: https://conda.anaconda.org/conda-forge/osx-64/pillow-10.3.0-py312h0c923fa_0.conda
+  sha256: 3e33ce8ba364948eeeeb06da435059b1ed0e6cfb2b1195931b76e190ee671310
+  md5: 6f0591ae972e9b815739da3392fbb3c3
   depends:
   - freetype >=2.12.1,<3.0a0
   - lcms2 >=2.16,<3.0a0
   - libjpeg-turbo >=3.0.0,<4.0a0
   - libtiff >=4.6.0,<4.7.0a0
   - libwebp-base >=1.3.2,<2.0a0
   - libxcb >=1.15,<1.16.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openjpeg >=2.5.2,<3.0a0
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - tk >=8.6.13,<8.7.0a0
   license: HPND
-  size: 41189766
-  timestamp: 1712154782357
+  size: 42531277
+  timestamp: 1712154782302
 - kind: conda
   name: pillow
   version: 10.3.0
-  build: py38h894f861_0
+  build: py312h6f6a607_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py38h894f861_0.conda
-  sha256: d661083709fd0e2262388adeae52a0c8591c762a54582a6fa0941158990ecd68
-  md5: 9b2eb85eed298007db9c714981ab87fe
+  url: https://conda.anaconda.org/conda-forge/win-64/pillow-10.3.0-py312h6f6a607_0.conda
+  sha256: f1621c28346609886ccce14b6ae0069b5cb34925ace73e05a8c06770d2ad7a19
+  md5: 8d5f5f1fa36200f1ef987299a47de403
   depends:
   - freetype >=2.12.1,<3.0a0
   - lcms2 >=2.16,<3.0a0
   - libjpeg-turbo >=3.0.0,<4.0a0
   - libtiff >=4.6.0,<4.7.0a0
   - libwebp-base >=1.3.2,<2.0a0
   - libxcb >=1.15,<1.16.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openjpeg >=2.5.2,<3.0a0
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - tk >=8.6.13,<8.7.0a0
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: HPND
-  size: 40924506
-  timestamp: 1712155038917
+  size: 42439434
+  timestamp: 1712155248737
 - kind: conda
   name: pillow
   version: 10.3.0
-  build: py38h9e66945_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py38h9e66945_0.conda
-  sha256: b44195d022fa378808397b29406447f0a9e0e4486d03a8a97f014e8f78b091a5
-  md5: 06a7c758cf349a5bf24989f179bb504e
+  build: py312h8a801b1_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pillow-10.3.0-py312h8a801b1_0.conda
+  sha256: 26bc04e81ae5fce70e4b72478dadea29d32b693eed17640be7721108a3c9af0d
+  md5: 1d42544faaed27dce36268912b8dfedf
   depends:
   - freetype >=2.12.1,<3.0a0
   - lcms2 >=2.16,<3.0a0
-  - libgcc-ng >=12
   - libjpeg-turbo >=3.0.0,<4.0a0
   - libtiff >=4.6.0,<4.7.0a0
   - libwebp-base >=1.3.2,<2.0a0
   - libxcb >=1.15,<1.16.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openjpeg >=2.5.2,<3.0a0
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   - tk >=8.6.13,<8.7.0a0
   license: HPND
-  size: 42314111
-  timestamp: 1712154579877
+  size: 42729895
+  timestamp: 1712155044162
 - kind: conda
   name: pillow
   version: 10.3.0
-  build: py38h9ef4633_0
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pillow-10.3.0-py38h9ef4633_0.conda
-  sha256: 1d32b60ffb4b851e839e7d0ee5930b9d2a4c6158ee149b400ab9cf55f41c7a3c
-  md5: c43a7c5715ba3697fb8e9fc5da1a2d96
+  build: py312hdcec9eb_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pillow-10.3.0-py312hdcec9eb_0.conda
+  sha256: a7fdcc1e56b66d95622bad073cc8d347cc180988040419754abb2a4ed7b29471
+  md5: 425bb325f970e57a047ac57c4586489d
   depends:
   - freetype >=2.12.1,<3.0a0
   - lcms2 >=2.16,<3.0a0
+  - libgcc-ng >=12
   - libjpeg-turbo >=3.0.0,<4.0a0
   - libtiff >=4.6.0,<4.7.0a0
   - libwebp-base >=1.3.2,<2.0a0
   - libxcb >=1.15,<1.16.0a0
   - libzlib >=1.2.13,<1.3.0a0
   - openjpeg >=2.5.2,<3.0a0
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - tk >=8.6.13,<8.7.0a0
   license: HPND
-  size: 41460984
-  timestamp: 1712155043935
+  size: 41991755
+  timestamp: 1712154634705
 - kind: conda
   name: pip
   version: 23.2.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pip-23.2.1-pyhd8ed1ab_0.conda
@@ -4048,14 +4204,122 @@
   - xz >=5.2.6,<6.0a0
   constrains:
   - python_abi 3.8.* *_cp38
   license: Python-2.0
   size: 22357104
   timestamp: 1710939954552
 - kind: conda
+  name: python
+  version: 3.12.3
+  build: h1411813_0_cpython
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
+  sha256: 3b327ffc152a245011011d1d730781577a8274fde1cf6243f073749ead8f1c2a
+  md5: df1448ec6cbf8eceb03d29003cf72ae6
+  depends:
+  - __osx >=10.9
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 14557341
+  timestamp: 1713208068012
+- kind: conda
+  name: python
+  version: 3.12.3
+  build: h2628c8c_0_cpython
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
+  sha256: 1a95494abe572a8819c933f978df89f00bde72ea9432d46a70632599e8029ea4
+  md5: f07c8c5dd98767f9a652de5d039b284e
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - openssl >=3.2.1,<4.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 16179248
+  timestamp: 1713205644673
+- kind: conda
+  name: python
+  version: 3.12.3
+  build: h4a7b5fc_0_cpython
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
+  sha256: c761fb3713ea66bce3889b33b6f400afb2dd192d1fc2686446e9d8166cfcec6b
+  md5: 8643ab37bece6ae8f112464068d9df9c
+  depends:
+  - __osx >=11.0
+  - bzip2 >=1.0.8,<2.0a0
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 13207557
+  timestamp: 1713206576646
+- kind: conda
+  name: python
+  version: 3.12.3
+  build: hab00c5b_0_cpython
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
+  sha256: f9865bcbff69f15fd89a33a2da12ad616e98d65ce7c83c644b92e66e5016b227
+  md5: 2540b74d304f71d3e89c81209db4db84
+  depends:
+  - bzip2 >=1.0.8,<2.0a0
+  - ld_impl_linux-64 >=2.36.1
+  - libexpat >=2.6.2,<3.0a0
+  - libffi >=3.4,<4.0a0
+  - libgcc-ng >=12
+  - libnsl >=2.0.1,<2.1.0a0
+  - libsqlite >=3.45.2,<4.0a0
+  - libuuid >=2.38.1,<3.0a0
+  - libxcrypt >=4.4.36
+  - libzlib >=1.2.13,<1.3.0a0
+  - ncurses >=6.4.20240210,<7.0a0
+  - openssl >=3.2.1,<4.0a0
+  - readline >=8.2,<9.0a0
+  - tk >=8.6.13,<8.7.0a0
+  - tzdata
+  - xz >=5.2.6,<6.0a0
+  constrains:
+  - python_abi 3.12.* *_cp312
+  license: Python-2.0
+  size: 31991381
+  timestamp: 1713208036041
+- kind: conda
   name: python-dateutil
   version: 2.9.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
   sha256: f3ceef02ac164a8d3a080d0d32f8e2ebe10dd29e3a685d240e38b3599e146320
@@ -4124,14 +4388,74 @@
   constrains:
   - python 3.8.* *_cpython
   license: BSD-3-Clause
   license_family: BSD
   size: 6751
   timestamp: 1695147671006
 - kind: conda
+  name: python_abi
+  version: '3.12'
+  build: 4_cp312
+  build_number: 4
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
+  sha256: 182a329de10a4165f6e8a3804caf751f918f6ea6176dd4e5abcdae1ed3095bf6
+  md5: dccc2d142812964fcc6abdc97b672dff
+  constrains:
+  - python 3.12.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6385
+  timestamp: 1695147396604
+- kind: conda
+  name: python_abi
+  version: '3.12'
+  build: 4_cp312
+  build_number: 4
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
+  sha256: 82c154d95c1637604671a02a89e72f1382e89a4269265a03506496bd928f6f14
+  md5: 87201ac4314b911b74197e588cca3639
+  constrains:
+  - python 3.12.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6496
+  timestamp: 1695147498447
+- kind: conda
+  name: python_abi
+  version: '3.12'
+  build: 4_cp312
+  build_number: 4
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
+  sha256: db25428e4f24f8693ffa39f3ff6dfbb8fd53bc298764b775b57edab1c697560f
+  md5: bbb3a02c78b2d8219d7213f76d644a2a
+  constrains:
+  - python 3.12.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6508
+  timestamp: 1695147497048
+- kind: conda
+  name: python_abi
+  version: '3.12'
+  build: 4_cp312
+  build_number: 4
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
+  sha256: 488f8519d04b48f59bd6fde21ebe2d7a527718ff28aac86a8b53aa63658bdef6
+  md5: 17f4ccf6be9ded08bd0a376f489ac1a6
+  constrains:
+  - python 3.12.* *_cpython
+  license: BSD-3-Clause
+  license_family: BSD
+  size: 6785
+  timestamp: 1695147430513
+- kind: conda
   name: pytz
   version: '2024.1'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pytz-2024.1-pyhd8ed1ab_0.conda
   sha256: 1a7d6b233f7e6e3bbcbad054c8fd51e690a67b129a899a056a5e45dd9f00cb41
@@ -4141,84 +4465,84 @@
   license: MIT
   license_family: MIT
   size: 188538
   timestamp: 1706886944988
 - kind: conda
   name: pyyaml
   version: 6.0.1
-  build: py38h01eb140_1
+  build: py312h02f2b3b_1
   build_number: 1
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py38h01eb140_1.conda
-  sha256: 7741529957e3b3428af73f003f043c9983ed672c69dc4aafef848b2583c4571b
-  md5: 5f05353ae9a6c37e1b4aebc9f7834d23
-  depends:
-  - libgcc-ng >=12
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
+  sha256: b6b4027b89c17b9bbd8089aec3e44bc29f802a7d5668d5a75b5358d7ed9705ca
+  md5: a0c843e52a1c4422d8657dd76e9eb994
+  depends:
+  - python >=3.12.0rc3,<3.13.0a0
+  - python >=3.12.0rc3,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   - yaml >=0.2.5,<0.3.0a0
   license: MIT
   license_family: MIT
-  size: 182153
-  timestamp: 1695373618370
+  size: 182705
+  timestamp: 1695373895409
 - kind: conda
   name: pyyaml
   version: 6.0.1
-  build: py38h91455d4_1
+  build: py312h104f124_1
   build_number: 1
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py38h91455d4_1.conda
-  sha256: 1cd8fe0f885c7e491b41e55611f546d011db8ac45941202eb2ef1549f6df0507
-  md5: 4d9ea280b4f91fa5b0c0d34f2fce99cb
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
+  sha256: 04aa180782cb675b960c0bf4aad439b4a7a08553c6af74d0b8e5df9a0c7cc4f4
+  md5: 260ed90aaf06061edabd7209638cf03b
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - yaml >=0.2.5,<0.3.0a0
   license: MIT
   license_family: MIT
-  size: 151945
-  timestamp: 1695373981322
+  size: 185636
+  timestamp: 1695373742454
 - kind: conda
   name: pyyaml
   version: 6.0.1
-  build: py38hb192615_1
+  build: py312h98912ed_1
   build_number: 1
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py38hb192615_1.conda
-  sha256: a4bcd94eda8611ade946a52cb52cf60ca6aa4d69915a9c68a9d9b7cbf02e4ac0
-  md5: 72ee6bc5ee0182fb7c5f26461504cbf5
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
+  sha256: 7f347a10a7121b08d79d21cd4f438c07c23479ea0c74dfb89d6dc416f791bb7f
+  md5: e3fd78d8d490af1d84763b9fe3f2e552
   depends:
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - libgcc-ng >=12
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - yaml >=0.2.5,<0.3.0a0
   license: MIT
   license_family: MIT
-  size: 158422
-  timestamp: 1695373866893
+  size: 196583
+  timestamp: 1695373632212
 - kind: conda
   name: pyyaml
   version: 6.0.1
-  build: py38hcafd530_1
+  build: py312he70551f_1
   build_number: 1
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py38hcafd530_1.conda
-  sha256: cd1dceaa9bb8296ddea04cfb5e933bf5ab2b189c566bb55e1a3c9a38efffa82d
-  md5: 17cfcfdd18fa2fe701ff68c9bbcea9a5
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
+  sha256: a72fa8152791b4738432f270e70b3a9a4d583ef059a78aa1c62f4b4ab7b15494
+  md5: f91e0baa89ba21166916624ba7bfb422
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12.0rc3,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   - yaml >=0.2.5,<0.3.0a0
   license: MIT
   license_family: MIT
-  size: 161848
-  timestamp: 1695373748011
+  size: 167932
+  timestamp: 1695374097139
 - kind: conda
   name: pyyaml-env-tag
   version: '0.1'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
@@ -4275,77 +4599,79 @@
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
   size: 255870
   timestamp: 1679532707590
 - kind: conda
   name: regex
-  version: 2024.4.16
-  build: py38h01eb140_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/regex-2024.4.16-py38h01eb140_0.conda
-  sha256: 6be2e931308e4245aefaab5a4658de2353da895f3f4a860f9c672ce021063f7d
-  md5: ab3c16328ee4d9702eb90c56c8228450
+  version: 2024.4.28
+  build: py312h4389bb4_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/regex-2024.4.28-py312h4389bb4_0.conda
+  sha256: b16227dbc411267d9b23ea9bfc9778bbae4a8593b1e84fac71fb1cdf829d1d61
+  md5: fc45482d8e83a3c85acb107385550166
   depends:
-  - libgcc-ng >=12
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   license: Python-2.0
   license_family: PSF
-  size: 346393
-  timestamp: 1713305283145
+  size: 358313
+  timestamp: 1714348290002
 - kind: conda
   name: regex
-  version: 2024.4.16
-  build: py38h336bac9_0
+  version: 2024.4.28
+  build: py312h4a164c9_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/regex-2024.4.16-py38h336bac9_0.conda
-  sha256: c7cd0f88c7ccfa53d85f47881f4d4b100c64301a3e216e1d854739a00f5b52d4
-  md5: 4c1ff46c475f150365b38560c0126928
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/regex-2024.4.28-py312h4a164c9_0.conda
+  sha256: a9cbb9201f987a1449634f70877939795c17fa58c50ff466191194e7ea955af1
+  md5: bb22ba0467f1fd98413d2c1a3df76231
   depends:
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - __osx >=11.0
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   license: Python-2.0
   license_family: PSF
-  size: 307898
-  timestamp: 1713305521381
+  size: 361720
+  timestamp: 1714348060826
 - kind: conda
   name: regex
-  version: 2024.4.16
-  build: py38h91455d4_0
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/regex-2024.4.16-py38h91455d4_0.conda
-  sha256: 8d23a0e3f5c6dd727f62b7f9c47b28df6b305a562bee0dce42053afbe7c0b39a
-  md5: ff05c0626ba6b41b284639d6f23b192a
+  version: 2024.4.28
+  build: py312h5fa3f64_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/regex-2024.4.28-py312h5fa3f64_0.conda
+  sha256: 9b4386d84b0511ad48ea1d208f177a388d2b10c2c8062850ee35f123738ba78e
+  md5: 025920a03909118fc0f208c1dcc62b94
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  - __osx >=10.9
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   license: Python-2.0
   license_family: PSF
-  size: 306076
-  timestamp: 1713305834816
+  size: 366832
+  timestamp: 1714347981911
 - kind: conda
   name: regex
-  version: 2024.4.16
-  build: py38hae2e43d_0
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/regex-2024.4.16-py38hae2e43d_0.conda
-  sha256: f32549036335e1056746c1f501ffe9208de094be6efdf2656c09e3c24bd7517c
-  md5: 7a5e00f13c2862b7e0a53ad92e7dea9b
+  version: 2024.4.28
+  build: py312h9a8786e_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/regex-2024.4.28-py312h9a8786e_0.conda
+  sha256: 3ee80b9a7bc73fe1a68feeb3eebedf19d6cc57f4181e5e7f75a772afb269f221
+  md5: 39fbec9483427256beaec8b6104e52c0
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - libgcc-ng >=12
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   license: Python-2.0
   license_family: PSF
-  size: 312856
-  timestamp: 1713305547739
+  size: 399284
+  timestamp: 1714347894590
 - kind: conda
   name: requests
   version: 2.31.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
@@ -4432,14 +4758,141 @@
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: MIT
   license_family: MIT
   size: 6343187
   timestamp: 1712963346969
 - kind: conda
+  name: rust
+  version: 1.77.2
+  build: h4ff7c5d_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/rust-1.77.2-h4ff7c5d_0.conda
+  sha256: 048ffabbbbd1b5109d59ec15610cf0e489c39b4f6f380953816bcb26dad8da17
+  md5: 4083c1a9d7f5c9591273f578530d6388
+  depends:
+  - rust-std-aarch64-apple-darwin 1.77.2 hf6ec828_0
+  license: MIT
+  license_family: MIT
+  size: 145759919
+  timestamp: 1712743398771
+- kind: conda
+  name: rust
+  version: 1.77.2
+  build: h70c747d_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/rust-1.77.2-h70c747d_0.conda
+  sha256: 3b8cf09335d23c52d6e7150e4cc6d999ed4e2b3dc2307652f20e1a4669ff0846
+  md5: ba764892e80fe0380bb7fa99751b186d
+  depends:
+  - gcc_impl_linux-64
+  - libgcc-ng >=12
+  - libzlib >=1.2.13,<1.3.0a0
+  - rust-std-x86_64-unknown-linux-gnu 1.77.2 h2c6d0dc_0
+  license: MIT
+  license_family: MIT
+  size: 186765686
+  timestamp: 1712741423714
+- kind: conda
+  name: rust
+  version: 1.77.2
+  build: h7e1429e_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/rust-1.77.2-h7e1429e_0.conda
+  sha256: d12cde3691eb50148b49460ac2bff0c0716204099a38d36132762ffb0c6c79fd
+  md5: 13c8a97dd157999cdd23adaac7919047
+  depends:
+  - rust-std-x86_64-apple-darwin 1.77.2 h38e4360_0
+  license: MIT
+  license_family: MIT
+  size: 192493395
+  timestamp: 1712743664947
+- kind: conda
+  name: rust
+  version: 1.77.2
+  build: hf8d6059_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/rust-1.77.2-hf8d6059_0.conda
+  sha256: 978228c14a3d2af2d9d52230443f232d7a22cbbe98d359a306b1a761773d4589
+  md5: ba05fee8761e5bd25ae642a4b77d2ed7
+  depends:
+  - rust-std-x86_64-pc-windows-msvc 1.77.2 h17fc481_0
+  license: MIT
+  license_family: MIT
+  size: 187565499
+  timestamp: 1712743189902
+- kind: conda
+  name: rust-std-aarch64-apple-darwin
+  version: 1.77.2
+  build: hf6ec828_0
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/rust-std-aarch64-apple-darwin-1.77.2-hf6ec828_0.conda
+  sha256: 19b17ddca3896f12a640858b45a7ba5e8495ca07286b622535ca5a4bf8217906
+  md5: 729f181cdeb249ff2da37f434b548633
+  depends:
+  - __unix
+  constrains:
+  - rust >=1.77.2,<1.77.3.0a0
+  license: MIT
+  license_family: MIT
+  size: 30933811
+  timestamp: 1712740743456
+- kind: conda
+  name: rust-std-x86_64-apple-darwin
+  version: 1.77.2
+  build: h38e4360_0
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-apple-darwin-1.77.2-h38e4360_0.conda
+  sha256: 1d0a99136ab0a2b05d9df4d5a7a8d665595c2e72ee1d19fcad0c6f1b402f37d1
+  md5: 67db6d59468a8145fb076d75d156b69c
+  depends:
+  - __unix
+  constrains:
+  - rust >=1.77.2,<1.77.3.0a0
+  license: MIT
+  license_family: MIT
+  size: 31857486
+  timestamp: 1712740749097
+- kind: conda
+  name: rust-std-x86_64-pc-windows-msvc
+  version: 1.77.2
+  build: h17fc481_0
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-pc-windows-msvc-1.77.2-h17fc481_0.conda
+  sha256: 0c290c52a3cf1ac43a316d6caf0e073614351ccae31c681d6953dec7a2ff21e3
+  md5: 2149767f1c882154246a9a569991e3c3
+  depends:
+  - __win
+  constrains:
+  - rust >=1.77.2,<1.77.3.0a0
+  license: MIT
+  license_family: MIT
+  size: 25276039
+  timestamp: 1712742986757
+- kind: conda
+  name: rust-std-x86_64-unknown-linux-gnu
+  version: 1.77.2
+  build: h2c6d0dc_0
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/rust-std-x86_64-unknown-linux-gnu-1.77.2-h2c6d0dc_0.conda
+  sha256: 73f7537db6bc0471135a85a261798abe77e7e83794f945a0355c4068973f31f6
+  md5: db8b81b3806faafe2f6f7bd431f72e37
+  depends:
+  - __unix
+  constrains:
+  - rust >=1.77.2,<1.77.3.0a0
+  license: MIT
+  license_family: MIT
+  size: 33827015
+  timestamp: 1712741238767
+- kind: conda
   name: setuptools
   version: 69.5.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
   sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
@@ -4462,14 +4915,30 @@
   depends:
   - python
   license: MIT
   license_family: MIT
   size: 14259
   timestamp: 1620240338595
 - kind: conda
+  name: sysroot_linux-64
+  version: '2.12'
+  build: he073ed8_17
+  build_number: 17
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/sysroot_linux-64-2.12-he073ed8_17.conda
+  sha256: b4e4d685e41cb36cfb16f0cb15d2c61f8f94f56fab38987a44eff95d8a673fb5
+  md5: 595db67e32b276298ff3d94d07d47fbf
+  depends:
+  - kernel-headers_linux-64 2.6.32 he073ed8_17
+  license: LGPL-2.0-or-later AND LGPL-2.0-or-later WITH exceptions AND GPL-2.0-or-later AND MPL-2.0
+  license_family: GPL
+  size: 15127123
+  timestamp: 1708000843849
+- kind: conda
   name: tinycss2
   version: 1.3.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.3.0-pyhd8ed1ab_0.conda
   sha256: bc55e5899e66805589c02061e315bfc23ae6cc2f2811f5cc13fb189a5ed9d90f
@@ -4586,14 +5055,26 @@
   depends:
   - python >=3.8
   license: PSF-2.0
   license_family: PSF
   size: 37583
   timestamp: 1712330089194
 - kind: conda
+  name: tzdata
+  version: 2024a
+  build: h0c530f3_0
+  subdir: noarch
+  noarch: generic
+  url: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
+  sha256: 7b2b69c54ec62a243eb6fba2391b5e443421608c3ae5dbff938ad33ca8db5122
+  md5: 161081fc7cec0bfda0d86d7cb595f8d8
+  license: LicenseRef-Public-Domain
+  size: 119815
+  timestamp: 1706886945727
+- kind: conda
   name: ucrt
   version: 10.0.22621.0
   build: h57928b3_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
   sha256: f29cdaf8712008f6b419b8b1a403923b00ab2504bfe0fb2ba8eb60e72d4f14c6
   md5: 72608f6cd3e5898229c3ea16deb1ac43
@@ -4668,76 +5149,76 @@
   license: BSD-3-Clause
   license_family: BSD
   size: 16988
   timestamp: 1702511261442
 - kind: conda
   name: watchdog
   version: 4.0.0
-  build: py38h2bea1e5_0
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py38h2bea1e5_0.conda
-  sha256: e8505e3d0453cc290f11c96ba5d56330be2a021b6848164811f37fe49828d7d7
-  md5: 0d0a92d705e8a42ea70651eb6f3e2e8c
+  build: py312h2e8e312_0
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py312h2e8e312_0.conda
+  sha256: 4b1eeaecccadf55a5c322e25290d75c8bed7b0d5e25fa6dfa03fc16fc9919fc4
+  md5: 186ec4486a2c5d738c002067665b50be
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - pyyaml >=3.10
   license: Apache-2.0
   license_family: APACHE
-  size: 118056
-  timestamp: 1707295680540
+  size: 152911
+  timestamp: 1707295573907
 - kind: conda
   name: watchdog
   version: 4.0.0
-  build: py38h336bac9_0
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py38h336bac9_0.conda
-  sha256: 8acd6290c7f09b5b791eb9eeb43508eaed5aa22b75f81aad01e7f8287f98a77d
-  md5: 6987169f47c17148af8b2073726810b8
+  build: py312h7900ff3_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
+  sha256: db3ef9753934826c008216b198f04a6637150e1d91d72733148c0822e4a042a2
+  md5: 1b87b82dd803565550e6358c0790f3d2
   depends:
-  - python >=3.8,<3.9.0a0
-  - python >=3.8,<3.9.0a0 *_cpython
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - pyyaml >=3.10
   license: Apache-2.0
   license_family: APACHE
-  size: 118848
-  timestamp: 1707295730630
+  size: 136845
+  timestamp: 1707295261797
 - kind: conda
   name: watchdog
   version: 4.0.0
-  build: py38h578d9bd_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py38h578d9bd_0.conda
-  sha256: f6a07da2d18ed7366e2b07832de4626cdd7a82d2c42d64866c20decbc10996b0
-  md5: fd6f9afe747e1ec3744158e83728fc0b
+  build: py312hc2c2f20_0
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
+  sha256: f333e1f11d60e096d8b0f2b7dbe313fc9ee22d6c09f0a0cc7d3c9fed56ee48dd
+  md5: ebd7ea0d23052393f0a62efe8a508e99
   depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  - python >=3.12,<3.13.0a0
+  - python_abi 3.12.* *_cp312
   - pyyaml >=3.10
   license: Apache-2.0
   license_family: APACHE
-  size: 110414
-  timestamp: 1707295340662
+  size: 144711
+  timestamp: 1707295580304
 - kind: conda
   name: watchdog
   version: 4.0.0
-  build: py38haa244fe_0
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/watchdog-4.0.0-py38haa244fe_0.conda
-  sha256: 53248a9bc2f0cead364d18fde7f3e169bdd8ea1284dd71e04684bd45601dcad2
-  md5: 6c76373804c8f4b37dec9b23522d9624
-  depends:
-  - python >=3.8,<3.9.0a0
-  - python_abi 3.8.* *_cp38
+  build: py312he37b823_0
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
+  sha256: 3e7486e161e4478a1bb63cb124a446b21b0af113458522d215ba76eebb1a473a
+  md5: c483c04540c229b50564201c5432667c
+  depends:
+  - python >=3.12,<3.13.0a0
+  - python >=3.12,<3.13.0a0 *_cpython
+  - python_abi 3.12.* *_cp312
   - pyyaml >=3.10
   license: Apache-2.0
   license_family: APACHE
-  size: 127122
-  timestamp: 1707295617098
+  size: 145347
+  timestamp: 1707295575866
 - kind: conda
   name: webencodings
   version: 0.5.1
   build: pyhd8ed1ab_2
   build_number: 2
   subdir: noarch
   noarch: python
```

### Comparing `py_rattler-0.5.0/pixi.toml` & `py_rattler-0.6.0/pixi.toml`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [tasks]
 
 [dependencies]
 
 [feature.build.dependencies]
 maturin = "~=1.2.2"
 pip = "~=23.2.1"
+rust = "~=1.77"
 
 [feature.build.tasks]
 build = "PIP_REQUIRE_VIRTUALENV=false maturin develop"
 build-release = "PIP_REQUIRE_VIRTUALENV=false maturin develop --release"
 
 [feature.build.target.linux-64.dependencies]
 patchelf = "~=0.17.2"
@@ -50,19 +51,20 @@
 fmt-python-check = "ruff format rattler --diff"
 fmt-check = { depends_on = ["fmt-python-check", "fmt-rust-check"] }
 
 [feature.docs.dependencies]
 mkdocs = "1.5.3.*"
 mkdocstrings-python = ">=1.9.0,<1.10"
 mkdocstrings = ">=0.24.1,<0.25"
-mkdocs-material = ">=9.5.17"
+mkdocs-material = ">=9.5.20"
+mdx_truly_sane_lists = ">=1.3,<2"
 cairosvg = "2.7.1.*"
 pillow = ">=9.4.0"
 
 [feature.docs.tasks]
 docs = { cmd = "mkdocs serve" }
 build-docs = { cmd = "mkdocs build" }
 
 [environments]
-build = [ "build" ]
-test = [ "test" ]
-docs = [ "docs" ]
+#build = { features = ["build"], solve-group = "default" }
+test = { features = ["build", "test"], solve-group = "default" }
+docs = ["docs"]
```

### Comparing `py_rattler-0.5.0/pyproject.toml` & `py_rattler-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/__init__.py` & `py_rattler-0.6.0/rattler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,43 +2,46 @@
 from rattler.match_spec import MatchSpec, NamelessMatchSpec
 from rattler.repo_data import (
     PackageRecord,
     RepoData,
     RepoDataRecord,
     PatchInstructions,
     SparseRepoData,
+    Gateway,
+    SourceConfig,
 )
 from rattler.channel import Channel, ChannelConfig, ChannelPriority
 from rattler.networking import AuthenticatedClient, fetch_repo_data
 from rattler.virtual_package import GenericVirtualPackage, VirtualPackage
 from rattler.package import (
     PackageName,
     AboutJson,
     RunExportsJson,
     PathsJson,
     PathsEntry,
     PathType,
     PrefixPlaceholder,
     FileMode,
+    IndexJson,
 )
 from rattler.prefix import PrefixRecord, PrefixPaths, PrefixPathsEntry, PrefixPathType
-from rattler.solver import solve
 from rattler.platform import Platform
 from rattler.utils.rattler_version import get_rattler_version as _get_rattler_version
-from rattler.linker import link
+from rattler.install import install
 from rattler.index import index
 from rattler.lock import (
     LockFile,
     Environment,
     LockChannel,
     PackageHashes,
     LockedPackage,
     PypiPackageData,
     PypiPackageEnvironmentData,
 )
+from rattler.solver import solve
 
 __version__ = _get_rattler_version()
 del _get_rattler_version
 
 __all__ = [
     "Version",
     "VersionWithSource",
@@ -66,18 +69,20 @@
     "LockChannel",
     "PackageHashes",
     "LockedPackage",
     "PypiPackageData",
     "PypiPackageEnvironmentData",
     "solve",
     "Platform",
-    "link",
+    "install",
     "index",
     "AboutJson",
     "RunExportsJson",
     "PathsJson",
     "PathsEntry",
     "PathType",
     "PrefixPlaceholder",
     "FileMode",
     "IndexJson",
+    "Gateway",
+    "SourceConfig",
 ]
```

### Comparing `py_rattler-0.5.0/rattler/channel/channel.py` & `py_rattler-0.6.0/rattler/channel/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/channel/channel_config.py` & `py_rattler-0.6.0/rattler/channel/channel_config.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/exceptions.py` & `py_rattler-0.6.0/rattler/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
         CacheDirError,
         FetchRepoDataError,
         SolverError,
         ConvertSubdirError,
         VersionBumpError,
         EnvironmentCreationError,
         ExtractError,
+        GatewayError,
     )
 except ImportError:
     # They are only redefined for documentation purposes
     # when there is no binary yet
 
     class InvalidVersionError(Exception):  # type: ignore[no-redef]
         """Error that can occur when parsing a Version"""
@@ -77,14 +78,17 @@
 
     class EnvironmentCreationError(Exception):  # type: ignore[no-redef]
         """An error that can occur when creating an environment."""
 
     class ExtractError(Exception):  # type: ignore[no-redef]
         """An error that can occur when extracting an archive."""
 
+    class GatewayError(Exception):  # type: ignore[no-redef]
+        """An error that can occur when querying the repodata gateway."""
+
 
 __all__ = [
     "ActivationError",
     "CacheDirError",
     "DetectVirtualPackageError",
     "FetchRepoDataError",
     "InvalidChannelError",
@@ -98,8 +102,9 @@
     "ParsePlatformError",
     "SolverError",
     "TransactionError",
     "ConvertSubdirError",
     "VersionBumpError",
     "EnvironmentCreationError",
     "ExtractError",
+    "GatewayError",
 ]
```

### Comparing `py_rattler-0.5.0/rattler/index/index.py` & `py_rattler-0.6.0/rattler/index/index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/linker/linker.py` & `py_rattler-0.6.0/rattler/install/installer.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,50 +3,77 @@
 from typing import List, Optional
 
 from rattler.networking.authenticated_client import AuthenticatedClient
 from rattler.platform.platform import Platform
 from rattler.prefix.prefix_record import PrefixRecord
 from rattler.repo_data.record import RepoDataRecord
 
-from rattler.rattler import py_link
+from rattler.rattler import py_install
 
 
-async def link(
-    dependencies: List[RepoDataRecord],
+async def install(
+    records: List[RepoDataRecord],
     target_prefix: os.PathLike[str],
-    cache_dir: os.PathLike[str],
+    cache_dir: Optional[os.PathLike[str]] = None,
     installed_packages: Optional[List[PrefixRecord]] = None,
     platform: Optional[Platform] = None,
-    execute_link_scripts: bool = True,
+    execute_link_scripts: bool = False,
+    show_progress: bool = True,
+    client: Optional[AuthenticatedClient] = None,
 ) -> None:
     """
     Create an environment by downloading and linking the `dependencies` in
     the `target_prefix` directory.
 
+    !!! warning
+
+        When `execute_link_scripts` is set to `True` the post-link and pre-unlink scripts of
+        packages will be executed. These scripts are not sandboxed and can be used to execute
+        arbitraty code. It is therefor discouraged to enable executing link scripts.
+
+    Example
+    -------
+    ```python
+    >>> import asyncio
+    >>> from rattler import solve, install
+    >>> async def main():
+    ...     # Solve an environment with python 3.9 for the current platform
+    ...     records = await solve(channels=["conda-forge"], specs=["python=3.9"])
+    ...
+    ...     # Link the environment in the directory `my-env`.
+    ...     await install(records, target_prefix="my-env")
+    ...
+    ...     # That's it! The environment is now created.
+    >>> asyncio.run(main())
+
+    ```
+
     Arguments:
-        dependencies: A list of solved `RepoDataRecord`s.
+        records: A list of solved `RepoDataRecord`s.
         target_prefix: Path to the directory where the environment should
-                       be created.
+                be created.
         cache_dir: Path to directory where the dependencies will be
-                   downloaded and cached.
+                downloaded and cached.
         installed_packages: A list of `PrefixRecord`s which are
-                                      already installed in the
-                                      `target_prefix`. This can be obtained
-                                      by loading `PrefixRecord`s from
-                                      `{target_prefix}/conda-meta/`.
+                already installed in the `target_prefix`. This can be obtained by loading
+                `PrefixRecord`s from `{target_prefix}/conda-meta/`.
+                If `None` is specified then the `target_prefix` will be scanned for installed
+                packages.
         platform: Target platform to create and link the
-                            environment. Defaults to current platform.
+                environment. Defaults to current platform.
         execute_link_scripts: Wether to execute the post-link and pre-unlink scripts
-                              that may be part of a package. Defaults to True.
+                that may be part of a package. Defaults to False.
+        show_progress: If set to `True` a progress bar will be shown on the CLI.
+        client: An authenticated client to use for downloading packages. If not specified a default
+                client will be used.
     """
-    platform = platform or Platform.current()
-    client = AuthenticatedClient()
 
-    await py_link(
-        dependencies,
-        target_prefix,
-        cache_dir,
-        installed_packages or [],
-        platform._inner,
-        client._client,
-        execute_link_scripts,
+    await py_install(
+        records=records,
+        target_prefix=target_prefix,
+        cache_dir=cache_dir,
+        installed_packages=installed_packages,
+        platform=platform._inner if platform is not None else None,
+        client=client._client if client is not None else None,
+        execute_link_scripts=execute_link_scripts,
+        show_progress=show_progress,
     )
```

### Comparing `py_rattler-0.5.0/rattler/lock/channel.py` & `py_rattler-0.6.0/rattler/lock/channel.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/lock/environment.py` & `py_rattler-0.6.0/rattler/lock/environment.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/lock/hash.py` & `py_rattler-0.6.0/rattler/lock/hash.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/lock/lock_file.py` & `py_rattler-0.6.0/rattler/lock/lock_file.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/lock/package.py` & `py_rattler-0.6.0/rattler/lock/package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/lock/pypi.py` & `py_rattler-0.6.0/rattler/lock/pypi.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/match_spec/match_spec.py` & `py_rattler-0.6.0/rattler/match_spec/match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/match_spec/nameless_match_spec.py` & `py_rattler-0.6.0/rattler/match_spec/nameless_match_spec.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/networking/authenticated_client.py` & `py_rattler-0.6.0/rattler/networking/authenticated_client.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/networking/fetch_repo_data.py` & `py_rattler-0.6.0/rattler/networking/fetch_repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/package/__init__.py` & `py_rattler-0.6.0/rattler/package/__init__.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/package/about_json.py` & `py_rattler-0.6.0/rattler/package/about_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/package/index_json.py` & `py_rattler-0.6.0/rattler/package/index_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/package/package_name.py` & `py_rattler-0.6.0/rattler/package/package_name.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/package/paths_json.py` & `py_rattler-0.6.0/rattler/package/paths_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,15 +448,15 @@
 
 
 class FileMode:
     """
     The file mode of the entry.
     """
 
-    _inner: PyFileMode
+    _inner: PyFileMode | None = None
 
     @property
     def binary(self) -> bool:
         """
         The file is a binary file (needs binary prefix replacement).
 
         Examples
@@ -468,15 +468,15 @@
         >>> entry = paths_json.paths[-1]
         >>> file_mode = entry.prefix_placeholder.file_mode
         >>> file_mode.binary
         False
         >>>
         ```
         """
-        return self._inner.binary
+        return self._inner.binary if self._inner else False
 
     @property
     def text(self) -> bool:
         """
         The file is a text file (needs text prefix replacement).
 
         Examples
@@ -488,15 +488,33 @@
         >>> entry = paths_json.paths[-1]
         >>> file_mode = entry.prefix_placeholder.file_mode
         >>> file_mode.text
         True
         >>>
         ```
         """
-        return self._inner.text
+        return self._inner.text if self._inner else False
+
+    @property
+    def unknown(self) -> bool:
+        """
+        The file mode is unknown/unspecified
+        Examples
+        --------
+        ```python
+        >>> paths_json = PathsJson.from_package_archive(
+        ...     "../test-data/conda-22.9.0-py38haa244fe_2.tar.bz2"
+        ... )
+        >>> entry = paths_json.paths[-1]
+        >>> file_mode = entry.prefix_placeholder.file_mode
+        >>> file_mode.unknown
+        False
+        >>>
+        """
+        return self._inner is None
 
     @classmethod
     def _from_py_file_mode(cls, py_file_mode: PyFileMode) -> FileMode:
         file_mode = cls.__new__(cls)
         file_mode._inner = py_file_mode
 
         return file_mode
```

### Comparing `py_rattler-0.5.0/rattler/package/run_exports_json.py` & `py_rattler-0.6.0/rattler/package/run_exports_json.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/platform/arch.py` & `py_rattler-0.6.0/rattler/platform/arch.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/platform/platform.py` & `py_rattler-0.6.0/rattler/platform/platform.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/prefix/prefix_paths.py` & `py_rattler-0.6.0/rattler/prefix/prefix_paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
         >>> paths = r.paths_data
         >>> file_mode = paths.paths[0].file_mode
         >>>
         ```
         """
         return FileMode._from_py_file_mode(self._inner.file_mode)
 
+    @property
     def sha256(self) -> bytes:
         """
         The sha256 of the path.
 
         Examples
         --------
         ```python
@@ -194,14 +195,15 @@
         >>> paths = r.paths_data
         >>> sha256 = paths.paths[0].sha256
         >>>
         ```
         """
         return self._inner.sha256
 
+    @property
     def sha256_in_prefix(self) -> bytes:
         """
         The sha256 of the path in the prefix.
 
         Examples
         --------
         ```python
```

### Comparing `py_rattler-0.5.0/rattler/prefix/prefix_record.py` & `py_rattler-0.6.0/rattler/prefix/prefix_record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/repo_data/package_record.py` & `py_rattler-0.6.0/rattler/repo_data/package_record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 import os
 from typing import List, Optional
+
+from rattler import VersionWithSource
 from rattler.match_spec.match_spec import MatchSpec
+from rattler.package.no_arch_type import NoArchType
 from rattler.package.package_name import PackageName
-
 from rattler.rattler import PyRecord
-from rattler.version.version import Version
 
 
 class PackageRecord:
     """
     A single record in the Conda repodata. A single
     record refers to a single binary distribution
     of a package on a Conda channel.
@@ -284,14 +285,42 @@
         PackageName("libsqlite")
         >>>
         ```
         """
         return PackageName._from_py_package_name(self._record.name)
 
     @property
+    def noarch(self) -> Optional[str]:
+        """
+        The noarch type of the package.
+
+        Examples
+        --------
+        ```python
+        >>> from rattler import PrefixRecord
+        >>> record = PrefixRecord.from_path(
+        ...     "../test-data/conda-meta/libsqlite-3.40.0-hcfcfb64_0.json"
+        ... )
+        >>> record.noarch
+        >>> record = PrefixRecord.from_path(
+        ...     "../test-data/conda-meta/pip-23.0-pyhd8ed1ab_0.json"
+        ... )
+        >>> record.noarch
+        'python'
+        >>>
+        ```
+        """
+        noarchtype = NoArchType._from_py_no_arch_type(self._record.noarch)
+        if noarchtype.python:
+            return "python"
+        if noarchtype.generic:
+            return "generic"
+        return None
+
+    @property
     def platform(self) -> Optional[str]:
         """
         Optionally the platform the package supports.
 
         Examples
         --------
         ```python
@@ -401,31 +430,31 @@
         []
         >>>
         ```
         """
         return self._record.track_features
 
     @property
-    def version(self) -> Version:
+    def version(self) -> VersionWithSource:
         """
         The version of the package.
 
         Examples
         --------
         ```python
         >>> from rattler import PrefixRecord
         >>> record = PrefixRecord.from_path(
         ...     "../test-data/conda-meta/libsqlite-3.40.0-hcfcfb64_0.json"
         ... )
         >>> record.version
-        Version("3.40.0")
+        VersionWithSource(version="3.40.0", source="3.40.0")
         >>>
         ```
         """
-        return Version._from_py_version(self._record.version)
+        return VersionWithSource._from_py_version(*self._record.version)
 
     def __str__(self) -> str:
         """
         Returns the string representation of the PackageRecord.
 
         Examples
         --------
```

### Comparing `py_rattler-0.5.0/rattler/repo_data/patch_instructions.py` & `py_rattler-0.6.0/rattler/repo_data/patch_instructions.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/repo_data/record.py` & `py_rattler-0.6.0/rattler/repo_data/record.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/repo_data/repo_data.py` & `py_rattler-0.6.0/rattler/repo_data/repo_data.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/repo_data/sparse.py` & `py_rattler-0.6.0/rattler/repo_data/sparse.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/shell/shell.py` & `py_rattler-0.6.0/rattler/shell/shell.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/utils/rattler_version.py` & `py_rattler-0.6.0/rattler/utils/rattler_version.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/version/version.py` & `py_rattler-0.6.0/rattler/version/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     Empty segments (i.e. two consecutive dots, a leading/trailing
     underscore) are not permitted. An optional epoch number - an
     integer followed by '!' - can precede the actual version string
     (this is useful to indicate a change in the versioning scheme itself).
     Version comparison is case-insensitive.
     """
 
+    _version: PyVersion
+
     def __init__(self, version: str) -> None:
         if isinstance(version, str):
             self._version = PyVersion(version)
         else:
             raise TypeError(
                 "Version constructor received unsupported type "
                 f" {type(version).__name__!r} for the `version` parameter"
```

### Comparing `py_rattler-0.5.0/rattler/virtual_package/generic.py` & `py_rattler-0.6.0/rattler/virtual_package/generic.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/rattler/virtual_package/virtual_package.py` & `py_rattler-0.6.0/rattler/virtual_package/virtual_package.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/about_json.rs` & `py_rattler-0.6.0/src/about_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/channel/mod.rs` & `py_rattler-0.6.0/src/channel/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     fn root_dir(&self) -> String {
         self.inner.root_dir.to_string_lossy().into()
     }
 }
 
 #[pyclass]
 #[repr(transparent)]
-#[derive(Clone)]
+#[derive(Clone, Hash, Eq, PartialEq)]
 pub struct PyChannel {
     pub(crate) inner: Channel,
 }
 
 impl From<Channel> for PyChannel {
     fn from(value: Channel) -> Self {
         Self { inner: value }
@@ -75,15 +75,15 @@
     #[getter]
     fn base_url(&self) -> String {
         self.inner.base_url.to_string()
     }
 
     /// Returns the Urls for the given platform.
     pub fn platform_url(&self, platform: &PyPlatform) -> String {
-        self.inner.platform_url(platform.clone().into()).into()
+        self.inner.platform_url((*platform).into()).into()
     }
 }
 
 #[pyclass]
 #[derive(Clone)]
 pub enum PyChannelPriority {
     /// The channel that the package is first found in will be used as the only channel
```

### Comparing `py_rattler-0.5.0/src/generic_virtual_package.rs` & `py_rattler-0.6.0/src/generic_virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/index.rs` & `py_rattler-0.6.0/src/index.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/index_json.rs` & `py_rattler-0.6.0/src/index_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/lib.rs` & `py_rattler-0.6.0/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,90 @@
 mod about_json;
 mod channel;
 mod error;
 mod generic_virtual_package;
 mod index;
-mod linker;
+mod installer;
 mod lock;
 mod match_spec;
 mod meta;
 mod nameless_match_spec;
 mod networking;
+mod no_arch_type;
 mod package_name;
 mod paths_json;
 mod platform;
 mod prefix_paths;
 mod record;
 mod repo_data;
 mod shell;
 mod solver;
 mod version;
 mod virtual_package;
 
 mod index_json;
 mod run_exports_json;
+
+use std::ops::Deref;
+
 use about_json::PyAboutJson;
 use channel::{PyChannel, PyChannelConfig, PyChannelPriority};
 use error::{
     ActivationException, CacheDirException, ConvertSubdirException, DetectVirtualPackageException,
     EnvironmentCreationException, ExtractException, FetchRepoDataException,
     InvalidChannelException, InvalidMatchSpecException, InvalidPackageNameException,
     InvalidUrlException, InvalidVersionException, IoException, LinkException, ParseArchException,
     ParsePlatformException, PyRattlerError, SolverException, TransactionException,
     VersionBumpException,
 };
 use generic_virtual_package::PyGenericVirtualPackage;
+use index::py_index;
 use index_json::PyIndexJson;
+use installer::py_install;
 use lock::{
     PyEnvironment, PyLockChannel, PyLockFile, PyLockedPackage, PyPackageHashes, PyPypiPackageData,
     PyPypiPackageEnvironmentData,
 };
 use match_spec::PyMatchSpec;
+use meta::get_rattler_version;
 use nameless_match_spec::PyNamelessMatchSpec;
 use networking::{authenticated_client::PyAuthenticatedClient, py_fetch_repo_data};
+use no_arch_type::PyNoArchType;
 use package_name::PyPackageName;
 use paths_json::{PyFileMode, PyPathType, PyPathsEntry, PyPathsJson, PyPrefixPlaceholder};
+use platform::{PyArch, PyPlatform};
 use prefix_paths::{PyPrefixPathType, PyPrefixPaths, PyPrefixPathsEntry};
-use repo_data::{patch_instructions::PyPatchInstructions, sparse::PySparseRepoData, PyRepoData};
-use run_exports_json::PyRunExportsJson;
-use version::PyVersion;
-
 use pyo3::prelude::*;
-
-use index::py_index;
-use linker::py_link;
-use meta::get_rattler_version;
-use platform::{PyArch, PyPlatform};
 use record::PyRecord;
+use repo_data::{
+    gateway::{PyGateway, PySourceConfig},
+    patch_instructions::PyPatchInstructions,
+    sparse::PySparseRepoData,
+    PyRepoData,
+};
+use run_exports_json::PyRunExportsJson;
 use shell::{PyActivationResult, PyActivationVariables, PyActivator, PyShellEnum};
 use solver::py_solve;
+use version::PyVersion;
 use virtual_package::PyVirtualPackage;
 
+use crate::error::GatewayException;
+
+/// A struct to make it easy to wrap a type as a python type.
+#[repr(transparent)]
+#[derive(Clone)]
+pub struct Wrap<T>(pub T);
+
+impl<T> Deref for Wrap<T> {
+    type Target = T;
+    fn deref(&self) -> &Self::Target {
+        &self.0
+    }
+}
+
 #[pymodule]
 fn rattler(py: Python<'_>, m: &PyModule) -> PyResult<()> {
     m.add_class::<PyVersion>().unwrap();
 
     m.add_class::<PyMatchSpec>().unwrap();
     m.add_class::<PyNamelessMatchSpec>().unwrap();
 
@@ -81,25 +103,29 @@
     m.add_class::<PyActivationResult>().unwrap();
     m.add_class::<PyShellEnum>().unwrap();
     m.add_class::<PyActivator>().unwrap();
 
     m.add_class::<PySparseRepoData>().unwrap();
     m.add_class::<PyRepoData>().unwrap();
     m.add_class::<PyPatchInstructions>().unwrap();
+    m.add_class::<PyGateway>().unwrap();
+    m.add_class::<PySourceConfig>().unwrap();
 
     m.add_class::<PyRecord>().unwrap();
 
     m.add_function(wrap_pyfunction!(py_fetch_repo_data, m).unwrap())
         .unwrap();
     m.add_class::<PyGenericVirtualPackage>().unwrap();
     m.add_class::<PyVirtualPackage>().unwrap();
     m.add_class::<PyPrefixPathsEntry>().unwrap();
     m.add_class::<PyPrefixPathType>().unwrap();
     m.add_class::<PyPrefixPaths>().unwrap();
 
+    m.add_class::<PyNoArchType>().unwrap();
+
     m.add_class::<PyLockFile>().unwrap();
     m.add_class::<PyEnvironment>().unwrap();
     m.add_class::<PyLockChannel>().unwrap();
     m.add_class::<PyLockedPackage>().unwrap();
     m.add_class::<PyPypiPackageData>().unwrap();
     m.add_class::<PyPypiPackageEnvironmentData>().unwrap();
     m.add_class::<PyPackageHashes>().unwrap();
@@ -114,15 +140,15 @@
     m.add_class::<PyFileMode>().unwrap();
     m.add_class::<PyIndexJson>().unwrap();
 
     m.add_function(wrap_pyfunction!(py_solve, m).unwrap())
         .unwrap();
     m.add_function(wrap_pyfunction!(get_rattler_version, m).unwrap())
         .unwrap();
-    m.add_function(wrap_pyfunction!(py_link, m).unwrap())
+    m.add_function(wrap_pyfunction!(py_install, m).unwrap())
         .unwrap();
     m.add_function(wrap_pyfunction!(py_index, m).unwrap())
         .unwrap();
 
     // Exceptions
     m.add(
         "InvalidVersionError",
@@ -186,9 +212,12 @@
         py.get_type::<EnvironmentCreationException>(),
     )
     .unwrap();
 
     m.add("ExtractError", py.get_type::<ExtractException>())
         .unwrap();
 
+    m.add("GatewayError", py.get_type::<GatewayException>())
+        .unwrap();
+
     Ok(())
 }
```

### Comparing `py_rattler-0.5.0/src/lock/mod.rs` & `py_rattler-0.6.0/src/lock/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/match_spec.rs` & `py_rattler-0.6.0/src/match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/nameless_match_spec.rs` & `py_rattler-0.6.0/src/nameless_match_spec.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/networking/authenticated_client.rs` & `py_rattler-0.6.0/src/networking/authenticated_client.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/networking/cached_repo_data.rs` & `py_rattler-0.6.0/src/networking/cached_repo_data.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/networking/mod.rs` & `py_rattler-0.6.0/src/networking/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 use futures::future::try_join_all;
 use pyo3::{pyfunction, types::PyTuple, Py, PyAny, PyResult, Python, ToPyObject};
 use pyo3_asyncio::tokio::future_into_py;
 
 use rattler_repodata_gateway::fetch::{
-    fetch_repo_data, CachedRepoData, DownloadProgress, FetchRepoDataError, FetchRepoDataOptions,
+    fetch_repo_data, CachedRepoData, FetchRepoDataError, FetchRepoDataOptions,
 };
 use url::Url;
 
-use std::{path::PathBuf, str::FromStr};
+use std::{path::PathBuf, str::FromStr, sync::Arc};
 
 use crate::{
     channel::PyChannel, error::PyRattlerError, platform::PyPlatform,
     repo_data::sparse::PySparseRepoData,
 };
 use authenticated_client::PyAuthenticatedClient;
+use rattler_repodata_gateway::Reporter;
 
 pub mod authenticated_client;
 pub mod cached_repo_data;
 
 /// High-level function to fetch repodata for all the subdirectory of channels and platform.
 /// Returns a list of `PyRepoData`.
 #[pyfunction]
@@ -28,32 +29,31 @@
     cache_path: PathBuf,
     callback: Option<&'a PyAny>,
 ) -> PyResult<&'a PyAny> {
     let mut meta_futures = Vec::new();
     let client = PyAuthenticatedClient::new();
 
     for (subdir, chan) in get_subdir_urls(channels, platforms)? {
-        let progress = if let Some(callback) = callback {
-            let callback = callback.to_object(py);
-            Some(get_progress_func(callback))
-        } else {
-            None
-        };
+        let callback = callback.map(|callback| {
+            Arc::new(ProgressReporter {
+                callback: callback.to_object(py),
+            }) as _
+        });
         let cache_path = cache_path.clone();
         let client = client.clone();
 
         // Push all the future into meta_future vec to be resolve later
         meta_futures.push(async move {
             Ok((
                 fetch_repo_data(
                     subdir,
                     client.into(),
                     cache_path,
                     FetchRepoDataOptions::default(),
-                    progress,
+                    callback,
                 )
                 .await?,
                 chan,
             )) as Result<(CachedRepoData, PyChannel), FetchRepoDataError>
         });
     }
 
@@ -68,22 +68,31 @@
                 })
                 .collect::<Result<Vec<_>, _>>(),
             Err(e) => Err(PyRattlerError::from(e).into()),
         }
     })
 }
 
-/// Creates a closure to show progress of Download
-fn get_progress_func(callback: Py<PyAny>) -> Box<dyn FnMut(DownloadProgress) + Send + Sync> {
-    Box::new(move |progress: DownloadProgress| {
+struct ProgressReporter {
+    callback: Py<PyAny>,
+}
+
+impl Reporter for ProgressReporter {
+    fn on_download_progress(
+        &self,
+        _url: &Url,
+        _index: usize,
+        bytes_downloaded: usize,
+        total_bytes: Option<usize>,
+    ) {
         Python::with_gil(|py| {
-            let args = PyTuple::new(py, [Some(progress.bytes), progress.total]);
-            callback.call1(py, args).expect("Callback failed!");
+            let args = PyTuple::new(py, [Some(bytes_downloaded), total_bytes]);
+            self.callback.call1(py, args).expect("Callback failed!");
         });
-    })
+    }
 }
 
 /// Creates a subdir urls out of channels and channels.
 fn get_subdir_urls(
     channels: Vec<PyChannel>,
     platforms: Vec<PyPlatform>,
 ) -> PyResult<Vec<(Url, PyChannel)>> {
```

### Comparing `py_rattler-0.5.0/src/package_name.rs` & `py_rattler-0.6.0/src/package_name.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/paths_json.rs` & `py_rattler-0.6.0/src/paths_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/platform.rs` & `py_rattler-0.6.0/src/platform.rs`

 * *Files 21% similar despite different names*

```diff
@@ -49,15 +49,16 @@
 }
 
 ///////////////////////////
 /// Platform            ///
 ///////////////////////////
 
 #[pyclass]
-#[derive(Clone, Eq, PartialEq, Hash)]
+#[repr(transparent)]
+#[derive(Clone, Copy, Eq, PartialEq, Hash, Ord, PartialOrd)]
 pub struct PyPlatform {
     pub inner: Platform,
 }
 
 impl From<Platform> for PyPlatform {
     fn from(value: Platform) -> Self {
         PyPlatform { inner: value }
@@ -66,26 +67,14 @@
 
 impl From<PyPlatform> for Platform {
     fn from(value: PyPlatform) -> Self {
         value.inner
     }
 }
 
-impl PartialOrd for PyPlatform {
-    fn partial_cmp(&self, other: &Self) -> Option<std::cmp::Ordering> {
-        Some(self.cmp(other))
-    }
-}
-
-impl Ord for PyPlatform {
-    fn cmp(&self, other: &Self) -> std::cmp::Ordering {
-        self.inner.cmp(&other.inner)
-    }
-}
-
 impl FromStr for PyPlatform {
     type Err = PyRattlerError;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         let platform = Platform::from_str(s).map_err(PyRattlerError::from)?;
         Ok(platform.into())
     }
```

### Comparing `py_rattler-0.5.0/src/prefix_paths.rs` & `py_rattler-0.6.0/src/prefix_paths.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/record.rs` & `py_rattler-0.6.0/src/record.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     package::{IndexJson, PackageFile},
     PackageRecord, PrefixRecord, RepoDataRecord,
 };
 
 use rattler_digest::{parse_digest_from_hex, Md5, Sha256};
 
 use crate::{
-    error::PyRattlerError, package_name::PyPackageName, prefix_paths::PyPrefixPaths,
-    version::PyVersion,
+    error::PyRattlerError, no_arch_type::PyNoArchType, package_name::PyPackageName,
+    prefix_paths::PyPrefixPaths, version::PyVersion,
 };
 
 /// Python bindings for `PrefixRecord`, `RepoDataRecord`, `PackageRecord`.
 /// This is to expose these structs in Object Oriented manner, via a single
 /// class. This class handles the conversion on its own.
 /// It uses a `RecordInner` enum and (try_)as_{x}_record methods for this interface.
 ///
@@ -194,14 +194,20 @@
 
     /// The subdirectory where the package can be found.
     #[getter]
     pub fn subdir(&self) -> String {
         self.as_package_record().subdir.clone()
     }
 
+    /// The noarch type this package implements, if any.
+    #[getter]
+    pub fn noarch(&self) -> PyNoArchType {
+        self.as_package_record().noarch.into()
+    }
+
     /// The date this entry was created.
     #[getter]
     pub fn timestamp(&self) -> Option<i64> {
         self.as_package_record()
             .timestamp
             .map(|time| time.timestamp())
     }
@@ -213,20 +219,20 @@
     #[getter]
     pub fn track_features(&self) -> Vec<String> {
         self.as_package_record().track_features.clone()
     }
 
     /// The version of the package.
     #[getter]
-    pub fn version(&self) -> PyVersion {
-        self.as_package_record()
-            .version
-            .clone()
-            .into_version()
-            .into()
+    pub fn version(&self) -> (PyVersion, String) {
+        let version = &self.as_package_record().version;
+        (
+            version.version().clone().into(),
+            version.as_str().into_owned(),
+        )
     }
 
     /// The filename of the package.
     #[getter]
     pub fn file_name(&self) -> PyResult<String> {
         Ok(self.try_as_repodata_record()?.file_name.clone())
     }
```

### Comparing `py_rattler-0.5.0/src/repo_data/mod.rs` & `py_rattler-0.6.0/src/repo_data/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 use pyo3::{pyclass, pymethods, PyResult};
 use rattler_conda_types::RepoData;
 
 use crate::{channel::PyChannel, error::PyRattlerError, record::PyRecord};
 
 use patch_instructions::PyPatchInstructions;
 
+pub mod gateway;
 pub mod patch_instructions;
 pub mod sparse;
 
 #[pyclass]
 #[repr(transparent)]
 #[derive(Clone)]
 pub struct PyRepoData {
```

### Comparing `py_rattler-0.5.0/src/repo_data/sparse.rs` & `py_rattler-0.6.0/src/repo_data/sparse.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/run_exports_json.rs` & `py_rattler-0.6.0/src/run_exports_json.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/shell.rs` & `py_rattler-0.6.0/src/shell.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/version/component.rs` & `py_rattler-0.6.0/src/version/component.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/version/mod.rs` & `py_rattler-0.6.0/src/version/mod.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/src/virtual_package.rs` & `py_rattler-0.6.0/src/virtual_package.rs`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/tests/unit/test_fetch_repo_data.py` & `py_rattler-0.6.0/tests/unit/test_fetch_repo_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from rattler.repo_data.record import RepoDataRecord
 
 
 @pytest.fixture(scope="session")
 def serve_repo_data(xprocess) -> None:
     port, repo_name = 8912, "test-repo"
 
-    test_data_dir = os.path.join(
-        os.path.dirname(__file__), "../../../test-data/test-server"
-    )
+    test_data_dir = os.path.join(os.path.dirname(__file__), "../../../test-data/test-server")
 
     class Starter(ProcessStarter):
         # startup pattern
         pattern = f"Server started at localhost:{port}"
 
         # command to start process
         args = [
@@ -66,11 +64,8 @@
     package = PackageName(repodata.package_names()[0])
     repodata_record = repodata.load_records(package)[0]
     assert isinstance(repodata_record, RepoDataRecord)
 
     assert repodata_record.channel == f"http://localhost:{port}/{repo}/"
     assert repodata_record.file_name == "test-package-0.1-0.tar.bz2"
     assert repodata_record.name == PackageName("test-package")
-    assert (
-        repodata_record.url
-        == f"http://localhost:{port}/test-repo/noarch/test-package-0.1-0.tar.bz2"
-    )
+    assert repodata_record.url == f"http://localhost:{port}/test-repo/noarch/test-package-0.1-0.tar.bz2"
```

### Comparing `py_rattler-0.5.0/tests/unit/test_index.py` & `py_rattler-0.6.0/tests/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `py_rattler-0.5.0/tests/unit/test_prefix_record.py` & `py_rattler-0.6.0/tests/unit/test_prefix_record.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,25 +13,31 @@
     assert r.channel == "https://conda.anaconda.org/conda-forge/win-64"
     assert len(r.constrains) == 0
     assert len(r.depends) == 2
     assert str(r.extracted_package_dir) == "C:\\Users\\bas\\micromamba\\envs\\conda\\pkgs\\tk-8.6.12-h8ffe710_0"
     assert r.features is None
     assert r.file_name == "tk-8.6.12-h8ffe710_0.tar.bz2"
     assert len(r.files) == len(r.paths_data.paths) == 1099
+    assert r.subdir == "win-64"
+    assert r.noarch is None
     paths = r.paths_data
     assert isinstance(paths, PrefixPaths)
     paths_with_placeholder = 0
     assert paths.paths_version == 1
     for entry in paths.paths:
         assert isinstance(entry, PrefixPathsEntry)
         assert entry.relative_path is not None
         assert isinstance(entry.path_type, PrefixPathType)
         if entry.prefix_placeholder is not None:
             paths_with_placeholder += 1
             assert isinstance(entry.file_mode, FileMode)
             assert entry.file_mode.text or entry.file_mode.binary
-            assert entry.sha256_in_prefix is not None
-        assert entry.sha256 is not None
+            assert entry.sha256_in_prefix.hex() is not None
+        else:
+            assert entry.file_mode.unknown
+            assert entry.sha256.hex() is not None
         assert entry.size_in_bytes > 0
 
         # check that it implements os.PathLike
         isinstance(entry, os.PathLike)
+
+    assert paths_with_placeholder == 3
```

### Comparing `py_rattler-0.5.0/Cargo.lock` & `py_rattler-0.6.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -57,26 +57,26 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.82"
+version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
+checksum = "b3d1d046238990b9cf5bcde22a3fb3584ee5cf65fb2765f454ed428c7a0063da"
 
 [[package]]
 name = "archspec"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9db67cd9cf4f56a10d2cbae6a3b552e5bd36701fd37b74a18c14a231bdf446c7"
 dependencies = [
  "cfg-if",
- "itertools",
+ "itertools 0.12.1",
  "libc",
  "serde",
  "serde_json",
  "sysctl",
 ]
 
 [[package]]
@@ -87,51 +87,49 @@
 dependencies = [
  "event-listener 2.5.3",
  "futures-core",
 ]
 
 [[package]]
 name = "async-channel"
-version = "2.2.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f28243a43d821d11341ab73c80bed182dc015c514b951616cf79bd4af39af0c3"
+checksum = "89b47800b0be77592da0afd425cc03468052844aff33b84e33cc696f64e77b6a"
 dependencies = [
  "concurrent-queue",
- "event-listener 5.2.0",
- "event-listener-strategy 0.5.0",
+ "event-listener-strategy 0.5.2",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-compression"
-version = "0.4.8"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07dbbf24db18d609b1462965249abdf49129ccad073ec257da372adc83259c60"
+checksum = "9c90a406b4495d129f00461241616194cb8a032c8d1c53c657f0961d5f8e0498"
 dependencies = [
  "bzip2",
  "flate2",
  "futures-core",
  "memchr",
  "pin-project-lite",
  "tokio",
  "zstd",
  "zstd-safe",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.8.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ae5ebefcc48e7452b4987947920dac9450be1110cadf34d1b8c116bdbaf97c"
+checksum = "c8828ec6e544c02b0d6691d21ed9f9218d0384a82542855073c2a3f58304aaf0"
 dependencies = [
- "async-lock 3.3.0",
  "async-task",
  "concurrent-queue",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-lite 2.3.0",
  "slab",
 ]
 
 [[package]]
 name = "async-fs"
 version = "1.6.0"
@@ -172,16 +170,16 @@
 dependencies = [
  "async-lock 3.3.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
  "futures-lite 2.3.0",
  "parking",
- "polling 3.5.0",
- "rustix 0.38.32",
+ "polling 3.7.0",
+ "rustix 0.38.34",
  "slab",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-lock"
@@ -212,75 +210,75 @@
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-signal",
  "blocking",
  "cfg-if",
  "event-listener 3.1.0",
  "futures-lite 1.13.0",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-recursion"
-version = "1.1.0"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30c5ef0ede93efbf733c1a727f3b6b5a1060bbedd5600183e66f6e4be4af0ec5"
+checksum = "3b43422f69d8ff38f95f1b2bb76517c91589a924d1559a0e935d7c8ce0274c11"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "async-signal"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e47d90f65a225c4527103a8d747001fc56e375203592b25ad103e1ca13124c5"
+checksum = "afe66191c335039c7bb78f99dc7520b0cbb166b3a1cb33a03f53d8a1c6f2afda"
 dependencies = [
  "async-io 2.3.2",
- "async-lock 2.8.0",
+ "async-lock 3.3.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "signal-hook-registry",
  "slab",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-task"
-version = "4.7.0"
+version = "4.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbb36e985947064623dbd357f727af08ffd077f93d696782f3c56365fa2e2799"
+checksum = "8b75356056920673b02621b35afd0f7dda9306d03c79a30f5c56c44cf256e3de"
 
 [[package]]
 name = "async-trait"
 version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "backtrace"
 version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
@@ -297,17 +295,17 @@
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "base64"
-version = "0.22.0"
+version = "0.22.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
+checksum = "72b3254f16251a8381aa12e40e3c4d2f0199f8c6508fbecb9d91f575e0fbb8c6"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -361,33 +359,30 @@
 name = "block-padding"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d696c370c750c948ada61c69a0ee2cbbb9c50b1019ddb86d9317157a99c2cae"
 
 [[package]]
 name = "blocking"
-version = "1.5.1"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a37913e8dc4ddcc604f0c6d3bf2887c995153af3611de9e23c352b44c1b9118"
+checksum = "703f41c54fc768e63e091340b424302bb1c29ef4aa0c7f10fe849dfb114d29ea"
 dependencies = [
  "async-channel",
- "async-lock 3.3.0",
  "async-task",
- "fastrand 2.0.2",
  "futures-io",
  "futures-lite 2.3.0",
  "piper",
- "tracing",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
@@ -422,20 +417,21 @@
 name = "cache_control"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bf2a5fb3207c12b5d208ebc145f967fea5cac41a021c37417ccc31ba40f39ee"
 
 [[package]]
 name = "cc"
-version = "1.0.94"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
+ "once_cell",
 ]
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
@@ -444,38 +440,53 @@
 name = "chrono"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
+ "js-sys",
  "num-traits",
  "serde",
+ "wasm-bindgen",
  "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "cipher"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ee52072ec15386f770805afd189a01c8841be8696bed250fa2f13c4c0d6dfb7"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "concurrent-queue"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d16048cd947b08fa32c24458a22f5dc5e835264f689f4f5653210c69fd107363"
+checksum = "4ca0197aee26d1ae37445ee532fefce43251d24cc7c166799f4d46817f1d3973"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
+name = "console"
+version = "0.15.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0e1f83fc076bd6dd27517eacdf25fef6c4dfe5f1d7448bafaaf3a26f13b5e4eb"
+dependencies = [
+ "encode_unicode",
+ "lazy_static",
+ "libc",
+ "unicode-width",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "core-foundation"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -494,70 +505,83 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.4.0"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
+checksum = "a97769d94ddab943e4510d138150169a2758b5ef3eb191a9ee688de3e23ef7b3"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+checksum = "22ec99545bb0ed0ea7bb9b8e1e9122ea386ff8a48c0922e43f36d45ab09e0e80"
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "darling"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
+checksum = "83b2eb4d90d12bdda5ed17de686c2acb4c57914f8f921b8da7e112b5a36f3fe1"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
+checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
+checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
+]
+
+[[package]]
+name = "dashmap"
+version = "5.5.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "978747c1d849a7d2ee5e8adc0159961c48fb7e5db2f06af6723b80123bb53856"
+dependencies = [
+ "cfg-if",
+ "hashbrown 0.14.5",
+ "lock_api",
+ "once_cell",
+ "parking_lot_core",
 ]
 
 [[package]]
 name = "deranged"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
@@ -607,28 +631,34 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
 name = "elsa"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d98e71ae4df57d214182a2e5cb90230c0192c6ddfcaa05c36453d46a54713e10"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
+name = "encode_unicode"
+version = "0.3.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
+
+[[package]]
 name = "encoding_rs"
 version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
@@ -638,27 +668,27 @@
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "enum_dispatch"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa18ce2bc66555b3218614519ac839ddb759a7d6720732f979ef8d13be147ecd"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "enumflags2"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3278c9d5fb675e0a51dabcf4c0d355f692b064171535ba72361be1528a9d8e8d"
@@ -671,28 +701,28 @@
 name = "enumflags2_derive"
 version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
+checksum = "534c5cf6194dfab3db3242765c03bbe257cf92f22b38f6bc0c58d59108a820ba"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "event-listener"
@@ -720,17 +750,17 @@
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener"
-version = "5.2.0"
+version = "5.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b5fb89194fa3cad959b833185b3063ba881dbfc7030680b314250779fb4cc91"
+checksum = "6d9944b8ca13534cdfb2800775f8dd4902ff3fc75a50101466decadfdf322a24"
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -741,60 +771,70 @@
 dependencies = [
  "event-listener 4.0.3",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "event-listener-strategy"
-version = "0.5.0"
+version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "feedafcaa9b749175d5ac357452a9d41ea2911da598fde46ce1fe02c37751291"
+checksum = "0f214dc438f977e6d4e3500aaa277f5ad94ca83fbbd9b1a15713ce2344ccc5a1"
 dependencies = [
- "event-listener 5.2.0",
+ "event-listener 5.3.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.2"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
+checksum = "9fc0510504f03c51ada170672ac806f1f105a88aa97a5281117e1ddc3368e51a"
+
+[[package]]
+name = "file_url"
+version = "0.1.1"
+dependencies = [
+ "itertools 0.12.1",
+ "percent-encoding",
+ "typed-path",
+ "url",
+]
 
 [[package]]
 name = "filetime"
 version = "0.2.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1ee447700ac8aa0b2f2bd7bc4462ad686ba06baa6727ac149a2d6277f0d240fd"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall",
+ "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flate2"
-version = "1.0.28"
+version = "1.0.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
+checksum = "5f54427cfd1c7829e2a139fcefea601bf088ebca651d2bf53ebc600eac295dae"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -916,30 +956,30 @@
 
 [[package]]
 name = "futures-lite"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52527eb5074e35e9339c6b4e8d12600c7128b68fb25dcb9fa9dec18f7c25f3a5"
 dependencies = [
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-core",
  "futures-io",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -979,23 +1019,24 @@
 
 [[package]]
 name = "generic-array"
 version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
+ "serde",
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.14"
+version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
+checksum = "c4567c8db10ae91089c99af84c68c38da3ec2f087c3f82960bcdbf3656b6f4d7"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
@@ -1070,24 +1111,43 @@
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
+name = "h2"
+version = "0.4.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fa82e28a107a8cc405f0839610bdc9b15f1e25ec7d696aa5cf173edbcb1486ab"
+dependencies = [
+ "atomic-waker",
+ "bytes",
+ "fnv",
+ "futures-core",
+ "futures-sink",
+ "http 1.1.0",
+ "indexmap 2.2.6",
+ "slab",
+ "tokio",
+ "tokio-util",
+ "tracing",
+]
+
+[[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "hashbrown"
-version = "0.14.3"
+version = "0.14.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
+checksum = "e5274423e17b7c9fc20b6e7e208532f9b19825d82dfd615708b70edd83df41f1"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
@@ -1186,14 +1246,37 @@
  "futures-core",
  "http 1.1.0",
  "http-body 1.0.0",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "http-cache-semantics"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "92baf25cf0b8c9246baecf3a444546360a97b569168fdf92563ee6a47829920c"
+dependencies = [
+ "http 1.1.0",
+ "http-serde",
+ "reqwest 0.12.4",
+ "serde",
+ "time",
+]
+
+[[package]]
+name = "http-serde"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1133cafcce27ea69d35e56b3a8772e265633e04de73c5f4e1afdffc1d19b5419"
+dependencies = [
+ "http 1.1.0",
+ "serde",
+]
+
+[[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d897f394bad6a705d5f4104762e116a75639e470d80901eed05a860a95cb1904"
 
 [[package]]
 name = "httpdate"
@@ -1222,22 +1305,22 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
- "h2",
+ "h2 0.3.26",
  "http 0.2.12",
  "http-body 0.4.6",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.4.10",
+ "socket2 0.5.7",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -1245,14 +1328,15 @@
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe575dd17d0862a9a33781c8c4696a55c320909004a67a00fb286ba8b1bc496d"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
+ "h2 0.4.5",
  "http 1.1.0",
  "http-body 1.0.0",
  "httparse",
  "itoa",
  "pin-project-lite",
  "smallvec",
  "tokio",
@@ -1264,30 +1348,30 @@
 version = "0.24.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec3efd23720e2049821a693cbc7e65ea87c72f1c58ff2f9522ff332b1491e590"
 dependencies = [
  "futures-util",
  "http 0.2.12",
  "hyper 0.14.28",
- "rustls 0.21.11",
+ "rustls 0.21.12",
  "tokio",
  "tokio-rustls 0.24.1",
 ]
 
 [[package]]
 name = "hyper-rustls"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0bea761b46ae2b24eb4aef630d8d1c398157b6fc29e6350ecf090a0b70c952c"
 dependencies = [
  "futures-util",
  "http 1.1.0",
  "hyper 1.3.1",
  "hyper-util",
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "tokio",
  "tokio-rustls 0.25.0",
  "tower-service",
 ]
 
 [[package]]
@@ -1317,26 +1401,26 @@
  "tokio",
  "tokio-native-tls",
  "tower-service",
 ]
 
 [[package]]
 name = "hyper-util"
-version = "0.1.3"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca38ef113da30126bbff9cd1705f9273e15d45498615d138b0c20279ac7a76aa"
+checksum = "3d8d52be92d09acc2e01dddb7fde3ad983fc6489c7db4837e605bc3fca4cb63e"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "http 1.1.0",
  "http-body 1.0.0",
  "hyper 1.3.1",
  "pin-project-lite",
- "socket2 0.5.6",
+ "socket2 0.5.7",
  "tokio",
  "tower",
  "tower-service",
  "tracing",
 ]
 
 [[package]]
@@ -1392,29 +1476,42 @@
 [[package]]
 name = "indexmap"
 version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.3",
+ "hashbrown 0.14.5",
  "serde",
 ]
 
 [[package]]
+name = "indicatif"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "763a5a8f45087d6bcea4222e7b72c291a054edf80e4ef6efd2a4979878c7bea3"
+dependencies = [
+ "console",
+ "instant",
+ "number_prefix",
+ "portable-atomic",
+ "unicode-width",
+]
+
+[[package]]
 name = "indoc"
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
-version = "0.1.12"
+version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
+checksum = "e0242819d153cba4b4b05a5a8f2a7e9bbf97b6055b2a002b395c96b5ff3c0222"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "inventory"
 version = "0.3.15"
@@ -1444,24 +1541,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
+checksum = "d2b099aaa34a9751c5bf0878add70444e1ed2dd73f347be99003d4577277de6e"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
 version = "0.3.69"
@@ -1469,22 +1575,21 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "json-patch"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "55ff1e1486799e3f64129f8ccad108b38290df9cd7015cd31bed17239f0789d6"
+checksum = "ec9ad60d674508f3ca8f380a928cfe7b096bc729c4e2dbfe3852bc45da3ab30b"
 dependencies = [
  "serde",
  "serde_json",
  "thiserror",
- "treediff",
 ]
 
 [[package]]
 name = "jsonwebtoken"
 version = "9.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ae10193d25051e74945f1ea2d0b42e03cc3b890f7e4cc5faa44997d808193f"
@@ -1496,17 +1601,17 @@
  "serde",
  "serde_json",
  "simple_asn1",
 ]
 
 [[package]]
 name = "keyring"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1be8bc4c6b6e9d85ecdad090fcf342a9216f53d747a537cc05e3452fd650ca46"
+checksum = "363387f0019d714aa60cc30ab4fe501a747f4c08fc58f069dd14be971bd495a0"
 dependencies = [
  "byteorder",
  "lazy_static",
  "linux-keyutils",
  "secret-service",
  "security-framework",
  "windows-sys 0.52.0",
@@ -1528,28 +1633,28 @@
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44bcd58e6c97a7fcbaffcdc95728b393b8d98933bfadad49ed4097845b57ef0b"
 dependencies = [
  "proc-macro2",
  "quote",
  "regex",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.153"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
@@ -1561,31 +1666,27 @@
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
-version = "0.0.1"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
+checksum = "c0ff37bd590ca25063e35af745c343cb7a0271906fb7b37e4813e8f79f00268d"
 dependencies = [
  "bitflags 2.5.0",
  "libc",
- "redox_syscall",
 ]
 
 [[package]]
 name = "line-wrap"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30344350a2a51da54c1d53be93fade8a237e545dbcc4bdbe635413f2117cab9"
-dependencies = [
- "safemem",
-]
+checksum = "dd1bc4d24ad230d21fb898d1116b1801d7adfc449d42026475862ab48b11e70e"
 
 [[package]]
 name = "linux-keyutils"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "761e49ec5fd8a5a463f9b84e877c373d888935b71c6be78f3767fe2ae6bed18e"
 dependencies = [
@@ -1597,23 +1698,23 @@
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.13"
+version = "0.4.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
+checksum = "78b3ae25bc7c8c38cec158d1f2757ee79e9b3740fbc7ccf0e59e4b08d793fa89"
 
 [[package]]
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
@@ -1653,17 +1754,17 @@
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
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
 name = "mime"
 version = "0.3.17"
@@ -1674,17 +1775,17 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.2"
+version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
+checksum = "87dfd01fe195c66b572b37921ad8803d010623c0aca821bea2302239d155cdae"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.11"
@@ -1740,42 +1841,41 @@
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "35bd024e8b2ff75562e5f34e7f4905839deb4b22955ef5e73d2fea1b9813cb23"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
 ]
 
 [[package]]
 name = "num-bigint"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608e7659b5c3d7cba262d894801b9ec9d00de989e8a82bd4bef91d08da45cdc0"
+checksum = "c165a9ab64cf766f73521c0dd2cfdff64f488b8f0b3e621face3462d3db536d7"
 dependencies = [
- "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
+checksum = "73f88a1307638156682bada9d7604135552957b7818057dcef22705b4d509495"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-conv"
 version = "0.1.0"
@@ -1789,40 +1889,39 @@
 checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.44"
+version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
+checksum = "1429034a0490724d0075ebb2bc9e875d6503c3cf69e235a8941aa757d83ef5bf"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "f83d14da390562dca69fc84082e73e548e1ad308d24accdedd2720017cb37824"
 dependencies = [
- "autocfg",
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num_cpus"
 version = "1.16.0"
@@ -1830,14 +1929,20 @@
 checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
+name = "number_prefix"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
+
+[[package]]
 name = "object"
 version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
@@ -1873,28 +1978,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "300.2.3+3.2.1"
+version = "300.3.0+3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5cff92b6f71555b61bb9315f7c64da3ca43d87531622120fea0195fc761b4843"
+checksum = "eba8804a1c5765b18c4b3f907e6897ebabeedebc9830e1a0046c4a4cf44663e1"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
 version = "0.9.102"
@@ -1922,73 +2027,79 @@
 dependencies = [
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "ouroboros"
-version = "0.18.3"
+version = "0.18.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97b7be5a8a3462b752f4be3ff2b2bf2f7f1d00834902e46be2a4d68b87b0573c"
+checksum = "944fa20996a25aded6b4795c6d63f10014a7a83f8be9828a11860b08c5fc4a67"
 dependencies = [
  "aliasable",
  "ouroboros_macro",
  "static_assertions",
 ]
 
 [[package]]
 name = "ouroboros_macro"
-version = "0.18.3"
+version = "0.18.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b645dcde5f119c2c454a92d0dfa271a2a3b205da92e4292a68ead4bdbfde1f33"
+checksum = "39b0deead1528fd0e5947a8546a9642a9777c25f6e1e26f34c97b204bbb465bd"
 dependencies = [
  "heck",
- "itertools",
+ "itertools 0.12.1",
  "proc-macro2",
  "proc-macro2-diagnostics",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "parking"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
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
- "redox_syscall",
+ "redox_syscall 0.5.1",
  "smallvec",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
+name = "paste"
+version = "1.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57c0d7b74b563b49d38dae00a0c37d4d6de9b432382b2892f0574ddcae73fd0a"
+
+[[package]]
 name = "pem"
 version = "3.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e459365e590736a54c3fa561947c84837534b8e9af6fc5bf781307e82658fae"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "serde",
 ]
 
 [[package]]
 name = "pep440_rs"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2021,17 +2132,17 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "petgraph"
-version = "0.6.4"
+version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1d3afd2628e69da2be385eb6f2fd57c8ac7977ceeff6dc166ff1657b0e386a9"
+checksum = "b4c5cc86750666a3ed20bdaf5ca2a0344f9c67674cae0515bec2da16fbaa47db"
 dependencies = [
  "fixedbitset",
  "indexmap 2.2.6",
 ]
 
 [[package]]
 name = "phf"
@@ -2059,15 +2170,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3444646e286606587e49f3bcf1679b8cef1dc2c5ecc29ddacaffc305180d464b"
 dependencies = [
  "phf_generator",
  "phf_shared",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "unicase",
 ]
 
 [[package]]
 name = "phf_shared"
 version = "0.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2090,15 +2201,15 @@
 name = "pin-project-internal"
 version = "1.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f38a4412a78282e09a2cf38d195ea5420d15ba0602cb375210efbc877243965"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
@@ -2107,34 +2218,34 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "piper"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "668d31b1c4eba19242f2088b2bf3316b82ca31082a8335764db4e083db7485d4"
+checksum = "464db0c665917b13ebb5d453ccdec4add5658ee1adc7affc7677615356a8afaf"
 dependencies = [
  "atomic-waker",
- "fastrand 2.0.2",
+ "fastrand 2.1.0",
  "futures-io",
 ]
 
 [[package]]
 name = "pkg-config"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "plist"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5699cc8a63d1aa2b1ee8e12b9ad70ac790d65788cd36101fa37f87ea46c4cef"
+checksum = "d9d34169e64b3c7a80c8621a48adaf44e0cf62c78a9b25dd9dd35f1881a17cf9"
 dependencies = [
  "base64 0.21.7",
  "indexmap 2.2.6",
  "line-wrap",
  "quick-xml",
  "serde",
  "time",
@@ -2154,22 +2265,23 @@
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.5.0"
+version = "3.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24f040dee2588b4963afb4e420540439d126f73fdacf4a9c486a96d840bac3c9"
+checksum = "645493cf344456ef24219d02a768cf1fb92ddf8c92161679ae3d91b91a637be3"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
+ "hermit-abi",
  "pin-project-lite",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "portable-atomic"
 version = "1.6.0"
@@ -2196,54 +2308,55 @@
 dependencies = [
  "once_cell",
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.81"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1597b0c024618f09a9c3b8655b7e430397a36d23fdafec26d6965e9eec3eba"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "proc-macro2-diagnostics"
 version = "0.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af066a9c399a26e020ada66a034357a868728e72cd426f3adcd35f80d88d88c8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "version_check",
  "yansi",
 ]
 
 [[package]]
 name = "purl"
-version = "0.1.2"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d153044e55fb5c0a6f0f0f974c3335d15a842263ba4b208d2656120fe530a5ab"
+checksum = "c14fe28c8495f7eaf77a6e6106966f95211c0a2404b9da50d248fc32af3a3f14"
 dependencies = [
  "hex",
  "percent-encoding",
  "phf",
  "serde",
  "smartstring",
  "thiserror",
  "unicase",
 ]
 
 [[package]]
 name = "py-rattler"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "anyhow",
+ "chrono",
  "futures",
  "openssl",
  "pep508_rs",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-build-config 0.21.2",
  "rattler",
@@ -2253,32 +2366,33 @@
  "rattler_lock",
  "rattler_networking",
  "rattler_package_streaming",
  "rattler_repodata_gateway",
  "rattler_shell",
  "rattler_solve",
  "rattler_virtual_packages",
- "reqwest 0.12.3",
+ "reqwest 0.12.4",
  "reqwest-middleware",
  "thiserror",
  "tokio",
  "url",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
+ "chrono",
  "indoc",
  "inventory",
  "libc",
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "parking_lot",
  "portable-atomic",
  "pyo3-build-config 0.20.3",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
@@ -2331,28 +2445,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config 0.20.3",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.31.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
@@ -2403,252 +2517,277 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rattler"
-version = "0.23.1"
+version = "0.26.0"
 dependencies = [
  "anyhow",
  "bytes",
  "chrono",
+ "console",
  "digest",
  "dirs",
  "fs-err",
  "futures",
  "fxhash",
+ "humantime",
  "indexmap 2.2.6",
- "itertools",
+ "indicatif",
+ "itertools 0.12.1",
  "memchr",
  "memmap2",
  "once_cell",
+ "parking_lot",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_networking",
  "rattler_package_streaming",
  "rattler_shell",
  "reflink-copy",
  "regex",
- "reqwest 0.12.3",
+ "reqwest 0.12.4",
  "reqwest-middleware",
+ "simple_spawn_blocking",
  "smallvec",
  "tempfile",
  "thiserror",
  "tokio",
  "tokio-stream",
  "tracing",
  "url",
  "uuid",
 ]
 
 [[package]]
 name = "rattler_conda_types"
-version = "0.22.0"
+version = "0.24.0"
 dependencies = [
  "chrono",
+ "file_url",
  "fxhash",
  "glob",
  "hex",
- "itertools",
+ "itertools 0.12.1",
  "lazy-regex",
  "nom",
  "purl",
  "rattler_digest",
  "rattler_macros",
  "regex",
  "serde",
  "serde_json",
  "serde_repr",
  "serde_with",
  "smallvec",
  "strum",
  "thiserror",
  "tracing",
+ "typed-path",
  "url",
 ]
 
 [[package]]
 name = "rattler_digest"
-version = "0.19.3"
+version = "0.19.4"
 dependencies = [
  "blake2",
  "digest",
+ "generic-array",
  "hex",
  "md-5",
  "serde",
  "serde_with",
  "sha2",
  "tokio",
 ]
 
 [[package]]
 name = "rattler_index"
-version = "0.19.8"
+version = "0.19.13"
 dependencies = [
  "fs-err",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_package_streaming",
  "serde_json",
  "tracing",
  "walkdir",
 ]
 
 [[package]]
 name = "rattler_lock"
-version = "0.22.3"
+version = "0.22.8"
 dependencies = [
  "chrono",
+ "file_url",
  "fxhash",
  "indexmap 2.2.6",
- "itertools",
+ "itertools 0.12.1",
  "pep440_rs",
  "pep508_rs",
- "percent-encoding",
  "purl",
  "rattler_conda_types",
  "rattler_digest",
  "serde",
  "serde_json",
+ "serde_repr",
  "serde_with",
  "serde_yaml",
  "thiserror",
  "url",
 ]
 
 [[package]]
 name = "rattler_macros"
 version = "0.19.3"
 dependencies = [
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "rattler_networking"
-version = "0.20.3"
+version = "0.20.8"
 dependencies = [
  "anyhow",
  "async-trait",
- "base64 0.22.0",
+ "base64 0.22.1",
+ "bytes",
  "chrono",
  "dirs",
  "fslock",
+ "futures",
  "getrandom",
  "google-cloud-auth",
  "http 1.1.0",
- "itertools",
+ "itertools 0.12.1",
  "keyring",
  "netrc-rs",
- "reqwest 0.12.3",
+ "pin-project-lite",
+ "reqwest 0.12.4",
  "reqwest-middleware",
  "retry-policies",
  "serde",
  "serde_json",
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_package_streaming"
-version = "0.20.6"
+version = "0.21.0"
 dependencies = [
  "bzip2",
  "chrono",
  "futures-util",
  "num_cpus",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_networking",
- "reqwest 0.12.3",
+ "reqwest 0.12.4",
  "reqwest-middleware",
  "serde_json",
  "tar",
  "tempfile",
  "thiserror",
  "tokio",
  "tokio-util",
  "url",
  "zip",
  "zstd",
 ]
 
 [[package]]
 name = "rattler_repodata_gateway"
-version = "0.19.9"
+version = "0.20.2"
 dependencies = [
  "anyhow",
  "async-compression",
+ "async-trait",
  "blake2",
+ "bytes",
  "cache_control",
  "chrono",
+ "dashmap",
+ "dirs",
+ "file_url",
  "futures",
  "hex",
+ "http 1.1.0",
+ "http-cache-semantics",
  "humansize",
  "humantime",
- "itertools",
+ "itertools 0.12.1",
  "json-patch",
  "libc",
+ "md-5",
  "memmap2",
  "ouroboros",
+ "parking_lot",
+ "percent-encoding",
  "pin-project-lite",
  "rattler_conda_types",
  "rattler_digest",
  "rattler_networking",
- "reqwest 0.12.3",
+ "reqwest 0.12.4",
  "reqwest-middleware",
+ "rmp-serde",
  "serde",
  "serde_json",
  "serde_with",
+ "simple_spawn_blocking",
  "superslice",
  "tempfile",
  "thiserror",
  "tokio",
  "tokio-util",
  "tracing",
  "url",
  "windows-sys 0.52.0",
+ "zstd",
 ]
 
 [[package]]
 name = "rattler_shell"
-version = "0.20.1"
+version = "0.20.5"
 dependencies = [
  "enum_dispatch",
  "indexmap 2.2.6",
- "itertools",
+ "itertools 0.12.1",
  "rattler_conda_types",
  "serde_json",
  "shlex",
  "tempfile",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "rattler_solve"
-version = "0.21.0"
+version = "0.23.0"
 dependencies = [
  "chrono",
  "futures",
- "itertools",
+ "itertools 0.12.1",
  "rattler_conda_types",
  "rattler_digest",
  "resolvo",
  "tempfile",
  "thiserror",
  "tracing",
  "url",
 ]
 
 [[package]]
 name = "rattler_virtual_packages"
-version = "0.19.8"
+version = "0.19.12"
 dependencies = [
  "archspec",
  "libloading",
  "nom",
  "once_cell",
  "plist",
  "rattler_conda_types",
@@ -2664,32 +2803,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
+name = "redox_syscall"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
+dependencies = [
+ "bitflags 2.5.0",
+]
+
+[[package]]
 name = "redox_users"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a18479200779601e498ada4e8c1e1f50e3ee19deb0259c25825a98b5603b2cb4"
+checksum = "bd283d9651eeda4b2a83a43c1c91b266c40fd76ecd39a50a8c630ae69dc72891"
 dependencies = [
  "getrandom",
  "libredox",
  "thiserror",
 ]
 
 [[package]]
 name = "reflink-copy"
-version = "0.1.16"
+version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dea9fb2ba3bcc8c51607906e56fe392ba2eb9947dcc84597f26d73f56877c66"
+checksum = "7c3138c30c59ed9b8572f82bed97ea591ecd7e45012566046cc39e72679cff22"
 dependencies = [
  "cfg-if",
- "rustix 0.38.32",
+ "rustix 0.38.34",
  "windows",
 ]
 
 [[package]]
 name = "regex"
 version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2710,44 +2858,44 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
 version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
  "base64 0.21.7",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
- "h2",
+ "h2 0.3.26",
  "http 0.2.12",
  "http-body 0.4.6",
  "hyper 0.14.28",
  "hyper-rustls 0.24.2",
  "hyper-tls 0.5.0",
  "ipnet",
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.21.11",
+ "rustls 0.21.12",
  "rustls-pemfile 1.0.4",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "system-configuration",
  "tokio",
@@ -2760,23 +2908,24 @@
  "web-sys",
  "webpki-roots 0.25.4",
  "winreg 0.50.0",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.12.3"
+version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
+checksum = "566cafdd92868e0939d3fb961bd0dc25fcfaaed179291093b3d43e6b3150ea10"
 dependencies = [
  "async-compression",
- "base64 0.22.0",
+ "base64 0.22.1",
  "bytes",
  "futures-core",
  "futures-util",
+ "h2 0.4.5",
  "http 1.1.0",
  "http-body 1.0.0",
  "http-body-util",
  "hyper 1.3.1",
  "hyper-rustls 0.26.0",
  "hyper-tls 0.6.0",
  "hyper-util",
@@ -2784,15 +2933,15 @@
  "js-sys",
  "log",
  "mime",
  "native-tls",
  "once_cell",
  "percent-encoding",
  "pin-project-lite",
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pemfile 2.1.2",
  "rustls-pki-types",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "sync_wrapper",
  "tokio",
@@ -2807,38 +2956,38 @@
  "web-sys",
  "webpki-roots 0.26.1",
  "winreg 0.52.0",
 ]
 
 [[package]]
 name = "reqwest-middleware"
-version = "0.3.0"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0209efb52486ad88136190094ee214759ef7507068b27992256ed6610eb71a01"
+checksum = "a45d100244a467870f6cb763c4484d010a6bed6bd610b3676e3825d93fb4cfbd"
 dependencies = [
  "anyhow",
  "async-trait",
  "http 1.1.0",
- "reqwest 0.12.3",
+ "reqwest 0.12.4",
  "serde",
  "thiserror",
  "tower-service",
 ]
 
 [[package]]
 name = "resolvo"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2016584c3fd9df0fd859a7dcbc7fafdc7fdd2d87b53a576e8e63e62fad140e33"
+checksum = "d299d168910c5d71f3c0f5441abe38ca4a6ae21f70fae909bfc6bead28f6620f"
 dependencies = [
  "bitvec",
  "elsa",
- "event-listener 5.2.0",
+ "event-listener 5.3.0",
  "futures",
- "itertools",
+ "itertools 0.13.0",
  "petgraph",
  "tracing",
 ]
 
 [[package]]
 name = "retry-policies"
 version = "0.3.0"
@@ -2862,18 +3011,40 @@
  "libc",
  "spin",
  "untrusted",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
+name = "rmp"
+version = "0.8.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "228ed7c16fa39782c3b3468e974aec2795e9089153cd08ee2e9aefb3613334c4"
+dependencies = [
+ "byteorder",
+ "num-traits",
+ "paste",
+]
+
+[[package]]
+name = "rmp-serde"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "52e599a477cf9840e92f2cde9a7189e67b42c57532749bf90aea6ec10facd4db"
+dependencies = [
+ "byteorder",
+ "rmp",
+ "serde",
+]
+
+[[package]]
 name = "rustc-demangle"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
+checksum = "719b953e2095829ee67db738b3bfa9fa368c94900df327b3f07fe6e794d2fe1f"
 
 [[package]]
 name = "rustix"
 version = "0.37.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fea8ca367a3a01fe35e6943c400addf443c0f57670e6ec51196f71a4b8762dd2"
 dependencies = [
@@ -2883,47 +3054,47 @@
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.32"
+version = "0.38.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
+checksum = "70dc5ec042f7a43c4a73241207cecc9873a06d45debb38b329f8541d85c2730f"
 dependencies = [
  "bitflags 2.5.0",
  "errno",
  "libc",
- "linux-raw-sys 0.4.13",
+ "linux-raw-sys 0.4.14",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.11"
+version = "0.21.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7fecbfb7b1444f477b345853b1fce097a2c6fb637b2bfb87e6bc5db0f043fae4"
+checksum = "3f56a14d1f48b391359b22f731fd4bd7e43c97f3c50eee276f3aa09c94784d3e"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki 0.101.7",
  "sct",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.22.3"
+version = "0.22.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
+checksum = "bf4ef73721ac7bcd79b2b315da7779d8fc09718c6b3d2d1b2d94850eb8c18432"
 dependencies = [
  "log",
  "ring",
  "rustls-pki-types",
- "rustls-webpki 0.102.2",
+ "rustls-webpki 0.102.4",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.4"
@@ -2935,62 +3106,56 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.22.0",
+ "base64 0.22.1",
  "rustls-pki-types",
 ]
 
 [[package]]
 name = "rustls-pki-types"
-version = "1.4.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
 version = "0.101.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.2"
+version = "0.102.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
-
-[[package]]
-name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
-name = "safemem"
-version = "0.3.3"
+name = "ryu"
+version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef703b7cb59335eae2eb93ceb664c0eb7ea6bf567079d843e09420219668e072"
+checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -3039,76 +3204,76 @@
  "serde",
  "sha2",
  "zbus",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
+checksum = "c627723fd09706bacdb5cf41499e95098555af3c3c29d014dc3c458ef6be11c0"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.10.0"
+version = "2.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
+checksum = "317936bbbd05227752583946b9e66d7ce3b489f84e11a94a510b4437fef407d7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.198"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9846a40c979031340571da2545a4e5b7c4163bdae79b301d5f86d03979451fcc"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.198"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e88edab869b01783ba905e7d0153f9fc1a6505a96e4ad3018011eedb838566d9"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.116"
+version = "1.0.117"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
+checksum = "455182ea6142b14f93f4bc5320a2b31c1f266b66a4a5c858b013302a5d8cbfc3"
 dependencies = [
  "indexmap 2.2.6",
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
-version = "0.1.18"
+version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
+checksum = "6c64451ba24fc7a6a2d60fc75dd9c83c90903b19028d4eff35e88fc1e86564e9"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d3491c14715ca2294c4d6a88f15e84739788c1d030eed8c110436aafdaa2f3fd"
@@ -3117,40 +3282,40 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_with"
-version = "3.7.0"
+version = "3.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee80b0e361bbf88fd2f6e242ccd19cfda072cb0faa6ae694ecee08199938569a"
+checksum = "0ad483d2ab0149d5a5ebcd9972a3852711e0153d863bf5a5d0391d28883c4a20"
 dependencies = [
- "base64 0.21.7",
+ "base64 0.22.1",
  "chrono",
  "hex",
  "indexmap 1.9.3",
  "indexmap 2.2.6",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_with_macros",
  "time",
 ]
 
 [[package]]
 name = "serde_with_macros"
-version = "3.7.0"
+version = "3.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6561dc161a9224638a31d876ccdfefbc1df91d3f3a8342eddb35f055d48c7655"
+checksum = "65569b702f41443e8bc8bbb1c5779bd0450bbe723b56198980e80ec45780bce2"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "serde_yaml"
 version = "0.9.34+deprecated"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a8b1a1a2ebf674015cc02edccce75287f1a0130d394307b36743c2f5d504b47"
@@ -3188,17 +3353,17 @@
 name = "shlex"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.1"
+version = "1.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
+checksum = "a9e9e0b4211b72e7b8b6e85c807d36c212bdb33ea8587f7569562a84df5465b1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simple_asn1"
 version = "0.6.2"
@@ -3208,14 +3373,21 @@
  "num-bigint",
  "num-traits",
  "thiserror",
  "time",
 ]
 
 [[package]]
+name = "simple_spawn_blocking"
+version = "1.0.0"
+dependencies = [
+ "tokio",
+]
+
+[[package]]
 name = "siphasher"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38b58827f4464d87d377d175e90bf58eb00fd8716ff0a62f80356b5e61555d0d"
 
 [[package]]
 name = "slab"
@@ -3254,17 +3426,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.6"
+version = "0.5.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
+checksum = "ce305eb0b4296696835b71df73eb912e0f1ffd2556a501fcede6e0c50349191c"
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
@@ -3282,17 +3454,17 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "7da8b5736845d9f2fcb837ea5d9e2628564b3b043a70948a3f0b778838c5fb4f"
 
 [[package]]
 name = "strum"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d8cec3501a5194c432b2b7976db6b7d10ec95c253208b45f83f7136aa985e29"
 dependencies = [
@@ -3305,15 +3477,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6cf59daf282c0a494ba14fd21610a0325f9f90ec9d1231dea26bcb1d696c946"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "subtle"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
@@ -3333,17 +3505,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.59"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -3413,44 +3585,44 @@
 [[package]]
 name = "tempfile"
 version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
- "fastrand 2.0.2",
- "rustix 0.38.32",
+ "fastrand 2.1.0",
+ "rustix 0.38.34",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
+checksum = "c546c80d6be4bc6a00c0f01730c08df82eaa7a7a61f11d656526506112cc1709"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.58"
+version = "1.0.61"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
+checksum = "46c3384250002a6d5af4d114f2845d37b57521033f30d5c3f46c4d70e1197533"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -3461,17 +3633,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
@@ -3497,28 +3669,28 @@
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "parking_lot",
  "pin-project-lite",
- "socket2 0.5.6",
+ "socket2 0.5.7",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -3529,25 +3701,25 @@
 
 [[package]]
 name = "tokio-rustls"
 version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
- "rustls 0.21.11",
+ "rustls 0.21.12",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-rustls"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "775e0c0f0adb3a2f22a00c4745d728b479985fc15ee7ca6a2608388c5569860f"
 dependencies = [
- "rustls 0.22.3",
+ "rustls 0.22.4",
  "rustls-pki-types",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-stream"
 version = "0.1.15"
@@ -3558,31 +3730,30 @@
  "pin-project-lite",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.10"
+version = "0.7.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
+checksum = "9cf6b47b3771c49ac75ad09a6162f53ad4b8088b76ac60e8ec1455b31a189fe1"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
- "tracing",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 
 [[package]]
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
@@ -3600,15 +3771,14 @@
  "futures-core",
  "futures-util",
  "pin-project",
  "pin-project-lite",
  "tokio",
  "tower-layer",
  "tower-service",
- "tracing",
 ]
 
 [[package]]
 name = "tower-layer"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c20c8dbed6283a09604c3e69b4b7eeb54e298b8a600d4d5ecb5ad39de609f1d0"
@@ -3621,68 +3791,64 @@
 
 [[package]]
 name = "tracing"
 version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
-name = "treediff"
-version = "4.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d127780145176e2b5d16611cc25a900150e86e9fd79d3bde6ff3a37359c9cb5"
-dependencies = [
- "serde_json",
-]
-
-[[package]]
 name = "try-lock"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
+name = "typed-path"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6069e2cc1d241fd4ff5fa067e8882996fcfce20986d078696e05abccbcf27b43"
+
+[[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
 name = "uds_windows"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89daebc3e6fd160ac4aa9fc8b3bf71e1f74fbf92367ae71fb83a037e8bf164b9"
 dependencies = [
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "tempfile",
  "winapi",
 ]
 
 [[package]]
 name = "unicase"
 version = "2.7.0"
@@ -3711,17 +3877,17 @@
 checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-width"
-version = "0.1.11"
+version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
+checksum = "68f5e5f3158ecfd4b8ff6fe086db7c8467a2dfdac97fe420f2b7c4aa97af66d6"
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
@@ -3781,17 +3947,17 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "waker-fn"
-version = "1.1.1"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3c4517f54858c779bbcbf228f4fca63d121bf85fbecb2dc578cdf4a39395690"
+checksum = "317211a0dc0ceedd78fb2ca9a44aed3d7b9b26f81870d485c07122b4350673b7"
 
 [[package]]
 name = "walkdir"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
@@ -3831,15 +3997,15 @@
 checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3865,15 +4031,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.92"
@@ -3932,19 +4098,19 @@
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
@@ -3984,26 +4150,26 @@
 name = "windows-implement"
 version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6fc35f58ecd95a9b71c4f2329b911016e6bec66b3f2e6a4aad86bd2e99e2f9b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "windows-interface"
 version = "0.56.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08990546bf4edef8f431fa6326e032865f27138718c587dc21bc0265bbcb57cc"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.59",
+ "syn 2.0.66",
 ]
 
 [[package]]
 name = "windows-result"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "749f0da9cc72d82e600d8d2e44cadd0b9eedb9038f71a1c58556ac1c5791813b"
@@ -4191,16 +4357,16 @@
 [[package]]
 name = "xattr"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8da84f1a25939b27f6820d92aed108f83ff920fdf11a7b19366c27c4cda81d4f"
 dependencies = [
  "libc",
- "linux-raw-sys 0.4.13",
- "rustix 0.38.32",
+ "linux-raw-sys 0.4.14",
+ "rustix 0.38.34",
 ]
 
 [[package]]
 name = "xdg-home"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "21e5a325c3cb8398ad6cf859c1135b25dd29e186679cf2da7581d9679f63b38e"
@@ -4279,17 +4445,17 @@
  "serde",
  "static_assertions",
  "zvariant",
 ]
 
 [[package]]
 name = "zeroize"
-version = "1.7.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+checksum = "ced3678a2879b30306d323f4542626697a464a97c0a07c9aebf7ebca65cd4dde"
 
 [[package]]
 name = "zip"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
```

### Comparing `py_rattler-0.5.0/PKG-INFO` & `py_rattler-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-rattler
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed
@@ -51,41 +51,37 @@
 Rattler is a library that provides common functionality used within the conda ecosystem ([what is conda & conda-forge?](#what-is-conda--conda-forge)).
 The goal of the library is to enable programs and other libraries to easily interact with the conda ecosystem without being dependent on Python.
 Its primary use case is as a library that you can use to provide conda related workflows in your own tools.
 
 Rattler is written in Rust and tries to provide a clean API to its functionalities (see: [Components](#components)). 
 With the primary goal in mind we aim to provide bindings to different languages to make it easy to integrate Rattler in non-rust projects.
 
-Rattler is actively used within the https://prefix.dev backend.
+Rattler is actively used by [pixi](https://github.com/prefix-dev/pixi), [rattler-build](https://github.com/prefix-dev/rattler-build), and the https://prefix.dev backend.
 
 ## Showcase
 
 This repository also contains a binary (use `cargo run` to try) that shows some of the capabilities of the library.
 This is an example of installing an environment containing `cowpy` and all its dependencies _from scratch_ (including Python!):
 
 ![Installing an environment](https://github.com/mamba-org/rattler/assets/4995967/c7946f6e-28a9-41ef-8836-ef4b4c94d273)
 
 ## Give it a try!
 
 Before you begin, make sure you have the following prerequisites:
 - A recent version of [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
-- A recent version of [micromamba](https://github.com/mamba-org/micromamba-releases)
+- A recent version of [pixi](https://github.com/prefix-dev/pixi)
 
 Follow these steps to clone, compile, and run the rattler project:
 ```shell
 # Clone the rattler repository along with its submodules:
 git clone --recursive https://github.com/mamba-org/rattler.git
 cd rattler
 
-# Set up an environment with the required dependencies for compiling rattler and libsolv:
-micromamba create -f environment.yml
-micromamba activate rattler-env
-
 # Compile and execute rattler to create a JupyterLab instance:
-cargo run --release --bin rattler create jupyterlab
+pixi run rattler create jupyterlab
 ```
 
 The above command will execute the `rattler` executable in release mode.
 It will download and install an environment into the `.prefix` folder that contains [`jupyterlab`](https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) and all the dependencies required to run it (like `python`)
 
 Run the following command to start jupyterlab:
 
@@ -115,19 +111,26 @@
 
 * **rattler_conda_types**: foundational types for all datastructures used withing the conda eco-system.
 * **rattler_package_streaming**: provides functionality to download, extract and create conda package archives.  
 * **rattler_repodata_gateway**: downloads, reads and processes information about existing conda packages from an index.
 * **rattler_shell**: code to activate an existing environment and run programs in it.
 * **rattler_solve**: a backend agnostic library to solve the package satisfiability problem.
 * **rattler_virtual_packages**: a crate to detect system capabilities.
+* **rattler_index**: create local conda channels from local packages.
 * **rattler**: functionality to create complete environments from scratch using the crates above.
+* **rattler-lock**: a library to create and parse lockfiles for conda environments.
+* **rattler-networking**: common functionality for networking, like authentication, mirroring and more.
 * **rattler-bin**: an example of a package manager using all the crates above (see: [showcase](#showcase))
 
 You can find these crates in the `crates` folder.
 
+Additionally, we provide Python bindings for most of the functionalities provided by the above crates.
+A python package `py-rattler` is available on [conda-forge](https://prefix.dev/channels/conda-forge/packages/py-rattler) and [PyPI](https://pypi.org/project/py-rattler/).
+Documatation for the python bindings can be found [here](https://mamba-org.github.io/rattler/py-rattler).
+
 ## What is conda & conda-forge?
 
 The conda ecosystem provides **cross-platform**, **binary** packages that you can use with **any programming language**.
 `conda` is an open-source package management system and environment management system that can install and manage multiple versions of software packages and their dependencies.
 `conda` is written in Python.
 The aim of Rattler is to provide all functionality required to work with the conda ecosystem from Rust.
 Rattler is not a reimplementation of `conda`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: py-rattler Version: 0.5.0 Classifier: Development
+Metadata-Version: 2.1 Name: py-rattler Version: 0.6.0 Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Typing :: Typed License-File: LICENSE Summary: A blazing fast
 library to work with the conda ecosystem Author-email: Bas Zalmstra
 gmail.com>, Tarun Pratap Singh
@@ -32,32 +32,31 @@
 conda-forge?](#what-is-conda--conda-forge)). The goal of the library is to
 enable programs and other libraries to easily interact with the conda ecosystem
 without being dependent on Python. Its primary use case is as a library that
 you can use to provide conda related workflows in your own tools. Rattler is
 written in Rust and tries to provide a clean API to its functionalities (see:
 [Components](#components)). With the primary goal in mind we aim to provide
 bindings to different languages to make it easy to integrate Rattler in non-
-rust projects. Rattler is actively used within the https://prefix.dev backend.
-## Showcase This repository also contains a binary (use `cargo run` to try)
-that shows some of the capabilities of the library. This is an example of
-installing an environment containing `cowpy` and all its dependencies _from
-scratch_ (including Python!): ![Installing an environment](https://github.com/
-mamba-org/rattler/assets/4995967/c7946f6e-28a9-41ef-8836-ef4b4c94d273) ## Give
-it a try! Before you begin, make sure you have the following prerequisites: - A
-recent version of [git](https://git-scm.com/book/en/v2/Getting-Started-
-Installing-Git) - A recent version of [micromamba](https://github.com/mamba-
-org/micromamba-releases) Follow these steps to clone, compile, and run the
+rust projects. Rattler is actively used by [pixi](https://github.com/prefix-
+dev/pixi), [rattler-build](https://github.com/prefix-dev/rattler-build), and
+the https://prefix.dev backend. ## Showcase This repository also contains a
+binary (use `cargo run` to try) that shows some of the capabilities of the
+library. This is an example of installing an environment containing `cowpy` and
+all its dependencies _from scratch_ (including Python!): ![Installing an
+environment](https://github.com/mamba-org/rattler/assets/4995967/c7946f6e-28a9-
+41ef-8836-ef4b4c94d273) ## Give it a try! Before you begin, make sure you have
+the following prerequisites: - A recent version of [git](https://git-scm.com/
+book/en/v2/Getting-Started-Installing-Git) - A recent version of [pixi](https:/
+/github.com/prefix-dev/pixi) Follow these steps to clone, compile, and run the
 rattler project: ```shell # Clone the rattler repository along with its
 submodules: git clone --recursive https://github.com/mamba-org/rattler.git cd
-rattler # Set up an environment with the required dependencies for compiling
-rattler and libsolv: micromamba create -f environment.yml micromamba activate
-rattler-env # Compile and execute rattler to create a JupyterLab instance:
-cargo run --release --bin rattler create jupyterlab ``` The above command will
-execute the `rattler` executable in release mode. It will download and install
-an environment into the `.prefix` folder that contains [`jupyterlab`](https://
+rattler # Compile and execute rattler to create a JupyterLab instance: pixi run
+rattler create jupyterlab ``` The above command will execute the `rattler`
+executable in release mode. It will download and install an environment into
+the `.prefix` folder that contains [`jupyterlab`](https://
 jupyterlab.readthedocs.io/en/stable/getting_started/overview.html) and all the
 dependencies required to run it (like `python`) Run the following command to
 start jupyterlab: ```shell # on windows .\.prefix\Scripts\jupyter-lab.exe # on
 linux or macOS ./.prefix/bin/jupyter-lab ``` Voila! You have a working
 installation of jupyterlab installed on your system! You can of course install
 any package you want this way. Try it! ## Contributing ð We would love to
 have you contribute! See the CONTRIBUTION.md for more info. For questions,
@@ -68,23 +67,32 @@
 the conda eco-system. * **rattler_package_streaming**: provides functionality
 to download, extract and create conda package archives. *
 **rattler_repodata_gateway**: downloads, reads and processes information about
 existing conda packages from an index. * **rattler_shell**: code to activate an
 existing environment and run programs in it. * **rattler_solve**: a backend
 agnostic library to solve the package satisfiability problem. *
 **rattler_virtual_packages**: a crate to detect system capabilities. *
+**rattler_index**: create local conda channels from local packages. *
 **rattler**: functionality to create complete environments from scratch using
-the crates above. * **rattler-bin**: an example of a package manager using all
-the crates above (see: [showcase](#showcase)) You can find these crates in the
-`crates` folder. ## What is conda & conda-forge? The conda ecosystem provides
-**cross-platform**, **binary** packages that you can use with **any programming
-language**. `conda` is an open-source package management system and environment
-management system that can install and manage multiple versions of software
-packages and their dependencies. `conda` is written in Python. The aim of
-Rattler is to provide all functionality required to work with the conda
-ecosystem from Rust. Rattler is not a reimplementation of `conda`. `conda` is a
-package management tool. Rattler is a _library_ to work with the conda
-ecosystem from different languages and applications. For example, it powers the
-backend of https://prefix.dev. `conda-forge` is a community-driven effort to
-bring new and existing software into the conda ecosystem. It provides _tens-of-
-thousands of up-to-date_ packages that are maintained by a community of
-contributors. For an overview of available packages see https://prefix.dev.
+the crates above. * **rattler-lock**: a library to create and parse lockfiles
+for conda environments. * **rattler-networking**: common functionality for
+networking, like authentication, mirroring and more. * **rattler-bin**: an
+example of a package manager using all the crates above (see: [showcase]
+(#showcase)) You can find these crates in the `crates` folder. Additionally, we
+provide Python bindings for most of the functionalities provided by the above
+crates. A python package `py-rattler` is available on [conda-forge](https://
+prefix.dev/channels/conda-forge/packages/py-rattler) and [PyPI](https://
+pypi.org/project/py-rattler/). Documatation for the python bindings can be
+found [here](https://mamba-org.github.io/rattler/py-rattler). ## What is conda
+& conda-forge? The conda ecosystem provides **cross-platform**, **binary**
+packages that you can use with **any programming language**. `conda` is an
+open-source package management system and environment management system that
+can install and manage multiple versions of software packages and their
+dependencies. `conda` is written in Python. The aim of Rattler is to provide
+all functionality required to work with the conda ecosystem from Rust. Rattler
+is not a reimplementation of `conda`. `conda` is a package management tool.
+Rattler is a _library_ to work with the conda ecosystem from different
+languages and applications. For example, it powers the backend of https://
+prefix.dev. `conda-forge` is a community-driven effort to bring new and
+existing software into the conda ecosystem. It provides _tens-of-thousands of
+up-to-date_ packages that are maintained by a community of contributors. For an
+overview of available packages see https://prefix.dev.
```

