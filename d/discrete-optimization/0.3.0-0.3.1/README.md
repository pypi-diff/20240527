# Comparing `tmp/discrete_optimization-0.3.0.tar.gz` & `tmp/discrete_optimization-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discrete_optimization-0.3.0.tar", last modified: Fri May  3 16:06:56 2024, max compression
+gzip compressed data, was "discrete_optimization-0.3.1.tar", last modified: Mon May 27 14:44:40 2024, max compression
```

## Comparing `discrete_optimization-0.3.0.tar` & `discrete_optimization-0.3.1.tar`

### file list

```diff
@@ -1,507 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.985409 discrete_optimization-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.997409 discrete_optimization-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/.github/workflows/build-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16684 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/.github/workflows/deploy-doc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.997409 discrete_optimization-0.3.0/binder/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/binder/apt.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/binder/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/binder/postBuild
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/binder/start
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/credits.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.997409 discrete_optimization-0.3.0/discrete_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.997409 discrete_optimization-0.3.0/discrete_optimization/coloring/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.001409 discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_clique.mzn
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_for_lns.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_subset_nodes.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.001409 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_asp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_lns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_lns_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cpsat_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_lp_lns_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18495 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_lp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_solver_with_starting_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_toulbar_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/greedy_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.001409 discrete_optimization-0.3.0/discrete_optimization/facility/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/facility_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/facility_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/facility_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.001409 discrete_optimization-0.3.0/discrete_optimization/facility/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/minizinc/facility_int.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/minizinc/facility_int_lns.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.005409 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6761 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_cp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_lp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    20455 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_lp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/gphh_facility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/facility/solvers/greedy_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.005409 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/generic_rcpsp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    23073 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/gphh_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/graph_tools_rcpsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/large_neighborhood_search_scheduling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/ls_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    27888 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/neighbor_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    70708 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/neighbor_tools_rcpsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/postpro_local_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/solution_repair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.009409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/asp_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.009409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/early_stoppers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/loggers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)    12741 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/cp_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25765 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.009409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/alternating_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/deap_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19249 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/ga_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/nsga.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ghh_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/graph_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.009409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/hyperparameter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/hyperparametrizable.py
--rw-r--r--   0 runner    (1001) docker     (127)    23640 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/lns_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/lns_mip.py
--rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/lp_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.009409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/hill_climber.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/local_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/simulated_annealing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mip/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mip/pymip_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mixed_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_integer.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/permutation_mutations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/optuna/
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/optuna/timed_percentile_pruner.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/ortools_cpsat_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/path_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/pytools/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/pytools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/pytools/timeout_decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/multiobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/result_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8389 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/resultcomparator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/generic_tools/robustness/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/robustness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/generic_tools/robustness/robustness_tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/knapsack/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.013409 discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/knapsack_global.mzn
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/knapsack_mzn.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/multidim_multiscenario_knapsack.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/multidimension_knapsack.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/knapsack/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/mutation/mutation_knapsack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/cp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/dyn_prog_knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/gphh_knapsack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/greedy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_asp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_cpmpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_cpsat_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_lns_cp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/lp_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/builders/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/builders/instance_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    30837 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/gpdp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp.mzn
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp_example.dzn
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp_flow.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp_resources.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.017409 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/plots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/plots/gpdp_plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.021409 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   103658 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/lp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    58969 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/lp_solver_pymip.py
--rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/ortools_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/pickup_vrp_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.021409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58841 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/fast_function_rcpsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.025409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative_reif.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/mrcpsp_mode_satisfy.mzn
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/my_cumulative.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_calendar.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_no_bool.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive_calendar.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_with_faketasks.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_resource_feasibility_mzn.mzn
--rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multiscenario.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_mzn_calendar_boxes.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_no_search.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive_calendar.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_with_second_optim.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_resource.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/resumee_rcpsp.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.025409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/mutations/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/mutations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/mutations/mutation_rcpsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.025409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20249 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/plots/rcpsp_utils_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)    38623 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    55482 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_model_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    52689 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)     8983 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/robust_rcpsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/sgs_without_array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.029409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_lns_methods_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    51928 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_lns_methods_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_model_input.py
--rw-r--r--   0 runner    (1001) docker     (127)   112690 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7511 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_solvers_multiscenario.py
--rw-r--r--   0 runner    (1001) docker     (127)    27339 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cpm.py
--rw-r--r--   0 runner    (1001) docker     (127)    24339 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cpsat_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    25883 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_cp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_ga_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    40928 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    18546 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_solver_gantt.py
--rw-r--r--   0 runner    (1001) docker     (127)    25284 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_pile.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/special_constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.029409 discrete_optimization-0.3.0/discrete_optimization/rcpsp/specialized_rcpsp/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/specialized_rcpsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59744 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/specialized_rcpsp/rcpsp_specialized_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp/transform_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.029409 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64776 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/fast_function_ms_rcpsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.033409 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative_reif.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_compute_workers_for_tasks.mzn
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource.mzn
--rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource_nomultitasking.mzn
--rw-r--r--   0 runner    (1001) docker     (127)    16161 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive.mzn
--rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive_partially_preemptive.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/mspsp.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/mspsp_compatible_all_solvers.mzn
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/my_cumulative.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ressource_allocation_mspsp.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/multiskill_to_rcpsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.033409 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14883 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/plots/plot_solution.py
--rw-r--r--   0 runner    (1001) docker     (127)   154045 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mslib_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mspsp_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28730 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/calendar_solver_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     9655 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/cp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/cp_solver_mspsp_instlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    86656 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/cp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/lns_post_process_rcpsp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/lp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_cp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_ga_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_lp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/multimode_transposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/solver_rcpsp_based.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/common_tools_tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/tsp/minizinc/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/minizinc/tsp_float.mzn
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/minizinc/tsp_int.mzn
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/tsp/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/mutation/mutation_tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/tsp/plots/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/plots/plot_tsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/solver_lp_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/solver_ortools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/tsp_cp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/solver/tsp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_solvers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.037409 discrete_optimization-0.3.0/discrete_optimization/vrp/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/discrete_optimization/vrp/mutation/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/mutation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/mutation/mutation_vrp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/greedy_vrp.py
--rw-r--r--   0 runner    (1001) docker     (127)    45065 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/lp_vrp_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/lp_vrp_iterative_pymip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/solver_ortools.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/solver/vrp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_toolbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/discrete_optimization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-03 16:06:55.000000 discrete_optimization-0.3.0/discrete_optimization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21201 2024-05-03 16:06:55.000000 discrete_optimization-0.3.0/discrete_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:06:55.000000 discrete_optimization-0.3.0/discrete_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-03 16:06:55.000000 discrete_optimization-0.3.0/discrete_optimization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-03 16:06:55.000000 discrete_optimization-0.3.0/discrete_optimization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/generate_nb_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/_static/versions.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/_templates/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.041409 discrete_optimization-0.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/api/modules.md
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/contribute.md
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/getting_started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/docs/source/notebooks.template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.993409 discrete_optimization-0.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.045409 discrete_optimization-0.3.0/examples/coloring/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/coloring_asp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/coloring_cpspat_solver_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/coloring_gurobi_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/coloring_run_all_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/optuna_all_solvers_coloring_with_pruning_based_on_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/optuna_all_solvers_coloring_without_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/optuna_full_example_all_solvers_timed_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/optuna_full_example_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/coloring/toulbar_coloring_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.045409 discrete_optimization-0.3.0/examples/facility/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/facility/gphh_facility_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.045409 discrete_optimization-0.3.0/examples/knapsack/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/knapsack_asp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/knapsack_cpmpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/knapsack_cpsat_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/knapsack_decomposition_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/knapsack_multidimensional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/multiscenario_knap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/optuna_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/knapsack/solvers_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/pickup_vrp/
--rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/classic_ortools_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/cp_solver_gpdp_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/linear_flow_solver_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/loading_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/optuna_full_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4_auto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/pickup_vrp/plots_wip/
--rw-r--r--   0 runner    (1001) docker     (127)    29684 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/plots_wip/animated_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/pickup_vrp/time_windows_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/rcpsp/
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_cpsat_solver_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_lns_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna_multiobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna_with_pruning.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_lp_cplex_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_pareto_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/rcpsp_solvers_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp/robustness_experiments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/rcpsp_multiskill/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/rcpsp_multiskill/mslib/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp_multiskill/mslib/mslib_parse_and_solve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/rcpsp_multiskill/mspsp/
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp_multiskill/mspsp/mspsp_parse_and_solve.py
--rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp_multiskill/sgs_runs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/rcpsp_multiskill/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)    18015 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/rcpsp_multiskill/solvers/rcpsp_multiskills_runs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/examples/vrp/
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/examples/vrp/vrp_solver_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.049409 discrete_optimization-0.3.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/Knapsack tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-1 Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-2 Heuristics Solving.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20659 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-3 Local search.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-4 Linear programming.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-5 Constraint Programming.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-6 Large Neighbourhood Search .ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/notebooks/img/
--rw-r--r--   0 runner    (1001) docker     (127)   359364 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/img/sgs.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/notebooks/z_Advanced/
--rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/z_Advanced/callbacks.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/notebooks/z_Advanced/optuna.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/scripts/trigger_binder.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/coloring/
--rw-r--r--   0 runner    (1001) docker     (127)    15824 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/coloring/test_coloring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/facility/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_greedy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_lp_lns.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/facility/test_facility_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/generic_rcpsp_tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_rcpsp_tools/test_graph_tools_rcpsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/generic_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/generic_tools/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/callbacks/test_ortools_with_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/callbacks/test_sa_with_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/generic_tools/ea/
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/ea/test_ga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.053408 discrete_optimization-0.3.0/tests/generic_tools/hyperparameters/
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/hyperparameters/test_hyperparameter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.057409 discrete_optimization-0.3.0/tests/generic_tools/mutations/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/mutations/test_bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/generic_tools/test_multiobj_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.057409 discrete_optimization-0.3.0/tests/knapsack/
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cpmyp.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cpsat_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_decomposition_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_gphh.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_greedy_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_lns_cp_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_lp_lns_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_ls_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_nsga.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_knapsack_solvers.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/knapsack/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:55.993409 discrete_optimization-0.3.0/tests/pickup_vrp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.057409 discrete_optimization-0.3.0/tests/pickup_vrp/builders/
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/pickup_vrp/builders/test_instance_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/pickup_vrp/builders/test_linear_flow_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/pickup_vrp/builders/test_linear_flow_solver_pymip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.057409 discrete_optimization-0.3.0/tests/pickup_vrp/solvers/
--rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/pickup_vrp/solvers/test_ortools_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.061409 discrete_optimization-0.3.0/tests/rcpsp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.061409 discrete_optimization-0.3.0/tests/rcpsp/solver/
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_large_neighborhood_search_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5964 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cp_lns.py
--rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cpm.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_find_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_local_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_lp_lns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_pile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_resource_optim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_distance_between_solutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_model_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_nsga.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)    46394 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_uncertain_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp/test_sgs_without_array.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.061409 discrete_optimization-0.3.0/tests/rcpsp_multiskill/
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_mspsp_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11519 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_lp_lns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_partially_preemptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_rcpsp_based_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_to_rcpsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/show_do_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/test_import_all_submodules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/tests/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_common_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_lp_iterative.py
--rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_mutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/tsp/test_tsp_ortools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:06:56.065409 discrete_optimization-0.3.0/tests/vrp/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-03 16:06:46.000000 discrete_optimization-0.3.0/tests/vrp/test_vrp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.769585 discrete_optimization-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.677585 discrete_optimization-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.689585 discrete_optimization-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/.github/workflows/build-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/.github/workflows/deploy-doc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-27 14:44:40.769585 discrete_optimization-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.693585 discrete_optimization-0.3.1/binder/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/binder/apt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/binder/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/binder/postBuild
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/binder/start
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/credits.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.693585 discrete_optimization-0.3.1/discrete_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.693585 discrete_optimization-0.3.1/discrete_optimization/coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16740 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.697585 discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_clique.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_for_lns.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_subset_nodes.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.697585 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_asp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_lns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_lns_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cpsat_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_lp_lns_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18495 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_lp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_solver_with_starting_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_toulbar_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/greedy_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11946 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.697585 discrete_optimization-0.3.1/discrete_optimization/facility/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10145 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/facility_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/facility_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/facility_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.701585 discrete_optimization-0.3.1/discrete_optimization/facility/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/minizinc/facility_int.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/minizinc/facility_int_lns.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.701585 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_cp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_lp_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20455 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_lp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12784 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/gphh_facility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/facility/solvers/greedy_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.701585 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/generic_rcpsp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23073 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/gphh_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/graph_tools_rcpsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25700 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/large_neighborhood_search_scheduling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/ls_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27888 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/neighbor_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72538 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/neighbor_tools_rcpsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/postpro_local_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/solution_repair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.705585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/asp_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.705585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/early_stoppers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/loggers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/cp_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25765 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/alternating_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/deap_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19961 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5184 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/ga_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16770 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/nsga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ghh_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/graph_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/hyperparameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9755 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/hyperparametrizable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28559 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/lns_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/lns_mip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/lp_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10307 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/hill_climber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/local_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/simulated_annealing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mip/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mip/pymip_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mixed_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/permutation_mutations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/optuna/
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/optuna/timed_percentile_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/ortools_cpsat_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/path_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.709585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/pytools/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/pytools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/pytools/timeout_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/qiskit_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.713585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/multiobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12740 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/result_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/resultcomparator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.713585 discrete_optimization-0.3.1/discrete_optimization/generic_tools/robustness/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/robustness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/generic_tools/robustness/robustness_tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.713585 discrete_optimization-0.3.1/discrete_optimization/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18072 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.713585 discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/knapsack_global.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/knapsack_mzn.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/multidim_multiscenario_knapsack.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/multidimension_knapsack.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.713585 discrete_optimization-0.3.1/discrete_optimization/knapsack/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/mutation/mutation_knapsack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/cp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/dyn_prog_knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/gphh_knapsack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/greedy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_asp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_cpmpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_cpsat_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_lns_cp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/lp_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/mis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/mis_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/mis_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/mis_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/mis_gurobi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/mis_kamis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/mis_ortools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/mis_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/maximum_independent_set/solvers/mis_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22082 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/builders/instance_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30837 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/gpdp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp_example.dzn
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp_flow.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8612 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp_resources.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.717585 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/plots/gpdp_plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.721585 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103658 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/lp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58969 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/lp_solver_pymip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/ortools_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/pickup_vrp_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.721585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58841 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/fast_function_rcpsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.725585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative_reif.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/mrcpsp_mode_satisfy.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/my_cumulative.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8703 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_calendar.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_no_bool.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8678 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive_calendar.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_with_faketasks.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_resource_feasibility_mzn.mzn
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6803 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multiscenario.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_mzn_calendar_boxes.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_no_search.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive_calendar.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_with_second_optim.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_resource.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/resumee_rcpsp.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.725585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/mutations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6094 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/mutations/mutation_rcpsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.725585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20336 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/plots/rcpsp_utils_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38623 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55482 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_model_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52689 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7928 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/robust_rcpsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/sgs_without_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.729585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_lns_methods_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_model_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)   112835 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7968 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_solvers_multiscenario.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27339 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24650 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cpsat_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_cp_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_ga_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19028 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41188 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_solver_gantt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25711 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/special_constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.729585 discrete_optimization-0.3.1/discrete_optimization/rcpsp/specialized_rcpsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/specialized_rcpsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59744 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/specialized_rcpsp/rcpsp_specialized_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp/transform_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.733585 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64776 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/fast_function_ms_rcpsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.733585 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative_reif.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_compute_workers_for_tasks.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)    10459 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource_nomultitasking.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)    16161 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)    18666 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive_partially_preemptive.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/mspsp.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     6698 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/mspsp_compatible_all_solvers.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/my_cumulative.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ressource_allocation_mspsp.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     7131 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/multiskill_to_rcpsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.733585 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14990 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/plots/plot_solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154045 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mslib_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4012 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mspsp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/cp_solver_mspsp_instlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86656 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/cp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/lns_post_process_rcpsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14705 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/lp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_ga_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_lp_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/multimode_transposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/solver_rcpsp_based.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/common_tools_tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/tsp/minizinc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/minizinc/tsp_float.mzn
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/minizinc/tsp_int.mzn
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/tsp/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/mutation/mutation_tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/tsp/plots/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/plots/plot_tsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.737585 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/solver_lp_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/solver_ortools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/tsp_cp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/solver/tsp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15826 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/discrete_optimization/vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/discrete_optimization/vrp/mutation/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/mutation/mutation_vrp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/greedy_vrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45065 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/lp_vrp_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/lp_vrp_iterative_pymip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8296 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/solver_ortools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/solver/vrp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_toolbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.765585 discrete_optimization-0.3.1/discrete_optimization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-05-27 14:44:40.000000 discrete_optimization-0.3.1/discrete_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21635 2024-05-27 14:44:40.000000 discrete_optimization-0.3.1/discrete_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:44:40.000000 discrete_optimization-0.3.1/discrete_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 14:44:40.000000 discrete_optimization-0.3.1/discrete_optimization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 14:44:40.000000 discrete_optimization-0.3.1/discrete_optimization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10191 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/generate_nb_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/_static/versions.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/_templates/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.741585 discrete_optimization-0.3.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/api/modules.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12680 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/docs/source/notebooks.template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.685585 discrete_optimization-0.3.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.745585 discrete_optimization-0.3.1/examples/coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/coloring_asp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/coloring_cpspat_solver_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/coloring_gurobi_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/coloring_run_all_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/optuna_all_solvers_coloring_with_pruning_based_on_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/optuna_all_solvers_coloring_without_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/optuna_full_example_all_solvers_timed_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/optuna_full_example_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/coloring/toulbar_coloring_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.745585 discrete_optimization-0.3.1/examples/facility/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/facility/gphh_facility_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.745585 discrete_optimization-0.3.1/examples/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/knapsack_asp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/knapsack_cpmpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/knapsack_cpsat_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/knapsack_decomposition_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/knapsack_multidimensional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/multiscenario_knap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6045 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/optuna_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/knapsack/solvers_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.745585 discrete_optimization-0.3.1/examples/maximum_independent_set/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/maximum_independent_set/qiskit_application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/pickup_vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)    11815 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/classic_ortools_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53464 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/cp_solver_gpdp_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/linear_flow_solver_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10605 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/loading_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/optuna_full_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4_auto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/pickup_vrp/plots_wip/
+-rw-r--r--   0 runner    (1001) docker     (127)    29684 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/plots_wip/animated_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/pickup_vrp/time_windows_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/rcpsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_cpsat_solver_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_lns_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna_multiobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna_with_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_lp_cplex_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7890 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_pareto_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/rcpsp_solvers_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15565 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp/robustness_experiments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/rcpsp_multiskill/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/rcpsp_multiskill/mslib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp_multiskill/mslib/mslib_parse_and_solve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/rcpsp_multiskill/mspsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp_multiskill/mspsp/mspsp_parse_and_solve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8028 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp_multiskill/sgs_runs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/rcpsp_multiskill/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)    18015 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/rcpsp_multiskill/solvers/rcpsp_multiskills_runs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/examples/vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/examples/vrp/vrp_solver_example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.749585 discrete_optimization-0.3.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/Knapsack tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)    17801 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-1 Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-2 Heuristics Solving.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20659 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-3 Local search.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9498 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-4 Linear programming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    10066 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-5 Constraint Programming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13381 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-6 Large Neighbourhood Search .ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/notebooks/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   359364 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/img/sgs.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/notebooks/z_Advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)    16216 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/z_Advanced/callbacks.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    28862 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/notebooks/z_Advanced/optuna.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/scripts/trigger_binder.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:44:40.769585 discrete_optimization-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/tests/coloring/
+-rw-r--r--   0 runner    (1001) docker     (127)    16344 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/coloring/test_coloring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/tests/facility/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_lp_lns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/facility/test_facility_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.753585 discrete_optimization-0.3.1/tests/generic_rcpsp_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_rcpsp_tools/test_graph_tools_rcpsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/generic_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/generic_tools/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/callbacks/test_ortools_with_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11175 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/callbacks/test_sa_with_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/generic_tools/ea/
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/ea/test_ga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/generic_tools/hyperparameters/
+-rw-r--r--   0 runner    (1001) docker     (127)    11061 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/hyperparameters/test_hyperparameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/generic_tools/mutations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/mutations/test_bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/generic_tools/test_multiobj_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cpmyp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cpsat_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_decomposition_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_gphh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_greedy_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6427 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_lns_cp_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2672 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_lp_lns_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_ls_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_nsga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_knapsack_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/knapsack/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.757585 discrete_optimization-0.3.1/tests/maximum_independent_set/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/maximum_independent_set/test_maximum_independent_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.689585 discrete_optimization-0.3.1/tests/pickup_vrp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.761585 discrete_optimization-0.3.1/tests/pickup_vrp/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_instance_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_linear_flow_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9235 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_linear_flow_solver_pymip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.761585 discrete_optimization-0.3.1/tests/pickup_vrp/solvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/pickup_vrp/solvers/test_ortools_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.761585 discrete_optimization-0.3.1/tests/rcpsp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.761585 discrete_optimization-0.3.1/tests/rcpsp/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_large_neighborhood_search_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10987 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_cpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_find_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_local_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_lp_lns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_resource_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_distance_between_solutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_model_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_nsga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46394 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_uncertain_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp/test_sgs_without_array.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.765585 discrete_optimization-0.3.1/tests/rcpsp_multiskill/
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_mspsp_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_lp_lns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_partially_preemptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_rcpsp_based_solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_to_rcpsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/show_do_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/test_import_all_submodules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.765585 discrete_optimization-0.3.1/tests/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_common_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_lp_iterative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/tsp/test_tsp_ortools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:44:40.765585 discrete_optimization-0.3.1/tests/vrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-27 14:44:29.000000 discrete_optimization-0.3.1/tests/vrp/test_vrp_solver.py
```

### Comparing `discrete_optimization-0.3.0/.github/workflows/build-doc.yml` & `discrete_optimization-0.3.1/.github/workflows/build-doc.yml`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/.github/workflows/build.yml` & `discrete_optimization-0.3.1/.github/workflows/build.yml`

 * *Files 1% similar despite different names*

```diff
@@ -154,19 +154,19 @@
           cache: "pip"
           cache-dependency-path: pyproject.toml
       - name: Download artifacts
         uses: actions/download-artifact@v4
         with:
           name: dist
           path: dist
-      - name: Install prerelease version of pymip (only for macos arm64)
-        if: matrix.os == 'macos-latest'
+      - name: Prevent installing newest release or ortools on windows (segmentation fault)
+        if: matrix.os == 'windows-latest'
         run: |
           python -m pip install -U pip
-          pip install mip==1.16rc0
+          pip install "ortools<9.10"
       - name: Install only discrete-optimization
         run: |
           python -m pip install -U pip
           wheelfile=$(ls ./dist/discrete_optimization*.whl)
           pip install ${wheelfile}
       - name: Check import work without minizinc if DO_SKIP_MZN_CHECK set
         run: |
```

### Comparing `discrete_optimization-0.3.0/.github/workflows/deploy-doc.yml` & `discrete_optimization-0.3.1/.github/workflows/deploy-doc.yml`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/.pre-commit-config.yaml` & `discrete_optimization-0.3.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/LICENSE` & `discrete_optimization-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/PKG-INFO` & `discrete_optimization-0.3.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-optimization
-Version: 0.3.0
+Version: 0.3.1
 Summary: Discrete optimization library
 Author-email: Airbus AI Research <scikit-decide@airbus.com>
 License: MIT
 Project-URL: documentation, https://airbus.github.io/discrete-optimization
 Project-URL: repository, https://github.com/airbus/discrete-optimization
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,17 @@
 Requires-Dist: typing-extensions>=4.0
 Requires-Dist: cpmpy>=0.9.9
 Requires-Dist: scipy
 Requires-Dist: numpy>=1.21
 Requires-Dist: typing_extensions>=4.4
 Requires-Dist: clingo>=5.6
 Requires-Dist: setuptools
+Requires-Dist: qiskit>=1.0.2
+Requires-Dist: qiskit-algorithms>=0.3.0
+Requires-Dist: qiskit-optimization>=0.6.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scikit-learn>=1.0; extra == "test"
 Requires-Dist: optuna; extra == "test"
 
 # Discrete Optimization
```

### Comparing `discrete_optimization-0.3.0/README.md` & `discrete_optimization-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/binder/start` & `discrete_optimization-0.3.1/binder/start`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/credits.md` & `discrete_optimization-0.3.1/credits.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/__init__.py` & `discrete_optimization-0.3.1/discrete_optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_model.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_plot.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_plot.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/coloring_toolbox.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/coloring_toolbox.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring.mzn` & `discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_clique.mzn` & `discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_clique.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_for_lns.mzn` & `discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_for_lns.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/minizinc/coloring_subset_nodes.mzn` & `discrete_optimization-0.3.1/discrete_optimization/coloring/minizinc/coloring_subset_nodes.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_asp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_asp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_lns.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_lns.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,24 +14,29 @@
 )
 from discrete_optimization.coloring.solvers.coloring_cp_solvers import (
     ColoringCP,
     ColoringCPModel,
 )
 from discrete_optimization.coloring.solvers.coloring_solver import SolverColoring
 from discrete_optimization.generic_tools.callbacks.callback import Callback
-from discrete_optimization.generic_tools.cp_tools import ParametersCP
+from discrete_optimization.generic_tools.cp_tools import MinizincCPSolver, ParametersCP
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
 from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
     SubBrickHyperparameter,
     SubBrickKwargsHyperparameter,
 )
 from discrete_optimization.generic_tools.lns_cp import (
     LNS_CP,
+    ConstraintHandler,
     TrivialPostProcessSolution,
 )
+from discrete_optimization.generic_tools.lns_mip import (
+    InitialSolution,
+    PostProcessSolution,
+)
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 
 
 def build_default_cp_model(coloring_model: ColoringProblem, **kwargs):
     cp_model = ColoringCP(problem=coloring_model, **kwargs)
@@ -69,159 +74,106 @@
     return InitialColoring(
         problem=coloring_model,
         initial_method=InitialColoringMethod.GREEDY,
         params_objective_function=params_objective_function,
     )
 
 
-class LnsCpColoring(SolverColoring):
+class LnsCpColoring(LNS_CP, SolverColoring):
     """
     Most easy way to use LNS-CP for coloring with some default parameters for constraint handler.
     """
 
-    hyperparameters = [
-        SubBrickHyperparameter("cp_solver_cls", choices=[ColoringCP], default=None),
-        SubBrickKwargsHyperparameter(
-            "cp_solver_kwargs", subbrick_hyperparameter="cp_solver_cls"
-        ),
-        SubBrickHyperparameter(
-            "initial_solution_provider_cls", choices=[InitialColoring], default=None
-        ),
-        SubBrickKwargsHyperparameter(
-            "initial_solution_provider_kwargs",
-            subbrick_hyperparameter="initial_solution_provider_cls",
-        ),
-        SubBrickHyperparameter(
-            "constraint_handler_cls",
-            choices=[ConstraintHandlerFixColorsCP],
-            default=None,
+    hyperparameters = LNS_CP.copy_and_update_hyperparameters(
+        cp_solver_cls=dict(choices=[ColoringCP]),
+        initial_solution_provider_cls=dict(choices=[InitialColoring]),
+        constraint_handler_cls=dict(choices=[ConstraintHandlerFixColorsCP]),
+        post_process_solution_cls=dict(
+            choices=[TrivialPostProcessSolution, PostProcessSolutionColoring]
         ),
-        SubBrickKwargsHyperparameter(
-            "constraint_handler_kwargs",
-            subbrick_hyperparameter="constraint_handler_cls",
-        ),
-        SubBrickHyperparameter(
-            "post_process_solution_cls",
-            choices=[TrivialPostProcessSolution, PostProcessSolutionColoring],
-            default=None,
-        ),
-        SubBrickKwargsHyperparameter(
-            "post_process_solution_kwargs",
-            subbrick_hyperparameter="post_process_solution_cls",
-        ),
-    ]
+    )
 
     def __init__(
         self,
         problem: ColoringProblem,
+        cp_solver: Optional[MinizincCPSolver] = None,
+        initial_solution_provider: Optional[InitialSolution] = None,
+        constraint_handler: Optional[ConstraintHandler] = None,
+        post_process_solution: Optional[PostProcessSolution] = None,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs
     ):
-        super().__init__(
-            problem=problem, params_objective_function=params_objective_function
+        SolverColoring.__init__(
+            self, problem=problem, params_objective_function=params_objective_function
         )
-
         kwargs = self.complete_with_default_hyperparameters(kwargs)
 
-        solver = kwargs.get("cp_solver", None)
-        if solver is None:
+        if cp_solver is None:
             if kwargs["cp_solver_kwargs"] is None:
                 cp_solver_kwargs = kwargs
             else:
                 cp_solver_kwargs = kwargs["cp_solver_kwargs"]
             if kwargs["cp_solver_cls"] is None:
-                solver = build_default_cp_model(
+                cp_solver = build_default_cp_model(
                     coloring_model=self.problem, **cp_solver_kwargs
                 )
             else:
                 cp_solver_cls = kwargs["cp_solver_cls"]
-                solver = cp_solver_cls(problem=self.problem, **cp_solver_kwargs)
-                solver.init_model(**cp_solver_kwargs)
-        self.cp_solver = solver
-
-        self.parameters_cp = kwargs.get("parameters_cp", ParametersCP.default())
+                cp_solver = cp_solver_cls(problem=self.problem, **cp_solver_kwargs)
+                cp_solver.init_model(**cp_solver_kwargs)
+        self.cp_solver = cp_solver
 
-        self.constraint_handler = kwargs.get("constraint_handler", None)
-        if self.constraint_handler is None:
+        if constraint_handler is None:
             if kwargs["constraint_handler_kwargs"] is None:
                 constraint_handler_kwargs = kwargs
             else:
                 constraint_handler_kwargs = kwargs["constraint_handler_kwargs"]
             if kwargs["constraint_handler_cls"] is None:
-                self.constraint_handler = build_default_constraint_handler(
+                constraint_handler = build_default_constraint_handler(
                     coloring_model=self.problem, **constraint_handler_kwargs
                 )
             else:
                 constraint_handler_cls = kwargs["constraint_handler_cls"]
-                self.constraint_handler = constraint_handler_cls(
+                constraint_handler = constraint_handler_cls(
                     problem=self.problem, **constraint_handler_kwargs
                 )
+        self.constraint_handler = constraint_handler
 
-        self.post_pro = kwargs.get("post_process_solution", None)
-        if self.post_pro is None:
+        if post_process_solution is None:
             if kwargs["post_process_solution_kwargs"] is None:
                 post_process_solution_kwargs = kwargs
             else:
                 post_process_solution_kwargs = kwargs["post_process_solution_kwargs"]
             if kwargs["post_process_solution_cls"] is None:
-                self.post_pro = build_default_postprocess(
+                post_process_solution = build_default_postprocess(
                     coloring_model=self.problem,
                     params_objective_function=self.params_objective_function,
                 )
             else:
                 post_process_solution_cls = kwargs["post_process_solution_cls"]
-                self.post_pro = post_process_solution_cls(
+                post_process_solution = post_process_solution_cls(
                     problem=self.problem,
                     params_objective_function=self.params_objective_function,
                     **post_process_solution_kwargs
                 )
+        self.post_process_solution = post_process_solution
 
-        self.initial_solution_provider = kwargs.get("initial_solution_provider", None)
-        if self.initial_solution_provider is None:
+        if initial_solution_provider is None:
             if kwargs["initial_solution_provider_kwargs"] is None:
                 initial_solution_provider_kwargs = kwargs
             else:
                 initial_solution_provider_kwargs = kwargs[
                     "initial_solution_provider_kwargs"
                 ]
             if kwargs["initial_solution_provider_cls"] is None:
-                self.initial_solution_provider = build_default_initial_solution(
+                initial_solution_provider = build_default_initial_solution(
                     coloring_model=self.problem,
                     params_objective_function=self.params_objective_function,
                 )
             else:
                 initial_solution_provider_cls = kwargs["initial_solution_provider_cls"]
-                self.initial_solution_provider = initial_solution_provider_cls(
+                initial_solution_provider = initial_solution_provider_cls(
                     problem=self.problem,
                     params_objective_function=self.params_objective_function,
                     **initial_solution_provider_kwargs
                 )
-
-        self.lns_solver = LNS_CP(
-            problem=self.problem,
-            cp_solver=self.cp_solver,
-            initial_solution_provider=self.initial_solution_provider,
-            constraint_handler=self.constraint_handler,
-            post_process_solution=self.post_pro,
-            params_objective_function=self.params_objective_function,
-        )
-
-    def solve(
-        self,
-        nb_iteration_lns: int,
-        parameters_cp: Optional[ParametersCP] = None,
-        nb_iteration_no_improvement: Optional[int] = None,
-        skip_first_iteration: bool = False,
-        stop_first_iteration_if_optimal: bool = True,
-        callbacks: Optional[List[Callback]] = None,
-        **args
-    ) -> ResultStorage:
-        if parameters_cp is None:
-            parameters_cp = ParametersCP.default()
-        return self.lns_solver.solve_lns(
-            parameters_cp=parameters_cp,
-            skip_first_iteration=skip_first_iteration,
-            stop_first_iteration_if_optimal=stop_first_iteration_if_optimal,
-            nb_iteration_no_improvement=nb_iteration_no_improvement,
-            nb_iteration_lns=nb_iteration_lns,
-            callbacks=callbacks,
-        )
+        self.initial_solution_provider = initial_solution_provider
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_lns_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_lns_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_cpsat_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_cpsat_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_lp_lns_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_lp_lns_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_lp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_lp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_solver_with_starting_solution.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_solver_with_starting_solution.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/coloring_toulbar_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/coloring_toulbar_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/coloring/solvers/greedy_coloring.py` & `discrete_optimization-0.3.1/discrete_optimization/coloring/solvers/greedy_coloring.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/datasets.py` & `discrete_optimization-0.3.1/discrete_optimization/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import glob
+import gzip
 import os
+import shutil
 import tempfile
 import zipfile
 from typing import Optional
 from urllib.request import urlcleanup, urlretrieve
 
 DO_DEFAULT_DATAHOME = "~/discrete_optimization_data"
 DO_DEFAULT_DATAHOME_ENVVARNAME = "DISCRETE_OPTIMIZATION_DATA"
@@ -39,14 +41,23 @@
 MSPSPLIB_REPO_URL = "https://github.com/youngkd/MSPSP-InstLib"
 MSPSPLIB_REPO_URL_SHA1 = "f77644175b84beed3bd365315412abee1a15eea1"
 
 
 MSLIB_DATASET_URL = "http://www.projectmanagement.ugent.be/sites/default/files/datasets/MSRCPSP/MSLIB.zip"
 MSLIB_DATASET_RELATIVE_PATH = "MSLIB.zip"
 
+MIS_FILES = [
+    "https://oeis.org/A265032/a265032_1dc.64.txt.gz",
+    "https://oeis.org/A265032/a265032_1dc.128.txt.gz",
+    "https://oeis.org/A265032/a265032_1dc.256.txt.gz",
+    "https://oeis.org/A265032/a265032_1dc.512.txt.gz",
+    "https://oeis.org/A265032/a265032_1dc.1024.txt.gz",
+    "https://oeis.org/A265032/a265032_1dc.2048.txt.gz",
+]
+
 
 def get_data_home(data_home: Optional[str] = None) -> str:
     """Return the path of the discrete-optimization data directory.
 
     This folder is used by some large dataset loaders to avoid downloading the
     data several times.
     By default the data dir is set to a folder named 'discrete_optimization_data' in the
@@ -258,23 +269,57 @@
             with zipfile.ZipFile(local_file_path) as zipf:
                 zipf.extractall(path=rcpsp_multiskill_dir)
     finally:
         # remove temporary files
         urlcleanup()
 
 
+def decompress_gz_to_folder(input_file, output_folder, url):
+    with gzip.open(input_file, "rb") as f_in:
+        # Get the base name of the gzipped file without the .gz extension
+        base_name = url[33:]
+        file_name = os.path.splitext(base_name)[0]
+        # Create the output folder if it doesn't exist
+        os.makedirs(output_folder, exist_ok=True)
+        # Construct the output file path for each extracted file
+        output_file = os.path.join(output_folder, f"{file_name}")
+        # Open the output file in write-binary mode ('wb')
+        with open(output_file, "wb") as f_out:
+            # Write the extracted file data to the output file
+            shutil.copyfileobj(f_in, f_out)
+
+
+def fetch_data_for_mis(data_home: Optional[str] = None):
+    #  get the proper data directory
+    data_home = get_data_home(data_home=data_home)
+
+    # get mis data directory
+    mis_dir = f"{data_home}/mis"
+    os.makedirs(mis_dir, exist_ok=True)
+
+    try:
+        # download each datasets
+        for url in MIS_FILES:
+            filename, _ = urlretrieve(url)
+            decompress_gz_to_folder(filename, mis_dir, url)
+    finally:
+        # remove temporary files
+        urlcleanup()
+
+
 def fetch_all_datasets(data_home: Optional[str] = None):
     """Fetch data used by examples for all packages.
 
     Params:
         data_home: Specify the cache folder for the datasets. By default
             all discrete-optimization data is stored in '~/discrete_optimization_data' subfolders.
 
     """
     fetch_data_from_coursera(data_home=data_home)
     fetch_data_from_psplib(data_home=data_home)
     fetch_data_from_imopse(data_home=data_home)
     fetch_data_from_solutionsupdate(data_home=data_home)
+    fetch_data_for_mis(data_home=data_home)
 
 
 if __name__ == "__main__":
     fetch_all_datasets()
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/facility_model.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/facility_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/facility_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/facility_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/facility_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/facility_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/minizinc/facility_int.mzn` & `discrete_optimization-0.3.1/discrete_optimization/facility/minizinc/facility_int.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/minizinc/facility_int_lns.mzn` & `discrete_optimization-0.3.1/discrete_optimization/facility/minizinc/facility_int_lns.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_cp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_cp_solvers.py`

 * *Files 15% similar despite different names*

```diff
@@ -148,32 +148,7 @@
                 and the computed variables as defined in minizinc model.
 
         Returns:
 
         """
         facility = kwargs["facility_for_customer"]
         return FacilitySolution(self.problem, [f - 1 for f in facility])
-
-    @deprecated(
-        deprecated_in="0.1", details="Use rather initial solution provider utilities"
-    )
-    def get_solution(self, **kwargs: Any) -> FacilitySolution:
-        greedy_start = kwargs.get("greedy_start", True)
-        if greedy_start:
-            logger.info("Computing greedy solution")
-            greedy_solver = GreedySolverDistanceBased(self.problem)
-            result = greedy_solver.solve()
-            solution = result.get_best_solution()
-            if solution is None:
-                raise RuntimeError(
-                    "greedy_solver.solve().get_best_solution() " "should not be None."
-                )
-            if not isinstance(solution, FacilitySolution):
-                raise RuntimeError(
-                    "greedy_solver.solve().get_best_solution() "
-                    "should be a FacilitySolution."
-                )
-        else:
-            logger.info("Get dummy solution")
-            solution = self.problem.get_dummy_solution()
-        logger.info("Greedy Done")
-        return solution
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_lp_lns_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_lp_lns_solver.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     GreedySolverFacility,
     ResultStorage,
 )
 from discrete_optimization.generic_tools.do_problem import (
     ParamsObjectiveFunction,
     build_aggreg_function_and_params_objective,
 )
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    EnumHyperparameter,
+)
 from discrete_optimization.generic_tools.lns_mip import (
     ConstraintHandler,
     InitialSolution,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -43,14 +46,21 @@
     """Initial solution provider for lns algorithm.
 
     Attributes:
         problem (FacilityProblem): input coloring problem
         initial_method (InitialFacilityMethod): the method to use to provide the initial solution.
     """
 
+    hyperparameters = [
+        EnumHyperparameter(
+            name="initial_method",
+            enum=InitialFacilityMethod,
+        ),
+    ]
+
     def __init__(
         self,
         problem: FacilityProblem,
         initial_method: InitialFacilityMethod,
         params_objective_function: ParamsObjectiveFunction,
     ):
         self.problem = problem
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/solvers/facility_lp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/solvers/facility_lp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/solvers/gphh_facility.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/solvers/gphh_facility.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/facility/solvers/greedy_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/facility/solvers/greedy_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/gphh_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/gphh_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/graph_tools_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/graph_tools_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/large_neighborhood_search_scheduling.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/large_neighborhood_search_scheduling.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 from enum import Enum
-from typing import List, Optional
+from typing import Any, Optional
 
 import discrete_optimization.rcpsp.solver.rcpsp_cp_lns_solver as rcpsp_lns
 from discrete_optimization.generic_rcpsp_tools.generic_rcpsp_solver import (
     SolverGenericRCPSP,
 )
 from discrete_optimization.generic_rcpsp_tools.graph_tools_rcpsp import (
     build_graph_rcpsp_object,
@@ -32,21 +32,29 @@
     NeighborRandomAndNeighborGraph,
     ParamsConstraintBuilder,
 )
 from discrete_optimization.generic_rcpsp_tools.solution_repair import (
     NeighborRepairProblems,
 )
 from discrete_optimization.generic_rcpsp_tools.typing import ANY_RCPSP
-from discrete_optimization.generic_tools.callbacks.callback import Callback
-from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
+from discrete_optimization.generic_tools.cp_tools import CPSolverName, MinizincCPSolver
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
-from discrete_optimization.generic_tools.lns_cp import LNS_CP
-from discrete_optimization.generic_tools.lns_mip import InitialSolutionFromSolver
-from discrete_optimization.generic_tools.result_storage.result_storage import (
-    ResultStorage,
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    EnumHyperparameter,
+    FloatHyperparameter,
+    IntegerHyperparameter,
+    SubBrickHyperparameter,
+    SubBrickKwargsHyperparameter,
+)
+from discrete_optimization.generic_tools.lns_cp import LNS_CP, ConstraintHandler
+from discrete_optimization.generic_tools.lns_mip import (
+    InitialSolution,
+    InitialSolutionFromSolver,
+    PostProcessSolution,
 )
 from discrete_optimization.rcpsp.solver.cp_lns_methods_preemptive import (
     PostProLeftShift,
 )
 from discrete_optimization.rcpsp.solver.cp_solvers import (
     CP_MRCPSP_MZN,
     CP_MRCPSP_MZN_PREEMPTIVE,
@@ -96,15 +104,15 @@
                     if x
                     not in [
                         "nb_preemptive",
                         "max_preempted",
                         "fake_tasks",
                         "add_partial_solution_hard_constraint",
                     ]
-                }
+                },
             )
             return solver
     if rcpsp_problem.is_preemptive():
         if not rcpsp_problem.is_multiskill():
             if rcpsp_problem.is_rcpsp_multimode():
                 solver = CP_MRCPSP_MZN_PREEMPTIVE(
                     problem=rcpsp_problem,
@@ -130,15 +138,15 @@
                         if x
                         not in [
                             "nb_preemptive",
                             "max_preempted",
                             "fake_tasks",
                             "add_partial_solution_hard_constraint",
                         ]
-                    }
+                    },
                 )
                 return solver
             if not rcpsp_problem.is_rcpsp_multimode():
                 solver = CP_RCPSP_MZN_PREEMPTIVE(
                     problem=rcpsp_problem,
                     cp_solver_name=kwargs.get("cp_solver_name", CPSolverName.CHUFFED),
                 )
@@ -162,15 +170,15 @@
                         if x
                         not in [
                             "nb_preemptive",
                             "max_preempted",
                             "fake_tasks",
                             "add_partial_solution_hard_constraint",
                         ]
-                    }
+                    },
                 )
                 return solver
     if not rcpsp_problem.is_preemptive():
         if rcpsp_problem.is_multiskill():
             solver = CP_MS_MRCPSP_MZN(
                 problem=rcpsp_problem,
                 cp_solver_name=kwargs.get("cp_solver_name", CPSolverName.CHUFFED),
@@ -185,15 +193,15 @@
                 add_partial_solution_hard_constraint=kwargs.get(
                     "add_partial_solution_hard_constraint", False
                 ),
                 **{
                     x: kwargs[x]
                     for x in kwargs
                     if x not in ["add_partial_solution_hard_constraint"]
-                }
+                },
             )
             return solver
         if not rcpsp_problem.is_multiskill():
             if rcpsp_problem.is_rcpsp_multimode():
                 solver = CP_MRCPSP_MZN(
                     problem=rcpsp_problem,
                     cp_solver_name=kwargs.get("cp_solver_name", CPSolverName.CHUFFED),
@@ -204,15 +212,15 @@
                     add_partial_solution_hard_constraint=kwargs.get(
                         "add_partial_solution_hard_constraint", False
                     ),
                     **{
                         x: kwargs[x]
                         for x in kwargs
                         if x not in ["add_partial_solution_hard_constraint"]
-                    }
+                    },
                 )
                 return solver
             if not rcpsp_problem.is_rcpsp_multimode():
                 solver = CP_RCPSP_MZN(
                     problem=rcpsp_problem,
                     cp_solver_name=kwargs.get("cp_solver_name", CPSolverName.CHUFFED),
                 )
@@ -222,15 +230,15 @@
                     add_partial_solution_hard_constraint=kwargs.get(
                         "add_partial_solution_hard_constraint", False
                     ),
                     **{
                         x: kwargs[x]
                         for x in kwargs
                         if x not in ["add_partial_solution_hard_constraint"]
-                    }
+                    },
                 )
                 return solver
 
 
 def build_default_postpro(rcpsp_problem: ANY_RCPSP, partial_solution=None, **kwargs):
     if not rcpsp_problem.is_multiskill():
         if rcpsp_problem.is_preemptive():
@@ -303,59 +311,77 @@
                 list_neighbor=[n1, n2], weight_neighbor=[0.5, 0.5]
             )
         basic_constraint_builder = BasicConstraintBuilder(
             neighbor_builder=n_mix,
             preemptive=kwargs.get("preemptive", False),
             multiskill=kwargs.get("multiskill", False),
         )
-        params_list = kwargs.get(
-            "params_list",
-            [
-                ParamsConstraintBuilder(
+        if "params_list" in kwargs:
+            params_list = kwargs["params_list"]
+        else:
+            if kwargs["params_0_kwargs"] is None:
+                params_0 = ParamsConstraintBuilder(
                     minus_delta_primary=6000,
                     plus_delta_primary=6000,
                     minus_delta_secondary=400,
                     plus_delta_secondary=400,
                     constraint_max_time_to_current_solution=False,
-                ),
-                ParamsConstraintBuilder(
+                )
+            else:
+                params_0_cls = kwargs["params_0_cls"]
+                params_0_kwargs = kwargs["params_0_kwargs"]
+                params_0 = params_0_cls(**params_0_kwargs)
+            if kwargs["params_1_kwargs"] is None:
+                params_1 = ParamsConstraintBuilder(
                     minus_delta_primary=6000,
                     plus_delta_primary=6000,
                     minus_delta_secondary=0,
                     plus_delta_secondary=0,
                     constraint_max_time_to_current_solution=False,
-                ),
-            ],
-        )
+                )
+            else:
+                params_1_cls = kwargs["params_1_cls"]
+                params_1_kwargs = kwargs["params_1_kwargs"]
+                params_1 = params_1_cls(**params_1_kwargs)
+            params_list = [params_0, params_1]
         constraint_handler = ConstraintHandlerScheduling(
             problem=rcpsp_problem,
             basic_constraint_builder=basic_constraint_builder,
             params_list=params_list,
             use_makespan_of_subtasks=kwargs.get("use_makespan_of_subtasks", False),
         )
     elif constraint_handler_type == ConstraintHandlerType.SOLUTION_REPAIR:
-        params_list = kwargs.get(
-            "params_list",
-            [
-                ParamsConstraintBuilder(
+        if "params_list" in kwargs:
+            params_list = kwargs["params_list"]
+        else:
+            if kwargs["params_0_kwargs"] is None:
+                params_0 = ParamsConstraintBuilder(
                     minus_delta_primary=6000,
                     plus_delta_primary=6000,
                     minus_delta_secondary=400,
                     plus_delta_secondary=400,
                     constraint_max_time_to_current_solution=False,
-                ),
-                ParamsConstraintBuilder(
+                )
+            else:
+                params_0_cls = kwargs["params_0_cls"]
+                params_0_kwargs = kwargs["params_0_kwargs"]
+                params_0 = params_0_cls(**params_0_kwargs)
+            if kwargs["params_1_kwargs"] is None:
+                params_1 = ParamsConstraintBuilder(
                     minus_delta_primary=5000,
                     plus_delta_primary=5000,
                     minus_delta_secondary=2,
                     plus_delta_secondary=2,
                     constraint_max_time_to_current_solution=False,
-                ),
-            ],
-        )
+                )
+            else:
+                params_1_cls = kwargs["params_1_cls"]
+                params_1_kwargs = kwargs["params_1_kwargs"]
+                params_1 = params_1_cls(**params_1_kwargs)
+            params_list = [params_0, params_1]
         constraint_handler = NeighborRepairProblems(
             problem=rcpsp_problem, params_list=params_list
         )
     return constraint_handler
 
 
 def build_constraint_handler_helper(rcpsp_problem: ANY_RCPSP, graph, **kwargs):
@@ -447,74 +473,155 @@
                     ),
                 ],
             ),
         )
     return constraint_handler
 
 
-class LargeNeighborhoodSearchScheduling(SolverGenericRCPSP):
+class LargeNeighborhoodSearchScheduling(LNS_CP, SolverGenericRCPSP):
+    hyperparameters = [
+        EnumHyperparameter(
+            name="cp_solver_name", enum=CPSolverName, default=CPSolverName.CHUFFED
+        ),
+        CategoricalHyperparameter(name="do_ls", choices=[True, False], default=False),
+        EnumHyperparameter(
+            name="constraint_handler_type",
+            enum=ConstraintHandlerType,
+            default=ConstraintHandlerType.MIX_SUBPROBLEMS,
+        ),
+        FloatHyperparameter(
+            name="fraction_subproblem", default=0.05, low=0.0, high=1.0
+        ),
+        IntegerHyperparameter(name="nb_cut_part", default=10, low=0, high=100),
+        CategoricalHyperparameter(
+            name="use_makespan_of_subtasks", choices=[True, False], default=False
+        ),
+        SubBrickHyperparameter(
+            name="params_0_cls",
+            choices=[ParamsConstraintBuilder],
+            default=ParamsConstraintBuilder,
+        ),
+        SubBrickKwargsHyperparameter(
+            name="params_0_kwargs", subbrick_hyperparameter="params_0_cls"
+        ),
+        SubBrickHyperparameter(
+            name="params_1_cls",
+            choices=[ParamsConstraintBuilder],
+            default=ParamsConstraintBuilder,
+        ),
+        SubBrickKwargsHyperparameter(
+            name="params_1_kwargs", subbrick_hyperparameter="params_1_cls"
+        ),
+    ]
+
     def __init__(
         self,
         problem: ANY_RCPSP,
         partial_solution=None,
+        cp_solver: Optional[MinizincCPSolver] = None,
+        initial_solution_provider: Optional[InitialSolution] = None,
+        constraint_handler: Optional[ConstraintHandler] = None,
+        post_process_solution: Optional[PostProcessSolution] = None,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
-        **kwargs
+        **kwargs: Any,
     ):
-        super().__init__(
-            problem=problem, params_objective_function=params_objective_function
+        SolverGenericRCPSP.__init__(
+            self, problem=problem, params_objective_function=params_objective_function
         )
         graph = build_graph_rcpsp_object(self.problem)
-        solver = kwargs.get("cp_solver", None)
-        if solver is None:
-            solver = build_default_cp_model(
-                rcpsp_problem=problem, partial_solution=partial_solution, **kwargs
-            )
-        self.cp_solver = solver
-        self.parameters_cp = kwargs.get("parameters_cp", ParametersCP.default())
-        self.constraint_handler = kwargs.get("constraint_handler", None)
-        if self.constraint_handler is None:
-            self.constraint_handler = build_constraint_handler(
-                rcpsp_problem=self.problem,
-                graph=graph,
-                multiskill=self.problem.is_multiskill(),
-                preemptive=self.problem.is_preemptive(),
-                **kwargs
-            )
-        self.post_pro = kwargs.get("post_process_solution", None)
-        if self.post_pro is None:
-            self.post_pro = build_default_postpro(
-                rcpsp_problem=self.problem, partial_solution=partial_solution, **kwargs
-            )
-        self.initial_solution_provider = kwargs.get("initial_solution_provider", None)
-        if self.initial_solution_provider is None:
-            self.initial_solution_provider = build_default_initial_solution(
-                rcpsp_problem=self.problem, **kwargs
-            )
-        self.lns_solver = LNS_CP(
-            problem=self.problem,
-            cp_solver=self.cp_solver,
-            initial_solution_provider=self.initial_solution_provider,
-            constraint_handler=self.constraint_handler,
-            post_process_solution=self.post_pro,
-            params_objective_function=self.params_objective_function,
-        )
+        kwargs = self.complete_with_default_hyperparameters(kwargs)
 
-    def solve(
-        self,
-        nb_iteration_lns: int,
-        parameters_cp: Optional[ParametersCP] = None,
-        nb_iteration_no_improvement: Optional[int] = None,
-        skip_first_iteration: bool = False,
-        stop_first_iteration_if_optimal: bool = True,
-        callbacks: Optional[List[Callback]] = None,
-        **args
-    ) -> ResultStorage:
-        if parameters_cp is None:
-            parameters_cp = ParametersCP.default()
-        return self.lns_solver.solve_lns(
-            parameters_cp=parameters_cp,
-            skip_first_iteration=skip_first_iteration,
-            stop_first_iteration_if_optimal=stop_first_iteration_if_optimal,
-            nb_iteration_no_improvement=nb_iteration_no_improvement,
-            nb_iteration_lns=nb_iteration_lns,
-            callbacks=callbacks,
-        )
+        if cp_solver is None:
+            if "cp_solver_kwargs" not in kwargs or kwargs["cp_solver_kwargs"] is None:
+                cp_solver_kwargs = kwargs
+            else:
+                cp_solver_kwargs = kwargs["cp_solver_kwargs"]
+            if "cp_solver_cls" not in kwargs or kwargs["cp_solver_cls"] is None:
+                cp_solver = build_default_cp_model(
+                    rcpsp_problem=problem,
+                    partial_solution=partial_solution,
+                    **cp_solver_kwargs,
+                )
+            else:
+                cp_solver_cls = kwargs["cp_solver_cls"]
+                cp_solver = cp_solver_cls(problem=self.problem, **cp_solver_kwargs)
+                cp_solver.init_model(**cp_solver_kwargs)
+        self.cp_solver = cp_solver
+
+        if constraint_handler is None:
+            if (
+                "constraint_handler_kwargs" not in kwargs
+                or kwargs["constraint_handler_kwargs"] is None
+            ):
+                constraint_handler_kwargs = kwargs
+            else:
+                constraint_handler_kwargs = kwargs["constraint_handler_kwargs"]
+            if (
+                "constraint_handler_cls" not in kwargs
+                or kwargs["constraint_handler_cls"] is None
+            ):
+                constraint_handler = build_constraint_handler(
+                    rcpsp_problem=self.problem,
+                    graph=graph,
+                    multiskill=self.problem.is_multiskill(),
+                    preemptive=self.problem.is_preemptive(),
+                    **constraint_handler_kwargs,
+                )
+            else:
+                constraint_handler_cls = kwargs["constraint_handler_cls"]
+                constraint_handler = constraint_handler_cls(
+                    problem=self.problem, **constraint_handler_kwargs
+                )
+        self.constraint_handler = constraint_handler
+
+        if post_process_solution is None:
+            if (
+                "post_process_solution_kwargs" not in kwargs
+                or kwargs["post_process_solution_kwargs"] is None
+            ):
+                post_process_solution_kwargs = kwargs
+            else:
+                post_process_solution_kwargs = kwargs["post_process_solution_kwargs"]
+            if (
+                "post_process_solution_cls" not in kwargs
+                or kwargs["post_process_solution_cls"] is None
+            ):
+                post_process_solution = build_default_postpro(
+                    rcpsp_problem=self.problem,
+                    partial_solution=partial_solution,
+                    **post_process_solution_kwargs,
+                )
+            else:
+                post_process_solution_cls = kwargs["post_process_solution_cls"]
+                post_process_solution = post_process_solution_cls(
+                    problem=self.problem,
+                    params_objective_function=self.params_objective_function,
+                    **post_process_solution_kwargs,
+                )
+        self.post_process_solution = post_process_solution
+
+        if initial_solution_provider is None:
+            if (
+                "initial_solution_provider_kwargs" not in kwargs
+                or kwargs["initial_solution_provider_kwargs"] is None
+            ):
+                initial_solution_provider_kwargs = kwargs
+            else:
+                initial_solution_provider_kwargs = kwargs[
+                    "initial_solution_provider_kwargs"
+                ]
+            if (
+                "initial_solution_provider_cls" not in kwargs
+                or kwargs["initial_solution_provider_cls"] is None
+            ):
+                initial_solution_provider = build_default_initial_solution(
+                    rcpsp_problem=self.problem,
+                    **initial_solution_provider_kwargs,
+                )
+            else:
+                initial_solution_provider_cls = kwargs["initial_solution_provider_cls"]
+                initial_solution_provider = initial_solution_provider_cls(
+                    problem=self.problem,
+                    params_objective_function=self.params_objective_function,
+                    **initial_solution_provider_kwargs,
+                )
+        self.initial_solution_provider = initial_solution_provider
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/ls_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/ls_solver.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import logging
 from enum import Enum
+from typing import List, Optional
 
 import numpy as np
 
 from discrete_optimization.generic_rcpsp_tools.generic_rcpsp_solver import (
     SolverGenericRCPSP,
 )
 from discrete_optimization.generic_rcpsp_tools.typing import ANY_RCPSP
+from discrete_optimization.generic_tools.callbacks.callback import Callback
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    EnumHyperparameter,
+    FloatHyperparameter,
+    IntegerHyperparameter,
+)
 from discrete_optimization.generic_tools.ls.hill_climber import HillClimber
 from discrete_optimization.generic_tools.ls.local_search import (
     ModeMutation,
     RestartHandlerLimit,
 )
 from discrete_optimization.generic_tools.ls.simulated_annealing import (
     SimulatedAnnealing,
@@ -41,27 +49,39 @@
 
 class LS_SOLVER(Enum):
     SA = 0
     HC = 1
 
 
 class LS_RCPSP_Solver(SolverGenericRCPSP):
+    hyperparameters = [
+        CategoricalHyperparameter(
+            name="init_solution_process", choices=[True, False], default=False
+        ),
+        EnumHyperparameter(name="ls_solver", enum=LS_SOLVER, default=LS_SOLVER.SA),
+        FloatHyperparameter(name="temperature", low=0.01, high=10, default=3),
+        IntegerHyperparameter(
+            name="nb_iteration_no_improvement", low=10, high=2000, default=200
+        ),
+    ]
+
     def __init__(
         self,
         problem: ANY_RCPSP,
         params_objective_function: ParamsObjectiveFunction = None,
         ls_solver: LS_SOLVER = LS_SOLVER.SA,
         **args
     ):
         super().__init__(
             problem=problem, params_objective_function=params_objective_function
         )
         self.ls_solver = ls_solver
 
-    def solve(self, **kwargs):
+    def solve(self, callbacks: Optional[List[Callback]] = None, **kwargs):
+        kwargs = self.complete_with_default_hyperparameters(kwargs)
         model = self.problem
         dummy = kwargs.get("starting_point", model.get_dummy_solution())
         find_better_starting_solution = kwargs.get("init_solution_process", False)
         if isinstance(model, MS_RCPSPModel) and find_better_starting_solution:
             init = InitialSolutionMS_RCPSP(
                 problem=self.problem,
                 initial_method=InitialMethodRCPSP.PILE_CALENDAR,
@@ -77,24 +97,24 @@
             for mutate in mutations
             if mutate[0] == PermutationMutationRCPSP
         ]
         mixed_mutation = BasicPortfolioMutation(
             list_mutation, np.ones((len(list_mutation)))
         )
         res = RestartHandlerLimit(
-            nb_iteration_no_improvement=kwargs.get("nb_iteration_no_improvement", 300),
+            nb_iteration_no_improvement=kwargs["nb_iteration_no_improvement"],
         )
         ls = None
         if self.ls_solver == LS_SOLVER.SA:
             ls = SimulatedAnnealing(
                 problem=model,
                 mutator=mixed_mutation,
                 restart_handler=res,
                 temperature_handler=TemperatureSchedulingFactor(
-                    temperature=kwargs.get("temperature", 3),
+                    temperature=kwargs["temperature"],
                     restart_handler=res,
                     coefficient=kwargs.get("decay_temperature", 0.9999),
                 ),
                 mode_mutation=ModeMutation.MUTATE,
                 params_objective_function=self.params_objective_function,
                 store_solution=False,
             )
@@ -105,10 +125,11 @@
                 restart_handler=res,
                 mode_mutation=ModeMutation.MUTATE,
                 params_objective_function=self.params_objective_function,
                 store_solution=True,
             )
         result_sa = ls.solve(
             dummy,
+            callbacks=callbacks,
             nb_iteration_max=kwargs.get("nb_iteration_max", 2000),
         )
         return result_sa
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/neighbor_builder.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/neighbor_builder.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/neighbor_tools_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/neighbor_tools_rcpsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     ANY_CP_SOLVER,
     ANY_MSRCPSP,
     ANY_RCPSP,
     ANY_SOLUTION,
     ANY_SOLUTION_PREEMPTIVE,
 )
 from discrete_optimization.generic_tools.cp_tools import CPSolver, SignEnum
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    FloatHyperparameter,
+    IntegerHyperparameter,
+)
+from discrete_optimization.generic_tools.hyperparameters.hyperparametrizable import (
+    Hyperparametrizable,
+)
 from discrete_optimization.generic_tools.lns_cp import ConstraintHandler
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import RCPSPSolutionPreemptive
 from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
@@ -56,15 +64,48 @@
 logger = logging.getLogger(__name__)
 
 
 def get_max_time_solution(solution: ANY_SOLUTION):
     return solution.get_max_end_time()
 
 
-class ParamsConstraintBuilder:
+class ParamsConstraintBuilder(Hyperparametrizable):
+    hyperparameters = [
+        IntegerHyperparameter(name="minus_delta_primary", low=0, default=100),
+        IntegerHyperparameter(name="plus_delta_primary", low=0, default=100),
+        IntegerHyperparameter(name="minus_delta_secondary", low=0, default=0),
+        IntegerHyperparameter(name="plus_delta_secondary", low=0, default=0),
+        IntegerHyperparameter(name="minus_delta_primary_duration", default=5, low=0),
+        IntegerHyperparameter(name="plus_delta_primary_duration", default=5, low=0),
+        IntegerHyperparameter(name="minus_delta_secondary_duration", default=5, low=0),
+        IntegerHyperparameter(name="plus_delta_secondary_duration", default=5, low=0),
+        CategoricalHyperparameter(
+            name="constraint_max_time_to_current_solution",
+            choices=[True, False],
+            default=False,
+        ),
+        FloatHyperparameter(
+            name="fraction_of_task_assigned_multiskill", default=0.6, low=0.0, high=1.0
+        ),
+        CategoricalHyperparameter(
+            name="except_assigned_multiskill_primary_set",
+            choices=[True, False],
+            default=False,
+        ),
+        CategoricalHyperparameter(
+            name="first_method_multiskill", choices=[True, False], default=True
+        ),
+        CategoricalHyperparameter(
+            name="second_method_multiskill", choices=[True, False], default=False
+        ),
+        CategoricalHyperparameter(
+            name="additional_methods", choices=[True, False], default=False
+        ),
+    ]
+
     def __init__(
         self,
         minus_delta_primary: int,
         plus_delta_primary: int,
         minus_delta_secondary: int,
         plus_delta_secondary: int,
         minus_delta_primary_duration: int = 5,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/postpro_local_search.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/postpro_local_search.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/solution_repair.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/solution_repair.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_rcpsp_tools/typing.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_rcpsp_tools/typing.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/asp_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/asp_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/backup.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/backup.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/callback.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/early_stoppers.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/early_stoppers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/loggers.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/loggers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/callbacks/optuna.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/callbacks/optuna.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/cp_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/cp_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 from discrete_optimization.generic_tools.callbacks.callback import (
     Callback,
     CallbackList,
 )
 from discrete_optimization.generic_tools.do_problem import Solution
 from discrete_optimization.generic_tools.do_solver import SolverDO
 from discrete_optimization.generic_tools.exceptions import SolveEarlyStop
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    EnumHyperparameter,
+)
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -235,14 +238,19 @@
     def get_status_solver(self) -> Union[StatusSolver, None]:
         return self.status_solver
 
 
 class MinizincCPSolver(CPSolver):
     """CP solver wrapping a minizinc solver."""
 
+    hyperparameters = [
+        EnumHyperparameter(
+            name="cp_solver_name", enum=CPSolverName, default=CPSolverName.CHUFFED
+        )
+    ]
     instance: Optional[Instance] = None
     silent_solve_error: bool = False
     """If True and `solve` should raise an error, a warning is raised instead and an empty ResultStorage returned."""
 
     def solve(
         self,
         callbacks: Optional[List[Callback]] = None,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_mutation.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_mutation.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_problem.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_problem.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/do_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/do_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/alternating_ga.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/alternating_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/deap_wrappers.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/deap_wrappers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/ga.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/ga.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,19 @@
     Problem,
     TypeAttribute,
     lower_bound_vector_encoding_from_dict,
     upper_bound_vector_encoding_from_dict,
 )
 from discrete_optimization.generic_tools.do_solver import SolverDO
 from discrete_optimization.generic_tools.ea.deap_wrappers import generic_mutate_wrapper
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    EnumHyperparameter,
+    FloatHyperparameter,
+    IntegerHyperparameter,
+)
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 
 logger = logging.getLogger(__name__)
 
 
@@ -78,14 +83,25 @@
             name (str) of an encoding registered in the register solution of Problem
             or a dictionary of the form {'type': TypeAttribute, 'n': int} where type refers to a TypeAttribute and n
              to the dimension of the problem in this encoding (e.g. length of the vector)
             by default, the first encoding in the problem register_solution will be used.
 
     """
 
+    hyperparameters = [
+        EnumHyperparameter(name="crossover", enum=DeapCrossover, default=None),
+        EnumHyperparameter(
+            name="selection", enum=DeapSelection, default=DeapSelection.SEL_TOURNAMENT
+        ),
+        IntegerHyperparameter(name="pop_size", low=1, high=1000, default=100),
+        FloatHyperparameter(name="mut_rate", low=0, high=0.9, default=0.1),
+        FloatHyperparameter(name="crossover_rate", low=0, high=1, default=0.9),
+        FloatHyperparameter(name="tournament_size", low=0, high=1, default=0.2),
+    ]
+
     def __init__(
         self,
         problem: Problem,
         objectives: Union[str, List[str]],
         mutation: Optional[Union[Mutation, DeapMutation]] = None,
         crossover: Optional[DeapCrossover] = None,
         selection: DeapSelection = DeapSelection.SEL_TOURNAMENT,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/ga_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/ga_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ea/nsga.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ea/nsga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ghh_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ghh_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/graph_api.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/graph_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
-
+import string
 from typing import Any, Dict, Hashable, KeysView, List, Optional, Set, Tuple, Union
 
 import networkx as nx
 
 
 class Graph:
     def __init__(
@@ -155,7 +155,20 @@
         nodes=[(n, graph_nx.nodes[n]) for n in graph_nx.nodes()],
         edges=[(e[0], e[1], graph_nx.edges[e]) for e in graph_nx.edges()],
         undirected=undirected
         if undirected is not None
         else not isinstance(graph_nx, nx.DiGraph),
         compute_predecessors=compute_predecessors,
     )
+
+
+# this method is implemented to bypass the fact that networkX >= 3.2 is not compatible with python 3.8
+def get_node_attributes(graph: nx.Graph, name: string, default: Any):
+    """
+    @param graph: a nx.Graph
+    @param name: name of attribut of intereste
+    @param default:  default value if no value for attribute of interest
+    @return: a dictionnary with for each node of graph, the attribute value corresponding
+    """
+    if default is not None:
+        return {n: d.get(name, default) for n, d in graph.nodes.items()}
+    return {n: d[name] for n, d in graph.nodes.items() if name in d}
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/hyperparameter.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/hyperparameter.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/hyperparameters/hyperparametrizable.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/hyperparameters/hyperparametrizable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 #  Copyright (c) 2024 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 from __future__ import annotations  # see annotations as str
 
+import inspect
+from collections import defaultdict
+from copy import deepcopy
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
     Hyperparameter,
     SubBrickKwargsHyperparameter,
 )
 
@@ -50,14 +53,41 @@
 
     @classmethod
     def get_hyperparameter(cls, name: str) -> Hyperparameter:
         """Get hyperparameter from given name."""
         return cls.get_hyperparameters_by_name()[name]
 
     @classmethod
+    def copy_and_update_hyperparameters(
+        cls, names: Optional[List[str]] = None, **kwargs_by_name: Dict[str, Any]
+    ) -> List[Hyperparameter]:
+        """Copy hyperparameters definition of this class and update them with specified kwargs.
+
+        This is useful to define hyperparameters for a child class
+        for which only choices of the hyperparameter change for instance.
+
+        Args:
+            names: names of hyperparameters to copy. Default to all.
+            **kwargs_by_name: for each hyperparameter specified by its name,
+                the attributes to update. If a given hyperparameter name is not specified,
+                the hyperparameter is copied without further update.
+
+        Returns:
+
+        """
+        if names is None:
+            names = cls.get_hyperparameters_names()
+        kwargs_by_name = defaultdict(dict, kwargs_by_name)  # add missing names
+        return [
+            _copy_and_update_attributes(h, **kwargs_by_name[h.name])
+            for h in cls.hyperparameters
+            if h.name in names
+        ]
+
+    @classmethod
     def get_default_hyperparameters(
         cls, names: Optional[List[str]] = None
     ) -> Dict[str, Any]:
         """Get hyperparameters default values.
 
         Args:
             names: names of the hyperparameters to choose.
@@ -203,7 +233,17 @@
             suggested_hyperparameters[
                 hyperparameter.name
             ] = cls.suggest_hyperparameter_with_optuna(
                 trial=trial, name=hyperparameter.name, **kwargs_for_optuna_suggestion
             )
 
         return suggested_hyperparameters
+
+
+def _copy_and_update_attributes(h: Hyperparameter, **kwargs) -> Hyperparameter:
+    hyperparameter_cls = h.__class__
+    init_args_names = list(inspect.signature(h.__init__).parameters)
+    for name in init_args_names:
+        if name not in kwargs:
+            kwargs[name] = getattr(h, name)
+    h_new = hyperparameter_cls(**kwargs)
+    return h_new
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/lns_cp.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/lns_cp.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 )
 from discrete_optimization.generic_tools.do_problem import (
     ModeOptim,
     ParamsObjectiveFunction,
     Problem,
 )
 from discrete_optimization.generic_tools.do_solver import SolverDO
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    IntegerHyperparameter,
+    SubBrickHyperparameter,
+    SubBrickKwargsHyperparameter,
+)
 from discrete_optimization.generic_tools.hyperparameters.hyperparametrizable import (
     Hyperparametrizable,
 )
 from discrete_optimization.generic_tools.lns_mip import (
     InitialSolution,
     PostProcessSolution,
     TrivialPostProcessSolution,
@@ -68,34 +74,130 @@
         child_instance: Instance,
         previous_constraints: Iterable[Any],
     ) -> None:
         ...
 
 
 class LNS_CP(SolverDO):
+    hyperparameters = [
+        SubBrickHyperparameter("cp_solver_cls", choices=[], default=None),
+        SubBrickKwargsHyperparameter(
+            "cp_solver_kwargs", subbrick_hyperparameter="cp_solver_cls"
+        ),
+        SubBrickHyperparameter(
+            "initial_solution_provider_cls", choices=[], default=None
+        ),
+        SubBrickKwargsHyperparameter(
+            "initial_solution_provider_kwargs",
+            subbrick_hyperparameter="initial_solution_provider_cls",
+        ),
+        SubBrickHyperparameter(
+            "constraint_handler_cls",
+            choices=[],
+            default=None,
+        ),
+        SubBrickKwargsHyperparameter(
+            "constraint_handler_kwargs",
+            subbrick_hyperparameter="constraint_handler_cls",
+        ),
+        SubBrickHyperparameter(
+            "post_process_solution_cls",
+            choices=[],
+            default=TrivialPostProcessSolution,
+        ),
+        SubBrickKwargsHyperparameter(
+            "post_process_solution_kwargs",
+            subbrick_hyperparameter="post_process_solution_cls",
+        ),
+        CategoricalHyperparameter(
+            name="skip_first_iteration", choices=[True, False], default=False
+        ),
+    ]
+
     def __init__(
         self,
         problem: Problem,
-        cp_solver: MinizincCPSolver,
-        initial_solution_provider: InitialSolution,
-        constraint_handler: ConstraintHandler,
+        cp_solver: Optional[MinizincCPSolver] = None,
+        initial_solution_provider: Optional[InitialSolution] = None,
+        constraint_handler: Optional[ConstraintHandler] = None,
         post_process_solution: Optional[PostProcessSolution] = None,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
+        **kwargs: Any,
     ):
         super().__init__(
             problem=problem, params_objective_function=params_objective_function
         )
+        kwargs = self.complete_with_default_hyperparameters(kwargs)
+
+        if cp_solver is None:
+            if kwargs["cp_solver_kwargs"] is None:
+                cp_solver_kwargs = kwargs
+            else:
+                cp_solver_kwargs = kwargs["cp_solver_kwargs"]
+            if kwargs["cp_solver_cls"] is None:
+                raise ValueError(
+                    "`cp_solver_cls` cannot be None if `cp_solver` is not specified."
+                )
+            else:
+                cp_solver_cls = kwargs["cp_solver_cls"]
+                cp_solver = cp_solver_cls(problem=self.problem, **cp_solver_kwargs)
+                cp_solver.init_model(**cp_solver_kwargs)
         self.cp_solver = cp_solver
-        self.initial_solution_provider = initial_solution_provider
+
+        if constraint_handler is None:
+            if kwargs["constraint_handler_kwargs"] is None:
+                constraint_handler_kwargs = kwargs
+            else:
+                constraint_handler_kwargs = kwargs["constraint_handler_kwargs"]
+            if kwargs["constraint_handler_cls"] is None:
+                raise ValueError(
+                    "`constraint_handler_cls` cannot be None if `constraint_handler` is not specified."
+                )
+            else:
+                constraint_handler_cls = kwargs["constraint_handler_cls"]
+                constraint_handler = constraint_handler_cls(
+                    problem=self.problem, **constraint_handler_kwargs
+                )
         self.constraint_handler = constraint_handler
-        self.post_process_solution: PostProcessSolution
+
         if post_process_solution is None:
-            self.post_process_solution = TrivialPostProcessSolution()
-        else:
-            self.post_process_solution = post_process_solution
+            if kwargs["post_process_solution_kwargs"] is None:
+                post_process_solution_kwargs = kwargs
+            else:
+                post_process_solution_kwargs = kwargs["post_process_solution_kwargs"]
+            if kwargs["post_process_solution_cls"] is None:
+                post_process_solution = None
+            else:
+                post_process_solution_cls = kwargs["post_process_solution_cls"]
+                post_process_solution = post_process_solution_cls(
+                    problem=self.problem,
+                    params_objective_function=self.params_objective_function,
+                    **post_process_solution_kwargs,
+                )
+        self.post_process_solution = post_process_solution
+
+        if initial_solution_provider is None:
+            if kwargs["initial_solution_provider_kwargs"] is None:
+                initial_solution_provider_kwargs = kwargs
+            else:
+                initial_solution_provider_kwargs = kwargs[
+                    "initial_solution_provider_kwargs"
+                ]
+            if kwargs["initial_solution_provider_cls"] is None:
+                initial_solution_provider = (
+                    None  # ok if solve_lns with skip_first_iteration
+                )
+            else:
+                initial_solution_provider_cls = kwargs["initial_solution_provider_cls"]
+                initial_solution_provider = initial_solution_provider_cls(
+                    problem=self.problem,
+                    params_objective_function=self.params_objective_function,
+                    **initial_solution_provider_kwargs,
+                )
+        self.initial_solution_provider = initial_solution_provider
 
     def solve_lns(
         self,
         parameters_cp: ParametersCP,
         nb_iteration_lns: int,
         nb_iteration_no_improvement: Optional[int] = None,
         skip_first_iteration: bool = False,
@@ -104,25 +206,33 @@
         **kwargs: Any,
     ) -> ResultStorage:
         # wrap all callbacks in a single one
         callbacks_list = CallbackList(callbacks=callbacks)
         # start of solve callback
         callbacks_list.on_solve_start(solver=self)
 
+        # manage None post_process_solution (can happen in subclasses __init__)
+        if self.post_process_solution is None:
+            self.post_process_solution = TrivialPostProcessSolution()
+
         sense = self.params_objective_function.sense_function
         if nb_iteration_no_improvement is None:
             nb_iteration_no_improvement = 2 * nb_iteration_lns
         current_nb_iteration_no_improvement = 0
         if self.cp_solver.instance is None:
             self.cp_solver.init_model()
             if self.cp_solver.instance is None:  # for mypy
                 raise RuntimeError(
                     "CP model instance must not be None after calling init_model()!"
                 )
         if not skip_first_iteration:
+            if self.initial_solution_provider is None:
+                raise ValueError(
+                    "self.initial_solution_provider cannot be None if not skip_first_iteration."
+                )
             store_lns = self.initial_solution_provider.get_starting_solution()
             store_lns = self.post_process_solution.build_other_solution(store_lns)
             init_solution, objective = store_lns.get_best_solution_fit()
             if init_solution is None:
                 satisfy = False
             else:
                 satisfy = self.problem.satisfy(init_solution)
@@ -260,22 +370,24 @@
 
         # end of solve callback
         callbacks_list.on_solve_end(res=store_lns, solver=self)
         return store_lns
 
     def solve(
         self,
-        parameters_cp: ParametersCP,
         nb_iteration_lns: int,
+        parameters_cp: Optional[ParametersCP] = None,
         nb_iteration_no_improvement: Optional[int] = None,
         skip_first_iteration: bool = False,
         stop_first_iteration_if_optimal: bool = True,
         callbacks: Optional[List[Callback]] = None,
         **kwargs: Any,
     ) -> ResultStorage:
+        if parameters_cp is None:
+            parameters_cp = ParametersCP.default()
         return self.solve_lns(
             parameters_cp=parameters_cp,
             nb_iteration_lns=nb_iteration_lns,
             nb_iteration_no_improvement=nb_iteration_no_improvement,
             skip_first_iteration=skip_first_iteration,
             stop_first_iteration_if_optimal=stop_first_iteration_if_optimal,
             callbacks=callbacks,
@@ -431,21 +543,23 @@
 
         # end of solve callback
         callbacks_list.on_solve_end(res=store_lns, solver=self)
         return store_lns
 
     def solve(
         self,
-        parameters_cp: ParametersCP,
         nb_iteration_lns: int,
+        parameters_cp: Optional[ParametersCP] = None,
         nb_iteration_no_improvement: Optional[int] = None,
         skip_first_iteration: bool = False,
         callbacks: Optional[List[Callback]] = None,
         **kwargs: Any,
     ) -> ResultStorage:
+        if parameters_cp is None:
+            parameters_cp = ParametersCP.default()
         return self.solve_lns(
             parameters_cp=parameters_cp,
             nb_iteration_lns=nb_iteration_lns,
             nb_iteration_no_improvement=nb_iteration_no_improvement,
             skip_first_iteration=skip_first_iteration,
             callbacks=callbacks,
             **kwargs,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/lns_mip.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/lns_mip.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/lp_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/lp_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/hill_climber.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/hill_climber.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/local_search.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/local_search.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ls/simulated_annealing.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ls/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mip/pymip_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mip/pymip_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mixed_mutation.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mixed_mutation.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_bool.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_bool.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_catalog.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_catalog.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_integer.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_integer.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/mutation_util.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/mutation_util.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/mutations/permutation_mutations.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/mutations/permutation_mutations.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/optuna/timed_percentile_pruner.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/optuna/timed_percentile_pruner.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/ortools_cpsat_tools.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/ortools_cpsat_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/pytools/timeout_decorator.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/pytools/timeout_decorator.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/multiobj_utils.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/multiobj_utils.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/result_storage.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/result_storage.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/result_storage/resultcomparator.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/result_storage/resultcomparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import logging
 import math
 from typing import Dict, List, Optional, Tuple, cast
 
-import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
 from discrete_optimization.generic_tools.do_problem import (
     Problem,
     Solution,
     TupleFitness,
 )
+from discrete_optimization.generic_tools.plot_utils import get_cmap_with_nb_colors
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ParetoFront,
     ResultStorage,
     fitness_class,
     plot_pareto_2d,
     result_storage_to_pareto_front,
 )
@@ -135,16 +135,17 @@
             objectives_index = [0, 1]
         else:
             objecives_names = objectives_str
             objectives_index = []
             for obj in objectives_str:
                 obj_index = self.objectives_str.index(obj)
                 objectives_index.append(obj_index)
-
-        colors = cm.rainbow(np.linspace(0, 1, len(self.list_result_storage)))
+        colors = get_cmap_with_nb_colors(
+            color_map_str="rainbow", nb_colors=len(self.list_result_storage)
+        )
         fig, ax = plt.subplots(1)
         ax.set_xlabel(objecives_names[0])
         ax.set_ylabel(objecives_names[1])
 
         for i in range(len(self.list_result_storage)):
             ax.scatter(
                 x=[
@@ -161,30 +162,32 @@
         return ax
 
     def plot_all_2d_paretos_subplots(
         self, objectives_str: Optional[List[str]] = None
     ) -> Figure:
 
         if objectives_str is None:
-            objecives_names = self.objectives_str[:2]
+            objectives_names = self.objectives_str[:2]
             objectives_index = [0, 1]
         else:
-            objecives_names = objectives_str
+            objectives_names = objectives_str
             objectives_index = []
             for obj in objectives_str:
                 obj_index = self.objectives_str.index(obj)
                 objectives_index.append(obj_index)
 
         cols = 2
         rows = math.ceil(
             len(self.list_result_storage) / cols
         )  # I have to do this to ensure at least 2 rows or else it creates axs with only 1 diumension and it crashes
         fig, axs = plt.subplots(rows, cols)
         axis = axs.flatten()
-        colors = cm.rainbow(np.linspace(0, 1, len(self.list_result_storage)))
+        colors = get_cmap_with_nb_colors(
+            color_map_str="rainbow", nb_colors=len(self.list_result_storage)
+        )
         for i, ax in zip(
             range(len(self.list_result_storage)), axis[: len(self.list_result_storage)]
         ):
             x = [
                 p[1].vector_fitness[objectives_index[0]]  # type: ignore
                 for p in self.list_result_storage[i].list_solution_fits
             ]
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/generic_tools/robustness/robustness_tool.py` & `discrete_optimization-0.3.1/discrete_optimization/generic_tools/robustness/robustness_tool.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_model.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/knapsack_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/knapsack_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/knapsack_mzn.mzn` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/knapsack_mzn.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/multidim_multiscenario_knapsack.mzn` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/multidim_multiscenario_knapsack.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/minizinc/multidimension_knapsack.mzn` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/minizinc/multidimension_knapsack.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/mutation/mutation_knapsack.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/mutation/mutation_knapsack.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/cp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/cp_solvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     CPSolverName,
     MinizincCPSolver,
     find_right_minizinc_solver_name,
 )
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
 from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
     EnumHyperparameter,
+    FloatHyperparameter,
 )
 from discrete_optimization.generic_tools.lns_cp import ConstraintHandler
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.knapsack.knapsack_model import (
     KnapsackModel,
@@ -304,14 +305,18 @@
 
         """
         taken = kwargs["taken"]
         return KnapsackSolutionMultidimensional(problem=self.problem, list_taken=taken)
 
 
 class KnapConstraintHandler(ConstraintHandler):
+    hyperparameters = [
+        FloatHyperparameter(name="fraction_fix", default=0.95, low=0.0, high=1.0),
+    ]
+
     def __init__(self, fraction_fix: float = 0.95):
         self.fraction_fix = fraction_fix
 
     def adding_constraint_from_results_store(
         self,
         cp_solver: CPSolver,
         child_instance: Instance,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/dyn_prog_knapsack.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/dyn_prog_knapsack.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/gphh_knapsack.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/gphh_knapsack.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/greedy_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/greedy_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_asp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_asp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_cpmpy.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_cpmpy.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_cpsat_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_cpsat_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_decomposition.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_decomposition.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_lns_cp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_lns_cp_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,31 @@
 
 import random
 from typing import Any, Iterable, Optional
 
 from minizinc import Instance
 
 from discrete_optimization.generic_tools.cp_tools import CPSolver
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    FloatHyperparameter,
+)
 from discrete_optimization.generic_tools.lns_cp import ConstraintHandler
 from discrete_optimization.knapsack.knapsack_model import (
     KnapsackModel,
     KnapsackSolution,
 )
 from discrete_optimization.knapsack.solvers.cp_solvers import CPKnapsackMZN2
 from discrete_optimization.knapsack.solvers.greedy_solvers import ResultStorage
 
 
 class ConstraintHandlerKnapsack(ConstraintHandler):
+    hyperparameters = [
+        FloatHyperparameter(name="fraction_to_fix", default=0.9, low=0.0, high=1.0),
+    ]
+
     def __init__(self, problem: KnapsackModel, fraction_to_fix: float = 0.9):
         self.problem = problem
         self.fraction_to_fix = fraction_to_fix
         self.iter = 0
 
     def adding_constraint_from_results_store(
         self,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/knapsack_lns_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/knapsack_lns_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 from enum import Enum
 from typing import Any, Dict, Hashable, Mapping
 
 from discrete_optimization.generic_tools.do_problem import (
     ParamsObjectiveFunction,
     build_aggreg_function_and_params_objective,
 )
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    EnumHyperparameter,
+)
 from discrete_optimization.generic_tools.lns_mip import (
     ConstraintHandler,
     InitialSolution,
 )
 from discrete_optimization.generic_tools.lp_tools import MilpSolver, MilpSolverName
 from discrete_optimization.knapsack.knapsack_model import (
     KnapsackModel,
@@ -28,14 +31,21 @@
 
 class InitialKnapsackMethod(Enum):
     DUMMY = 0
     GREEDY = 1
 
 
 class InitialKnapsackSolution(InitialSolution):
+    hyperparameters = [
+        EnumHyperparameter(
+            name="initial_method",
+            enum=InitialKnapsackMethod,
+        ),
+    ]
+
     def __init__(
         self,
         problem: KnapsackModel,
         initial_method: InitialKnapsackMethod,
         params_objective_function: ParamsObjectiveFunction,
     ):
         self.problem = problem
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/knapsack/solvers/lp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/knapsack/solvers/lp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/builders/instance_builders.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/builders/instance_builders.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/gpdp.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/gpdp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp.mzn` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp_flow.mzn` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp_flow.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/minizinc/gpdp_resources.mzn` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/minizinc/gpdp_resources.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/plots/gpdp_plot_utils.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/plots/gpdp_plot_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,34 +2,33 @@
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 from __future__ import print_function
 
 from typing import Tuple
 
 import matplotlib.pyplot as plt
-from matplotlib import pyplot as plt
 from matplotlib.axes import Axes
 from matplotlib.figure import Figure
 
+from discrete_optimization.generic_tools.plot_utils import get_cmap_with_nb_colors
 from discrete_optimization.pickup_vrp.gpdp import GPDP, GPDPSolution
 
 
 def plot_gpdp_solution(
     sol: GPDPSolution,
     problem: GPDP,
 ) -> Tuple[Figure, Axes]:
     if problem.coordinates_2d is None:
         raise ValueError(
             "problem.coordinates_2d cannot be None when calling plot_ortools_solution."
         )
     vehicle_tours = sol.trajectories
     fig, ax = plt.subplots(1)
-    nb_colors = problem.number_vehicle
     nb_colors_clusters = len(problem.clusters_set)
-    colors_nodes = plt.cm.get_cmap("hsv", nb_colors_clusters)
+    colors_nodes = get_cmap_with_nb_colors("hsv", nb_colors_clusters)
     ax.scatter(
         [problem.coordinates_2d[node][0] for node in problem.clusters_dict],
         [problem.coordinates_2d[node][1] for node in problem.clusters_dict],
         s=1,
         color=[
             colors_nodes(problem.clusters_dict[node]) for node in problem.clusters_dict
         ],
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/lp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/lp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/lp_solver_pymip.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/lp_solver_pymip.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/pickup_vrp/solver/ortools_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/pickup_vrp/solver/ortools_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/__init__.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/__init__.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/fast_function_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/fast_function_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative_reif.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/fzn_my_cumulative_reif.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/mrcpsp_mode_satisfy.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/mrcpsp_mode_satisfy.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/my_cumulative.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/my_cumulative.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_calendar.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_calendar.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_no_bool.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_no_bool.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive_calendar.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_preemptive_calendar.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_with_faketasks.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_mzn_with_faketasks.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_resource_feasibility_mzn.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multi_mode_resource_feasibility_mzn.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_multiscenario.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_multiscenario.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_mzn_calendar_boxes.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_mzn_calendar_boxes.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_no_search.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_no_search.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive_calendar.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_preemptive_calendar.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_with_second_optim.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_mzn_with_second_optim.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_resource.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_resource.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/minizinc/resumee_rcpsp.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/minizinc/resumee_rcpsp.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/mutations/mutation_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/mutations/mutation_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/plots/rcpsp_utils_preemptive.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/plots/rcpsp_utils_preemptive.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import logging
 from typing import List, Union
 
-import matplotlib.cm
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.collections import PatchCollection
 from matplotlib.font_manager import FontProperties
 from matplotlib.patches import Polygon as pp
 from shapely.geometry import Polygon
 
+from discrete_optimization.generic_tools.plot_utils import (
+    get_cmap,
+    get_cmap_with_nb_colors,
+)
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import (
     RCPSPModelPreemptive,
     RCPSPSolutionPreemptive,
 )
 
 logger = logging.getLogger(__name__)
 
@@ -145,15 +148,15 @@
             index += 1
     for i in range(len(list_resource)):
         patches = []
         for polygon in polygons_ax[i]:
             x, y = polygon.exterior.xy
             ax[i].plot(x, y, zorder=-1, color="b")
             patches.append(pp(xy=polygon.exterior.coords))
-        p = PatchCollection(patches, cmap=matplotlib.cm.get_cmap("Blues"), alpha=0.4)
+        p = PatchCollection(patches, cmap=get_cmap("Blues"), alpha=0.4)
 
         ax[i].add_collection(p)
     merged_times, merged_cons = compute_nice_resource_consumption(
         rcpsp_model, rcpsp_sol, list_resources=list_resource
     )
     for i in range(len(list_resource)):
         ax[i].plot(
@@ -222,15 +225,15 @@
         + rcpsp_model.index_task[x],
     )
     max_time = rcpsp_sol.rcpsp_schedule[sorted_task_by_end[-1]]["ends"][-1]
     min_time = rcpsp_sol.rcpsp_schedule[sorted_task_by_start[0]]["starts"][0]
     patches = []
     for j in range(nb_task):
         nb_colors = len(tasks) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for start, end in zip(
             rcpsp_sol.rcpsp_schedule[tasks[j]]["starts"],
             rcpsp_sol.rcpsp_schedule[tasks[j]]["ends"],
         ):
             box = [
                 (j - 0.25, start),
                 (j - 0.25, end),
@@ -477,15 +480,15 @@
         fig.suptitle(title_figure)
         if len(array_ressource_usage) == 1:
             ax = [ax]
 
     for i in range(len(resources_list)):
         patches = []
         nb_colors = len(sorted_task_by_start) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for boxe in array_ressource_usage[resources_list[i]]["boxes_time"]:
             polygon = Polygon([(b[1], b[0]) for b in boxe])
             activity = boxe[0][2]
             x, y = polygon.exterior.xy
             ax[i].plot(x, y, zorder=-1, color="b")
             patches.append(
                 pp(
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_model.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_model_preemptive.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_model_preemptive.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_solution.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_solution.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_solvers.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,22 @@
 )
 from discrete_optimization.generic_tools.lp_tools import MilpSolverName, ParametersMilp
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import RCPSPModelPreemptive
-from discrete_optimization.rcpsp.solver.cp_lns_solver import (
-    LargeNeighborhoodSearchRCPSP,
-)
 from discrete_optimization.rcpsp.solver.cp_solvers import (
     CP_MRCPSP_MZN,
     CP_MRCPSP_MZN_PREEMPTIVE,
     CP_RCPSP_MZN,
     CP_RCPSP_MZN_PREEMPTIVE,
 )
 from discrete_optimization.rcpsp.solver.cpm import CPM
 from discrete_optimization.rcpsp.solver.cpsat_solver import CPSatRCPSPSolver
-from discrete_optimization.rcpsp.solver.rcpsp_cp_lns_solver import LNS_CP_RCPSP_SOLVER
 from discrete_optimization.rcpsp.solver.rcpsp_ga_solver import (
     GA_MRCPSP_Solver,
     GA_RCPSP_Solver,
 )
 from discrete_optimization.rcpsp.solver.rcpsp_lp_lns_solver import LNS_LP_RCPSP_SOLVER
 from discrete_optimization.rcpsp.solver.rcpsp_lp_solver import LP_MRCPSP, LP_RCPSP
 from discrete_optimization.rcpsp.solver.rcpsp_pile import (
@@ -111,44 +107,21 @@
     ],
     "critical-path": [(CPM, {})],
     "lns": [
         (
             LNS_LP_RCPSP_SOLVER,
             {"nb_iteration_lns": 100, "lp_solver": MilpSolverName.CBC},
         ),
-        (
-            LNS_CP_RCPSP_SOLVER,
-            {"nb_iteration_lns": 100, "nb_iteration_no_improvement": 100},
-        ),
     ],
     "lns-lp": [
         (
             LNS_LP_RCPSP_SOLVER,
             {"nb_iteration_lns": 100, "lp_solver": MilpSolverName.CBC},
         )
     ],
-    "lns-cp": [
-        (
-            LNS_CP_RCPSP_SOLVER,
-            {"nb_iteration_lns": 100, "nb_iteration_no_improvement": 100},
-        )
-    ],
-    "lns-cp-rcpsp": [
-        (
-            LargeNeighborhoodSearchRCPSP,
-            {
-                "nb_iteration_lns": 100,
-                "nb_iteration_no_improvement": 100,
-                "parameters_cp": ParametersCP.default(),
-                "cut_part": 1,
-                "add_objective_makespan": False,
-                "fraction_subproblem": 0.6,
-            },
-        )
-    ],
     "lns-scheduling": [
         (
             LargeNeighborhoodSearchScheduling,
             {
                 "nb_iteration_lns": 100,
                 "nb_iteration_no_improvement": 100,
                 "parameters_cp": ParametersCP.default_fast_lns(),
@@ -185,17 +158,14 @@
         RCPSPModel,
     ],
     CP_RCPSP_MZN_PREEMPTIVE: [RCPSPModelPreemptive],
     CP_MRCPSP_MZN_PREEMPTIVE: [RCPSPModelPreemptive],
     LNS_LP_RCPSP_SOLVER: [
         RCPSPModel,
     ],
-    LNS_CP_RCPSP_SOLVER: [
-        RCPSPModel,
-    ],
     LS_RCPSP_Solver: [
         RCPSPModelPreemptive,
         RCPSPModelSpecialConstraintsPreemptive,
         RCPSPModel,
     ],
     GA_RCPSP_Solver: [
         RCPSPModelPreemptive,
@@ -203,19 +173,14 @@
         RCPSPModel,
     ],
     GA_MRCPSP_Solver: [
         RCPSPModelPreemptive,
         RCPSPModelSpecialConstraintsPreemptive,
         RCPSPModel,
     ],
-    LargeNeighborhoodSearchRCPSP: [
-        RCPSPModelPreemptive,
-        RCPSPModelSpecialConstraintsPreemptive,
-        RCPSPModel,
-    ],
     LargeNeighborhoodSearchScheduling: [
         RCPSPModelPreemptive,
         RCPSPModelSpecialConstraintsPreemptive,
         RCPSPModel,
     ],
     CPM: [
         RCPSPModelPreemptive,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/rcpsp_utils.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/rcpsp_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,29 @@
     List,
     Optional,
     Sequence,
     Tuple,
     Union,
 )
 
+import matplotlib
 import matplotlib.cm
 import matplotlib.pyplot as plt
 import numpy as np
 import numpy.typing as npt
 import scipy.stats
 from matplotlib.collections import PatchCollection
 from matplotlib.patches import Polygon as pp
 from shapely.geometry import Polygon
 
 from discrete_optimization.generic_tools.graph_api import Graph
+from discrete_optimization.generic_tools.plot_utils import (
+    get_cmap,
+    get_cmap_with_nb_colors,
+)
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import RCPSPSolutionPreemptive
 
 if TYPE_CHECKING:  # avoid circular imports due to annotations
     from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
     from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
 
 logger = logging.getLogger(__name__)
@@ -154,15 +159,15 @@
                     break
     for i in range(len(list_resource)):
         patches = []
         for polygon in polygons_ax[i]:
             x, y = polygon.exterior.xy
             ax[i].plot(x, y, zorder=-1, color="b")
             patches.append(pp(xy=polygon.exterior.coords))
-        p = PatchCollection(patches, cmap=matplotlib.cm.get_cmap("Blues"), alpha=0.4)
+        p = PatchCollection(patches, cmap=get_cmap("Blues"), alpha=0.4)
         ax[i].add_collection(p)
     merged_times, merged_cons = compute_nice_resource_consumption(
         rcpsp_model, rcpsp_sol, list_resources=list_resource
     )
     for i in range(len(list_resource)):
         ax[i].plot(
             merged_times[i],
@@ -223,15 +228,15 @@
         key=lambda x: 100000 * rcpsp_sol.get_end_time(x) + rcpsp_model.index_task[x],
     )
     max_time = rcpsp_sol.get_end_time(sorted_task_by_end[-1])
     min_time = rcpsp_sol.get_start_time(sorted_task_by_start[0])
     patches = []
     for j in range(nb_task):
         nb_colors = len(tasks) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         box = [
             (j - 0.25, rcpsp_sol.rcpsp_schedule[tasks[j]]["start_time"]),
             (j - 0.25, rcpsp_sol.rcpsp_schedule[tasks[j]]["end_time"]),
             (j + 0.25, rcpsp_sol.rcpsp_schedule[tasks[j]]["end_time"]),
             (j + 0.25, rcpsp_sol.rcpsp_schedule[tasks[j]]["start_time"]),
             (j - 0.25, rcpsp_sol.rcpsp_schedule[tasks[j]]["start_time"]),
         ]
@@ -424,15 +429,15 @@
             ax = ax_
     if ax is None:  # for mypy
         raise RuntimeError("ax cannot be None at this point")
 
     for i in range(len(resources_list)):
         patches = []
         nb_colors = len(sorted_task_by_start) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for boxe in array_ressource_usage[resources_list[i]]["boxes_time"]:
             polygon = Polygon([(b[1], b[0]) for b in boxe])
             activity = boxe[0][2]
             x, y = polygon.exterior.xy
             ax[i].plot(x, y, zorder=-1, color="b")
             patches.append(
                 pp(
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/robust_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/robust_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/sgs_without_array.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/sgs_without_array.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_lns_methods_preemptive.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/specialized_rcpsp/rcpsp_specialized_constraints.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1291 +1,1415 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import logging
-import math
 import random
-from enum import Enum
-from typing import Any, Hashable, Iterable, List, Optional, Set, Union
+from copy import deepcopy
+from functools import partial
+from typing import Dict, Hashable, List, Optional, Set, Type, Union
 
-import networkx as nx
 import numpy as np
-from minizinc import Instance
 
-from discrete_optimization.generic_rcpsp_tools.graph_tools_rcpsp import (
-    GraphRCPSP,
-    GraphRCPSPSpecialConstraints,
-)
-from discrete_optimization.generic_rcpsp_tools.ls_solver import (
-    LS_SOLVER,
-    LS_RCPSP_Solver,
-)
-from discrete_optimization.generic_tools.cp_tools import CPSolver, SignEnum
 from discrete_optimization.generic_tools.do_problem import (
-    ParamsObjectiveFunction,
-    build_aggreg_function_and_params_objective,
+    ModeOptim,
+    ObjectiveDoc,
+    ObjectiveHandling,
+    ObjectiveRegister,
+    Problem,
+    Solution,
+    TypeObjective,
 )
-from discrete_optimization.generic_tools.lns_cp import ConstraintHandler
-from discrete_optimization.generic_tools.lns_mip import PostProcessSolution
-from discrete_optimization.generic_tools.result_storage.result_storage import (
-    ResultStorage,
+from discrete_optimization.rcpsp.fast_function_rcpsp import (
+    compute_mean_ressource,
+    sgs_fast_partial_schedule_preemptive,
+    sgs_fast_partial_schedule_preemptive_minduration,
+    sgs_fast_preemptive_minduration,
+    sgs_fast_preemptive_some_special_constraints,
 )
+from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import (
-    PartialSolutionPreemptive,
     RCPSPModelPreemptive,
     RCPSPSolutionPreemptive,
 )
-from discrete_optimization.rcpsp.rcpsp_utils import (
-    get_max_time_solution,
-    get_tasks_ending_between_two_times,
-)
-from discrete_optimization.rcpsp.solver.cp_solvers import (
-    CP_MRCPSP_MZN_PREEMPTIVE,
-    CP_RCPSP_MZN,
-    CP_RCPSP_MZN_PREEMPTIVE,
-)
-from discrete_optimization.rcpsp.specialized_rcpsp.rcpsp_specialized_constraints import (
-    RCPSPModelSpecialConstraintsPreemptive,
-    RCPSPSolutionSpecialPreemptive,
-    compute_constraints_details,
+from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
+from discrete_optimization.rcpsp.rcpsp_utils import intersect
+from discrete_optimization.rcpsp.special_constraints import (
+    SpecialConstraintsDescription,
 )
 
 logger = logging.getLogger(__name__)
 
 
-def last_opti_solution(last_result_store: ResultStorage):
-    current_solution, fit = next(
-        (
-            last_result_store.list_solution_fits[j]
-            for j in range(len(last_result_store.list_solution_fits))
-            if "opti_from_cp"
-            in last_result_store.list_solution_fits[j][0].__dict__.keys()
-        ),
-        (None, None),
-    )
-    if current_solution is None or fit != last_result_store.get_best_solution_fit()[1]:
-        current_solution, fit = last_result_store.get_last_best_solution()
-    return current_solution
+class RCPSPSolutionSpecialPreemptive(RCPSPSolutionPreemptive):
+    def change_problem(self, new_problem: Problem):
+        self.__init__(
+            problem=new_problem,
+            rcpsp_permutation=self.rcpsp_permutation,
+            rcpsp_modes=self.rcpsp_modes,
+        )
 
+    def __setattr__(self, key, value):
+        super.__setattr__(self, key, value)
+        if key == "rcpsp_permutation":
+            self._schedule_to_recompute = True
 
-class PostProLeftShift(PostProcessSolution):
-    def __init__(
-        self,
-        problem: RCPSPModelPreemptive,
-        params_objective_function: ParamsObjectiveFunction = None,
-        do_ls: bool = False,
-        **kwargs
-    ):
-        self.problem = problem
-        self.params_objective_function = params_objective_function
-        (
-            self.aggreg_from_sol,
-            self.aggreg_from_dict,
-            self.params_objective_function,
-        ) = build_aggreg_function_and_params_objective(
+    def copy(self):
+        return RCPSPSolutionSpecialPreemptive(
             problem=self.problem,
-            params_objective_function=self.params_objective_function,
+            rcpsp_permutation=deepcopy(self.rcpsp_permutation),
+            rcpsp_modes=deepcopy(self.rcpsp_modes),
+            rcpsp_schedule=deepcopy(self.rcpsp_schedule),
+            rcpsp_schedule_feasible=self.rcpsp_schedule_feasible,
+            standardised_permutation=self.standardised_permutation,
         )
-        self.graph = self.problem.compute_graph()
-        if isinstance(problem, RCPSPModelSpecialConstraintsPreemptive):
-            self.graph_rcpsp = GraphRCPSPSpecialConstraints(problem=self.problem)
-            self.special_constraints = True
-        else:
-            self.graph_rcpsp = GraphRCPSP(problem=self.problem)
-            self.special_constraints = False
-        self.successors = {
-            n: nx.algorithms.descendants(self.graph.graph_nx, n)
-            for n in self.graph.graph_nx.nodes()
-        }
-        self.predecessors = {
-            n: nx.algorithms.descendants(self.graph.graph_nx, n)
-            for n in self.graph.graph_nx.nodes()
-        }
-        self.immediate_predecessors = {
-            n: self.graph.get_predecessors(n) for n in self.graph.nodes_name
-        }
-        self.do_ls = do_ls
-        self.dict_params = kwargs
 
-    def build_other_solution(self, result_storage: ResultStorage) -> ResultStorage:
-        new_solution = sgs_variant(
-            solution=last_opti_solution(result_storage),
+    def lazy_copy(self):
+        return RCPSPSolutionSpecialPreemptive(
             problem=self.problem,
-            predecessors_dict=self.immediate_predecessors,
+            rcpsp_permutation=self.rcpsp_permutation,
+            rcpsp_modes=self.rcpsp_modes,
+            rcpsp_schedule=self.rcpsp_schedule,
+            rcpsp_schedule_feasible=self.rcpsp_schedule_feasible,
+            standardised_permutation=self.standardised_permutation,
         )
-        fit = self.aggreg_from_sol(new_solution)
-        result_storage.add_solution(new_solution, fit)
-        if self.do_ls:
-            solver = LS_RCPSP_Solver(problem=self.problem, ls_solver=LS_SOLVER.SA)
-            s = result_storage.get_best_solution().copy()
-            if self.problem != s.problem:
-                s.change_problem(self.problem)
-            result_store = solver.solve(
-                nb_iteration_max=self.dict_params.get("nb_iteration_max", 200),
-                init_solution=s,
-            )
-            solution, f = result_store.get_last_best_solution()
-            result_storage.list_solution_fits += [
-                (solution, self.aggreg_from_sol(solution))
-            ]
-        return result_storage
-
 
-def sgs_variant(
-    solution: RCPSPSolutionPreemptive, problem: RCPSPModelPreemptive, predecessors_dict
-):
-    new_proposed_schedule = {}
-    new_horizon = min(solution.get_end_time(problem.sink_task) * 3, problem.horizon)
-    resource_avail_in_time = {}
-    modes_dict = problem.build_mode_dict(solution.rcpsp_modes)
-    for r in problem.resources_list:
-        if problem.is_varying_resource():
-            resource_avail_in_time[r] = np.copy(problem.resources[r][:new_horizon])
-        else:
-            resource_avail_in_time[r] = problem.resources[r] * np.ones(new_horizon)
-    sorted_tasks = sorted(
-        solution.rcpsp_schedule.keys(), key=lambda x: (solution.get_start_time(x), x)
-    )
-    for task in list(sorted_tasks):
-        if len(solution.rcpsp_schedule[task]["starts"]) > 1:
-            new_proposed_schedule[task] = {
-                "starts": solution.rcpsp_schedule[task]["starts"],
-                "ends": solution.rcpsp_schedule[task]["ends"],
-            }
-            for s, e in zip(
-                new_proposed_schedule[task]["starts"],
-                new_proposed_schedule[task]["ends"],
-            ):
-                for res in problem.resources_list:
-                    resource_avail_in_time[res][s:e] -= problem.mode_details[task][
-                        modes_dict[task]
-                    ].get(res, 0)
-            sorted_tasks.remove(task)
-
-    def is_startable(tt):
-        if isinstance(problem, RCPSPModelSpecialConstraintsPreemptive):
-            return (
-                all(
-                    x in new_proposed_schedule
-                    for x in problem.special_constraints.dict_start_after_nunit_reverse.get(
-                        tt, {}
-                    )
-                )
-                and all(
-                    x in new_proposed_schedule
-                    for x in problem.special_constraints.dict_start_at_end_reverse.get(
-                        tt, {}
-                    )
-                )
-                and all(
-                    x in new_proposed_schedule
-                    for x in problem.special_constraints.dict_start_at_end_offset_reverse.get(
-                        tt, {}
-                    )
-                )
-                and all(t in new_proposed_schedule for t in predecessors_dict[tt])
-            )
-        return all(t in new_proposed_schedule for t in predecessors_dict[tt])
-
-    while True:
-        task = next((t for t in sorted_tasks if is_startable(t)))
-        sorted_tasks.remove(task)
-        if len(solution.rcpsp_schedule[task]["starts"]) > 1:
-            continue
-        times_predecessors = [
-            new_proposed_schedule[t]["ends"][-1]
-            if t in new_proposed_schedule
-            else solution.rcpsp_schedule[t]["ends"][-1]
-            for t in predecessors_dict[task]
-        ]
-        if isinstance(problem, RCPSPModelSpecialConstraintsPreemptive):
-            times_predecessors += [
-                new_proposed_schedule[t]["starts"][0]
-                if t in new_proposed_schedule
-                else solution.rcpsp_schedule[t]["starts"][0]
-                for t in problem.special_constraints.dict_start_together.get(
-                    task, set()
-                )
-            ]
-            times_predecessors += [
-                new_proposed_schedule[t]["starts"][0]
-                + problem.special_constraints.dict_start_after_nunit_reverse.get(task)[
-                    t
-                ]
-                if t in new_proposed_schedule
-                else solution.rcpsp_schedule[t]["starts"][0]
-                + problem.special_constraints.dict_start_after_nunit_reverse.get(task)[
-                    t
-                ]
-                for t in problem.special_constraints.dict_start_after_nunit_reverse.get(
-                    task, {}
-                )
-            ]
-            times_predecessors += [
-                new_proposed_schedule[t]["ends"][-1]
-                if t in new_proposed_schedule
-                else solution.rcpsp_schedule[t]["ends"][-1]
-                for t in problem.special_constraints.dict_start_at_end_reverse.get(
-                    task, {}
-                )
-            ]
-            times_predecessors += [
-                new_proposed_schedule[t]["ends"][-1]
-                + problem.special_constraints.dict_start_at_end_offset_reverse.get(
-                    task
-                )[t]
-                if t in new_proposed_schedule
-                else solution.rcpsp_schedule[t]["ends"][-1]
-                + problem.special_constraints.dict_start_at_end_offset_reverse.get(
-                    task
-                )[t]
-                for t in problem.special_constraints.dict_start_at_end_offset_reverse.get(
-                    task, {}
-                )
-            ]
-        if len(times_predecessors) > 0:
-            min_time = max(times_predecessors)
+    def __str__(self):
+        if self.rcpsp_schedule is None:
+            sched_str = "None"
         else:
-            min_time = 0
-        if solution.get_start_time(task) == solution.get_end_time(task):
-            new_proposed_schedule[task] = {"starts": [min_time], "ends": [min_time]}
-        if len(solution.rcpsp_schedule[task]["starts"]) > 1:
-            new_proposed_schedule[task] = {
-                "starts": solution.rcpsp_schedule[task]["starts"],
-                "ends": solution.rcpsp_schedule[task]["ends"],
-            }
+            sched_str = str(self.rcpsp_schedule)
+        val = "RCPSP solution (rcpsp_schedule): " + sched_str
+        return val
+
+    def generate_schedule_from_permutation_serial_sgs(self, do_fast=True):
+        if do_fast:
+            super().generate_schedule_from_permutation_serial_sgs(do_fast=True)
         else:
-            for t in range(min_time, problem.horizon):
-                if all(
-                    resource_avail_in_time[res][time]
-                    >= problem.mode_details[task][modes_dict[task]].get(res, 0)
-                    for res in problem.resources_list
-                    for time in range(
-                        t, t + problem.mode_details[task][modes_dict[task]]["duration"]
-                    )
-                ):
-                    new_starting_time = t
-                    break
-            new_proposed_schedule[task] = {
-                "starts": [new_starting_time],
-                "ends": [
-                    new_starting_time
-                    + problem.mode_details[task][modes_dict[task]]["duration"]
-                ],
-            }
-            for s, e in zip(
-                new_proposed_schedule[task]["starts"],
-                new_proposed_schedule[task]["ends"],
-            ):
-                for res in problem.resources_list:
-                    resource_avail_in_time[res][s:e] -= problem.mode_details[task][
-                        modes_dict[task]
-                    ].get(res, 0)
-        if len(sorted_tasks) == 0:
-            break
-    new_solution = RCPSPSolutionSpecialPreemptive(
-        problem=problem,
-        rcpsp_schedule=new_proposed_schedule,
-        rcpsp_schedule_feasible=True,
-        rcpsp_modes=solution.rcpsp_modes,
-    )
-    logger.debug(
-        ("New : ", problem.evaluate(new_solution), problem.satisfy(new_solution))
-    )
-    logger.debug(("Old : ", problem.evaluate(solution), problem.satisfy(solution)))
-    return new_solution
-
-
-def constraints_strings(
-    current_solution: RCPSPSolutionPreemptive,
-    subtasks: Set[Hashable],
-    minus_delta: int,
-    plus_delta: int,
-    jobs_to_fix: Set[Hashable],
-    cp_solver: Union[CP_RCPSP_MZN_PREEMPTIVE, CP_MRCPSP_MZN_PREEMPTIVE],
-    constraint_max_time=True,
-    minus_delta_2=0,
-    plus_delta_2=0,
-):
-    max_time = get_max_time_solution(solution=current_solution)
-    list_strings = []
-    for job in subtasks:
-        for j in range(len(current_solution.rcpsp_schedule[job]["starts"])):
-            start_time_j = current_solution.rcpsp_schedule[job]["starts"][j]
-            end_time_j = current_solution.rcpsp_schedule[job]["ends"][j]
-            duration_j = end_time_j - start_time_j
-            string1Start = cp_solver.constraint_start_time_string_preemptive_i(
-                task=job,
-                start_time=max(0, start_time_j - minus_delta),
-                sign=SignEnum.UEQ,
-                part_id=j + 1,
-            )
-            string2Start = cp_solver.constraint_start_time_string_preemptive_i(
-                task=job,
-                start_time=min(max_time, start_time_j + plus_delta)
-                if constraint_max_time
-                else start_time_j + plus_delta,
-                sign=SignEnum.LEQ,
-                part_id=j + 1,
+            schedule, feasible = self.problem.sgs_func(
+                solution=self, rcpsp_problem=self.problem
             )
-            string1Dur = cp_solver.constraint_duration_string_preemptive_i(
-                task=job,
-                duration=max(duration_j - 5, 0),
-                sign=SignEnum.UEQ,
-                part_id=j + 1,
-            )
-            string2Dur = cp_solver.constraint_duration_string_preemptive_i(
-                task=job, duration=duration_j + 5, sign=SignEnum.LEQ, part_id=j + 1
-            )
-            list_strings += [string1Dur, string1Start, string2Dur, string2Start]
-        for k in range(
-            len(current_solution.rcpsp_schedule[job]["starts"]), cp_solver.nb_preemptive
-        ):
-            string1Dur = cp_solver.constraint_duration_string_preemptive_i(
-                task=job, duration=0, sign=SignEnum.EQUAL, part_id=k + 1
-            )
-            list_strings += [string1Dur]
-    for job in jobs_to_fix:
-        is_paused = len(current_solution.rcpsp_schedule[job]["starts"]) > 1
-        is_paused_str = "true" if is_paused else "false"
-        list_strings += [
-            "constraint is_paused["
-            + str(cp_solver.index_in_minizinc[job])
-            + "]=="
-            + is_paused_str
-            + ";\n"
-        ]
-    for job in jobs_to_fix:
-        if job in subtasks:
-            continue
-        for j in range(len(current_solution.rcpsp_schedule[job]["starts"])):
-            start_time_j = current_solution.rcpsp_schedule[job]["starts"][j]
-            end_time_j = current_solution.rcpsp_schedule[job]["ends"][j]
-            duration_j = end_time_j - start_time_j
-            if minus_delta_2 == 0 and plus_delta_2 == 0:
-                string1Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=start_time_j,
-                    sign=SignEnum.EQUAL,
-                    part_id=j + 1,
-                )
-                string1Dur = cp_solver.constraint_duration_string_preemptive_i(
-                    task=job, duration=duration_j, sign=SignEnum.EQUAL, part_id=j + 1
-                )
-                list_strings += [string1Dur, string1Start]
-            else:
-                string1Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=max(0, start_time_j - minus_delta_2),
-                    sign=SignEnum.UEQ,
-                    part_id=j + 1,
-                )
-                string2Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=min(max_time, start_time_j + plus_delta_2)
-                    if constraint_max_time
-                    else start_time_j + plus_delta_2,
-                    sign=SignEnum.LEQ,
-                    part_id=j + 1,
-                )
-                string1Dur = cp_solver.constraint_duration_string_preemptive_i(
-                    task=job,
-                    duration=max(duration_j - 5, 0),
-                    sign=SignEnum.UEQ,
-                    part_id=j + 1,
-                )
-                string2Dur = cp_solver.constraint_duration_string_preemptive_i(
-                    task=job, duration=duration_j + 5, sign=SignEnum.LEQ, part_id=j + 1
-                )
-                list_strings += [string1Dur, string1Start, string2Dur, string2Start]
-        for k in range(
-            len(current_solution.rcpsp_schedule[job]["starts"]), cp_solver.nb_preemptive
-        ):
-            if minus_delta_2 == 0 and plus_delta_2 == 0:
-                string1Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=current_solution.rcpsp_schedule[job]["ends"][-1],
-                    sign=SignEnum.EQUAL,
-                    part_id=k + 1,
-                )
-                list_strings += [string1Start]
-            else:
-                string1Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=current_solution.rcpsp_schedule[job]["ends"][-1]
-                    - minus_delta_2,
-                    sign=SignEnum.UEQ,
-                    part_id=k + 1,
-                )
-                string2Start = cp_solver.constraint_start_time_string_preemptive_i(
-                    task=job,
-                    start_time=min(
-                        max_time,
-                        current_solution.rcpsp_schedule[job]["ends"][-1] + plus_delta_2,
-                    )
-                    if constraint_max_time
-                    else current_solution.rcpsp_schedule[job]["ends"][-1]
-                    + plus_delta_2,
-                    sign=SignEnum.LEQ,
-                    part_id=k + 1,
-                )
-                list_strings += [string2Start, string1Start]
-            string1Dur = cp_solver.constraint_duration_string_preemptive_i(
-                task=job, duration=0, sign=SignEnum.EQUAL, part_id=k + 1
-            )
-            list_strings += [string1Dur]
+            self.rcpsp_schedule = schedule
+            self.rcpsp_schedule_feasible = feasible
+            self._schedule_to_recompute = False
 
-    return list_strings
+    def generate_schedule_from_permutation_serial_sgs_2(
+        self,
+        current_t: int = 0,
+        completed_tasks: Optional[Set[Hashable]] = None,
+        partial_schedule: Optional[Dict[Hashable, Dict[str, List[int]]]] = None,
+        do_fast: bool = True,
+    ):
+        if do_fast:
+            super().generate_schedule_from_permutation_serial_sgs_2(
+                current_t=current_t,
+                completed_tasks=completed_tasks,
+                partial_schedule=partial_schedule,
+                do_fast=do_fast,
+            )
+        else:
+            if completed_tasks is None:
+                completed_tasks = {}
+            if partial_schedule is None:
+                partial_schedule = partial_schedule
+            schedule, feasible = self.problem.sgs_func_partial(
+                solution=self,
+                current_t=current_t,
+                partial_schedule=partial_schedule,
+                completed_tasks=completed_tasks,
+                rcpsp_problem=self.problem,
+            )
+            self.rcpsp_schedule = schedule
+            self.rcpsp_schedule_feasible = not feasible
+            self._schedule_to_recompute = False
 
 
-class NeighborFixStart(ConstraintHandler):
+class RCPSPModelSpecialConstraintsPreemptive(RCPSPModelPreemptive):
     def __init__(
         self,
-        problem: RCPSPModelPreemptive,
-        fraction_to_fix: float = 0.9,
-        delta_time_from_makepan_to_not_fix: int = 5,
+        resources: Union[Dict[str, int], Dict[str, List[int]]],
+        non_renewable_resources: List[str],
+        mode_details: Dict[Hashable, Dict[Union[str, int], Dict[str, int]]],
+        successors: Dict[Union[int, str], List[Union[str, int]]],
+        horizon,
+        special_constraints: SpecialConstraintsDescription = None,
+        preemptive_indicator: Dict[Hashable, bool] = None,
+        relax_the_start_at_end: bool = True,
+        tasks_list: List[Union[int, str]] = None,
+        source_task=None,
+        sink_task=None,
+        name_task: Dict[int, str] = None,
+        **kwargs
     ):
-        self.problem = problem
-        self.fraction_to_fix = fraction_to_fix
-        self.delta_time_from_makepan_to_not_fix = delta_time_from_makepan_to_not_fix
-
-    def adding_constraint_from_results_store(
-        self,
-        cp_solver: Union[CP_RCPSP_MZN_PREEMPTIVE, CP_MRCPSP_MZN_PREEMPTIVE],
-        child_instance: Instance,
-        result_storage: ResultStorage,
-        last_result_store: Optional[ResultStorage] = None,
-    ) -> Iterable[Any]:
-        current_solution, fit = result_storage.get_best_solution_fit()
-        current_solution: RCPSPSolutionPreemptive = current_solution
-        max_time = get_max_time_solution(solution=current_solution)
-        nb_jobs = self.problem.n_jobs
-        jobs_to_fix = set(
-            random.sample(
-                list(current_solution.rcpsp_schedule),
-                int(self.fraction_to_fix * nb_jobs),
-            )
+        super().__init__(
+            resources=resources,
+            non_renewable_resources=non_renewable_resources,
+            mode_details=mode_details,
+            successors=successors,
+            horizon=horizon,
+            tasks_list=tasks_list,
+            source_task=source_task,
+            sink_task=sink_task,
+            name_task=name_task,
+            preemptive_indicator=preemptive_indicator,
         )
-        subtasks = set(
-            [s for s in current_solution.rcpsp_schedule if s not in jobs_to_fix]
+
+        self.special_constraints = special_constraints
+        self.do_special_constraints = special_constraints is not None
+        if self.special_constraints is None:
+            self.special_constraints = SpecialConstraintsDescription()
+        self.predecessors_dict = {task: [] for task in self.tasks_list}
+        for task in self.successors:
+            for stask in self.successors[task]:
+                self.predecessors_dict[stask] += [task]
+        if self.do_special_constraints:
+            for t1, t2 in self.special_constraints.start_at_end:
+                if t2 not in self.successors[t1]:
+                    self.successors[t1].append(t2)
+            for t1, t2, off in self.special_constraints.start_at_end_plus_offset:
+                if t2 not in self.successors[t1]:
+                    self.successors[t1].append(t2)
+            for t1, t2 in self.special_constraints.start_together:
+                for predt1 in self.predecessors_dict[t1]:
+                    if t2 not in self.successors[predt1]:
+                        self.successors[predt1] += [t2]
+                for predt2 in self.predecessors_dict[t2]:
+                    if t1 not in self.successors[predt2]:
+                        self.successors[predt2] += [t1]
+        self.graph = self.compute_graph()
+        self.predecessors = self.graph.predecessors_dict
+        self.sgs_func = generate_schedule_from_permutation_serial_sgs_preemptive
+        self.sgs_func_partial = (
+            generate_schedule_from_permutation_serial_sgs_partial_schedule_preempptive
         )
-        list_strings = constraints_strings(
-            current_solution=current_solution,
-            subtasks=subtasks,
-            minus_delta=max_time,
-            plus_delta=max_time,
-            jobs_to_fix=jobs_to_fix,
-            cp_solver=cp_solver,
-        )
-        for s in list_strings:
-            child_instance.add_string(s)
-        return list_strings
+        self.relax_the_start_at_end = relax_the_start_at_end
+        (
+            self.func_sgs,
+            self.func_sgs_2,
+            self.compute_mean_resource,
+        ) = create_np_data_and_jit_functions(self)
 
-    def remove_constraints_from_previous_iteration(
-        self,
-        cp_solver: CP_RCPSP_MZN,
-        child_instance,
-        previous_constraints: Iterable[Any],
-    ):
-        pass
+    def is_preemptive(self):
+        return True
 
+    def has_special_constraints(self):
+        return self.do_special_constraints
 
-class MethodSubproblem(Enum):
-    BLOCK_TIME = 0
-    BLOCK_TIME_AND_PREDECESSORS = 1
+    def update_function(self):
+        (
+            self.func_sgs,
+            self.func_sgs_2,
+            self.compute_mean_resource,
+        ) = create_np_data_and_jit_functions(self)
+
+    def update_functions(self):
+        self.update_function()
+
+    def copy(self):
+        return RCPSPModelSpecialConstraintsPreemptive(
+            resources=deepcopy(self.resources),
+            non_renewable_resources=deepcopy(self.non_renewable_resources),
+            mode_details=deepcopy(self.mode_details),
+            successors=deepcopy(self.successors),
+            horizon=self.horizon,
+            special_constraints=deepcopy(self.special_constraints),
+            preemptive_indicator=deepcopy(self.preemptive_indicator),
+            relax_the_start_at_end=self.relax_the_start_at_end,
+            tasks_list=deepcopy(self.tasks_list),
+            source_task=self.source_task,
+            sink_task=self.sink_task,
+            name_task=deepcopy(self.name_task),
+        )
 
+    def lazy_copy(self):
+        return RCPSPModelSpecialConstraintsPreemptive(
+            resources=self.resources,
+            non_renewable_resources=self.non_renewable_resources,
+            mode_details=self.mode_details,
+            successors=self.successors,
+            horizon=self.horizon,
+            special_constraints=self.special_constraints,
+            preemptive_indicator=self.preemptive_indicator,
+            relax_the_start_at_end=self.relax_the_start_at_end,
+            tasks_list=self.tasks_list,
+            source_task=self.source_task,
+            sink_task=self.sink_task,
+            name_task=self.name_task,
+        )
 
-def intersect(i1, i2):
-    if i2[0] >= i1[1] or i1[0] >= i2[1]:
+    def evaluate_from_encoding(self, int_vector, encoding_name):
+        if encoding_name == "rcpsp_permutation":
+            single_mode_list = [1 for i in range(self.n_jobs_non_dummy)]
+            rcpsp_sol = RCPSPSolutionSpecialPreemptive(
+                problem=self, rcpsp_permutation=int_vector, rcpsp_modes=single_mode_list
+            )
+            objectives = self.evaluate(rcpsp_sol)
+            return objectives
         return None
-    else:
-        s = max(i1[0], i2[0])
-        e = min(i1[1], i2[1])
-        return [s, e]
 
-
-class NeighborFixStartSubproblem(ConstraintHandler):
-    def __init__(
-        self,
-        problem: RCPSPModelPreemptive,
-        nb_cut_part: int = 20,
-        fraction_size_subproblem: float = 0.1,
-        method: MethodSubproblem = MethodSubproblem.BLOCK_TIME,
-    ):
-        self.problem = problem
-        self.fraction_size_subproblem = fraction_size_subproblem
-        self.nb_jobs_subproblem = int(
-            self.fraction_size_subproblem * self.problem.n_jobs
-        )
-        self.method = method
-        self.graph = self.problem.compute_graph()
-        self.graph_nx = self.graph.graph_nx
-        if isinstance(
-            problem,
-            RCPSPModelSpecialConstraintsPreemptive,
-        ):
-            self.graph_rcpsp = GraphRCPSPSpecialConstraints(problem=self.problem)
-            self.special_constraints = True
-        else:
-            self.graph_rcpsp = GraphRCPSP(problem=self.problem)
-            self.special_constraints = False
-        self.nb_cut_part = nb_cut_part
-        self.current_sub_part = 0
-
-    def adding_constraint_from_results_store(
-        self,
-        cp_solver: Union[CP_RCPSP_MZN_PREEMPTIVE, CP_MRCPSP_MZN_PREEMPTIVE],
-        child_instance: Instance,
-        result_storage: ResultStorage,
-        last_result_store: Optional[ResultStorage] = None,
-    ) -> Iterable[Any]:
-        if last_result_store is not None:
-            current_solution, fit = next(
-                (
-                    last_result_store.list_solution_fits[j]
-                    for j in range(len(last_result_store.list_solution_fits))
-                    if "opti_from_cp"
-                    in last_result_store.list_solution_fits[j][0].__dict__.keys()
-                ),
-                (None, None),
+    def evaluate_function(self, rcpsp_sol: RCPSPSolutionPreemptive):
+        if rcpsp_sol._schedule_to_recompute:
+            rcpsp_sol.generate_schedule_from_permutation_serial_sgs()
+        makespan = rcpsp_sol.get_end_time(task=self.sink_task)
+        if rcpsp_sol.rcpsp_schedule_feasible:
+            penalty = evaluate_constraints(
+                solution=rcpsp_sol, constraints=self.special_constraints
             )
         else:
-            current_solution, fit = next(
-                (
-                    result_storage.list_solution_fits[j]
-                    for j in range(len(result_storage.list_solution_fits))
-                    if "opti_from_cp"
-                    in result_storage.list_solution_fits[j][0].__dict__.keys()
-                ),
-                (None, None),
-            )
-        if current_solution is None or fit != result_storage.get_best_solution_fit()[1]:
-            current_solution, fit = result_storage.get_last_best_solution()
-        current_solution: RCPSPSolutionPreemptive = current_solution
-        method = random.choices([0, 1, 2], weights=[0.5, 0.1, 0.4], k=1)[0]
-        if method == 0:
-            subtasks = create_subproblem_cut_time(
-                current_solution=current_solution, neighbor_fix_problem=self
-            )
-        elif method == 1:
-            subtasks = create_subproblems_random_and_predecessors(
-                current_solution=current_solution, neighbor_fix_problem=self
-            )
-        elif method == 2:
-            subtasks = create_subproblems_problems(
-                current_solution=current_solution, neighbor_fix_problem=self
-            )
-        subtasks = set(subtasks)
-        evaluation = self.problem.evaluate(current_solution)
-        if evaluation["constraint_penalty"] == 0:
-            list_strings = constraints_strings(
-                current_solution=current_solution,
-                subtasks=subtasks,
-                plus_delta=6000,
-                minus_delta=6000,
-                plus_delta_2=1,
-                minus_delta_2=1,
-                jobs_to_fix=set(self.problem.tasks_list),
-                cp_solver=cp_solver,
-                constraint_max_time=True,
-            )
-        else:
-            list_strings = constraints_strings(
-                current_solution=current_solution,
-                subtasks=subtasks,
-                plus_delta=6000,
-                minus_delta=6000,
-                plus_delta_2=400,
-                minus_delta_2=400,
-                jobs_to_fix=set(self.problem.tasks_list),
-                cp_solver=cp_solver,
-                constraint_max_time=False,
-            )
-        for s in list_strings:
-            child_instance.add_string(s)
-        child_instance.add_string(
-            "constraint sec_objective<="
-            + str(100 * evaluation["constraint_penalty"])
-            + ";\n"
-        )
-        if evaluation["constraint_penalty"] > 0:
-            strings = cp_solver.constraint_objective_max_time_set_of_jobs(
-                [self.problem.sink_task]
-            )
-        else:
-            strings = cp_solver.constraint_objective_max_time_set_of_jobs(subtasks)
-        for s in strings:
-            child_instance.add_string(s)
-            list_strings += [s]
-        self.current_sub_part = self.current_sub_part % self.nb_cut_part
-        return list_strings
+            penalty = 0
+        return makespan, penalty
 
-    def remove_constraints_from_previous_iteration(
-        self,
-        cp_solver: CP_RCPSP_MZN,
-        child_instance,
-        previous_constraints: Iterable[Any],
-    ):
-        pass
+    def evaluate(self, rcpsp_sol: RCPSPSolutionPreemptive) -> Dict[str, float]:
+        obj_makespan, penalty = self.evaluate_function(rcpsp_sol)
+        return {"makespan": obj_makespan, "constraint_penalty": penalty}
+
+    def get_objective_register(self) -> ObjectiveRegister:
+        dict_objective = {
+            "makespan": ObjectiveDoc(type=TypeObjective.OBJECTIVE, default_weight=-1.0),
+            "constraint_penalty": ObjectiveDoc(
+                type=TypeObjective.PENALTY, default_weight=-100.0
+            ),
+        }
+        return ObjectiveRegister(
+            objective_sense=ModeOptim.MAXIMIZATION,
+            objective_handling=ObjectiveHandling.AGGREGATE,
+            dict_objective_to_doc=dict_objective,
+        )
+
+    def satisfy(self, rcpsp_sol: RCPSPSolutionPreemptive):
+        s = check_solution(
+            problem=self,
+            solution=rcpsp_sol,
+            relax_the_start_at_end=self.relax_the_start_at_end,
+        )
+        if not s:
+            return s
+        return super().satisfy(rcpsp_sol)
+
+    def get_dummy_solution(self, random_perm: bool = False):
+        rcpsp_permutation = list(range(self.n_jobs_non_dummy))
+        if random_perm:
+            random.shuffle(rcpsp_permutation)
+        sol = RCPSPSolutionSpecialPreemptive(
+            problem=self,
+            rcpsp_permutation=rcpsp_permutation,
+            rcpsp_modes=[1 for i in range(self.n_jobs_non_dummy)],
+        )
+        return sol
+
+    def get_solution_type(self) -> Type[Solution]:
+        return RCPSPSolutionSpecialPreemptive
 
 
-def create_subproblem_cut_time(
-    current_solution, neighbor_fix_problem: NeighborFixStartSubproblem, subtasks=None
+def evaluate_constraints(
+    solution: Union[RCPSPSolution, RCPSPSolutionPreemptive],
+    constraints: SpecialConstraintsDescription,
 ):
-    nb_job_sub = math.ceil(
-        neighbor_fix_problem.problem.n_jobs / neighbor_fix_problem.nb_cut_part
-    )
-    task_of_interest = sorted(
-        current_solution.rcpsp_schedule,
-        key=lambda x: current_solution.rcpsp_schedule[x]["ends"][-1],
-    )
-    task_of_interest = task_of_interest[
-        neighbor_fix_problem.current_sub_part
-        * nb_job_sub : (neighbor_fix_problem.current_sub_part + 1)
-        * nb_job_sub
-    ]
-    if subtasks is None:
-        subtasks = task_of_interest
-    else:
-        subtasks.update(task_of_interest)
-    neighbor_fix_problem.current_sub_part = neighbor_fix_problem.current_sub_part + 1
-    return subtasks
+    list_constraints_not_respected = compute_constraints_details(solution, constraints)
+    return sum([x[-1] for x in list_constraints_not_respected])
 
 
-def create_subproblems_random_and_predecessors(
-    current_solution, neighbor_fix_problem: NeighborFixStartSubproblem, subtasks=None
+def compute_constraints_details(
+    solution: Union[RCPSPSolution, RCPSPSolutionPreemptive],
+    constraints: SpecialConstraintsDescription,
 ):
-    if subtasks is None:
-        subtasks = set()
-        len_subtask = 0
-    else:
-        len_subtask = len(subtasks)
-    while len_subtask < neighbor_fix_problem.nb_jobs_subproblem:
-        random_pick = random.choice(neighbor_fix_problem.problem.tasks_list)
-        interval = (
-            current_solution.rcpsp_schedule[random_pick]["starts"][0],
-            current_solution.rcpsp_schedule[random_pick]["ends"][0],
-        )
-        task_intersect = [
-            t
-            for t in current_solution.rcpsp_schedule
-            if intersect(
-                interval,
-                (
-                    current_solution.rcpsp_schedule[t]["starts"][0],
-                    current_solution.rcpsp_schedule[t]["ends"][0],
-                ),
-            )
-            is not None
-        ]
-        for k in set(task_intersect):
-            task_intersect += list(neighbor_fix_problem.graph.get_predecessors(k)) + [
-                l for l in neighbor_fix_problem.graph.get_neighbors(k)
+    if (
+        "rcpsp_schedule_feasible" in solution.__dict__.keys()
+        and not solution.rcpsp_schedule_feasible
+    ):
+        return []
+    start_together = constraints.start_together
+    start_at_end = constraints.start_at_end
+    start_at_end_plus_offset = constraints.start_at_end_plus_offset
+    start_after_nunit = constraints.start_after_nunit
+    disjunctive = constraints.disjunctive_tasks
+    list_constraints_not_respected = []
+    for (t1, t2) in start_together:
+        time1 = solution.get_start_time(t1)
+        time2 = solution.get_start_time(t2)
+        b = time1 == time2
+        if not b:
+            list_constraints_not_respected += [
+                ("start_together", t1, t2, time1, time2, abs(time2 - time1))
             ]
-            if isinstance(
-                neighbor_fix_problem.problem, RCPSPModelSpecialConstraintsPreemptive
-            ):
-                task_intersect += list(
-                    neighbor_fix_problem.problem.special_constraints.dict_start_at_end.get(
-                        k, {}
-                    )
-                )
-                task_intersect += list(
-                    neighbor_fix_problem.problem.special_constraints.dict_start_at_end_reverse.get(
-                        k, {}
+    for (t1, t2) in start_at_end:
+        time1 = solution.get_end_time(t1)
+        time2 = solution.get_start_time(t2)
+        b = time1 == time2
+        if not b:
+            list_constraints_not_respected += [
+                ("start_at_end", t1, t2, time1, time2, abs(time2 - time1))
+            ]
+    for (t1, t2, off) in start_at_end_plus_offset:
+        time1 = solution.get_end_time(t1) + off
+        time2 = solution.get_start_time(t2)
+        b = time2 >= time1
+        if not b:
+            list_constraints_not_respected += [
+                ("start_at_end_plus_offset", t1, t2, time1, time2, abs(time2 - time1))
+            ]
+    for (t1, t2, off) in start_after_nunit:
+        time1 = solution.get_start_time(t1) + off
+        time2 = solution.get_start_time(t2)
+        b = time2 >= time1
+        if not b:
+            list_constraints_not_respected += [
+                ("start_after_nunit", t1, t2, time1, time2, abs(time2 - time1))
+            ]
+    for t1, t2 in disjunctive:
+        b = intersect(
+            [solution.get_start_time(t1), solution.get_end_time(t1)],
+            [solution.get_start_time(t2), solution.get_end_time(t2)],
+        )
+        if b is not None:
+            list_constraints_not_respected += [
+                ("disjunctive", t1, t2, None, None, b[1] - b[0])
+            ]
+    for t in constraints.start_times_window:
+        if constraints.start_times_window[t][0] is not None:
+            if solution.get_start_time(t) < constraints.start_times_window[t][0]:
+                list_constraints_not_respected += [
+                    (
+                        "start_window_0",
+                        t,
+                        t,
+                        None,
+                        None,
+                        constraints.start_times_window[t][0]
+                        - solution.get_start_time(t),
                     )
-                )
-        subtasks.update(task_intersect)
-        len_subtask = len(subtasks)
-    return subtasks
-
+                ]
 
-def create_subproblems_problems(
-    current_solution, neighbor_fix_problem: NeighborFixStartSubproblem
-):
-    if neighbor_fix_problem.special_constraints:
-        details_constraints = compute_constraints_details(
-            solution=current_solution,
-            constraints=neighbor_fix_problem.problem.special_constraints,
-        )
-        sorted_constraints = sorted(details_constraints, key=lambda x: -x[-1])
-        random.shuffle(sorted_constraints)
-        subtasks = set()
-        len_subtasks = 0
-        j = 0
-        while (
-            j <= len(sorted_constraints) - 1
-            and len_subtasks < 4 * neighbor_fix_problem.nb_jobs_subproblem
-        ):
-            t1, t2 = sorted_constraints[j][1], sorted_constraints[j][2]
-            subtasks.add(t1)
-            subtasks.add(t2)
-            subtasks.update(
-                neighbor_fix_problem.graph_rcpsp.components_graph_constraints[
-                    neighbor_fix_problem.graph_rcpsp.index_components[t1]
+        if constraints.start_times_window[t][1] is not None:
+            if solution.get_start_time(t) > constraints.start_times_window[t][1]:
+                list_constraints_not_respected += [
+                    (
+                        "start_window_1",
+                        t,
+                        t,
+                        None,
+                        None,
+                        -constraints.start_times_window[t][1]
+                        + solution.get_start_time(t),
+                    )
                 ]
-            )
-            for c in set(
-                neighbor_fix_problem.graph_rcpsp.components_graph_constraints[
-                    neighbor_fix_problem.graph_rcpsp.index_components[t1]
+
+    for t in constraints.end_times_window:
+        if constraints.end_times_window[t][0] is not None:
+            if solution.get_end_time(t) < constraints.end_times_window[t][0]:
+                list_constraints_not_respected += [
+                    (
+                        "end_window_0",
+                        t,
+                        t,
+                        None,
+                        None,
+                        constraints.end_times_window[t][0] - solution.get_end_time(t),
+                    )
                 ]
-            ):
-                subtasks.update(neighbor_fix_problem.graph_rcpsp.get_next_activities(c))
-                subtasks.update(
-                    neighbor_fix_problem.graph_rcpsp.get_descendants_activities(c)
-                )
-                subtasks.update(
-                    neighbor_fix_problem.graph_rcpsp.get_ancestors_activities(c)
-                )
-                subtasks.update(neighbor_fix_problem.graph_rcpsp.get_pred_activities(c))
-            len_subtasks = len(subtasks)
-            j += 1
-        if len_subtasks < neighbor_fix_problem.nb_jobs_subproblem:
-            subtasks = create_subproblem_cut_time(
-                current_solution, neighbor_fix_problem, subtasks
-            )
-        return subtasks
-    else:
-        return create_subproblem_cut_time(current_solution, neighbor_fix_problem)
 
+        if constraints.end_times_window[t][1] is not None:
+            if solution.get_end_time(t) > constraints.end_times_window[t][1]:
+                list_constraints_not_respected += [
+                    (
+                        "end_window_1",
+                        t,
+                        t,
+                        None,
+                        None,
+                        -constraints.end_times_window[t][1] + solution.get_end_time(t),
+                    )
+                ]
+    return list_constraints_not_respected
 
-class NeighborFlexibleStart(ConstraintHandler):
-    def __init__(
-        self,
-        problem: RCPSPModelPreemptive,
-        fraction_to_fix: float = 0.9,
-        minus_delta: int = 2,
-        plus_delta: int = 2,
-        delta_time_from_makepan_to_not_fix: int = 5,
-    ):
-        self.problem = problem
-        self.fraction_to_fix = fraction_to_fix
-        self.minus_delta = minus_delta
-        self.plus_delta = plus_delta
-        self.delta_time_from_makepan_to_not_fix = delta_time_from_makepan_to_not_fix
 
-    def adding_constraint_from_results_store(
-        self,
-        cp_solver: Union[CP_RCPSP_MZN_PREEMPTIVE, CP_MRCPSP_MZN_PREEMPTIVE],
-        child_instance: Instance,
-        result_storage: ResultStorage,
-        last_result_store: Optional[ResultStorage] = None,
-    ) -> Iterable[Any]:
-        if last_result_store is not None:
-            current_solution, fit = next(
-                (
-                    last_result_store.list_solution_fits[j]
-                    for j in range(len(last_result_store.list_solution_fits))
-                    if "opti_from_cp"
-                    in last_result_store.list_solution_fits[j][0].__dict__.keys()
-                ),
-                (None, None),
-            )
+def check_solution(
+    problem: RCPSPModelSpecialConstraintsPreemptive,
+    solution: Union[
+        RCPSPSolutionSpecialPreemptive,
+        RCPSPSolution,
+        RCPSPSolutionPreemptive,
+    ],
+    relax_the_start_at_end: bool = True,
+):
+    if not solution.rcpsp_schedule_feasible:
+        return False
+    start_together = problem.special_constraints.start_together
+    start_at_end = problem.special_constraints.start_at_end
+    start_at_end_plus_offset = problem.special_constraints.start_at_end_plus_offset
+    start_after_nunit = problem.special_constraints.start_after_nunit
+    disjunctive = problem.special_constraints.disjunctive_tasks
+    for (t1, t2) in start_together:
+        if not relax_the_start_at_end:
+            b = solution.get_start_time(t1) == solution.get_start_time(t2)
+            if not b:
+                return False
+    for (t1, t2) in start_at_end:
+        if relax_the_start_at_end:
+            b = solution.get_start_time(t2) >= solution.get_end_time(t1)
         else:
-            current_solution, fit = next(
+            b = solution.get_start_time(t2) == solution.get_end_time(t1)
+        if not b:
+            return False
+    for (t1, t2, off) in start_at_end_plus_offset:
+        b = solution.get_start_time(t2) >= solution.get_end_time(t1) + off
+        if not b:
+            logger.debug(("start_at_end_plus_offset NOT respected: ", t1, t2, off))
+            logger.debug(
                 (
-                    result_storage.list_solution_fits[j]
-                    for j in range(len(result_storage.list_solution_fits))
-                    if "opti_from_cp"
-                    in result_storage.list_solution_fits[j][0].__dict__.keys()
-                ),
-                (None, None),
-            )
-        if current_solution is None or fit != result_storage.get_best_solution_fit()[1]:
-            current_solution, fit = result_storage.get_last_best_solution()
-        current_solution: RCPSPSolutionPreemptive = current_solution
-        max_time = get_max_time_solution(current_solution)
-        last_jobs = get_tasks_ending_between_two_times(
-            solution=current_solution,
-            time_1=max_time - self.delta_time_from_makepan_to_not_fix,
-            time_2=max_time,
-        )
-        nb_jobs = self.problem.n_jobs
-        jobs_to_fix = set(
-            random.sample(
-                list(current_solution.rcpsp_schedule),
-                int(self.fraction_to_fix * nb_jobs),
-            )
+                    solution.get_start_time(t2),
+                    " >= ",
+                    solution.get_end_time(t1),
+                    "+",
+                    off,
+                )
+            )
+            return False
+    for (t1, t2, off) in start_after_nunit:
+        b = solution.get_start_time(t2) >= solution.get_start_time(t1) + off
+        if not b:
+            logger.debug(("start_after_nunit NOT respected: ", t1, t2, off))
+            return False
+    for t1, t2 in disjunctive:
+        b = intersect(
+            [solution.get_start_time(t1), solution.get_end_time(t1)],
+            [solution.get_start_time(t2), solution.get_end_time(t2)],
         )
-        for lj in last_jobs:
-            if lj in jobs_to_fix:
-                jobs_to_fix.remove(lj)
-        list_strings = constraints_strings(
-            current_solution,
-            subtasks=jobs_to_fix,
-            minus_delta=self.minus_delta,
-            plus_delta=self.plus_delta,
-            jobs_to_fix=set(),
-            cp_solver=cp_solver,
-        )
-        for s in list_strings:
-            child_instance.add_string(s)
-        return list_strings
-
-    def remove_constraints_from_previous_iteration(
-        self,
-        cp_solver: CP_RCPSP_MZN,
-        child_instance,
-        previous_constraints: Iterable[Any],
-    ):
-        pass
-
-
-def get_ressource_breaks(
-    problem_calendar: RCPSPModelPreemptive, solution: RCPSPSolutionPreemptive
-):
-    ressources = problem_calendar.resources_list
-    ressource_arrays = {}
-    ressource_arrays_usage = {}
-    makespan = get_max_time_solution(solution=solution)
-    for r in ressources:
-        ressource_arrays[r] = np.zeros(makespan)
-        ressource_arrays_usage[r] = np.zeros((makespan, len(solution.rcpsp_schedule)))
-    sorted_keys_schedule = problem_calendar.tasks_list
-    modes = problem_calendar.build_mode_dict(solution.rcpsp_modes)
-    for ji in range(len(sorted_keys_schedule)):
-        j = sorted_keys_schedule[ji]
-        for r in problem_calendar.resources_list:
-            if problem_calendar.mode_details[j][modes[j]].get(r, 0) == 0:
-                continue
+        if b is not None:
+            return False
+    for t in problem.special_constraints.start_times_window:
+        if problem.special_constraints.start_times_window[t][0] is not None:
             if (
-                solution.rcpsp_schedule[j]["starts"][0]
-                == solution.rcpsp_schedule[j]["ends"][-1]
+                solution.get_start_time(t)
+                < problem.special_constraints.start_times_window[t][0]
             ):
-                continue
-            for s, e, index in zip(
-                solution.rcpsp_schedule[j]["starts"],
-                solution.rcpsp_schedule[j]["ends"],
-                range(len(solution.rcpsp_schedule[j]["starts"])),
+                logger.debug(
+                    (
+                        "start time 0, ",
+                        t,
+                        solution.get_start_time(t),
+                        problem.special_constraints.start_times_window[t][0],
+                    )
+                )
+                return False
+        if problem.special_constraints.start_times_window[t][1] is not None:
+            if (
+                solution.get_start_time(t)
+                > problem.special_constraints.start_times_window[t][1]
             ):
-                ressource_arrays_usage[r][s:e, ji] = index + 1
-                ressource_arrays[r][s:e] += problem_calendar.mode_details[j][modes[j]][
-                    r
-                ]
-    index_ressource = {}
-    task_concerned = {}
-    constraints = {}
-    for r in ressource_arrays:
-        if problem_calendar.is_varying_resource():
-            index = np.argwhere(
-                ressource_arrays[r] > problem_calendar.resources[r][:makespan]
-            )
-        else:
-            index = np.argwhere(ressource_arrays[r] > problem_calendar.resources[r])
-        index_ressource[r] = index
-        task_concerned[r] = [
-            j
-            for j in range(ressource_arrays_usage[r].shape[1])
-            if any(
-                ressource_arrays_usage[r][ind[0], j] >= 1
-                for ind in index
-                if problem_calendar.get_resource_available(r, ind[0]) == 0
-            )
-        ]
-        task_concerned[r] = [sorted_keys_schedule[rr] for rr in task_concerned[r]]
-        constraints[r] = {}
-        for t in task_concerned[r]:
-            current_start = solution.rcpsp_schedule[t]["starts"][0]
-            first_possible_start_future = next(
-                (
-                    st
-                    for st in range(current_start, problem_calendar.horizon)
-                    if problem_calendar.get_resource_available(r, st)
-                    >= problem_calendar.mode_details[t][modes[t]][r]
-                ),
-                None,
-            )
-            first_possible_start_before = next(
-                (
-                    st - problem_calendar.mode_details[t][modes[t]]["duration"] + 1
-                    for st in range(solution.rcpsp_schedule[t]["ends"][-1], -1, -1)
-                    if problem_calendar.get_resource_available(r, st - 1)
-                    >= problem_calendar.mode_details[t][modes[t]][r]
-                    and problem_calendar.get_resource_available(
-                        r,
-                        max(
-                            0,
-                            st
-                            - problem_calendar.mode_details[t][modes[t]]["duration"]
-                            + 1,
-                        ),
+                logger.debug(
+                    (
+                        "start time 1, ",
+                        t,
+                        solution.get_start_time(t),
+                        problem.special_constraints.start_times_window[t][1],
                     )
-                    >= problem_calendar.mode_details[t][1][r]
-                ),
-                None,
-            )
-            constraints[r][t] = (
-                first_possible_start_before,
-                first_possible_start_future,
-            )
-    return index_ressource, constraints
+                )
+                return False
+    for t in problem.special_constraints.end_times_window:
+        if problem.special_constraints.end_times_window[t][0] is not None:
+            if (
+                solution.get_end_time(t)
+                < problem.special_constraints.end_times_window[t][0]
+            ):
+                logger.debug(
+                    (
+                        "end time 0, ",
+                        t,
+                        solution.get_end_time(t),
+                        problem.special_constraints.end_times_window[t][0],
+                    )
+                )
+                return False
+        if problem.special_constraints.end_times_window[t][1] is not None:
+            if (
+                solution.get_end_time(t)
+                > problem.special_constraints.end_times_window[t][1]
+            ):
+                logger.debug(
+                    (
+                        "end time 1, ",
+                        t,
+                        solution.get_end_time(t),
+                        problem.special_constraints.end_times_window[t][1],
+                    )
+                )
+                return False
+    return True
 
 
-class PostProcessSolutionNonFeasible(PostProcessSolution):
-    def __init__(
-        self,
-        problem_calendar: RCPSPModelPreemptive,
-        problem_no_calendar: RCPSPModelPreemptive,
-        partial_solution: PartialSolutionPreemptive = None,
-        params_objective_function: ParamsObjectiveFunction = None,
-        do_ls=True,
-        **kwargs
-    ):
-        self.problem_calendar = problem_calendar
-        self.problem_no_calendar = problem_no_calendar
-        self.partial_solution = partial_solution
-        (
-            self.aggreg_from_sol,
-            self.aggreg_from_dict,
-            self.params_objective_function,
-        ) = build_aggreg_function_and_params_objective(
-            problem=self.problem_calendar,
-            params_objective_function=params_objective_function,
-        )
-        if self.partial_solution is None:
+def generate_schedule_from_permutation_serial_sgs_preemptive(
+    solution, rcpsp_problem: RCPSPModelSpecialConstraintsPreemptive
+):
+    activity_end_times = {}
 
-            def check_solution(problem, solution):
-                return True
+    unfeasible_non_renewable_resources = False
+    new_horizon = rcpsp_problem.horizon
 
+    resource_avail_in_time = {}
+    for res in rcpsp_problem.resources_list:
+        if rcpsp_problem.is_varying_resource():
+            resource_avail_in_time[res] = np.copy(
+                rcpsp_problem.resources[res][: new_horizon + 1]
+            )
         else:
+            resource_avail_in_time[res] = np.full(
+                new_horizon, rcpsp_problem.resources[res], dtype=np.int_
+            ).tolist()
+    minimum_starting_time = {}
+    for act in rcpsp_problem.tasks_list:
+        minimum_starting_time[act] = 0
+        if rcpsp_problem.do_special_constraints:
+            if act in rcpsp_problem.special_constraints.start_times_window:
+                minimum_starting_time[act] = (
+                    rcpsp_problem.special_constraints.start_times_window[act][0]
+                    if rcpsp_problem.special_constraints.start_times_window[act][0]
+                    is not None
+                    else 0
+                )
 
-            def check_solution(problem, solution):
-                start_together = partial_solution.start_together
-                start_at_end = partial_solution.start_at_end
-                start_at_end_plus_offset = partial_solution.start_at_end_plus_offset
-                start_after_nunit = partial_solution.start_after_nunit
-                for (t1, t2) in start_together:
-                    b = (
-                        solution.rcpsp_schedule[t1]["starts"][0]
-                        == solution.rcpsp_schedule[t2]["starts"][0]
-                    )
-                    if not b:
-                        return False
-                for (t1, t2) in start_at_end:
-                    b = (
-                        solution.rcpsp_schedule[t2]["starts"][0]
-                        == solution.rcpsp_schedule[t1]["ends"][-1]
-                    )
-                    if not b:
-                        return False
-                for (t1, t2, off) in start_at_end_plus_offset:
-                    b = (
-                        solution.rcpsp_schedule[t2]["starts"][0]
-                        >= solution.rcpsp_schedule[t1]["ends"][-1] + off
-                    )
-                    if not b:
-                        return False
-                for (t1, t2, off) in start_after_nunit:
-                    b = (
-                        solution.rcpsp_schedule[t2]["starts"][0]
-                        >= solution.rcpsp_schedule[t1]["starts"][0] + off
-                    )
-                    if not b:
-                        return False
-                return True
-
-        self.check_sol = check_solution
-        self.do_ls = do_ls
-        self.dict_params = kwargs
-
-    def build_other_solution(self, result_storage: ResultStorage) -> ResultStorage:
-        for sol in list(result_storage.list_solution_fits):
-            solution: RCPSPSolutionPreemptive = sol[0]
-            if "satisfy" not in solution.__dict__.keys():
-                rb, constraints = get_ressource_breaks(self.problem_calendar, solution)
-                solution.satisfy = not (any(len(rb[r]) > 0 for r in rb))
-                solution.constraints = constraints
-            if self.partial_solution is None:
-                solution_p = RCPSPSolutionPreemptive(
-                    problem=self.problem_calendar,
-                    rcpsp_permutation=solution.rcpsp_permutation,
-                    rcpsp_modes=solution.rcpsp_modes,
+    perm_extended = [
+        rcpsp_problem.tasks_list_non_dummy[x] for x in solution.rcpsp_permutation
+    ]
+    perm_extended.insert(0, rcpsp_problem.source_task)
+    perm_extended.append(rcpsp_problem.sink_task)
+    modes_dict = rcpsp_problem.build_mode_dict(solution.rcpsp_modes)
+
+    for k in modes_dict:
+        if modes_dict[k] not in rcpsp_problem.mode_details[k]:
+            modes_dict[k] = 1
+    expected_durations_task = {
+        k: rcpsp_problem.mode_details[k][modes_dict[k]]["duration"] for k in modes_dict
+    }
+    schedules = {}
+
+    def ressource_consumption(res, task, duration, mode):
+        dur = rcpsp_problem.mode_details[task][mode]["duration"]
+        if duration > dur:
+            return 0
+        return rcpsp_problem.mode_details[task][mode].get(res, 0)
+
+    def look_for_task(perm, ignore_sc=False):
+        act_ids = []
+        for task_id in perm:
+            respected = True
+            # Check all kind of precedence constraints....
+            for pred in rcpsp_problem.predecessors.get(task_id, {}):
+                if pred in perm_extended:
+                    respected = False
+                    break
+            if not ignore_sc:
+                for (
+                    pred
+                ) in rcpsp_problem.special_constraints.dict_start_at_end_reverse.get(
+                    task_id, {}
+                ):
+                    if pred in perm_extended:
+                        respected = False
+                        break
+                for (
+                    pred
+                ) in rcpsp_problem.special_constraints.dict_start_at_end_offset_reverse.get(
+                    task_id, {}
+                ):
+                    if pred in perm_extended:
+                        respected = False
+                        break
+                for (
+                    pred
+                ) in rcpsp_problem.special_constraints.dict_start_after_nunit_reverse.get(
+                    task_id, {}
+                ):
+                    if pred in perm_extended:
+                        respected = False
+                        break
+            task_to_start_too = set()
+            if respected:
+                task_to_start_too = (
+                    rcpsp_problem.special_constraints.dict_start_together.get(
+                        task_id, set()
+                    )
                 )
-                solution_p.satisfy = self.check_sol(self.problem_calendar, solution_p)
-                result_storage.list_solution_fits += [
-                    (solution_p, -self.aggreg_from_sol(solution_p))
-                ]
-        if self.do_ls:
-            solver = LS_RCPSP_Solver(
-                problem=self.problem_calendar, ls_solver=LS_SOLVER.SA
-            )
-            satisfiable = [
-                (s, f) for s, f in result_storage.list_solution_fits if s.satisfy
+                if not ignore_sc:
+                    if len(task_to_start_too) > 0:
+                        if not all(
+                            s not in perm_extended
+                            for t in task_to_start_too
+                            for s in rcpsp_problem.predecessors[t]
+                        ):
+                            respected = False
+                        if not all(
+                            s not in perm_extended
+                            for t in task_to_start_too
+                            for s in rcpsp_problem.special_constraints.dict_start_at_end_reverse.get(
+                                t, {}
+                            )
+                        ):
+                            respected = False
+                        if not all(
+                            s not in perm_extended
+                            for t in task_to_start_too
+                            for s in rcpsp_problem.special_constraints.dict_start_at_end_offset_reverse.get(
+                                t, {}
+                            )
+                        ):
+                            respected = False
+                        if not all(
+                            s not in perm_extended
+                            for t in task_to_start_too
+                            for s in rcpsp_problem.special_constraints.dict_start_after_nunit_reverse.get(
+                                t, {}
+                            )
+                        ):
+                            respected = False
+            if respected:
+                act_ids = [task_id] + list(task_to_start_too)
+                break
+        return act_ids
+
+    unfeasible = False
+    while len(perm_extended) > 0 and not unfeasible_non_renewable_resources:
+        act_ids = look_for_task(
+            [
+                k
+                for k in rcpsp_problem.special_constraints.dict_start_at_end_reverse
+                if k in perm_extended
             ]
-            if len(satisfiable) > 0:
-                s: RCPSPSolutionPreemptive = max(satisfiable, key=lambda x: x[1])[
-                    0
-                ].copy()
+        )
+        if len(act_ids) == 0:
+            act_ids = look_for_task(perm_extended)
+        if (
+            len(act_ids) == 0
+        ):  # The constraints in the model are not necessarly trustable, leading to this problem.
+            act_ids = look_for_task(perm_extended, ignore_sc=True)
+        current_min_time = max([minimum_starting_time[act_id] for act_id in act_ids])
+        starts = {act_id: [] for act_id in act_ids}
+        ends = {act_id: [] for act_id in act_ids}
+        cur_duration = {act_id: 0 for act_id in act_ids}
+        valid = False
+        first_step = (
+            False  # we force the starting of all act_id to be the same current time
+        )
+        while not valid:
+            if all(expected_durations_task[act_id] for act_id in act_ids) == 0:
+                for act_id in act_ids:
+                    starts[act_id] += [current_min_time]
+                    ends[act_id] += [current_min_time]
+                    cur_duration[act_id] += ends[act_id][-1] - starts[act_id][-1]
             else:
-                s = result_storage.get_best_solution().copy()
-            if self.problem_calendar != s.problem:
-                s.change_problem(self.problem_calendar)
-            result_store = solver.solve(
-                nb_iteration_max=self.dict_params.get("nb_iteration_max", 200),
-                init_solution=s,
+                reached_end = True
+                if not first_step:
+                    current_min_time = next(
+                        (
+                            t
+                            for t in range(current_min_time, new_horizon)
+                            if all(
+                                resource_avail_in_time[res][t]
+                                >= sum(
+                                    [
+                                        ressource_consumption(
+                                            res=res,
+                                            task=ac,
+                                            mode=modes_dict[ac],
+                                            duration=cur_duration[ac],
+                                        )
+                                        for ac in act_ids
+                                    ]
+                                )
+                                for res in rcpsp_problem.resources_list
+                            )
+                        ),
+                        None,
+                    )
+                    if current_min_time is None:
+                        unfeasible = True
+                        break
+                    current_min_time_dict = {ac: current_min_time for ac in act_ids}
+                    first_step = True
+                reached_dict = {}
+                for ac in act_ids:
+                    reached_t = None
+                    for t in range(
+                        current_min_time_dict[ac],
+                        current_min_time_dict[ac]
+                        + expected_durations_task[ac]
+                        - cur_duration[ac],
+                    ):
+                        if t >= new_horizon:
+                            reached_end = False
+                            unfeasible_non_renewable_resources = True
+                            break
+                        if any(
+                            resource_avail_in_time[res][t]
+                            < rcpsp_problem.mode_details[ac][modes_dict[ac]].get(res, 0)
+                            for res in rcpsp_problem.resources_list
+                        ):
+                            reached_end = False
+                            break
+                        else:
+                            reached_t = t
+                    reached_dict[ac] = reached_t
+                    if reached_t is not None and rcpsp_problem.can_be_preempted(ac):
+                        starts[ac] += [current_min_time_dict[ac]]
+                        ends[ac] += [reached_dict[ac] + 1]
+                        cur_duration[ac] += ends[ac][-1] - starts[ac][-1]
+                        for res in rcpsp_problem.resources_list:
+                            for t in range(starts[ac][-1], ends[ac][-1]):
+                                resource_avail_in_time[res][
+                                    t
+                                ] -= rcpsp_problem.mode_details[ac][modes_dict[ac]].get(
+                                    res, 0
+                                )
+                                if resource_avail_in_time[res][t] < 0:
+                                    logger.warning(
+                                        "Resources available should not be negative"
+                                    )
+                    if (
+                        reached_end
+                        and reached_dict[ac] is not None
+                        and not rcpsp_problem.can_be_preempted(ac)
+                    ):
+                        starts[ac] += [current_min_time_dict[ac]]
+                        ends[ac] += [reached_dict[ac] + 1]
+                        cur_duration[ac] += ends[ac][-1] - starts[ac][-1]
+                        for res in rcpsp_problem.resources_list:
+                            for t in range(starts[ac][-1], ends[ac][-1]):
+                                resource_avail_in_time[res][
+                                    t
+                                ] -= rcpsp_problem.mode_details[ac][modes_dict[ac]].get(
+                                    res, 0
+                                )
+                                if resource_avail_in_time[res][t] < 0:
+                                    logger.warning(
+                                        "Resources available should not be negative"
+                                    )
+                                if (
+                                    res in rcpsp_problem.non_renewable_resources
+                                    and t == ends[ac][-1] - 1
+                                ):
+                                    for tt in range(t + 1, new_horizon):
+                                        resource_avail_in_time[res][
+                                            tt
+                                        ] -= rcpsp_problem.mode_details[ac][
+                                            modes_dict[ac]
+                                        ].get(
+                                            res, 0
+                                        )
+                                        if resource_avail_in_time[res][tt] < 0:
+                                            unfeasible_non_renewable_resources = True
+            valid = all(
+                cur_duration[ac] == expected_durations_task[ac] for ac in act_ids
+            )
+            if not valid:
+                current_min_time_dict = {
+                    ac: next(
+                        (
+                            t
+                            for t in range(
+                                reached_dict[ac] + 2
+                                if reached_dict[ac] is not None
+                                else current_min_time_dict[ac] + 1,
+                                new_horizon,
+                            )
+                            if all(
+                                resource_avail_in_time[res][t]
+                                >= sum(
+                                    [
+                                        ressource_consumption(
+                                            res=res,
+                                            task=ac,
+                                            mode=modes_dict[ac],
+                                            duration=cur_duration[ac] + 1,
+                                        )
+                                    ]
+                                )
+                                for res in rcpsp_problem.resources_list
+                            )
+                        ),
+                        None,
+                    )
+                    for ac in act_ids
+                }
+                if any(
+                    current_min_time_dict[ac] is None for ac in current_min_time_dict
+                ):
+                    unfeasible = True
+                    break
+        if not unfeasible_non_renewable_resources and not unfeasible:
+            for ac in starts:
+                activity_end_times[ac] = ends[ac][-1]
+                schedules[ac] = (starts[ac], ends[ac])
+                perm_extended.remove(ac)
+                for s in rcpsp_problem.successors[ac]:
+                    minimum_starting_time[s] = max(
+                        minimum_starting_time[s], activity_end_times[ac]
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_at_end.get(
+                    ac, {}
+                ):
+                    minimum_starting_time[s] = max(
+                        minimum_starting_time[s], activity_end_times[ac]
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_after_nunit.get(
+                    ac, {}
+                ):
+                    minimum_starting_time[s] = max(
+                        starts[ac][0]
+                        + rcpsp_problem.special_constraints.dict_start_after_nunit[ac][
+                            s
+                        ],
+                        minimum_starting_time[s],
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_at_end_offset.get(
+                    ac, {}
+                ):
+                    minimum_starting_time[s] = max(
+                        activity_end_times[ac]
+                        + rcpsp_problem.special_constraints.dict_start_at_end_offset[
+                            ac
+                        ][s],
+                        minimum_starting_time[s],
+                    )
+        else:
+            break
+    rcpsp_schedule = {}
+    for act_id in activity_end_times:
+        rcpsp_schedule[act_id] = {}
+        rcpsp_schedule[act_id]["starts"] = schedules[act_id][0]
+        rcpsp_schedule[act_id]["ends"] = schedules[act_id][1]
+    if unfeasible_non_renewable_resources or unfeasible:
+        logger.debug(
+            (
+                "unfeasible: ",
+                unfeasible,
+                "unfeasible_non_renewable_resources: ",
+                unfeasible_non_renewable_resources,
             )
-            for solution, f in result_store.list_solution_fits:
-                solution.satisfy = self.check_sol(self.problem_calendar, solution)
-                result_storage.list_solution_fits += [
-                    (solution, -self.aggreg_from_sol(solution))
-                ]
-        return result_storage
+        )
+        rcpsp_schedule_feasible = False
+        last_act_id = rcpsp_problem.sink_task
+        if last_act_id not in rcpsp_schedule:
+            rcpsp_schedule[last_act_id] = {}
+            rcpsp_schedule[last_act_id]["starts"] = [9999999]
+            rcpsp_schedule[last_act_id]["ends"] = [9999999]
+    else:
+        rcpsp_schedule_feasible = True
+    return rcpsp_schedule, rcpsp_schedule_feasible
 
 
-class ConstraintHandlerAddCalendarConstraint(ConstraintHandler):
-    def __init__(
-        self,
-        problem_calendar: RCPSPModelPreemptive,
-        problem_no_calendar: RCPSPModelPreemptive,
-        other_constraint: ConstraintHandler,
-    ):
-        self.problem_calendar = problem_calendar
-        self.problem_no_calendar = problem_no_calendar
-        self.other_constraint = other_constraint
-        self.store_constraints = set()
+def generate_schedule_from_permutation_serial_sgs_partial_schedule_preempptive(
+    solution,
+    rcpsp_problem,
+    partial_schedule: Dict[Hashable, Dict[str, List[int]]],
+    current_t,
+    completed_tasks,
+):
+    activity_end_times = {}
+    unfeasible_non_renewable_resources = False
+    new_horizon = rcpsp_problem.horizon
+    resource_avail_in_time = {}
+    for res in rcpsp_problem.resources_list:
+        if rcpsp_problem.is_varying_resource():
+            resource_avail_in_time[res] = list(
+                rcpsp_problem.resources[res][: new_horizon + 1]
+            )
+        else:
+            resource_avail_in_time[res] = np.full(
+                new_horizon, rcpsp_problem.resources[res], dtype=np.int_
+            ).tolist()
+    minimum_starting_time = {}
+    for act in rcpsp_problem.tasks_list:
+        minimum_starting_time[act] = current_t
+
+        if rcpsp_problem.do_special_constraints:
+            if act in rcpsp_problem.special_constraints.start_times_window:
+                minimum_starting_time[act] = (
+                    max(
+                        rcpsp_problem.special_constraints.start_times_window[act][0],
+                        minimum_starting_time[act],
+                    )
+                    if rcpsp_problem.special_constraints.start_times_window[act][0]
+                    is not None
+                    else minimum_starting_time[act]
+                )
+    perm_extended = [
+        rcpsp_problem.tasks_list_non_dummy[x] for x in solution.rcpsp_permutation
+    ]
+    perm_extended.insert(0, rcpsp_problem.source_task)
+    perm_extended.append(rcpsp_problem.sink_task)
 
-    def adding_constraint_from_results_store(
-        self,
-        cp_solver: Union[CP_RCPSP_MZN_PREEMPTIVE, CP_MRCPSP_MZN_PREEMPTIVE],
-        child_instance: Instance,
-        result_storage: ResultStorage,
-        last_result_store: Optional[ResultStorage] = None,
-    ) -> Iterable[Any]:
-        if last_result_store is None:
-            raise ValueError("This constraint need last_result_store to be not None.")
-        list_strings = []
-        r = random.random()
-        if r <= 0.2:
-            solution, fit = last_result_store.get_last_best_solution()
-        elif r <= 0.4:
-            solution, fit = last_result_store.get_best_solution_fit()
-        elif r <= 0.99:
-            solution, fit = last_result_store.get_random_best_solution()
+    modes_dict = rcpsp_problem.build_mode_dict(solution.rcpsp_modes)
+    for k in modes_dict:
+        if modes_dict[k] not in rcpsp_problem.mode_details[k]:
+            modes_dict[k] = 1
+    expected_durations_task = {
+        k: rcpsp_problem.mode_details[k][modes_dict[k]]["duration"] for k in modes_dict
+    }
+    done_duration_task = {k: 0 for k in modes_dict}
+    schedules = deepcopy(partial_schedule)
+    # Update current resource usage by the scheduled task (ongoing task, in practice)
+    for task in partial_schedule:
+        starts = partial_schedule[task]["starts"]
+        ends = partial_schedule[task]["ends"]
+        done_duration_task[task] = sum(
+            [ends[i] - starts[i] for i in range(len(starts))]
+        )
+        end_t = ends[-1]
+        for s, e in zip(starts, ends):
+            for t in range(s, e):
+                for res in resource_avail_in_time:
+                    resource_avail_in_time[res][t] -= rcpsp_problem.mode_details[task][
+                        modes_dict[task]
+                    ].get(res, 0)
+                    if res in rcpsp_problem.non_renewable_resources and t == end_t - 1:
+                        for tt in range(end_t, new_horizon):
+                            resource_avail_in_time[res][
+                                tt
+                            ] -= rcpsp_problem.mode_details[task][modes_dict[task]].get(
+                                res, 0
+                            )
+                            if resource_avail_in_time[res][tt] < 0:
+                                unfeasible_non_renewable_resources = True
+        if done_duration_task[task] == expected_durations_task[task]:
+            activity_end_times[task] = end_t
+            perm_extended.remove(task)
+            for s in rcpsp_problem.successors[task]:
+                minimum_starting_time[s] = max(
+                    minimum_starting_time[s], activity_end_times[task]
+                )
         else:
-            solution, fit = last_result_store.get_random_solution()
-        for s in self.store_constraints:  # we keep trace of already
-            child_instance.add_string(s)
-        if "satisfy" in solution.__dict__.keys() and solution.satisfy:
-            return self.other_constraint.adding_constraint_from_results_store(
-                cp_solver, child_instance, result_storage, last_result_store
-            )
-        ressource_breaks, constraints = get_ressource_breaks(
-            self.problem_calendar, solution
+            minimum_starting_time[task] = ends[-1]
+    perm_extended = [x for x in perm_extended if x not in completed_tasks]
+    # fix modes in case specified mode not in mode details for the activites
+    for ac in modes_dict:
+        if modes_dict[ac] not in rcpsp_problem.mode_details[ac]:
+            modes_dict[ac] = 1
+
+    def ressource_consumption(res, task, duration, mode):
+        dur = rcpsp_problem.mode_details[task][mode]["duration"]
+        if duration > dur:
+            return 0
+        return rcpsp_problem.mode_details[task][mode].get(res, 0)
+
+    def look_for_task(perm):
+        act_ids = []
+        for task_id in perm:
+            respected = True
+            # Check all kind of precedence constraints....
+            for pred in rcpsp_problem.predecessors.get(task_id, {}):
+                if pred in perm_extended:
+                    respected = False
+                    break
+            for pred in rcpsp_problem.special_constraints.dict_start_at_end_reverse.get(
+                task_id, {}
+            ):
+                if pred in perm_extended:
+                    respected = False
+                    break
+            for (
+                pred
+            ) in rcpsp_problem.special_constraints.dict_start_at_end_offset_reverse.get(
+                task_id, {}
+            ):
+                if pred in perm_extended:
+                    respected = False
+                    break
+            for (
+                pred
+            ) in rcpsp_problem.special_constraints.dict_start_after_nunit_reverse.get(
+                task_id, {}
+            ):
+                if pred in perm_extended:
+                    respected = False
+                    break
+            task_to_start_too = set()
+            if respected:
+                task_to_start_too = (
+                    rcpsp_problem.special_constraints.dict_start_together.get(
+                        task_id, set()
+                    )
+                )
+                if len(task_to_start_too) > 0:
+                    if not all(
+                        s not in perm_extended
+                        for t in task_to_start_too
+                        for s in rcpsp_problem.predecessors[t]
+                    ):
+                        respected = False
+                    if not all(
+                        s not in perm_extended
+                        for t in task_to_start_too
+                        for s in rcpsp_problem.special_constraints.dict_start_at_end_reverse.get(
+                            t, {}
+                        )
+                    ):
+                        respected = False
+                    if not all(
+                        s not in perm_extended
+                        for t in task_to_start_too
+                        for s in rcpsp_problem.special_constraints.dict_start_at_end_offset_reverse.get(
+                            t, {}
+                        )
+                    ):
+                        respected = False
+                    if not all(
+                        s not in perm_extended
+                        for t in task_to_start_too
+                        for s in rcpsp_problem.special_constraints.dict_start_after_nunit_reverse.get(
+                            t, {}
+                        )
+                    ):
+                        respected = False
+            if respected:
+                act_ids = [task_id] + list(task_to_start_too)
+                break
+        return act_ids
+
+    while len(perm_extended) > 0 and not unfeasible_non_renewable_resources:
+        act_ids = look_for_task(
+            [
+                k
+                for k in rcpsp_problem.special_constraints.dict_start_at_end_reverse
+                if k in perm_extended
+            ]
+        )
+        if len(act_ids) == 0:
+            act_ids = look_for_task(perm_extended)
+        current_min_time = max([minimum_starting_time[act_id] for act_id in act_ids])
+        starts = {act_id: [] for act_id in act_ids}
+        ends = {act_id: [] for act_id in act_ids}
+        cur_duration = {act_id: 0 for act_id in act_ids}
+        valid = False
+        first_step = (
+            False  # we force the starting of all act_id to be the same current time
         )
-        for r in ressource_breaks:
-            if len(ressource_breaks[r]) == 0:
-                continue
-            prev_time = None
-            for index_range in range(len(ressource_breaks[r])):
-                ind = ressource_breaks[r][index_range][0]
-                if (prev_time is None or ind >= prev_time + 20) or (
-                    index_range >= 1
-                    and ind > ressource_breaks[r][index_range - 1][0] + 1
+        while not valid:
+            if all(expected_durations_task[act_id] for act_id in act_ids) == 0:
+                for act_id in act_ids:
+                    starts[act_id] += [current_min_time]
+                    ends[act_id] += [current_min_time]
+                    cur_duration[act_id] += ends[act_id][-1] - starts[act_id][-1]
+            else:
+                reached_end = True
+                if not first_step:
+                    current_min_time = next(
+                        t
+                        for t in range(current_min_time, new_horizon)
+                        if all(
+                            resource_avail_in_time[res][t]
+                            >= sum(
+                                [
+                                    ressource_consumption(
+                                        res=res,
+                                        task=ac,
+                                        mode=modes_dict[ac],
+                                        duration=cur_duration[ac],
+                                    )
+                                    for ac in act_ids
+                                ]
+                            )
+                            for res in rcpsp_problem.resources_list
+                        )
+                    )
+                    current_min_time_dict = {ac: current_min_time for ac in act_ids}
+                    first_step = True
+                reached_dict = {}
+                for ac in act_ids:
+                    reached_t = None
+                    for t in range(
+                        current_min_time_dict[ac],
+                        current_min_time_dict[ac]
+                        + expected_durations_task[ac]
+                        - cur_duration[ac],
+                    ):
+                        if t >= new_horizon:
+                            reached_end = False
+                            unfeasible_non_renewable_resources = True
+                            break
+                        if any(
+                            resource_avail_in_time[res][t]
+                            < rcpsp_problem.mode_details[ac][modes_dict[ac]].get(res, 0)
+                            for res in rcpsp_problem.resources_list
+                        ):
+                            reached_end = False
+                            break
+                        else:
+                            reached_t = t
+                    reached_dict[ac] = reached_t
+                    if reached_t is not None and rcpsp_problem.can_be_preempted(ac):
+                        starts[ac] += [current_min_time_dict[ac]]
+                        ends[ac] += [reached_dict[ac] + 1]
+                        cur_duration[ac] += ends[ac][-1] - starts[ac][-1]
+                        for res in rcpsp_problem.resources_list:
+                            for t in range(starts[ac][-1], ends[ac][-1]):
+                                resource_avail_in_time[res][
+                                    t
+                                ] -= rcpsp_problem.mode_details[ac][modes_dict[ac]][res]
+                                if resource_avail_in_time[res][t] < 0:
+                                    logger.warning(
+                                        "Resources available should not be negative"
+                                    )
+                    if (
+                        reached_end
+                        and reached_dict[ac] is not None
+                        and not rcpsp_problem.can_be_preempted(ac)
+                    ):
+                        starts[ac] += [current_min_time_dict[ac]]
+                        ends[ac] += [reached_dict[ac] + 1]
+                        cur_duration[ac] += ends[ac][-1] - starts[ac][-1]
+                        for res in rcpsp_problem.resources_list:
+                            for t in range(starts[ac][-1], ends[ac][-1]):
+                                resource_avail_in_time[res][
+                                    t
+                                ] -= rcpsp_problem.mode_details[ac][modes_dict[ac]][res]
+                                if resource_avail_in_time[res][t] < 0:
+                                    logger.warning(
+                                        "Resources available should not be negative"
+                                    )
+                                if (
+                                    res in rcpsp_problem.non_renewable_resources
+                                    and t == ends[ac][-1] - 1
+                                ):
+                                    for tt in range(t + 1, new_horizon):
+                                        resource_avail_in_time[res][
+                                            tt
+                                        ] -= rcpsp_problem.mode_details[ac][
+                                            modes_dict[ac]
+                                        ][
+                                            res
+                                        ]
+                                        if resource_avail_in_time[res][tt] < 0:
+                                            unfeasible_non_renewable_resources = True
+            valid = all(
+                cur_duration[ac] == expected_durations_task[ac] for ac in act_ids
+            )
+            if not valid:
+                current_min_time_dict = {
+                    ac: next(
+                        t
+                        for t in range(
+                            reached_dict[ac] + 2
+                            if reached_dict[ac] is not None
+                            else current_min_time_dict[ac] + 1,
+                            new_horizon,
+                        )
+                        if all(
+                            resource_avail_in_time[res][t]
+                            >= sum(
+                                [
+                                    ressource_consumption(
+                                        res=res,
+                                        task=ac,
+                                        mode=modes_dict[ac],
+                                        duration=cur_duration[ac] + 1,
+                                    )
+                                ]
+                            )
+                            for res in rcpsp_problem.resources_list
+                        )
+                    )
+                    for ac in act_ids
+                }
+        if not unfeasible_non_renewable_resources:
+            for ac in starts:
+                activity_end_times[ac] = ends[ac][-1]
+                schedules[ac] = (starts[ac], ends[ac])
+                perm_extended.remove(ac)
+                for s in rcpsp_problem.successors[ac]:
+                    minimum_starting_time[s] = max(
+                        minimum_starting_time[s], activity_end_times[ac]
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_at_end.get(
+                    ac, {}
                 ):
-                    prev_time = ind
-                else:
-                    continue
-                rq = self.problem_calendar.get_resource_available(r, ind)
-                s = cp_solver.constraint_ressource_requirement_at_time_t(
-                    time=ind, ressource=r, ressource_number=rq, sign=SignEnum.UEQ
-                )
-                child_instance.add_string(s)
-                list_strings += [s]
-        satisfiable = [
-            (s, f)
-            for s, f in last_result_store.list_solution_fits
-            if "satisfy" in s.__dict__.keys() and s.satisfy
-        ]
-        if len(satisfiable) > 0:
-            res = ResultStorage(
-                list_solution_fits=satisfiable, mode_optim=result_storage.mode_optim
-            )
-            self.other_constraint.adding_constraint_from_results_store(
-                cp_solver, child_instance, res, last_result_store
-            )
-        self.store_constraints.update(list_strings)
-        return self.store_constraints
-
-    def remove_constraints_from_previous_iteration(
-        self,
-        cp_solver: CP_RCPSP_MZN,
-        child_instance,
-        previous_constraints: Iterable[Any],
-    ):
-        pass
-
-
-class OptionNeighbor(Enum):
-    MIX_ALL = 0
-    MIX_FAST = 1
-    MIX_LARGE_NEIGH = 2
-    LARGE = 4
-    DEBUG = 3
-
-
-class Params:
-    fraction_to_fix: float
-    minus_delta: int
-    plus_delta: int
-    delta_time_from_makepan_to_not_fix: int
-
-    def __init__(
-        self,
-        fraction_to_fix: float = 0.9,
-        minus_delta: int = 2,
-        plus_delta: int = 2,
-        delta_time_from_makepan_to_not_fix: int = 5,
-    ):
-        self.fraction_to_fix = fraction_to_fix
-        self.minus_delta = minus_delta
-        self.plus_delta = plus_delta
-        self.delta_time_from_makepan_to_not_fix = delta_time_from_makepan_to_not_fix
+                    minimum_starting_time[s] = max(
+                        minimum_starting_time[s], activity_end_times[ac]
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_after_nunit.get(
+                    ac, {}
+                ):
+                    minimum_starting_time[s] = max(
+                        starts[ac][0]
+                        + rcpsp_problem.special_constraints.dict_start_after_nunit[ac][
+                            s
+                        ],
+                        minimum_starting_time[s],
+                    )
+                for s in rcpsp_problem.special_constraints.dict_start_at_end_offset.get(
+                    ac, {}
+                ):
+                    minimum_starting_time[s] = max(
+                        activity_end_times[ac]
+                        + rcpsp_problem.special_constraints.dict_start_at_end_offset[
+                            ac
+                        ][s],
+                        minimum_starting_time[s],
+                    )
+    rcpsp_schedule = {}
+    for act_id in activity_end_times:
+        rcpsp_schedule[act_id] = schedules[act_id]
+    for act_id in completed_tasks:
+        rcpsp_schedule[act_id] = partial_schedule[act_id]
+    if unfeasible_non_renewable_resources:
+        rcpsp_schedule_feasible = False
+        last_act_id = rcpsp_problem.sink_task
+        if last_act_id not in rcpsp_schedule:
+            rcpsp_schedule[last_act_id] = {}
+            rcpsp_schedule[last_act_id]["starts"] = [99999999]
+            rcpsp_schedule[last_act_id]["ends"] = [9999999]
+    else:
+        rcpsp_schedule_feasible = True
+    return rcpsp_schedule, rcpsp_schedule_feasible
 
 
-class ConstraintHandlerMix(ConstraintHandler):
-    def __init__(
-        self,
-        problem: RCPSPModelPreemptive,
-        list_params: List[Params],
-        list_proba: List[float],
-    ):
-        self.problem = problem
-        self.list_params = list_params
-        self.list_proba = list_proba
-        if isinstance(self.list_proba, list):
-            self.list_proba = np.array(self.list_proba)
-        self.list_proba = self.list_proba / np.sum(self.list_proba)
-        self.index_np = np.array(range(len(self.list_proba)), dtype=np.int_)
-        self.current_iteration = 0
-        self.status = {
-            i: {"nb_usage": 0, "nb_improvement": 0}
-            for i in range(len(self.list_params))
-        }
-        self.last_index_param = None
-        self.last_fitness = None
+def create_np_data_and_jit_functions(
+    rcpsp_problem: Union[RCPSPModelSpecialConstraintsPreemptive],
+):
+    consumption_array = np.zeros(
+        (
+            rcpsp_problem.n_jobs,
+            rcpsp_problem.max_number_of_mode,
+            len(rcpsp_problem.resources_list),
+        ),
+        dtype=np.int_,
+    )
+    duration_array = np.zeros(
+        (rcpsp_problem.n_jobs, rcpsp_problem.max_number_of_mode), dtype=np.int_
+    )
+    predecessors = np.zeros((rcpsp_problem.n_jobs, rcpsp_problem.n_jobs), dtype=np.int_)
+    successors = np.zeros((rcpsp_problem.n_jobs, rcpsp_problem.n_jobs), dtype=np.int_)
+    preemptive_tag = np.zeros(rcpsp_problem.n_jobs, dtype=np.bool_)
+    horizon = rcpsp_problem.horizon
+    ressource_available = np.zeros(
+        (len(rcpsp_problem.resources_list), horizon), dtype=np.int_
+    )
+    ressource_renewable = np.ones((len(rcpsp_problem.resources_list)), dtype=bool)
+    min_duration_preemptive_bool = np.zeros(rcpsp_problem.n_jobs, dtype=bool)
+    min_duration_preemptive = np.zeros(rcpsp_problem.n_jobs, dtype=np.int_)
+    for i in range(len(rcpsp_problem.tasks_list)):
+        task = rcpsp_problem.tasks_list[i]
+        min_duration_preemptive_bool[i] = rcpsp_problem.duration_subtask[task][0]
+        min_duration_preemptive[i] = rcpsp_problem.duration_subtask[task][1]
+
+    for i in range(len(rcpsp_problem.tasks_list)):
+        task = rcpsp_problem.tasks_list[i]
+        preemptive_tag[i] = rcpsp_problem.can_be_preempted(task)
+        index_mode = 0
+        for mode in sorted(
+            rcpsp_problem.mode_details[rcpsp_problem.tasks_list[i]].keys()
+        ):
+            for k in range(len(rcpsp_problem.resources_list)):
+                consumption_array[i, index_mode, k] = rcpsp_problem.mode_details[task][
+                    mode
+                ].get(rcpsp_problem.resources_list[k], 0)
+            duration_array[i, index_mode] = rcpsp_problem.mode_details[task][mode][
+                "duration"
+            ]
+            index_mode += 1
 
-    def adding_constraint_from_results_store(
-        self,
-        cp_solver: Union[CP_MRCPSP_MZN_PREEMPTIVE, CP_RCPSP_MZN_PREEMPTIVE],
-        child_instance: Instance,
-        result_storage: ResultStorage,
-        last_result_store: Optional[ResultStorage] = None,
-    ) -> Iterable[Any]:
-        new_fitness = result_storage.get_best_solution_fit()[1]
-        if self.last_index_param is not None:
-            if new_fitness != self.last_fitness:
-                self.status[self.last_index_param]["nb_improvement"] += 1
-                self.last_fitness = new_fitness
-                self.list_proba[self.last_index_param] *= 1.05
-                self.list_proba = self.list_proba / np.sum(self.list_proba)
-            else:
-                self.list_proba[self.last_index_param] *= 0.95
-                self.list_proba = self.list_proba / np.sum(self.list_proba)
+    task_index = {rcpsp_problem.tasks_list[i]: i for i in range(rcpsp_problem.n_jobs)}
+    for k in range(len(rcpsp_problem.resources_list)):
+        if rcpsp_problem.is_varying_resource():
+            ressource_available[k, :] = rcpsp_problem.resources[
+                rcpsp_problem.resources_list[k]
+            ][: ressource_available.shape[1]]
         else:
-            self.last_fitness = new_fitness
-        if random.random() <= 0.95:
-            choice = np.random.choice(self.index_np, size=1, p=self.list_proba)[0]
-        else:
-            max_improvement = max(
-                [
-                    self.status[x]["nb_improvement"]
-                    / max(self.status[x]["nb_usage"], 1)
-                    for x in self.status
-                ]
-            )
-            choice = random.choice(
-                [
-                    x
-                    for x in self.status
-                    if self.status[x]["nb_improvement"]
-                    / max(self.status[x]["nb_usage"], 1)
-                    == max_improvement
-                ]
-            )
-        d_params = {
-            key: getattr(self.list_params[int(choice)], key)
-            for key in self.list_params[0].__dict__.keys()
-        }
-        ch = NeighborFlexibleStart(problem=self.problem, **d_params)
-        self.current_iteration += 1
-        self.last_index_param = choice
-        self.status[self.last_index_param]["nb_usage"] += 1
-        return ch.adding_constraint_from_results_store(
-            cp_solver, child_instance, result_storage, last_result_store
+            ressource_available[k, :] = np.full(
+                ressource_available.shape[1],
+                rcpsp_problem.resources[rcpsp_problem.resources_list[k]],
+                dtype=np.int_,
+            )
+        if rcpsp_problem.resources_list[k] in rcpsp_problem.non_renewable_resources:
+            ressource_renewable[k] = False
+
+    for i in range(len(rcpsp_problem.tasks_list)):
+        task = rcpsp_problem.tasks_list[i]
+        for s in rcpsp_problem.successors[task]:
+            index_s = task_index[s]
+            predecessors[index_s, i] = 1
+            successors[i, index_s] = 1
+    minimum_starting_time_array = np.zeros(rcpsp_problem.n_jobs, dtype=np.int_)
+    for t in rcpsp_problem.special_constraints.start_times_window:
+        if rcpsp_problem.special_constraints.start_times_window[t][0] is not None:
+            minimum_starting_time_array[
+                rcpsp_problem.index_task[t]
+            ] = rcpsp_problem.special_constraints.start_times_window[t][0]
+
+    start_at_end_plus_offset = np.zeros(
+        (len(rcpsp_problem.special_constraints.start_at_end_plus_offset), 3),
+        dtype=np.int_,
+    )
+    start_after_nunit = np.zeros(
+        (len(rcpsp_problem.special_constraints.start_after_nunit), 3), dtype=np.int_
+    )
+    j = 0
+    for t1, t2, off in rcpsp_problem.special_constraints.start_at_end_plus_offset:
+        start_at_end_plus_offset[j, 0] = rcpsp_problem.index_task[t1]
+        start_at_end_plus_offset[j, 1] = rcpsp_problem.index_task[t2]
+        start_at_end_plus_offset[j, 2] = off
+        j += 1
+    j = 0
+    for t1, t2, off in rcpsp_problem.special_constraints.start_after_nunit:
+        start_after_nunit[j, 0] = rcpsp_problem.index_task[t1]
+        start_after_nunit[j, 1] = rcpsp_problem.index_task[t2]
+        start_after_nunit[j, 2] = off
+        j += 1
+    if not rcpsp_problem.is_duration_minimum_preemption():
+        func_sgs = partial(
+            sgs_fast_preemptive_some_special_constraints,
+            consumption_array=consumption_array,
+            preemptive_tag=preemptive_tag,
+            start_after_nunit=start_after_nunit,
+            start_at_end_plus_offset=start_at_end_plus_offset,
+            minimum_starting_time_array=minimum_starting_time_array,
+            duration_array=duration_array,
+            predecessors=predecessors,
+            successors=successors,
+            horizon=horizon,
+            ressource_available=ressource_available,
+            ressource_renewable=ressource_renewable,
         )
-
-    def remove_constraints_from_previous_iteration(
-        self, cp_solver: CPSolver, child_instance, previous_constraints: Iterable[Any]
-    ):
-        pass
-
-
-def build_neighbor_operator(option_neighbor: OptionNeighbor, rcpsp_model):
-    params_om = [Params(fraction_to_fix=0.75, minus_delta=100, plus_delta=100)]
-    params_all = [
-        Params(fraction_to_fix=0.9, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.85, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.9, minus_delta=4, plus_delta=4),
-        Params(fraction_to_fix=0.9, minus_delta=4, plus_delta=4),
-        Params(fraction_to_fix=0.92, minus_delta=10, plus_delta=0),
-        Params(fraction_to_fix=0.88, minus_delta=0, plus_delta=10),
-        Params(fraction_to_fix=0.9, minus_delta=10, plus_delta=0),
-        Params(fraction_to_fix=0.8, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=15, plus_delta=15),
-        Params(fraction_to_fix=0.9, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=1.0, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.8, minus_delta=2, plus_delta=2),
-        Params(fraction_to_fix=0.85, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.95, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.95, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.85, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.9, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.9, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.8, minus_delta=2, plus_delta=2),
-        Params(fraction_to_fix=0.98, minus_delta=2, plus_delta=2),
-        Params(fraction_to_fix=0.9, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.98, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.98, minus_delta=8, plus_delta=8),
-        Params(fraction_to_fix=0.98, minus_delta=10, plus_delta=10),
-    ]
-    params_fast = [
-        Params(fraction_to_fix=0.9, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.8, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.8, minus_delta=2, plus_delta=2),
-        Params(fraction_to_fix=0.9, minus_delta=1, plus_delta=1),
-        Params(fraction_to_fix=0.92, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.98, minus_delta=7, plus_delta=7),
-        Params(fraction_to_fix=0.95, minus_delta=5, plus_delta=5),
-    ]
-    params_debug = [Params(fraction_to_fix=1.0, minus_delta=0, plus_delta=0)]
-    params_large = [
-        Params(fraction_to_fix=0.9, minus_delta=12, plus_delta=12),
-        Params(fraction_to_fix=0.8, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.7, minus_delta=12, plus_delta=12),
-        Params(fraction_to_fix=0.7, minus_delta=5, plus_delta=5),
-        Params(fraction_to_fix=0.6, minus_delta=3, plus_delta=3),
-        Params(fraction_to_fix=0.4, minus_delta=2, plus_delta=2),
-        Params(fraction_to_fix=0.9, minus_delta=4, plus_delta=4),
-        Params(fraction_to_fix=0.7, minus_delta=4, plus_delta=4),
-        Params(fraction_to_fix=0.8, minus_delta=5, plus_delta=5),
-    ]
-    params = None
-    if option_neighbor.name == OptionNeighbor.MIX_ALL.name:
-        params = params_all
-    if option_neighbor.name == OptionNeighbor.MIX_FAST.name:
-        params = params_fast
-    if option_neighbor.name == OptionNeighbor.MIX_LARGE_NEIGH.name:
-        params = params_large
-    if option_neighbor.name == OptionNeighbor.DEBUG.name:
-        params = params_debug
-    if option_neighbor.name == OptionNeighbor.LARGE.name:
-        params = params_om
-    probas = [1 / len(params)] * len(params)
-    constraint_handler = ConstraintHandlerMix(
-        problem=rcpsp_model, list_params=params, list_proba=probas
+        func_sgs_2 = partial(
+            sgs_fast_partial_schedule_preemptive,
+            consumption_array=consumption_array,
+            preemptive_tag=preemptive_tag,
+            duration_array=duration_array,
+            predecessors=predecessors,
+            successors=successors,
+            horizon=horizon,
+            ressource_available=ressource_available,
+            ressource_renewable=ressource_renewable,
+        )
+    else:
+        func_sgs = partial(
+            sgs_fast_preemptive_minduration,
+            consumption_array=consumption_array,
+            preemptive_tag=preemptive_tag,
+            duration_array=duration_array,
+            predecessors=predecessors,
+            successors=successors,
+            horizon=horizon,
+            ressource_available=ressource_available,
+            ressource_renewable=ressource_renewable,
+            min_duration_preemptive=min_duration_preemptive,
+            min_duration_preemptive_bool=min_duration_preemptive_bool,
+        )
+        func_sgs_2 = partial(
+            sgs_fast_partial_schedule_preemptive_minduration,
+            consumption_array=consumption_array,
+            preemptive_tag=preemptive_tag,
+            duration_array=duration_array,
+            predecessors=predecessors,
+            successors=successors,
+            horizon=horizon,
+            ressource_available=ressource_available,
+            ressource_renewable=ressource_renewable,
+            min_duration_preemptive=min_duration_preemptive,
+            min_duration_preemptive_bool=min_duration_preemptive_bool,
+        )
+    func_compute_mean_resource = partial(
+        compute_mean_ressource,
+        consumption_array=consumption_array,
+        ressource_available=ressource_available,
+        ressource_renewable=ressource_renewable,
     )
-    return constraint_handler
+    return func_sgs, func_sgs_2, func_compute_mean_resource
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_lns_solver.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/loading_example.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,310 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
-from typing import List, Optional, Union
+import logging
+import os
+import pickle
+import random
+import time
 
-import discrete_optimization.rcpsp.solver.rcpsp_cp_lns_solver as rcpsp_lns
-from discrete_optimization.generic_rcpsp_tools.graph_tools_rcpsp import (
-    build_graph_rcpsp_object,
-)
-from discrete_optimization.generic_rcpsp_tools.neighbor_builder import (
-    OptionNeighborRandom,
-    build_neighbor_mixing_cut_parts,
-    build_neighbor_mixing_methods,
-    build_neighbor_random,
-    mix_both,
-)
-from discrete_optimization.generic_rcpsp_tools.neighbor_tools_rcpsp import (
-    ParamsConstraintBuilder,
-)
-from discrete_optimization.generic_tools.callbacks.callback import Callback
-from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
-from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
-from discrete_optimization.generic_tools.lns_cp import LNS_CP
-from discrete_optimization.generic_tools.result_storage.result_storage import (
-    ResultStorage,
-)
-from discrete_optimization.rcpsp.rcpsp_model_preemptive import PartialSolutionPreemptive
-from discrete_optimization.rcpsp.solver.cp_lns_methods_clean import (
-    RCPSPModel,
-    RCPSPModelPreemptive,
-    RCPSPModelSpecialConstraintsPreemptive,
+import matplotlib.pyplot as plt
+import numpy as np
+import scipy.spatial.distance as dist
+from sklearn.cluster import KMeans
+
+import discrete_optimization.tsp.tsp_parser as tsp_parser
+import discrete_optimization.vrp.vrp_parser as vrp_parser
+from discrete_optimization.pickup_vrp.builders.instance_builders import (
+    create_pickup_and_delivery,
+    create_selective_tsp,
 )
-from discrete_optimization.rcpsp.solver.cp_lns_methods_preemptive import (
-    PostProLeftShift,
+from discrete_optimization.pickup_vrp.gpdp import (
+    GPDP,
+    GPDPSolution,
+    ProxyClass,
+    build_pruned_problem,
 )
-from discrete_optimization.rcpsp.solver.cp_solvers import (
-    CP_MRCPSP_MZN,
-    CP_MRCPSP_MZN_PREEMPTIVE,
-    CP_RCPSP_MZN,
-    CP_RCPSP_MZN_PREEMPTIVE,
+from discrete_optimization.pickup_vrp.plots.gpdp_plot_utils import plot_gpdp_solution
+from discrete_optimization.pickup_vrp.solver.lp_solver import (
+    LinearFlowSolver,
+    ParametersMilp,
 )
-from discrete_optimization.rcpsp.solver.rcpsp_lp_lns_solver import (
-    InitialMethodRCPSP,
-    InitialSolutionRCPSP,
+from discrete_optimization.pickup_vrp.solver.ortools_solver import (
+    FirstSolutionStrategy,
+    LocalSearchMetaheuristic,
+    ORToolsGPDP,
+    ParametersCost,
 )
-from discrete_optimization.rcpsp.solver.rcpsp_solver import SolverRCPSP
 
-GENERIC_CLASS = Union[
-    RCPSPModel,
-    RCPSPModelPreemptive,
-    RCPSPModelSpecialConstraintsPreemptive,
-]
-
-
-def build_default_cp_model(
-    rcpsp_problem: GENERIC_CLASS, partial_solution=None, **kwargs
-):
-    if isinstance(
-        rcpsp_problem, (RCPSPModelPreemptive, RCPSPModelSpecialConstraintsPreemptive)
-    ):
-        if rcpsp_problem.is_rcpsp_multimode():
-            solver = CP_MRCPSP_MZN_PREEMPTIVE(
-                problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED
-            )
-            solver.init_model(
-                output_type=True,
-                model_type="multi-preemptive",
-                nb_preemptive=12,
-                max_preempted=100,
-                partial_solution=partial_solution,
-                **kwargs
-            )
-        else:
-            solver = CP_RCPSP_MZN_PREEMPTIVE(
-                problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED
-            )
-            solver.init_model(
-                output_type=True,
-                model_type="single-preemptive",
-                nb_preemptive=12,
-                max_preempted=100,
-                partial_solution=partial_solution,
-                **kwargs
-            )
-        return solver
-    else:
-        if rcpsp_problem.is_rcpsp_multimode():
-            solver = CP_MRCPSP_MZN(
-                problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED
-            )
-            solver.init_model(
-                output_type=True,
-                model_type="multi",
-                partial_solution=partial_solution,
-                **kwargs
-            )
-        else:
-            solver = CP_RCPSP_MZN(
-                problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED
-            )
-            if "model_type" not in kwargs:
-                kwargs["model_type"] = "single"  # you can use "single-no-search" too.
-            solver.init_model(
-                output_type=True, partial_solution=partial_solution, **kwargs
-            )
-        return solver
+logging.basicConfig(level=logging.DEBUG)
 
 
-class LargeNeighborhoodSearchRCPSP(SolverRCPSP):
-    def __init__(
-        self,
-        problem: GENERIC_CLASS,
-        partial_solution: PartialSolutionPreemptive = None,
-        params_objective_function: Optional[ParamsObjectiveFunction] = None,
-        **kwargs
-    ):
-        super().__init__(
-            problem=problem, params_objective_function=params_objective_function
-        )
-        graph = build_graph_rcpsp_object(problem)
-        solver = build_default_cp_model(
-            rcpsp_problem=problem, partial_solution=partial_solution, **kwargs
-        )
-        constraint_handler = None
-        option = kwargs.get("option_neighbor_operator", 2)
-        if option == 0:
-            constraint_handler = build_neighbor_random(
-                option_neighbor=kwargs.get(
-                    "option_neighbor_random", OptionNeighborRandom.MIX_ALL
-                ),
-                rcpsp_model=problem,
-            )
-        if option == 1:
-            constraint_handler = mix_both(
-                rcpsp_model=problem,
-                option_neighbor_random=kwargs.get(
-                    "option_neighbor_random", OptionNeighborRandom.MIX_ALL
-                ),
-                graph=graph,
-                fraction_subproblem=kwargs.get("fraction_subproblem", 0.05),
-                cut_part=kwargs.get("cut_part", 10),
-                params_list=kwargs.get(
-                    "params_list",
-                    [
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=400,
-                            plus_delta_secondary=400,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=0,
-                            plus_delta_secondary=0,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                    ],
-                ),
-            )
-        if option == 2:
-            constraint_handler = build_neighbor_mixing_methods(
-                rcpsp_model=problem,
-                graph=graph,
-                fraction_subproblem=kwargs.get("fraction_subproblem", 0.05),
-                cut_part=kwargs.get("cut_part", 10),
-                params_list=kwargs.get(
-                    "params_list",
-                    [
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=400,
-                            plus_delta_secondary=400,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=0,
-                            plus_delta_secondary=0,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                    ],
-                ),
-            )
-        if option == 3:
-            constraint_handler = build_neighbor_mixing_cut_parts(
-                rcpsp_model=problem,
-                graph=graph,
-                params_list=kwargs.get(
-                    "params_list",
-                    [
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=400,
-                            plus_delta_secondary=400,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                        ParamsConstraintBuilder(
-                            minus_delta_primary=6000,
-                            plus_delta_primary=6000,
-                            minus_delta_secondary=0,
-                            plus_delta_secondary=0,
-                            constraint_max_time_to_current_solution=False,
-                        ),
-                    ],
-                ),
-            )
-        initial_solution_provider = kwargs.get("initial_solution_provider", None)
-        if initial_solution_provider is None:
-            initial_solution_provider = InitialSolutionRCPSP(
-                problem=problem,
-                initial_method=InitialMethodRCPSP.DUMMY,
-                params_objective_function=self.params_objective_function,
-            )
-        self.initial_solution_provider = initial_solution_provider
-        self.constraint_handler = constraint_handler
-        self.params_objective_function = params_objective_function
-        self.cp_solver = solver
-        if isinstance(
-            problem,
-            (RCPSPModelPreemptive, RCPSPModelSpecialConstraintsPreemptive),
-        ):
-            self.post_process_solution = PostProLeftShift(
-                problem=problem,
-                params_objective_function=self.params_objective_function,
-                do_ls=kwargs.get("do_ls", False),
-            )
-        else:
-            self.post_process_solution = rcpsp_lns.PostProcessLeftShift(
-                rcpsp_problem=problem, partial_solution=None
-            )
-        self.lns_solver = LNS_CP(
-            problem=problem,
-            cp_solver=self.cp_solver,
-            post_process_solution=self.post_process_solution,
-            initial_solution_provider=self.initial_solution_provider,
-            constraint_handler=self.constraint_handler,
-            params_objective_function=self.params_objective_function,
-        )
+def load_vrp_and_transform():
+    file_path = vrp_parser.get_data_available()[1]
+    vrp_model = vrp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model)
+
+
+def load_tsp_and_transform():
+    files_available = tsp_parser.get_data_available()
+    file_path = files_available[1]
+    tsp_model = tsp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model)
 
-    def solve(
-        self,
-        nb_iteration_lns: int,
-        parameters_cp: Optional[ParametersCP] = None,
-        nb_iteration_no_improvement: Optional[int] = None,
-        skip_first_iteration: bool = False,
-        stop_first_iteration_if_optimal: bool = True,
-        callbacks: Optional[List[Callback]] = None,
-        **kwargs
-    ) -> ResultStorage:
-        if parameters_cp is None:
-            parameters_cp = ParametersCP.default()
-        return self.lns_solver.solve_lns(
-            parameters_cp=parameters_cp,
-            skip_first_iteration=skip_first_iteration,
-            stop_first_iteration_if_optimal=stop_first_iteration_if_optimal,
-            nb_iteration_no_improvement=nb_iteration_no_improvement,
-            nb_iteration_lns=nb_iteration_lns,
-            callbacks=callbacks,
-            **kwargs
+
+def debug_lp():
+    vrp = False
+    tsp = True
+    if tsp:
+        files_available = tsp_parser.get_data_available()
+        file_path = files_available[16]
+        tsp_model = tsp_parser.parse_file(file_path)
+        gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
+    else:
+        file_path = vrp_parser.get_data_available()[1]
+        vrp_model = vrp_parser.parse_file(file_path)
+        gpdp = ProxyClass.from_vrp_model_to_gpdp(
+            vrp_model=vrp_model, compute_graph=True
         )
+    simplify = False
+    if simplify:
+        gpdp = build_pruned_problem(gpdp)
+    print(gpdp.graph.get_nodes())
+    print(len(gpdp.graph.get_nodes()))
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    p = ParametersMilp.default()
+    p.time_limit = 2000
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=False, nb_iteration_max=4, include_subtour=False
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+    plt.show()
+
+
+def selective_tsp():
+    gpdp = create_selective_tsp()
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    p = ParametersMilp.default()
+    p.time_limit = 30
+    linear_flow_solver.init_model(
+        one_visit_per_cluster=True, one_visit_per_node=False, include_subtour=False
+    )
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=True, nb_iteration_max=4, include_subtour=False
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+    plt.show()
+
+
+def vrp_capacity():
+    file_path = vrp_parser.get_data_available()[4]
+    print(file_path)
+    vrp_model = vrp_parser.parse_file(file_path)
+    print("Nb vehicle : ", vrp_model.vehicle_count)
+    print("Capacities : ", vrp_model.vehicle_capacities)
+    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model, compute_graph=True)
+    simplify = False
+    if simplify:
+        gpdp = build_pruned_problem(gpdp)
+    print(gpdp.graph.get_nodes())
+    print(len(gpdp.graph.get_nodes()))
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    p = ParametersMilp.default()
+    p.time_limit = 30
+    linear_flow_solver.init_model(
+        include_capacity=True,
+        include_resources=False,
+        one_visit_per_node=True,
+        include_time_evolution=False,
+    )
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=True, nb_iteration_max=4
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+    plt.show()
+
+
+def run_ortools_solver():
+    file_path = vrp_parser.get_data_available()[4]
+    print(file_path)
+    vrp_model = vrp_parser.parse_file(file_path)
+    print("Nb vehicle : ", vrp_model.vehicle_count)
+    print("Capacities : ", vrp_model.vehicle_capacities)
+    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model)
+    solver = ORToolsGPDP(problem=gpdp)
+    solver.init_model(
+        one_visit_per_cluster=False,
+        one_visit_per_node=True,
+        time_limit=10,
+    )
+    result_storage = solver.solve()
+    best_sol = result_storage.best_solution
+    plot_gpdp_solution(best_sol, gpdp)
+    plt.show()
+
+
+def run_ortools_solver_selective():
+    gpdp = create_selective_tsp(nb_nodes=600, nb_vehicles=5, nb_clusters=100)
+    solver = ORToolsGPDP(
+        problem=gpdp, factor_multiplier_distance=1, factor_multiplier_time=1
+    )
+    solver.init_model(
+        one_visit_per_cluster=True,
+        one_visit_per_node=False,
+        include_time_dimension=True,
+        include_demand=True,
+        include_mandatory=True,
+        include_pickup_and_delivery=False,
+        include_equilibrate_charge=True,
+        charge_constraint={
+            v: (len(gpdp.clusters_to_node) // (2 * gpdp.number_vehicle), None)
+            for v in range(gpdp.number_vehicle)
+        },
+        parameters_cost=[ParametersCost(dimension_name="Distance")],
+        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
+        first_solution_strategy=FirstSolutionStrategy.SAVINGS,
+        time_limit=200,
+    )
+    result_storage = solver.solve()
+    best_sol = result_storage.best_solution
+    plot_gpdp_solution(best_sol, gpdp)
+    plt.show()
+
+
+def run_ortools_pickup_delivery():
+    def check_solution(res, gpdp: GPDP):
+        for p, d in gpdp.list_pickup_deliverable:
+            index_vehicles_p = set(
+                [[i for i in range(len(res)) if pp in res[i]][0] for pp in p]
+            )
+            index_vehicles_d = set(
+                [[i for i in range(len(res)) if dd in res[i]][0] for dd in d]
+            )
+            assert len(index_vehicles_p) == 1
+            assert len(index_vehicles_d) == 1
+            vehicle_p = list(index_vehicles_p)[0]
+            vehicle_d = list(index_vehicles_d)[0]
+            assert vehicle_p == vehicle_d
+            index_p = [res[vehicle_p].index(pp) for pp in p]
+            index_d = [res[vehicle_d].index(dd) for dd in d]
+            assert max(index_p) < min(index_d)
+
+    model = create_pickup_and_delivery(
+        number_of_vehicles=4,
+        number_of_node=100,
+        include_pickup=True,
+        fraction_of_pickup_deliver=0.125,
+        include_cluster=False,
+        pickup_per_cluster=False,
+    )
+    list_params_cost = [
+        ParametersCost(
+            dimension_name="Distance",
+            global_span=True,
+            sum_over_vehicles=False,
+            coefficient_vehicles=10,
+        ),
+        ParametersCost(
+            dimension_name="Distance",
+            global_span=False,
+            sum_over_vehicles=True,
+            coefficient_vehicles=[1] * model.number_vehicle,
+        ),
+    ]
+    solver = ORToolsGPDP(problem=model)
+    solver.init_model(
+        one_visit_per_cluster=False,
+        one_visit_per_node=True,
+        include_pickup_and_delivery=True,
+        use_lns=True,
+        parameters_cost=list_params_cost,
+        include_equilibrate_charge=True,
+        charge_constraint={
+            v: (len(model.all_nodes) // (4 * model.number_vehicle), None)
+            for v in range(model.number_vehicle)
+        },
+        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
+        first_solution_strategy=FirstSolutionStrategy.SAVINGS,
+        time_limit=100,
+    )
+    logging.basicConfig(level=logging.DEBUG)
+    result_storage = solver.solve()
+    best_sol = result_storage.best_solution
+    assert best_sol.check_pickup_deliverable()
+    plot_gpdp_solution(best_sol, model)
+    plt.show()
+
+
+def run_ortools_pickup_delivery_cluster():
+    gpdp = create_pickup_and_delivery(
+        number_of_node=200,
+        include_cluster=True,
+        include_pickup=False,
+        pickup_per_cluster=True,
+    )
+    solver = ORToolsGPDP(problem=gpdp)
+    solver.init_model(
+        one_visit_per_cluster=True,
+        one_visit_per_node=False,
+        include_pickup_and_delivery=False,
+        include_mandatory=False,
+        include_pickup_and_delivery_per_cluster=True,
+        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
+        first_solution_strategy=FirstSolutionStrategy.PARALLEL_CHEAPEST_INSERTION,
+        time_limit=30,
+    )
+    result_storage = solver.solve()
+    best_sol = result_storage.best_solution
+    assert best_sol.check_pickup_deliverable()
+    plot_gpdp_solution(best_sol, gpdp)
+    plt.show()
+
+
+def create_examples_script(folder_to_save):
+    if not os.path.exists(folder_to_save):
+        os.makedirs(folder_to_save)
+    sizes = [10, 50, 150, 300, 1000]
+    sizes = [1000]
+    include_cluster = [True, False]
+    include_pickup = [True, False]
+    pickup_per_cluster = [True, False]
+    for s in sizes:
+        for cl in include_cluster:
+            for picdel in include_pickup:
+                for pickupcluster in pickup_per_cluster:
+                    if pickupcluster and not include_cluster:
+                        continue
+                    if picdel and not cl and pickup_per_cluster:
+                        continue
+                    for n in range(1):
+                        gpdp = create_pickup_and_delivery(
+                            number_of_node=s,
+                            include_cluster=cl,
+                            include_pickup=picdel,
+                            pickup_per_cluster=pickupcluster,
+                        )
+                        t = time.time_ns()
+                        pickle.dump(
+                            gpdp,
+                            file=open(
+                                os.path.join(
+                                    folder_to_save,
+                                    f"gpdp_size{s}_cluster{cl}_pickup{picdel}_pickuppercluster{pickupcluster}_time{t}.pk",
+                                ),
+                                "wb",
+                            ),
+                        )
+
+
+if __name__ == "__main__":
+    # debug_lp()
+    # selective_tsp()
+    # vrp_capacity()
+    run_ortools_solver()
+    # run_ortools_pickup_delivery()
+    # run_ortools_solver_selective()
+    # run_ortools_pickup_delivery_cluster()
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_model_input.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_model_input.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_solvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,17 @@
     SignEnum,
     find_right_minizinc_solver_name,
 )
 from discrete_optimization.generic_tools.do_problem import (
     ParamsObjectiveFunction,
     build_aggreg_function_and_params_objective,
 )
-from discrete_optimization.generic_tools.result_storage.result_storage import (
-    ResultStorage,
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    EnumHyperparameter,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import (
     RCPSPModelPreemptive,
     RCPSPSolutionPreemptive,
 )
 from discrete_optimization.rcpsp.rcpsp_solution import PartialSolution, RCPSPSolution
@@ -119,15 +120,15 @@
             "fakereq": [[] for r in rcpsp_model.resources_list],
             "include_fake_tasks": False,
         }
         return dict_to_add_in_instance
 
 
 class CP_RCPSP_MZN(MinizincCPSolver, SolverRCPSP):
-
+    hyperparameters = MinizincCPSolver.hyperparameters
     problem: RCPSPModel
 
     def __init__(
         self,
         problem: RCPSPModel,
         cp_solver_name: CPSolverName = CPSolverName.CHUFFED,
         params_objective_function: ParamsObjectiveFunction = None,
@@ -349,15 +350,15 @@
         )
 
     def get_stats(self):
         return self.stats
 
 
 class CP_MRCPSP_MZN(MinizincCPSolver, SolverRCPSP):
-
+    hyperparameters = MinizincCPSolver.hyperparameters
     problem: RCPSPModel
 
     def __init__(
         self,
         problem: RCPSPModel,
         cp_solver_name: CPSolverName = CPSolverName.CHUFFED,
         params_objective_function: ParamsObjectiveFunction = None,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cp_solvers_multiscenario.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cp_solvers_multiscenario.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 from discrete_optimization.generic_tools.cp_tools import (
     CPSolverName,
     MinizincCPSolver,
     find_right_minizinc_solver_name,
 )
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    IntegerHyperparameter,
+)
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_model_preemptive import RCPSPModelPreemptive
 from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
 from discrete_optimization.rcpsp.rcpsp_utils import create_fake_tasks
 from discrete_optimization.rcpsp.robust_rcpsp import AggregRCPSPModel
 
 logger = logging.getLogger(__name__)
@@ -67,14 +71,20 @@
             "fakereq": [[] for r in rcpsp_model.resources_list],
             "include_fake_tasks": False,
         }
         return dict_to_add_in_instance
 
 
 class CP_MULTISCENARIO(MinizincCPSolver):
+    hyperparameters = MinizincCPSolver.hyperparameters + [
+        CategoricalHyperparameter(
+            name="relax_ordering", default=False, choices=[True, False]
+        ),
+        IntegerHyperparameter(name="nb_incoherence_limit", low=0, high=10, default=3),
+    ]
     problem: AggregRCPSPModel
 
     def __init__(
         self,
         problem: AggregRCPSPModel,
         cp_solver_name: CPSolverName = CPSolverName.CHUFFED,
         params_objective_function: ParamsObjectiveFunction = None,
@@ -91,14 +101,15 @@
         ]  # For now, I've put the var name of the CP model (not the rcpsp_model)
 
     @property
     def base_problem(self):
         return self.problem
 
     def init_model(self, **args):
+        args = self.complete_with_default_hyperparameters(args)
         model_type = args.get("model_type", "multiscenario")
         max_time = args.get("max_time", self.problem.horizon)
         fake_tasks = args.get(
             "fake_tasks", True
         )  # to modelize varying quantity of resource.
         add_objective_makespan = args.get("add_objective_makespan", True)
         ignore_sec_objective = args.get("ignore_sec_objective", True)
@@ -158,16 +169,16 @@
                     self.problem.return_index_task(x, offset=1)
                     for x in self.problem.successors[task]
                 ]
             )
             for task in sorted_tasks
         ]
         instance["suc"] = suc
-        instance["relax_ordering"] = args.get("relax_ordering", False)
-        instance["nb_incoherence_limit"] = args.get("nb_incoherence_limit", 3)
+        instance["relax_ordering"] = args["relax_ordering"]
+        instance["nb_incoherence_limit"] = args["nb_incoherence_limit"]
         self.instance = instance
         self.index_in_minizinc = {
             task: self.problem.return_index_task(task, offset=1)
             for task in self.problem.tasks_list
         }
         self.instance["sink_task"] = self.index_in_minizinc[self.problem.sink_task]
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cpm.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cpm.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/cpsat_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/cpsat_solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     CpSolverSolutionCallback,
     IntervalVar,
     IntVar,
 )
 
 from discrete_optimization.generic_tools.cp_tools import StatusSolver
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+)
 from discrete_optimization.generic_tools.ortools_cpsat_tools import OrtoolsCPSatSolver
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel, RCPSPSolution
 from discrete_optimization.rcpsp.rcpsp_utils import (
     create_fake_tasks,
     get_end_bounds_from_additional_constraint,
     get_start_bounds_from_additional_constraint,
 )
@@ -150,15 +153,15 @@
                 )
                 for task in self.problem.tasks_list
                 for mode in self.problem.mode_details[task]
                 if self.problem.mode_details[task][mode].get(resource, 0) > 0
             ]
             fake_task_res = [
                 (
-                    model.NewFixedSizeIntervalVar(
+                    model.NewFixedSizedIntervalVar(
                         start=f["start"], size=f["duration"], name=f"res_"
                     ),
                     f.get(resource, 0),
                 )
                 for f in fake_task
                 if f.get(resource, 0) > 0
             ]
@@ -350,15 +353,15 @@
                 if self.problem.mode_details[task][mode].get(resource, 0) > 0
             ]
             if len(task_modes_consuming) == 0:
                 # when empty, the constraints don't work !
                 return
             fake_task_res = [
                 (
-                    model.NewFixedSizeIntervalVar(
+                    model.NewFixedSizedIntervalVar(
                         start=f["start"], size=f["duration"], name=f"res_"
                     ),
                     int(f.get(resource, 0)),
                 )
                 for f in fake_task
                 if f.get(resource, 0) > 0
             ]
@@ -439,14 +442,22 @@
 
 class CPSatRCPSPSolverCumulativeResource(CPSatRCPSPSolver):
     """
     Specific solver to minimize the minimum resource amount needed to accomplish the scheduling problem.
     In this version we sum up the resource for each given time to do the resource optimisation.
     """
 
+    hyperparameters = [
+        CategoricalHyperparameter(
+            name="use_overlap_for_disjunctive_resource",
+            default=True,
+            choices=[True, False],
+        )
+    ]
+
     def create_resource_capacity_var(self, model: CpModel):
         resource_capacity_var = {}
         for resource in self.problem.resources_list:
             resource_capacity_var[resource] = model.NewIntVar(
                 lb=0,
                 ub=self.problem.get_max_resource_capacity(resource),
                 name=f"res_{resource}",
@@ -488,15 +499,15 @@
                 if self.problem.mode_details[task][mode].get(resource, 0) > 0
             ]
             if len(task_modes_consuming) == 0:
                 # when empty, the constraints don't work !
                 return
             fake_task_res = [
                 (
-                    model.NewFixedSizeIntervalVar(
+                    model.NewFixedSizedIntervalVar(
                         start=f["start"], size=f["duration"], name=f"res_"
                     ),
                     f.get(resource, 0),
                 )
                 for f in fake_task
                 if f.get(resource, 0) > 0
             ]
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_ga_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_ga_solver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
+from typing import Optional
 
 from discrete_optimization.generic_tools.ea.alternating_ga import AlternatingGa
 from discrete_optimization.generic_tools.ea.ga import Ga
 from discrete_optimization.generic_tools.ea.ga_tools import (
     ParametersAltGa,
     ParametersGa,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.solver.rcpsp_solver import SolverRCPSP
 
 
 class GA_RCPSP_Solver(SolverRCPSP):
     problem: RCPSPModel
+    hyperparameters = Ga.hyperparameters
 
-    def solve(self, parameters_ga: ParametersGa = ParametersGa.default_rcpsp(), **args):
+    def solve(self, parameters_ga: Optional[ParametersGa] = None, **args):
+        if parameters_ga is None:
+            parameters_ga = ParametersGa.default_rcpsp()
+            args = self.complete_with_default_hyperparameters(args)
+        for key in args:
+            setattr(parameters_ga, key, args[key])
         ga_solver = Ga(
             problem=self.problem,
             encoding=parameters_ga.encoding,
             objective_handling=parameters_ga.objective_handling,
             objectives=parameters_ga.objectives,
             objective_weights=parameters_ga.objective_weights,
             mutation=parameters_ga.mutation,
@@ -33,18 +40,24 @@
             deap_verbose=parameters_ga.deap_verbose,
         )
         return ga_solver.solve()
 
 
 class GA_MRCPSP_Solver(SolverRCPSP):
     problem: RCPSPModel
+    hyperparameters = Ga.hyperparameters
 
     def solve(
         self, parameters_ga: ParametersAltGa = ParametersAltGa.default_mrcpsp(), **args
     ):
+        if parameters_ga is None:
+            parameters_ga = ParametersAltGa.default_mrcpsp()
+            args = self.complete_with_default_hyperparameters(args)
+        for key in args:
+            setattr(parameters_ga, key, args[key])
         ga_solver = AlternatingGa(
             problem=self.problem,
             encodings=parameters_ga.encodings,
             objective_handling=parameters_ga.objective_handling,
             objectives=parameters_ga.objectives,
             objective_weights=parameters_ga.objective_weights,
             mutations=parameters_ga.mutations,
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_lns_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_lns_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import logging
 from itertools import product
 from typing import Any, Callable, Dict, Hashable, List, Optional, Tuple, Union
 
 from mip import BINARY, INTEGER, MINIMIZE, Model, Var, xsum
 
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    CategoricalHyperparameter,
+    EnumHyperparameter,
+)
 from discrete_optimization.generic_tools.lp_tools import (
     CplexMilpSolver,
     GurobiMilpSolver,
     MilpSolver,
     MilpSolverName,
     ParametersMilp,
     PymipMilpSolver,
@@ -49,14 +53,22 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class LP_RCPSP(PymipMilpSolver, SolverRCPSP):
     problem: RCPSPModel
+    hyperparameters = [
+        EnumHyperparameter(
+            name="lp_solver", enum=MilpSolverName, default=MilpSolverName.CBC
+        ),
+        CategoricalHyperparameter(
+            name="greedy_start", choices=[True, False], default=True
+        ),
+    ]
 
     def __init__(
         self,
         problem: RCPSPModel,
         lp_solver: MilpSolverName = MilpSolverName.CBC,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs,
@@ -279,14 +291,19 @@
             rcpsp_schedule_feasible=True,
         )
 
 
 class _BaseLP_MRCPSP(MilpSolver, SolverRCPSP):
     problem: RCPSPModel
     x: Dict[Tuple[Hashable, int, int], Any]
+    hyperparameters = [
+        CategoricalHyperparameter(
+            name="greedy_start", choices=[True, False], default=True
+        )
+    ]
 
     def __init__(
         self,
         problem: RCPSPModel,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs,
     ):
@@ -318,14 +335,16 @@
             rcpsp_schedule=rcpsp_schedule,
             rcpsp_modes=modes_vec,
             rcpsp_schedule_feasible=True,
         )
 
 
 class LP_MRCPSP(PymipMilpSolver, _BaseLP_MRCPSP):
+    hyperparameters = LP_RCPSP.hyperparameters
+
     def __init__(
         self,
         problem: RCPSPModel,
         lp_solver: MilpSolverName = MilpSolverName.CBC,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs,
     ):
@@ -334,15 +353,16 @@
             params_objective_function=params_objective_function,
             **kwargs,
         )
         self.lp_solver = lp_solver
         self.solver_name = map_solver[lp_solver]
 
     def init_model(self, **args):
-        greedy_start = args.get("greedy_start", True)
+        args = self.complete_with_default_hyperparameters(args)
+        greedy_start = args["greedy_start"]
         start_solution = args.get("start_solution", None)
         if start_solution is None:
             if greedy_start:
                 logger.info("Computing greedy solution")
                 greedy_solver = PileSolverRCPSP(self.problem)
                 store_solution = greedy_solver.solve(
                     greedy_choice=GreedyChoice.MOST_SUCCESSORS
@@ -546,16 +566,19 @@
     ) -> ResultStorage:
         if self.model is None:
             self.init_model(greedy_start=False, **kwargs)
         return super().solve(parameters_milp=parameters_milp, **kwargs)
 
 
 class LP_MRCPSP_GUROBI(GurobiMilpSolver, _BaseLP_MRCPSP):
+    hyperparameters = _BaseLP_MRCPSP.hyperparameters
+
     def init_model(self, **args):
-        greedy_start = args.get("greedy_start", True)
+        args = self.complete_with_default_hyperparameters(args)
+        greedy_start = args["greedy_start"]
         start_solution = args.get("start_solution", None)
         max_horizon = args.get("max_horizon", None)
         if start_solution is None:
             if greedy_start:
                 logger.info("Computing greedy solution")
                 if self.problem.is_varying_resource():
                     greedy_solver = PileSolverRCPSP_Calendar(self.problem)
@@ -808,23 +831,18 @@
                     ]
             self.constraints_partial_solutions = constraints
             logger.debug(
                 f"Partial solution constraints : {self.constraints_partial_solutions}"
             )
             self.model.update()
 
-    def solve(
-        self, parameters_milp: Optional[ParametersMilp] = None, **kwargs
-    ) -> ResultStorage:
-        if self.model is None:
-            self.init_model(greedy_start=False, **kwargs)
-        return super().solve(parameters_milp=parameters_milp, **kwargs)
-
 
 class LP_RCPSP_CPLEX(CplexMilpSolver, _BaseLP_MRCPSP):
+    hyperparameters = _BaseLP_MRCPSP.hyperparameters
+
     def init_model(self, **args):
         greedy_start = args.get("greedy_start", True)
         start_solution = args.get("start_solution", None)
         max_horizon = args.get("max_horizon", None)
         if start_solution is None:
             if greedy_start:
                 logger.info("Computing greedy solution")
@@ -1001,14 +1019,7 @@
                     task, mode, time = k
                     if start_time_j == time and mode == modes_dict[j]:
                         warmstart.add_var_value(self.x[k], 1)
                         warmstart.add_var_value(self.starts[task], time)
                     else:
                         warmstart.add_var_value(self.x[k], 0)
             self.model.add_mip_start(warmstart)
-
-    def solve(
-        self, parameters_milp: Optional[ParametersMilp] = None, **kwargs
-    ) -> ResultStorage:
-        if self.model is None:
-            self.init_model(greedy_start=False, **kwargs)
-        return super().solve(parameters_milp=parameters_milp, **kwargs)
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_lp_solver_gantt.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_lp_solver_gantt.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,17 @@
         s = max(i1[0], i2[0])
         e = min(i1[1], i2[1])
         return [s, e]
 
 
 class ConstraintTaskIndividual:
     list_tuple: List[Tuple[str, int, int, bool]]
-    # task, ressource, ressource_individual, has or has not to do a task
-    # indicates constraint for a given resource individual that has to do a tas
+    # task, resource, resource_individual, has or has not to do a task
+    # indicates constraint for a given resource individual that has to do a task
+
     def __init__(self, list_tuple):
         self.list_tuple = list_tuple
 
 
 class ConstraintWorkDuration:
     ressource: str
     individual: int
@@ -242,16 +243,16 @@
                                     for key in keys_variable
                                 ]
                             )
                             <= 1
                         )
 
 
-# gurobi solver which is ussefull to get a pool of solution (indeed, using the other one we dont have usually a lot of
-# ssolution since we converge rapidly to the "optimum" (we don't have an objective value..)
+# gurobi solver which is usefull to get a pool of solution (indeed, using the other one we dont have usually a lot of
+# solution since we converge rapidly to the "optimum" (we don't have an objective value..)
 class LP_MRCPSP_GANTT_GUROBI(GurobiMilpSolver, _Base_LP_MRCPSP_GANTT):
     def init_model(self, **args):
         self.model = gurobi.Model("Gantt")
         self.ressource_id_usage = {
             k: {i: {} for i in range(len(self.problem.calendar_details[k]))}
             for k in self.problem.calendar_details.keys()
         }
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/solver/rcpsp_pile.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/solver/rcpsp_pile.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 from typing import Dict, List, Optional
 
 import networkx as nx
 import numpy as np
 
 from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
 from discrete_optimization.generic_tools.do_problem import ParamsObjectiveFunction
+from discrete_optimization.generic_tools.hyperparameters.hyperparameter import (
+    EnumHyperparameter,
+)
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_solution import PartialSolution, RCPSPSolution
 from discrete_optimization.rcpsp.solver.cp_solvers import CP_MRCPSP_MZN_MODES
 from discrete_optimization.rcpsp.solver.rcpsp_solver import SolverRCPSP
@@ -32,14 +35,22 @@
 
 
 pop = heappop
 push = heappush
 
 
 class PileSolverRCPSP(SolverRCPSP):
+    hyperparameters = [
+        EnumHyperparameter(
+            name="greedy_choice",
+            enum=GreedyChoice,
+            default=GreedyChoice.MOST_SUCCESSORS,
+        )
+    ]
+
     def __init__(
         self,
         problem: RCPSPModel,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs,
     ):
         super().__init__(
@@ -81,15 +92,16 @@
             self.modes_dict = {}
             for i in range(len(one_mode_setting)):
                 self.modes_dict[i + 1] = one_mode_setting[i]
         else:
             self.modes_dict = {t: 1 for t in self.mode_details}
 
     def solve(self, **kwargs) -> ResultStorage:
-        greedy_choice = kwargs.get("greedy_choice", GreedyChoice.MOST_SUCCESSORS)
+        kwargs = self.complete_with_default_hyperparameters(kwargs)
+        greedy_choice: GreedyChoice = kwargs["greedy_choice"]
         current_succ = {
             k: {
                 "succs": set(self.successors_map[k]["succs"]),
                 "nb": self.successors_map[k]["nb"],
             }
             for k in self.successors_map
         }
@@ -232,14 +244,15 @@
             best_solution=sol,
             mode_optim=self.params_objective_function.sense_function,
         )
         return result_storage
 
 
 class PileSolverRCPSP_Calendar(SolverRCPSP):
+    hyperparameters = PileSolverRCPSP.hyperparameters
     problem: RCPSPModel
 
     def __init__(
         self,
         problem: RCPSPModel,
         params_objective_function: Optional[ParamsObjectiveFunction] = None,
         **kwargs,
@@ -285,15 +298,16 @@
             for i in range(len(one_mode_setting)):
                 self.modes_dict[self.problem.tasks_list[i]] = one_mode_setting[i]
         else:
             self.modes_dict = {t: 1 for t in self.mode_details}
         self.with_calendar = problem.is_varying_resource()
 
     def solve(self, **kwargs) -> ResultStorage:
-        greedy_choice = kwargs.get("greedy_choice", GreedyChoice.MOST_SUCCESSORS)
+        kwargs = self.complete_with_default_hyperparameters(kwargs)
+        greedy_choice = kwargs["greedy_choice"]
         current_succ = {
             k: {
                 "succs": set(self.successors_map[k]["succs"]),
                 "nb": self.successors_map[k]["nb"],
             }
             for k in self.successors_map
         }
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/special_constraints.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/special_constraints.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp/transform_model.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp/transform_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/fast_function_ms_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/fast_function_ms_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative_reif.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/fzn_my_cumulative_reif.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_compute_workers_for_tasks.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_compute_workers_for_tasks.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource_nomultitasking.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_multi_mode_mzn_calendar_no_ressource_nomultitasking.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive_partially_preemptive.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ms_rcpsp_preemptive_partially_preemptive.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/mspsp.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/mspsp.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/mspsp_compatible_all_solvers.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/mspsp_compatible_all_solvers.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/my_cumulative.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/my_cumulative.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/minizinc/ressource_allocation_mspsp.mzn` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/minizinc/ressource_allocation_mspsp.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/multiskill_to_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/multiskill_to_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/plots/plot_solution.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/plots/plot_solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.collections import PatchCollection
 from matplotlib.font_manager import FontProperties
 from matplotlib.patches import Polygon as pp
 from shapely.geometry import Polygon
 
+from discrete_optimization.generic_tools.plot_utils import get_cmap_with_nb_colors
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill import (
     MS_RCPSPModel,
     MS_RCPSPSolution,
     MS_RCPSPSolution_Preemptive,
 )
 
 
@@ -159,15 +160,15 @@
     if fig is None or ax is None:
         fig, ax = plt.subplots(1, figsize=(12, 6))
         fig.suptitle(title_figure)
     position_label = {}
     for i in range(len(sorted_employees)):
         patches = []
         nb_colors = len(sorted_task_by_start) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for boxe in array_ressource_usage[sorted_employees[i]]["boxes_time"]:
             polygon = Polygon([(b[1], b[0]) for b in boxe])
             activity = boxe[0][2]
             x, y = polygon.exterior.xy
             ax.plot(x, y, zorder=-1, color="b")
             patches.append(
                 pp(
@@ -249,15 +250,15 @@
     if fig is None or ax is None:
         fig, ax = plt.subplots(1, figsize=(12, 6))
         fig.suptitle(title_figure)
     position_label = {}
     for i in range(len(sorted_employees)):
         patches = []
         nb_colors = len(sorted_task_by_start) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for boxe in array_ressource_usage[sorted_employees[i]]["boxes_time"]:
             polygon = Polygon([(b[1], b[0]) for b in boxe])
             activity = boxe[0][2]
             if activity not in subtasks:
                 continue
             x, y = polygon.exterior.xy
             ax.plot(x, y, zorder=-1, color="b")
@@ -332,15 +333,15 @@
         key=lambda x: 100000 * rcpsp_sol.get_end_time(x) + rcpsp_model.index_task[x],
     )
     max_time = rcpsp_sol.get_end_time(sorted_task_by_end[-1])
     min_time = rcpsp_sol.get_start_time(sorted_task_by_start[0])
     patches = []
     for j in range(nb_task):
         nb_colors = len(tasks) // 2
-        colors = plt.cm.get_cmap("hsv", nb_colors)
+        colors = get_cmap_with_nb_colors("hsv", nb_colors)
         for start, end in zip(
             rcpsp_sol.get_start_times_list(tasks[j]),
             rcpsp_sol.get_end_times_list(tasks[j]),
         ):
             box = [
                 (j - 0.25, start),
                 (j - 0.25, end),
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mslib_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mslib_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mspsp_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_mspsp_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/rcpsp_multiskill_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/cp_solver_mspsp_instlib.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/cp_solver_mspsp_instlib.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/cp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/cp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/lns_post_process_rcpsp.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/lns_post_process_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/lp_model.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/lp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_ga_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_ga_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_lp_lns_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_lp_lns_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/multimode_transposition.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/multimode_transposition.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/rcpsp_multiskill/solvers/solver_rcpsp_based.py` & `discrete_optimization-0.3.1/discrete_optimization/rcpsp_multiskill/solvers/solver_rcpsp_based.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/common_tools_tsp.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/common_tools_tsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/minizinc/tsp_float.mzn` & `discrete_optimization-0.3.1/discrete_optimization/tsp/minizinc/tsp_float.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/minizinc/tsp_int.mzn` & `discrete_optimization-0.3.1/discrete_optimization/tsp/minizinc/tsp_int.mzn`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/mutation/mutation_tsp.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/mutation/mutation_tsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/plots/plot_tsp.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/plots/plot_tsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/solver/solver_lp_iterative.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/solver/solver_lp_iterative.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/solver/solver_ortools.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/solver/solver_ortools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/solver/tsp_cp_solver.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/solver/tsp_cp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_model.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/tsp/tsp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/tsp/tsp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/mutation/mutation_vrp.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/mutation/mutation_vrp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/solver/greedy_vrp.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/solver/greedy_vrp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/solver/lp_vrp_iterative.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/solver/lp_vrp_iterative.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/solver/lp_vrp_iterative_pymip.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/solver/lp_vrp_iterative_pymip.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/solver/solver_ortools.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/solver/solver_ortools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_model.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_parser.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_solvers.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization/vrp/vrp_toolbox.py` & `discrete_optimization-0.3.1/discrete_optimization/vrp/vrp_toolbox.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/discrete_optimization.egg-info/PKG-INFO` & `discrete_optimization-0.3.1/discrete_optimization.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discrete-optimization
-Version: 0.3.0
+Version: 0.3.1
 Summary: Discrete optimization library
 Author-email: Airbus AI Research <scikit-decide@airbus.com>
 License: MIT
 Project-URL: documentation, https://airbus.github.io/discrete-optimization
 Project-URL: repository, https://github.com/airbus/discrete-optimization
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,17 @@
 Requires-Dist: typing-extensions>=4.0
 Requires-Dist: cpmpy>=0.9.9
 Requires-Dist: scipy
 Requires-Dist: numpy>=1.21
 Requires-Dist: typing_extensions>=4.4
 Requires-Dist: clingo>=5.6
 Requires-Dist: setuptools
+Requires-Dist: qiskit>=1.0.2
+Requires-Dist: qiskit-algorithms>=0.3.0
+Requires-Dist: qiskit-optimization>=0.6.1
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: scikit-learn>=1.0; extra == "test"
 Requires-Dist: optuna; extra == "test"
 
 # Discrete Optimization
```

### Comparing `discrete_optimization-0.3.0/discrete_optimization.egg-info/SOURCES.txt` & `discrete_optimization-0.3.1/discrete_optimization.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -74,14 +74,16 @@
 discrete_optimization/generic_tools/ghh_tools.py
 discrete_optimization/generic_tools/graph_api.py
 discrete_optimization/generic_tools/lns_cp.py
 discrete_optimization/generic_tools/lns_mip.py
 discrete_optimization/generic_tools/lp_tools.py
 discrete_optimization/generic_tools/ortools_cpsat_tools.py
 discrete_optimization/generic_tools/path_tools.py
+discrete_optimization/generic_tools/plot_utils.py
+discrete_optimization/generic_tools/qiskit_tools.py
 discrete_optimization/generic_tools/callbacks/__init__.py
 discrete_optimization/generic_tools/callbacks/backup.py
 discrete_optimization/generic_tools/callbacks/callback.py
 discrete_optimization/generic_tools/callbacks/early_stoppers.py
 discrete_optimization/generic_tools/callbacks/loggers.py
 discrete_optimization/generic_tools/callbacks/optuna.py
 discrete_optimization/generic_tools/ea/__init__.py
@@ -134,14 +136,23 @@
 discrete_optimization/knapsack/solvers/knapsack_cpmpy.py
 discrete_optimization/knapsack/solvers/knapsack_cpsat_solver.py
 discrete_optimization/knapsack/solvers/knapsack_decomposition.py
 discrete_optimization/knapsack/solvers/knapsack_lns_cp_solver.py
 discrete_optimization/knapsack/solvers/knapsack_lns_solver.py
 discrete_optimization/knapsack/solvers/knapsack_solver.py
 discrete_optimization/knapsack/solvers/lp_solvers.py
+discrete_optimization/maximum_independent_set/mis_model.py
+discrete_optimization/maximum_independent_set/mis_parser.py
+discrete_optimization/maximum_independent_set/mis_plot.py
+discrete_optimization/maximum_independent_set/mis_solvers.py
+discrete_optimization/maximum_independent_set/solvers/mis_gurobi.py
+discrete_optimization/maximum_independent_set/solvers/mis_kamis.py
+discrete_optimization/maximum_independent_set/solvers/mis_ortools.py
+discrete_optimization/maximum_independent_set/solvers/mis_quantum.py
+discrete_optimization/maximum_independent_set/solvers/mis_solver.py
 discrete_optimization/pickup_vrp/__init__.py
 discrete_optimization/pickup_vrp/gpdp.py
 discrete_optimization/pickup_vrp/builders/__init__.py
 discrete_optimization/pickup_vrp/builders/instance_builders.py
 discrete_optimization/pickup_vrp/minizinc/gpdp.mzn
 discrete_optimization/pickup_vrp/minizinc/gpdp_example.dzn
 discrete_optimization/pickup_vrp/minizinc/gpdp_flow.mzn
@@ -186,17 +197,15 @@
 discrete_optimization/rcpsp/minizinc/rcpsp_single_mode_resource.mzn
 discrete_optimization/rcpsp/minizinc/resumee_rcpsp.mzn
 discrete_optimization/rcpsp/mutations/__init__.py
 discrete_optimization/rcpsp/mutations/mutation_rcpsp.py
 discrete_optimization/rcpsp/plots/__init__.py
 discrete_optimization/rcpsp/plots/rcpsp_utils_preemptive.py
 discrete_optimization/rcpsp/solver/__init__.py
-discrete_optimization/rcpsp/solver/cp_lns_methods_clean.py
 discrete_optimization/rcpsp/solver/cp_lns_methods_preemptive.py
-discrete_optimization/rcpsp/solver/cp_lns_solver.py
 discrete_optimization/rcpsp/solver/cp_model_input.py
 discrete_optimization/rcpsp/solver/cp_solvers.py
 discrete_optimization/rcpsp/solver/cp_solvers_multiscenario.py
 discrete_optimization/rcpsp/solver/cpm.py
 discrete_optimization/rcpsp/solver/cpsat_solver.py
 discrete_optimization/rcpsp/solver/rcpsp_cp_lns_solver.py
 discrete_optimization/rcpsp/solver/rcpsp_ga_solver.py
@@ -226,21 +235,18 @@
 discrete_optimization/rcpsp_multiskill/minizinc/mspsp.mzn
 discrete_optimization/rcpsp_multiskill/minizinc/mspsp_compatible_all_solvers.mzn
 discrete_optimization/rcpsp_multiskill/minizinc/my_cumulative.mzn
 discrete_optimization/rcpsp_multiskill/minizinc/ressource_allocation_mspsp.mzn
 discrete_optimization/rcpsp_multiskill/plots/__init__.py
 discrete_optimization/rcpsp_multiskill/plots/plot_solution.py
 discrete_optimization/rcpsp_multiskill/solvers/__init__.py
-discrete_optimization/rcpsp_multiskill/solvers/calendar_solver_iterative.py
-discrete_optimization/rcpsp_multiskill/solvers/cp_lns_solver.py
 discrete_optimization/rcpsp_multiskill/solvers/cp_solver_mspsp_instlib.py
 discrete_optimization/rcpsp_multiskill/solvers/cp_solvers.py
 discrete_optimization/rcpsp_multiskill/solvers/lns_post_process_rcpsp.py
 discrete_optimization/rcpsp_multiskill/solvers/lp_model.py
-discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_cp_lns_solver.py
 discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_ga_solver.py
 discrete_optimization/rcpsp_multiskill/solvers/ms_rcpsp_lp_lns_solver.py
 discrete_optimization/rcpsp_multiskill/solvers/multimode_transposition.py
 discrete_optimization/rcpsp_multiskill/solvers/solver_rcpsp_based.py
 discrete_optimization/tsp/__init__.py
 discrete_optimization/tsp/common_tools_tsp.py
 discrete_optimization/tsp/tsp_model.py
@@ -297,14 +303,15 @@
 examples/knapsack/knapsack_cpmpy.py
 examples/knapsack/knapsack_cpsat_solver.py
 examples/knapsack/knapsack_decomposition_solver.py
 examples/knapsack/knapsack_multidimensional.py
 examples/knapsack/multiscenario_knap.py
 examples/knapsack/optuna_example.py
 examples/knapsack/solvers_run.py
+examples/maximum_independent_set/qiskit_application.py
 examples/pickup_vrp/classic_ortools_example.py
 examples/pickup_vrp/cp_solver_gpdp_example.py
 examples/pickup_vrp/linear_flow_solver_examples.py
 examples/pickup_vrp/loading_example.py
 examples/pickup_vrp/optuna_full_example.py
 examples/pickup_vrp/pickup_vrp_ortools_with_optuna.py
 examples/pickup_vrp/pickup_vrp_ortools_with_optuna_auto.py
@@ -365,14 +372,15 @@
 tests/knapsack/test_knapsack_greedy_solvers.py
 tests/knapsack/test_knapsack_lns_cp_solver.py
 tests/knapsack/test_knapsack_lp_lns_solver.py
 tests/knapsack/test_knapsack_ls_solver.py
 tests/knapsack/test_knapsack_nsga.py
 tests/knapsack/test_knapsack_solvers.py
 tests/knapsack/test_parser.py
+tests/maximum_independent_set/test_maximum_independent_set.py
 tests/pickup_vrp/builders/test_instance_builders.py
 tests/pickup_vrp/builders/test_linear_flow_solver.py
 tests/pickup_vrp/builders/test_linear_flow_solver_pymip.py
 tests/pickup_vrp/solvers/test_ortools_solver.py
 tests/rcpsp/test_rcpsp_distance_between_solutions.py
 tests/rcpsp/test_rcpsp_ga.py
 tests/rcpsp/test_rcpsp_model.py
@@ -381,15 +389,14 @@
 tests/rcpsp/test_rcpsp_parser.py
 tests/rcpsp/test_rcpsp_preemptive.py
 tests/rcpsp/test_rcpsp_uncertain_model.py
 tests/rcpsp/test_rcpsp_utils.py
 tests/rcpsp/test_sgs_without_array.py
 tests/rcpsp/solver/test_large_neighborhood_search_solver.py
 tests/rcpsp/solver/test_rcpsp_cp.py
-tests/rcpsp/solver/test_rcpsp_cp_lns.py
 tests/rcpsp/solver/test_rcpsp_cpm.py
 tests/rcpsp/solver/test_rcpsp_find_modes.py
 tests/rcpsp/solver/test_rcpsp_local_search.py
 tests/rcpsp/solver/test_rcpsp_lp.py
 tests/rcpsp/solver/test_rcpsp_lp_lns.py
 tests/rcpsp/solver/test_rcpsp_pile.py
 tests/rcpsp/solver/test_rcpsp_resource_optim.py
```

### Comparing `discrete_optimization-0.3.0/docs/Makefile` & `discrete_optimization-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/README.md` & `discrete_optimization-0.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/generate_nb_index.py` & `discrete_optimization-0.3.1/docs/generate_nb_index.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/make.bat` & `discrete_optimization-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/source/_static/versions.js` & `discrete_optimization-0.3.1/docs/source/_static/versions.js`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/source/conf.py` & `discrete_optimization-0.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/source/contribute.md` & `discrete_optimization-0.3.1/docs/source/contribute.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/source/index.md` & `discrete_optimization-0.3.1/docs/source/index.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/docs/source/install.md` & `discrete_optimization-0.3.1/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/coloring_asp_solver.py` & `discrete_optimization-0.3.1/examples/coloring/coloring_asp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/coloring_cpspat_solver_example.py` & `discrete_optimization-0.3.1/examples/coloring/coloring_cpspat_solver_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/coloring_gurobi_solver.py` & `discrete_optimization-0.3.1/examples/coloring/coloring_gurobi_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/coloring_run_all_solvers.py` & `discrete_optimization-0.3.1/examples/coloring/coloring_run_all_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/optuna_all_solvers_coloring_with_pruning_based_on_time.py` & `discrete_optimization-0.3.1/examples/coloring/optuna_all_solvers_coloring_with_pruning_based_on_time.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/optuna_all_solvers_coloring_without_pruning.py` & `discrete_optimization-0.3.1/examples/coloring/optuna_all_solvers_coloring_without_pruning.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/optuna_full_example_all_solvers_timed_pruning.py` & `discrete_optimization-0.3.1/examples/coloring/optuna_full_example_all_solvers_timed_pruning.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/optuna_full_example_coloring.py` & `discrete_optimization-0.3.1/examples/coloring/optuna_full_example_coloring.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/coloring/toulbar_coloring_example.py` & `discrete_optimization-0.3.1/examples/coloring/toulbar_coloring_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/facility/gphh_facility_example.py` & `discrete_optimization-0.3.1/examples/facility/gphh_facility_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/knapsack_asp_solver.py` & `discrete_optimization-0.3.1/examples/knapsack/knapsack_asp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/knapsack_cpmpy.py` & `discrete_optimization-0.3.1/examples/knapsack/knapsack_cpmpy.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/knapsack_cpsat_solver.py` & `discrete_optimization-0.3.1/examples/knapsack/knapsack_cpsat_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/knapsack_decomposition_solver.py` & `discrete_optimization-0.3.1/examples/knapsack/knapsack_decomposition_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/knapsack_multidimensional.py` & `discrete_optimization-0.3.1/examples/knapsack/knapsack_multidimensional.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/multiscenario_knap.py` & `discrete_optimization-0.3.1/examples/knapsack/multiscenario_knap.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/optuna_example.py` & `discrete_optimization-0.3.1/examples/knapsack/optuna_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/knapsack/solvers_run.py` & `discrete_optimization-0.3.1/examples/knapsack/solvers_run.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/classic_ortools_example.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/classic_ortools_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/cp_solver_gpdp_example.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/cp_solver_gpdp_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/linear_flow_solver_examples.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/linear_flow_solver_examples.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/loading_example.py` & `discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_linear_flow_solver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,310 +1,299 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
-import logging
-import os
-import pickle
-import random
-import time
-
-import matplotlib.pyplot as plt
-import numpy as np
-import scipy.spatial.distance as dist
-from sklearn.cluster import KMeans
+import pytest
+from matplotlib import pyplot as plt
 
 import discrete_optimization.tsp.tsp_parser as tsp_parser
 import discrete_optimization.vrp.vrp_parser as vrp_parser
+from discrete_optimization.generic_tools.callbacks.early_stoppers import (
+    NbIterationStopper,
+)
+from discrete_optimization.generic_tools.result_storage.result_storage import (
+    ResultStorage,
+)
 from discrete_optimization.pickup_vrp.builders.instance_builders import (
-    create_pickup_and_delivery,
     create_selective_tsp,
 )
 from discrete_optimization.pickup_vrp.gpdp import (
-    GPDP,
     GPDPSolution,
     ProxyClass,
     build_pruned_problem,
 )
 from discrete_optimization.pickup_vrp.plots.gpdp_plot_utils import plot_gpdp_solution
 from discrete_optimization.pickup_vrp.solver.lp_solver import (
     LinearFlowSolver,
     ParametersMilp,
 )
-from discrete_optimization.pickup_vrp.solver.ortools_solver import (
-    FirstSolutionStrategy,
-    LocalSearchMetaheuristic,
-    ORToolsGPDP,
-    ParametersCost,
-)
 
-logging.basicConfig(level=logging.DEBUG)
+try:
+    import gurobipy as grb
+except ImportError:
+    gurobi_available = False
+else:
+    gurobi_available = True
 
+epsilon = 0.000001
 
-def load_vrp_and_transform():
-    file_path = vrp_parser.get_data_available()[1]
-    vrp_model = vrp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model)
 
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_tsp_new_api():
+    files_available = tsp_parser.get_data_available()
+    file_path = [f for f in files_available if "tsp_5_1" in f][0]
+    tsp_model = tsp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
+    )
+    p = ParametersMilp.default()
+
+    p.time_limit = 100
+    res = linear_flow_solver.solve(
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    )
+    assert isinstance(res, ResultStorage)
+    sol = res.get_best_solution()
+    assert isinstance(sol, GPDPSolution)
+    assert len(sol.times) == 0
+    # check origin and target for each trajectory
+    for v, trajectory in sol.trajectories.items():
+        assert trajectory[0] == gpdp.origin_vehicle[v]
+        assert trajectory[-1] == gpdp.target_vehicle[v]
+    # check size of trajectories
+    nb_nodes_visited = sum([len(traj) for traj in sol.trajectories.values()])
+    assert nb_nodes_visited == len(gpdp.all_nodes)
 
-def load_tsp_and_transform():
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_tsp_cb():
     files_available = tsp_parser.get_data_available()
-    file_path = files_available[1]
+    file_path = [f for f in files_available if "tsp_5_1" in f][0]
     tsp_model = tsp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
+    )
+    p = ParametersMilp.default()
 
+    p.time_limit = 100
+    iteration_stopper = NbIterationStopper(nb_iteration_max=2)
+    res = linear_flow_solver.solve(
+        parameters_milp=p,
+        do_lns=False,
+        nb_iteration_max=20,
+        include_subtour=False,
+        callbacks=[iteration_stopper],
+    )
+    assert (
+        iteration_stopper.nb_iteration > 0
+        and iteration_stopper.nb_iteration <= iteration_stopper.nb_iteration_max
+    )
 
-def debug_lp():
-    vrp = False
-    tsp = True
-    if tsp:
-        files_available = tsp_parser.get_data_available()
-        file_path = files_available[16]
-        tsp_model = tsp_parser.parse_file(file_path)
-        gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
-    else:
-        file_path = vrp_parser.get_data_available()[1]
-        vrp_model = vrp_parser.parse_file(file_path)
-        gpdp = ProxyClass.from_vrp_model_to_gpdp(
-            vrp_model=vrp_model, compute_graph=True
-        )
-    simplify = False
-    if simplify:
-        gpdp = build_pruned_problem(gpdp)
-    print(gpdp.graph.get_nodes())
-    print(len(gpdp.graph.get_nodes()))
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_tsp_new_api_with_time():
+    files_available = tsp_parser.get_data_available()
+    file_path = [f for f in files_available if "tsp_5_1" in f][0]
+    tsp_model = tsp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=True
+    )
     p = ParametersMilp.default()
-    p.time_limit = 2000
+
+    p.time_limit = 100
+    res = linear_flow_solver.solve(
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    )
+    assert isinstance(res, ResultStorage)
+    sol = res.get_best_solution()
+    assert isinstance(sol, GPDPSolution)
+    # check origin + target + times increasing for each trajectory
+    for v, trajectory in sol.trajectories.items():
+        assert trajectory[0] == gpdp.origin_vehicle[v]
+        assert trajectory[-1] == gpdp.target_vehicle[v]
+        for i in range(len(trajectory) - 1):
+            assert (
+                sol.times[trajectory[i]]
+                + gpdp.time_delta[trajectory[i]][trajectory[i + 1]]
+                <= sol.times[trajectory[i + 1]] + epsilon
+            )
+    # check size of trajectories
+    nb_nodes_visited = sum([len(traj) for traj in sol.trajectories.values()])
+    assert nb_nodes_visited == len(gpdp.all_nodes)
+
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_tsp():
+    files_available = tsp_parser.get_data_available()
+    file_path = [f for f in files_available if "tsp_5_1" in f][0]
+    tsp_model = tsp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
+    )
+    p = ParametersMilp.default()
+
+    p.time_limit = 100
     res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=4, include_subtour=False
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
     )
     sol: GPDPSolution = res.get_best_solution()
     plot_gpdp_solution(sol, gpdp)
-    plt.show()
 
 
-def selective_tsp():
-    gpdp = create_selective_tsp()
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_tsp_simplified():
+    files_available = tsp_parser.get_data_available()
+    file_path = [f for f in files_available if "tsp_5_1" in f][0]
+    tsp_model = tsp_parser.parse_file(file_path)
+    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
+    gpdp = build_pruned_problem(gpdp, compute_graph=True)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    p = ParametersMilp.default()
-    p.time_limit = 30
     linear_flow_solver.init_model(
-        one_visit_per_cluster=True, one_visit_per_node=False, include_subtour=False
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
     )
+    p = ParametersMilp.default()
+
+    p.time_limit = 100
     res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=True, nb_iteration_max=4, include_subtour=False
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
     )
     sol: GPDPSolution = res.get_best_solution()
     plot_gpdp_solution(sol, gpdp)
-    plt.show()
 
 
-def vrp_capacity():
-    file_path = vrp_parser.get_data_available()[4]
-    print(file_path)
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_vrp():
+    files_available = vrp_parser.get_data_available()
+    file_path = [f for f in files_available if "vrp_16_3_1" in f][0]
     vrp_model = vrp_parser.parse_file(file_path)
-    print("Nb vehicle : ", vrp_model.vehicle_count)
-    print("Capacities : ", vrp_model.vehicle_capacities)
     gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model, compute_graph=True)
-    simplify = False
-    if simplify:
-        gpdp = build_pruned_problem(gpdp)
-    print(gpdp.graph.get_nodes())
-    print(len(gpdp.graph.get_nodes()))
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    p = ParametersMilp.default()
-    p.time_limit = 30
     linear_flow_solver.init_model(
-        include_capacity=True,
-        include_resources=False,
-        one_visit_per_node=True,
-        include_time_evolution=False,
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
     )
+    p = ParametersMilp.default()
+
+    p.time_limit = 100
     res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=True, nb_iteration_max=4
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
     )
     sol: GPDPSolution = res.get_best_solution()
     plot_gpdp_solution(sol, gpdp)
-    plt.show()
 
 
-def run_ortools_solver():
-    file_path = vrp_parser.get_data_available()[4]
-    print(file_path)
+@pytest.mark.skip(reason="build_pruned_problem() is buggy for now.")
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_vrp_simplified():
+    files_available = vrp_parser.get_data_available()
+    file_path = [f for f in files_available if "vrp_16_3_1" in f][0]
     vrp_model = vrp_parser.parse_file(file_path)
-    print("Nb vehicle : ", vrp_model.vehicle_count)
-    print("Capacities : ", vrp_model.vehicle_capacities)
-    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model)
-    solver = ORToolsGPDP(problem=gpdp)
-    solver.init_model(
-        one_visit_per_cluster=False,
-        one_visit_per_node=True,
-        time_limit=10,
-    )
-    result_storage = solver.solve()
-    best_sol = result_storage.best_solution
-    plot_gpdp_solution(best_sol, gpdp)
-    plt.show()
-
-
-def run_ortools_solver_selective():
-    gpdp = create_selective_tsp(nb_nodes=600, nb_vehicles=5, nb_clusters=100)
-    solver = ORToolsGPDP(
-        problem=gpdp, factor_multiplier_distance=1, factor_multiplier_time=1
+    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model, compute_graph=True)
+    gpdp = build_pruned_problem(gpdp, compute_graph=True)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
     )
-    solver.init_model(
-        one_visit_per_cluster=True,
+    p = ParametersMilp.default()
+    p.time_limit = 100
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_selective_tsp():
+    gpdp = create_selective_tsp(nb_nodes=20, nb_vehicles=1, nb_clusters=4)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
         one_visit_per_node=False,
-        include_time_dimension=True,
-        include_demand=True,
-        include_mandatory=True,
-        include_pickup_and_delivery=False,
-        include_equilibrate_charge=True,
-        charge_constraint={
-            v: (len(gpdp.clusters_to_node) // (2 * gpdp.number_vehicle), None)
-            for v in range(gpdp.number_vehicle)
-        },
-        parameters_cost=[ParametersCost(dimension_name="Distance")],
-        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
-        first_solution_strategy=FirstSolutionStrategy.SAVINGS,
-        time_limit=200,
-    )
-    result_storage = solver.solve()
-    best_sol = result_storage.best_solution
-    plot_gpdp_solution(best_sol, gpdp)
-    plt.show()
-
-
-def run_ortools_pickup_delivery():
-    def check_solution(res, gpdp: GPDP):
-        for p, d in gpdp.list_pickup_deliverable:
-            index_vehicles_p = set(
-                [[i for i in range(len(res)) if pp in res[i]][0] for pp in p]
-            )
-            index_vehicles_d = set(
-                [[i for i in range(len(res)) if dd in res[i]][0] for dd in d]
-            )
-            assert len(index_vehicles_p) == 1
-            assert len(index_vehicles_d) == 1
-            vehicle_p = list(index_vehicles_p)[0]
-            vehicle_d = list(index_vehicles_d)[0]
-            assert vehicle_p == vehicle_d
-            index_p = [res[vehicle_p].index(pp) for pp in p]
-            index_d = [res[vehicle_d].index(dd) for dd in d]
-            assert max(index_p) < min(index_d)
-
-    model = create_pickup_and_delivery(
-        number_of_vehicles=4,
-        number_of_node=100,
-        include_pickup=True,
-        fraction_of_pickup_deliver=0.125,
-        include_cluster=False,
-        pickup_per_cluster=False,
-    )
-    list_params_cost = [
-        ParametersCost(
-            dimension_name="Distance",
-            global_span=True,
-            sum_over_vehicles=False,
-            coefficient_vehicles=10,
-        ),
-        ParametersCost(
-            dimension_name="Distance",
-            global_span=False,
-            sum_over_vehicles=True,
-            coefficient_vehicles=[1] * model.number_vehicle,
-        ),
-    ]
-    solver = ORToolsGPDP(problem=model)
-    solver.init_model(
-        one_visit_per_cluster=False,
-        one_visit_per_node=True,
-        include_pickup_and_delivery=True,
-        use_lns=True,
-        parameters_cost=list_params_cost,
-        include_equilibrate_charge=True,
-        charge_constraint={
-            v: (len(model.all_nodes) // (4 * model.number_vehicle), None)
-            for v in range(model.number_vehicle)
-        },
-        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
-        first_solution_strategy=FirstSolutionStrategy.SAVINGS,
-        time_limit=100,
-    )
-    logging.basicConfig(level=logging.DEBUG)
-    result_storage = solver.solve()
-    best_sol = result_storage.best_solution
-    assert best_sol.check_pickup_deliverable()
-    plot_gpdp_solution(best_sol, model)
-    plt.show()
-
-
-def run_ortools_pickup_delivery_cluster():
-    gpdp = create_pickup_and_delivery(
-        number_of_node=200,
-        include_cluster=True,
-        include_pickup=False,
-        pickup_per_cluster=True,
+        one_visit_per_cluster=True,
+        include_capacity=False,
+        include_time_evolution=False,
     )
-    solver = ORToolsGPDP(problem=gpdp)
-    solver.init_model(
+    p = ParametersMilp.default()
+    p.time_limit = 100
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_selective_vrp():
+    gpdp = create_selective_tsp(nb_nodes=20, nb_vehicles=3, nb_clusters=4)
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
+        one_visit_per_node=False,
         one_visit_per_cluster=True,
+        include_capacity=False,
+        include_time_evolution=False,
+    )
+    p = ParametersMilp.default()
+    p.time_limit = 100
+    res = linear_flow_solver.solve_iterative(
+        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    )
+    sol: GPDPSolution = res.get_best_solution()
+    plot_gpdp_solution(sol, gpdp)
+
+
+@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+def test_selective_vrp_new_api_with_time():
+    nb_nodes = 10
+    nb_vehicles = 2
+    nb_clusters = 4
+    gpdp = create_selective_tsp(
+        nb_nodes=nb_nodes, nb_vehicles=nb_vehicles, nb_clusters=nb_clusters
+    )
+    linear_flow_solver = LinearFlowSolver(problem=gpdp)
+    linear_flow_solver.init_model(
         one_visit_per_node=False,
-        include_pickup_and_delivery=False,
-        include_mandatory=False,
-        include_pickup_and_delivery_per_cluster=True,
-        local_search_metaheuristic=LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH,
-        first_solution_strategy=FirstSolutionStrategy.PARALLEL_CHEAPEST_INSERTION,
-        time_limit=30,
-    )
-    result_storage = solver.solve()
-    best_sol = result_storage.best_solution
-    assert best_sol.check_pickup_deliverable()
-    plot_gpdp_solution(best_sol, gpdp)
-    plt.show()
-
-
-def create_examples_script(folder_to_save):
-    if not os.path.exists(folder_to_save):
-        os.makedirs(folder_to_save)
-    sizes = [10, 50, 150, 300, 1000]
-    sizes = [1000]
-    include_cluster = [True, False]
-    include_pickup = [True, False]
-    pickup_per_cluster = [True, False]
-    for s in sizes:
-        for cl in include_cluster:
-            for picdel in include_pickup:
-                for pickupcluster in pickup_per_cluster:
-                    if pickupcluster and not include_cluster:
-                        continue
-                    if picdel and not cl and pickup_per_cluster:
-                        continue
-                    for n in range(1):
-                        gpdp = create_pickup_and_delivery(
-                            number_of_node=s,
-                            include_cluster=cl,
-                            include_pickup=picdel,
-                            pickup_per_cluster=pickupcluster,
-                        )
-                        t = time.time_ns()
-                        pickle.dump(
-                            gpdp,
-                            file=open(
-                                os.path.join(
-                                    folder_to_save,
-                                    f"gpdp_size{s}_cluster{cl}_pickup{picdel}_pickuppercluster{pickupcluster}_time{t}.pk",
-                                ),
-                                "wb",
-                            ),
-                        )
+        one_visit_per_cluster=True,
+        include_capacity=False,
+        include_time_evolution=True,
+    )
+    p = ParametersMilp.default()
+    p.time_limit = 100
+    res = linear_flow_solver.solve(
+        parameters_milp=p,
+        do_lns=False,
+        nb_iteration_max=20,
+    )
+    assert isinstance(res, ResultStorage)
+    sol = res.get_best_solution()
+    assert isinstance(sol, GPDPSolution)
+
+    # check origin + target + times increasing for each trajectory
+    for v, trajectory in sol.trajectories.items():
+        assert trajectory[0] == gpdp.origin_vehicle[v]
+        assert trajectory[-1] == gpdp.target_vehicle[v]
+        for i in range(len(trajectory) - 1):
+            assert (
+                sol.times[trajectory[i]]
+                + gpdp.time_delta[trajectory[i]][trajectory[i + 1]]
+                <= sol.times[trajectory[i + 1]] + epsilon
+            )
+    #  check clusters visited at least once
+    node_visited = set()
+    for trajectory in sol.trajectories.values():
+        node_visited.update(trajectory)
+    nb_visit_per_cluster = {
+        cluster: len([node for node in nodes if node in node_visited])
+        for cluster, nodes in gpdp.clusters_to_node.items()
+    }
+    for cluster, nb_visit in nb_visit_per_cluster.items():
+        assert nb_visit > 0
 
 
 if __name__ == "__main__":
-    # debug_lp()
-    # selective_tsp()
-    # vrp_capacity()
-    run_ortools_solver()
-    # run_ortools_pickup_delivery()
-    # run_ortools_solver_selective()
-    # run_ortools_pickup_delivery_cluster()
+    test_vrp()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/optuna_full_example.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/optuna_full_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_auto.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_auto.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4_auto.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/pickup_vrp_ortools_with_optuna_with_pruning_v4_auto.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/plots_wip/animated_plot.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/plots_wip/animated_plot.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/pickup_vrp/time_windows_example.py` & `discrete_optimization-0.3.1/examples/pickup_vrp/time_windows_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_cpsat_solver_example.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_cpsat_solver_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_lns_example.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_cp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-#  Copyright (c) 2024 AIRBUS and its affiliates.
+#  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
-import logging
 
-from discrete_optimization.generic_rcpsp_tools.large_neighborhood_search_scheduling import (
-    LargeNeighborhoodSearchScheduling,
-)
-from discrete_optimization.generic_tools.callbacks.early_stoppers import TimerStopper
-from discrete_optimization.generic_tools.cp_tools import ParametersCP
-from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
-from discrete_optimization.rcpsp.rcpsp_parser import get_data_available, parse_file
-
-logging.basicConfig(level=logging.INFO)
-
-
-def example_lns_solver():
-    files_available = get_data_available()
-    file = [f for f in files_available if "j1201_1.sm" in f][0]
-    rcpsp_problem: RCPSPModel = parse_file(file)
-    solver = LargeNeighborhoodSearchScheduling(problem=rcpsp_problem)
-    parameters_cp = ParametersCP.default()
-    parameters_cp.time_limit_iter0 = 5
-    parameters_cp.time_limit = 2
-    results = solver.solve(
-        nb_iteration_lns=100,
-        skip_first_iteration=False,
-        stop_first_iteration_if_optimal=False,
-        parameters_cp=parameters_cp,
-        nb_iteration_no_improvement=200,
-        callbacks=[TimerStopper(total_seconds=100)],
+import sys
+
+import pytest
+
+from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
+from discrete_optimization.tsp.solver.tsp_cp_solver import TSP_CP_Solver, TSP_CPModel
+from discrete_optimization.tsp.tsp_parser import get_data_available, parse_file
+
+
+@pytest.mark.skipif(sys.platform.startswith("win"), reason="Much too long on windows")
+def test_int_cp():
+    files = get_data_available()
+    files = [f for f in files if "tsp_100_3" in f]
+    model = parse_file(files[0], start_index=0, end_index=10)
+    model_type = TSP_CPModel.INT_VERSION
+    cp_solver = TSP_CP_Solver(
+        model, model_type=model_type, cp_solver_name=CPSolverName.CHUFFED
     )
-    sol, fit = results.get_best_solution_fit()
-    assert rcpsp_problem.satisfy(sol)
+    parameters_cp = ParametersCP.default()
+    parameters_cp.time_limit = 20
+    cp_solver.init_model()
+    var, fit = cp_solver.solve(parameters_cp=parameters_cp).get_best_solution_fit()
+    assert model.satisfy(var)
+
+
+def test_float_cp():
+    files = get_data_available()
+    files = [f for f in files if "tsp_100_3" in f]
+    model = parse_file(files[0], start_index=0, end_index=10)
+    model_type = TSP_CPModel.FLOAT_VERSION
+    cp_solver = TSP_CP_Solver(
+        model, model_type=model_type, cp_solver_name=CPSolverName.GECODE
+    )  # CHUFFED WONT WORK FOR FLOAT
+    parameters_cp = ParametersCP.default()
+    parameters_cp.time_limit = 20
+    cp_solver.init_model()
+    var, fit = cp_solver.solve(parameters_cp=parameters_cp).get_best_solution_fit()
+    assert model.satisfy(var)
 
 
 if __name__ == "__main__":
-    example_lns_solver()
+    test_int_cp()
```

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna_multiobj.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna_multiobj.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_local_search_with_optuna_with_pruning.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_local_search_with_optuna_with_pruning.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_lp_cplex_solver.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_lp_cplex_solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #  Copyright (c) 2023 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 import os
 
+from discrete_optimization.datasets import get_data_home
+
 os.environ["DO_SKIP_MZN_CHECK"] = "1"
 from discrete_optimization.generic_tools.lp_tools import ParametersMilp
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_parser import get_data_available, parse_file
@@ -32,9 +34,27 @@
     print(results_storage.list_solution_fits)
     assert rcpsp_problem.satisfy(solution)
     plot_resource_individual_gantt(rcpsp_problem, solution)
     plot_ressource_view(rcpsp_problem, solution)
     plt.show()
 
 
+def run_rcpsp_lp_cplex():
+    data_folder_rcp = f"{get_data_home()}/rcpsp/RG300/"
+    files_patterson = get_data_available(data_folder=data_folder_rcp)
+    file = [f for f in files_patterson if "RG300_190.rcp" in f][0]
+    rcpsp_problem: RCPSPModel = parse_file(file)
+    solver = LP_RCPSP_CPLEX(problem=rcpsp_problem)
+    solver.init_model(greedy_start=False, max_horizon=370)
+    parameters_milp = ParametersMilp.default()
+    parameters_milp.time_limit = 10000
+    results_storage: ResultStorage = solver.solve(parameters_milp=parameters_milp)
+    solution, fit = results_storage.get_best_solution_fit()
+    print(results_storage.list_solution_fits)
+    assert rcpsp_problem.satisfy(solution)
+    plot_resource_individual_gantt(rcpsp_problem, solution)
+    plot_ressource_view(rcpsp_problem, solution)
+    plt.show()
+
+
 if __name__ == "__main__":
-    run_rcpsp_sm_lp_cplex()
+    run_rcpsp_lp_cplex()
```

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_pareto_example.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_pareto_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/rcpsp_solvers_script.py` & `discrete_optimization-0.3.1/examples/rcpsp/rcpsp_solvers_script.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp/robustness_experiments.py` & `discrete_optimization-0.3.1/examples/rcpsp/robustness_experiments.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp_multiskill/mslib/mslib_parse_and_solve.py` & `discrete_optimization-0.3.1/examples/rcpsp_multiskill/mslib/mslib_parse_and_solve.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp_multiskill/mspsp/mspsp_parse_and_solve.py` & `discrete_optimization-0.3.1/examples/rcpsp_multiskill/mspsp/mspsp_parse_and_solve.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp_multiskill/sgs_runs.py` & `discrete_optimization-0.3.1/examples/rcpsp_multiskill/sgs_runs.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/rcpsp_multiskill/solvers/rcpsp_multiskills_runs.py` & `discrete_optimization-0.3.1/examples/rcpsp_multiskill/solvers/rcpsp_multiskills_runs.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/examples/vrp/vrp_solver_example.py` & `discrete_optimization-0.3.1/examples/vrp/vrp_solver_example.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/Knapsack tutorial.ipynb` & `discrete_optimization-0.3.1/notebooks/Knapsack tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-1 Introduction.ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-1 Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-2 Heuristics Solving.ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-2 Heuristics Solving.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-3 Local search.ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-3 Local search.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-4 Linear programming.ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-4 Linear programming.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-5 Constraint Programming.ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-5 Constraint Programming.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/RCPSP tutorials/RCPSP-6 Large Neighbourhood Search .ipynb` & `discrete_optimization-0.3.1/notebooks/RCPSP tutorials/RCPSP-6 Large Neighbourhood Search .ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/img/sgs.png` & `discrete_optimization-0.3.1/notebooks/img/sgs.png`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/z_Advanced/callbacks.ipynb` & `discrete_optimization-0.3.1/notebooks/z_Advanced/callbacks.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/notebooks/z_Advanced/optuna.ipynb` & `discrete_optimization-0.3.1/notebooks/z_Advanced/optuna.ipynb`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/pyproject.toml` & `discrete_optimization-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     "typing-extensions>=4.0",
     "cpmpy>=0.9.9",
     "scipy",
     "numpy>=1.21",
     "typing_extensions>=4.4",
     "clingo>=5.6",
     "setuptools",
+    "qiskit>=1.0.2",
+    "qiskit-algorithms>=0.3.0",
+    "qiskit-optimization>=0.6.1"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov", "scikit-learn>=1.0", "optuna"]
 
 [project.urls]
```

### Comparing `discrete_optimization-0.3.0/scripts/trigger_binder.sh` & `discrete_optimization-0.3.1/scripts/trigger_binder.sh`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/coloring/test_coloring.py` & `discrete_optimization-0.3.1/tests/coloring/test_coloring.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 import logging
+import platform
 import random
 import sys
 
 import numpy as np
 import pytest
 from minizinc.solver import Solver
 
@@ -53,15 +54,15 @@
 from discrete_optimization.generic_tools.do_problem import (
     ObjectiveHandling,
     TypeAttribute,
     get_default_objective_setup,
 )
 from discrete_optimization.generic_tools.ea.ga import DeapMutation, Ga
 from discrete_optimization.generic_tools.ea.nsga import Nsga
-from discrete_optimization.generic_tools.lp_tools import ParametersMilp
+from discrete_optimization.generic_tools.lp_tools import ParametersMilp, PymipMilpSolver
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     plot_storage_2d,
 )
 
 try:
     import gurobipy
 except ImportError:
@@ -99,43 +100,54 @@
     assert coloring_model.satisfy(dummy_solution)
 
 
 @pytest.mark.parametrize("solver_class", solvers_map)
 def test_solvers(solver_class):
     if solver_class == ColoringLP and not gurobi_available:
         pytest.skip("You need Gurobi to test this solver.")
+    if issubclass(solver_class, PymipMilpSolver) and platform.machine() == "arm64":
+        pytest.skip(
+            "Python-mip has issues with cbclib on macos arm64. "
+            "See https://github.com/coin-or/python-mip/issues/167"
+        )
     small_example = [f for f in get_data_available() if "gc_20_1" in f][0]
     coloring_model: ColoringProblem = parse_file(small_example)
     results = solve(
         method=solver_class, problem=coloring_model, **solvers_map[solver_class][1]
     )
     sol, fit = results.get_best_solution_fit()
 
 
-def test_solvers_subset():
+@pytest.mark.parametrize("solver_class", solvers_map)
+def test_solvers_subset(solver_class):
+    if solver_class == ColoringLP and not gurobi_available:
+        pytest.skip("You need Gurobi to test this solver.")
+    if issubclass(solver_class, PymipMilpSolver) and platform.machine() == "arm64":
+        pytest.skip(
+            "Python-mip has issues with cbclib on macos arm64. "
+            "See https://github.com/coin-or/python-mip/issues/167"
+        )
+
     small_example = [f for f in get_data_available() if "gc_20_1" in f][0]
     coloring_model: ColoringProblem = parse_file(small_example)
     coloring_model = transform_coloring_problem(
         coloring_model,
         subset_nodes=set(range(10)),
         constraints_coloring=ConstraintsColoring(color_constraint={0: 0, 1: 1, 2: 2}),
     )
     assert coloring_model.graph is not None
     assert coloring_model.number_of_nodes is not None
     assert coloring_model.graph.nodes_name is not None
-    solvers = solvers_map.keys()
-    for s in solvers:
-        logger.info(f"Running {s}")
-        if s == ColoringLP and not gurobi_available:
-            # you need a gurobi licence to test this solver.
-            continue
-        results = solve(method=s, problem=coloring_model, **solvers_map[s][1])
-        sol, fit = results.get_best_solution_fit()
-        print(f"Solver {s}, fitness = {fit}")
-        print(f"Evaluation : {coloring_model.evaluate(sol)}")
+
+    results = solve(
+        method=solver_class, problem=coloring_model, **solvers_map[solver_class][1]
+    )
+    sol, fit = results.get_best_solution_fit()
+    print(f"Solver {solver_class}, fitness = {fit}")
+    print(f"Evaluation : {coloring_model.evaluate(sol)}")
 
 
 def test_mzn_solver_cb(caplog):
     small_example = [f for f in get_data_available() if "gc_50_9" in f][0]
     coloring_model: ColoringProblem = parse_file(small_example)
     parameters_cp = ParametersCP.default()
     parameters_cp.time_limit = 10
```

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_cp.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_cp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_ga.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_greedy.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_greedy.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_lp.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_lp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import os
+import platform
 
 import pytest
 
 from discrete_optimization.facility.facility_parser import (
     get_data_available,
     parse_file,
 )
@@ -51,14 +52,21 @@
         parameters_milp=parameters_lp,
         use_matrix_indicator_heuristic=False,
     ).get_best_solution_fit()
     assert color_problem.satisfy(solution)
 
 
 @pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+@pytest.mark.skipif(
+    platform.machine() == "arm64",
+    reason=(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167"
+    ),
+)
 def test_facility_lp_pymip():
     file = [f for f in get_data_available() if os.path.basename(f) == "fl_100_7"][0]
     facility_problem = parse_file(file)
     params_objective_function = get_default_objective_setup(problem=facility_problem)
     parameters_lp = ParametersMilp.default()
     parameters_lp.time_limit = 20
     solver = LP_Facility_Solver_PyMip(
```

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_lp_lns.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_lp_lns.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
 import os
+import platform
 
 import pytest
 
 from discrete_optimization.facility.facility_parser import (
     get_data_available,
     parse_file,
 )
@@ -29,14 +30,21 @@
 except ImportError:
     gurobi_available = False
 else:
     gurobi_available = True
 
 
 @pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
+@pytest.mark.skipif(
+    platform.machine() == "arm64",
+    reason=(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167"
+    ),
+)
 def test_facility_lns():
     file = [f for f in get_data_available() if os.path.basename(f) == "fl_16_1"][0]
     facility_problem = parse_file(file)
     params_objective_function = get_default_objective_setup(problem=facility_problem)
     params_milp = ParametersMilp(
         time_limit=20,
         pool_solutions=1000,
```

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_parser.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/facility/test_facility_problem.py` & `discrete_optimization-0.3.1/tests/facility/test_facility_problem.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_rcpsp_tools/test_graph_tools_rcpsp.py` & `discrete_optimization-0.3.1/tests/generic_rcpsp_tools/test_graph_tools_rcpsp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/callbacks/test_ortools_with_callbacks.py` & `discrete_optimization-0.3.1/tests/generic_tools/callbacks/test_ortools_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/callbacks/test_sa_with_callbacks.py` & `discrete_optimization-0.3.1/tests/generic_tools/callbacks/test_sa_with_callbacks.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/ea/test_ga.py` & `discrete_optimization-0.3.1/tests/generic_tools/ea/test_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/hyperparameters/test_hyperparameter.py` & `discrete_optimization-0.3.1/tests/generic_tools/hyperparameters/test_hyperparameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,29 +47,37 @@
 
     def solve(
         self, callbacks: Optional[List[Callback]] = None, **kwargs: Any
     ) -> ResultStorage:
         return ResultStorage([])
 
 
-class MetaSolver(SolverDO):
+class BaseMetaSolver(SolverDO):
     hyperparameters = [
         IntegerHyperparameter("nb", low=0, high=1, default=1),
-        SubBrickHyperparameter("subsolver", choices=[DummySolver, DummySolver2]),
+        SubBrickHyperparameter("subsolver", choices=[DummySolver]),
         SubBrickKwargsHyperparameter(
             "kwargs_subsolver", subbrick_hyperparameter="subsolver"
         ),
     ]
 
     def solve(
         self, callbacks: Optional[List[Callback]] = None, **kwargs: Any
     ) -> ResultStorage:
         return ResultStorage([])
 
 
+class MetaSolver(BaseMetaSolver):
+    # we check that copy_and_update_hyperparameters create a hyperparameter subsolver
+    # whose attribute choices_str2cls is working properly
+    hyperparameters = BaseMetaSolver.copy_and_update_hyperparameters(
+        subsolver=dict(choices=[DummySolver, DummySolver2]),
+    )
+
+
 class MetaMetaSolver(SolverDO):
     hyperparameters = [
         IntegerHyperparameter("nb", low=1, high=1, default=1),
         SubBrickHyperparameter("subsolver", choices=[MetaSolver]),
         SubBrickKwargsHyperparameter(
             "kwargs_subsolver", subbrick_hyperparameter="subsolver"
         ),
@@ -298,7 +306,24 @@
 
     study = optuna.create_study(
         sampler=optuna.samplers.BruteForceSampler(),
     )
     study.optimize(objective)
 
     assert len(study.trials) == 2 * (3 * 5)
+
+
+def test_copy_and_update_hyperparameters():
+    hyperparameters = DummySolver.copy_and_update_hyperparameters(
+        nb=dict(high=5), use_it=dict(choices=[False])
+    )
+    original_hyperparameters = DummySolver.hyperparameters
+    assert len(hyperparameters) == len(original_hyperparameters)
+    for h, ho in zip(hyperparameters, original_hyperparameters):
+        assert h.name == ho.name
+        assert h is not ho
+        if h.name == "nb":
+            assert h.high == 5
+            assert ho.high == 2
+        elif h.name == "use_it":
+            assert len(h.choices) == 1
+            assert len(ho.choices) == 2
```

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/mutations/test_bool.py` & `discrete_optimization-0.3.1/tests/generic_tools/mutations/test_bool.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/test_graph_api.py` & `discrete_optimization-0.3.1/tests/generic_tools/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/generic_tools/test_multiobj_utils.py` & `discrete_optimization-0.3.1/tests/generic_tools/test_multiobj_utils.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cp_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cpmyp.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cpmyp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_cpsat_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_cpsat_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_decomposition_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_decomposition_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_ga.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_gphh.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_gphh.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_greedy_solvers.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_greedy_solvers.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_lns_cp_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_lns_cp_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_lp_lns_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_lp_lns_solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
+import platform
+
+import pytest
+
 from discrete_optimization.generic_tools.callbacks.early_stoppers import TimerStopper
 from discrete_optimization.generic_tools.do_problem import get_default_objective_setup
 from discrete_optimization.generic_tools.lns_mip import LNS_MILP
 from discrete_optimization.generic_tools.lp_tools import MilpSolverName, ParametersMilp
 from discrete_optimization.knapsack.knapsack_parser import (
     get_data_available,
     parse_file,
@@ -13,14 +17,21 @@
     ConstraintHandlerKnapsack,
     InitialKnapsackMethod,
     InitialKnapsackSolution,
 )
 from discrete_optimization.knapsack.solvers.lp_solvers import KnapsackModel, LPKnapsack
 
 
+@pytest.mark.skipif(
+    platform.machine() == "arm64",
+    reason=(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167"
+    ),
+)
 def test_knapsack_lns():
     model_file = [f for f in get_data_available() if "ks_30_0" in f][0]
     model: KnapsackModel = parse_file(model_file)
     params_objective_function = get_default_objective_setup(problem=model)
     params_milp = ParametersMilp(
         time_limit=10,
         pool_solutions=1000,
```

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_ls_solver.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_ls_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_nsga.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_nsga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_knapsack_solvers.py` & `discrete_optimization-0.3.1/tests/knapsack/test_knapsack_solvers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 import logging
+import platform
 import random
 
 import numpy as np
 import pytest
 
+from discrete_optimization.generic_tools.lp_tools import PymipMilpSolver
 from discrete_optimization.knapsack.knapsack_model import (
     KnapsackModel,
     KnapsackSolution,
 )
 from discrete_optimization.knapsack.knapsack_parser import (
     get_data_available,
     parse_file,
@@ -35,19 +37,25 @@
 @pytest.mark.parametrize("knapsack_problem_file", get_data_available())
 def test_load_file(knapsack_problem_file):
     knapsack_model: KnapsackModel = parse_file(knapsack_problem_file)
     dummy_solution = knapsack_model.get_dummy_solution()
     assert knapsack_model.satisfy(dummy_solution)
 
 
-def test_solvers():
+@pytest.mark.parametrize("solver_class", solvers_map)
+def test_solvers(solver_class):
+    if solver_class == LPKnapsackGurobi and not gurobi_available:
+        pytest.skip("You need Gurobi to test this solver.")
+    if issubclass(solver_class, PymipMilpSolver) and platform.machine() == "arm64":
+        pytest.skip(
+            "Python-mip has issues with cbclib on macos arm64. "
+            "See https://github.com/coin-or/python-mip/issues/167"
+        )
+
     logging.basicConfig(level=logging.INFO)
     small_example = [f for f in get_data_available() if "ks_40_0" in f][0]
     knapsack_model: KnapsackModel = parse_file(small_example)
-    solvers = solvers_map.keys()
-    for s in solvers:
-        if s == LPKnapsackGurobi:
-            continue
-        logging.info(f"Solver {s}")
-        results = solve(method=s, problem=knapsack_model, **solvers_map[s][1])
-        s, f = results.get_best_solution_fit()
-        logging.info(f"fitness={f}")
+    results = solve(
+        method=solver_class, problem=knapsack_model, **solvers_map[solver_class][1]
+    )
+    s, f = results.get_best_solution_fit()
+    logging.info(f"fitness={f}")
```

### Comparing `discrete_optimization-0.3.0/tests/knapsack/test_parser.py` & `discrete_optimization-0.3.1/tests/knapsack/test_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/pickup_vrp/builders/test_instance_builders.py` & `discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_instance_builders.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/pickup_vrp/builders/test_linear_flow_solver.py` & `discrete_optimization-0.3.1/tests/pickup_vrp/builders/test_linear_flow_solver_pymip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
+import platform
 
 import pytest
-from matplotlib import pyplot as plt
 
 import discrete_optimization.tsp.tsp_parser as tsp_parser
 import discrete_optimization.vrp.vrp_parser as vrp_parser
 from discrete_optimization.generic_tools.callbacks.early_stoppers import (
     NbIterationStopper,
 )
 from discrete_optimization.generic_tools.result_storage.result_storage import (
@@ -17,102 +17,106 @@
     create_selective_tsp,
 )
 from discrete_optimization.pickup_vrp.gpdp import (
     GPDPSolution,
     ProxyClass,
     build_pruned_problem,
 )
-from discrete_optimization.pickup_vrp.plots.gpdp_plot_utils import plot_gpdp_solution
-from discrete_optimization.pickup_vrp.solver.lp_solver import (
+from discrete_optimization.pickup_vrp.solver.lp_solver_pymip import (
     LinearFlowSolver,
     ParametersMilp,
 )
 
 try:
     import gurobipy as grb
 except ImportError:
     gurobi_available = False
 else:
     gurobi_available = True
+import logging
 
 epsilon = 0.000001
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_tsp_new_api():
+if platform.machine() == "arm64":
+    pytest.skip(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167",
+        allow_module_level=True,
+    )
+
+
+def test_tsp():
+    logging.basicConfig(level=logging.DEBUG)
     files_available = tsp_parser.get_data_available()
     file_path = [f for f in files_available if "tsp_5_1" in f][0]
     tsp_model = tsp_parser.parse_file(file_path)
     gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
+        one_visit_per_node=True,
+        include_capacity=False,
+        include_time_evolution=False,
     )
     p = ParametersMilp.default()
 
     p.time_limit = 100
     res = linear_flow_solver.solve(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+        parameters_milp=p,
+        do_lns=True,
+        nb_iteration_max=20,
     )
     assert isinstance(res, ResultStorage)
     sol = res.get_best_solution()
     assert isinstance(sol, GPDPSolution)
     assert len(sol.times) == 0
     # check origin and target for each trajectory
     for v, trajectory in sol.trajectories.items():
         assert trajectory[0] == gpdp.origin_vehicle[v]
         assert trajectory[-1] == gpdp.target_vehicle[v]
     # check size of trajectories
     nb_nodes_visited = sum([len(traj) for traj in sol.trajectories.values()])
     assert nb_nodes_visited == len(gpdp.all_nodes)
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
 def test_tsp_cb():
     files_available = tsp_parser.get_data_available()
     file_path = [f for f in files_available if "tsp_5_1" in f][0]
     tsp_model = tsp_parser.parse_file(file_path)
     gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
+        one_visit_per_node=True,
+        include_capacity=False,
+        include_time_evolution=False,
     )
     p = ParametersMilp.default()
-
-    p.time_limit = 100
     iteration_stopper = NbIterationStopper(nb_iteration_max=2)
     res = linear_flow_solver.solve(
         parameters_milp=p,
-        do_lns=False,
+        do_lns=True,
         nb_iteration_max=20,
-        include_subtour=False,
         callbacks=[iteration_stopper],
     )
-    assert (
-        iteration_stopper.nb_iteration > 0
-        and iteration_stopper.nb_iteration <= iteration_stopper.nb_iteration_max
-    )
+    assert iteration_stopper.nb_iteration == iteration_stopper.nb_iteration_max
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_tsp_new_api_with_time():
+def test_tsp_with_time():
     files_available = tsp_parser.get_data_available()
     file_path = [f for f in files_available if "tsp_5_1" in f][0]
     tsp_model = tsp_parser.parse_file(file_path)
     gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
         one_visit_per_node=True, include_capacity=False, include_time_evolution=True
     )
     p = ParametersMilp.default()
 
     p.time_limit = 100
-    res = linear_flow_solver.solve(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
-    )
+    res = linear_flow_solver.solve(parameters_milp=p, do_lns=False, nb_iteration_max=20)
     assert isinstance(res, ResultStorage)
     sol = res.get_best_solution()
     assert isinstance(sol, GPDPSolution)
     # check origin + target + times increasing for each trajectory
     for v, trajectory in sol.trajectories.items():
         assert trajectory[0] == gpdp.origin_vehicle[v]
         assert trajectory[-1] == gpdp.target_vehicle[v]
@@ -123,138 +127,100 @@
                 <= sol.times[trajectory[i + 1]] + epsilon
             )
     # check size of trajectories
     nb_nodes_visited = sum([len(traj) for traj in sol.trajectories.values()])
     assert nb_nodes_visited == len(gpdp.all_nodes)
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_tsp():
-    files_available = tsp_parser.get_data_available()
-    file_path = [f for f in files_available if "tsp_5_1" in f][0]
-    tsp_model = tsp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
-    linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
-    )
-    p = ParametersMilp.default()
-
-    p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
-    )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
-
-
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_tsp_simplified():
-    files_available = tsp_parser.get_data_available()
-    file_path = [f for f in files_available if "tsp_5_1" in f][0]
-    tsp_model = tsp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_tsp_model_gpdp(tsp_model=tsp_model, compute_graph=True)
-    gpdp = build_pruned_problem(gpdp, compute_graph=True)
-    linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
-    )
-    p = ParametersMilp.default()
-
-    p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
-    )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
-
-
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_vrp():
-    files_available = vrp_parser.get_data_available()
-    file_path = [f for f in files_available if "vrp_16_3_1" in f][0]
-    vrp_model = vrp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model, compute_graph=True)
-    linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
-    )
-    p = ParametersMilp.default()
-
-    p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
-    )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
-
-
-@pytest.mark.skip(reason="build_pruned_problem() is buggy for now.")
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_vrp_simplified():
-    files_available = vrp_parser.get_data_available()
-    file_path = [f for f in files_available if "vrp_16_3_1" in f][0]
-    vrp_model = vrp_parser.parse_file(file_path)
-    gpdp = ProxyClass.from_vrp_model_to_gpdp(vrp_model=vrp_model, compute_graph=True)
-    gpdp = build_pruned_problem(gpdp, compute_graph=True)
-    linear_flow_solver = LinearFlowSolver(problem=gpdp)
-    linear_flow_solver.init_model(
-        one_visit_per_node=True, include_capacity=False, include_time_evolution=False
-    )
-    p = ParametersMilp.default()
-    p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+def test_selective_tsp_with_time():
+    nb_nodes = 20
+    nb_vehicles = 1
+    nb_clusters = 4
+    gpdp = create_selective_tsp(
+        nb_nodes=nb_nodes, nb_vehicles=nb_vehicles, nb_clusters=nb_clusters
     )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
-
-
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_selective_tsp():
-    gpdp = create_selective_tsp(nb_nodes=20, nb_vehicles=1, nb_clusters=4)
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
         one_visit_per_node=False,
         one_visit_per_cluster=True,
         include_capacity=False,
-        include_time_evolution=False,
+        include_time_evolution=True,
     )
     p = ParametersMilp.default()
     p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
-    )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
+    res = linear_flow_solver.solve(parameters_milp=p, do_lns=False, nb_iteration_max=20)
+    assert isinstance(res, ResultStorage)
+    sol = res.get_best_solution()
+    assert isinstance(sol, GPDPSolution)
+    # check origin + target + times increasing for each trajectory
+    for v, trajectory in sol.trajectories.items():
+        assert trajectory[0] == gpdp.origin_vehicle[v]
+        assert trajectory[-1] == gpdp.target_vehicle[v]
+        for i in range(len(trajectory) - 1):
+            assert (
+                sol.times[trajectory[i]]
+                + gpdp.time_delta[trajectory[i]][trajectory[i + 1]]
+                <= sol.times[trajectory[i + 1]] + epsilon
+            )
+    # check clusters visited at least once
+    node_visited = set()
+    for trajectory in sol.trajectories.values():
+        node_visited.update(trajectory)
+    nb_visit_per_cluster = {
+        cluster: len([node for node in nodes if node in node_visited])
+        for cluster, nodes in gpdp.clusters_to_node.items()
+    }
+    for cluster, nb_visit in nb_visit_per_cluster.items():
+        assert nb_visit > 0
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
 def test_selective_vrp():
-    gpdp = create_selective_tsp(nb_nodes=20, nb_vehicles=3, nb_clusters=4)
+    nb_nodes = 20
+    nb_vehicles = 3
+    nb_clusters = 4
+    gpdp = create_selective_tsp(
+        nb_nodes=nb_nodes, nb_vehicles=nb_vehicles, nb_clusters=nb_clusters
+    )
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
         one_visit_per_node=False,
         one_visit_per_cluster=True,
         include_capacity=False,
         include_time_evolution=False,
     )
     p = ParametersMilp.default()
     p.time_limit = 100
-    res = linear_flow_solver.solve_iterative(
-        parameters_milp=p, do_lns=False, nb_iteration_max=20, include_subtour=False
+    res = linear_flow_solver.solve(
+        parameters_milp=p,
+        do_lns=False,
+        nb_iteration_max=20,
     )
-    sol: GPDPSolution = res.get_best_solution()
-    plot_gpdp_solution(sol, gpdp)
+    assert isinstance(res, ResultStorage)
+    sol = res.get_best_solution()
+    assert isinstance(sol, GPDPSolution)
+    assert len(sol.times) == 0  # no time computed
+    # check origin and target for each trajectory
+    for v, trajectory in sol.trajectories.items():
+        assert trajectory[0] == gpdp.origin_vehicle[v]
+        assert trajectory[-1] == gpdp.target_vehicle[v]
+    #  check clusters visited at least once
+    node_visited = set()
+    for trajectory in sol.trajectories.values():
+        node_visited.update(trajectory)
+    nb_visit_per_cluster = {
+        cluster: len([node for node in nodes if node in node_visited])
+        for cluster, nodes in gpdp.clusters_to_node.items()
+    }
+    for cluster, nb_visit in nb_visit_per_cluster.items():
+        assert nb_visit > 0
 
 
-@pytest.mark.skipif(not gurobi_available, reason="You need Gurobi to test this solver.")
-def test_selective_vrp_new_api_with_time():
-    nb_nodes = 10
-    nb_vehicles = 2
+def test_selective_vrp_with_time():
+    nb_nodes = 20
+    nb_vehicles = 3
     nb_clusters = 4
     gpdp = create_selective_tsp(
         nb_nodes=nb_nodes, nb_vehicles=nb_vehicles, nb_clusters=nb_clusters
     )
     linear_flow_solver = LinearFlowSolver(problem=gpdp)
     linear_flow_solver.init_model(
         one_visit_per_node=False,
@@ -268,15 +234,14 @@
         parameters_milp=p,
         do_lns=False,
         nb_iteration_max=20,
     )
     assert isinstance(res, ResultStorage)
     sol = res.get_best_solution()
     assert isinstance(sol, GPDPSolution)
-
     # check origin + target + times increasing for each trajectory
     for v, trajectory in sol.trajectories.items():
         assert trajectory[0] == gpdp.origin_vehicle[v]
         assert trajectory[-1] == gpdp.target_vehicle[v]
         for i in range(len(trajectory) - 1):
             assert (
                 sol.times[trajectory[i]]
@@ -289,11 +254,7 @@
         node_visited.update(trajectory)
     nb_visit_per_cluster = {
         cluster: len([node for node in nodes if node in node_visited])
         for cluster, nodes in gpdp.clusters_to_node.items()
     }
     for cluster, nb_visit in nb_visit_per_cluster.items():
         assert nb_visit > 0
-
-
-if __name__ == "__main__":
-    test_vrp()
```

### Comparing `discrete_optimization-0.3.0/tests/pickup_vrp/solvers/test_ortools_solver.py` & `discrete_optimization-0.3.1/tests/pickup_vrp/solvers/test_ortools_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_large_neighborhood_search_solver.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_large_neighborhood_search_solver.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cp.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_cp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cp_lns.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_lp_lns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,142 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
-from discrete_optimization.generic_tools.callbacks.early_stoppers import TimerStopper
-from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
-from discrete_optimization.generic_tools.do_problem import get_default_objective_setup
-from discrete_optimization.generic_tools.lns_cp import LNS_CP
-from discrete_optimization.generic_tools.lns_mip import TrivialInitialSolution
-from discrete_optimization.generic_tools.result_storage.result_storage import (
-    from_solutions_to_result_storage,
+
+import platform
+
+import pytest
+
+from discrete_optimization.generic_tools.do_problem import (
+    ModeOptim,
+    ObjectiveHandling,
+    ParamsObjectiveFunction,
+    get_default_objective_setup,
 )
+from discrete_optimization.generic_tools.lns_mip import LNS_MILP
+from discrete_optimization.generic_tools.lp_tools import MilpSolverName, ParametersMilp
 from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
 from discrete_optimization.rcpsp.rcpsp_parser import get_data_available, parse_file
 from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
 from discrete_optimization.rcpsp.rcpsp_utils import (
     plot_resource_individual_gantt,
     plot_ressource_view,
 )
-from discrete_optimization.rcpsp.solver.cp_solvers import CP_MRCPSP_MZN, CP_RCPSP_MZN
-from discrete_optimization.rcpsp.solver.rcpsp_cp_lns_solver import (
-    LNS_CP_RCPSP_SOLVER,
-    ConstraintHandlerStartTimeInterval_CP,
-    OptionNeighbor,
-)
 from discrete_optimization.rcpsp.solver.rcpsp_lp_lns_solver import (
+    ConstraintHandlerFixStartTime,
+    ConstraintHandlerStartTimeInterval,
+    ConstraintHandlerStartTimeIntervalMRCPSP,
     InitialMethodRCPSP,
     InitialSolutionRCPSP,
 )
+from discrete_optimization.rcpsp.solver.rcpsp_lp_solver import LP_MRCPSP, LP_RCPSP
+
+if platform.machine() == "arm64":
+    pytest.skip(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167",
+        allow_module_level=True,
+    )
 
 
 def test_lns_sm():
     files_available = get_data_available()
-    file = [f for f in files_available if "j1201_1.sm" in f][0]
-    rcpsp_problem: RCPSPModel = parse_file(file)
-    solver = CP_RCPSP_MZN(problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED)
-    solver.init_model(output_type=True)
-    parameters_cp = ParametersCP.default()
-    parameters_cp.time_limit = 5
+    file = [f for f in files_available if "j301_1.sm" in f][0]
+    rcpsp_problem = parse_file(file)
+    solver = LP_RCPSP(problem=rcpsp_problem, lp_solver=MilpSolverName.CBC)
+    solver.init_model(greedy_start=False)
+    parameters_milp = ParametersMilp(
+        time_limit=10,
+        pool_solutions=1000,
+        mip_gap_abs=0.001,
+        mip_gap=0.001,
+        retrieve_all_solution=True,
+        n_solutions_max=100,
+    )
     params_objective_function = get_default_objective_setup(problem=rcpsp_problem)
-    constraint_handler = ConstraintHandlerStartTimeInterval_CP(
-        problem=rcpsp_problem,
-        fraction_to_fix=1.0,
-        # here i want to apply bounds constraint on all the tasks
-        minus_delta=10,
-        plus_delta=10,
+    constraint_handler = ConstraintHandlerStartTimeInterval(
+        problem=rcpsp_problem, fraction_to_fix=0.8, minus_delta=5, plus_delta=5
     )
-
-    some_solution = rcpsp_problem.get_dummy_solution()  # starting solution
-    initial_solution_provider = TrivialInitialSolution(
-        solution=from_solutions_to_result_storage(
-            [some_solution], problem=rcpsp_problem
-        )
+    initial_solution_provider = InitialSolutionRCPSP(
+        problem=rcpsp_problem,
+        initial_method=InitialMethodRCPSP.DUMMY,
+        params_objective_function=params_objective_function,
     )
-    lns_solver = LNS_CP(
+    lns_solver = LNS_MILP(
         problem=rcpsp_problem,
-        cp_solver=solver,
+        milp_solver=solver,
         initial_solution_provider=initial_solution_provider,
         constraint_handler=constraint_handler,
         params_objective_function=params_objective_function,
     )
     result_store = lns_solver.solve_lns(
-        parameters_cp=parameters_cp, nb_iteration_lns=10
+        parameters_milp=parameters_milp, nb_iteration_lns=10
     )
     solution, fit = result_store.get_best_solution_fit()
     solution_rebuilt = RCPSPSolution(
         problem=rcpsp_problem, rcpsp_permutation=solution.rcpsp_permutation
     )
     fit_2 = rcpsp_problem.evaluate(solution_rebuilt)
     assert rcpsp_problem.evaluate(solution) == fit_2
     assert rcpsp_problem.satisfy(solution)
     plot_resource_individual_gantt(rcpsp_problem, solution)
     plot_ressource_view(rcpsp_problem, solution)
 
 
 def test_lns_mm():
     files_available = get_data_available()
-    file = [f for f in files_available if "j1010_9.mm" in f][0]
+    file = [f for f in files_available if "j1201_1.sm" in f][0]
     rcpsp_problem: RCPSPModel = parse_file(file)
     if rcpsp_problem.is_rcpsp_multimode():
         rcpsp_problem.set_fixed_modes([1 for i in range(rcpsp_problem.n_jobs)])
-    solver = CP_MRCPSP_MZN(problem=rcpsp_problem, cp_solver_name=CPSolverName.CHUFFED)
-    solver.init_model()
-    parameters_cp = ParametersCP.default()
-    parameters_cp.time_limit = 5
     params_objective_function = get_default_objective_setup(problem=rcpsp_problem)
-    constraint_handler = ConstraintHandlerStartTimeInterval_CP(
-        problem=rcpsp_problem, fraction_to_fix=0.7, minus_delta=5, plus_delta=5
+    params_objective_function = ParamsObjectiveFunction(
+        objectives=["makespan"],
+        weights=[-1],
+        objective_handling=ObjectiveHandling.AGGREGATE,
+        sense_function=ModeOptim.MAXIMIZATION,
+    )
+    solver = LP_MRCPSP(
+        problem=rcpsp_problem,
+        lp_solver=MilpSolverName.CBC,
+        params_objective_function=params_objective_function,
+    )
+    solver.init_model(greedy_start=False)
+    parameters_milp = ParametersMilp(
+        time_limit=10,
+        pool_solutions=1000,
+        mip_gap_abs=0.001,
+        mip_gap=0.001,
+        retrieve_all_solution=True,
+        n_solutions_max=100,
+    )
+    constraint_handler = ConstraintHandlerFixStartTime(
+        problem=rcpsp_problem, fraction_fix_start_time=0.3
+    )
+    constraint_handler = ConstraintHandlerStartTimeIntervalMRCPSP(
+        problem=rcpsp_problem, fraction_to_fix=0.5, minus_delta=2, plus_delta=2
     )
     initial_solution_provider = InitialSolutionRCPSP(
         problem=rcpsp_problem,
-        initial_method=InitialMethodRCPSP.LS,
+        initial_method=InitialMethodRCPSP.DUMMY,
         params_objective_function=params_objective_function,
     )
-    lns_solver = LNS_CP(
+    lns_solver = LNS_MILP(
         problem=rcpsp_problem,
-        cp_solver=solver,
+        milp_solver=solver,
         initial_solution_provider=initial_solution_provider,
         constraint_handler=constraint_handler,
         params_objective_function=params_objective_function,
     )
     result_store = lns_solver.solve_lns(
-        parameters_cp=parameters_cp, nb_iteration_lns=10
-    )
-    solution, fit = result_store.get_best_solution_fit()
-    solution_rebuilt = RCPSPSolution(
-        problem=rcpsp_problem,
-        rcpsp_permutation=solution.rcpsp_permutation,
-        rcpsp_modes=solution.rcpsp_modes,
-    )
-    fit_2 = rcpsp_problem.evaluate(solution_rebuilt)
-    assert rcpsp_problem.evaluate(solution) == fit_2
-    assert rcpsp_problem.satisfy(solution)
-    plot_resource_individual_gantt(rcpsp_problem, solution)
-    plot_ressource_view(rcpsp_problem, solution)
-
-
-def test_lns_solver():
-    files_available = get_data_available()
-    file = [f for f in files_available if "j1201_1.sm" in f][0]
-    rcpsp_problem: RCPSPModel = parse_file(file)
-    parameters_cp = ParametersCP.default()
-    parameters_cp.time_limit = 20
-    lns_solver = LNS_CP_RCPSP_SOLVER(
-        problem=rcpsp_problem, option_neighbor=OptionNeighbor.MIX_ALL
-    )
-    result_store = lns_solver.solve(
-        parameters_cp=parameters_cp,
+        parameters_milp=parameters_milp,
         nb_iteration_lns=10,
-        callbacks=[TimerStopper(total_seconds=20)],
-        nb_iteration_no_improvement=10,
+        skip_first_iteration=False,
     )
     solution, fit = result_store.get_best_solution_fit()
-    solution_rebuilt = RCPSPSolution(
-        problem=rcpsp_problem, rcpsp_permutation=solution.rcpsp_permutation
-    )
-    fit_2 = rcpsp_problem.evaluate(solution_rebuilt)
-    assert rcpsp_problem.evaluate(solution) == fit_2
     assert rcpsp_problem.satisfy(solution)
     plot_resource_individual_gantt(rcpsp_problem, solution)
     plot_ressource_view(rcpsp_problem, solution)
 
 
 if __name__ == "__main__":
     test_lns_sm()
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_cpm.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_cpm.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_find_modes.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_find_modes.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_local_search.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_local_search.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_lp.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_lp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
+import platform
+
+import pytest
+
 from discrete_optimization.generic_tools.lp_tools import MilpSolverName, ParametersMilp
 from discrete_optimization.generic_tools.result_storage.result_storage import (
     ResultStorage,
 )
 from discrete_optimization.rcpsp.rcpsp_parser import get_data_available, parse_file
 from discrete_optimization.rcpsp.rcpsp_solution import PartialSolution, RCPSPSolution
 from discrete_optimization.rcpsp.rcpsp_utils import (
     plot_resource_individual_gantt,
     plot_ressource_view,
 )
 from discrete_optimization.rcpsp.solver.rcpsp_lp_solver import LP_MRCPSP, LP_RCPSP
 
+if platform.machine() == "arm64":
+    pytest.skip(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167",
+        allow_module_level=True,
+    )
+
 
 def test_rcpsp_sm_lp_cbc():
     files_available = get_data_available()
     file = [f for f in files_available if "j301_1.sm" in f][0]
     rcpsp_problem = parse_file(file)
     solver = LP_RCPSP(problem=rcpsp_problem, lp_solver=MilpSolverName.CBC)
     solver.init_model()
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_lp_lns.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_partially_preemptive.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,131 +1,138 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
-from discrete_optimization.generic_tools.do_problem import (
-    ModeOptim,
-    ObjectiveHandling,
-    ParamsObjectiveFunction,
-    get_default_objective_setup,
+from typing import Dict, List
+
+import pytest
+
+from discrete_optimization.generic_rcpsp_tools.ls_solver import (
+    LS_SOLVER,
+    LS_RCPSP_Solver,
 )
-from discrete_optimization.generic_tools.lns_mip import LNS_MILP
-from discrete_optimization.generic_tools.lp_tools import MilpSolverName, ParametersMilp
-from discrete_optimization.rcpsp.rcpsp_model import RCPSPModel
-from discrete_optimization.rcpsp.rcpsp_parser import get_data_available, parse_file
-from discrete_optimization.rcpsp.rcpsp_solution import RCPSPSolution
-from discrete_optimization.rcpsp.rcpsp_utils import (
-    plot_resource_individual_gantt,
-    plot_ressource_view,
+from discrete_optimization.generic_tools.cp_tools import ParametersCP
+from discrete_optimization.rcpsp.plots.rcpsp_utils_preemptive import plot_ressource_view
+from discrete_optimization.rcpsp.special_constraints import (
+    SpecialConstraintsDescription,
 )
-from discrete_optimization.rcpsp.solver.rcpsp_lp_lns_solver import (
-    ConstraintHandlerFixStartTime,
-    ConstraintHandlerStartTimeInterval,
-    ConstraintHandlerStartTimeIntervalMRCPSP,
-    InitialMethodRCPSP,
-    InitialSolutionRCPSP,
+from discrete_optimization.rcpsp_multiskill.plots.plot_solution import (
+    plot_resource_individual_gantt_preemptive,
+)
+from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill import (
+    Employee,
+    MS_RCPSPModel,
+    MS_RCPSPModel_Variant,
+    SkillDetail,
+    compute_constraints_details,
+)
+from discrete_optimization.rcpsp_multiskill.solvers.cp_solvers import (
+    CP_MS_MRCPSP_MZN_PARTIAL_PREEMPTIVE,
 )
-from discrete_optimization.rcpsp.solver.rcpsp_lp_solver import LP_MRCPSP, LP_RCPSP
-
-
-def test_lns_sm():
-    files_available = get_data_available()
-    file = [f for f in files_available if "j301_1.sm" in f][0]
-    rcpsp_problem = parse_file(file)
-    solver = LP_RCPSP(problem=rcpsp_problem, lp_solver=MilpSolverName.CBC)
-    solver.init_model(greedy_start=False)
-    parameters_milp = ParametersMilp(
-        time_limit=10,
-        pool_solutions=1000,
-        mip_gap_abs=0.001,
-        mip_gap=0.001,
-        retrieve_all_solution=True,
-        n_solutions_max=100,
-    )
-    params_objective_function = get_default_objective_setup(problem=rcpsp_problem)
-    constraint_handler = ConstraintHandlerStartTimeInterval(
-        problem=rcpsp_problem, fraction_to_fix=0.8, minus_delta=5, plus_delta=5
-    )
-    initial_solution_provider = InitialSolutionRCPSP(
-        problem=rcpsp_problem,
-        initial_method=InitialMethodRCPSP.DUMMY,
-        params_objective_function=params_objective_function,
-    )
-    lns_solver = LNS_MILP(
-        problem=rcpsp_problem,
-        milp_solver=solver,
-        initial_solution_provider=initial_solution_provider,
-        constraint_handler=constraint_handler,
-        params_objective_function=params_objective_function,
-    )
-    result_store = lns_solver.solve_lns(
-        parameters_milp=parameters_milp, nb_iteration_lns=10
-    )
-    solution, fit = result_store.get_best_solution_fit()
-    solution_rebuilt = RCPSPSolution(
-        problem=rcpsp_problem, rcpsp_permutation=solution.rcpsp_permutation
-    )
-    fit_2 = rcpsp_problem.evaluate(solution_rebuilt)
-    assert rcpsp_problem.evaluate(solution) == fit_2
-    assert rcpsp_problem.satisfy(solution)
-    plot_resource_individual_gantt(rcpsp_problem, solution)
-    plot_ressource_view(rcpsp_problem, solution)
-
-
-def test_lns_mm():
-    files_available = get_data_available()
-    file = [f for f in files_available if "j1201_1.sm" in f][0]
-    rcpsp_problem: RCPSPModel = parse_file(file)
-    if rcpsp_problem.is_rcpsp_multimode():
-        rcpsp_problem.set_fixed_modes([1 for i in range(rcpsp_problem.n_jobs)])
-    params_objective_function = get_default_objective_setup(problem=rcpsp_problem)
-    params_objective_function = ParamsObjectiveFunction(
-        objectives=["makespan"],
-        weights=[-1],
-        objective_handling=ObjectiveHandling.AGGREGATE,
-        sense_function=ModeOptim.MAXIMIZATION,
-    )
-    solver = LP_MRCPSP(
-        problem=rcpsp_problem,
-        lp_solver=MilpSolverName.CBC,
-        params_objective_function=params_objective_function,
-    )
-    solver.init_model(greedy_start=False)
-    parameters_milp = ParametersMilp(
-        time_limit=10,
-        pool_solutions=1000,
-        mip_gap_abs=0.001,
-        mip_gap=0.001,
-        retrieve_all_solution=True,
-        n_solutions_max=100,
-    )
-    constraint_handler = ConstraintHandlerFixStartTime(
-        problem=rcpsp_problem, fraction_fix_start_time=0.3
-    )
-    constraint_handler = ConstraintHandlerStartTimeIntervalMRCPSP(
-        problem=rcpsp_problem, fraction_to_fix=0.5, minus_delta=2, plus_delta=2
-    )
-    initial_solution_provider = InitialSolutionRCPSP(
-        problem=rcpsp_problem,
-        initial_method=InitialMethodRCPSP.DUMMY,
-        params_objective_function=params_objective_function,
-    )
-    lns_solver = LNS_MILP(
-        problem=rcpsp_problem,
-        milp_solver=solver,
-        initial_solution_provider=initial_solution_provider,
-        constraint_handler=constraint_handler,
-        params_objective_function=params_objective_function,
-    )
-    result_store = lns_solver.solve_lns(
-        parameters_milp=parameters_milp,
-        nb_iteration_lns=10,
-        skip_first_iteration=False,
-    )
-    solution, fit = result_store.get_best_solution_fit()
-    assert rcpsp_problem.satisfy(solution)
-    plot_resource_individual_gantt(rcpsp_problem, solution)
-    plot_ressource_view(rcpsp_problem, solution)
 
 
-if __name__ == "__main__":
-    test_lns_sm()
+@pytest.fixture
+def model():
+    skills_set = {"l1", "l2", "l3", "l4"}
+    resource_set = {"R1"}
+    resources_availability = {"R1": [2] * 100}
+    employee: Dict[int, Employee] = {
+        1: Employee(
+            dict_skill={
+                "l1": SkillDetail(1.0, 1.0, 1.0),
+                "l3": SkillDetail(1.0, 1.0, 1.0),
+            },
+            calendar_employee=[True] * 100,
+        ),
+        2: Employee(
+            dict_skill={
+                "l1": SkillDetail(1.0, 1.0, 1.0),
+                "l2": SkillDetail(1.0, 1.0, 1.0),
+                "l4": SkillDetail(1.0, 1.0, 1.0),
+            },
+            calendar_employee=[True] * 100,
+        ),
+    }
+
+    employees_availability: List[int] = [2] * 1000
+    mode_details = {
+        "A0": {1: {"R1": 0, "duration": 0}},
+        "A1": {1: {"R1": 1, "l1": 1, "duration": 5}},
+        "A2": {1: {"R1": 1, "l3": 1, "l4": 1, "duration": 1}},
+        "A3": {1: {"R1": 1, "l2": 1, "duration": 3}},
+        "A4": {1: {"R1": 0, "l3": 1, "duration": 2}},
+        "A5": {1: {"R1": 0, "duration": 0}},
+    }
+    successors: Dict[str, List[str]] = {
+        "A0": ["A" + str(i) for i in range(1, 6)],
+        "A1": ["A5"],
+        "A2": ["A5"],
+        "A3": ["A5"],
+        "A4": ["A5"],
+        "A5": [],
+    }
+    partial_preemptive_data = {
+        t: {m: {"R1": True} for m in mode_details[t]} for t in mode_details
+    }
+    special_constraint_description = SpecialConstraintsDescription(
+        start_times_window={"A2": (2, None), "A4": (5, None)},
+        end_times_window={"A2": (None, 3)},
+    )
+    return MS_RCPSPModel(
+        skills_set=skills_set,
+        resources_set=resource_set,
+        non_renewable_resources=set(),
+        resources_availability=resources_availability,
+        employees=employee,
+        employees_availability=employees_availability,
+        mode_details=mode_details,
+        successors=successors,
+        horizon=12,
+        tasks_list=["A" + str(i) for i in range(6)],
+        source_task="A0",
+        sink_task="A5",
+        preemptive=True,
+        preemptive_indicator={"A1": True, "A2": False, "A3": True, "A4": False},
+        special_constraints=special_constraint_description,
+        partial_preemption_data=partial_preemptive_data,
+    )
+
+
+def test_partial_preemptive(model):
+    model_variant: MS_RCPSPModel_Variant = model.to_variant_model()
+
+    dummy_solution = model_variant.get_dummy_solution(preemptive=True)
+    model.evaluate(dummy_solution)
+    compute_constraints_details(dummy_solution, model.special_constraints)
+    assert model.satisfy(dummy_solution)
+
+    plot_resource_individual_gantt_preemptive(
+        rcpsp_model=model, rcpsp_sol=dummy_solution
+    )
+    plot_ressource_view(rcpsp_model=model, rcpsp_sol=dummy_solution)
+    cp_solver = CP_MS_MRCPSP_MZN_PARTIAL_PREEMPTIVE(problem=model)
+    cp_solver.init_model(
+        max_time=20,
+        max_preempted=3,
+        nb_preemptive=10,
+        possibly_preemptive=[
+            model.preemptive_indicator.get(t, True) for t in model.tasks_list
+        ],
+        partial_solution=model.special_constraints,
+        add_partial_solution_hard_constraint=True,
+        unit_usage_preemptive=True,
+    )
+    result_storage = cp_solver.solve(parameters_cp=ParametersCP.default())
+    rcpsp_sol = result_storage.get_last_best_solution()[0]
+    assert model.satisfy(rcpsp_sol)
+    plot_resource_individual_gantt_preemptive(rcpsp_model=model, rcpsp_sol=rcpsp_sol)
+    plot_ressource_view(rcpsp_model=model, rcpsp_sol=rcpsp_sol)
+
+
+def test_ls(model):
+    model_variant: MS_RCPSPModel_Variant = model.to_variant_model()
+    solver = LS_RCPSP_Solver(problem=model_variant, ls_solver=LS_SOLVER.SA)
+    result_storage = solver.solve(nb_iteration_max=5000)
+    rcpsp_sol = result_storage.get_last_best_solution()[0]
+    assert model.satisfy(rcpsp_sol)
+    plot_resource_individual_gantt_preemptive(rcpsp_model=model, rcpsp_sol=rcpsp_sol)
+    plot_ressource_view(rcpsp_model=model, rcpsp_sol=rcpsp_sol)
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_pile.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_pile.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/solver/test_rcpsp_resource_optim.py` & `discrete_optimization-0.3.1/tests/rcpsp/solver/test_rcpsp_resource_optim.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_distance_between_solutions.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_distance_between_solutions.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_ga.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_model.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_model_preemptive.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_model_preemptive.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_nsga.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_nsga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_parser.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_parser.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_preemptive.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_preemptive.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_uncertain_model.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_uncertain_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_rcpsp_utils.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_rcpsp_utils.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp/test_sgs_without_array.py` & `discrete_optimization-0.3.1/tests/rcpsp/test_sgs_without_array.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_mspsp_cp.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_mspsp_cp.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_cp.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_ga.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
+import random
 from typing import Dict, List, Set
 
-from discrete_optimization.generic_tools.callbacks.early_stoppers import TimerStopper
-from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
-from discrete_optimization.rcpsp.solver.rcpsp_lp_lns_solver import InitialMethodRCPSP
+import numpy as np
+import pytest
+
+from discrete_optimization.generic_tools.do_problem import ObjectiveHandling
+from discrete_optimization.generic_tools.ea.alternating_ga import AlternatingGa
+from discrete_optimization.generic_tools.ea.ga import DeapCrossover, DeapMutation, Ga
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill import (
     Employee,
+    MS_RCPSPModel,
     MS_RCPSPModel_Variant,
-    MS_RCPSPSolution,
     SkillDetail,
 )
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill_parser import (
     get_data_available,
     parse_file,
 )
-from discrete_optimization.rcpsp_multiskill.solvers.cp_solvers import (
-    CP_MS_MRCPSP_MZN,
-    SearchStrategyMS_MRCPSP,
-)
-from discrete_optimization.rcpsp_multiskill.solvers.ms_rcpsp_cp_lns_solver import (
-    LNS_CP_MS_RCPSP_SOLVER,
-    OptionNeighbor,
-)
-from discrete_optimization.rcpsp_multiskill.solvers.ms_rcpsp_lp_lns_solver import (
-    InitialSolutionMS_RCPSP,
-)
+
+
+@pytest.fixture
+def random_seed():
+    random.seed(0)
+    np.random.seed(0)
 
 
 def create_toy_msrcpsp():
     skills_set: Set[str] = {"S1", "S2", "S3"}
     resources_set: Set[str] = {"R1", "R2", "R3"}
     non_renewable_resources = set()
     resources_availability = {"R1": [2] * 100, "R2": [4] * 100, "R3": [3] * 100}
@@ -45,50 +44,33 @@
             calendar_employee=[True] * 100,
         ),
         3: Employee(
             dict_skill={"S3": SkillDetail(1.0, 1.0, 1.0)},
             calendar_employee=[True] * 100,
         ),
     }
-    employee = {
-        1: Employee(
-            dict_skill={
-                "S1": SkillDetail(10, 0, 0),
-                "S2": SkillDetail(10, 0, 0),
-                "S3": SkillDetail(10, 0, 0),
-            },
-            calendar_employee=[True] * 100,
-        ),
-        2: Employee(
-            dict_skill={"S2": SkillDetail(10, 0, 0), "S3": SkillDetail(10, 0, 0)},
-            calendar_employee=[True] * 100,
-        ),
-        3: Employee(
-            dict_skill={"S3": SkillDetail(10, 0, 0)}, calendar_employee=[True] * 100
-        ),
-    }
     index = 5
     for emp in sorted(employee):
         indexes = [index + 8 * i for i in range(10)] + [
             index + 1 + 8 * i for i in range(10)
         ]
         for i in indexes:
-            employee[emp].calendar_employee[i] = True
+            employee[emp].calendar_employee[i] = False
         index += 1
 
     employees_availability: List[int] = [3] * 1000
     mode_details: Dict[int, Dict[int, Dict[str, int]]] = {
         1: {1: {"R1": 0, "R2": 0, "R3": 0, "duration": 0}},
         2: {
             1: {"S1": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 2},
             2: {"S2": 1, "R1": 0, "R2": 0, "R3": 0, "duration": 3},
         },
         3: {1: {"S2": 1, "R1": 1, "R2": 2, "R3": 0, "duration": 4}},
         4: {1: {"S3": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 5}},
-        5: {1: {"R1": 2, "R2": 0, "R3": 0, "S1": 1, "duration": 5}},
+        5: {1: {"R1": 2, "R2": 0, "R3": 0, "duration": 5}},
         6: {1: {"S3": 1, "S2": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 5}},
         7: {
             1: {"S3": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 1},
             2: {"R1": 2, "R2": 0, "R3": 0, "duration": 2},
         },
         8: {1: {"R1": 0, "R2": 0, "R3": 0, "duration": 0}},
     }
@@ -98,86 +80,86 @@
         3: [4],
         4: [5],
         5: [6, 7],
         6: [8],
         7: [8],
         8: [],
     }
-    model = MS_RCPSPModel_Variant(
+
+    model = MS_RCPSPModel(
         skills_set=skills_set,
         resources_set=resources_set,
         non_renewable_resources=non_renewable_resources,
         resources_availability=resources_availability,
         employees=employee,
         employees_availability=employees_availability,
         mode_details=mode_details,
         successors=successors,
         horizon=100,
         horizon_multiplier=1,
     )
     return model
 
 
-def create_toy_v2():
+def create_toy_msrcpsp_variant():
     skills_set: Set[str] = {"S1", "S2", "S3"}
     resources_set: Set[str] = {"R1", "R2", "R3"}
     non_renewable_resources = set()
-    resources_availability = {"R1": [200] * 100, "R2": [400] * 100, "R3": [300] * 100}
-
+    resources_availability = {"R1": [2] * 100, "R2": [4] * 100, "R3": [3] * 100}
     employee: Dict[int, Employee] = {
         1: Employee(
-            dict_skill={
-                "S1": SkillDetail(10, 0, 0),
-                "S2": SkillDetail(10, 0, 0),
-                "S3": SkillDetail(10, 0, 0),
-            },
+            dict_skill={"S1": SkillDetail(1.0, 1.0, 1.0)},
             calendar_employee=[True] * 100,
         ),
         2: Employee(
-            dict_skill={"S2": SkillDetail(10, 0, 0), "S3": SkillDetail(10, 0, 0)},
+            dict_skill={"S2": SkillDetail(1.0, 1.0, 1.0)},
             calendar_employee=[True] * 100,
         ),
-        3: Employee(
-            dict_skill={"S3": SkillDetail(10, 0, 0)}, calendar_employee=[True] * 100
+        4: Employee(
+            dict_skill={"S3": SkillDetail(1.0, 1.0, 1.0)},
+            calendar_employee=[True] * 100,
         ),
     }
     index = 5
     for emp in sorted(employee):
         indexes = [index + 8 * i for i in range(10)] + [
             index + 1 + 8 * i for i in range(10)
         ]
         for i in indexes:
-            employee[emp].calendar_employee[i] = True
+            employee[emp].calendar_employee[i] = False
         index += 1
 
     employees_availability: List[int] = [3] * 1000
     mode_details: Dict[int, Dict[int, Dict[str, int]]] = {
         1: {1: {"R1": 0, "R2": 0, "R3": 0, "duration": 0}},
-        2: {1: {"S1": 1, "S3": 1, "R1": 1, "R2": 0, "R3": 0, "duration": 2}},
+        2: {
+            1: {"S1": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 2},
+            2: {"S2": 1, "R1": 0, "R2": 0, "R3": 0, "duration": 3},
+        },
         3: {1: {"S2": 1, "R1": 1, "R2": 2, "R3": 0, "duration": 4}},
-        4: {1: {"S3": 1, "S2": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 5}},
-        5: {1: {"R1": 2, "R2": 0, "R3": 0, "S1": 1, "duration": 5}},
-        6: {1: {"S3": 1, "S2": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 6}},
+        4: {1: {"S3": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 5}},
+        5: {1: {"R1": 2, "R2": 0, "R3": 0, "duration": 5}},
+        6: {1: {"S3": 1, "S2": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 5}},
         7: {
             1: {"S3": 1, "R1": 2, "R2": 0, "R3": 0, "duration": 1},
-            2: {"R1": 2, "R2": 0, "R3": 0, "duration": 1},
+            2: {"R1": 2, "R2": 0, "R3": 0, "duration": 2},
         },
         8: {1: {"R1": 0, "R2": 0, "R3": 0, "duration": 0}},
     }
-
     successors: Dict[int, List[int]] = {
-        1: [],
-        2: [],
-        3: [],
-        4: [],
-        5: [],
-        6: [],
-        7: [],
+        1: [2, 3],
+        2: [5],
+        3: [4],
+        4: [5],
+        5: [6, 7],
+        6: [8],
+        7: [8],
         8: [],
     }
+
     model = MS_RCPSPModel_Variant(
         skills_set=skills_set,
         resources_set=resources_set,
         non_renewable_resources=non_renewable_resources,
         resources_availability=resources_availability,
         employees=employee,
         employees_availability=employees_availability,
@@ -185,137 +167,116 @@
         successors=successors,
         horizon=100,
         horizon_multiplier=1,
     )
     return model
 
 
-def test_cp_toy_model():
-    model_msrcpsp = create_toy_v2()
-
-    cp_model = CP_MS_MRCPSP_MZN(
-        problem=model_msrcpsp, cp_solver_name=CPSolverName.GECODE
-    )
-    cp_model.init_model(
-        add_calendar_constraint_unit=False,
-        fake_tasks=True,
-        output_type=True,
-        exact_skills_need=False,
-    )
-    parameters_cp = ParametersCP.default()
-    parameters_cp.intermediate_solution = True
-    parameters_cp.time_limit = 200
-    result_storage = cp_model.solve(parameters_cp=parameters_cp)
-    solution: MS_RCPSPSolution = result_storage.get_best_solution()
-    assert model_msrcpsp.satisfy(solution)
-
-
-def test_cp_imopse():
-
-    file = [f for f in get_data_available() if "100_5_20_9_D3.def" in f][0]
-    model_msrcpsp, new_tame_to_original_task_id = parse_file(file, max_horizon=1000)
-    cp_model = CP_MS_MRCPSP_MZN(
-        problem=model_msrcpsp,
-        one_ressource_per_task=True,
-        cp_solver_name=CPSolverName.CHUFFED,
-    )
-    cp_model.init_model(
-        model_type="multi-calendar",
-        add_calendar_constraint_unit=False,
-        fake_tasks=False,
-        add_objective_makespan=True,
-        ignore_sec_objective=True,
-        output_type=True,
-        max_time=500,  # here you put makespan constraint. by default,
-        # would use model_msrcpsp.horizon if not provided.
-        search_strategy=SearchStrategyMS_MRCPSP.PRIORITY_SEARCH_START_UNIT_USED,
-        exact_skills_need=False,
-    )
-    parameters_cp = ParametersCP.default()
-    parameters_cp.free_search = False
-    # With parameters_cp.free_search=True you get fast results but quite bad !
-    # but can be a good thing to be used in findmus algo
-    # with free_search=False, you get first results after 10 seconds or so, but good quality.
-    parameters_cp.intermediate_solution = True
-    parameters_cp.time_limit = 30
-    result_storage = cp_model.solve(parameters_cp=parameters_cp)
-    solution: MS_RCPSPSolution = result_storage.get_best_solution()
-    assert model_msrcpsp.satisfy(solution)
-    model_msrcpsp.evaluate(solution)
-
-
-def test_lns_small_neighbor():
-    files = [f for f in get_data_available() if f.endswith("100_5_64_9.def")]
-    f = files[0]
-    model_msrcpsp, new_tame_to_original_task_id = parse_file(f, max_horizon=2000)
-    model_msrcpsp = model_msrcpsp.to_variant_model()
-    initial_solution_provider = InitialSolutionMS_RCPSP(
-        problem=model_msrcpsp,
-        initial_method=InitialMethodRCPSP.PILE_CALENDAR,
-        params_objective_function=None,
-    )
-    solution = initial_solution_provider.get_starting_solution().get_best_solution()
-    makespan = model_msrcpsp.evaluate(solution)["makespan"]
-    model_msrcpsp.horizon = makespan + 5
-    lns_cp = LNS_CP_MS_RCPSP_SOLVER(
-        problem=model_msrcpsp,
-        option_neighbor=OptionNeighbor.MIX_FAST,
-        one_ressource_per_task=True,
-    )
-    parameters_cp = ParametersCP.default()
-    parameters_cp.intermediate_solution = True
-    parameters_cp.all_solutions = False
-    parameters_cp.time_limit = 10
-    parameters_cp.time_limit_iter0 = 10
-    result_storage = lns_cp.solve(
-        parameters_cp=parameters_cp,
-        nb_iteration_lns=100,
-        callbacks=[TimerStopper(total_seconds=100)],
-        nb_iteration_no_improvement=100,
-        skip_first_iteration=False,
-    )
-    solution: MS_RCPSPSolution = result_storage.get_best_solution()
-    assert model_msrcpsp.satisfy(solution)
-    model_msrcpsp.evaluate(solution)
-
-
-def test_lns():
-    file = [f for f in get_data_available() if "100_5_22_15.def" in f][0]
-
-    model_msrcpsp, new_tame_to_original_task_id = parse_file(file, max_horizon=2000)
-    model_msrcpsp = model_msrcpsp.to_variant_model()
-    initial_solution_provider = InitialSolutionMS_RCPSP(
-        problem=model_msrcpsp,
-        initial_method=InitialMethodRCPSP.PILE_CALENDAR,
-        params_objective_function=None,
-    )
-    solution = initial_solution_provider.get_starting_solution().get_best_solution()
-    makespan = model_msrcpsp.evaluate(solution)["makespan"]
-    model_msrcpsp.horizon = makespan + 5
-    model_rcpsp = model_msrcpsp.build_multimode_rcpsp_calendar_representative()
-    lns_cp = LNS_CP_MS_RCPSP_SOLVER(
-        problem=model_msrcpsp,
-        option_neighbor=OptionNeighbor.MIX_ALL,
-        one_ressource_per_task=True,
-        fake_tasks=True,
-        output_type=True,
-        exact_skills_need=False,
-    )
-    parameters_cp = ParametersCP.default()
-    parameters_cp.intermediate_solution = True
-    parameters_cp.all_solutions = False
-    parameters_cp.time_limit = 10
-    parameters_cp.time_limit_iter0 = 10
-    result_storage = lns_cp.solve(
-        parameters_cp=parameters_cp,
-        nb_iteration_lns=100,
-        callbacks=[TimerStopper(total_seconds=100)],
-        nb_iteration_no_improvement=100,
-        skip_first_iteration=False,
-    )
-    solution: MS_RCPSPSolution = result_storage.get_best_solution()
-    assert model_msrcpsp.satisfy(solution)
-    model_msrcpsp.evaluate(solution)
-
-
-if __name__ == "__main__":
-    test_cp_imopse()
+def test_alternating_ga_specific_mode_arity(random_seed):
+    msrcpsp_model = create_toy_msrcpsp_variant()
+    files = [f for f in get_data_available() if "100_5_64_9.def" in f]
+    msrcpsp_model, new_tame_to_original_task_id = parse_file(files[0], max_horizon=2000)
+    msrcpsp_model = msrcpsp_model.to_variant_model()
+
+    total_evals = 50
+    evals_per_ga_runs_perm = 0.33 * total_evals
+    evals_per_ga_runs_modes = 0.33 * total_evals
+    evals_per_ga_runs_resource_perm = 0.34 * total_evals
+
+    mode_mutation = DeapMutation.MUT_UNIFORM_INT
+    task_permutation_mutation = DeapMutation.MUT_SHUFFLE_INDEXES
+    resource_permutation_mutation = DeapMutation.MUT_SHUFFLE_INDEXES
+
+    # Initialise the task permutation that will be used to first search through the modes
+    initial_task_permutation = [i for i in range(msrcpsp_model.n_jobs_non_dummy)]
+    msrcpsp_model.set_fixed_task_permutation(initial_task_permutation)
+
+    # Initialise the resource permutation that will be used to first search through the modes
+    initial_resource_permutation = [
+        i for i in range(len(msrcpsp_model.tasks) * len(msrcpsp_model.employees.keys()))
+    ]
+    msrcpsp_model.set_fixed_priority_worker_per_task_from_permutation(
+        initial_resource_permutation
+    )
+
+    # Run a GA for evals_per_ga_runs evals on modes
+    ga_solver = Ga(
+        msrcpsp_model,
+        encoding="modes_arity_fix_from_0",
+        objective_handling=ObjectiveHandling.AGGREGATE,
+        objectives=["makespan"],
+        objective_weights=[-1],
+        mutation=mode_mutation,
+        max_evals=evals_per_ga_runs_modes,
+    )
+    tmp_sol = ga_solver.solve().get_best_solution()
+    # Fix the resulting modes
+    msrcpsp_model.set_fixed_modes(tmp_sol.modes_vector)
+
+    # Run a GA for evals_per_ga_runs evals on permutation
+    ga_solver = Ga(
+        msrcpsp_model,
+        encoding="priority_list_task",
+        objective_handling=ObjectiveHandling.AGGREGATE,
+        objectives=["makespan"],
+        objective_weights=[-1],
+        mutation=task_permutation_mutation,
+        max_evals=evals_per_ga_runs_perm,
+    )
+    tmp_sol = ga_solver.solve().get_best_solution()
+
+    # Fix the resulting permutation
+    msrcpsp_model.set_fixed_task_permutation(tmp_sol.priority_list_task)
+
+    # Run a GA for evals_per_ga_runs evals on permutation resource
+    ga_solver = Ga(
+        msrcpsp_model,
+        encoding="priority_worker_per_task_perm",
+        objective_handling=ObjectiveHandling.AGGREGATE,
+        objectives=["makespan"],
+        objective_weights=[-1],
+        mutation=resource_permutation_mutation,
+        max_evals=evals_per_ga_runs_resource_perm,
+    )
+    sol = ga_solver.solve().get_best_solution()
+
+    # Fix the resulting permutation
+    msrcpsp_model.set_fixed_priority_worker_per_task(sol.priority_worker_per_task)
+
+    assert msrcpsp_model.satisfy(sol)
+    msrcpsp_model.evaluate(tmp_sol)
+
+
+def test_alternating_ga_specific_mode_arity_single_solver(random_seed):
+    msrcpsp_model = create_toy_msrcpsp_variant()
+
+    total_evals = 1000
+
+    sub_evals = [50, 50, 50]
+
+    ga_solver = AlternatingGa(
+        msrcpsp_model,
+        encodings=[
+            "modes_arity_fix_from_0",
+            "priority_list_task",
+            "priority_worker_per_task_perm",
+        ],
+        objective_handling=ObjectiveHandling.AGGREGATE,
+        objectives=["makespan"],
+        objective_weights=[-1],
+        mutations=[
+            DeapMutation.MUT_UNIFORM_INT,
+            DeapMutation.MUT_SHUFFLE_INDEXES,
+            DeapMutation.MUT_SHUFFLE_INDEXES,
+        ],
+        crossovers=[
+            DeapCrossover.CX_ONE_POINT,
+            DeapCrossover.CX_PARTIALY_MATCHED,
+            DeapCrossover.CX_PARTIALY_MATCHED,
+        ],
+        max_evals=total_evals,
+        sub_evals=sub_evals,
+    )
+
+    tmp_sol = ga_solver.solve().get_best_solution()
+    assert msrcpsp_model.satisfy(tmp_sol)
+    assert msrcpsp_model.evaluate(tmp_sol) == {"makespan": 30}
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_lp.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_lp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
-
+import platform
 from typing import Dict, List, Set
 
+import pytest
+
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill import (
     Employee,
     MS_RCPSPModel,
     SkillDetail,
 )
 from discrete_optimization.rcpsp_multiskill.solvers.lp_model import (
     LP_Solver_MRSCPSP,
     MilpSolverName,
     ParametersMilp,
 )
 
+if platform.machine() == "arm64":
+    pytest.skip(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167",
+        allow_module_level=True,
+    )
+
 
 def test_lp():
     skills_set: Set[str] = {"S1", "S2", "S3"}
     resources_set: Set[str] = {"R1", "R2", "R3"}
     non_renewable_resources = set()
     resources_availability = {"R1": [2] * 100, "R2": [4] * 100, "R3": [3] * 100}
     employee: Dict[int, Employee] = {
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_lp_lns.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_lp_lns.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_ls.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_ls.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_model.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_rcpsp_based_solver.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_rcpsp_based_solver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 #  Copyright (c) 2022 AIRBUS and its affiliates.
 #  This source code is licensed under the MIT license found in the
 #  LICENSE file in the root directory of this source tree.
 
+import platform
 from typing import Dict, List, Set
 
+import pytest
+
 from discrete_optimization.generic_tools.lp_tools import MilpSolverName
 from discrete_optimization.rcpsp.rcpsp_solvers import LP_MRCPSP, solvers
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill import (
     Employee,
     MS_RCPSPModel_Variant,
     MS_RCPSPSolution,
     SkillDetail,
 )
 from discrete_optimization.rcpsp_multiskill.solvers.solver_rcpsp_based import (
     Solver_RCPSP_Based,
 )
 
+if platform.machine() == "arm64":
+    pytest.skip(
+        "Python-mip has issues with cbclib on macos arm64. "
+        "See https://github.com/coin-or/python-mip/issues/167",
+        allow_module_level=True,
+    )
+
 
 def create_toy_msrcpsp():
     skills_set: Set[str] = {"S1", "S2", "S3"}
     resources_set: Set[str] = {"R1", "R2", "R3"}
     non_renewable_resources = set()
     resources_availability = {"R1": [2] * 100, "R2": [4] * 100, "R3": [3] * 100}
     employee: Dict[int, Employee] = {
```

### Comparing `discrete_optimization-0.3.0/tests/rcpsp_multiskill/test_rcpsp_ms_to_rcpsp.py` & `discrete_optimization-0.3.1/tests/rcpsp_multiskill/test_rcpsp_ms_to_rcpsp.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 
 import random
 import sys
 
 import numpy as np
 import pytest
 
-from discrete_optimization.generic_tools.callbacks.early_stoppers import TimerStopper
 from discrete_optimization.generic_tools.cp_tools import CPSolverName, ParametersCP
 from discrete_optimization.rcpsp.solver.cp_solvers import CP_MRCPSP_MZN
-from discrete_optimization.rcpsp.solver.rcpsp_cp_lns_solver import (
-    LNS_CP_RCPSP_SOLVER,
-    OptionNeighbor,
-)
 from discrete_optimization.rcpsp_multiskill.multiskill_to_rcpsp import MultiSkillToRCPSP
 from discrete_optimization.rcpsp_multiskill.rcpsp_multiskill_parser import (
     get_data_available,
     parse_file,
 )
 
 
@@ -37,43 +32,14 @@
         check_resource_compliance=True,
         max_number_of_mode=100,
     )
     assert rcpsp_model.n_jobs == 202
 
 
 @pytest.mark.skipif(sys.platform.startswith("win"), reason="Much too long on windows")
-def test_solve_rcpsp_imopse1(random_seed):
-    files = [f for f in get_data_available() if "200_40_133_15.def" in f]
-    model_msrcpsp, new_name_to_original_task_id = parse_file(files[0], max_horizon=2000)
-    algorithm = MultiSkillToRCPSP(model_msrcpsp)
-    rcpsp_model = algorithm.construct_rcpsp_by_worker_type(
-        limit_number_of_mode_per_task=True,
-        check_resource_compliance=True,
-        max_number_of_mode=5,
-        one_worker_type_per_task=True,
-    )
-    params_cp = ParametersCP.default()
-    params_cp.time_limit = 50
-    params_cp.time_limit_iter0 = 100
-    params_cp.free_search = False
-    lns_solver = LNS_CP_RCPSP_SOLVER(
-        problem=rcpsp_model, option_neighbor=OptionNeighbor.MIX_FAST
-    )
-    result_storage = lns_solver.solve(
-        parameters_cp=params_cp,
-        nb_iteration_lns=5,
-        callbacks=[TimerStopper(total_seconds=100)],
-        nb_iteration_no_improvement=100,
-        skip_first_iteration=False,
-    )
-    best_solution = result_storage.get_best_solution()
-    assert rcpsp_model.satisfy(best_solution)
-
-
-@pytest.mark.skipif(sys.platform.startswith("win"), reason="Much too long on windows")
 def test_solve_rcpsp_imopse2(random_seed):
     files = [f for f in get_data_available() if "200_40_133_15.def" in f]
     model_msrcpsp, new_name_to_original_task_id = parse_file(files[0], max_horizon=2000)
     algorithm = MultiSkillToRCPSP(model_msrcpsp)
     rcpsp_model = algorithm.construct_rcpsp_by_worker_type(
         limit_number_of_mode_per_task=True,
         check_resource_compliance=True,
```

### Comparing `discrete_optimization-0.3.0/tests/test_import_all_submodules.py` & `discrete_optimization-0.3.1/tests/test_import_all_submodules.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_common_tools.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_common_tools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_ga.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_ga.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_lp_iterative.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_lp_iterative.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_ls.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_ls.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_model.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_model.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_mutation.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_mutation.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/tsp/test_tsp_ortools.py` & `discrete_optimization-0.3.1/tests/tsp/test_tsp_ortools.py`

 * *Files identical despite different names*

### Comparing `discrete_optimization-0.3.0/tests/vrp/test_vrp_solver.py` & `discrete_optimization-0.3.1/tests/vrp/test_vrp_solver.py`

 * *Files identical despite different names*

