# Comparing `tmp/movement_primitives-0.7.0.tar.gz` & `tmp/movement_primitives-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movement_primitives-0.7.0.tar", last modified: Tue Nov 28 13:49:07 2023, max compression
+gzip compressed data, was "movement_primitives-0.7.1.tar", last modified: Mon May 27 10:09:25 2024, max compression
```

## Comparing `movement_primitives-0.7.0.tar` & `movement_primitives-0.7.1.tar`

### file list

```diff
@@ -1,149 +1,49 @@
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.292380 movement_primitives-0.7.0/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      481 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/.coveragerc
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.248381 movement_primitives-0.7.0/.github/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/.github/workflows/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1101 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/.github/workflows/python-package.yml
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      212 2023-02-13 12:45:49.000000 movement_primitives-0.7.0/.gitignore
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1608 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/LICENSE
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       64 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/MANIFEST.in
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17582 2023-11-28 13:49:07.292380 movement_primitives-0.7.0/PKG-INFO
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17171 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/README.md
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/benchmarks/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1058 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/benchmarks/benchmark_cartesian_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1138 2023-11-17 09:30:16.000000 movement_primitives-0.7.0/benchmarks/benchmark_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      743 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/benchmarks/benchmark_dmp_phase.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      881 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/benchmarks/benchmark_dual_dmp.py
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/doc/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      638 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/Makefile
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      804 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/make.bat
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/doc/source/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.256381 movement_primitives-0.7.0/doc/source/_static/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    10690 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/241-logo-bmwi-jpg.jpg
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    74283 2023-11-14 15:19:55.000000 movement_primitives-0.7.0/doc/source/_static/DFKI_Logo.jpg
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    79218 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/doc/source/_static/cart_dmp_ur5.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   243002 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/conditional_promps.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    99133 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/contextual_promps_kuka_panel_width_open3d.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   133381 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/doc/source/_static/contextual_promps_kuka_panel_width_open3d2.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    46635 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/coupled_dual_cart_dmps_gripper_open3d.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   131634 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/coupled_dual_cart_dmps_rh5_pybullet.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   420418 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dmp_potential_field.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   758089 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_matplotlib.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   131501 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_open3d.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1993579 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/doc/source/_static/dmp_ur5_minimum_jerk.gif
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   130337 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dmp_with_final_velocity.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1964555 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/doc/source/_static/dual_cart_dmp_rh5_with_panel.gif
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   505925 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dual_cart_dmps_rh5_open3d.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   178623 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/dual_cart_dmps_rh5_pybullet.png
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   122973 2023-02-13 12:45:44.000000 movement_primitives-0.7.0/doc/source/_static/promp_lasa.png
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.256381 movement_primitives-0.7.0/doc/source/_templates/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      611 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/source/_templates/class.rst
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3963 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/source/api.rst
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2958 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/source/conf.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17171 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/doc/source/index.md
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.256381 movement_primitives-0.7.0/docker/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      486 2023-02-13 12:45:41.000000 movement_primitives-0.7.0/docker/Dockerfile
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.260381 movement_primitives-0.7.0/examples/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/examples/data/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.248381 movement_primitives-0.7.0/examples/data/meshes/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.252381 movement_primitives-0.7.0/examples/data/meshes/ur5/
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.264381 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    28984 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/base.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    52584 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/forearm.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    33784 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/shoulder.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    58884 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/upperarm.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    35184 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/wrist1.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    35184 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/wrist2.stl
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    22384 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/collision/wrist3.stl
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.280381 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   156606 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/base.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1473169 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/forearm.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1011530 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/shoulder.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  2008753 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/upperarm.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   952454 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/wrist1.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   951267 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/wrist2.dae
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)   127695 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/meshes/ur5/visual/wrist3.dae
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.284381 movement_primitives-0.7.0/examples/data/urdf/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    10172 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/data/urdf/ur5.urdf
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.284381 movement_primitives-0.7.0/examples/external_dependencies/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5147 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/external_dependencies/plot_contextual_promp_distribution.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1253 2023-11-21 10:40:12.000000 movement_primitives-0.7.0/examples/external_dependencies/plot_imitate_panel_rh5.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1786 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/external_dependencies/plot_relative_trajectories_kuka.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3567 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/external_dependencies/sim_cartesian_dual_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3899 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/external_dependencies/sim_solar_panel.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6169 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/external_dependencies/sim_solar_panel_rh5v2.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5058 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_cartesian_dual_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5593 2023-11-21 12:24:01.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_contextual_dmp_distribution.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4221 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_contextual_promp_distribution.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6293 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_contextual_promp_distribution_screws.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4918 2023-11-21 13:28:57.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_dmp_to_state_variance.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1415 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_kuka_ik.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3546 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_sample_dmp_distribution_kuka.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2169 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_sample_promp_distribution_kuka.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9718 2023-11-21 16:55:25.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_solar_panel.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5588 2023-11-21 13:39:51.000000 movement_primitives-0.7.0/examples/external_dependencies/vis_solar_panel_from_exported_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4422 2023-11-14 13:54:21.000000 movement_primitives-0.7.0/examples/plot_cartesian_pose_coupling_dual_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1894 2023-11-14 13:15:29.000000 movement_primitives-0.7.0/examples/plot_conditional_promp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1923 2023-11-21 16:35:43.000000 movement_primitives-0.7.0/examples/plot_coupling_1d_to_1d.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2104 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_coupling_3d_to_3d.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      754 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_dmp_1d_frequencies.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3250 2023-07-18 08:57:47.000000 movement_primitives-0.7.0/examples/plot_dmp_potential_field.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2489 2023-11-23 18:14:43.000000 movement_primitives-0.7.0/examples/plot_dmp_scaling.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1681 2023-11-17 14:26:13.000000 movement_primitives-0.7.0/examples/plot_dmp_stepwise_execution.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1729 2023-11-21 15:49:43.000000 movement_primitives-0.7.0/examples/plot_dmp_with_final_velocity.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2987 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_kinematics.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      528 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/plot_minimum_jerk.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1291 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_obstacle_avoidance_2d.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1450 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_obstacle_avoidance_3d.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1581 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_promp_lasa.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2270 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_promp_velocities.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1220 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/plot_state_following_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1711 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/sim_cartesian_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2071 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/sim_cartesian_orientation_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1967 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/examples/sim_spring_damper.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2647 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/examples/vis_cartesian_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      908 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/manifest.xml
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.288380 movement_primitives-0.7.0/movement_primitives/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      118 2023-11-23 17:53:24.000000 movement_primitives-0.7.0/movement_primitives/__init__.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       22 2023-11-28 13:45:46.000000 movement_primitives-0.7.0/movement_primitives/_version.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4508 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/base.py
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.288380 movement_primitives-0.7.0/movement_primitives/data/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      284 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/data/__init__.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     4109 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/data/_lasa.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2687 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/data/_minimum_jerk.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2553 2023-07-18 08:57:47.000000 movement_primitives-0.7.0/movement_primitives/data/_toy_1d.py
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.288380 movement_primitives-0.7.0/movement_primitives/dmp/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2175 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/__init__.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1800 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_base.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1983 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/dmp/_canonical_system.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    22599 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_cartesian_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    21610 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_coupling_terms.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    27240 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    13772 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_dmp_with_final_velocity.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    14559 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_dual_cartesian_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3824 2023-11-23 17:44:49.000000 movement_primitives-0.7.0/movement_primitives/dmp/_forcing_term.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     7484 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp/_state_following_dmp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)  1039382 2023-11-23 18:03:23.000000 movement_primitives-0.7.0/movement_primitives/dmp_fast.c
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    28450 2023-11-23 17:53:29.000000 movement_primitives-0.7.0/movement_primitives/dmp_fast.pyx
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3578 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/dmp_potential_field.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5295 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/dmp_to_state_space_distribution.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     3726 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/io.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    16900 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/kinematics.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1771 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/minimum_jerk_trajectory.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     6454 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/plot.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    20617 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/promp.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     9103 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/spring_damper.py
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.292380 movement_primitives-0.7.0/movement_primitives/testing/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       56 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/testing/__init__.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    30096 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/movement_primitives/testing/simulation.py
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     2266 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/movement_primitives/visualization.py
-drwxr-xr-x   0 afabisch (1545608986) domänen-benutzer (1545600513)        0 2023-11-28 13:49:07.288380 movement_primitives-0.7.0/movement_primitives.egg-info/
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)    17582 2023-11-28 13:49:07.000000 movement_primitives-0.7.0/movement_primitives.egg-info/PKG-INFO
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     5036 2023-11-28 13:49:07.000000 movement_primitives-0.7.0/movement_primitives.egg-info/SOURCES.txt
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)        1 2023-11-28 13:49:07.000000 movement_primitives-0.7.0/movement_primitives.egg-info/dependency_links.txt
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)        1 2023-02-13 12:45:47.000000 movement_primitives-0.7.0/movement_primitives.egg-info/not-zip-safe
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      169 2023-11-28 13:49:07.000000 movement_primitives-0.7.0/movement_primitives.egg-info/requires.txt
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       20 2023-11-28 13:49:07.000000 movement_primitives-0.7.0/movement_primitives.egg-info/top_level.txt
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      109 2023-07-18 08:55:55.000000 movement_primitives-0.7.0/pyproject.toml
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)       81 2023-02-13 12:45:45.000000 movement_primitives-0.7.0/requirements.txt
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)      240 2023-11-28 13:49:07.292380 movement_primitives-0.7.0/setup.cfg
--rw-r--r--   0 afabisch (1545608986) domänen-benutzer (1545600513)     1840 2023-11-28 13:45:59.000000 movement_primitives-0.7.0/setup.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.410456 movement_primitives-0.7.1/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1598 2024-05-08 14:12:51.000000 movement_primitives-0.7.1/LICENSE
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       64 2022-04-26 15:19:29.000000 movement_primitives-0.7.1/MANIFEST.in
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21036 2024-05-27 10:09:25.410456 movement_primitives-0.7.1/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    20625 2024-05-27 10:06:28.000000 movement_primitives-0.7.1/README.md
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.402456 movement_primitives-0.7.1/movement_primitives/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      118 2022-01-19 15:16:06.000000 movement_primitives-0.7.1/movement_primitives/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       22 2024-05-27 09:38:16.000000 movement_primitives-0.7.1/movement_primitives/_version.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4508 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/base.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.406456 movement_primitives-0.7.1/movement_primitives/data/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      284 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/data/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     4083 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/data/_lasa.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2687 2022-02-22 15:53:25.000000 movement_primitives-0.7.1/movement_primitives/data/_minimum_jerk.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2553 2023-11-17 21:14:00.000000 movement_primitives-0.7.1/movement_primitives/data/_toy_1d.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.406456 movement_primitives-0.7.1/movement_primitives/dmp/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2175 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/dmp/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1800 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/dmp/_base.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1983 2022-01-19 15:16:06.000000 movement_primitives-0.7.1/movement_primitives/dmp/_canonical_system.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    22803 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/dmp/_cartesian_dmp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21610 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/dmp/_coupling_terms.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    27629 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/dmp/_dmp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    14184 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/dmp/_dmp_with_final_velocity.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    14763 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/dmp/_dual_cartesian_dmp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3824 2023-11-24 22:09:14.000000 movement_primitives-0.7.1/movement_primitives/dmp/_forcing_term.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     7484 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/dmp/_state_following_dmp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)  1039039 2024-05-27 10:00:14.000000 movement_primitives-0.7.1/movement_primitives/dmp_fast.c
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    28450 2023-11-24 22:09:14.000000 movement_primitives-0.7.1/movement_primitives/dmp_fast.pyx
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3578 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/dmp_potential_field.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     5295 2022-02-22 15:53:25.000000 movement_primitives-0.7.1/movement_primitives/dmp_to_state_space_distribution.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     3726 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/io.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    16900 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/kinematics.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1771 2022-02-22 15:53:25.000000 movement_primitives-0.7.1/movement_primitives/minimum_jerk_trajectory.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     6454 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/plot.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    21188 2024-05-05 09:37:08.000000 movement_primitives-0.7.1/movement_primitives/promp.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     9103 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/spring_damper.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.410456 movement_primitives-0.7.1/movement_primitives/testing/
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       56 2022-01-19 15:16:06.000000 movement_primitives-0.7.1/movement_primitives/testing/__init__.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)    30096 2022-02-08 15:54:28.000000 movement_primitives-0.7.1/movement_primitives/testing/simulation.py
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     2266 2023-11-29 19:56:13.000000 movement_primitives-0.7.1/movement_primitives/visualization.py
+drwxrwxr-x   0 afabisch  (1000) afabisch  (1000)        0 2024-05-27 10:09:25.406456 movement_primitives-0.7.1/movement_primitives.egg-info/
+-rw-r--r--   0 afabisch  (1000) afabisch  (1000)    21036 2024-05-27 10:09:24.000000 movement_primitives-0.7.1/movement_primitives.egg-info/PKG-INFO
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1461 2024-05-27 10:09:25.000000 movement_primitives-0.7.1/movement_primitives.egg-info/SOURCES.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2024-05-27 10:09:24.000000 movement_primitives-0.7.1/movement_primitives.egg-info/dependency_links.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)        1 2021-01-11 16:54:02.000000 movement_primitives-0.7.1/movement_primitives.egg-info/not-zip-safe
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      173 2024-05-27 10:09:24.000000 movement_primitives-0.7.1/movement_primitives.egg-info/requires.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)       24 2024-05-27 10:09:24.000000 movement_primitives-0.7.1/movement_primitives.egg-info/top_level.txt
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      109 2022-01-19 15:16:06.000000 movement_primitives-0.7.1/pyproject.toml
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)      259 2024-05-27 10:09:25.410456 movement_primitives-0.7.1/setup.cfg
+-rw-rw-r--   0 afabisch  (1000) afabisch  (1000)     1844 2024-05-08 14:12:51.000000 movement_primitives-0.7.1/setup.py
```

### Comparing `movement_primitives-0.7.0/LICENSE` & `movement_primitives-0.7.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020-2021 Alexander Fabisch (DFKI GmbH, Robotics Innovation Center),
+Copyright Alexander Fabisch (DFKI GmbH, Robotics Innovation Center),
 Jannik Klemm (University of Bremen, Robotics Research Group),
 and movement_primitives contributors.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
```

### Comparing `movement_primitives-0.7.0/PKG-INFO` & `movement_primitives-0.7.1/movement_primitives.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: movement_primitives
-Version: 0.7.0
+Name: movement-primitives
+Version: 0.7.1
 Summary: Movement primitives
 Home-page: https://github.com/dfki-ric/movement_primitives
 Author: Alexander Fabisch
 Author-email: alexander.fabisch@dfki.de
 License: BSD-3-clause
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -18,34 +18,67 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6491361.svg)](https://doi.org/10.5281/zenodo.6491361)
 
 # Movement Primitives
 
 > Dynamical movement primitives (DMPs), probabilistic movement primitives
 > (ProMPs), and spatially coupled bimanual DMPs for imitation learning.
 
-Movement primitives are a common group of policy representations in robotics.
-There are many types and variations. This repository focuses mainly on
-imitation learning, generalization, and adaptation of movement primitives for
-Cartesian motions of robots. It provides implementations in Python and Cython
-and can be installed directly from
+Movement primitives are a common representation of movements in robotics for
+imitation learning, reinforcement learning, and black-box optimization of
+behaviors. There are many types and variations. The Python library
+movement_primitives focuses on imitation learning, generalization, and
+adaptation of movement primitives in Cartesian space. It implements dynamical
+movement primitives, probabilistic movement primitives, as well as Cartesian
+and dual Cartesian movement primitives with coupling terms to constrain
+relative movements in bimanual manipulation. They are implemented in Cython to
+speed up online execution and batch processing in an offline setting. In
+addition, the library provides tools for data analysis and movement evaluation.
+It can be installed directly from
 [PyPI](https://pypi.org/project/movement-primitives/).
 
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/summary.png" width="100%" />
+
 ## Content
 
+* [Statement of Need](#statement-of-need)
 * [Features](#features)
 * [API Documentation](#api-documentation)
 * [Install Library](#install-library)
 * [Examples](#examples)
 * [Build API Documentation](#build-api-documentation)
 * [Test](#test)
 * [Contributing](#contributing)
 * [Non-public Extensions](#non-public-extensions)
 * [Related Publications](#related-publications)
 * [Funding](#funding)
 
+## Statement of Need
+
+Movement primitives are a common group of policy representations in robotics.
+They are able to represent complex movement patterns, allow temporal and
+spatial modification, offer stability guarantees, and are suitable for
+imitation learning without complicated hyperparameter tuning, which are
+advantages over general function approximators like neural networks. Movement
+primitives are white-box models for movement generation and allow to control
+several aspects of the movement. There are types of dynamical movement
+primitives that allow to directly control the goal in state space, the final
+velocity, or the relative pose of two robotic end-effectors. Probabilistic
+movement primitives capture distributions of movements adequately and allow
+conditioning in state space and blending of multiple movements. The main
+disadvantage of movement primitives in comparison to general function
+approximators is that they are limited in their capacity to represent behavior
+that takes into account complex sensor data during execution. Nevertheless,
+various types of movement primitives have proven to be a reliable and effective
+tool in robot learning. A reliable tool deserves a similarly reliable open
+source implementation. However, there are only a few actively maintained,
+documented, and easy to use implementations. One of these is the library
+*movement_primitives*. It combines several types of dynamical movement
+primitives and probabilistic movement primitives in a single library with
+a focus on Cartesian and bimanual movements.
+
 ## Features
 
 * Dynamical Movement Primitives (DMPs) for
     * positions (with fast Runge-Kutta integration)
     * Cartesian position and orientation (with fast Cython implementation)
     * Dual Cartesian position and orientation (with fast Cython implementation)
 * Coupling terms for synchronization of position and/or orientation of dual Cartesian DMPs
@@ -65,62 +98,76 @@
 ## Install Library
 
 This library requires Python 3.6 or later and pip is recommended for the
 installation. In the following instructions, we assume that the command
 `python` refers to Python 3. If you use the system's Python version, you
 might have to add the flag `--user` to any installation command.
 
-I recommend to install the library via pip:
+### PyPI (Recommended)
+
+I recommend to install the library via pip from the Python package index
+(PyPI):
 
 ```bash
 python -m pip install movement_primitives[all]
 ```
 
-or clone the git repository and install it in editable mode:
+If you don't want to have all dependencies installed, just omit `[all]`.
+
+This will install the latest release. If you want to install the latest
+development version, you have to install from git.
+
+### Git + Editable Mode
+
+Editable mode means that you don't have to install the library after editing
+the source code. Changes will be directly available in the installed library
+since pip creates a symlink.
+
+You can clone the git repository and install it in editable mode with pip:
 
 ```bash
+git clone https://github.com/dfki-ric/movement_primitives.git
 python -m pip install -e .[all]
 ```
 
 If you don't want to have all dependencies installed, just omit `[all]`.
-Alternatively, you can install dependencies with
+
+### Git
+
+Alternatively, you can install the library and its dependencies without pip
+from the git repository:
 
 ```bash
-python -m pip install -r requirements.txt
+git clone https://github.com/dfki-ric/movement_primitives.git
+python setup.py install
 ```
 
+### Build Cython Extension
+
 You could also just build the Cython extension with
 
 ```bash
 python setup.py build_ext --inplace
 ```
 
-or install the library with
+### Dependencies
+
+An alternative way to install dependencies is the requirements.txt file in the
+main folder of the git repository:
 
 ```bash
-python setup.py install
+python -m pip install -r requirements.txt
 ```
 
 ## Examples
 
 You will find a lot of examples in the subfolder
 [`examples/`](https://github.com/dfki-ric/movement_primitives/tree/main/examples).
 Here are just some highlights to showcase the library.
 
-### Conditional ProMPs
-
-<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
-
-Probabilistic Movement Primitives (ProMPs) define distributions over
-trajectories that can be conditioned on viapoints. In this example, we
-plot the resulting posterior distribution after conditioning on varying
-start positions.
-
-[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
-
 ### Potential Field of 2D DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_potential_field.png" width="800px" />
 
 A Dynamical Movement Primitive defines a potential field that superimposes
 several components: transformation system (goal-directed movement), forcing
 term (learned shape), and coupling terms (e.g., obstacle avoidance).
@@ -144,52 +191,66 @@
 The LASA Handwriting dataset learned with ProMPs. The dataset consists of
 2D handwriting motions. The first and third column of the plot represent
 demonstrations and the second and fourth column show the imitated ProMPs
 with 1-sigma interval.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_promp_lasa.py)
 
+### Conditional ProMPs
+
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
+
+Probabilistic Movement Primitives (ProMPs) define distributions over
+trajectories that can be conditioned on viapoints. In this example, we
+plot the resulting posterior distribution after conditioning on varying
+start positions.
+
+[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
+
 ### Cartesian DMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/cart_dmp_ur5.png" width="100%" />
 
 A trajectory is created manually, imitated with a Cartesian DMP, converted
 to a joint trajectory by inverse kinematics, and executed with a UR5.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/vis_cartesian_dmp.py)
 
 ### Contextual ProMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d2.png" width="40%" />
 
-We use a dataset of [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
-with 10 demonstrations per 3 different panel widths that were obtained through
-kinesthetic teaching. The panel width is considered to be the context over
-which we generalize with contextual ProMPs. Each color in the above
-visualizations corresponds to a ProMP for a different context.
+We use a dataset of [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779),
+in which a dual-arm robot rotates panels of varying widths. 10 demonstrations
+were recorded for 3 different panel widths through kinesthetic teaching.
+The panel width is the context over which we generalize with contextual ProMPs.
+We learn a joint distribution of contexts and ProMP weights, and then condition
+the distribution on the contexts to obtain a ProMP adapted to the context. Each
+color in the above visualizations corresponds to a ProMP for a different
+context.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_contextual_promp_distribution.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm Kuka system from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ### Dual Cartesian DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_open3d.png" width="50%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_pybullet.png" width="50%" />
 
-We offer specific dual Cartesian DMPs to control dual-arm robotic systems like
-humanoid robots.
+This library implements specific dual Cartesian DMPs to control dual-arm
+robotic systems like humanoid robots.
 
 Scripts: [Open3D](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_solar_panel.py), [PyBullet](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/sim_solar_panel.py)
 
 **Dependencies that are not publicly available:**
 
 * MoCap library
 * URDF of [DFKI RIC's RH5 robot](https://www.youtube.com/watch?v=jjGQNstmLvY):
@@ -224,26 +285,31 @@
 
 ### Propagation of DMP Distribution to State Space
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_matplotlib.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_open3d.png" width="40%" />
 
 If we have a distribution over DMP parameters, we can propagate them to state
 space through an unscented transform.
+On the left we see the original demonstration of a dual-arm movement in state
+space (two 3D positions and two quaternions) and the distribution of several
+DMP weight vectors projected to the state space.
+On the right side we see several dual-arm trajectories sampled from the
+distribution in state space.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_dmp_to_state_variance.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm
   [Kuka system](https://robotik.dfki-bremen.de/en/research/robot-systems/imrk/)
   from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ## Build API Documentation
 
 You can build an API documentation with sphinx.
@@ -266,17 +332,18 @@
 To run the tests some python libraries are required:
 
 ```bash
 python -m pip install -e .[test]
 ```
 
 The tests are located in the folder `test/` and can be executed with:
-`python -m nose test`
+`python -m pytest`
 
-This command searches for all files with `test` and executes the functions with `test_*`.
+This command searches for all files with `test` and executes the functions
+with `test_*`. You will find a test coverage report at `htmlcov/index.html`.
 
 ## Contributing
 
 You can report bugs in the [issue tracker](https://github.com/dfki-ric/movement_primitives/issues).
 If you have questions about the software, please use the [discussions
 section](https://github.com/dfki-ric/movement_primitives/discussions).
 To add new features, documentation, or fix bugs you can open a pull request
```

### Comparing `movement_primitives-0.7.0/README.md` & `movement_primitives-0.7.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,34 +3,67 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6491361.svg)](https://doi.org/10.5281/zenodo.6491361)
 
 # Movement Primitives
 
 > Dynamical movement primitives (DMPs), probabilistic movement primitives
 > (ProMPs), and spatially coupled bimanual DMPs for imitation learning.
 
-Movement primitives are a common group of policy representations in robotics.
-There are many types and variations. This repository focuses mainly on
-imitation learning, generalization, and adaptation of movement primitives for
-Cartesian motions of robots. It provides implementations in Python and Cython
-and can be installed directly from
+Movement primitives are a common representation of movements in robotics for
+imitation learning, reinforcement learning, and black-box optimization of
+behaviors. There are many types and variations. The Python library
+movement_primitives focuses on imitation learning, generalization, and
+adaptation of movement primitives in Cartesian space. It implements dynamical
+movement primitives, probabilistic movement primitives, as well as Cartesian
+and dual Cartesian movement primitives with coupling terms to constrain
+relative movements in bimanual manipulation. They are implemented in Cython to
+speed up online execution and batch processing in an offline setting. In
+addition, the library provides tools for data analysis and movement evaluation.
+It can be installed directly from
 [PyPI](https://pypi.org/project/movement-primitives/).
 
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/summary.png" width="100%" />
+
 ## Content
 
+* [Statement of Need](#statement-of-need)
 * [Features](#features)
 * [API Documentation](#api-documentation)
 * [Install Library](#install-library)
 * [Examples](#examples)
 * [Build API Documentation](#build-api-documentation)
 * [Test](#test)
 * [Contributing](#contributing)
 * [Non-public Extensions](#non-public-extensions)
 * [Related Publications](#related-publications)
 * [Funding](#funding)
 
+## Statement of Need
+
+Movement primitives are a common group of policy representations in robotics.
+They are able to represent complex movement patterns, allow temporal and
+spatial modification, offer stability guarantees, and are suitable for
+imitation learning without complicated hyperparameter tuning, which are
+advantages over general function approximators like neural networks. Movement
+primitives are white-box models for movement generation and allow to control
+several aspects of the movement. There are types of dynamical movement
+primitives that allow to directly control the goal in state space, the final
+velocity, or the relative pose of two robotic end-effectors. Probabilistic
+movement primitives capture distributions of movements adequately and allow
+conditioning in state space and blending of multiple movements. The main
+disadvantage of movement primitives in comparison to general function
+approximators is that they are limited in their capacity to represent behavior
+that takes into account complex sensor data during execution. Nevertheless,
+various types of movement primitives have proven to be a reliable and effective
+tool in robot learning. A reliable tool deserves a similarly reliable open
+source implementation. However, there are only a few actively maintained,
+documented, and easy to use implementations. One of these is the library
+*movement_primitives*. It combines several types of dynamical movement
+primitives and probabilistic movement primitives in a single library with
+a focus on Cartesian and bimanual movements.
+
 ## Features
 
 * Dynamical Movement Primitives (DMPs) for
     * positions (with fast Runge-Kutta integration)
     * Cartesian position and orientation (with fast Cython implementation)
     * Dual Cartesian position and orientation (with fast Cython implementation)
 * Coupling terms for synchronization of position and/or orientation of dual Cartesian DMPs
@@ -50,62 +83,76 @@
 ## Install Library
 
 This library requires Python 3.6 or later and pip is recommended for the
 installation. In the following instructions, we assume that the command
 `python` refers to Python 3. If you use the system's Python version, you
 might have to add the flag `--user` to any installation command.
 
-I recommend to install the library via pip:
+### PyPI (Recommended)
+
+I recommend to install the library via pip from the Python package index
+(PyPI):
 
 ```bash
 python -m pip install movement_primitives[all]
 ```
 
-or clone the git repository and install it in editable mode:
+If you don't want to have all dependencies installed, just omit `[all]`.
+
+This will install the latest release. If you want to install the latest
+development version, you have to install from git.
+
+### Git + Editable Mode
+
+Editable mode means that you don't have to install the library after editing
+the source code. Changes will be directly available in the installed library
+since pip creates a symlink.
+
+You can clone the git repository and install it in editable mode with pip:
 
 ```bash
+git clone https://github.com/dfki-ric/movement_primitives.git
 python -m pip install -e .[all]
 ```
 
 If you don't want to have all dependencies installed, just omit `[all]`.
-Alternatively, you can install dependencies with
+
+### Git
+
+Alternatively, you can install the library and its dependencies without pip
+from the git repository:
 
 ```bash
-python -m pip install -r requirements.txt
+git clone https://github.com/dfki-ric/movement_primitives.git
+python setup.py install
 ```
 
+### Build Cython Extension
+
 You could also just build the Cython extension with
 
 ```bash
 python setup.py build_ext --inplace
 ```
 
-or install the library with
+### Dependencies
+
+An alternative way to install dependencies is the requirements.txt file in the
+main folder of the git repository:
 
 ```bash
-python setup.py install
+python -m pip install -r requirements.txt
 ```
 
 ## Examples
 
 You will find a lot of examples in the subfolder
 [`examples/`](https://github.com/dfki-ric/movement_primitives/tree/main/examples).
 Here are just some highlights to showcase the library.
 
-### Conditional ProMPs
-
-<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
-
-Probabilistic Movement Primitives (ProMPs) define distributions over
-trajectories that can be conditioned on viapoints. In this example, we
-plot the resulting posterior distribution after conditioning on varying
-start positions.
-
-[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
-
 ### Potential Field of 2D DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_potential_field.png" width="800px" />
 
 A Dynamical Movement Primitive defines a potential field that superimposes
 several components: transformation system (goal-directed movement), forcing
 term (learned shape), and coupling terms (e.g., obstacle avoidance).
@@ -129,52 +176,66 @@
 The LASA Handwriting dataset learned with ProMPs. The dataset consists of
 2D handwriting motions. The first and third column of the plot represent
 demonstrations and the second and fourth column show the imitated ProMPs
 with 1-sigma interval.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_promp_lasa.py)
 
+### Conditional ProMPs
+
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
+
+Probabilistic Movement Primitives (ProMPs) define distributions over
+trajectories that can be conditioned on viapoints. In this example, we
+plot the resulting posterior distribution after conditioning on varying
+start positions.
+
+[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
+
 ### Cartesian DMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/cart_dmp_ur5.png" width="100%" />
 
 A trajectory is created manually, imitated with a Cartesian DMP, converted
 to a joint trajectory by inverse kinematics, and executed with a UR5.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/vis_cartesian_dmp.py)
 
 ### Contextual ProMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d2.png" width="40%" />
 
-We use a dataset of [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
-with 10 demonstrations per 3 different panel widths that were obtained through
-kinesthetic teaching. The panel width is considered to be the context over
-which we generalize with contextual ProMPs. Each color in the above
-visualizations corresponds to a ProMP for a different context.
+We use a dataset of [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779),
+in which a dual-arm robot rotates panels of varying widths. 10 demonstrations
+were recorded for 3 different panel widths through kinesthetic teaching.
+The panel width is the context over which we generalize with contextual ProMPs.
+We learn a joint distribution of contexts and ProMP weights, and then condition
+the distribution on the contexts to obtain a ProMP adapted to the context. Each
+color in the above visualizations corresponds to a ProMP for a different
+context.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_contextual_promp_distribution.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm Kuka system from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ### Dual Cartesian DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_open3d.png" width="50%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_pybullet.png" width="50%" />
 
-We offer specific dual Cartesian DMPs to control dual-arm robotic systems like
-humanoid robots.
+This library implements specific dual Cartesian DMPs to control dual-arm
+robotic systems like humanoid robots.
 
 Scripts: [Open3D](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_solar_panel.py), [PyBullet](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/sim_solar_panel.py)
 
 **Dependencies that are not publicly available:**
 
 * MoCap library
 * URDF of [DFKI RIC's RH5 robot](https://www.youtube.com/watch?v=jjGQNstmLvY):
@@ -209,26 +270,31 @@
 
 ### Propagation of DMP Distribution to State Space
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_matplotlib.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_open3d.png" width="40%" />
 
 If we have a distribution over DMP parameters, we can propagate them to state
 space through an unscented transform.
+On the left we see the original demonstration of a dual-arm movement in state
+space (two 3D positions and two quaternions) and the distribution of several
+DMP weight vectors projected to the state space.
+On the right side we see several dual-arm trajectories sampled from the
+distribution in state space.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_dmp_to_state_variance.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm
   [Kuka system](https://robotik.dfki-bremen.de/en/research/robot-systems/imrk/)
   from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ## Build API Documentation
 
 You can build an API documentation with sphinx.
@@ -251,17 +317,18 @@
 To run the tests some python libraries are required:
 
 ```bash
 python -m pip install -e .[test]
 ```
 
 The tests are located in the folder `test/` and can be executed with:
-`python -m nose test`
+`python -m pytest`
 
-This command searches for all files with `test` and executes the functions with `test_*`.
+This command searches for all files with `test` and executes the functions
+with `test_*`. You will find a test coverage report at `htmlcov/index.html`.
 
 ## Contributing
 
 You can report bugs in the [issue tracker](https://github.com/dfki-ric/movement_primitives/issues).
 If you have questions about the software, please use the [discussions
 section](https://github.com/dfki-ric/movement_primitives/discussions).
 To add new features, documentation, or fix bugs you can open a pull request
```

### Comparing `movement_primitives-0.7.0/doc/source/index.md` & `movement_primitives-0.7.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,84 @@
+Metadata-Version: 2.1
+Name: movement_primitives
+Version: 0.7.1
+Summary: Movement primitives
+Home-page: https://github.com/dfki-ric/movement_primitives
+Author: Alexander Fabisch
+Author-email: alexander.fabisch@dfki.de
+License: BSD-3-clause
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: doc
+Provides-Extra: test
+License-File: LICENSE
+
 ![CI](https://github.com/dfki-ric/movement_primitives/actions/workflows/python-package.yml/badge.svg)
 [![codecov](https://codecov.io/gh/dfki-ric/movement_primitives/branch/main/graph/badge.svg?token=EFHUC81DBL)](https://codecov.io/gh/dfki-ric/movement_primitives)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6491361.svg)](https://doi.org/10.5281/zenodo.6491361)
 
 # Movement Primitives
 
 > Dynamical movement primitives (DMPs), probabilistic movement primitives
 > (ProMPs), and spatially coupled bimanual DMPs for imitation learning.
 
-Movement primitives are a common group of policy representations in robotics.
-There are many types and variations. This repository focuses mainly on
-imitation learning, generalization, and adaptation of movement primitives for
-Cartesian motions of robots. It provides implementations in Python and Cython
-and can be installed directly from
+Movement primitives are a common representation of movements in robotics for
+imitation learning, reinforcement learning, and black-box optimization of
+behaviors. There are many types and variations. The Python library
+movement_primitives focuses on imitation learning, generalization, and
+adaptation of movement primitives in Cartesian space. It implements dynamical
+movement primitives, probabilistic movement primitives, as well as Cartesian
+and dual Cartesian movement primitives with coupling terms to constrain
+relative movements in bimanual manipulation. They are implemented in Cython to
+speed up online execution and batch processing in an offline setting. In
+addition, the library provides tools for data analysis and movement evaluation.
+It can be installed directly from
 [PyPI](https://pypi.org/project/movement-primitives/).
 
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/summary.png" width="100%" />
+
 ## Content
 
+* [Statement of Need](#statement-of-need)
 * [Features](#features)
 * [API Documentation](#api-documentation)
 * [Install Library](#install-library)
 * [Examples](#examples)
 * [Build API Documentation](#build-api-documentation)
 * [Test](#test)
 * [Contributing](#contributing)
 * [Non-public Extensions](#non-public-extensions)
 * [Related Publications](#related-publications)
 * [Funding](#funding)
 
+## Statement of Need
+
+Movement primitives are a common group of policy representations in robotics.
+They are able to represent complex movement patterns, allow temporal and
+spatial modification, offer stability guarantees, and are suitable for
+imitation learning without complicated hyperparameter tuning, which are
+advantages over general function approximators like neural networks. Movement
+primitives are white-box models for movement generation and allow to control
+several aspects of the movement. There are types of dynamical movement
+primitives that allow to directly control the goal in state space, the final
+velocity, or the relative pose of two robotic end-effectors. Probabilistic
+movement primitives capture distributions of movements adequately and allow
+conditioning in state space and blending of multiple movements. The main
+disadvantage of movement primitives in comparison to general function
+approximators is that they are limited in their capacity to represent behavior
+that takes into account complex sensor data during execution. Nevertheless,
+various types of movement primitives have proven to be a reliable and effective
+tool in robot learning. A reliable tool deserves a similarly reliable open
+source implementation. However, there are only a few actively maintained,
+documented, and easy to use implementations. One of these is the library
+*movement_primitives*. It combines several types of dynamical movement
+primitives and probabilistic movement primitives in a single library with
+a focus on Cartesian and bimanual movements.
+
 ## Features
 
 * Dynamical Movement Primitives (DMPs) for
     * positions (with fast Runge-Kutta integration)
     * Cartesian position and orientation (with fast Cython implementation)
     * Dual Cartesian position and orientation (with fast Cython implementation)
 * Coupling terms for synchronization of position and/or orientation of dual Cartesian DMPs
@@ -50,62 +98,76 @@
 ## Install Library
 
 This library requires Python 3.6 or later and pip is recommended for the
 installation. In the following instructions, we assume that the command
 `python` refers to Python 3. If you use the system's Python version, you
 might have to add the flag `--user` to any installation command.
 
-I recommend to install the library via pip:
+### PyPI (Recommended)
+
+I recommend to install the library via pip from the Python package index
+(PyPI):
 
 ```bash
 python -m pip install movement_primitives[all]
 ```
 
-or clone the git repository and install it in editable mode:
+If you don't want to have all dependencies installed, just omit `[all]`.
+
+This will install the latest release. If you want to install the latest
+development version, you have to install from git.
+
+### Git + Editable Mode
+
+Editable mode means that you don't have to install the library after editing
+the source code. Changes will be directly available in the installed library
+since pip creates a symlink.
+
+You can clone the git repository and install it in editable mode with pip:
 
 ```bash
+git clone https://github.com/dfki-ric/movement_primitives.git
 python -m pip install -e .[all]
 ```
 
 If you don't want to have all dependencies installed, just omit `[all]`.
-Alternatively, you can install dependencies with
+
+### Git
+
+Alternatively, you can install the library and its dependencies without pip
+from the git repository:
 
 ```bash
-python -m pip install -r requirements.txt
+git clone https://github.com/dfki-ric/movement_primitives.git
+python setup.py install
 ```
 
+### Build Cython Extension
+
 You could also just build the Cython extension with
 
 ```bash
 python setup.py build_ext --inplace
 ```
 
-or install the library with
+### Dependencies
+
+An alternative way to install dependencies is the requirements.txt file in the
+main folder of the git repository:
 
 ```bash
-python setup.py install
+python -m pip install -r requirements.txt
 ```
 
 ## Examples
 
 You will find a lot of examples in the subfolder
 [`examples/`](https://github.com/dfki-ric/movement_primitives/tree/main/examples).
 Here are just some highlights to showcase the library.
 
-### Conditional ProMPs
-
-<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
-
-Probabilistic Movement Primitives (ProMPs) define distributions over
-trajectories that can be conditioned on viapoints. In this example, we
-plot the resulting posterior distribution after conditioning on varying
-start positions.
-
-[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
-
 ### Potential Field of 2D DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_potential_field.png" width="800px" />
 
 A Dynamical Movement Primitive defines a potential field that superimposes
 several components: transformation system (goal-directed movement), forcing
 term (learned shape), and coupling terms (e.g., obstacle avoidance).
@@ -129,52 +191,66 @@
 The LASA Handwriting dataset learned with ProMPs. The dataset consists of
 2D handwriting motions. The first and third column of the plot represent
 demonstrations and the second and fourth column show the imitated ProMPs
 with 1-sigma interval.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_promp_lasa.py)
 
+### Conditional ProMPs
+
+<img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/conditional_promps.png" width="800px" />
+
+Probabilistic Movement Primitives (ProMPs) define distributions over
+trajectories that can be conditioned on viapoints. In this example, we
+plot the resulting posterior distribution after conditioning on varying
+start positions.
+
+[Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/plot_conditional_promp.py)
+
 ### Cartesian DMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/cart_dmp_ur5.png" width="100%" />
 
 A trajectory is created manually, imitated with a Cartesian DMP, converted
 to a joint trajectory by inverse kinematics, and executed with a UR5.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/vis_cartesian_dmp.py)
 
 ### Contextual ProMPs
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/contextual_promps_kuka_panel_width_open3d2.png" width="40%" />
 
-We use a dataset of [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
-with 10 demonstrations per 3 different panel widths that were obtained through
-kinesthetic teaching. The panel width is considered to be the context over
-which we generalize with contextual ProMPs. Each color in the above
-visualizations corresponds to a ProMP for a different context.
+We use a dataset of [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779),
+in which a dual-arm robot rotates panels of varying widths. 10 demonstrations
+were recorded for 3 different panel widths through kinesthetic teaching.
+The panel width is the context over which we generalize with contextual ProMPs.
+We learn a joint distribution of contexts and ProMP weights, and then condition
+the distribution on the contexts to obtain a ProMP adapted to the context. Each
+color in the above visualizations corresponds to a ProMP for a different
+context.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_contextual_promp_distribution.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm Kuka system from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ### Dual Cartesian DMP
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_open3d.png" width="50%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dual_cart_dmps_rh5_pybullet.png" width="50%" />
 
-We offer specific dual Cartesian DMPs to control dual-arm robotic systems like
-humanoid robots.
+This library implements specific dual Cartesian DMPs to control dual-arm
+robotic systems like humanoid robots.
 
 Scripts: [Open3D](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_solar_panel.py), [PyBullet](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/sim_solar_panel.py)
 
 **Dependencies that are not publicly available:**
 
 * MoCap library
 * URDF of [DFKI RIC's RH5 robot](https://www.youtube.com/watch?v=jjGQNstmLvY):
@@ -209,26 +285,31 @@
 
 ### Propagation of DMP Distribution to State Space
 
 <img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_matplotlib.png" width="60%" /><img src="https://raw.githubusercontent.com/dfki-ric/movement_primitives/main/doc/source/_static/dmp_state_space_distribution_kuka_peginhole_open3d.png" width="40%" />
 
 If we have a distribution over DMP parameters, we can propagate them to state
 space through an unscented transform.
+On the left we see the original demonstration of a dual-arm movement in state
+space (two 3D positions and two quaternions) and the distribution of several
+DMP weight vectors projected to the state space.
+On the right side we see several dual-arm trajectories sampled from the
+distribution in state space.
 
 [Script](https://github.com/dfki-ric/movement_primitives/blob/main/examples/external_dependencies/vis_dmp_to_state_variance.py)
 
 **Dependencies that are not publicly available:**
 
 * Dataset: panel rotation dataset of
-  [Mronga and Kirchner (2021)](https://www.sciencedirect.com/science/article/abs/pii/S0921889021000646)
+  [Mronga and Kirchner (2021)](https://doi.org/10.1016/j.robot.2021.103779)
 * MoCap library
 * URDF of dual arm
   [Kuka system](https://robotik.dfki-bremen.de/en/research/robot-systems/imrk/)
   from
-  [DFKI RIC's MRK lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/mrk-lab/):
+  [DFKI RIC's HRC lab](https://robotik.dfki-bremen.de/en/research/research-facilities-labs/hrc-lab):
   ```bash
   git clone git@git.hb.dfki.de:models-robots/kuka_lbr.git
   ```
 
 ## Build API Documentation
 
 You can build an API documentation with sphinx.
@@ -251,17 +332,18 @@
 To run the tests some python libraries are required:
 
 ```bash
 python -m pip install -e .[test]
 ```
 
 The tests are located in the folder `test/` and can be executed with:
-`python -m nose test`
+`python -m pytest`
 
-This command searches for all files with `test` and executes the functions with `test_*`.
+This command searches for all files with `test` and executes the functions
+with `test_*`. You will find a test coverage report at `htmlcov/index.html`.
 
 ## Contributing
 
 You can report bugs in the [issue tracker](https://github.com/dfki-ric/movement_primitives/issues).
 If you have questions about the software, please use the [discussions
 section](https://github.com/dfki-ric/movement_primitives/discussions).
 To add new features, documentation, or fix bugs you can open a pull request
```

### Comparing `movement_primitives-0.7.0/movement_primitives/base.py` & `movement_primitives-0.7.1/movement_primitives/base.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/data/_lasa.py` & `movement_primitives-0.7.1/movement_primitives/data/_lasa.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,19 @@
 
 
 def load_lasa(shape_idx):
     """Load demonstrations from LASA dataset.
 
     The LASA dataset contains 2D handwriting motions recorded from a
     Tablet-PC. It can be found `here
-    <https://bitbucket.org/khansari/lasahandwritingdataset>`_
+    <https://bitbucket.org/khansari/lasahandwritingdataset>`_.
     Take a look at the `detailed explanation
-    <http://cs.stanford.edu/people/khansari/DSMotions#SEDS_Benchmark_Dataset>`_
-    for more information.
-
-    The following plot shows multiple demonstrations for the same shape.
-
-    .. plot::
-
-        import matplotlib.pyplot as plt
-        from movement_primitives.data import load_lasa
-        X, Xd, Xdd, dt, shape_name = load_lasa(0)
-        plt.figure()
-        plt.title(shape_name)
-        plt.plot(X[:, :, 0].T, X[:, :, 1].T)
-        plt.show()
+    <https://cs.stanford.edu/people/khansari/download.html>`_
+    for more information. It was initially used to evaluate stable estimators
+    of dynamical systems [1]_.
 
     Parameters
     ----------
     shape_idx : int
         Choose demonstrated shape, must be within range(30).
 
     Returns
@@ -56,14 +45,21 @@
 
     dt : float
         Time between steps
 
     shape_name : string
         Name of the Matlab file from which we load the demonstrations
         (without suffix).
+
+    References
+    ----------
+    .. [1] Khansari-Zadeh, S. M., Billard, A. (2011).
+       Learning Stable Nonlinear Dynamical Systems With Gaussian Mixture Models.
+       IEEE Transactions on Robotics, 27 (5), 943-957. DOI:
+       10.1109/TRO.2011.2159412
     """
     dataset_path = get_common_dataset_path()
     if not os.path.isdir(dataset_path + "lasa_data"):  # pragma: no cover
         url = urlopen(LASA_URL)
         z = zipfile.ZipFile(io.BytesIO(url.read()))
         z.extractall(dataset_path)
         os.rename(dataset_path + z.namelist()[0],
```

### Comparing `movement_primitives-0.7.0/movement_primitives/data/_minimum_jerk.py` & `movement_primitives-0.7.1/movement_primitives/data/_minimum_jerk.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/data/_toy_1d.py` & `movement_primitives-0.7.1/movement_primitives/data/_toy_1d.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/__init__.py` & `movement_primitives-0.7.1/movement_primitives/dmp/__init__.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_base.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_base.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_canonical_system.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_canonical_system.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_cartesian_dmp.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_cartesian_dmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,14 +386,18 @@
             self.smooth_scaling)
         return T, np.hstack((Yp, Yr))
 
     def imitate(self, T, Y, regularization_coefficient=0.0,
                 allow_final_velocity=False):
         """Imitate demonstration.
 
+        Target forces for the forcing term are computed for the positions
+        in a similar way as in :func:`DMP.imitate`. For the orientations
+        we adapt this to handle quaternions adequately.
+
         Parameters
         ----------
         T : array, shape (n_steps,)
             Time for each step.
 
         Y : array, shape (n_steps, 7)
             State at each step.
```

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_coupling_terms.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_coupling_terms.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_dmp.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_dmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,15 +541,29 @@
             coupling_term,
             run_t, self.int_dt,
             step_function,
             smooth_scaling=self.smooth_scaling)
 
     def imitate(self, T, Y, regularization_coefficient=0.0,
                 allow_final_velocity=False):
-        """Imitate demonstration.
+        r"""Imitate demonstration.
+
+        Target forces of the forcing term are computed according to
+
+        .. math::
+
+            f_{target} =
+            \tau^2 \ddot{y}_{demo}
+            - \alpha_y(
+                \beta_y (g-y_{demo})
+                - \tau \dot{y}_{demo}
+                - \underline{\beta_y (g-y_0) z}
+            ),
+
+        where the underlined part is only used when smooth scaling is used.
 
         Parameters
         ----------
         T : array, shape (n_steps,)
             Time for each step.
 
         Y : array, shape (n_steps, n_dims)
```

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_dmp_with_final_velocity.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_dmp_with_final_velocity.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,30 @@
             run_t, self.int_dt,
             dmp_step_euler_with_constraints,
             start_yd=self.start_yd, start_ydd=self.start_ydd,
             goal_yd=self.goal_yd, goal_ydd=self.goal_ydd,
             smooth_scaling=self.smooth_scaling)
 
     def imitate(self, T, Y, regularization_coefficient=0.0):
-        """Imitate demonstration.
+        r"""Imitate demonstration.
+
+        Target forces of the forcing term are computed according to
+
+        .. math::
+
+            f_{target} =
+            \tau^2 \ddot{y}_{demo}
+            - \alpha_y(
+                \beta_y (g-y_{demo})
+                + \tau (\dot{g} - \dot{y}_{demo})
+            )
+            - \tau^2 \ddot{g},
+
+        where :math:`g, \dot{g}, \ddot{g}` are constraints that will be
+        recomputed in each step.
 
         Parameters
         ----------
         T : array, shape (n_steps,)
             Time for each step.
 
         Y : array, shape (n_steps, n_dims)
```

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_dual_cartesian_dmp.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_dual_cartesian_dmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -360,14 +360,18 @@
         self.t = 0.0
         return np.array(T), np.vstack(Y)
 
     def imitate(self, T, Y, regularization_coefficient=0.0,
                 allow_final_velocity=False):
         """Imitate demonstration.
 
+        Target forces for the forcing term are computed for the positions
+        in a similar way as in :func:`DMP.imitate`. For the orientations
+        we adapt this to handle quaternions adequately.
+
         Parameters
         ----------
         T : array, shape (n_steps,)
             Time for each step.
 
         Y : array, shape (n_steps, 14)
             State at each step.
```

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_forcing_term.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_forcing_term.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp/_state_following_dmp.py` & `movement_primitives-0.7.1/movement_primitives/dmp/_state_following_dmp.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp_fast.c` & `movement_primitives-0.7.1/movement_primitives/dmp_fast.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.5 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "movement_primitives.dmp_fast",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_5" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030005F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -578,26 +608,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -610,15 +641,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -643,15 +673,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -729,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -938,15 +973,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1082,15 +1117,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1169,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1283,32 +1318,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1350,15 +1368,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1470,15 +1488,15 @@
 static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__) && !defined(_MSC_VER))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -1538,177 +1556,177 @@
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1737,42 +1755,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2062,33 +2080,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-    static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2288,30 +2307,30 @@
 static void __Pyx_RaiseBufferIndexError(int axis);
 
 /* RaiseNoneIterError.proto */
 static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void);
 
 #define __Pyx_BufPtrStrided2d(type, buf, i0, s0, i1, s1) (type)((char*)buf + i0 * s0 + i1 * s1)
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_5
-#define __PYX_HAVE_RT_ImportType_proto_3_0_5
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_5(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_5 {
-   __Pyx_ImportType_CheckSize_Error_3_0_5 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_5 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_5 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportDottedModule.proto */
 static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
@@ -2413,15 +2432,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -3583,261 +3602,261 @@
 #define __pyx_codeobj__34 __pyx_mstate_global->__pyx_codeobj__34
 #define __pyx_codeobj__37 __pyx_mstate_global->__pyx_codeobj__37
 #define __pyx_codeobj__39 __pyx_mstate_global->__pyx_codeobj__39
 #define __pyx_codeobj__41 __pyx_mstate_global->__pyx_codeobj__41
 #define __pyx_codeobj__43 __pyx_mstate_global->__pyx_codeobj__43
 /* #### Code section: module_code ### */
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3846,29 +3865,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3879,15 +3898,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3896,29 +3915,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3929,15 +3948,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3946,29 +3965,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3979,15 +3998,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3996,29 +4015,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4029,15 +4048,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4046,29 +4065,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4079,217 +4098,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4305,15 +4324,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4321,68 +4340,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4390,15 +4409,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4413,15 +4432,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4437,15 +4456,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4453,68 +4472,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4522,15 +4541,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4545,15 +4564,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4569,15 +4588,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4585,68 +4604,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4654,15 +4673,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4677,170 +4696,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -16242,26 +16261,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../tmp/pip-build-env-6erj_v0p/overlay/lib/python3.9/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../tmp/pip-build-env-rhn8g0rh/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
@@ -16604,41 +16623,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_5(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_5); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_5(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_5(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_5); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 866, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -16845,15 +16864,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("dmp_fast", __pyx_methods, __pyx_k_Cython_implementations_of_basic, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to dmp_fast pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "dmp_fast" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -17894,22 +17913,22 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
         return NULL;
     for (i=0; i<nkwargs; i++) {
         PyObject *key = PyTuple_GET_ITEM(kwnames, i);
@@ -18011,15 +18030,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -18030,15 +18049,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -18062,15 +18081,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -19014,17 +19033,18 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
   static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -19157,15 +19177,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -19232,18 +19252,18 @@
 
 /* RaiseNoneIterError */
   static CYTHON_INLINE void __Pyx_RaiseNoneNotIterableError(void) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_5
-#define __PYX_HAVE_RT_ImportType_3_0_5
-static PyTypeObject *__Pyx_ImportType_3_0_5(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_5 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -19289,23 +19309,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_5 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_5 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -20556,15 +20576,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -21015,15 +21035,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp_fast.pyx` & `movement_primitives-0.7.1/movement_primitives/dmp_fast.pyx`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp_potential_field.py` & `movement_primitives-0.7.1/movement_primitives/dmp_potential_field.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/dmp_to_state_space_distribution.py` & `movement_primitives-0.7.1/movement_primitives/dmp_to_state_space_distribution.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/io.py` & `movement_primitives-0.7.1/movement_primitives/io.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/kinematics.py` & `movement_primitives-0.7.1/movement_primitives/kinematics.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/minimum_jerk_trajectory.py` & `movement_primitives-0.7.1/movement_primitives/minimum_jerk_trajectory.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/plot.py` & `movement_primitives-0.7.1/movement_primitives/plot.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/promp.py` & `movement_primitives-0.7.1/movement_primitives/promp.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,23 +104,25 @@
         Y : array, shape (n_steps, n_dims)
             Trajectory
         """
         return self._rbfs_nd_sequence(T).T.dot(weights).reshape(
             self.n_dims, len(T)).T
 
     def condition_position(self, y_mean, y_cov=None, t=0, t_max=1.0):
-        """Condition ProMP on a specific position (see page 4 of [1]).
+        """Condition ProMP on a specific position.
+
+        For details, see page 4 of [1]_
 
         Parameters
         ----------
         y_mean : array, shape (n_dims,)
-            Position mean
+            Position mean.
 
         y_cov : array, shape (n_dims, n_dims), optional (default: 0)
-            Covariance of position
+            Covariance of position.
 
         t : float, optional (default: 0)
             Time at which the activations of RBFs will be queried. Note that
             we internally normalize the time so that t_max == 1.
 
         t_max : float, optional (default: 1)
             Duration of the ProMP
@@ -128,16 +130,19 @@
         Returns
         -------
         conditional_promp : ProMP
             New conditional ProMP
 
         References
         ----------
-        [1] Paraschos et al.: Probabilistic movement primitives, NeurIPS (2013),
-        https://papers.nips.cc/paper/2013/file/e53a0a2978c28872a4505bdb51db06dc-Paper.pdf
+        .. [1] Paraschos, A., Daniel, C., Peters, J., Neumann, G. (2013).
+           Probabilistic movement primitives, In C.J. Burges and L. Bottou and
+           M. Welling and Z. Ghahramani and K.Q. Weinberger (Eds.), Advances in
+           Neural Information Processing Systems, 26,
+           https://papers.nips.cc/paper/2013/file/e53a0a2978c28872a4505bdb51db06dc-Paper.pdf
         """
         Psi_t = _nd_block_diagonal(
             self._rbfs_1d_point(t, t_max)[:, np.newaxis], self.n_dims)
         if y_cov is None:
             y_cov = 0.0
 
         common_term = self.weight_cov.dot(Psi_t).dot(
@@ -293,15 +298,19 @@
             This object
         """
         self.weight_mean = mean
         self.weight_cov = cov
         return self
 
     def imitate(self, Ts, Ys, n_iter=1000, min_delta=1e-5, verbose=0):
-        """Learn ProMP from multiple demonstrations.
+        r"""Learn ProMP from multiple demonstrations.
+
+        For details, see Section 3.2 of [1]_. We use the parameters
+        :math:`P = I` (identity matrix), :math:`\mu_0 = 0, k_0 = 0, \nu_0 = 0,
+        \Sigma_0 = 0,\alpha_0 = 0,\beta_0 = 0`.
 
         Parameters
         ----------
         Ts : array, shape (n_demos, n_steps)
             Time steps of demonstrations
 
         Ys : array, shape (n_demos, n_steps, n_dims)
@@ -311,23 +320,23 @@
             Maximum number of iterations
 
         min_delta : float, optional (default: 1e-5)
             Minimum delta between means to continue iteration
 
         verbose : int, optional (default: 0)
             Verbosity level
+
+        References
+        ----------
+        .. [1] Lazaric, A., Ghavamzadeh, M. (2010).
+           Bayesian Multi-Task Reinforcement Learning. In Proceedings of the
+           27th International Conference on International Conference on Machine
+           Learning (ICML'10) (pp. 599-606).
+           https://hal.inria.fr/inria-00475214/document
         """
-        # Section 3.2 of https://hal.inria.fr/inria-00475214/document
-        # P = I
-        # mu_0 = 0
-        # k_0 = 0
-        # nu_0 = 0
-        # Sigma_0 = 0
-        # alpha_0 = 0
-        # beta_0 = 0
         gamma = 0.7
 
         n_demos = len(Ts)
         self.variance = 1.0
 
         means = np.zeros((n_demos, self.n_weights))
         covs = np.empty((n_demos, self.n_weights, self.n_weights))
@@ -574,15 +583,15 @@
 
         centered = means - self.weight_mean
         self.weight_cov = (centered.T.dot(centered) + np.sum(covs, axis=0)) / M
         # TODO what is d + 2?
 
         self.variance = 0.0
         for i in range(len(means)):
-            # a trace is the same irrelevant of the order of matrix
+            # trace is the same, independent of the order of matrix
             # multiplications, see:
             # https://www.math.uwaterloo.ca/~hwolkowi/matrixcookbook.pdf,
             # Equation 16
             self.variance += np.trace(PhiHTHPhiTs[i].dot(covs[i]))
 
             self.variance += RRs[i]
             self.variance -= 2.0 * PhiHTR[i].T.dot(means[i].T)
```

### Comparing `movement_primitives-0.7.0/movement_primitives/spring_damper.py` & `movement_primitives-0.7.1/movement_primitives/spring_damper.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/testing/simulation.py` & `movement_primitives-0.7.1/movement_primitives/testing/simulation.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/movement_primitives/visualization.py` & `movement_primitives-0.7.1/movement_primitives/visualization.py`

 * *Files identical despite different names*

### Comparing `movement_primitives-0.7.0/setup.py` & `movement_primitives-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         packages=find_packages(),
         install_requires=[],
         extras_require={
             "all": ["pytransform3d", "cython", "numpy", "scipy", "matplotlib",
                     "open3d", "tqdm", "gmr", "PyYAML", "numba", "pybullet"],
             "doc": ["sphinx", "sphinx-bootstrap-theme", "numpydoc",
                     "myst-parser"],
-            "test": ["nose", "coverage"]
+            "test": ["pytest", "pytest-cov"]
         }
     )
     try:
         from Cython.Build import cythonize
         import numpy
         cython_config = dict(
             ext_modules=cythonize("movement_primitives/dmp_fast.pyx"),
```

