# Comparing `tmp/nrv-py-1.0.1.tar.gz` & `tmp/nrv_py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nrv-py-1.0.1.tar", last modified: Fri Jan 26 18:46:39 2024, max compression
+gzip compressed data, was "nrv_py-1.1.0.tar", last modified: Mon May 27 14:33:13 2024, max compression
```

## Comparing `nrv-py-1.0.1.tar` & `nrv_py-1.1.0.tar`

### file list

```diff
@@ -1,255 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.861634 nrv-py-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-01-26 18:46:25.000000 nrv-py-1.0.1/Licence.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-01-26 18:46:25.000000 nrv-py-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-01-26 18:46:39.861634 nrv-py-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-01-26 18:46:25.000000 nrv-py-1.0.1/ReadMe.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.797634 nrv-py-1.0.1/nrv/
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.797634 nrv-py-1.0.1/nrv/_misc/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/NRV.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.801634 nrv-py-1.0.1/nrv/_misc/OTF_PP/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/is_blocked.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/is_excited.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/is_onset.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/raster_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/rmv_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/OTF_PP/vmem_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.801634 nrv-py-1.0.1/nrv/_misc/comsol_templates/
--rw-r--r--   0 runner    (1001) docker     (127)   972710 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph
--rw-r--r--   0 runner    (1001) docker     (127)   442553 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph
--rw-r--r--   0 runner    (1001) docker     (127)   460556 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.805634 nrv-py-1.0.1/nrv/_misc/geom/
--rw-r--r--   0 runner    (1001) docker     (127)  1736930 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/geom/smoothed_edges_white.dxf
--rw-r--r--   0 runner    (1001) docker     (127)    81236 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/geom/smoothed_edges_white.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.805634 nrv-py-1.0.1/nrv/_misc/log/
--rw-r--r--   0 runner    (1001) docker     (127)  8377101 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/log/NRV.log
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.817634 nrv-py-1.0.1/nrv/_misc/materials/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/bone.mat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/cerebrospinal_fluid.mat
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/dura.mat
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/endoneurium_bhadra.mat
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/endoneurium_ranck.mat
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/epidural_space.mat
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/epineurium.mat
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/material_1.mat
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/material_2.mat
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/muscle.mat
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/perineurium.mat
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/platinum.mat
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/saline.mat
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/materials/silicone.mat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.829634 nrv-py-1.0.1/nrv/_misc/mods/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/AXNODE.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/CaPump.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/DNav18.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/KCa.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/NaCaPump.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/Nakpump.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/NakpumpSchild.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/Nav11_a.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/Nav16_a.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/RattayAberham.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/caextscale.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/caintscale.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/can.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/cat.mod
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/extrapump.mod
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/flut_motor.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/flut_sensory.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/h.mod
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/k_ion_dynamics.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/ka.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kaslow.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kd.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kdr.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kdr_Tiger.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kds.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kf.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kmtype.mod
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/kna.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/ks.mod
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/leak.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/leakSchild.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/mysa_motor.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/mysa_sensory.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/na3.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/na_ion_dynamics.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/naf.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/naf97.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/naf97mean.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nahh.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nas.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nas97.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nas97mean.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nattxs.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nav1p9.mod
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/nax.mod
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/node_motor.mod
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/node_sensory.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/stin_motor.mod
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/mods/stin_sensory.mod
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.837634 nrv-py-1.0.1/nrv/_misc/pops/
--rw-r--r--   0 runner    (1001) docker     (127)    23459 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)    23450 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)    23429 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)    23441 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)    23456 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)    23474 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_1000_axons_F.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_100_axons_F.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46916 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46879 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46946 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46882 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46948 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)    46923 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_2000_axons_F.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_200_axons_F.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117300 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117318 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117303 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117297 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117184 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)   117231 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_5000_axons_F.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_A.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_B.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11732 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_C.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_D.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_E.pop
--rw-r--r--   0 runner    (1001) docker     (127)    11710 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/pops/Population_of_500_axons_F.pop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.845634 nrv-py-1.0.1/nrv/_misc/ppops/
--rw-r--r--   0 runner    (1001) docker     (127)    63162 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    63158 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    63156 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    63146 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    63224 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    63118 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_F.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_F.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125839 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125735 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125872 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125804 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125951 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   125835 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_F.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_F.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316552 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316575 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316397 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316442 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316314 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)   316431 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31672 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31680 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31643 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31663 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop
--rw-r--r--   0 runner    (1001) docker     (127)    31668 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.849634 nrv-py-1.0.1/nrv/_misc/stats/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_11_A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_11_B.csv
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_11_C.csv
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_11_D.csv
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_9_A.csv
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_9_B.csv
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_9_C.csv
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Jacobs_9_D.csv
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Ochoa_M.csv
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Ochoa_U.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Schellens_1.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/_misc/stats/Schellens_2.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.849634 nrv-py-1.0.1/nrv/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     9416 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/MCore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/NRV_Class.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/NRV_Results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/NRV_Simulable.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/NRV_Singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/compileMods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/inouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/log_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/backend/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.853634 nrv-py-1.0.1/nrv/fmod/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.853634 nrv-py-1.0.1/nrv/fmod/FEM/
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/COMSOL_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/FEM.py
--rw-r--r--   0 runner    (1001) docker     (127)    21920 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/FENICS_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.853634 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/
--rw-r--r--   0 runner    (1001) docker     (127)    22805 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/FEMSimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15474 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/SimParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    16555 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/SimResult.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/fenics_materials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.853634 nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/
--rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/MshCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/NRV_Msh.py
--rw-r--r--   0 runner    (1001) docker     (127)    42858 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/NerveMshCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18022 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/electrodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    28918 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/extracellular.py
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/materials.py
--rw-r--r--   0 runner    (1001) docker     (127)    28036 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/fmod/stimulus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/nmod/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49940 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/axons.py
--rw-r--r--   0 runner    (1001) docker     (127)    33458 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/fascicle_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    65275 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/fascicles.py
--rw-r--r--   0 runner    (1001) docker     (127)    66698 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/myelinated.py
--rw-r--r--   0 runner    (1001) docker     (127)    27223 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/nerve.py
--rw-r--r--   0 runner    (1001) docker     (127)    41163 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nmod/unmyelinated.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5775 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/nrv2calm
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/CostFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/Optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/Problems.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/optim/optim_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/optim_utils/ContextModifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/optim_utils/CostEvaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/optim_utils/OptimFunctions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/optim/optim_utils/optim_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/utils/cell/
--rw-r--r--   0 runner    (1001) docker     (127)    11685 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/cell/CL_discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    40790 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/cell/CL_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41797 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/cell/CL_simulations.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/cell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.857634 nrv-py-1.0.1/nrv/utils/fascicle/
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/fascicle/FL_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/fascicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/nrv_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/saving_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-01-26 18:46:25.000000 nrv-py-1.0.1/nrv/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.861634 nrv-py-1.0.1/nrv_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-01-26 18:46:39.000000 nrv-py-1.0.1/nrv_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-01-26 18:46:39.000000 nrv-py-1.0.1/nrv_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 18:46:39.000000 nrv-py-1.0.1/nrv_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-26 18:46:39.000000 nrv-py-1.0.1/nrv_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-01-26 18:46:39.000000 nrv-py-1.0.1/nrv_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 18:46:39.861634 nrv-py-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-01-26 18:46:25.000000 nrv-py-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 18:46:39.797634 nrv-py-1.0.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10648 2024-01-26 18:46:25.000000 nrv-py-1.0.1/tests/NRV_test
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.301380 nrv_py-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    21778 2024-05-27 14:33:03.000000 nrv_py-1.1.0/Licence.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-27 14:33:03.000000 nrv_py-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-27 14:33:13.301380 nrv_py-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-27 14:33:03.000000 nrv_py-1.1.0/ReadMe.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.245380 nrv_py-1.1.0/nrv/
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.245380 nrv_py-1.1.0/nrv/_misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/NRV.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.249380 nrv_py-1.1.0/nrv/_misc/OTF_PP/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/ap_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/is_blocked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/is_excited.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/is_onset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/raster_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/rmv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/save_gmem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/OTF_PP/vmem_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.249380 nrv_py-1.1.0/nrv/_misc/comsol_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)   972710 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph
+-rw-r--r--   0 runner    (1001) docker     (127)   442553 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph
+-rw-r--r--   0 runner    (1001) docker     (127)   460556 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.253380 nrv_py-1.1.0/nrv/_misc/geom/
+-rw-r--r--   0 runner    (1001) docker     (127)  1736930 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/geom/smoothed_edges_white.dxf
+-rw-r--r--   0 runner    (1001) docker     (127)    81236 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/geom/smoothed_edges_white.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.253380 nrv_py-1.1.0/nrv/_misc/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/log/NRV.log
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.257381 nrv_py-1.1.0/nrv/_misc/materials/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/axoplasmic_mrg.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/bone.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/cerebrospinal_fluid.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/dura.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/endoneurium_bhadra.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/endoneurium_horn.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/endoneurium_ranck.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/epidural_space.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/epineurium.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/epineurium_horn.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/material_1.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/material_2.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/muscle.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/perineurium.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/perineurium_horn.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/platinum.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/saline.mat
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/materials/silicone.mat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.265380 nrv_py-1.1.0/nrv/_misc/mods/
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/AXNODE.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/CaPump.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/DNav18.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/KCa.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/NaCaPump.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/Nakpump.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/NakpumpSchild.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/Nav11_a.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/Nav16_a.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/RattayAberham.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/caextscale.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/caintscale.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/can.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/cat.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/extrapump.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/flut_motor.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/flut_sensory.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/h.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/k_ion_dynamics.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/ka.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kaslow.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kd.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kdr.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kdr_Tiger.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kds.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kf.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kmtype.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/kna.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/ks.mod
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/leak.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/leakSchild.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/mysa_motor.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/mysa_sensory.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/na3.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/na_ion_dynamics.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/naf.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/naf97.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/naf97mean.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nahh.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nas.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nas97.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nas97mean.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nattxs.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nav1p9.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/nax.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/node_motor.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/node_sensory.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/stin_motor.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/mods/stin_sensory.mod
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.273381 nrv_py-1.1.0/nrv/_misc/pops/
+-rw-r--r--   0 runner    (1001) docker     (127)    33459 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    33450 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    33429 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    33441 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    33456 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    33474 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_1000_axons_F.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_100_axons_F.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66916 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66879 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66946 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66882 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66948 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    66923 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_2000_axons_F.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)     6673 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_200_axons_F.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167300 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167318 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167303 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167297 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167184 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)   167231 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_5000_axons_F.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_A.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16730 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_B.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_C.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16720 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_D.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16705 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_E.pop
+-rw-r--r--   0 runner    (1001) docker     (127)    16710 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/pops/Population_of_500_axons_F.pop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.285380 nrv_py-1.1.0/nrv/_misc/ppops/
+-rw-r--r--   0 runner    (1001) docker     (127)    63162 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    63158 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    63156 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    63146 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    63224 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    63118 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_F.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6335 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_F.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125839 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125735 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125872 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125804 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125951 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   125835 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_F.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12703 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12674 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_F.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316552 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316575 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316397 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316442 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316314 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)   316431 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31672 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31680 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31643 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31663 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop
+-rw-r--r--   0 runner    (1001) docker     (127)    31668 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.285380 nrv_py-1.1.0/nrv/_misc/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Fugleholm.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_11_A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_11_B.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_11_C.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_11_D.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_9_A.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_9_B.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_9_C.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Jacobs_9_D.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Ochoa_M.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Ochoa_U.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Schellens_1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/_misc/stats/Schellens_2.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.289381 nrv_py-1.1.0/nrv/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     9798 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/MCore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/NRV_Class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/NRV_Results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/NRV_Simulable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/NRV_Singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/compileMods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/inouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/log_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/backend/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.289381 nrv_py-1.1.0/nrv/eit/
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/eit/Protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/eit/eit_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/eit/eit_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/eit/eit_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.289381 nrv_py-1.1.0/nrv/fmod/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.293381 nrv_py-1.1.0/nrv/fmod/FEM/
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/COMSOL_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/FEM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7933 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/FENICS_lumped_impedance_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23003 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/FENICS_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.293381 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    15517 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16226 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25303 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMSimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/f_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/fenics_materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/layered_materials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.293381 nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23142 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/MshCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/NRV_Msh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48805 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/NerveMshCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19806 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/electrodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29261 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/extracellular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/materials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28036 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19725 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/fmod/stimulus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.297381 nrv_py-1.1.0/nrv/nmod/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32592 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/axon_pop_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50404 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/axons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60175 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/fascicles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67208 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/myelinated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28795 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/nerve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.297381 nrv_py-1.1.0/nrv/nmod/results/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33128 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/axons_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/fascicles_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/myelinated_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/nerve_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/results/unmyelinated_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41163 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nmod/unmyelinated.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5775 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/nrv2calm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.297381 nrv_py-1.1.0/nrv/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/CostFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/Optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/Problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.297381 nrv_py-1.1.0/nrv/optim/optim_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/optim_utils/ContextModifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5937 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/optim_utils/CostEvaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/optim_utils/OptimFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/optim_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/optim/optim_utils/optim_results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.297381 nrv_py-1.1.0/nrv/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.301380 nrv_py-1.1.0/nrv/utils/cell/
+-rw-r--r--   0 runner    (1001) docker     (127)    39604 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/cell/CL_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38563 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/cell/CL_simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/cell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.301380 nrv_py-1.1.0/nrv/utils/fascicle/
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/fascicle/FL_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/fascicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19636 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/nrv_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/saving_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-27 14:33:03.000000 nrv_py-1.1.0/nrv/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.301380 nrv_py-1.1.0/nrv_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-05-27 14:33:13.000000 nrv_py-1.1.0/nrv_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8868 2024-05-27 14:33:13.000000 nrv_py-1.1.0/nrv_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:33:13.000000 nrv_py-1.1.0/nrv_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-27 14:33:13.000000 nrv_py-1.1.0/nrv_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-27 14:33:13.000000 nrv_py-1.1.0/nrv_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:33:13.301380 nrv_py-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-27 14:33:03.000000 nrv_py-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:33:13.245380 nrv_py-1.1.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10674 2024-05-27 14:33:03.000000 nrv_py-1.1.0/tests/NRV_test
```

### Comparing `nrv-py-1.0.1/Licence.txt` & `nrv_py-1.1.0/Licence.txt`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/PKG-INFO` & `nrv_py-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: nrv-py
-Version: 1.0.1
+Version: 1.1.0
 Summary: NeuRon Virtualizer (NRV)
 Home-page: https://github.com/fkolbl/NRV
 Author: Florian Kolbl, Roland Giraud, Louis Regnacq, Thomas Couppey
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Natural Language :: English
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh
 Requires-Dist: mph
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: neuron
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: ezdxf
 Requires-Dist: icecream
 Requires-Dist: pyswarms
+Requires-Dist: tqdm
 
 [![PyPI version](https://badge.fury.io/py/nrv-py.svg)](https://badge.fury.io/py/nrv-py)
 [![Documentation Status](https://readthedocs.org/projects/nrv/badge/?version=latest)](https://nrv.readthedocs.io/en/latest/?badge=latest)
 [![License: CeCill](https://img.shields.io/badge/Licence-CeCill-blue )](https://github.com/fkolbl/NRV/blob/master/Licence.txt)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10497741.svg)](https://doi.org/10.5281/zenodo.10497741)
 <!---[![DOI](xxxx)](xxx)-->
 <!---[![Build Status](xxxx)](xxx)-->
```

### Comparing `nrv-py-1.0.1/ReadMe.md` & `nrv_py-1.1.0/ReadMe.md`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/NRV.ini` & `nrv_py-1.1.0/nrv/_misc/NRV.ini`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 [FENICS]
 FENICS_STATUS = True
 FENICS_CPU = 1
 
 [GMSH]
 GMSH_STATUS = True
-GMSH_CPU = 1
+GMSH_CPU = 3
 
 [PARAVIEW]
 PARAVIEW = /Applications/ParaView-5.9.0.app/Contents/MacOS/paraview
 PARAVIEW_PYTHON = /Applications/ParaView-5.9.0.app/Contents/bin/pvpython
 PARAVIEW_SERVER = /Applications/ParaView-5.9.0.app/Contents/bin/pvserver
 PARAVIEW_SERVER_CPU = 3
 PARAVIEW_PORT = 11111
```

### Comparing `nrv-py-1.0.1/nrv/_misc/OTF_PP/is_blocked.py` & `nrv_py-1.1.0/nrv/_misc/OTF_PP/is_blocked.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/OTF_PP/is_excited.py` & `nrv_py-1.1.0/nrv/_misc/OTF_PP/is_excited.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/OTF_PP/is_onset.py` & `nrv_py-1.1.0/nrv/_misc/OTF_PP/is_onset.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/OTF_PP/raster_plot.py` & `nrv_py-1.1.0/nrv/_misc/OTF_PP/raster_plot.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 nrv.rasterize(axon_sim, "V_mem")
 nrv.remove_key(axon_sim, "V_mem", verbose=self.verbose)
 
 plt.figure()
 plt.scatter(axon_sim["V_mem_raster_time"], axon_sim["V_mem_raster_x_position"])
 plt.xlabel("time (ms)")
-plt.ylabel("position along the axon($\mu m$)")
+plt.ylabel(r'position along the axon($\mu m$)')
 title = (
     "Axon "
     + str(k)
     + ", myelination is "
     + str(axon_sim["myelinated"])
     + ", "
     + str(axon_sim["diameter"])
```

### Comparing `nrv-py-1.0.1/nrv/_misc/OTF_PP/vmem_plot.py` & `nrv_py-1.1.0/nrv/_misc/OTF_PP/vmem_plot.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph` & `nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph` & `nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph` & `nrv_py-1.1.0/nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/geom/smoothed_edges_white.dxf` & `nrv_py-1.1.0/nrv/_misc/geom/smoothed_edges_white.dxf`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/geom/smoothed_edges_white.png` & `nrv_py-1.1.0/nrv/_misc/geom/smoothed_edges_white.png`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/AXNODE.mod` & `nrv_py-1.1.0/nrv/_misc/mods/AXNODE.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/CaPump.mod` & `nrv_py-1.1.0/nrv/_misc/mods/CaPump.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/DNav18.mod` & `nrv_py-1.1.0/nrv/_misc/mods/DNav18.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/KCa.mod` & `nrv_py-1.1.0/nrv/_misc/mods/KCa.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/NaCaPump.mod` & `nrv_py-1.1.0/nrv/_misc/mods/NaCaPump.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/Nakpump.mod` & `nrv_py-1.1.0/nrv/_misc/mods/Nakpump.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/NakpumpSchild.mod` & `nrv_py-1.1.0/nrv/_misc/mods/NakpumpSchild.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/Nav11_a.mod` & `nrv_py-1.1.0/nrv/_misc/mods/Nav11_a.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/Nav16_a.mod` & `nrv_py-1.1.0/nrv/_misc/mods/Nav16_a.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/RattayAberham.mod` & `nrv_py-1.1.0/nrv/_misc/mods/RattayAberham.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/caextscale.mod` & `nrv_py-1.1.0/nrv/_misc/mods/caextscale.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/caintscale.mod` & `nrv_py-1.1.0/nrv/_misc/mods/caintscale.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/can.mod` & `nrv_py-1.1.0/nrv/_misc/mods/can.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/cat.mod` & `nrv_py-1.1.0/nrv/_misc/mods/cat.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/flut_motor.mod` & `nrv_py-1.1.0/nrv/_misc/mods/flut_motor.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/flut_sensory.mod` & `nrv_py-1.1.0/nrv/_misc/mods/flut_sensory.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/h.mod` & `nrv_py-1.1.0/nrv/_misc/mods/h.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/k_ion_dynamics.mod` & `nrv_py-1.1.0/nrv/_misc/mods/k_ion_dynamics.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/ka.mod` & `nrv_py-1.1.0/nrv/_misc/mods/ka.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kaslow.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kaslow.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kd.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kd.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kdr.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kdr.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kdr_Tiger.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kdr_Tiger.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kds.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kds.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kf.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kf.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kmtype.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kmtype.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/kna.mod` & `nrv_py-1.1.0/nrv/_misc/mods/kna.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/ks.mod` & `nrv_py-1.1.0/nrv/_misc/mods/ks.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/leak.mod` & `nrv_py-1.1.0/nrv/_misc/mods/leak.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/leakSchild.mod` & `nrv_py-1.1.0/nrv/_misc/mods/leakSchild.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/mysa_motor.mod` & `nrv_py-1.1.0/nrv/_misc/mods/mysa_motor.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/mysa_sensory.mod` & `nrv_py-1.1.0/nrv/_misc/mods/mysa_sensory.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/na3.mod` & `nrv_py-1.1.0/nrv/_misc/mods/na3.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/na_ion_dynamics.mod` & `nrv_py-1.1.0/nrv/_misc/mods/na_ion_dynamics.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/naf.mod` & `nrv_py-1.1.0/nrv/_misc/mods/naf.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/naf97.mod` & `nrv_py-1.1.0/nrv/_misc/mods/naf97.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/naf97mean.mod` & `nrv_py-1.1.0/nrv/_misc/mods/naf97mean.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nahh.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nahh.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nas.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nas.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nas97.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nas97.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nas97mean.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nas97mean.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nattxs.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nattxs.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nav1p9.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nav1p9.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/nax.mod` & `nrv_py-1.1.0/nrv/_misc/mods/nax.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/node_motor.mod` & `nrv_py-1.1.0/nrv/_misc/mods/node_motor.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/node_sensory.mod` & `nrv_py-1.1.0/nrv/_misc/mods/node_sensory.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/stin_motor.mod` & `nrv_py-1.1.0/nrv/_misc/mods/stin_motor.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/mods/stin_sensory.mod` & `nrv_py-1.1.0/nrv/_misc/mods/stin_sensory.mod`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_1000_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_1000_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_100_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_100_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_2000_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_2000_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_200_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_200_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop` & `nrv_py-1.1.0/nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/stats/Schellens_1.csv` & `nrv_py-1.1.0/nrv/_misc/stats/Schellens_1.csv`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/_misc/stats/Schellens_2.csv` & `nrv_py-1.1.0/nrv/_misc/stats/Schellens_2.csv`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/backend/MCore.py` & `nrv_py-1.1.0/nrv/backend/MCore.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if self.is_alone():
             print("Hi, I am the only core launched")
         elif self.is_master():
             print("Hi, I am the master core")
         else:
             print("Hi, I am a slave core, my ID is " + str(self.rank))
 
-    def split_job_from_arrays(self, len_arrays):
+    def split_job_from_arrays(self, len_arrays, stype="default"):
         """
         Split an array for parallel independant computing, by sharing independant sub-spaces \
         of array index
 
         Parameters
         ----------
         len_arrays  : int
@@ -94,20 +94,24 @@
         -------
         mask    : np.array
             subspace of the array indexes, specific to each instantiation of the programm
         """
         if self.is_alone():
             mask = np.arange(len_arrays)
         else:
-            if self.is_master():
-                all_indexes = np.arange(len_arrays)
-                mask_chunks = np.array_split(all_indexes, self.size, axis=0)
+            if stype=="comb":
+                mask = np.arange(len_arrays)
+                mask = np.where(self.rank == mask % self.size)[0]
             else:
-                mask_chunks = None
-            mask = comm.scatter(mask_chunks, root=0)
+                if self.is_master():
+                    all_indexes = np.arange(len_arrays)
+                    mask_chunks = np.array_split(all_indexes, self.size, axis=0)
+                else:
+                    mask_chunks = None
+                mask = comm.scatter(mask_chunks, root=0)
         return mask
 
     def split_job_from_arrays_to_slaves(self, len_arrays):
         """
         Split an array for parallel independant computing, by sharing independant sub-spaces \
         of array index, the master gets a table of all jobs to do initialized to False
 
@@ -184,14 +188,17 @@
         -------
         result  : dict
             global dict if master or alone, else None
         """
         if self.is_alone():
             final_result = partial_result
         else:
+            # Not ideal but prevent overwrite the type of master
+            if not self.is_master() and "nrv_type" in partial_result:
+                partial_result.pop("nrv_type")
             list_results = comm.gather(partial_result, root=0)
             if self.is_master():
                 final_result = list_results[0]
                 for i in range(1, len(list_results)):
                     final_result.update(list_results[i])
             else:
                 final_result = None
```

### Comparing `nrv-py-1.0.1/nrv/backend/NRV_Class.py` & `nrv_py-1.1.0/nrv/backend/NRV_Class.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/backend/NRV_Simulable.py` & `nrv_py-1.1.0/nrv/backend/NRV_Simulable.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 NRV-:class:`.NRV_simulable` handling.
 
 A generic class for all NRV simulable classes (:class:`~nrv.nmod.nerve`, :class:`~nrv.nmod.fascicle`, :class:`~nrv.nmod.myelinated`)
 """
 
 
 from .NRV_Class import NRV_class
-from .NRV_Results import sim_results
+from .NRV_Results import generate_results, sim_results
 
 
 def is_NRV_simulable(x):
     """
     Check if the object x is a :class:`.NRV_simulable`.
 
     Parameters
@@ -83,14 +83,15 @@
         record_V_mem=True,
         record_I_mem=False,
         record_I_ions=False,
         record_particles=False,
         record_g_mem=False,
         record_g_ions=False,
         loaded_footprints=None,
+        **kwargs
     ):
         super().__init__()
         self.t_sim = t_sim
         self.record_V_mem = record_V_mem
         self.record_I_mem = record_I_mem
         self.record_I_ions = record_I_ions
         self.record_particles = record_particles
@@ -171,9 +172,9 @@
         self.set_parameters(**kwargs)
         context = self.save(
             save=False,
             extracel_context=self.extracel_status(),
             intracel_context=self.intracel_status(),
             rec_context=self.rec_status(),
         )
-        results = sim_results(context)
+        results = generate_results(context)
         return results
```

### Comparing `nrv-py-1.0.1/nrv/backend/NRV_Singleton.py` & `nrv_py-1.1.0/nrv/backend/NRV_Singleton.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/backend/compileMods.py` & `nrv_py-1.1.0/nrv/backend/compileMods.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/backend/file_handler.py` & `nrv_py-1.1.0/nrv/backend/file_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 NRV-I/O File Handler.
 """
 import json
 import os
-
-import ezdxf
 import numpy as np
 
-from .log_interface import rise_error, rise_warning
+from .log_interface import rise_error, rise_warning, pass_info
 
 
 #################
 # Miscalleneous #
 #################
 def is_iterable(some_stuff):
     """
@@ -95,15 +93,15 @@
         name of the folder to create
     access_rights : int
         unix like rights
     """
     try:
         os.mkdir(foldername, access_rights)
     except OSError:
-        rise_warning(
+        pass_info(
             "Creation of the directory %s failed, this folder may already exist"
             % foldername
         )
 
 
 #######################
 ## JSON related code ##
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/COMSOL_model.py` & `nrv_py-1.1.0/nrv/fmod/FEM/COMSOL_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
         """
         Close the FEM simulation and the COMSOL link
         """
         if self.__has_client:
             self.client.disconnect()
             del self.client
             self.__has_client = False
-        print(self.handle_server or self.__has_server)
         if self.handle_server or self.__has_server:
             self.server.stop()
             del self.server
             self.__has_server = False
 
     def __del__(self):
         self.close()
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/FEM.py` & `nrv_py-1.1.0/nrv/fmod/FEM/FEM.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,21 @@
         Set the number of cores to use for the FEM
 
         Parameters
         ----------
         N       : int
             Number of cores to set
         """
+        if isinstance(N, bool):
+            if N:
+                N = MCH.size
+            else:
+                N = 1
+        if N is None:
+            N = 1
         self.Ncore = N
         if self.Ncore > MCH.size:
             rise_warning(
                 "MCH size is " + str(MCH.size) + " cannot set FEM on more processes"
             )
             self.Ncore = MCH.size
         self.is_multi_proc = self.Ncore > 1
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/FENICS_model.py` & `nrv_py-1.1.0/nrv/fmod/FEM/FENICS_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 import time
 
 import numpy as np
 from mpi4py import MPI
 
 from ...backend.file_handler import rmv_ext
 from ...utils.units import V, mm
+from ...utils.misc import get_perineurial_thickness
 from ...backend.MCore import MCH, synchronize_processes
+from ...backend.log_interface import rise_warning
 from .fenics_utils.FEMSimulation import FEMSimulation
 
 from .FEM import FEM_model
-from .fenics_utils.SimResult import save_sim_res_list
+from .fenics_utils.FEMResults import save_sim_res_list
 from .mesh_creator.NerveMshCreator import NerveMshCreator, ENT_DOM_offset, pi
 
 # built in FENICS models
 dir_path = os.environ["NRVPATH"] + "/_misc"
 # material_library = os.listdir(dir_path+"/fenics_templates/")
 
 ###############
@@ -29,25 +31,54 @@
 machine_config.read(config_fname)
 
 FENICS_Ncores = int(machine_config.get("FENICS", "FENICS_CPU"))
 FENICS_Status = machine_config.get("FENICS", "FENICS_STATUS") == "True"
 
 fem_verbose = True
 
+def check_sim_dom(sim:FEMSimulation, mesh:NerveMshCreator):
+    """
+    Check if all the physical domains of a mesh are linked to a material property.
+    This function can either prevent errors or help to debbug
+
+    Paramters
+    ---------
+    sim:    FEMSimulation
+        Simulation to check.
+    mesh:   NerveMshCreator
+        Mesh in used for the silmulation.
+
+    Returns
+    -------
+    bool
+        True if all domains are linked to a material, False otherwise.
+    """
+    uset_dom = []
+    mdom = mesh.domains_3D
+    if sim.D == 2:
+        mdom = mesh.domains_2D
+
+    for i in mdom:
+        if not i in sim.domains_list:
+            uset_dom += [i]
+    if len(uset_dom):
+        rise_warning(f" the following domains are not set {uset_dom}")
+        return False
+    return True
+
 
 class FENICS_model(FEM_model):
     """
     A class for FENICS Finite Element Models, inherits from FEM_model.
     """
 
     def __init__(
         self,
         fname=None,
         Ncore=None,
-        handle_server=False,
         elem=None,
         comm="default",
         rank=0,
     ):
         """
         Creates a instance of a FENICS Finite Element Model object.
 
@@ -63,38 +94,36 @@
         super().__init__(Ncore=Ncore)
         self.type = "FENICS"
         # Default paramerters
         self.L = 5000
         self.y_c = 0
         self.z_c = 0
         self.Outer_D = 5  # mm
-        self.Nerve_D = 250  # um
-        self.N_fascicle = 0
+        self.Nerve_D = 500  # um
         self.fascicles = {}
         self.Perineurium_thickness = {}
-        self.N_electrode = 0
         self.electrodes = {}
-        self.Istim = 1e-3  # A
+        self.i_stim = 1e-3  # A
         self.jstims = []
         self.j_electrode = {}
 
         self.Outer_mat = "saline"
         self.Epineurium_mat = "epineurium"
         self.Endoneurium_mat = "endoneurium_ranck"
         self.Perineurium_mat = "perineurium"
         self.Electrodes_mat = 1  # "platinum"
 
-        self.default_fascicle = {"D": 200, "y_c": 0, "z_c": 0, "res": 20}
+        self.default_fascicle = {"d": 250, "y_c": 0, "z_c": 0, "res": 250/3}
         self.default_electrode = {
             "elec_type": "LIFE",
             "x_c": self.L / 2,
             "y_c": 0,
             "z_c": 0,
             "length": 1000,
-            "D": 25,
+            "d": 25,
             "res": 3,
         }
 
         # Mesh
         self.mesh_file = fname
         self.mesh = None
         self.elem = elem
@@ -125,14 +154,22 @@
                 Length=self.L,
                 Outer_D=self.Outer_D,
                 Nerve_D=self.Nerve_D,
                 y_c=self.y_c,
                 z_c=self.z_c,
             )
 
+    @property
+    def N_fascicle(self):
+        return len(self.fascicles)
+
+    @property
+    def N_electrode(self):
+        return len(self.electrodes)
+
     def save(self, save=False, fname="Fenics_model.json", blacklist=[], **kwargs):
         """
         Save the changes to the model file. (Avoid for the overal weight of the package)
         """
         bl = [i for i in blacklist]
         bl += ["comm", "rank", "mesh", "sim", "sim_res"]
         return super().save(save=save, fname=fname, blacklist=bl, **kwargs)
@@ -172,15 +209,15 @@
             y_c=param["y_c"],
             z_c=param["z_c"],
         )
         for id in param["fascicles"]:
             fasc = param["fascicles"][id]
             per_th = param["Perineurium_thickness"][id]
             self.reshape_fascicle(
-                fasc["D"],
+                fasc["d"],
                 y_c=fasc["y_c"],
                 z_c=fasc["z_c"],
                 ID=int(id),
                 Perineurium_thickness=per_th,
                 res=fasc["res"],
             )
         for id in param["electrodes"]:
@@ -218,25 +255,23 @@
         """
         param = {}
         param["L"] = self.L
         param["y_c"] = self.y_c
         param["z_c"] = self.z_c
         param["Outer_D"] = self.Outer_D / mm
         param["Nerve_D"] = self.Nerve_D
-        param["N_fascicle"] = self.N_fascicle
         param["fascicles"] = self.fascicles
         param["Perineurium_thickness"] = self.Perineurium_thickness
         param["N_electrode"] = self.N_electrode
         param["electrodes"] = self.electrodes
         param["Outer_mat"] = self.Outer_mat
         param["Epineurium_mat"] = self.Epineurium_mat
         param["Endoneurium_mat"] = self.Endoneurium_mat
         param["Perineurium_mat"] = self.Perineurium_mat
-        param["Perineurium_mat"] = self.Perineurium_mat
-        param["Istim"] = self.Istim
+        param["i_stim"] = self.i_stim
         return param
 
     def __update_parameters(self, bcast=False):
         """
         Internal use only: updates all the parameters from the mesh
 
         Parameters
@@ -263,20 +298,18 @@
         reset model parameters
         """
         self.L = 5000
         self.y_c = 0
         self.z_c = 0
         self.Outer_D = 5  # mm
         self.Nerve_D = 250  # um
-        self.N_fascicle = 0
         self.fascicles = {}
         self.Perineurium_thickness = {}
-        self.N_electrode = 0
         self.electrodes = {}
-        self.Istim = 1e-3  # A
+        self.i_stim = 1e-3  # A
         self.jstims = []
         self.j_electrode = {}
 
         self.mesh_file_status = self.mesh_file is not None
         self.is_sim_ready = False
         self.is_meshed = False
         self.is_computed = False
@@ -305,15 +338,15 @@
         outer_D : float
             FEM simulation outer box diameter, in mm, WARNING, this is the only parameter in mm !
         """
         if not self.mesh_file_status:
             self.mesh.reshape_outerBox(Outer_D=Outer_D, res=res)
             self.__update_parameters()
 
-    def reshape_nerve(self, Nerve_D, Length, y_c=0, z_c=0, res="default"):
+    def reshape_nerve(self, Nerve_D=None, Length=None, y_c=0, z_c=0, res="default"):
         """
         Reshape the nerve of the FEM simulation
 
         Parameters
         ----------
         Nerve_D                 : float
             Nerve diameter, in um
@@ -323,23 +356,23 @@
             Nerve center y-coordinate in um, 0 by default
         z_c                     : float
             Nerve z-coordinate center in um, 0 by default
         Perineurium_thickness   :float
             Thickness of the Perineurium sheet surounding the fascicles in um, 5 by default
         """
         if not self.mesh_file_status:
-            self.L = Length
-            self.Nerve_D
+            self.L = Length or self.L
+            self.Nerve_D = Nerve_D or self.Nerve_D
             self.mesh.reshape_nerve(
-                Nerve_D=Nerve_D, Length=Length, y_c=y_c, z_c=z_c, res=res
+                Nerve_D=self.Nerve_D, Length=self.L, y_c=y_c, z_c=z_c, res=res
             )
             self.__update_parameters()
 
     def reshape_fascicle(
-        self, Fascicle_D, y_c=0, z_c=0, ID=None, Perineurium_thickness=5, res="default"
+        self, Fascicle_D, y_c=0, z_c=0, ID=None, Perineurium_thickness=None, res="default"
     ):
         """
         Reshape a fascicle of the FEM simulation
 
         Parameters
         ----------
         Fascicle_D  : float
@@ -355,33 +388,33 @@
             self.mesh.reshape_fascicle(Fascicle_D, y_c, z_c, ID, res)
             self.__update_parameters()
             if ID is None:
                 if self.Perineurium_thickness == {}:
                     ID = 0
                 else:  ## To check when not all ID are fixed
                     ID = max(self.Perineurium_thickness) + 1
-            self.Perineurium_thickness[ID] = Perineurium_thickness
+
+            p_th = Perineurium_thickness or get_perineurial_thickness(Fascicle_D)
+            self.Perineurium_thickness[ID] = p_th
 
     def remove_fascicles(self, ID=None):
         """
         remove a fascicle of the FEM simulation
 
         Parameters
         ----------
         ID          : int, None
             ID number of the fascicle to remove, if None, remove all fascicles, by default None
         """
         if ID is None:
             self.fascicles = {}
             self.Perineurium_thickness = {}
-            self.N_fascicle = 0
         elif ID in self.fascicles:
             del self.fascicles[ID]
             del self.Perineurium_thickness[ID]
-            self.N_fascicle -= 1
         self.mesh.remove_fascicles(ID=ID)
 
     def add_electrode(self, elec_type, ID=None, res="default", **kwargs):
         """
         TO BE WRITTEN
         """
         if not self.mesh_file_status:
@@ -408,64 +441,39 @@
                 mesh_file=self.mesh_file,
                 mesh=self.mesh,
                 elem=self.elem,
                 comm=self.comm,
                 rank=self.rank,
             )
             # Outerbox domain
-            self.sim.add_domain(
-                mesh_domain=ENT_DOM_offset["Outerbox"], mat_pty=self.Outer_mat
-            )
-            # Nerve domain
-            self.sim.add_domain(
-                mesh_domain=ENT_DOM_offset["Nerve"], mat_pty=self.Epineurium_mat
-            )
-            for i in self.fascicles.keys():
-                self.sim.add_domain(
-                    mesh_domain=ENT_DOM_offset["Fascicle"] + (2 * i),
-                    mat_pty=self.Endoneurium_mat,
-                )
-            for _, (i, elec) in enumerate(self.electrodes.items()):
-                if not elec["type"] == "LIFE":
-                    self.sim.add_domain(
-                        mesh_domain=ENT_DOM_offset["Electrode"] + (2 * i),
-                        mat_pty=self.Electrodes_mat,
-                    )
+            self.__set_domains()
             # SETTING INTERNAL BOUNDARY CONDITION (for perineuriums)
-            for i in self.fascicles:
-                thickness = self.Perineurium_thickness[i]
-                f_dom = ENT_DOM_offset["Fascicle"] + (2 * i)
-                self.sim.add_inboundary(
-                    mesh_domain=ENT_DOM_offset["Surface"] + f_dom,
-                    mat_pty=self.Perineurium_mat,
-                    thickness=thickness,
-                    in_domains=[f_dom],
-                )
+            self.__set_iboundaries()
             # SETTING BOUNDARY CONDITION
             # Ground (to the external ring of Outerbox)
             self.sim.add_boundary(mesh_domain=1, btype="Dirichlet", value=0)
             # Injected current from active electrode
             # For EIT change in for E in elec_patren:
             for _, (E, active_elec) in enumerate(self.electrodes.items()):
                 E_var = "E" + str(E)
                 mesh_domain_3D = self.__find_elec_subdomain(active_elec)
-                self.jstims += {self.__find_elec_jstim(active_elec)}
                 self.j_electrode[E_var] = 0
                 e_dom = (
                     ENT_DOM_offset["Surface"] + ENT_DOM_offset["Electrode"] + (2 * E)
                 )
                 self.sim.add_boundary(
                     mesh_domain=e_dom,
                     btype="Neuman",
                     variable=E_var,
                     mesh_domain_3D=mesh_domain_3D,
                 )
             # set a parallelizable preconditionner if sim solve on multiple precesses
             if self.is_multi_proc:
                 self.sim.set_solver_opt(pc_type="hypre")
+            self.sim.setup_sim(**self.j_electrode)
             self.is_sim_ready = True
             self.setup_timer += time.time() - t0
 
     def set_materials(
         self,
         Outer_mat=None,
         Epineurium_mat=None,
@@ -485,57 +493,89 @@
         Endoneurium_mat     :str
             Endoneurium material fname if None not changed, by default None
         Perineurium_mat     :str
             Outer material fname if None not changed, by default None
         Electrodes_mat      :str
             Electrodes material fname if None not changed, by default None
         """
-        if Outer_mat is not None:
-            self.Outer_mat = Outer_mat
-        if Epineurium_mat is not None:
-            self.Epineurium_mat = Epineurium_mat
-        if Endoneurium_mat is not None:
-            self.Endoneurium_mat = Endoneurium_mat
-        if Perineurium_mat is not None:
-            self.Perineurium_mat = Perineurium_mat
-        if Electrodes_mat is not None:
-            self.Electrodes_mat = Electrodes_mat
+        self.Outer_mat = Outer_mat or self.Outer_mat
+        self.Epineurium_mat = Epineurium_mat or self.Epineurium_mat
+        self.Endoneurium_mat = Endoneurium_mat or self.Endoneurium_mat
+        self.Perineurium_mat = Perineurium_mat or self.Perineurium_mat
+        self.Electrodes_mat = Electrodes_mat or self.Electrodes_mat
+
+    def __set_domains(self):
+        """
+        Internal use only: set the material properties of physical domains
+        """
+        self.sim.add_domain(
+            mesh_domain=ENT_DOM_offset["Outerbox"], mat_pty=self.Outer_mat
+        )
+        # Nerve domain
+        self.sim.add_domain(
+            mesh_domain=ENT_DOM_offset["Nerve"], mat_pty=self.Epineurium_mat
+        )
+        for i in self.fascicles.keys():
+            self.sim.add_domain(
+                mesh_domain=ENT_DOM_offset["Fascicle"] + (2 * i),
+                mat_pty=self.Endoneurium_mat,
+            )
+        for _, (i, elec) in enumerate(self.electrodes.items()):
+            if not elec["type"] == "LIFE":
+                self.sim.add_domain(
+                    mesh_domain=ENT_DOM_offset["Electrode"] + (2 * i),
+                    mat_pty=self.Electrodes_mat,
+                )
+
+    def __set_iboundaries(self):
+        """
+        Internal use only: set internam boundaries
+        """
+        for i in self.fascicles:
+            thickness = self.Perineurium_thickness[i]
+            f_dom = ENT_DOM_offset["Fascicle"] + (2 * i)
+            self.sim.add_inboundary(
+                mesh_domain=ENT_DOM_offset["Surface"] + f_dom,
+                mat_pty=self.Perineurium_mat,
+                thickness=thickness,
+                in_domains=[f_dom],
+            )
 
     def __find_elec_subdomain(self, elec) -> int:
         """
         Internal use only:
         """
         if elec["type"] == "LIFE":
             y_e, z_e = elec["kwargs"]["y_c"], elec["kwargs"]["z_c"]
             for i in self.fascicles:
                 fascicle = self.fascicles[i]
-                d_f, y_f, z_f = fascicle["D"], fascicle["y_c"], fascicle["z_c"]
+                d_f, y_f, z_f = fascicle["d"], fascicle["y_c"], fascicle["z_c"]
                 if (y_e - y_f) ** 2 + (z_e - z_f) ** 2 < (d_f / 2) ** 2:
                     return 10 + 2 * i
         return 0
 
     def __find_elec_jstim(self, elec, I=None) -> float:
         """
         Internal use only: return electrical current density in electrode
         from current valeu and electrode geometry
         """
         # Unitary stimulation
         if I is not None:
-            self.Istim = I
+            self.i_stim = I
 
-        if elec["type"] == "CUFF":
-            d_e = self.Nerve_D + 2 * elec["kwargs"]["contact_thickness"]
+        """if elec["type"] == "CUFF":
+            d_e = self.Nerve_D
             l_e = elec["kwargs"]["contact_length"]
 
         elif elec["type"] == "LIFE":
-            d_e = elec["kwargs"]["D"]
-            l_e = elec["kwargs"]["length"]
+            d_e = elec["kwargs"]["d"]
+            l_e = elec["kwargs"]["length"]"""
 
-        S = pi * (d_e) * (l_e)
-        jstim = self.Istim / S
+        S = self.sim
+        jstim = self.i_stim / S
         return jstim
 
     ###################
     ## Use the model ##
     ###################
 
     def get_meshes(self):
@@ -551,27 +591,27 @@
         Build the geometry and perform meshing process
         """
         if not self.mesh_file_status and not self.is_meshed:
             t0 = time.time()
             self.__update_parameters()
             if self.N_fascicle == 0:
                 self.reshape_fascicle(
-                    Fascicle_D=self.default_fascicle["D"],
+                    Fascicle_D=self.default_fascicle["d"],
                     y_c=self.default_fascicle["y_c"],
                     z_c=self.default_fascicle["z_c"],
                     res=self.default_fascicle["res"],
                 )
             if self.N_electrode == 0:
                 self.add_electrode(
                     elec_type=self.default_electrode["elec_type"],
                     x_c=self.default_electrode["x_c"],
                     y_c=self.default_electrode["y_c"],
                     z_c=self.default_electrode["z_c"],
                     length=self.default_electrode["length"],
-                    D=self.default_electrode["D"],
+                    d=self.default_electrode["d"],
                     res=self.default_electrode["res"],
                 )
             self.__update_parameters(bcast=self.is_multi_proc)
             if MCH.do_master_only_work():
                 self.mesh.compute_mesh()
             if self.is_multi_proc:
                 synchronize_processes()
@@ -587,15 +627,18 @@
             self.setup_simulations()
         if not self.is_computed:
             t0 = time.time()
             # For EIT change in for E in elec_patren:
             for E in range(self.N_electrode):
                 for i_elec in self.j_electrode:
                     if i_elec == "E" + str(E):
-                        self.j_electrode[i_elec] = self.jstims[E]
+                        e_dom = (
+                            ENT_DOM_offset["Surface"] + ENT_DOM_offset["Electrode"] + (2 * E)
+                        )
+                        self.j_electrode[i_elec] = self.i_stim/self.sim.get_surface(e_dom)
                     else:
                         self.j_electrode[i_elec] = 0
                 self.sim.setup_sim(**self.j_electrode)
                 self.sim_res += [self.sim.solve()]
                 self.sim_res[-1].vout.label = "E" + str(E)
             self.is_computed = True
             self.solving_timer += time.time() - t0
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/FEMSimulation.py` & `nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMSimulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 """
 NRV-:class:`.FEMSimulation` handling.
 """
 import os
 import time
 import numpy as np
+import sys
 
+from dolfinx import default_scalar_type
 from dolfinx.fem import (
     Constant,
     Function,
-    FunctionSpace,
+    functionspace,
     assemble_scalar,
     dirichletbc,
     form,
     locate_dofs_topological,
 )
 from dolfinx.fem.petsc import LinearProblem
 from mpi4py import MPI
 from petsc4py.PETSc import ScalarType, Viewer
 from ufl import (
-    FiniteElement,
     Measure,
-    MixedElement,
     TestFunction,
     TrialFunction,
     avg,
     inner,
     nabla_grad,
+    CellDiameter,
 )
+from basix.ufl import element, mixed_element
+
 
 from ....backend.log_interface import pass_info, rise_error, rise_warning
 from ....backend.file_handler import rmv_ext
 from ....utils.units import S, V, m
-from .fenics_materials import load_fenics_material
-from .SimParameters import SimParameters
-from .SimResult import read_gmsh, SimResult
+from .fenics_materials import fenics_material
+from .FEMParameters import FEMParameters
+from .FEMResults import read_gmsh, FEMResults
 
 # Lists of available solvers and conditioners
 # go to https://petsc4py.readthedocs.io/en/stable/manual/ksp/ for more info
 
 ksp_type_list = [
     "cg",
     "pipecg",
@@ -96,43 +99,43 @@
     "cholesky",
     "none",
     "shell",
     "hypre",
 ]
 
 
-class FEMSimulation(SimParameters):
+class FEMSimulation(FEMParameters):
     r"""
     Class usefull to solve the Static/Quasi-Static electrical current problem using FEM with
     FEniCSx algorithms (https://fenicsproject.org).
 
     .. math::
 
         \nabla \mathbf{j}(\mathbf{r}) = 0
 
     .. math::
 
         \mathbf{j}(\mathbf{r}) = \mathbf{\sigma} (\mathbf{r}) \nabla V (\mathbf{r}), \forall \mathbf{r} \in \Omega
 
     Where \\(\\Omega\\) is the simulation space, \\(\\bf{j}\\) the the current density and \\(V\\) the electrical potential
 
-    The problem parameters (domains and boundaries condition) can be define using SimParameters methods
+    The problem parameters (domains and boundaries condition) can be define using FEMParameters methods
     Contains methods to setup the matrix sytstem, to solve it and to access the results.
 
     Parameters
     ----------
     D               : int
         dim of the mesh, by default 3
         NB: only 3 is implemented
     mesh_file       : str
         mesh directory and file name: by default ""
     mesh            : None or MshCreator
         if not None, (MshCreator) from which the mesh sould be used, by default None
-    data            : str, dict or SimParameters
-        if not None, load SimParameters attribute from data, by default None
+    data            : str, dict or FEMParameters
+        if not None, load FEMParameters attribute from data, by default None
     elem            :tupple (str, int)
         if None, ("Lagrange", 1), else (element type, element order), by default None
     ummesh          : bool
         if True the scale of mesh space dimensions should be (um), else (m), by default True
         Usefull to link the update materials conductivity as in NRV conductivities are in S/m
         but NerveMshCreator space scale is um)
     comm            : int
@@ -206,14 +209,15 @@
             "ksp_rtol": 1e-4,
             "ksp_atol": 1e-7,
             "ksp_max_it": 1000,
         }
         self.cg_problem = None
         self.dg_problem = None
         self.u = None
+        self.v = None
         self.mixedvout = None
         self.vout = None
         self.result = None
 
         # Mcore attributes
         self.comm = comm
         self.rank = rank
@@ -223,14 +227,15 @@
 
         self.bcs = []
         # added for overzriting false option
         self.file = []
 
         self.data_status = True
         self.domain_status = False
+        self.material_map_satus = False
         self.dirichlet_BC_status = False
         self.neumann_BC_status = False
         self.bilinear_form_status = False
         self.jump_status = False
         self.linear_form_status = False
         self.setup_status = False
         self.solve_status = False
@@ -257,44 +262,42 @@
             mat_pty,
             mat_file,
             mat_perm,
             ID,
         )
         if self.setup_status:
             if mesh_domain in self.mat_map:
-                mat = load_fenics_material(mat_pty)
-                self.mat_map[mesh_domain].load_from_mat(mat)
+                self.mat_map[mesh_domain].update_mat(mat_pty)
             else:
                 rise_warning(
                     "Domain not added: new domain cannot be added between 2 simulations,\
                              (set domain before simulation or create a new one)"
                 )
 
     def add_domain(
         self, mesh_domain, mat_pty=None, mat_file=None, mat_perm=None, ID=None
     ):
         super().add_domain(mesh_domain, mat_pty, mat_file, mat_perm, ID)
         if self.setup_status:
             if mesh_domain in self.mat_map:
-                mat = load_fenics_material(mat_pty)
-                self.mat_map[mesh_domain].load_from_mat(mat)
+                self.mat_map[mesh_domain].update_mat(mat_pty)
             else:
                 rise_warning(
                     "Domain not added: new domain cannot be added between 2 simulations,\
                              (set domain before simulation or create a new one)"
                 )
 
     #####################################################
     ############ setup the matrix sytstem #############
     #####################################################
 
     def setup_sim(self, **kwargs):
         """
         setup Bilinear form, Linear form and boundary conditions using paramters and kwargs
-        to set the variable defined Neumann boundary conditions (see SimParameters.add_boundary)
+        to set the variable defined Neumann boundary conditions (see FEMParameters.add_boundary)
         If FEMSimulation already defined, can be used to modify variable defined NBC
         """
         t0 = time.time()
         if self.data_status:
             self.args = kwargs
             pass_info("Static/Quasi-Static electrical current problem")
             if self.D == 1:
@@ -303,15 +306,15 @@
                 # Initialize the domain
                 if not self.domain_status:
                     self.__init_domain()
                 # DIRICHLET BOUNDARY CONDITIONS
                 if not self.dirichlet_BC_status:
                     self.__set_dirichlet_BC()
                 # DEFINING THE VARIATIONAL PROBLEM
-                self.mixedvout = TrialFunction(self.V)
+                self.v = TrialFunction(self.V)
                 self.u = TestFunction(self.V)
                 # defining the bilinear form a(vout,u)
                 if not self.bilinear_form_status:
                     self.__set_bilinear_form()
                 # defining the linear form L(u)
                 # NB1: in the case of the current-problem, the source term is nul
                 if not self.linear_form_status:
@@ -332,21 +335,21 @@
             self.domain, self.subdomains, self.boundaries = read_gmsh(
                 self.mesh, comm=self.comm, rank=self.rank, gdim=3
             )
             # SPACE FOR INTEGRATION
             if self.inbound:
                 self.Nspace = self.Ninboundaries + 1
                 ME = [
-                    FiniteElement(self.elem[0], self.domain.ufl_cell(), self.elem[1])
-                    for k in range(self.Nspace)
+                    element(self.elem[0], self.domain.basix_cell(), self.elem[1], dtype=ScalarType)
+                    for _ in range(self.Nspace)
                 ]
-                self.multi_elem = MixedElement(ME)
+                self.multi_elem = mixed_element(ME)
             else:
                 self.multi_elem = self.elem
-            self.V = FunctionSpace(self.domain, self.multi_elem)
+            self.V = functionspace(self.domain, self.multi_elem)
             # MEASURES FOR INTEGRATION
             self.dx = Measure("dx", domain=self.domain, subdomain_data=self.subdomains)
             self.ds = Measure("ds", domain=self.domain, subdomain_data=self.boundaries)
             self.dS = Measure("dS", domain=self.domain, subdomain_data=self.boundaries)
             self.domain_status = True
 
     def __set_dirichlet_BC(self):
@@ -378,15 +381,15 @@
             )
         self.dirichlet_BC_status = True
 
     def __set_neumann_BC(self):
         """
         internal use only: set the Neuman boundary condition from parameters or update
         variable between to simulation
-        NB: Only variable NBC (see SimParameters.add_boundary) can be changed between simulations
+        NB: Only variable NBC (see FEMParameters.add_boundary) can be changed between simulations
         """
         if not self.neumann_BC_status:
             for i_bound in self.boundaries_list:
                 bound = self.boundaries_list[i_bound]
                 condition = bound["condition"]
                 if condition.lower() in "neumann":
                     dom = int(bound["mesh_domain"])
@@ -424,80 +427,86 @@
         """
         internal use only: set the bilinear form a(vout, u) from the parameters
         """
         pass_info("FEN4NRV: setup the bilinear form")
         self.__set_material_map()
         for i_space in range(self.Nspace):
             for i_domain in self.domains_list:
-                dom = self.get_mixedspace_domain(i_space=i_space, i_domain=i_domain)
+                i_mat = self.get_mixedspace_domain(i_space=i_space, i_domain=i_domain)
                 if self.a is None:
-                    self.a = self.__get_static_component(i_domain, dom, i_space)
+                    self.a = self.__get_static_component(i_domain, i_mat, i_space)
                 else:
-                    self.a += self.__get_static_component(i_domain, dom, i_space)
+                    self.a += self.__get_static_component(i_domain, i_mat, i_space)
         if self.inbound:
             self.__set_jump()
         self.bilinear_form_status = True
 
     def __get_static_component(self, i_dom, i_mat, i_space):
-        """
+        r"""
         Set a static componnent of the bimlinear form:
-        a = ∇v[i_space] x 𝜎[i_mat]∇u[i_space] dx(i_dom)
+
+        .. math::
+
+            a = \nablav[i_{space}] \sigma[i_mat] \nabla u[i_{space}] dx(i_{dom})
+
         Parameters
         ----------
         i_dom    : int
             id of the domain on which the component should be set
         i_mat       : int
             id of the material corresponding domain on which the component should be set
         i_space     : int
             id of the i_space
         """
         if not self.inbound:
             return inner(
-                nabla_grad(self.mixedvout),
+                nabla_grad(self.v),
                 self.mat_map[i_mat].sigma_fen * nabla_grad(self.u),
             ) * self.dx(i_dom)
         else:
             return inner(
-                nabla_grad(self.mixedvout[i_space]),
+                nabla_grad(self.v[i_space]),
                 self.mat_map[i_mat].sigma_fen * nabla_grad(self.u[i_space]),
             ) * self.dx(i_dom)
 
     def __set_jump(self):
         """
         internal use only: set the jump for all internale boundary to mimic the thin layers
         """
         for i_ibound in self.inboundaries_list:
             in_space, out_space = self.get_spaces_of_ibound(i_ibound)
             local_thickness = Constant(
                 self.domain, ScalarType(self.inboundaries_list[i_ibound]["thickness"])
             )
-            jmp_v = avg(self.mixedvout[out_space]) - avg(self.mixedvout[in_space])
+            jmp_v = avg(self.v[out_space]) - avg(self.v[in_space])
             jmp_u = avg(self.u[out_space]) - avg(self.u[in_space])
             self.a += (
                 self.mat_map[i_ibound].sigma_fen
                 / local_thickness
                 * jmp_u
                 * jmp_v
                 * self.dS(i_ibound)
             )
         self.jump_status = True
 
     def __set_material_map(self):
         """
         internal use only: build a dictionnary mat_map containing a material for every domain and layer
         """
-        if self.mat_unit == "S/um":
-            UN = S / m
-        else:
-            UN = 1
-        for dom, pty in self.mat_pty_map.items():
-            self.mat_map[dom] = load_fenics_material(pty)
-            self.mat_map[dom].update_fenics_sigma(
-                domain=self.domain, elem=self.elem, UN=UN, id=dom
-            )
+        if not self.material_map_satus:
+            if self.mat_unit == "S/um":
+                UN = S / m
+            else:
+                UN = 1
+            for dom, pty in self.mat_pty_map.items():
+                self.mat_map[dom] = fenics_material(pty)
+                self.mat_map[dom].update_fenics_sigma(
+                    domain=self.domain, elem=self.elem, UN=UN, id=dom
+                )
+            self.material_map_satus = True
 
     def __set_linear_form(self):
         """
         internal use only: set the linear form L(u) from the parameters
         """
         pass_info("FEN4NRV: setup the linear form")
         # Check if quicker without
@@ -516,15 +525,15 @@
     def get_solver_opt(self):
         """
         get krylov solver options
         """
         return self.petsc_opt
 
     def set_solver_opt(
-        self, ksp_type=None, pc_type=None, ksp_rtol=None, ksp_atol=None, ksp_max_it=None
+        self, ksp_type=None, pc_type=None, ksp_rtol=None, ksp_atol=None, ksp_max_it=None, **kwargs,
     ):
         """
         set krylov solver options
 
         Parameters
         ----------
         ksp_type        : str
@@ -551,14 +560,21 @@
                 rise_warning(pc_type + " not set, should be in:\n" + pc_type_list)
         if ksp_rtol is not None:
             self.petsc_opt["ksp_rtol"] = ksp_rtol
         if ksp_atol is not None:
             self.petsc_opt["ksp_atol"] = ksp_atol
         if ksp_max_it is not None:
             self.petsc_opt["ksp_max_it"] = ksp_max_it
+        for key in kwargs:
+            if "pc" in key and self.petsc_opt["pc_type"] in key:
+                self.petsc_opt[key] = kwargs[key]
+            elif "ksp" in key and self.petsc_opt["ksp_type"] in key:
+                self.petsc_opt[key] = kwargs[key]
+            else:
+                rise_warning(key + " is not a valid solver option not set")
 
     def set_result_merging(self, to_merge=None):
         if isinstance(to_merge, bool):
             self.to_merge = to_merge
         else:
             self.to_merge = not self.to_merge
 
@@ -568,34 +584,35 @@
 
         Parameters
         ----------
         overwrite   : bool
             if true modify the existing sim_res value, else create a new one. by default False
         Returns
         -------
-        self.results    : SimResult
-            SimResult containing the result of the resulting field of the FEM simulation
+        self.results    : FEMResults
+            FEMResults containing the result of the resulting field of the FEM simulation
         """
         t0 = time.time()
         pass_info("FEN4NRV: solving electrical potential")
         if self.cg_problem is None:
+            self.mixedvout = Function(self.V)
             self.cg_problem = LinearProblem(
                 self.a, self.L, bcs=self.bcs, petsc_options=self.petsc_opt
             )
-        self.mixedvout = self.cg_problem.solve()
+        self.mixedvout.x.array[:] = self.cg_problem.solve().x.array
         self.solve_status = True
 
         if self.inbound and self.to_merge:
             V_sol = self.__merge_mixed_solutions()
         else:
             self.vout = self.mixedvout.copy()
             V_sol = self.V
 
         # return simulation result
-        self.result = SimResult()
+        self.result = FEMResults()
         if not overwrite:
             vout = Function(V_sol)
             vout.x.array[:] = self.vout.x.array[:]
         else:
             vout = self.vout
         self.result.set_sim_result(
             mesh_file=self.mesh_file,
@@ -608,61 +625,107 @@
         self.solving_timer += time.time() - t0
         pass_info("FEN4NRV: solved in " + str(self.solving_timer) + " s")
         return self.result
 
     def __merge_mixed_solutions(self):
         if self.dg_problem is None:
             self.mixedvouts = self.mixedvout.split()
-            self.V_DG = FunctionSpace(
+            self.V_DG = functionspace(
                 self.domain, ("Discontinuous Lagrange", self.elem[1])
             )
-            u, v = TrialFunction(self.V_DG), TestFunction(self.V_DG)
-            adg = u * v * self.dx
+            u_, v_ = TrialFunction(self.V_DG), TestFunction(self.V_DG)
+            adg = u_ * v_ * self.dx
             Ldg = 0
             for i_domain in self.domainsID:
                 i_space = self.get_space_of_domain(i_domain)
-                Ldg += v * self.mixedvout[i_space] * self.dx(i_domain)
+                Ldg += v_ * self.mixedvout[i_space] * self.dx(i_domain)
             self.dg_problem = LinearProblem(
                 adg, Ldg, bcs=[], petsc_options=self.petsc_opt
             )
         else:
             mixedvouts = self.mixedvout.split()
             for i in range(len(mixedvouts)):
                 self.mixedvouts[i].x.array[:] = mixedvouts[i].x.array
         self.vout = self.dg_problem.solve()
         return self.V_DG
 
+    def compute_conductance(self, order=None):
+        self.__init_domain()
+        self.__set_material_map()
+        V_sigma = self.V
+        od = order or self.elem[1]
+        V_sigma = functionspace(
+            self.domain, ("DG", od)
+        )
+        sigma_out = []
+        for i_space in range(self.Nspace):
+            sigma = Function(V_sigma)
+            for i_domain in self.domainsID:
+                dom_cells = self.subdomains.find(i_domain)
+                dom_dofs = locate_dofs_topological(V_sigma, self.domain.topology.dim, dom_cells)
+                i_mat = self.get_mixedspace_domain(i_space=i_space, i_domain=i_domain)
+                mat = self.mat_map[i_mat].mat
+                if mat.is_isotropic():
+                    val = np.full_like(dom_dofs, mat.sigma, dtype=default_scalar_type)
+                elif not mat.is_func:
+                    #val = mat.sigma_fen.value
+                    _sig = sum(mat.sigma ** 2) ** 0.5
+                    val = np.full_like(dom_dofs, _sig, dtype=default_scalar_type)
+                elif mat.is_func:
+                    sig_ = Function(V_sigma)
+                    sig_.interpolate(mat.sigma_func)
+                    val = sig_.x.array[dom_dofs]
+                sigma.x.array[dom_dofs] = val
+            self.sigma_results = FEMResults()
+            self.sigma_results.set_sim_result(
+                mesh_file=self.mesh_file,
+                domain=self.domain,
+                elem=self.multi_elem,
+                V=V_sigma,
+                vout=sigma,
+                comm=self.domain.comm,
+            )
+            sigma_out += [self.sigma_results]
+        return sigma_out
+
     #####################################################
     ################ Access the results #################
     #####################################################
 
     def solver_info(self, txt_fname="solver.txt"):
         solver = self.cg_problem.solver
         viewer = Viewer().createASCII(txt_fname)
         solver.view(viewer)
         solver_output = open(txt_fname, "r")
         for line in solver_output.readlines():
-            print(line)
+            pass_info(line)
 
     def solve_and_save_sim(self, filename, save=True):
         if not self.solve_status:
             self.solve()
         fname = rmv_ext(filename)
         self.result.save(fname)
         return self.result
 
     def get_timers(self):
         return self.solving_timer
 
     def visualize_mesh(self):
         os.system("gmsh " + self.mesh_file + ".msh")
 
+    def get_surface(self, dom_id):
+        S = assemble_scalar(form(1 * self.ds(dom_id)))
+        if self.comm == MPI.COMM_WORLD:
+            S = self.comm.reduce(S, op=MPI.SUM, root=0)
+            S = self.comm.bcast(S, root=0)  
+        return S
+
     def get_domain_potential(self, dom_id, dim=2, space=0):
         if dim == 2:
             do = self.ds
         elif dim == 3:
             do = self.dx
-        Surf = assemble_scalar(form(1 * do(dom_id)))
+        Surf = self.get_surface(dom_id)
         if self.to_merge:
             return assemble_scalar(form(self.vout * do(dom_id))) / Surf * V
         else:
             return assemble_scalar(form(self.vout[space] * do(dom_id))) / Surf * V
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/SimParameters.py` & `nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMParameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 """
-NRV-:class:`.SimParameters` handling.
+NRV-:class:`.FEMParameters` handling.
 """
 import numpy as np
 
 from ....backend.file_handler import json_dump, json_load, rmv_ext
 from ....backend.log_interface import rise_error, rise_warning
 from ....backend.NRV_Class import NRV_class, is_empty_iterable
 
 
 def is_sim_param(X):
     """
-    check if an object is a SimParameters, return True if yes, else False
+    check if an object is a FEMParameters, return True if yes, else False
 
     Parameters
     ----------
     X : object
         object to test
 
     Returns
     -------
     bool
-        True it the type is a SimParameters object
+        True it the type is a FEMParameters object
     """
-    return isinstance(X, SimParameters)
+    return isinstance(X, FEMParameters)
 
 
-class SimParameters(NRV_class):
+class FEMParameters(NRV_class):
     """
     Class gathering parameters of a FEM FEniCS simulation. It allows to add,
     modify and store domains, boundaries condition and internal boundaries (thin layers)
     Can be saved and used to generate FEMsimulation.
     """
 
     def __init__(self, D=3, mesh_file="", data=None):
         """
-        initialisation of the SimParameters:
+        initialisation of the FEMParameters:
 
         Parameters
         ----------
         D               :int
             dim of the mesh, by default 3
             NB: only 3 is implemented
         mesh_file       :str
             mesh directory and file name: by default ""
-        data            :str, dict or SimParameters
-            if not None, load SimParameters attribute from data, by default None
-            (see SimParameters.load)
+        data            :str, dict or FEMParameters
+            if not None, load FEMParameters attribute from data, by default None
+            (see FEMParameters.load)
         """
         super().__init__()
         self.type = "simparameters"
         self.D = D
         self.mesh_file = rmv_ext(mesh_file)
 
         # domains
@@ -70,24 +70,24 @@
 
         # gather mat_pty name for domain and internal layer
         self.mat_pty_map = {}
 
         if data is not None:
             self.load(data)
 
-    def save(self, save=False, fname="SimParameters.json"):
+    def save(self, save=False, fname="FEMParameters.json"):
         """
-        Return SimParameters as dictionary and eventually save it as json file
+        Return FEMParameters as dictionary and eventually save it as json file
 
         Parameters
         ----------
         save    : bool
             if True, save in json files
         fname   : str
-            Path and Name of the saving file, by default "SimParameters.json"
+            Path and Name of the saving file, by default "FEMParameters.json"
 
         Returns
         -------
         sp_dic : dict
             dictionary containing all information
         """
         sp_dic = {}
@@ -106,20 +106,20 @@
         sp_dic["mat_pty_map"] = self.mat_pty_map
         if save:
             json_dump(sp_dic, fname)
         return sp_dic
 
     def load(self, data):
         """
-        Load all SimParameters properties from a dictionary or a json file
+        Load all FEMParameters properties from a dictionary or a json file
 
         Parameters
         ----------
         data    : str or dict
-            json file path or dictionary containing SimParameters information
+            json file path or dictionary containing FEMParameters information
         """
         if type(data) == str:
             sp_dic = json_load(data)
         elif is_sim_param(data):
             sp_dic = self.save()
         else:
             sp_dic = data
@@ -133,19 +133,19 @@
         self.boundaries_list = sp_dic["boundaries"]
         self.inbound = sp_dic["inbound"]
         self.Ninboundaries = sp_dic["Ninboundaries"]
         self.inboundariesID = sp_dic["inboundariesID"]
         self.inboundaries_list = sp_dic["inboundaries"]
         self.mat_pty_map = sp_dic["mat_pty_map"]
 
-    def save_SimParameters(self, save=False, fname="SimParameters.json"):
+    def save_SimParameters(self, save=False, fname="FEMParameters.json"):
         rise_warning("save_SimParameters is a deprecated method use save")
         return self.save(save=save, fname=fname)
 
-    def load_SimParameters(self, data="SimParameters.json"):
+    def load_SimParameters(self, data="FEMParameters.json"):
         rise_warning("load_SimParameters is a deprecated method use load")
         self.load(data=data)
 
     def set_mesh_file(self, new_mesh_file):
         """
         set a new mesh file name
 
@@ -289,20 +289,20 @@
         ID=None,
     ):
         """
         add new internal boundary or update if mesh_domain already exists
 
         Parameters
         ----------
-        mesh_domain     : int
-            Mesh ID of the boundary (should be 2D)
+        mesh_domain     : int or list(int)
+            Mesh ID or IDs of the boundary (should be 2D-domains)
         in_domains       : list
             List of mesh IDs of the domain (if 3D group) or internal boundary (if 2D group)
             inside the boundary
-        thickness       : float
+        thickness       : float or list(float)
             thicness of the internal boundary
         mat_pty         : str, float or list[3]
             Material property, either mat_file or mat_perm
         mat_file        : str
             Material filename (see fmod.material.py) if None use mat_perm,
                 by default None
         mat_perm        : float or list[3]
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/fenics_utils/SimResult.py` & `nrv_py-1.1.0/nrv/fmod/FEM/fenics_utils/FEMResults.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,104 +1,92 @@
 """
-NRV-:class:`.SimResult` handling.
+NRV-:class:`.FEMResults` handling.
 """
 
 import gmsh
 import numpy as np
 import scipy
-from dolfinx.fem import Expression, Function, FunctionSpace
+from dolfinx.fem import Expression, Function, functionspace
 from dolfinx.io.gmshio import model_to_mesh
 from dolfinx.io.utils import XDMFFile, VTXWriter, VTKFile
+from dolfinx.cpp.mesh import entities_to_geometry
+from dolfinx.geometry import (
+bb_tree,
+compute_colliding_cells,
+compute_collisions_points,
+compute_closest_entity,
+compute_distance_gjk,
+create_midpoint_tree,
+)
 from mpi4py import MPI
 
 
 from ....backend.file_handler import rmv_ext
 from ....backend.log_interface import rise_error, rise_warning
 from ....backend.parameters import parameters
 from ....backend.MCore import MCH, synchronize_processes
 from ....backend.NRV_Class import NRV_class
 from ..mesh_creator.MshCreator import (
     is_MshCreator,
     clear_gmsh,
 )
-# issue #38 See if this should be kept or not
-# Not ideal but requiered because of changes in dolfinx
-dfx_utd = parameters.check_dolfinx_version("0.7.0")
-if dfx_utd:
-    from dolfinx.geometry import (
-    bb_tree,
-    compute_colliding_cells,
-    compute_collisions_points,
-    )
-else:
-    from dolfinx.geometry import (
-    BoundingBoxTree,
-    compute_colliding_cells,
-    compute_collisions,
-    )
-# issue #38 ############
+
+
+
 
 ###############
 ## Functions ##
 ###############
 def is_sim_res(result):
     """
-    check if an object is a SimResult, return True if yes, else False
+    check if an object is a FEMResults, return True if yes, else False
 
     Parameters
     ----------
     result : object
         object to test
 
     Returns
     -------
     bool
-        True it the type is a SimResult object
+        True it the type is a FEMResults object
     """
-    return isinstance(result, SimResult)
+    return isinstance(result, FEMResults)
 
 
-def save_sim_res_list(sim_res_list, fname, vtxtype=True, dt=1.):
+def save_sim_res_list(sim_res_list, fname, dt=1.):
     r"""
     save a list of SimResults in a .bp folder which can be open with PrarView
 
     Parameters
     ----------
-    sim_res_list : list(SimResult)
-        list of :class:`.SimResult` to be saved
+    sim_res_list : list(FEMResults)
+        list of :class:`.FEMResults` to be saved
     fname : str
         File name and path
     ftype : str 
         - if True .bp folder, else saved in a .xdmf file.
     dt : float
         time step between each results
 
     Warning
     -------
     For this function to work dolfinx and ParaView must be up to date: 
         -   dolfinx \\(\\geq\\) 0.8.0
         -   ParaView \\(\\geq\\) 5.12.0
     """
-    if vtxtype and dfx_utd:
-        fname = rmv_ext(fname) + ".bp"
-        N_list = len(sim_res_list)
-        vcp = sim_res_list[0].vout
-        vtxf = VTXWriter(sim_res_list[0].domain.comm, fname, vcp)
-        for i in range(N_list):
-            vcp.x.array[:] = sim_res_list[i].vout.x.array
-            vtxf.write(i * dt)
-        vtxf.close()
-    # issue #38 See if this should be kept or not
-    else:
-        fname = rmv_ext(fname) + ".xdmf"
-        xdmf = XDMFFile(sim_res_list[0].domain.comm, fname, "w")
-        xdmf.write_mesh(sim_res_list[0].domain)
-        for i in range(N_list):
-            xdmf.write_function(sim_res_list[i].vout, i * dt)
-    # issue #38 ############
+    N_list = len(sim_res_list)
+    fname = rmv_ext(fname) + ".bp"
+    vcp = sim_res_list[0].vout
+    vtxf = VTXWriter(sim_res_list[0].domain.comm, fname, vcp)
+    for i in range(N_list):
+        vcp = sim_res_list[i].vout
+        vtxf.write(i * dt)
+    vtxf.close()
+
 
 
 def read_gmsh(mesh, comm=MPI.COMM_WORLD, rank=0, gdim=3):
     """
     Given a mesh_file or a MeshCreator returns mesh cell_tags and facet_tags
     (see dolfinx.io.gmshio.model_to_mesh for more details)
     NB: copy of dolfinx.io.gmshio.read_from_msh verbose from gmsh
@@ -152,19 +140,28 @@
             domain of the mesh contain in the mesh_file
     """
     return read_gmsh(mesh_file)[0]
 
 
 def V_from_meshfile(mesh_file, elem=("Lagrange", 1)):
     mesh = domain_from_meshfile(mesh_file)
-    V = FunctionSpace(mesh, elem)
+    V = functionspace(mesh, elem)
     return V
 
 
-class SimResult(NRV_class):
+def closest_point_in_mesh(mesh, point, tree, tdim, midpoint_tree):
+    points = np.reshape(point, (1,3))
+    entity = compute_closest_entity(tree, midpoint_tree, mesh, points)
+    mesh_geom = mesh.geometry.x
+    geom_dofs = entities_to_geometry(mesh._cpp_object, tdim, entity, False)
+    mesh_nodes = mesh_geom[geom_dofs][0]
+    displacement = compute_distance_gjk(points, mesh_nodes)
+    return entity, points[0] - displacement
+
+class FEMResults(NRV_class):
     """
     Result of a FEMSimulation.
     Store the resulting function space giving the possibility to apply basic mathematical
     operations on multiple results
     """
 
     def __init__(
@@ -173,26 +170,26 @@
         domain=None,
         elem=("Lagrange", 1),
         V=None,
         vout=None,
         comm=MPI.COMM_WORLD,
     ):
         """
-        initialisation of the SimParameters:
+        initialisation of the FEMParameters:
 
         Parameters
         ----------
         mesh_file       :str
             mesh directory and file name: by default ""
         domain       : None or mesh
             mesh domain on which the result is defined, by default None
         elem            :tupple (str, int)
             if None, ("Lagrange", 1), else (element type, element order), by default None
-        V       : None or dolfinx.fem.FunctionSpace
-            FunctionSpace on which the result is defined, by default None
+        V       : None or dolfinx.fem.functionspace
+            functionspace on which the result is defined, by default None
         vout       : None or dolfinx.fem.Function
             Function resulting from the FEMSimulation, by default None
         comm            :int
             The MPI communicator to use for mesh creation, by default MPI.COMM_WORLD
         """
         super().__init__()
         self.type = "simresult"
@@ -216,15 +213,15 @@
             self.V = V
         if vout is not None:
             self.vout = vout
         self.comm = comm
 
     def save(self, file, ftype="vtx", overwrite=True, t=0.0):
         fname = rmv_ext(file)
-        if ftype.lower() == "vtx" and dfx_utd:
+        if ftype.lower() == "vtx": #and dfx_utd:
             fname += ".bp"
             with VTXWriter(self.domain.comm, fname, self.vout, "bp4") as f:
                 f.write(t)
         elif ftype == "xdmf":
             fname += ".xdmf"
             with XDMFFile(self.comm, fname, "w") as file:
                 if not overwrite:
@@ -247,15 +244,15 @@
     def load(self, file):
         fname = rmv_ext(file) + ".sres"
         mdict = scipy.io.loadmat(fname)
         self.mesh_file = mdict["mesh_file"][0]
         self.elem = (mdict["element"][0].strip(), int(mdict["element"][1]))
         if self.domain is None:
             self.domain = domain_from_meshfile(self.mesh_file)
-            self.V = FunctionSpace(self.domain, self.elem)
+            self.V = functionspace(self.domain, self.elem)
         self.vout = Function(self.V)
         self.vout.vector[:] = mdict["vout"]
 
     def save_sim_result(self, file, ftype="vtx", overwrite=True):
         rise_warning("save_sim_result is a deprecated method use save")
         self.save(file=file, ftype=ftype, overwrite=overwrite)
 
@@ -270,72 +267,70 @@
     #############
 
     def vector(self):
         return self.vout.x.array
 
     def aline_V(self, res2):
         """
-        Change the function space of the result to aline with the result of another SimResult
+        Change the function space of the result to aline with the result of another FEMResults
 
         Parameters
         ----------
-        res2 : SimResult
+        res2 : FEMResults
             result to aline with
         """
         if is_sim_res(res2):
             if self.mesh_file == res2.mesh_file:
                 expr = Expression(self.vout, res2.V.element.interpolation_points())
                 self.vout = Function(res2.V)
                 self.vout.interpolate(expr)
                 self.V = res2.V
             else:
                 rise_error(
                     "To aline mesh function reslults must have the same meshfile"
                 )
         else:
-            rise_error("Mesh function alinment must be done with SimResult")
+            rise_error("Mesh function alinment must be done with FEMResults")
 
     def eval(self, X, is_multi_proc=False):
         """
         Eval the result field at X position
         """
+        X = np.array(X)
         N = len(X)
-        to_round = False
         cells = []
         points_on_proc = []
-        if dfx_utd:
-            tree = bb_tree(self.domain, self.domain.geometry.dim)
-            # Find cells whose bounding-box collide with the the points
-            cells_candidates = compute_collisions_points(tree, X)
-            # issue #38 See if this should be kept or not
-        else:
-            tree = BoundingBoxTree(self.domain, self.domain.geometry.dim)
-            # Find cells whose bounding-box collide with the the points
-            cells_candidates = compute_collisions(tree, X)
-            # issue #38 ############
+        tdim = self.domain.geometry.dim
+        n_entities_local = self.domain.topology.index_map(tdim).size_local\
+            + self.domain.topology.index_map(tdim).num_ghosts
+        entities = np.arange(n_entities_local, dtype=np.int32)
+        midpoint_tree = create_midpoint_tree(self.domain, tdim, entities)
+        tree = bb_tree(self.domain, tdim)
+        # Find cells whose bounding-box collide with the the points
+        cells_candidates = compute_collisions_points(tree, X)
+
         # Choose one of the cells that contains the point
         cells_colliding = compute_colliding_cells(self.domain, cells_candidates, X)
         for i in range(N):
             cell = cells_colliding.links(i)
             if is_multi_proc:
                 if len(cell) > 0:
                     points_on_proc.append(X[i])
                     cells.append(cells_colliding.links(i)[0])
             else:
+                #point not in the mesh
                 if len(cell) == 0:
-                    if i == N - 1 and i > 0:
-                        to_round = True
-                    else:
-                        rise_warning(
-                            X[i], " not found in mesh, value of ", X[i - 1], " reused"
-                        )
-                    cells += [cells[-1]]
+                    cell, x_closest = closest_point_in_mesh(self.domain, X[i], tree, tdim, midpoint_tree)
+                    rise_warning(
+                        X[i], " not found in mesh, value of ", x_closest, " reused"
+                    )
+                    #compute_colliding_cells(self.domain, cells_candidates, X)
+                    cells += [cell[0]]
                 else:
                     cells += [cell[0]]
-
         if is_multi_proc:
             points_on_proc = np.array(points_on_proc, dtype=np.float64)
             s_values = self.vout.eval(points_on_proc, cells)
             if len(points_on_proc) > 0:
                 m_values = np.concatenate((points_on_proc.T, s_values.T)).T
             else:
                 m_values = np.array([])
@@ -357,40 +352,35 @@
                 values = np.empty((N), dtype="float64")
             synchronize_processes()
             self.comm.Bcast(values, root=0)
         else:
             values = self.vout.eval(X, cells)
             if N > 1:
                 values = values[:, 0]
-        if to_round:
-            X_1 = X[-1]
-            X_1[0] = round(X_1[0], 1)
-            value_1 = self.eval([X_1], is_multi_proc=is_multi_proc)
-            values[-1] = value_1[0]
         return values
 
     #####################
     ## special methods ##
     #####################
     def __abs__(self):
-        res = SimResult(
+        res = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         if self.vout is not None:
             expr = Expression(abs(self.vout), self.V.element.interpolation_points())
             res.vout = Function(self.V)
             self.vout.interpolate(expr)
         return res
 
     def __neg__(self):
-        res = SimResult(
+        res = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         if self.vout is not None:
@@ -402,15 +392,15 @@
     def __add__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(self.vout + b.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(self.vout + b, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
@@ -420,15 +410,15 @@
     def __sub__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(self.vout - b.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(self.vout - b, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
@@ -438,15 +428,15 @@
     def __mul__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(self.vout * b.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(self.vout * b, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
@@ -456,15 +446,15 @@
     def __radd__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(b.vout + self.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(b + self.vout, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
@@ -474,15 +464,15 @@
     def __rsub__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(b.vout - self.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(b - self.vout, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
@@ -492,15 +482,15 @@
     def __rmul__(self, b):
         if is_sim_res(b):
             self.aline_V(b)
             expr = Expression(b.vout * self.vout, self.V.element.interpolation_points())
         else:
             expr = Expression(b * self.vout, self.V.element.interpolation_points())
 
-        C = SimResult(
+        C = FEMResults(
             mesh_file=self.mesh_file,
             V=self.V,
             domain=self.domain,
             elem=self.elem,
             comm=self.comm,
         )
         C.vout = Function(self.V)
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/MshCreator.py` & `nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/MshCreator.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,16 +69,18 @@
         self.volumes_com = []
         self.volumes_bd = []
 
         self.faces = []
         self.faces_com = []
         self.faces_bd = []
 
-        self.N_domains = 0
-        self.domains = []
+        self.id_domains = np.array([], dtype=int)
+        self.dim_domains = np.array([], dtype=int)
+        self.name_domain = []
+
         self.file = ""
 
         self.Nfeild = 0
         self.res = 1
 
         clear_gmsh()
         gmsh.initialize()
@@ -100,15 +102,14 @@
             gmsh.option.set_number("Mesh.Algorithm3D", 10)
         else:
             gmsh.option.set_number("Mesh.Algorithm3D", 1)
 
     #####################
     ## special methods ##
     #####################
-
     def get_obj(self):
         """
         update and return list of mesh entities
 
         Returns
         -------
         self.entities       :dict
@@ -356,19 +357,19 @@
     def add_cylinder(self, x=0, y=0, z=0, L=5, R=1):
         """
         add a x-oriented cylinder to mesh entities
 
         Parameters
         ----------
         x       : float
-            x position of the first face center
+            x position of the x-min face center
         y       : float
-            y position of the first face center
+            y position of the x-min face center
         z       : float
-            z position of the first face center
+            z position of the x-min face center
         L       : float
             Cylinder length along x
         R       : float
             Cylinder radius
 
         Returns
         -------
@@ -387,14 +388,55 @@
                 "dim": 3,
             }
             return cyl
         else:
             rise_warning("Not added : add_cylinder requiere 3D mesh")
             return None
 
+    def add_cone(self, x=0, y=0, z=0, L=5, R1=1, R2=0):
+        """
+        add a x-oriented cone to mesh entities
+
+        Parameters
+        ----------
+        x       : float
+            x position of the x-min face center.
+        y       : float
+            y position of the x-min face center.
+        z       : float
+            z position of the x-min face center.
+        L       : float
+            Cone length along x.
+        R1       : float
+            Cone x-min face radius.
+        R2       : float
+            Cone x-max face radius.
+
+        Returns
+        -------
+        cone    : int
+            id of the added object
+        """
+        if self.D == 3:
+            parameters = {"x": x, "y": y, "z": z, "L": L, "R1": R1, "R2":R2}
+            cone = self.model.occ.addCone(x, y, z, L, 0, 0, R1, R2)
+            self.model.occ.synchronize()
+            bounds = self.model.getEntities(dim=2)[-3:]
+            self.entities[cone] = {
+                "type": "cone",
+                "parameters": parameters,
+                "bounds": bounds,
+                "dim": 3,
+            }
+            return cone
+        else:
+            rise_warning("Not added : add_cylinder requiere 3D mesh")
+            return None
+
+
     def rotate(self, volume, angle, x=0, y=0, z=0, ax=0, ay=0, az=0, rad=True):
         """
         rotate volume
 
         Parameters
         ----------
         volume      : int
@@ -482,19 +524,38 @@
             path and name of saving file. If ends with ".msh" only save in ".msh" file
         """
         if not np.iterable(obj_IDs):
             obj_IDs = [obj_IDs]
         if dim is None:
             dim = max([self.entities[k]["dim"] for k in obj_IDs])
         self.model.addPhysicalGroup(dim, obj_IDs, phys_ID)
-
         if name is None:
-            name = "domain " + str(self.N_domains)
-
-        self.domains += (dim, phys_ID, name)
+            name = "domain " + str(self.n_domains)
+        self.id_domains = np.append(self.id_domains, phys_ID)
+        self.dim_domains = np.append(self.dim_domains, dim)
+        self.name_domain += [name]
+
+    @property
+    def n_domains(self):
+        return len(self.id_domains)
+
+    @property
+    def domains_1D(self):
+        I = np.where(self.dim_domains==1)
+        return self.id_domains[I]
+
+    @property
+    def domains_2D(self):
+        I = np.where(self.dim_domains==2)
+        return self.id_domains[I]
+
+    @property
+    def domains_3D(self):
+        I = np.where(self.dim_domains==3)
+        return self.id_domains[I]
 
     ##############################################################################################
     #######################################   feilds methods  ####################################
     ##############################################################################################
     def refine_entities(self, ent_ID, res_in, dim, res_out=None, IncludeBoundary=True):
         """
         refine mesh resolution in a list of faces or volumes IDs
@@ -620,16 +681,14 @@
             if self.Nfeild > 0:
                 self.model.mesh.field.setAsBackgroundMesh(self.Nfeild)
             else:
                 gmsh.option.setNumber("Mesh.CharacteristicLengthMin", 0.1 * self.res)
                 gmsh.option.setNumber("Mesh.CharacteristicLengthMax", self.res)
 
             self.model.occ.synchronize()
-
-            # print("nt:", gmsh.option.getNumber("General.NumThreads"))
             self.model.mesh.generate(self.D)
             self.is_generated = True
 
     def save(self, fname, generate=True):
         """
         Save mesh in fname in ".msh"
```

### Comparing `nrv-py-1.0.1/nrv/fmod/FEM/mesh_creator/NerveMshCreator.py` & `nrv_py-1.1.0/nrv/fmod/FEM/mesh_creator/NerveMshCreator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 NRV-:class:`.NerveMshCreator` handling.
 """
 from cmath import phase
 import numpy as np
+from math import log10, floor
 
-from ....backend.NRV_Class import NRV_class
+from ....backend.NRV_Class import NRV_class, load_any
 from ....backend.log_interface import rise_error, rise_warning
+from ....backend.MCore import MCH
+#from ....nmod.myelinated import myelinated
 from ....utils.units import mm
 from ....backend.file_handler import rmv_ext
 from .MshCreator import MshCreator, pi
 
 ENT_DOM_offset = {
     "Volume": 0,
     "Surface": 1,
@@ -191,22 +194,23 @@
         NRV_class.load(self, data, **kwargs)
         self.electrodes = {int(k): v for k, v in self.electrodes.items()}
         self.fascicles = {int(k): v for k, v in self.fascicles.items()}
         self.axons = {int(k): v for k, v in self.axons.items()}
         if self.is_generated and self.file != "":
             super().load(self.file)
 
-    def compute_mesh(self):
+    def compute_mesh(self, master_only=True):
         """
         Compute mesh geometry, domains and resolution and then generate the mesh
         """
-        self.compute_geo()
-        self.compute_domains()
-        self.compute_res()
-        self.generate()
+        if  MCH.do_master_only_work() or not master_only:
+            self.compute_geo()
+            self.compute_domains()
+            self.compute_res()
+            self.generate()
 
     def set_gnd_facet(self, outfacet=None, lfacet=None, rfacet=None):
         """
         Set which of the outer facet should be the ground (element 1)
 
         Parameters
         ----------
@@ -238,23 +242,22 @@
         """
         if not self.is_geo:
             if self.is_outer:
                 self.add_cylinder(0, self.y_c, self.z_c, self.L, self.Outer_D / 2)
                 if self.default_res["Outerbox_tresholded"]:
                     self.Ox = self.add_line((0, 0, 0), (self.L, 0, 0))
             self.add_cylinder(0, self.y_c, self.z_c, self.L, self.Nerve_D / 2)
-            for i in self.fascicles:
-                fascicle = self.fascicles[i]
+
+            for fascicle in self.fascicles.values():
                 self.add_cylinder(
-                    0, fascicle["y_c"], fascicle["z_c"], self.L, fascicle["D"] / 2
+                    0, fascicle["y_c"], fascicle["z_c"], self.L, fascicle["d"] / 2
                 )
-
             for i in self.axons:
-                axon = self.axons[i]
-                self.add_cylinder(0, axon["y_c"], axon["z_c"], self.L, axon["D"] / 2)
+                self.add_axon(i)
+
             for i in self.electrodes:
                 electrode = self.electrodes[i]
                 if "CUFF MP" in electrode["type"]:
                     self.add_CUFF_MP(ID=i, **electrode["kwargs"])
                 elif "CUFF MEA" in electrode["type"]:
                     self.add_CUFF_MEA(ID=i, **electrode["kwargs"])
                 elif "CUFF" in electrode["type"]:
@@ -322,21 +325,21 @@
 
         if not res == "default":
             self.default_res["Nerve"] = res
 
         if self.default_res["Nerve"] > self.Nerve_D / 5:
             self.default_res["Nerve"] = self.Nerve_D / 5
 
-    def reshape_fascicle(self, D, y_c=0, z_c=0, ID=None, res="default"):
+    def reshape_fascicle(self, d, y_c=0, z_c=0, ID=None, res="default"):
         """
         Reshape a fascicle of the FEM simulation
 
         Parameters
         ----------
-        Fascicle_D  : float
+        d  : float
             Fascicle diameter, in um
         y_c         : float
             Fascicle center y-coodinate in um, 0 by default
         z_c         : float
             Fascicle center y-coodinate in um, 0 by default
         ID          : int
             If the simulation contains more than one fascicles, ID number of the fascicle to reshape as in COMSOL
@@ -346,21 +349,21 @@
                 ID = 0
                 while ID in self.fascicles:
                     ID += 1
             self.N_fascicle += 1
 
         if res == "default":
             res = self.default_res["Fascicle"]
-        if D / 5 < res:
-            res = D / 5
+        if d / 5 < res:
+            res = d / 5
 
         self.fascicles[ID] = {
             "y_c": y_c,
             "z_c": z_c,
-            "D": D,
+            "d": d,
             "res": res,
             "face": None,
             "volume": None,
         }
 
     def remove_fascicles(self, ID=None):
         """
@@ -374,21 +377,21 @@
         if ID is None:
             self.fascicles = {}
             self.N_fascicle = 0
         elif ID in self.fascicles:
             del self.fascicles[ID]
             self.N_fascicle -= 1
 
-    def reshape_axon(self, D, y_c=0, z_c=0, ID=None, res="default"):
+    def reshape_axon(self, d, y=0, z=0, ID=None, myelinated=False, res="default", res_node="default",**kwargs):
         """
         Reshape a axon of the FEM simulation
 
         Parameters
         ----------
-        Fascicle_D  : float
+        d  : float
             Fascicle diameter, in um
         y_c         : float
             Fascicle center y-coodinate in um, 0 by default
         z_c         : float
             Fascicle center y-coodinate in um, 0 by default
         ID          : int
             If the simulation contains more than one fascicles, ID number of the fascicle to reshape as in COMSOL
@@ -398,25 +401,30 @@
                 ID = 0
                 while ID in self.axons:
                     ID += 1
             self.N_axon += 1
 
         if res == "default":
             res = self.default_res["Axon"]
-        if D / 3 < res:
-            res = D / 3
-
-        self.axons[ID] = {
-            "y_c": y_c,
-            "z_c": z_c,
-            "D": D,
+        if d / 3 < res:
+            res = d / 3
+        if res_node == "default":
+            res_node = res / 3
+
+        self.axons[ID] = kwargs
+        self.axons[ID].update({
+            "y": y,
+            "z": z,
+            "d": d,
+            "myelinated": myelinated,
             "res": res,
-            "face": None,
-            "volume": None,
-        }
+            "res_node": res_node,
+            "face": [],
+            "volume": [],
+        })
 
     def add_electrode(self, elec_type, ID=None, res="default", **kwargs):
         """ """
         if elec_type not in ELEC_TYPES + ["CUFF MEA"]:
             rise_warning(
                 elec_type
                 + " not implemented, electrode will not be added\nList of Electrode types: "
@@ -435,33 +443,33 @@
                         ID += 1
             self.N_electrode += 1
 
         if res == "default":
             res = self.default_res["Electrode"]
 
         if "LIFE" in elec_type:
-            if "D" in kwargs:
-                D = kwargs["D"]
+            if "d" in kwargs:
+                d = kwargs["d"]
             else:
-                D = 25
-            if D / 3 < res:
-                res = D / 3
+                d = 25
+            if d / 3 < res:
+                res = d / 3
 
         self.electrodes[ID] = {"type": elec_type, "res": res, "kwargs": kwargs}
 
     ####################################################################################################
     #####################################   domains definition  ########################################
     ####################################################################################################
 
     def compute_domains(self):
         if not self.is_geo:
             rise_error("compute geometry before domain")
         elif not self.is_dom:
-            self.__link_entity_domains(2)
-            self.__link_entity_domains(3)
+            self.__link_entity_domains(dim=2)
+            self.__link_entity_domains(dim=3)
             self.compute_entity_domain()
             self.is_dom = True
 
     def __is_outerbox(self, dx, dy, dz, com, dim_key):
         """
         Internal use only: check if volume is the box or face is external face of box
 
@@ -522,24 +530,64 @@
         dim_key     :"face" or "volume"
             element type
         """
         fascicle = self.fascicles[ID]
         # Already computed
         status_test = fascicle[dim_key] is None
         # test good diameter
-        size_test = np.allclose([dx, dy, dz], [self.L, fascicle["D"], fascicle["D"]])
+        size_test = np.allclose([dx, dy, dz], [self.L, fascicle["d"], fascicle["d"]])
         # test center of mass in fascicle
         com_test = np.allclose(
             com,
             (self.L / 2, fascicle["y_c"], fascicle["z_c"]),
             rtol=1,
-            atol=fascicle["D"] / 2,
+            atol=fascicle["d"] / 2,
         )
         return status_test and size_test and com_test
 
+
+    def __is_axon_node(self, ID, dx, dy, dz, com, dim_key):
+        """
+        Internal use only: check if volume is axon ID or face is external face of axon ID
+
+        Parameters
+        ----------
+        ID          :int
+            ID of axon to test
+        dx          : float
+            length along x of the entity boundbox
+        dy          : float
+            length along y of the entity boundbox
+        dz          : float
+            length along z of the entity boundbox
+        com         : tupple(float)
+            entity Center of Mass
+        dim_key     :"face" or "volume"
+            element type
+        """
+        axon = self.axons[ID]
+        # Already computed
+        if not axon["myelinated"]:
+            return False
+        
+        # test good diameter
+        size_test = np.allclose([dx, dy, dz], [axon["node_l"], axon["node_d"], axon["node_d"]])
+
+        # test first and last node
+        if "first_node_l" in axon and not size_test:
+            size_test = np.allclose([dx, dy, dz], [axon["first_node_l"], axon["node_d"], axon["node_d"]])
+        if "last_node_l" in axon and not size_test:
+            size_test = np.allclose([dx, dy, dz], [axon["last_node_l"], axon["node_d"], axon["node_d"]])
+
+        # test center of mass in axon
+        com_test = np.allclose(
+            com[1:], (axon["y"], axon["z"])
+        )
+        return size_test and com_test
+
     def __is_axon(self, ID, dx, dy, dz, com, dim_key):
         """
         Internal use only: check if volume is axon ID or face is external face of axon ID
 
         Parameters
         ----------
         ID          :int
@@ -553,20 +601,21 @@
         com         : tupple(float)
             entity Center of Mass
         dim_key     :"face" or "volume"
             element type
         """
         axon = self.axons[ID]
         # Already computed
-        status_test = axon[dim_key] is None
+        status_test = True#axon[dim_key] is None
         # test good diameter
-        size_test = np.allclose([dx, dy, dz], [self.L, axon["D"], axon["D"]])
+        size_test = np.allclose([dy, dz], [axon["d"], axon["d"]])
+        size_test &= not np.isclose(dx, 0)
         # test center of mass in axon
         com_test = np.allclose(
-            com, (self.L / 2, axon["y_c"], axon["z_c"]), rtol=1, atol=axon["D"] / 2
+            com[1:], (axon["y"], axon["z"]), atol=axon["d"] / 2
         )
         return status_test and size_test and com_test
 
     def __is_CUFF_MP_electrode(self, ID, rc, dx, teta, com, dim_key):
         """
         Internal use only: check if volume is electrode ID or face is external face of fascicle ID
 
@@ -646,21 +695,21 @@
         """
 
         elec_kwargs = self.electrodes[ID]["kwargs"]
         if self.electrodes[ID]["type"] != "LIFE":
             return False
         # test good diameter
         size_test = np.allclose(
-            [dx, dy, dz], [elec_kwargs["length"], elec_kwargs["D"], elec_kwargs["D"]]
+            [dx, dy, dz], [elec_kwargs["length"], elec_kwargs["d"], elec_kwargs["d"]]
         )
         # test center of mass in LIFE
         com_test = np.allclose(
             com,
             (elec_kwargs["x_c"], elec_kwargs["y_c"], elec_kwargs["z_c"]),
-            atol=elec_kwargs["D"] / 2,
+            atol=elec_kwargs["d"] / 2,
         )
         return size_test and com_test
 
     def __link_entity_domains(self, dim):
         """
         Internal use only: link all entities from
 
@@ -695,16 +744,19 @@
                 self.Nerve_entities[key] += [entities[i][1]]
 
             for j in self.fascicles:
                 if self.__is_fascicle(j, bd_x, bd_y, bd_z, ent_com[i], key):
                     self.fascicles[j][key] = entities[i][1]
 
             for j in self.axons:
-                if self.__is_axon(j, bd_x, bd_y, bd_z, ent_com[i], key):
-                    self.axons[j][key] = entities[i][1]
+                if self.__is_axon_node(j, bd_x, bd_y, bd_z, ent_com[i], key):
+                    node_id = int(ent_com[i][0] // self.axons[j]["deltax"])
+                    self.axons[j]["nodes_"+key][node_id] = [entities[i][1]]
+                elif self.__is_axon(j, bd_x, bd_y, bd_z, ent_com[i], key):
+                    self.axons[j][key] += [entities[i][1]]
 
             for j in self.electrodes:
                 r_c = (
                     (ent_com[i][1] - self.y_c) ** 2 + (ent_com[i][2] - self.z_c) ** 2
                 ) ** 0.5
                 teta = phase(
                     complex(ent_com[i][2] - self.z_c, ent_com[i][1] - self.y_c)
@@ -760,19 +812,30 @@
                 id_ph += ENT_DOM_offset["Surface"]
                 self.add_domains(
                     obj_IDs=self.fascicles[j]["face"], phys_ID=id_ph, dim=2
                 )
             else:
                 rise_warning("Too much Fascicles: " + str(j) + " not added")
 
-        for j in self.axons:
+        for j, ax in self.axons.items():
             id_ph = ENT_DOM_offset["Axon"] + (2 * j)
-            self.add_domains(obj_IDs=self.axons[j]["volume"], phys_ID=id_ph, dim=3)
+            self.add_domains(obj_IDs=ax["volume"], phys_ID=id_ph, dim=3)
             id_ph += ENT_DOM_offset["Surface"]
-            self.add_domains(obj_IDs=self.axons[j]["face"], phys_ID=id_ph, dim=2)
+            self.add_domains(obj_IDs=ax["face"], phys_ID=id_ph, dim=2)
+            # adding one physical domain by node
+            if ax["myelinated"]:
+                for i_node in range(len(ax["nodes_volume"])):
+                    node_id = 2 * i_node
+                    n = floor(log10(node_id+1)+1)
+                    ax_id = (ENT_DOM_offset["Axon"] + (2 * j)) * 10**n
+                    id_ph = node_id + ax_id
+                    self.add_domains(obj_IDs=ax["nodes_volume"][i_node], phys_ID=id_ph, dim=3)
+                    id_ph += ENT_DOM_offset["Surface"]
+                    self.add_domains(obj_IDs=ax["nodes_face"][i_node], phys_ID=id_ph, dim=2)
+
 
         for j in self.electrodes:
             id_ph = ENT_DOM_offset["Electrode"] + (2 * j)
             if id_ph < ENT_DOM_offset["Axon"]:
                 if "CUFF MP" in self.electrodes[j]["type"]:
                     for ID_EA in range(self.electrodes[j]["kwargs"]["N"]):
                         if self.electrodes[j]["kwargs"]["is_volume"]:
@@ -821,41 +884,30 @@
                     res_in=self.default_res["Nerve"],
                     dim=3,
                     res_out=None,
                     IncludeBoundary=True,
                 )
             ]
             # Facsicle fields
-            for j in self.fascicles:
-                fascicle = self.fascicles[j]
+            for fascicle in self.fascicles.values():
                 fields += [
                     self.refine_entities(
                         ent_ID=fascicle["volume"],
                         res_in=fascicle["res"],
                         dim=3,
                         res_out=None,
                         IncludeBoundary=True,
                     )
                 ]
             # Axon fields
-            for j in self.axons:
-                axon = self.axons[j]
-                fields += [
-                    self.refine_entities(
-                        ent_ID=axon["volume"],
-                        res_in=axon["res"],
-                        dim=3,
-                        res_out=None,
-                        IncludeBoundary=True,
-                    )
-                ]
-            # Electrodes fields
-            for j in self.electrodes:
-                electrode = self.electrodes[j]
+            for axon in self.axons.values():
+                fields += self.__refine_axon(axon)
 
+            # Electrodes fields
+            for electrode in self.electrodes.values():
                 if electrode["type"] in ["CUFF MEA", "CUFF MP"]:
                     for ID_EA in range(electrode["kwargs"]["N"]):
                         fields += [
                             self.refine_entities(
                                 ent_ID=electrode["volume"][ID_EA],
                                 res_in=electrode["res"],
                                 dim=3,
@@ -869,18 +921,46 @@
                             ent_ID=electrode["volume"],
                             res_in=electrode["res"],
                             dim=3,
                             res_out=None,
                             IncludeBoundary=True,
                         )
                     ]
-
             self.refine_min(fields)
             self.is_refined = True
 
+    def __refine_axon(self, axon):
+        """
+        
+        """
+        # First set the field for unmyelinated axon or myeline
+        fields = [
+            self.refine_entities(
+                ent_ID=axon["volume"],
+                res_in=axon["res"],
+                dim=3,
+                res_out=None,
+                IncludeBoundary=True,
+            )
+        ]
+        # Then set the field for myelinated axon nodes
+        if axon["myelinated"]:
+            for i in range(len(axon["nodes_volume"])):
+                fields += [
+                    self.refine_entities(
+                        ent_ID=axon["nodes_volume"][i],
+                        res_in=axon["res_node"],
+                        dim=3,
+                        res_out=None,
+                        IncludeBoundary=True,
+                    )
+                ]
+        return fields
+
+
     def __refine_Outer_box(self, alpha=0.1):
         """ """
         if not self.default_res["Outerbox_tresholded"]:
             field = [
                 self.refine_entities(
                     ent_ID=self.Outer_entities["volume"],
                     res_in=self.default_res["Outerbox"],
@@ -900,20 +980,98 @@
                     res_max=self.default_res["Outerbox"],
                     dist_min=self.Nerve_D,
                     dist_max=dmax,
                 )
             ]
         return field
 
-    ####################################################################################################
-    ###################################   electrodes definition  #######################################
-    ####################################################################################################
+    ################################################################
+    ############## complex volumes adding methods ##################
+    ################################################################
+    def add_axon(self, ID):
+        """
+        Add an axon to the mesh.
+
+        Note
+        ----
+         - if the axon is unmyelinated this method add only a cylinder to the mesh
+        
+        Parameters
+        ----------
+        """
+        axon = self.axons[ID]
+        res_min = axon["res_node"]
+        if not axon["myelinated"]:
+            self.add_cylinder(0, axon["y"], axon["z"], self.L, axon["d"]/2)
+        else:
+            axon.update({
+                "L": self.L,
+                "rec":"all",
+                "N_seg_per_sec":True,
+                "__NRVObject__":True,
+                "nrv_type":"myelinated",
+            })
+            # Ideally it would be easier to use: ax = myelinated(**axon)
+            # But myelinated cannot be imported without causing an import loop
+            ax = load_any(data=axon)
+            x = ax.first_section_size
+            init_l = 0
+            n_nodes = 0
+            for sec in ax.axon_path_type[1:-1]:
+                if sec == "node":
+                    r_sec = ax.nodeD/2
+                    l_sec = ax.nodelength
+                    n_nodes += 1
+                else:
+                    r_sec = ax.d/2
+                    if sec == "MYSA":
+                        l_sec = ax.paralength1
+                    elif sec == "FLUT":
+                        l_sec = ax.paralength2
+                    elif sec == "STIN":
+                        l_sec = ax.interlength
+
+                # mrege the first (last) section with the next (previous) when it is too small
+                if  abs(x - l_sec) < res_min:
+                    init_l += l_sec
+                    ax.axon_path_type.pop(0)
+                    x += l_sec
+                elif abs(self.L - (l_sec + x)) < res_min:
+                    ax.axon_path_type.pop(-1)
+                else:
+                    self.add_cylinder(x, ax.y, ax.z, l_sec, r_sec)
+                    x += l_sec
+            # adding first section
+            if ax.axon_path_type[0] == "node":
+                r_sec = ax.nodeD/2
+                n_nodes += 1
+                self.axons[ID]["first_node_l"] = ax.first_section_size + init_l
+            else:
+                r_sec = ax.d/2
+            self.add_cylinder(0, ax.y, ax.z, ax.first_section_size + init_l, r_sec)
+            # adding first section
+            if ax.axon_path_type[-1] == "node":
+                r_sec = ax.nodeD/2
+                n_nodes += 1
+                self.axons[ID]["last_node_l"] = self.L-x
+            else:
+                r_sec = ax.d/2
+            self.add_cylinder(x, ax.y, ax.z, self.L-x, r_sec)
+
+            self.axons[ID]["node_d"] = ax.nodeD
+            self.axons[ID]["node_l"] = ax.nodelength
+            self.axons[ID]["deltax"] = ax.deltax
+            self.axons[ID]["n_nodes"] = n_nodes
+            self.axons[ID]["nodes_volume"] = [None for _ in range(n_nodes)]
+            self.axons[ID]["nodes_face"] = [None for _ in range(n_nodes)]
+            del ax
+
 
     def add_LIFE(
-        self, ID=None, x_c=0, y_c=0, z_c=0, length=1000, D=25, is_volume=False
+        self, ID=None, x_c=0, y_c=0, z_c=0, length=1000, d=25, is_volume=False
     ):
         """
         Add LIFE electrode to the mesh
 
         Parameters
         ----------
         ID          :int
@@ -922,29 +1080,29 @@
             x-position of the LIFE center in um, by default 0
         y_c         :float
             y-position of the LIFE center in um, by default 0
         z_c         :float
             z-position of the LIFE center in um, by default 0
         length      :float
             length of the LIFE electrod in um, by default 1000
-        D           :float
+        d           :float
             diameter of the LIFE electrod in um, by default 25
         is_volume   : bool
             if True in cylinder of the LIFE is kept on the mesh
 
         """
 
         if ID is not None:
             self.electrodes[ID]["volume"] = []
             self.electrodes[ID]["face"] = []
             self.electrodes[ID]["kwargs"]["is_volume"] = is_volume
         x_active = x_c - length / 2
         y_active = y_c
         z_active = z_c
-        self.add_cylinder(x_active, y_active, z_active, length, D / 2)
+        self.add_cylinder(x_active, y_active, z_active, length, d / 2)
 
     def add_CUFF(
         self,
         ID=None,
         x_c=0,
         contact_length=100,
         is_volume=True,
@@ -993,16 +1151,16 @@
         if ID is not None:
             self.electrodes[ID]["kwargs"]["contact_length"] = contact_length
             self.electrodes[ID]["kwargs"]["contact_thickness"] = contact_thickness
             self.electrodes[ID]["kwargs"]["is_volume"] = is_volume
             self.electrodes[ID]["kwargs"]["insulator_offset"] = insulator_offset
             self.electrodes[ID]["volume"] = []
             self.electrodes[ID]["face"] = []
-            if contact_length / 3 < self.electrodes[ID]["res"]:
-                self.electrodes[ID]["res"] = contact_length / 2
+            if self.electrodes[ID]["res"] > min(contact_length, insulator_thickness) / 2:
+                self.electrodes[ID]["res"] = min(contact_length, insulator_thickness) / 2
 
         x_active = x_c - contact_length / 2
         y_active = self.y_c
         z_active = self.z_c
         cyl_act = self.add_cylinder(
             x_active,
             y_active,
```

### Comparing `nrv-py-1.0.1/nrv/fmod/electrodes.py` & `nrv_py-1.1.0/nrv/fmod/electrodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 NRV-:class:`.electrode` handling.
 """
 import faulthandler
 
 import numpy as np
+import matplotlib.pyplot as plt
 
 from ..backend.file_handler import json_load
 from ..backend.log_interface import rise_error, rise_warning
-from ..backend.NRV_Class import NRV_class
+from ..backend.NRV_Class import NRV_class, abstractmethod
 
 # enable faulthandler to ease "segmentation faults" debug
 faulthandler.enable()
 
 
 def is_FEM_electrode(elec):
     """
@@ -111,15 +112,15 @@
     return False
 
 
 class electrode(NRV_class):
     """
     Objet for generic electrode description. Each electrode has an ID and a position.
     """
-
+    @abstractmethod
     def __init__(self, ID=0):
         """
         Instantiation of a generic electrode
 
         Parameters
         ----------
         ID  : int
@@ -160,15 +161,15 @@
         Parameters
         ----------
         ID  : int
             electrode identification number
         """
         self.ID = ID
 
-    def get_footptint(self):
+    def get_footprint(self):
         """
         get the footprint of a electrode
 
         Returns
         -------
         footprint : np.array
             identification number of the electrode
@@ -228,21 +229,28 @@
             self.x += x
         if y is not None:
             self.y += y
         if z is not None:
             self.z += z
         self.clear_footprint()
 
+    @abstractmethod
+    def plot(
+        self, axes:plt.axes, color:str="gold",**kwgs
+    )->None:
+        pass
+
+
+
 
 class point_source_electrode(electrode):
     """
     Point source electrode. Inherite from electrode. The electrode is punctual and act as a\
     monopole.
     """
-
     def __init__(self, x=0, y=0, z=0, ID=0):
         """
         Instantiation of a Point source electrode
 
         Parameters
         ----------
         x   : float
@@ -299,20 +307,25 @@
                 * np.sqrt(
                     sx * (1e-6 * (self.x - x)) ** 2
                     + sy * (1e-6 * (self.y - y)) ** 2
                     + sz * (1e-6 * (self.z - z)) ** 2
                 )
             )
 
+    def plot(self, axes: plt.axes, color: str="gold", **kwgs) -> None:
+        if ("nerve_d" in kwgs):
+            del kwgs["nerve_d"]
+        axes.plot(self.y, self.z, ".", color=color, **kwgs)
+
 
 class FEM_electrode(electrode):
     """
     Electrode located in Finite Element Model in Comsol
     """
-
+    @abstractmethod
     def __init__(self, label, ID=0):
         """
         Instrantiation of a FEM electrode
         """
         super().__init__(ID)
         self.label = label
         self.ID = ID
@@ -327,15 +340,14 @@
         Parameters:
         -----------
         V_1mA : list, array, numpy array
             Voltage response at 1mA
         """
         self.footprint = np.asarray(V_1mA)
 
-
 class LIFE_electrode(FEM_electrode):
     """
     Longitudinal IntraFascicular Electrode for FEM models
     """
 
     def __init__(
         self,
@@ -391,19 +403,27 @@
         else:
             model.add_electrode(
                 elec_type=self.type,
                 x_c=self.x + (self.length / 2),
                 y_c=self.y,
                 z_c=self.z,
                 length=self.length,
-                D=self.D,
+                d=self.D,
                 is_volume=self.is_volume,
                 res=res,
             )
 
+    def plot(self, axes: plt.axes, color: str="gold", **kwgs) -> None:
+        axes.add_patch(plt.Circle(
+            (self.y, self.z),
+            self.D / 2,
+            color=color,
+            fill=True,
+        ))
+
 
 class CUFF_electrode(FEM_electrode):
     """
     CUFF electrode for FEM models
     """
 
     def __init__(
@@ -424,15 +444,14 @@
 
         Parameters
         ----------
         label               : str
             name of the electrode in the COMSOL file
         x_center            :float
             x-position of the CUFF center in um, by default 0
-            length of the CUFF electrod in um, by default 100
         contact_length      :float
             length along x of the contact site in um, by default 100
         is_volume   : bool
             if True the contact is kept on the mesh as a volume, by default True
         contact_thickness   :float
             thickness of the contact site in um, by default 5
         insulator            :bool
@@ -507,14 +526,28 @@
                 contact_length=self.contact_length,
                 contact_thickness=self.contact_thickness,
                 insulator_offset=self.insulator_offset,
                 x_c=self.x,
                 res=res,
             )
 
+    def plot(self, axes: plt.axes, color: str = "gold", **kwgs) -> None:
+        if "nerve_d" in kwgs:
+            rad = kwgs["nerve_d"] / 2
+            del kwgs["nerve_d"]
+            axes.add_patch(plt.Circle(
+                (0, 0),
+                rad,
+                color=color,
+                fill=False,
+                linewidth=2,
+                **kwgs
+            ))
+        else:
+            rise_warning("Diameter has to be specifie to plot CUFF electrodes")
 
 class CUFF_MP_electrode(CUFF_electrode):
     """
     MultiPolar CUFF electrode for FEM models
     """
 
     def __init__(
@@ -596,7 +629,27 @@
                 contact_length=self.contact_length,
                 insulator=self.insulator,
                 contact_thickness=self.contact_thickness,
                 x_c=self.x,
                 insulator_offset=self.insulator_offset,
                 res=res,
             )
+
+    def plot(self, axes: plt.axes, color: str = "gold", **kwgs) -> None:
+        if "nerve_d" in kwgs:
+            rad = kwgs["nerve_d"] / 2
+            del kwgs["nerve_d"]
+            elec_theta = 0.9 * 2 * np.pi / self.N_contact
+            for i in range(self.N_contact):
+                theta_ = 2 * i * np.pi / self.N_contact
+                axes.add_patch(plt.Wedge(
+                    (0, 0),
+                    rad,
+                    theta1 = theta_,
+                    theta2 = theta_ + elec_theta,
+                    color=color,
+                    fill=False,
+                    linewidth=2,
+                    **kwgs
+                ))
+        else:
+            rise_warning("Diameter has to be specifie to plot CUFF MP electrodes")
```

### Comparing `nrv-py-1.0.1/nrv/fmod/extracellular.py` & `nrv_py-1.1.0/nrv/fmod/extracellular.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 NRV-:class:`.extracellular_context` handling.
 """
 import faulthandler
 
 import numpy as np
+import matplotlib.pyplot as plt
 
 from ..backend.file_handler import json_load
 from ..backend.log_interface import rise_error, rise_warning
 from ..backend.MCore import MCH
 from ..backend.NRV_Class import NRV_class, is_empty_iterable
+from ..utils.misc import get_perineurial_thickness
 from .electrodes import (
     is_analytical_electrode,
     is_FEM_electrode,
     check_electrodes_overlap,
 )
 from .FEM.COMSOL_model import COMSOL_model, COMSOL_Status
 from .FEM.FENICS_model import FENICS_model
@@ -252,15 +254,15 @@
     def clear_electrodes_footprints(self):
         """
         clear the footprints for all electrodes from existing array
         """
         for electrode in self.electrodes:
             electrode.clear_footprint()
 
-    def change_stimulus_from_elecrode(self, ID_elec, stimulus):
+    def change_stimulus_from_electrode(self, ID_elec, stimulus):
         """
         Change the stimulus of the ID_elec electrods
 
         Parameters:
         -----------
             ID_elec  : int
                 ID of the electrode which should be changed
@@ -276,14 +278,19 @@
                 "Only",
                 len(self.stimuli),
                 "electrode in extracellular_context:",
                 ID_elec,
                 "is not too big",
             )
 
+    def plot(self, axes: plt.axes, color: str = "gold", **kwgs) -> None:
+        for electrode in self.electrodes:
+            electrode.plot(axes, color , **kwgs)
+
+
 
 class stimulation(extracellular_context):
     """
     Stimulation object are designed to connect all other objects requierd to analyticaly compute the external potential voltage for axons :
     - the material surrounding the axon (only one)
     - a list of electrode(s)
     - a list of corresponding current stimuli
@@ -346,46 +353,47 @@
             electrode.compute_footprint(
                 np.asarray(x), np.asarray(y), np.asarray(z), self.material
             )
 
 
 class FEM_stimulation(extracellular_context):
     """
-    FEM_based_simulation object are designed to connect all other objects requierd to compute the external potential voltage for axons using FEM :
+    FEM_based_simulation object are designed to connect all other objects required to compute the external potential voltage for axons using FEM :
+
+    - Shape and positon of the nerve 
+    - Shape and position of each fascicle 
     - the materials for the FEM stimulation : endoneurium, perineurium, epineurium and external material
     - a list of electrode(s)
     - a list of corresponding current stimuli
+
+    Parameters
+    ----------
+    model_fname   : str
+        name of the comsol mph file to solve
+    endo_mat            : str
+        specification of the endoneurium material, see :class:`~nrv.fmod.materials.material` for further details
+    peri_mat            : str
+        specification of the perineurium material, see :class:`~nrv.fmod.materials.material` for further details
+    epi_mat             : str
+        specification of the epineurium material, see :class:`~nrv.fmod.materials.material` for further details
+    ext_mat             : str
+        specification of the external material (everything but the nerve), see :class:`~nrv.fmod.materials.material` for further details
     """
 
     def __init__(
         self,
         model_fname=None,
         endo_mat="endoneurium_ranck",
         peri_mat="perineurium",
         epi_mat="epineurium",
         ext_mat="saline",
         comsol=True,
         Ncore=None,
     ):
-        """
-        Implement a FEM_based_stimulation object.
 
-        Parameters
-        ----------
-        simuluation_fname   : str
-            name of the simluation file to compute the field
-        endo_mat            : material object
-            specification of the endoneurium material, see Material.py or material object help for further details
-        peri_mat            : material object
-            specification of the perineurium material, see Material.py or material object help for further details
-        epi_mat             : material object
-            specification of the epineurium material, see Material.py or material object help for further details
-        ext_mat             : material object
-            specification of the external material (everything but the nerve), see Material.py or material object help for further details
-        """
         super().__init__()
         self.electrodes_label = []
         self.model_fname = model_fname
         self.setup = False
         self.is_run = False
         self.Ncore = Ncore
         ## get material properties and add to model
@@ -475,14 +483,16 @@
         Parameters
         ----------
         data    : str or dict
             json file path or dictionary containing extracel_context information
         """
         super().load(data, **kwargs)
 
+        if self.fenics:
+            self.set_Ncore(self.Ncore)
         if C_model:
             if MCH.do_master_only_work():
                 self.model = COMSOL_model(self.model_fname)
             else:
                 # check that COMSOL is not turned OFF in order to continue
                 if not COMSOL_Status:
                     rise_warning(
@@ -503,28 +513,28 @@
         """
         if MCH.do_master_only_work():
             if self.comsol:
                 self.model.set_parameter("Outer_D", str(Outer_D) + "[mm]")
             else:
                 self.model.reshape_outerBox(Outer_D, res=res)
 
-    def reshape_nerve(self, Nerve_D, Length, y_c=0, z_c=0, res="default"):
+    def reshape_nerve(self, Nerve_D=None, Length=None, y_c=0, z_c=0, res="default"):
         """
         Reshape the nerve of the FEM simulation
 
         Parameters
         ----------
         Nerve_D                 : float
-            Nerve diameter, in um
+            Nerve diameter, in µm
         Length                  : float
-            Nerve length, in um
+            Nerve length, in µm
         y_c                     : float
-            Nerve center y-coordinate in um, 0 by default
+            Nerve center y-coordinate in µm, 0 by default
         z_c                     : float
-            Nerve z-coordinate center in um, 0 by default
+            Nerve z-coordinate center in µm, 0 by default
         res         : float or "default"
             mesh resolution for fenics_model cf NerveMshCreator, use with caution, by default "default"
         """
         if MCH.do_master_only_work():
             if self.comsol:
                 self.model.set_parameter("Nerve_D", str(Nerve_D) + "[um]")
                 self.model.set_parameter("Length", str(Length) + "[um]")
@@ -532,35 +542,36 @@
                 self.model.set_parameter("Nerve_z_c", str(z_c) + "[um]")
             else:
                 self.model.reshape_nerve(
                     Nerve_D=Nerve_D, Length=Length, y_c=y_c, z_c=z_c, res=res
                 )
 
     def reshape_fascicle(
-        self, Fascicle_D, y_c=0, z_c=0, ID=None, Perineurium_thickness=5, res="default"
+        self, Fascicle_D, y_c=0, z_c=0, ID=None, Perineurium_thickness=None, res="default"
     ):
         """
         Reshape a fascicle of the FEM simulation
 
         Parameters
         ----------
         Fascicle_D  : float
-            Fascicle diameter, in um
+            Fascicle diameter, in µm
         y_c         : float
-            Fascicle center y-coodinate in um, 0 by default
+            Fascicle center y-coodinate in µm, 0 by default
         z_c         : float
-            Fascicle center y-coodinate in um, 0 by default
+            Fascicle center y-coodinate in µm, 0 by default
         Perineurium_thickness   :float
-            Thickness of the Perineurium sheet surounding the fascicles in um, 5 by default
+            Thickness of the Perineurium sheet surounding the fascicles in µm. If None, thickness is determined according to the fascicle diameter 
         ID          : int
             If the simulation contains more than one fascicles, ID number of the fascicle to reshape as in COMSOL
         res         : float or "default"
             mesh resolution for fenics_model cf NerveMshCreator, use with caution, by default "default"
         """
         if MCH.do_master_only_work():
+            p_th = Perineurium_thickness or get_perineurial_thickness(Fascicle_D)
             if self.comsol:
                 if ID is None:
                     self.model.set_parameter("Fascicle_D", str(Fascicle_D) + "[um]")
                     self.model.set_parameter("Fascicle_y_c", str(y_c) + "[um]")
                     self.model.set_parameter("Fascicle_z_c", str(z_c) + "[um]")
                 else:
                     self.model.set_parameter(
@@ -569,23 +580,23 @@
                     self.model.set_parameter(
                         "Fascicle_" + str(ID) + "_y_c", str(y_c) + "[um]"
                     )
                     self.model.set_parameter(
                         "Fascicle_" + str(ID) + "_z_c", str(z_c) + "[um]"
                     )
                 self.model.set_parameter(
-                    "Perineurium_thickness", str(Perineurium_thickness) + "[um]"
+                    "Perineurium_thickness", str(p_th) + "[um]"
                 )
             else:
                 self.model.reshape_fascicle(
                     Fascicle_D=Fascicle_D,
                     y_c=y_c,
                     z_c=z_c,
                     ID=ID,
-                    Perineurium_thickness=Perineurium_thickness,
+                    Perineurium_thickness=p_th,
                     res=res,
                 )
 
     def remove_fascicles(self, ID=None):
         """
         remove a fascicle of the FEM simulation
 
@@ -611,15 +622,15 @@
             else
         """
         is_overlaping = False
         for elec in self.electrodes:
             is_overlaping = is_overlaping or check_electrodes_overlap(elec, electrode)
 
         if is_overlaping:
-            rise_warning("overlaping electrod: not added to context")
+            rise_warning("overlaping electrodes: not added to context")
         else:
             if is_FEM_electrode(electrode):
                 if not electrode.is_multipolar:
                     if not is_empty_iterable(self.electrodes):
                         electrode.set_ID_number(self.electrodes[-1].get_ID_number() + 1)
                     self.electrodes.append(electrode)
                     self.electrodes_label.append(electrode.label)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nrv-py-1.0.1/nrv/fmod/recording.py` & `nrv_py-1.1.0/nrv/fmod/recording.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/fmod/stimulus.py` & `nrv_py-1.1.0/nrv/fmod/stimulus.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import faulthandler
 
 import numpy as np
 
 from ..backend.log_interface import pass_info, rise_warning, rise_error
 from ..backend.NRV_Class import NRV_class
+import matplotlib.pyplot as plt
 
 # enable faulthandler to ease "segmentation faults" debug
 faulthandler.enable()
 
 
 ###############
 ## Functions ##
@@ -213,14 +214,25 @@
                 while i > j and not i_mask[i - j]:
                     j += 1
                 if self.t[i + 1] - self.t[i - j] < dt_min:
                     i_mask[i + 1] = False
         self.s = self.s[i_mask]
         self.t = self.t[i_mask]
 
+    def plot(self, ax:plt.axes, scatter=False, **ax_kwargs):
+        """
+        Plot the stimulus
+        """
+        if scatter:
+            ax.scatter(self.t, self.s, **ax_kwargs)
+        else:
+            ax.step(self.t, self.s, where="post", **ax_kwargs)
+
+
+
     #####################
     ## special methods ##
     #####################
     def __len__(self):
         return self.len()
 
     def __abs__(self):
@@ -366,26 +378,29 @@
 
         Parameters
         ----------
         start       : float
             starting time of the waveform, in ms
         s_cathod    : float
             cathodic (negative stimulation value) current, in uA
-            WARNING: always positive, the user give here the absolute value
         t_stim      : float
             stimulation time, in ms
         s_anod      : float
             anodic (positive stimulation value) current and, in uA
         t_inter     : float
             inter pulse timing, in ms
         anod_first  : bool
             if true, stimulation is anodic and begins with the anodic value
             and is balanced with cathodic value, else stimuation is cathodic
             and begins with the cathodic value and is balances with anodic value,
             by default set to False (cathodic first as most stimulation protocols)
+
+        WARNING
+        -------
+        `s_cathod` must always positive, the user give here the absolute value
         """
         if not anod_first:
             s_1 = -s_cathod
             s_2 = s_anod
         else:
             s_2 = -s_cathod
             s_1 = s_anod
@@ -418,17 +433,19 @@
             amplitude of the waveform, in uA
         freq        : float
             frequency of the waveform, in kHz
         offset      : float
             offset current of the waveform, in uA, by default set to 0
         phase       : float
             initial phase of the waveform, in rad, by default set to 0
-        dt          : float
-            sampling time period to generate the sinusoidal shape. If equal to 0,
-            dt is automatically set to match 100 samples per sinusoid period by default set to 0
+        anod_first  : bool
+            if true, stimulation is anodic and begins with the anodic value
+            and is balanced with cathodic value, else stimuation is cathodic
+            and begins with the cathodic value and is balances with anodic value,
+            by default set to False (cathodic first as most stimulation protocols)
         """
         # check the pseudo sampling period
         if dt == 0:
             dt = 1 / (freq * 100)
         elif freq > (1.0 / (2 * dt)):
             rise_warning(
                 "dt too low in stimulus creation, Shannon criterion not respected"
@@ -506,15 +523,15 @@
                 freq_harmonic = freq * (i + 2)
             s = s - np.max(s)  # shift s to avoid any postive values
             s = s * amplitude / np.max(np.abs(s))  # rescale s to finale amp
             s[-1] = 0
             t = np.linspace(start, start + t_pulse, num=Nb_points)
             self.concatenate(s, t, t_shift=0)
 
-    def square(self, start, duration, freq, amplitude, offset, dt):
+    def square(self, start, duration, freq, amplitude, offset, anod_first=False):
         """
         Create a repetitive (periodic) square waveform
 
         Parameters
         ----------
         start       : float
             starting time of the waveform, in ms
@@ -526,29 +543,25 @@
             frequency of the waveform, in kHz
         offset      : float
             offset current of the waveform, in uA, by default set to 0
         dt          : float
             sampling time period to generate the sinusoidal shape. If equal to 0,
             dt is automatically set to match 100 samples per sinusoid period by default set to 0
         """
-        Nb_points = int(duration / dt)
-        if start == 0:
-            Nb_points -= 1
-        T = 1 / freq
-        t = np.linspace(dt, start + duration, num=Nb_points)
-        s = np.ones(Nb_points)
-        point_start = int(start / dt)
-        for i in range(Nb_points):
-            if i < point_start:
-                s[i] = 0
-            else:
-                if t[i] % T < T / 2:
-                    s[i] = -s[i]
-                s[i] = amplitude * s[i] + offset
-        self.concatenate(s, t, t_shift=0)
+        Nb_pts = 2*int(duration / freq) - 1
+        dt = 1 / (2*freq)
+        t = np.linspace(0, duration, num=Nb_pts)
+        s = np.ones(Nb_pts)*amplitude
+        k_start = 0
+        if anod_first:
+            k_start = 1
+        for k in range(k_start, len(s), 2):
+            s[k]*=-1
+        s += offset
+        self.concatenate(s, t, t_shift=start)
 
     def ramp(
         self, slope, start, duration, dt, bounds=(0, float("inf")), printslope=False
     ):
         """
         Create a ramp waveform with slop value
```

### Comparing `nrv-py-1.0.1/nrv/nmod/axons.py` & `nrv_py-1.1.0/nrv/nmod/axons.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,20 +243,20 @@
         mesh_shape="plateau_sigmoid",
         alpha_max=0.3,
         d_lambda=0.1,
         v_init=None,
         T=None,
         ID=0,
         threshold=-40,
-        **kwarks,
+        **kwargs,
     ):
         """
         initialisation of the axon,
         """
-        super().__init__()
+        super().__init__(**kwargs)
         self.type = "axon"
         ## Given by user
         self.x = []
         self.y = y
         self.z = z
         self.d = d
         self.L = L
@@ -296,16 +296,16 @@
         self.record = False
         self.recorder = None
         ## abstract parameters
         self.x_rec = np.asarray([])
         self.rec = "all"
         self.node_index = None
         ## required for generate_axon_from_results
-        if "diameter" in kwarks:
-            self.d = kwarks["diameter"]
+        if "diameter" in kwargs:
+            self.d = kwargs["diameter"]
 
     def __del__(self):
         for section in neuron.h.allsec():
             section = None
         super().__del__()
 
     def __clear_reclists(self):
@@ -446,14 +446,31 @@
         extracel_context=False,
         intracel_context=False,
         rec_context=False,
     ):
         rise_warning("load_axon is a deprecated method use load")
         self.save(data, extracel_context, intracel_context, rec_context)
 
+    def plot(self, axes: plt.axes, color: str="blue", elec_color="gold", **kwgs) -> None:
+
+        alpha = 1
+        if "alpha" in kwgs:
+            alpha = kwgs["alpha"]
+
+        axes.add_patch(plt.Circle(
+            (self.y, self.z),
+            self.d / 2,
+            color=color,
+            fill=True,
+            alpha = alpha,
+        ))
+        if self.extra_stim is not None:
+            self.extra_stim.plot(axes=axes, color=elec_color, nerve_d=self.d)
+
+
     def __define_shape(self):
         """
         Define the shape of the axon after all sections creation
         """
         neuron.h.define_shape()
 
     def topology(self):
@@ -509,27 +526,27 @@
         ----------
         stim     : stimulation object
             see Extracellular.stimulation help for more details
         """
         if is_extra_stim(stim):
             self.extra_stim = stim
 
-    def change_stimulus_from_elecrode(self, ID_elec, stimulus):
+    def change_stimulus_from_electrode(self, ID_elec, stimulus):
         """
         Change the stimulus of the ID_elec electrods
 
         Parameters
         ----------
             ID_elec  : int
                 ID of the electrode which should be changed
             stimulus  : stimulus
                 New stimulus to set
         """
         if self.extra_stim is not None:
-            self.extra_stim.change_stimulus_from_elecrode(ID_elec, stimulus)
+            self.extra_stim.change_stimulus_from_electrode(ID_elec, stimulus)
         else:
             rise_warning("Cannot be changed: no extrastim in the axon")
 
     def get_electrodes_footprints_on_axon(
         self, save_ftp_only=False, filename="electrodes_footprint.ftpt"
     ):
         """
@@ -596,15 +613,15 @@
                 see unmyelinated/myelinated to see where recording occur
                 results stored with the key "V_mem"
         self.record_I_mem        : bool
             if true, the membrane current is recorded, set to False by default
         self.record_I_ions       : bool
             if true, the ionic currents are recorded, set to False by default
         record_particules   : bool
-            if true, the marticule states are recorded, set to False by default
+            if true, the particule states are recorded, set to False by default
         self.loaded_footprints           :dict or bool
             Dictionnary composed of extracellular footprint array, the keys are int value
             of the corresponding electrode ID, if None, footprints calculated during the simulation,
             set to None by default
 
         Returns
         -------
@@ -1085,18 +1102,18 @@
                         self.myelinated,
                     )
                     # compute extra-cellular potential and add it to already computed ones
                 self.recorder.set_time(axon_sim["t"])
                 self.recorder.add_axon_contribution(axon_sim["I_mem"], self.ID)
 
         except KeyboardInterrupt:
-            """rise_error(
-                "\n Caught KeyboardInterrupt, simulation stoped by user, stopping process..."
-            )"""
-            raise KeyboardInterrupt
+            rise_error(
+                KeyboardInterrupt,
+                "\n Caught KeyboardInterrupt, simulation stoped by user, stopping process...",
+            )
         except:
             axon_sim["Simulation_state"] = "Unsuccessful"
             axon_sim["Error_from_prompt"] = traceback.format_exc()
             rise_warning(
                 "Simulation induced an error while using neuron: \n"
                 + axon_sim["Error_from_prompt"]
             )
@@ -1170,15 +1187,15 @@
                 # save electrode positions
                 electrodes_x = []
                 electrodes_type = []
                 electrodes_y = []
                 electrodes_z = []
                 for electrode in self.extra_stim.electrodes:
                     if is_CUFF_electrode(electrode):
-                        electrodes_x.append(electrode.x_center)
+                        electrodes_x.append(electrode.x)
                         electrodes_y.append(0)
                         electrodes_z.append(0)
                         electrodes_type.append("CUFF")
                     else:
                         if is_LIFE_electrode(electrode):
                             electrodes_x.append(electrode.x + electrode.length / 2)
                             electrodes_type.append("LIFE")
```

### Comparing `nrv-py-1.0.1/nrv/nmod/fascicle_generator.py` & `nrv_py-1.1.0/nrv/nmod/axon_pop_generator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
-NRV-fascicule generator usefull functions.
+Axon population generator usefull functions.
 """
-import faulthandler
+import faulthandler 
 import math
 import os
+from tqdm import tqdm
 
 import matplotlib.pyplot as plt
-import numba
+from itertools import combinations
 import numpy as np
-from scipy import spatial, stats
 from scipy.optimize import curve_fit
-from scipy.stats import rv_continuous
+from scipy.stats import rv_continuous, gamma
 
-from ..backend.log_interface import pass_info, progression_popup
+from ..backend.log_interface import pass_info, progression_popup, rise_warning
 
 # WARNING:
 # no prompt message for numpy division by zeros: handled in the code !!!
 np.seterr(divide="ignore", invalid="ignore")
 
 # verbosity level
 fg_verbose = True
@@ -91,15 +91,15 @@
     c1      : float
         gain applied to the gamma function
 
     Note
     ----
     location of the gamma pdf function is fixed to 0.2, diameters will be interpolated above this minimal value.
     """
-    return c1 * (stats.gamma.pdf(x, a1, scale=1 / beta1, loc=0.2))
+    return c1 * (gamma.pdf(x, a1, scale=1 / beta1, loc=0.2))
 
 
 def two_Gamma(x, a1, beta1, c1, a2, beta2, c2, transition):
     """
     Gamma function, bi-modal, to interpolate myelinated statistics.
 
     Parameters
@@ -121,16 +121,16 @@
     transition  :float
         diameter value at the transition between the two lobes
 
     Note
     ----
     location of the gamma pdf first function is fixed to 2, diameters will be interpolated above this minimal value. This corresponds to the minimal A-delta diamter tolerated value.
     """
-    return c1 * (stats.gamma.pdf(x, a1, scale=1 / beta1, loc=2)) + c2 * (
-        stats.gamma.pdf(x, a2, scale=1 / beta2, loc=transition)
+    return c1 * (gamma.pdf(x, a1, scale=1 / beta1, loc=2)) + c2 * (
+        gamma.pdf(x, a2, scale=1 / beta2, loc=transition)
     )
 
 
 class nerve_gen_one_gamma(rv_continuous):
     """
     Class to create specific repartition law generator for unmyelinated axons. Inherits from scipy rv_continuous class. Some methods are overwritten
     """
@@ -167,15 +167,15 @@
         self.beta1 = beta1
         self.c1 = c1
 
     def _pdf(self, x):
         """
         overwritting the pdf to custom law, same definition as one_Gamma described upper.
         """
-        return self.c1 * (stats.gamma.pdf(x, self.a1, scale=1 / self.beta1, loc=0.2))
+        return self.c1 * (gamma.pdf(x, self.a1, scale=1 / self.beta1, loc=0.2))
 
 
 class nerve_gen_two_gamma(rv_continuous):
     """
     Class to create specific repartition law generator for myelinated axons. Inherits from scipy rv_continuous class. Some methods are overwritten
     """
 
@@ -224,17 +224,17 @@
         self.transition = transition
 
     def _pdf(self, x):
         """
         overwritting the pdf to custom law, same definition as two_Gamma described upper.
         """
         return self.c1 * (
-            stats.gamma.pdf(x, self.a1, scale=1 / self.beta1, loc=2)
+            gamma.pdf(x, self.a1, scale=1 / self.beta1, loc=2)
         ) + self.c2 * (
-            stats.gamma.pdf(x, self.a2, scale=1 / self.beta2, loc=self.transition)
+            gamma.pdf(x, self.a2, scale=1 / self.beta2, loc=self.transition)
         )
 
 
 def create_generator_from_stat(stat, myelinated=True, dmin=None, dmax=None):
     """
     Create a statistical generator (type rv_continuous) for a given statistic.
 
@@ -264,15 +264,15 @@
     # chose min max values for the axon diameters
     if dmin is None:
         dmin = min(diameters)
     if dmax is None:
         bin_size = diameters[1] - diameters[0]
         dmax = max(diameters) + bin_size
     # perform stat fitting and create generator
-    if myelinated:
+    if myelinated and dmax > 10:
         popt1, pcov1 = curve_fit(
             two_Gamma,
             xdata=diameters,
             ydata=presence,
             bounds=(
                 [1, 2, 0, 1, 0, 0, 2],
                 [np.inf, 15, np.inf, np.inf, 15, np.inf, 14],
@@ -461,435 +461,389 @@
     """
     shuffle_mask = np.random.permutation(len(axons_diameters))
     axons_diameters = axons_diameters[shuffle_mask]
     axons_type = axons_type[shuffle_mask]
     return axons_diameters, axons_type
 
 
-def save_axon_population(f_name, axons_diameters, axons_type, comment=None):
+#############################################
+#############################################
+#############################################
+def init_packing( 
+        diam: np.array,
+        delta: np.float32,
+        y_gc: np.float32,             
+        z_gc: np.float32,
+        ) -> np.array:
+    """
+    Initialize Axon packing Algorithm - Internal use Only
+    """
+    Naxon = len(diam)
+    ids = np.arange(Naxon)         #get IDs of each axons
+    max_diam = np.max(diam) # get max axon diameter
+
+    #Vector of initial velocity
+    velocity= np.zeros([2,Naxon])
+
+    ### create an initial square grid with the population of axons
+    N_init = np.int32(np.ceil(np.sqrt(Naxon)) ** 2)
+    N_side = np.int32(np.sqrt(N_init))
+    size_init = np.sqrt(N_init * (max_diam + delta) ** 2)
+    grid_size = (size_init / 2) - (size_init / (2 * N_side))
+    grid = np.linspace(-grid_size,grid_size,num=N_side,endpoint=True)
+    y_axons = np.tile(grid, N_side) + y_gc
+    z_axons = np.repeat(grid, N_side) + z_gc
+
+    ### remove unwanted places
+    N_remove = N_init - Naxon
+    ind_to_delete = np.random.choice(len(y_axons), size=N_remove, replace=False)
+    y_axons = np.delete(y_axons, ind_to_delete)
+    z_axons = np.delete(z_axons, ind_to_delete)
+
+    #Define position vector:
+    pos = np.array([y_axons, z_axons])
+
+    #Position of center of gravity
+    gc = np.array([y_gc,z_gc])
+
+    return(pos,velocity,gc,ids)
+
+def get_axon_combinaisons(ids: np.array)->np.array:
     """
-    Save an axonal population to a file
+    get all possible combinaison of axons IDs = n(n-1)/2 - Internal use only
+    """
+    return(np.asarray(list(combinations(ids,2))))
 
-    Parameters
-    ----------
-    f_name          : str
-        name of the file to store the population
-    axons_diameters : np.array
-        array containing the axons diameters
-    axons_type      : np.array
-        array containing the axons type ('1' for myelinated, '0' for unmyelinated)
-    comment         : str
-        comment added in the header of the file, optional
+"""def get_axon_interdistance(
+        pos: np.array,
+        ids_pairs: np.array
+    )-> np.array:
+    
+    Compute the distance between each pair of axons - Internal use only
+    @Note: The sqrt could probably be omitted  to increase speed
+    
+    #get the pairs of y and z positions of all axons
+    y_pairs = np.array([pos[0][ids_pairs[:,0]], pos[0][ids_pairs[:,1]]]).T  #we get the y,z position of each combinaison
+    z_pairs = np.array([pos[1][ids_pairs[:,0]], pos[1][ids_pairs[:,1]]]).T
+    #we get the dy and dz combinaison 
+    dy_pairs = np.diff(y_pairs, axis=1).ravel()
+    dz_pairs = np.diff(z_pairs, axis=1).ravel()
+    #We return the position.
+    return(np.sqrt(dz_pairs**2 + dy_pairs**2))"""
+
+def get_axon_inter_radius(
+        diam: np.array,
+        ids_pairs:  np.array
+    )-> np.array:
     """
-    f = open(f_name, "w")
-    if comment is not None:
-        line = "# " + comment
-        f.write(line)
-    for k in range(len(axons_diameters)):
-        line = str(axons_diameters[k]) + ", " + str(axons_type[k]) + "\n"
-        f.write(line)
-    f.close()
+    return the inter-radis of each pair of axons - Internal use only
+    """
+    diam_pair = np.array([diam[ids_pairs[:,0]], diam[ids_pairs[:,1]]]).T  #we get the diameter of each combinaison
+    return(np.abs(np.sum(diam_pair, axis=1).ravel())/2)
 
+def get_delta_pairs(pos:np.array, ids_pairs:np.array)-> np.array:
+    """
+    Evaluate the (z,y) distance of each axons pairs
+    """
+    return np.diff(np.array([pos[ids_pairs[:,0]], pos[ids_pairs[:,1]]]).T, axis=1).ravel()
 
-def load_axon_population(f_name):
+def get_deltad_pairs(pos:np.array, ids_pairs:np.array)-> np.array:
     """
-    Load a population from a file
+    Evaluate the eucledian distance coordinate of each axons pairs - Internal use only
+    @Note: The sqrt could probably be omitted to increase speed
+    """
+    return np.sqrt(get_delta_pairs(pos[0], ids_pairs)**2 + get_delta_pairs(pos[1], ids_pairs)**2)
 
-    Parameters
-    ----------
-    f_name          : str
-        name of the file where the population is stored
+def get_gravity_dr(pos:np.array,gc:np.array,Naxons:np.int32) -> np.array:
+    """
+    Evaluate the (z,y) distance to the gravity center of each axons - Internal use only
+    """
+    return((np.ones([2,Naxons]).T * gc).T - pos)     
 
-    Returns
-    -------
-    axons_diameters     : np.array
-        Array containing all the diameters of the generated axon population
-    axons_type          : np.array
-        Array containing a '1' value for indexes where the axon is myelinated (A-delta or not), else '0'
-    M_diam_list         : np.array
-        list of myelinated only diameters
-    U_diam_list         : np.array
-        list of unmyelinated only diamters
+def get_gravity_dist(pos:np.array,gc:np.array,Naxons:np.int32) -> np.array:
     """
-    population_file = np.genfromtxt(f_name, delimiter=",", comments="#")
-    axons_diameters = population_file[:, 0]
-    axons_type = population_file[:, 1]
-    ind_myel = np.argwhere(axons_type == 1)
-    ind_unmyel = np.argwhere(axons_type == 0)
-    M_diam_list = axons_diameters[ind_myel]
-    U_diam_list = axons_diameters[ind_unmyel]
-    return axons_diameters, axons_type, M_diam_list, U_diam_list
+    Evaluate the eucledian distance to the gravity center of each axons - Internal use only
+    @Note: The sqrt could probably be omitted to increase speed
+    """
+    return(np.sqrt(np.sum((get_gravity_dr(pos,gc,Naxons).T - gc) ** 2,axis = 1)+1e-10))   
 
+def compute_attraction_v(pos:np.array,gc:np.array,Naxons:np.int32,v_att:np.float32)-> np.array:
+    """
+    Evaluate the attraction velocity for every axons - Internal use only
+    """
+    return(v_att*get_gravity_dr(pos,gc,Naxons)/get_gravity_dist(pos,gc,Naxons))
 
-#############################################
-#############################################
-#############################################
-def axon_packer(
-    diameters,
-    Delta=0,
-    y_gc=0,
-    z_gc=0,
-    max_iter=20000,
-    probe=100,
-    monitor=False,
-    monitoring_Folder="",
-    monitoring_Niter=100,
-    v_att=0.01,
-    v_rep=0.1,
-):
+def compute_repulsion_v(pos1:np.array, pos2:np.array,v_rep:np.float32)-> np.array:
+    """
+    Evaluate the repulsion velocity for the colliding axons only - Internal use only
+    """
+    vnew = v_rep* (pos1-pos2)                        
+    return vnew, -vnew
+
+def get_colliding_ids(pos:np.array,id_pairs:np.array,diam_pairs:np.array,delta:np.float32)-> np.array:
+    """ 
+    get ids of colliding axons - Internal use only
+    """
+    return(id_pairs[get_deltad_pairs(pos, id_pairs) < (diam_pairs+delta)])
+
+def update_axon_packing(pos:np.array,
+                        id_pairs:np.array,
+                        diam_pairs:np.array,
+                        gc: np.array,
+                        v_att:np.float32,
+                        v_rep:np.float32,
+                        delta:np.float32,
+                        Naxon:np.int32)->np.array:
+    """ 
+    Update the axon array position by 1 increment - Internal use only
+    """
+
+    velocity = compute_attraction_v(pos,gc,Naxon,v_att)
+    ic = get_colliding_ids(pos,id_pairs,diam_pairs,delta)
+    velocity[:,ic[:,0]], velocity[:,ic[:,1]] = compute_repulsion_v(pos[:,ic[:,0]], pos[:,ic[:,1]],v_rep)
+    return (pos + velocity)
+
+def axon_packer(diameters: np.array,
+                 y_gc:np.float32 = 0,
+                 z_gc:np.float32 = 0,
+                 delta: np.float32 = 0.5,
+                 n_iter: np.int32 = 20000,
+                 v_att: np.float32 = 0.01,
+                 v_rep: np.float32 = 0.1,
+                 monitor = False,
+                 monitoring_Folder="",
+                 n_monitor = 200):
     """
     Axon Packing algorithm: this operation takes a vector of diameter (random population) and places it at best. The used algorithm is largely based on [1]
 
     Parameters
     ----------
     diameters           : np.array
         Array containing all the diameters of the axon population to pack
-    Delta               : float
+    delta               : float
         minimal inter-axon distance to respect before considering collision, in um
+    n_iter            : int
+        Number of iterations
+    v_att               : float
+        vector norm for attraction velocity, in um per iteration
+    v_rep               : float
+        vector norm for repulsion velocity, in um per iteration
     y_gc                : float
         y coordinate of the gravity center for the packing, in um
     z_gc                : float
         z coordinate of the gravity center for the packing, in um
-    max_iter            : int
-        Max. number of iterations
-    probe               : int
-        Number of iterations between two Fiber Volume Fraction probing
     monitor             : bool
-        if True, the packing process will be monitored and some steps are plotted and saved
+        monitor the packing algorithm by saving regularly plot of the population
     monitoring_Folder   : str
-        in case of monitoring, folder where the images of the packing process are stored
-    monitoring_Niter    : str
-        in case of monitoring, number of iterations between two monitoring images
-    v_att               : float
-        vector norm for attraction velocity, in um per iteration
-    v_rep               : float
-        vector norm for repulsion velocity, in um per iteration
+        where to save the monitoring plots
+    n_monitor           : int
+        number of iterration between two successive plots when monitoring the algorithm
 
     Returns
     -------
     y_axons         : np.array
         Array containing the y coordinates of axons, in um
     z_axons         : np.array
         Array containing the z coordinates of axons, in um
-    iteration       : int
-        number of iterations performed
-    FVF             : np.array
-        probed values for the Fiber Volume Fraction
-    probed_iter     : np.array
-        index of the FVF probed iterations
 
     Note
     ----
     - scientific reference
         [1] Mingasson, T., Duval, T., Stikov, N., and Cohen-Adad, J. (2017). AxonPacking: an open-source software to simulate arrangements of axons in white matter. Frontiers in neuroinformatics, 11, 5.
+    - This algorithm cannot be parallelized for the moment.
     - dev Note
         the algorithm perform a fixed number of iteration, the code could evoluate to tke into account the FVF convergence, however this value depends on the range on number of axons.
     """
-    N = len(diameters)
-    max_diam = max(diameters)
-    ##########
-    ## INIT ##
-    ##########
-    ### create an initial square grid with the population of axons
-    N_init = int(math.ceil(np.sqrt(N)) ** 2)
-    N_side = int(np.sqrt(N_init))
-    size_init = np.sqrt(N_init * (max_diam + Delta) ** 2)
-    placement_vector = np.linspace(
-        -((size_init / 2) - (size_init / (2 * N_side))),
-        ((size_init / 2) - (size_init / (2 * N_side))),
-        num=N_side,
-        endpoint=True,
-    )
-    y_axons = np.tile(placement_vector, N_side) + y_gc
-    z_axons = np.repeat(placement_vector, N_side) + z_gc
-    ### remove unwanted places
-    N_remove = N_init - N
-    ind_to_delete = np.random.choice(len(y_axons), size=N_remove, replace=False)
-    y_axons = np.delete(y_axons, ind_to_delete)
-    z_axons = np.delete(z_axons, ind_to_delete)
-    ### compute total total fiber surface and evaluate surface for FVF computation
-    ax_areas = np.power(diameters / 2, 2) * np.pi
-    A_axons = np.sum(ax_areas)
-    size_monitor_square = np.sqrt(A_axons * 1.4)
-    monitor_area = A_axons * 1.4
-    FVF = []
-    probed_iter = []
-    if fg_verbose:
-        pass_info("Axon Packer: initial grid computed...")
-    if monitor:
-        plot_situation(
-            diameters, y_axons, z_axons, size_init, title="Init", y_gc=y_gc, z_gc=z_gc
-        )
-        f_name = monitoring_Folder + "Packer_0.png"
-        plt.savefig(f_name)
-        plt.close()
-    ################
-    ## ITERATIONS ##
-    ################
-    if fg_verbose:
-        pass_info("Axon Packer: Begining iterations")
-    iteration = 0
-    while iteration < max_iter:
-        iteration += 1
-        if fg_verbose:
-            progression_popup(
-                iteration - 1, max_iter, begin_message="\t iteration ", endl="\r"
-            )
-            # print('\t iteration ' + f"{iteration}" + '/' + str(max_iter), end="\r")
-        # compute P matrix
-        P = compute_P_matrix(diameters, y_axons, z_axons, Delta, N)
-        # P = compute_P_fast(diameters, y_axons, z_axons, Delta)
-        # check overlap
-        colapse = np.argwhere(P < 0)
-        all_colapsed_ind = np.unique(colapse)
-        # compute velocity, initialy consider that all velocities are attraction
-        v_y, v_z = compute_attraction_velocities(y_axons, z_axons, y_gc, z_gc, N, v_att)
-        #### prevent from division by 0 in the upper line
-        np.nan_to_num(v_y, copy=False, nan=0.0)
-        np.nan_to_num(v_z, copy=False, nan=0.0)
-        v_y[all_colapsed_ind] = 0  # neutralize velocity where should be repulsion
-        v_z[all_colapsed_ind] = 0  # same
-        # compute velocities for colapsing cases
-        v_y, v_z = handle_collisions(
-            y_axons, z_axons, v_y, v_z, all_colapsed_ind, colapse, v_rep
-        )
-        # compute new positions
-        y_axons, z_axons = update_positions(y_axons, z_axons, v_y, v_z)
-        # compute FVF
-        if iteration % probe == 0:
-            # removing axons too much to the left
-            ax_left_pts = y_axons - diameters / 2
-            FVF_mask = np.argwhere(ax_left_pts > (-size_monitor_square / 2 + y_gc))
-            # removing axons too much to the right
-            ax_right_pts = y_axons + diameters / 2
-            FVF_mask = np.intersect1d(
-                FVF_mask, np.argwhere(ax_right_pts < (size_monitor_square / 2 + y_gc))
-            )
-            # removing the axons that are too high
-            ax_up_pts = z_axons + diameters / 2
-            FVF_mask = np.intersect1d(
-                FVF_mask, np.argwhere(ax_up_pts < (size_monitor_square / 2 + z_gc))
-            )
-            # removing the axons that are too low
-            ax_down_pts = z_axons - diameters / 2
-            FVF_mask = np.intersect1d(
-                FVF_mask, np.argwhere(ax_down_pts > (-size_monitor_square / 2 + z_gc))
-            )
-            FVF.append(np.sum(ax_areas[FVF_mask]) / monitor_area)
-            probed_iter.append(iteration)
-        # monitoring
-        if (iteration) % monitoring_Niter == 0 and monitor:
-            plot_situation(
-                diameters,
-                y_axons,
-                z_axons,
-                size_init,
-                title=str(iteration) + " Iterations",
-                y_gc=y_gc,
-                z_gc=z_gc,
-            )
-            f_name = monitoring_Folder + "Packer_" + str(iteration) + ".png"
-            plt.savefig(f_name)
-            plt.close()
-    pass_info("Axon Packer: Iterations done")
-    if monitor:
-        plot_situation(
-            diameters,
-            y_axons,
-            z_axons,
-            size_init,
-            title=str(iteration) + " Iterations",
-            y_gc=y_gc,
-            z_gc=z_gc,
-        )
-        f_name = monitoring_Folder + "Packer_final.png"
-        plt.savefig(f_name)
-        plt.close()
-    return y_axons, z_axons, iteration, np.asarray(FVF), np.asarray(probed_iter)
-
+    pass_info("Axon packing initiated. This might take a while...")
+    pos,velocity,gc,ids= init_packing(diameters,delta,y_gc,z_gc)
+    max_pos = 2.2 * (np.max(pos[0]) - y_gc)
+    id_pairs = get_axon_combinaisons(ids)
+    diam_pair = get_axon_inter_radius(diameters,id_pairs)
+    Naxon = len(pos[0])
+    #for _ in tqdm(range (n_iter)):
+    #    pos = update_axon_packing(pos,id_pairs,diam_pair,gc,v_att,v_rep,delta,Naxon)
+    fig, ax = plt.subplots(figsize=(8, 8))
+    ax.set_axis_off()
+    fig.add_axes(ax)
+    for i in tqdm(range (n_iter)):
+        pos = update_axon_packing(pos,id_pairs,diam_pair,gc,v_att,v_rep,delta,Naxon)
+        if monitor and i %n_monitor == 0:
+            y_prov = pos[0].copy()
+            z_prov = pos[1].copy()
+            ax.cla()
+            plot_population(diameters, y_prov, z_prov,ax,max_pos, y_gc=y_gc, z_gc=z_gc)
+            plt.savefig(monitoring_Folder+"vignette_"+str(i)+".png")
+    y_axons = pos[0].copy()
+    z_axons = pos[1].copy()
+    pass_info("Packing done!")
+    y_c, z_c = get_barycenter(diameters,y_axons,z_axons)    #center the population back to 0,0
+    return y_axons-y_c, z_axons-z_c
 
-@numba.jit(fastmath=True, cache=True)
-def compute_attraction_velocities(y_axons, z_axons, y_gc, z_gc, N, v_att):
+def expand_pop(y_axons:np.array, z_axons:np.array, factor:float) -> np.array:
     """
-    Computes attraction velocity for axon packing. Just in time compiled to speed up. For internal use only.
-    """
-    dy = np.ones(N) * y_gc - y_axons
-    dz = np.ones(N) * z_gc - z_axons
-    dist = np.sqrt((y_axons - y_gc) ** 2 + (z_axons - z_gc) ** 2)
-    v_y = v_att * dy / dist
-    v_z = v_att * dz / dist  # same
-    return v_y, v_z
-
+    Expand population of placed axons by a specified number
 
-@numba.njit(fastmath=True, cache=True)
-def compute_P_matrix(diameters, y_axons, z_axons, Delta, N):
-    """
-    Computes the proximity matrix for axon packing. Just in time compiled to speed up. For internal use only.
+    Parameters
+    ----------
+    y_axons     : np.array
+        y coordinate of the axons, in um
+    z_axons     : np.array
+        z coordinate of the axons, in um
+    factor          : float
+        expansion factor, unitless
     """
-    P = np.zeros((N, N))
-    for i in range(N):
-        for j in range(i + 1, N):
-            # P[i, j] = np.sqrt((y_axons[i] - y_axons[j])**2 + (z_axons[i] - z_axons[j])**2) -\
-            # ((diameters[i] + diameters[j])/2 + Delta)
-            # not hmogeneous to a distance, but work the same at the end and one square root less to compute...
-            P[i, j] = (
-                (y_axons[i] - y_axons[j]) ** 2 + (z_axons[i] - z_axons[j]) ** 2
-            ) - ((diameters[i] + diameters[j]) / 2 + Delta) ** 2
-    return P
-
+    if (factor<1):
+        rise_warning("expansion factor must be greater than one. Factor set to 1")
+        factor = 1
+    return(y_axons*factor,z_axons*factor)
 
-def compute_P_fast(diameters, y_axons, z_axons, Delta):
+def remove_collision(axons_diameters:np.array,y_axons:np.array,z_axons:np.array, axon_type:np.array, delta: float=0)-> np.array:
     """
-    Compyte the proximity matrix for axon packing. Based on numpy and scipy. Slower (just a bit) than JIT version on dev. For internal use only
-    """
-    points = np.column_stack((y_axons, z_axons))
-    N = len(diameters)
-    diams = np.tile(diameters, (N, 1))
-    # diams = diameters.repeat(N).reshape((-1, N))
-    P = spatial.distance.cdist(points, points, "euclidean") - (
-        (diams + np.transpose(diams)) * (1 / 2) + np.ones((N, N)) * Delta
-    )
-    np.fill_diagonal(P, 0)
-    return np.triu(P)
+    Remove collinding axons in a population
 
-
-@numba.njit(fastmath=True, cache=True)
-def handle_collisions(y_axons, z_axons, v_y, v_z, all_colapsed_ind, colapse, v_rep):
-    """
-    Handle collisions between axons for axon packing. Just in time compiled (doble loop...). For internal use only.
+    Parameters
+    ----------
+    axons_diameters : np.array
+        array containing the axons diameters
+    y_axons     : np.array
+        y coordinate of the axons to store, in um
+    z_axons     : np.array
+        z coordinate of the axons to store, in um
+    axon_type   : np.array
+        type of the axon (Myelinated = 1; Unmyelinated = 0)
+    delta               : float
+        minimal inter-axon distance to respect before considering collision, in um
     """
-    for k in all_colapsed_ind:
-        sum_y = 0
-        sum_z = 0
-        for i in range(len(colapse)):
-            duplet = colapse[i]
-            if k == duplet[0]:
-                sum_y += y_axons[k] - y_axons[duplet[1]]
-                sum_z += z_axons[k] - z_axons[duplet[1]]
-            elif k == duplet[1]:
-                sum_y += y_axons[k] - y_axons[duplet[0]]
-                sum_z += z_axons[k] - z_axons[duplet[0]]
-        if sum_y == 0 and sum_z == 0:
-            sum_y = 1e-12
-            sum_z = 1e-12
-        v_y[k] = v_rep * (sum_y / (np.sqrt(sum_y**2 + sum_z**2)))
-        v_z[k] = v_rep * (sum_z / (np.sqrt(sum_y**2 + sum_z**2)))
-    return v_y, v_z
 
+    Naxon = len(axons_diameters)
+    ids = np.arange(Naxon)    
+    id_pairs = get_axon_combinaisons(ids)
+    pos = np.zeros([2,Naxon])
+    pos[0,:] = y_axons
+    pos[1,:] = z_axons
+    diam_pairs = get_axon_inter_radius(axons_diameters,id_pairs)
+    ic = get_colliding_ids(pos,id_pairs,diam_pairs,delta) 
+    ic = ic[:,0]
+    if len(ic)>0:
+        rise_warning(f"{len(ic)} axon collisions detected - Axons discarded.")
+    return(np.delete(axons_diameters,ic),np.delete(y_axons,ic),np.delete(z_axons,ic),np.delete(axon_type,ic))
 
-@numba.njit(fastmath=True, cache=True)
-def update_positions(y_axons, z_axons, v_y, v_z):
-    """
-    Compute new positions considering velicities for axon packing. Just in time compiled to speed up. For internal use only.
+def get_circular_contour(axons_diameters:np.array,y_axons:np.array,z_axons:np.array, delta: float = 10)-> float:
     """
-    return y_axons + v_y, z_axons + v_z
+    Get a circular contour diameter of the axon population
 
+    Parameters
+    ----------
+    axons_diameters : np.array
+        array containing the axons diameters
+    y_axons     : np.array
+        y coordinate of the axons to store, in um
+    z_axons     : np.array
+        z coordinate of the axons to store, in um
+    delta               : float
+        distance between the contour and the closest axon, in um
+    """
+    dist_axon = np.sqrt((y_axons ** 2 + z_axons**2))
+    dist_axon+= axons_diameters/2
+    radius = np.max(dist_axon) + delta
+    return(radius*2)
 
-def delete_collisions(axons_diameters, axons_type, y_axons, z_axons, Delta=0):
+def remove_outlier_axons(axons_diameters:np.array, y_axons:np.array, z_axons:np.array, axon_type:np.array, diameter: float = 10)-> np.array:
     """
-    Delete collision cases in a placed population. In case of a detected collision, the axon or smaller diameter is removed.
+    Remove axons in a population located outside a circular border, defined by its diameter
 
     Parameters
     ----------
     axons_diameters : np.array
         array containing the axons diameters
-    axons_type      : np.array
-        array containing the axons type ('1' for myelinated, '0' for unmyelinated)
-    y_axons         : np.array
+    y_axons     : np.array
         y coordinate of the axons to store, in um
-    z_axons         : np.array
+    z_axons     : np.array
         z coordinate of the axons to store, in um
-    Delta           : float
-        space between axon fibers under which collision is considered, in um
+    axon_type   : np.array
+        type of the axon (Myelinated = 1; Unmyelinated = 0)
+    diameter               : float
+        diameter of the circular border, in um
+    """
+    dist_axon = np.sqrt((y_axons ** 2 + z_axons**2))
+    dist_axon+= axons_diameters/2
+    inside_border = dist_axon <= diameter/2
+    n_remove = len(np.where(inside_border==False)[0])
+    if (n_remove>0):
+        rise_warning(f"{n_remove} outlier axons discarded.")
 
-    Returns
-    -------
-    new_axons_diameters : np.array
-        array containing the axons diameters without collisions
-    new_axons_type      : np.array
-        array containing the axons type ('1' for myelinated, '0' for unmyelinated)
-    new_y_axons     : np.array
+    return(axons_diameters[inside_border],y_axons[inside_border],z_axons[inside_border],axon_type[inside_border])
+
+def get_barycenter(axons_diameters, y_axons, z_axons):
+    """
+    Compute barycenter of the population
+
+    Parameters
+    ----------
+    axons_diameters : np.array
+        array containing the axons diameters
+    y_axons     : np.array
         y coordinate of the axons to store, in um
-    new_z_axons     : np.array
+    z_axons     : np.array
         z coordinate of the axons to store, in um
     """
-    N = len(axons_diameters)
-    P = compute_P_matrix(axons_diameters, y_axons, z_axons, Delta, N)
-    colapse = np.argwhere(P < 0)
-    flag_Collision = colapse.size != 0
-
-    while flag_Collision:
-        # checking which axons to delete
-        ind_to_delete = []
-        handled_collisions = []
-        for collision in colapse:
-            if (collision[0] not in handled_collisions) and (
-                collision[1] not in handled_collisions
-            ):
-                handled_collisions.append(collision[0])
-                handled_collisions.append(collision[1])
-                if axons_diameters[collision[0]] < axons_diameters[collision[1]]:
-                    ind_to_delete.append(collision[0])
-                else:
-                    ind_to_delete.append(collision[1])
-        # deleting problematic axons
-        mask = np.ones(N, dtype=bool)
-        mask[ind_to_delete] = False
-        axons_diameters = axons_diameters[mask]
-        axons_type = axons_type[mask]
-        y_axons = y_axons[mask]
-        z_axons = z_axons[mask]
-        N = len(axons_diameters)
-        # check if there are remaing collisions
-        P = compute_P_matrix(axons_diameters, y_axons, z_axons, Delta, N)
-        colapse = np.argwhere(P < 0)
-        flag_Collision = colapse.size != 0
-
-    return axons_diameters, axons_type, y_axons, z_axons
+    diam_sum = np.sum(axons_diameters)
+    return(np.sum(axons_diameters * y_axons)/diam_sum,np.sum(axons_diameters * z_axons)/diam_sum)
 
-
-def plot_situation(diameters, y_axons, z_axons, size, title=None, y_gc=0, z_gc=0):
+def plot_population(diameters, y_axons, z_axons,ax,size, axon_type = None, y_gc=0, z_gc=0)->None:
     """
-    Discplay a population of axons. Doesn't return but declares a matplotlib figure
+    Display a population of axons. 
 
     Parameters
     ----------
     diameters   : np.array
         diamters of the axons to display, in um
     y_axons     : np.array
         y coordinate of the axons to display, in um
     z_axons     : np.array
         z coordinate of the axons to display, in um
+    ax          : matplotlib.axes
+        (sub-) plot of the matplotlib figure
     size        : float
         size of the window as a square side, in um
+    axon_type   : np.array
+        type of the axon (Myelinated = 1; Unmyelinated = 0) - Optionnal
     title       : str
         title of the figure
     y_gc        : float
         y coordinate of the gravity, in um
     z_gc        : float
         z coordinate of the gravity, in um
     """
-    circles = []
-    for k in range(len(diameters)):
-        circles.append(
-            plt.Circle(
-                (y_axons[k], z_axons[k]), diameters[k] / 2, color="r", fill=False
-            )
-        )
-    fig, ax = plt.subplots(figsize=(8, 8))
-    for circle in circles:
-        ax.add_patch(circle)
-    if title is not None:
-        plt.title(title)
-    plt.xlim(-size / 2 + y_gc, size / 2 + y_gc)
-    plt.ylim(-size / 2 + z_gc, size / 2 + z_gc)
+    if (axon_type is None):
+        for k in range(len(diameters)):
+            ax.add_patch(plt.Circle((y_axons[k], z_axons[k]), diameters[k] / 2, color="r", fill=True))
+    else:
+        # plot the final results, with distinction between un- and myelinated axons
+        myelinated_mask = np.argwhere(axon_type == 1)
+        y_myelinated = y_axons[myelinated_mask]
+        z_myelinated = z_axons[myelinated_mask]
+        M_diam_list = diameters[myelinated_mask]
+        for k in range(len(y_myelinated)):
+                ax.add_patch(plt.Circle((y_myelinated[k], z_myelinated[k]), M_diam_list[k]/2, color='r',fill=True))
+
+
+        unmyelinated_mask = np.argwhere(axon_type == 0) 
+        y_unmyelinated = y_axons[unmyelinated_mask]
+        z_unmyelinated = z_axons[unmyelinated_mask]
+        U_diam_list = diameters[unmyelinated_mask]
+        for k in range(len(y_unmyelinated)):
+                ax.add_patch(plt.Circle((y_unmyelinated[k], z_unmyelinated[k]), U_diam_list[k]/2, color='b',fill=True))
+
+    ax.set_xlim(-size / 2 + y_gc, size / 2 + y_gc)
+    ax.set_ylim(-size / 2 + z_gc, size / 2 + z_gc)
 
 
-def save_placed_axon_population(
-    f_name, axons_diameters, axons_type, y_axons, z_axons, comment=None
+def save_axon_population(
+    f_name, axons_diameters, axons_type, y_axons=None, z_axons=None, comment=None
 ):
     """
     Save a placed axonal population to a file
 
     Parameters
     ----------
     f_name          : str
@@ -901,14 +855,22 @@
     y_axons     : np.array
         y coordinate of the axons to store, in um
     z_axons     : np.array
         z coordinate of the axons to store, in um
     comment         : str
         comment added in the header of the file, optional
     """
+    if y_axons is None:
+        y_axons = np.zeros([len(axons_diameters)])
+        y_axons[:] = np.nan
+
+    if z_axons is None:
+        z_axons = np.zeros([len(axons_diameters)])
+        z_axons[:] = np.nan
+
     f = open(f_name, "w")
     if comment is not None:
         line = "# " + comment
         f.write(line)
     for k in range(len(axons_diameters)):
         line = (
             str(axons_diameters[k])
@@ -920,15 +882,15 @@
             + str(z_axons[k])
             + "\n"
         )
         f.write(line)
     f.close()
 
 
-def load_placed_axon_population(f_name):
+def load_axon_population(f_name):
     """
     Load a placed population from a file
 
     Parameters
     ----------
     f_name          : str
         name of the file where the population is stored
@@ -953,8 +915,13 @@
     axons_type = population_file[:, 1]
     y_axons = population_file[:, 2]
     z_axons = population_file[:, 3]
     ind_myel = np.argwhere(axons_type == 1)
     ind_unmyel = np.argwhere(axons_type == 0)
     M_diam_list = axons_diameters[ind_myel]
     U_diam_list = axons_diameters[ind_unmyel]
-    return axons_diameters, axons_type, y_axons, z_axons, M_diam_list, U_diam_list
+    
+
+    if (np.isnan(y_axons).all() or np.isnan(z_axons).all()):
+        rise_warning("Loaded population has no y,z coordinates.")
+
+    return axons_diameters, axons_type, M_diam_list, U_diam_list, y_axons, z_axons
```

### Comparing `nrv-py-1.0.1/nrv/nmod/fascicles.py` & `nrv_py-1.1.0/nrv/nmod/fascicles.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import faulthandler
 import os
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from ..backend.file_handler import *
-from ..backend.log_interface import pass_info, rise_warning
+from ..backend.log_interface import pass_info, rise_warning, pbar
 from ..backend.MCore import MCH, synchronize_processes
 from ..backend.NRV_Simulable import NRV_simulable, sim_results
 from ..fmod.extracellular import *
 from ..fmod.recording import *
 from ..utils.cell.CL_postprocessing import *
 from .axons import *
-from .fascicle_generator import *
+from .axon_pop_generator import *
 from .myelinated import *
 from .unmyelinated import *
 
 
 # Parallel computing options
 if not MCH.is_alone():
     fg_verbose = False
@@ -56,63 +56,46 @@
 
 class fascicle(NRV_simulable):
     """
     Class for Fascicle, defined as a group of axons near one to the other in the same Perineurium Sheath. All axons are independant of each other, no ephaptic coupling.
 
     Parameters
     ----------
-    dt              : float
-        simulation time stem for Neuron (ms), by default 1us
-    Nseg_per_sec    : float
-        number of segment per section in Neuron. If set to 0, the number of segment per section is calculated with the d-lambda rule
-    freq            : float
-        frequency of the d-lambda rule (Hz), by default 100Hz
-    freq_min        : float
-        minimum frequency for the d-lambda rule when meshing is irregular, 0 for regular meshing
-    v_init          : float
-        initial value for the membrane voltage (mV), specify None for automatic model choice of v_init
-    T               : float
-        temperature (C), specify None for automatic model choice of temperature
-    ID              : int
-        axon ID, by default set to 0
-    threshold       : int
-        membrane voltage threshold for spike detection (mV), by default -40mV
+    diameter              : float
+        Fascicle diameter, in um
+    ID    : int
+        Fascicle unique identifier
     """
 
-    def __init__(self, ID=0, **kwargs):
+    def __init__(self, diameter=None, ID=0, **kwargs):
         """
-        Instrantation of a Fascicle
+        Instantation of a Fascicle
         """
-        super().__init__()
+        super().__init__(**kwargs)
 
         # to add to a fascicle/nerve common mother class
         self.save_path = ""
         self.verbose = False
         self.postproc_script = "default"
         self.return_parameters_only = True
         self.loaded_footprints = True
         self.save_results = True
 
         self.config_filename = ""
         self.type = "fascicle"
         self.ID = ID
         self.type = None
         self.L = None
-        self.D = None
+        self.D = diameter
         # geometric properties
         self.y_grav_center = 0
         self.z_grav_center = 0
-        self.N_vertices = 0
-        self.y_vertices = np.array([])
-        self.z_vertices = np.array([])
-        self.A = 0
         # axonal content
-        self.N = 0
         self.axons_diameter = np.array([])
-        self.axons_type = np.array([])
+        self.axons_type = np.array([], dtype=int)
         self.axons_y = np.array([])
         self.axons_z = np.array([])
         self.NoR_relative_position = np.array([])
         # Axons objects default parameters
         self.unmyelinated_param = {
             "model": "Rattay_Aberham",
             "dt": 0.001,
@@ -191,15 +174,15 @@
             key to exclude from saving
         save:               bool
             if false only return the dictionary
 
         Returns
         -------
         key_dict:           dict
-            Pyhton dictionary containing all the fascicle information
+            Python dictionary containing all the fascicle information
         """
         bl = [i for i in blacklist]
         if not intracel_context:
             bl += [
                 "N_intra",
                 "intra_stim_position",
                 "intra_stim_t_start",
@@ -297,14 +280,38 @@
             data=fname,
             extracel_context=extracel_context,
             intracel_context=intracel_context,
             rec_context=rec_context,
         )
 
     ## Fascicle property method
+    @property
+    def n_ax(self):
+        """
+        Number of axons in the fascicle
+        """
+        return len(self.axons_diameter)
+
+    @property
+    def N(self):
+        rise_warning(
+            "DeprecationWarning: ",
+            "fascicle.N property is obsolete use fascicle.n_ax instead"
+        )
+        return self.n_ax
+
+    @property
+    def A(self):
+        """
+        Area of the fascicle 
+        """
+        if (self. D is None):
+            return None
+        return (np.pi * (self.D / 2) ** 2)
+    
     def set_ID(self, ID):
         """
         set the ID of the fascicle
 
         Parameters
         ----------
         ID : int
@@ -325,40 +332,33 @@
             rise_warning(
                 "Modifying length of a fascicle with extra or intra cellular context can lead to error"
             )
         self.L = L
         self.set_axons_parameters(unmyelinated_nseg=self.L // 25)
 
     ## generate stereotypic Fascicle
-    def define_circular_contour(self, D, y_c=None, z_c=None, N_vertices=100):
+    def define_circular_contour(self, D, y_c=None, z_c=None):
         """
         Define a circular countour to the fascicle
 
         Parameters
         ----------
         D           : float
             diameter of the circular fascicle contour, in um
         y_c         : float
             y coordinate of the circular contour center, in um
         z_c         : float
             z coordinate of the circular contour center, in um
-        N_vertices  : int
-            Number of vertice in the compute the contour
         """
         self.type = "Circular"
         self.D = D
         if y_c is not None:
             self.y_grav_center = y_c
         if z_c is not None:
             self.z_grav_center = z_c
-        self.N_vertices = N_vertices
-        theta = np.linspace(-np.pi, np.pi, num=N_vertices)
-        self.y_vertices = self.y_grav_center + (D / 2) * np.cos(theta)
-        self.z_vertices = self.z_grav_center + (D / 2) * np.sin(theta)
-        self.A = np.pi * (D / 2) ** 2
 
     def get_circular_contour(self):
         """
         Returns the properties of the fascicle contour considered as a circle (y and z center and diameter)
 
         Returns
         -------
@@ -367,39 +367,32 @@
         y : float
             y position of the contour center, in um
         z : float
             z position of the contour center, in um
         """
         y = self.y_grav_center
         z = self.z_grav_center
-        if self.y_vertices == np.array([]) and self.D is None:
-            D = 0
-        elif self.D is not None:
-            D = self.D
-        else:
-            y = (np.amax(self.y_vertices) - np.amin(self.y_vertices)) / 2
-            z = (np.amax(self.z_vertices) - np.amin(self.z_vertices)) / 2
-            D = np.abs(np.amax(self.y_vertices) - np.amin(self.y_vertices))
+        D = self.D
         return D, y, z
 
-    def fit_circular_contour(self, y_c=None, z_c=None, Delta=0.1, N_vertices=100):
+    def fit_circular_contour(self, y_c=None, z_c=None, Delta=0.1):
         """
         Define a circular countour to the fascicle
 
         Parameters
         ----------
         y_c         : float
             y coordinate of the circular contour center, in um
         z_c         : float
             z coordinate of the circular contour center, in um
         Delta       : float
             distance between farest axon and contour, in um
-        N_vertices  : int
-            Number of vertice in the compute the contour
         """
+        rise_warning("fit_circular_contour method usage is not recommended anymore and will be removed in future release.")
+        pass_info("Define fascicle size/shape at object creation instead.")
         N_axons = len(self.axons_diameter)
         D = 2 * Delta
 
         if y_c is not None:
             self.y_grav_center = y_c
         if z_c is not None:
             self.z_grav_center = z_c
@@ -412,15 +405,15 @@
                     + (
                         (self.y_grav_center - self.axons_y[axon]) ** 2
                         + (self.z_grav_center - self.axons_z[axon]) ** 2
                     )
                     ** 0.5
                 )
                 D = max(D, 2 * (dist_max + Delta))
-        self.define_circular_contour(D, y_c=None, z_c=None, N_vertices=N_vertices)
+        self.define_circular_contour(D, y_c=None, z_c=None)
 
     def define_ellipsoid_contour(self, a, b, y_c=0, z_c=0, rotate=0):
         """
         Define ellipsoidal contour
         """
         pass
 
@@ -458,14 +451,17 @@
         U_stat          : str
             name of the statistic in the librairy or path to a new librairy in csv for unmyelinated diameters repartition
         ppop_fname      : str
             optional, if specified, name file to store the placed population generated
         pop_fname       : str
             optional, if specified, name file to store the population generated
         """
+
+        rise_warning("fill method usage is not recommended anymore and will be removed in future release.")
+        pass_info("Use axon_pop_generator methods instead.")
         #### AXON GENERATION: parallelization if resquested ####
         Area_to_fill = 0
         # Note: generate a bit too much axons just in case
         if self.type == "Circular":
             Area_to_fill = np.pi * (self.D / 2 + 28) ** 2
         if parallel:
             if MCH.do_master_only_work():
@@ -504,228 +500,130 @@
         if MCH.do_master_only_work():
             N = len(axons_diameter)
             pass_info("\n ... " + str(N) + " axons generated")
             if pop_fname is not None:
                 save_axon_population(
                     pop_fname, axons_diameter, axons_type, comment=None
                 )
-            pass_info("Axon Packing is starting")
-            axons_y, axons_z, iteration, FVF_array, probed_iter = axon_packer(
+            axons_y, axons_z, = axon_packer(
                 axons_diameter,
-                Delta=0.1,
+                delta=0.1,
                 y_gc=self.y_grav_center,
                 z_gc=self.z_grav_center,
-                max_iter=20000,
-                monitor=False,
-            )
-            # check for remaining collisions and delete problematic axons
-            axons_diameter, axons_type, axons_y, axons_z = delete_collisions(
-                axons_diameter, axons_type, axons_y, axons_z
+                n_iter=20000,
             )
+
             N = len(axons_diameter)
-            pass_info("... Axon Packing done")
             # check if axons are inside the fascicle
             inside_axons = (
                 np.power(axons_y - self.y_grav_center, 2)
                 + np.power(axons_z - self.z_grav_center, 2)
                 - np.power(np.ones(N) * (self.D / 2) - axons_diameter / 2, 2)
             )
             axons_to_keep = np.argwhere(inside_axons < 0)
             axons_diameter = axons_diameter[axons_to_keep]
             axons_type = axons_type[axons_to_keep]
             axons_y = axons_y[axons_to_keep]
             axons_z = axons_z[axons_to_keep]
             N = len(axons_diameter)
             # save the good population
             if ppop_fname is not None:
-                save_placed_axon_population(
+                save_axon_population(
                     ppop_fname,
                     self.axons_diameter,
                     self.axons_type,
                     self.axons_y,
                     self.axons_z,
                     comment=None,
                 )
         else:
             axons_diameter = None
             axons_type = None
             axons_y = None
             axons_z = None
             N = None
         ## BRODCASTING RESULTS TO ALL PARALLEL OBJECTS
-        self.axons_diameter = MCH.master_broadcasts_array_to_all(
-            axons_diameter
-        ).flatten()
+        self.axons_diameter = MCH.master_broadcasts_array_to_all(axons_diameter).flatten()
         self.axons_type = MCH.master_broadcasts_array_to_all(axons_type).flatten()
         self.axons_y = MCH.master_broadcasts_array_to_all(axons_y).flatten()
         self.axons_z = MCH.master_broadcasts_array_to_all(axons_z).flatten()
-        self.N = MCH.master_broadcasts_array_to_all(N)
 
     def fill_with_population(
-        self, axons_diameter, axons_type, Delta=0.1, ppop_fname=None, FVF=0.55
-    ):
+        self, axons_diameter:np.array, axons_type:np.array, delta:float=1,
+        y_axons:np.array=None, z_axons:np.array=None, fit_to_size: bool = False, n_iter: int = 20_000
+    ) -> None: 
         """
-        Fill a geometricaly defined contour with an already generated axon population
+        Fill the fascicle with an axon population
 
         Parameters
         ----------
         axons_diameters     : np.array
             Array  containing all the diameters of the axon population
         axons_type          : np.array
             Array containing a '1' value for indexes where the axon is myelinated (A-delta or not), else '0'
-        ppop_fname      : str
-            optional, if specified, name file to store the placed population generated
-        FVF             : float
-            Fiber Volume Fraction estimated for the area. By default set to 0.55
+        delta               : float
+            axon-to-axon and axon to border minimal distance
+        y_axons             : np.array
+            y coordinate of the axon population, in um
+        z_axons             : np.array
+            z coordinate of the axons population, in um
+        fit_to_size         : bool
+            if true, the axon population is extended to fit within fascicle size, if not the population is kept as is
+        n_iter              : int
+            number of interation for the packing algorithm if the y-x axon coordinates are not specified
+        WARNING: If y_axons and z_axons are not specified then axon-packing algorithm is called within the method.
         """
         if MCH.do_master_only_work():
-            ## check the population area
-            total_ax_area = 0
-            for diam in axons_diameter:
-                total_ax_area += np.pi * ((diam / 2) ** 2)
-            if self.A * FVF > total_ax_area:
-                rise_warning(
-                    "Warning: the specified population maybe too small to fill the current fascicle"
-                )
-            N = len(axons_diameter)
-            pass_info("\n ... " + str(N) + " axons loaded")
-            if ppop_fname is not None:
-                save_axon_population(
-                    ppop_fname, axons_diameter, axons_type, comment=None
-                )
-            pass_info("Axon Packing is starting")
-            axons_y, axons_z, iteration, FVF_array, probed_iter = axon_packer(
-                axons_diameter,
-                Delta=Delta,
-                y_gc=self.y_grav_center,
-                z_gc=self.z_grav_center,
-                max_iter=20000,
-                monitor=False,
-            )
-            # check for remaining collisions and delete problematic axons
-            axons_diameter, axons_type, axons_y, axons_z = delete_collisions(
-                axons_diameter, axons_type, axons_y, axons_z
-            )
-            N = len(axons_diameter)
-            pass_info("... Axon Packing done")
-            # check if axons are inside the fascicle
-            inside_axons = (
-                np.power(axons_y - self.y_grav_center, 2)
-                + np.power(axons_z - self.z_grav_center, 2)
-                - np.power(np.ones(N) * (self.D / 2) - axons_diameter / 2, 2)
-            )
-            axons_to_keep = np.argwhere(inside_axons < 0)
-            axons_diameter = axons_diameter[axons_to_keep]
-            axons_type = axons_type[axons_to_keep]
-            axons_y = axons_y[axons_to_keep]
-            axons_z = axons_z[axons_to_keep]
             N = len(axons_diameter)
-            # save the good population
-            if ppop_fname is not None:
-                save_placed_axon_population(
-                    ppop_fname,
-                    self.axons_diameter,
-                    self.axons_type,
-                    self.axons_y,
-                    self.axons_z,
-                    comment=None,
+            if (y_axons is None) and (z_axons is None):
+                y_axons, z_axons = axon_packer(
+                    axons_diameter,
+                    delta=delta,
+                    n_iter=n_iter
                 )
+            if (fit_to_size):
+                d_pop = get_circular_contour(axons_diameter,y_axons,z_axons, delta)
+                if (d_pop) < self.D:
+                    exp_factor = 0.99*(self.D/d_pop)
+                    y_axons, z_axons = expand_pop(y_axons, z_axons, exp_factor)
+            
+            axons_diameter, y_axons, z_axons, axons_type = remove_collision(axons_diameter, y_axons, z_axons, axons_type)
+            axons_diameter, y_axons, z_axons, axons_type = remove_outlier_axons(axons_diameter, y_axons, z_axons, axons_type, self.D-delta)
+            
         else:
             axons_diameter = None
             axons_type = None
-            axons_y = None
-            axons_z = None
+            y_axons = None
+            z_axons = None
             N = None
         ## BRODCASTING RESULTS TO ALL PARALLEL OBJECTS
-        self.axons_diameter = MCH.master_broadcasts_array_to_all(
-            axons_diameter
-        ).flatten()
+        self.axons_diameter = MCH.master_broadcasts_array_to_all(axons_diameter).flatten()
         self.axons_type = MCH.master_broadcasts_array_to_all(axons_type).flatten()
-        self.axons_y = MCH.master_broadcasts_array_to_all(axons_y).flatten()
-        self.axons_z = MCH.master_broadcasts_array_to_all(axons_z).flatten()
-        self.N = MCH.master_broadcasts_array_to_all(N)
+        self.axons_y = MCH.master_broadcasts_array_to_all(y_axons).flatten()
+        self.axons_z = MCH.master_broadcasts_array_to_all(z_axons).flatten()
+        self.translate_axons(self.y_grav_center,self.z_grav_center)
 
-    def fill_with_placed_population(
-        self,
-        axons_diameter,
-        axons_type,
-        axons_y,
-        axons_z,
-        check_inside=True,
-        check_collision=True,
-        ppop_fname=None,
-    ):
+    def fit_population_to_size(self, delta: float = 1):
         """
-        Fill a geometricaly defined contour with an already generated axon population
+        Fit the axon positions to the size of the fascicle
 
         Parameters
         ----------
-        axons_diameters     : np.array
-            Array  containing all the diameters of the axon population
-        axons_type          : np.array
-            Array containing a '1' value for indexes where the axon is myelinated (A-delta or not), else '0'
-        axons_y             : np.array
-            y coordinate of the axons, in um
-        axons_z             : np.array
-            z coordinate of the axons, in um
-        check_inside        : bool
-            if True the placed axons position are checked to ensure all remaining axons at the end are inside the fascicle
-        check_collision     : bool
-            if True, possible remaining collisions are check in the loaded population, and thiner axons are deleted
-        ppop_fname          : str
-            optional, if specified, name file to store the placed population generated
+        delta   : float
+            minimum axon to fascicle border distance, in um
         """
-        if MCH.do_master_only_work():
-            N = len(axons_diameter)
-            if check_collision:
-                # check for remaining collisions and delete problematic axons
-                axons_diameter, axons_type, axons_y, axons_z = delete_collisions(
-                    axons_diameter, axons_type, axons_y, axons_z
-                )
-                N = len(axons_diameter)
-            # check if axons are inside the fascicle
-            if check_inside:
-                inside_axons = (
-                    np.power(axons_y - self.y_grav_center, 2)
-                    + np.power(axons_z - self.z_grav_center, 2)
-                    - np.power(np.ones(N) * (self.D / 2) - axons_diameter / 2, 2)
-                )
-                axons_to_keep = np.argwhere(inside_axons < 0)
-                axons_diameter = axons_diameter[axons_to_keep]
-                axons_type = axons_type[axons_to_keep]
-                axons_y = axons_y[axons_to_keep]
-                axons_z = axons_z[axons_to_keep]
-                N = len(axons_diameter)
-            # save the good population
-            if ppop_fname is not None:
-                save_placed_axon_population(
-                    ppop_fname,
-                    self.axons_diameter,
-                    self.axons_type,
-                    self.axons_y,
-                    self.axons_z,
-                    comment=None,
-                )
-        else:
-            axons_diameter = None
-            axons_type = None
-            axons_y = None
-            axons_z = None
-            N = None
-        ## BRODCASTING RESULTS TO ALL PARALLEL OBJECTS
-        self.axons_diameter = MCH.master_broadcasts_array_to_all(
-            axons_diameter
-        ).flatten()
-        self.axons_type = MCH.master_broadcasts_array_to_all(axons_type).flatten()
-        self.axons_y = MCH.master_broadcasts_array_to_all(axons_y).flatten()
-        self.axons_z = MCH.master_broadcasts_array_to_all(axons_z).flatten()
-        self.N = MCH.master_broadcasts_array_to_all(N)
+        self.translate_axons(-self.y_grav_center,-self.z_grav_center)
+        d_pop = get_circular_contour(self.axons_diameter,self.axons_y,self.axons_z, delta)
+        if (d_pop) < self.D:
+            exp_factor = 0.99*(self.D/d_pop)
+            self.axons_y, self.axons_z = expand_pop(self.axons_y, self.axons_z, exp_factor)
+        self.translate_axons(self.y_grav_center,self.z_grav_center)
 
     ## Move methods
-    def translate_axons(self, y, z):
+    def translate_axons(self, y, z): 
         """
         Move axons only in a fascicle by group translation
 
         Parameters
         ----------
         y   : float
             y axis value for the translation in um
@@ -744,16 +642,14 @@
         y   : float
             y axis value for the translation in um
         z   : float
             z axis value for the translation in um
         """
         self.y_grav_center += y
         self.z_grav_center += z
-        self.y_vertices += y
-        self.z_vertices += z
         self.translate_axons(y, z)
         if self.extra_stim is not None:
             self.extra_stim.translate(y=y, z=z)
         if self.recorder is not None:
             self.recorder.translate(y=y, z=z)
 
     def rotate_axons(self, theta, y_c=0, z_c=0):
@@ -793,65 +689,16 @@
             np.cos(theta) * (self.y_grav_center - y_c)
             - np.sin(theta) * (self.z_grav_center - z_c)
         ) + y_c
         self.z_grav_center = (
             np.sin(theta) * (self.y_grav_center - y_c)
             + np.cos(theta) * (self.z_grav_center - z_c)
         ) + z_c
-        self.y_vertices += (
-            np.cos(theta) * (self.y_vertices - y_c)
-            - np.sin(theta) * (self.z_vertices - z_c)
-        ) + y_c
-        self.z_vertices += (
-            np.sin(theta) * (self.y_vertices - y_c)
-            + np.cos(theta) * (self.z_vertices - z_c)
-        ) + z_c
         self.rotate_axons(theta, y_c=y_c, z_c=z_c)
 
-    def remove_axons_electrode_overlap(self, electrode):
-        """
-        Remove the axons that could overlap an electrode
-
-        Parameters
-        ----------
-        electrode : object
-            electrode instance, see electrodes for more details
-        """
-        y, z, D = 0, 0, 0
-        if is_LIFE_electrode(electrode):
-            D = electrode.D
-            y = electrode.y
-            z = electrode.z
-        elif is_analytical_electrode(electrode):
-            y = electrode.y
-            z = electrode.z
-        else:
-            # CUFF electrodes should not affect intrafascicular state
-            return 0
-        # compute the distance of all axons to electrode
-        D_vectors = np.sqrt((self.axons_y - y) ** 2 + (self.axons_z - z) ** 2) - (
-            self.axons_diameter / 2 + D / 2
-        )
-        colapse = np.argwhere(D_vectors < 0)
-        mask = np.ones(len(self.axons_diameter), dtype=bool)
-        mask[colapse] = False
-        # remove axons colliding the electrode
-        if len(colapse) > 0:
-            pass_info(
-                "From Fascicle level: Electrode/Axons overlap, "
-                + str(len(colapse))
-                + " axons will be removed from the fascicle"
-            )
-        self.N -= len(colapse)
-        pass_info(self.N, "axons remaining")
-        self.axons_diameter = self.axons_diameter[mask]
-        self.axons_type = self.axons_type[mask]
-        self.axons_y = self.axons_y[mask]
-        self.axons_z = self.axons_z[mask]
-
     ## Axons related method
     def set_axons_parameters(
         self, unmyelinated_only=False, myelinated_only=False, **kwargs
     ):
         """
         set parameters of axons in the fascicle
 
@@ -907,28 +754,26 @@
         Remove all unmyelinated fibers from the fascicle
         """
         mask = self.axons_type.astype(bool)
         self.axons_diameter = self.axons_diameter[mask]
         self.axons_y = self.axons_y[mask]
         self.axons_z = self.axons_z[mask]
         self.axons_type = self.axons_type[mask]
-        self.N = len(self.axons_diameter)
         if len(self.NoR_relative_position) != 0:
             self.NoR_relative_position = self.NoR_relative_position[mask]
 
     def remove_myelinated_axons(self):
         """
         Remove all myelinated fibers from the
         """
         mask = np.invert(self.axons_type.astype(bool))
         self.axons_diameter = self.axons_diameter[mask]
         self.axons_y = self.axons_y[mask]
         self.axons_z = self.axons_z[mask]
         self.axons_type = self.axons_type[mask]
-        self.N = len(self.axons_diameter)
         if len(self.NoR_relative_position) != 0:
             # almost useless but here for coherence
             self.NoR_relative_position = self.NoR_relative_position[mask]
 
     def remove_axons_size_threshold(self, d, min=True):
         """
         Remove fibers with diameters below/above a threshold
@@ -938,49 +783,50 @@
         else:
             mask = self.axons_diameter <= d
 
         self.axons_diameter = self.axons_diameter[mask]
         self.axons_y = self.axons_y[mask]
         self.axons_z = self.axons_z[mask]
         self.axons_type = self.axons_type[mask]
-        self.N = len(self.axons_diameter)
         if len(self.NoR_relative_position) != 0:
             # almost useless but here for coherence
             self.NoR_relative_position = self.NoR_relative_position[mask]
 
     ## Representation methods
     def plot(
-        self, fig, axes, contour_color="k", myel_color="r", unmyel_color="b", num=False
+        self, axes, contour_color="k", myel_color="r", unmyel_color="b", elec_color="gold", num=False
     ):
         """
         plot the fascicle in the Y-Z plane (transverse section)
 
         Parameters
         ----------
-        fig     : matplotlib.figure
-            figure to display the fascicle
         axes    : matplotlib.axes
             axes of the figure to display the fascicle
         contour_color   : str
             matplotlib color string applied to the contour. Black by default
         myel_color      : str
             matplotlib color string applied to the myelinated axons. Red by default
         unmyel_color    : str
             matplotlib color string applied to the myelinated axons. Blue by default
         num             : bool
             if True, the index of each axon is displayed on top of the circle
         """
         if MCH.do_master_only_work():
             ## plot contour
-            axes.plot(
-                self.y_vertices, self.z_vertices, linewidth=2, color=contour_color
-            )
+            axes.add_patch(plt.Circle(
+                (self.y_grav_center, self.z_grav_center),
+                self.D/2,
+                color=contour_color,
+                fill=False,
+                linewidth=2,
+            ))
             ## plot axons
             circles = []
-            for k in range(self.N):
+            for k in range(self.n_ax):
                 if self.axons_type[k] == 1:  # myelinated
                     circles.append(
                         plt.Circle(
                             (self.axons_y[k], self.axons_z[k]),
                             self.axons_diameter[k] / 2,
                             color=myel_color,
                             fill=True,
@@ -991,43 +837,32 @@
                         plt.Circle(
                             (self.axons_y[k], self.axons_z[k]),
                             self.axons_diameter[k] / 2,
                             color=unmyel_color,
                             fill=True,
                         )
                     )
-            if self.extra_stim is not None:
-                for electrode in self.extra_stim.electrodes:
-                    if electrode.type == "LIFE":
-                        circles.append(
-                            plt.Circle(
-                                (electrode.y, electrode.z),
-                                electrode.D / 2,
-                                color="gold",
-                                fill=True,
-                            )
-                        )
-                    elif not is_FEM_electrode(electrode):
-                        axes.scatter(electrode.y, electrode.z, color="gold")
             for circle in circles:
                 axes.add_patch(circle)
+            if self.extra_stim is not None:
+                self.extra_stim.plot(axes=axes, color=elec_color, nerve_d=self.D)
             if num:
-                for k in range(self.N):
+                for k in range(self.n_ax):
                     axes.text(self.axons_y[k], self.axons_z[k], str(k))
+            axes.set_xlim((-1.1*self.D/2, 1.1*self.D/2))
+            axes.set_ylim((-1.1*self.D/2, 1.1*self.D/2))
 
     def plot_x(
-        self, fig, axes, myel_color="r", unmyel_color="b", Myelinated_model="MRG"
+        self, axes, myel_color="r", unmyel_color="b", Myelinated_model="MRG"
     ):
         """
         plot the fascicle's axons along Xline (longitudinal)
 
         Parameters
         ----------
-        fig     : matplotlib.figure
-            figure to display the fascicle
         axes    : matplotlib.axes
             axes of the figure to display the fascicle
         myel_color      : str
             matplotlib color string applied to the myelinated axons. Red by default
         unmyel_color    : str
             matplotlib color string applied to the myelinated axons. Blue by default
         Myelinated_model : str
@@ -1036,15 +871,15 @@
         if MCH.do_master_only_work():
             if self.L is None or self.NoR_relative_position != []:
                 drange = [
                     min(self.axons_diameter.flatten()),
                     max(self.axons_diameter.flatten()),
                 ]
                 polysize = np.poly1d(np.polyfit(drange, [0.5, 5], 1))
-                for k in range(self.N):
+                for k in range(self.n_ax):
                     relative_pos = self.NoR_relative_position[k]
                     d = round(self.axons_diameter.flatten()[k], 2)
                     if self.axons_type.flatten()[k] == 0.0:
                         color = unmyel_color
                         size = polysize(d)
                         axes.plot([0, self.L], np.ones(2) + k - 1, color=color, lw=size)
                     else:
@@ -1070,19 +905,19 @@
                         )
 
                 ## plot electrode(s) if existings
                 if self.extra_stim is not None:
                     for electrode in self.extra_stim.electrodes:
                         if not is_FEM_electrode(electrode):
                             axes.plot(
-                                electrode.x * np.ones(2), [0, self.N - 1], color="gold"
+                                electrode.x * np.ones(2), [0, self.n_ax - 1], color="gold"
                             )
                 axes.set_xlabel("x (um)")
                 axes.set_ylabel("axon ID")
-                axes.set_yticks(np.arange(self.N))
+                axes.set_yticks(np.arange(self.n_ax))
                 axes.set_xlim(0, self.L)
                 plt.tight_layout()
 
     ## Context handling methods
     def clear_context(
         self, extracel_context=True, intracel_context=True, rec_context=True
     ):
@@ -1115,31 +950,65 @@
 
         Parameters
         ----------
             stimulation  : stimulation object, see Extracellular.stimulation help for more details
         """
         if is_extra_stim(stimulation):
             self.extra_stim = stimulation
-        # remove everlaping axons
+        # remove overlaping axons
         for electrode in stimulation.electrodes:
             self.remove_axons_electrode_overlap(electrode)
 
-    def change_stimulus_from_elecrode(self, ID_elec, stimulus):
+    def remove_axons_electrode_overlap(self, electrode):
+        """
+        Remove the axons that could overlap an electrode
+
+        Parameters
+        ----------
+        electrode : object
+            electrode instance, see electrodes for more details
+        """
+        y, z, D = 0, 0, 0
+        # CUFF electrodes do not affect intrafascicular state
+        if not is_CUFF_electrode(electrode):
+            y = electrode.y
+            z = electrode.z
+            if is_LIFE_electrode(electrode):
+                D = electrode.D
+            # compute the distance of all axons to electrode
+            D_vectors = np.sqrt((self.axons_y - y) ** 2 + (self.axons_z - z) ** 2) - (
+                self.axons_diameter / 2 + D / 2
+            )
+            colapse = np.argwhere(D_vectors < 0)
+            mask = np.ones(len(self.axons_diameter), dtype=bool)
+            mask[colapse] = False
+            # remove axons colliding the electrode
+            if len(colapse) > 0:
+                pass_info(
+                    f"From Fascicle {self.ID}: Electrode/Axons overlap, {len(colapse)} axons will be removed from the fascicle"
+                )
+                pass_info(self.n_ax, " axons remaining")
+            self.axons_diameter = self.axons_diameter[mask]
+            self.axons_type = self.axons_type[mask]
+            self.axons_y = self.axons_y[mask]
+            self.axons_z = self.axons_z[mask]
+
+    def change_stimulus_from_electrode(self, ID_elec, stimulus):
         """
         Change the stimulus of the ID_elec electrods
 
         Parameters
         ----------
             ID_elec  : int
                 ID of the electrode which should be changed
             stimulus  : stimulus
                 new stimulus to set
         """
         if self.extra_stim is not None:
-            self.extra_stim.change_stimulus_from_elecrode(ID_elec, stimulus)
+            self.extra_stim.change_stimulus_from_electrode(ID_elec, stimulus)
         else:
             rise_warning("Cannot be changed: no extrastim in the fascicle")
 
     def insert_I_Clamp(self, position, t_start, duration, amplitude, ax_list=None):
         """
         Insert a IC clamp stimulation
 
@@ -1161,15 +1030,15 @@
         self.intra_stim_t_start.append(t_start)
         self.intra_stim_duration.append(duration)
         self.intra_stim_amplitude.append(amplitude)
         self.intra_stim_ON.append(ax_list)
         self.N_intra += 1
 
     ## RECORDING MECHANIMS
-    def attach_extracellular_recorder(self, rec):
+    def attach_extracellular_recorder(self, rec:recorder):
         """
         attach an extracellular recorder to the axon
 
         Parameters
         ----------
         rec     : recorder object
             see Recording.recorder help for more details
@@ -1202,15 +1071,15 @@
         ----------
         x    : float
             x axsis value (um) on which node are lined, by default 0
         """
         # also generated for unmyelinated but the meaningless value won't be used
         self.NoR_relative_position = []
 
-        for i in range(self.N):
+        for i in range(self.n_ax):
             if self.axons_type.flatten()[i] == 0.0:
                 self.NoR_relative_position += [0.0]
             else:
                 d = round(self.axons_diameter.flatten()[i], 2)
                 node_length = get_MRG_parameters(d)[5]
                 self.NoR_relative_position += [(x - 0.5) % node_length / node_length]
                 # -0.5 to be at the node of Ranvier center as a node is 1um long
@@ -1483,15 +1352,15 @@
             fasc_sim    : sim_results
                 results of the simulation
         """
         if self.postproc_script is not None:
             import nrv  # not ideal at all but gives direct acces to nrv in the postprocessing script
         fasc_sim = super().simulate(**kwargs)
         if not MCH.do_master_only_work():
-            fasc_sim = sim_results({})
+            fasc_sim = sim_results({"dummy_res":1})
         # disable the result storage only if results are fully return
         # To use with caution (mostly for optimisatino)
         if not self.save_results:
             if self.return_parameters_only:
                 rise_warning(
                     "Fascicle's simulation parameters are misused",
                     "results are neither saved or return",
@@ -1629,20 +1498,27 @@
             if self.record:
                 self.recorder.gather_all_recordings(master_computed=False)
         ###### NO STIM OR ANALYTICAL STIM: all in parallel, OR FEM STIM NO PARALLEL
         else:
             is_master_slave = False
             ## split the job between Cores/Computation nodes
             this_core_mask = MCH.split_job_from_arrays(len(self.axons_diameter))
+            ## Set pbar
+            has_pbar = False
+            if self.verbose:
+                if "pbar" in kwargs:
+                    _pbar = kwargs["pbar"]
+                    _pbar.reset(n_tot=len(this_core_mask))
+                    self.verbose = False
+                else:
+                    pass_info("Simulating axons in fascicle " + str(self.ID))
+                    _pbar = pbar(n_tot=len(this_core_mask))
+                has_pbar = True
             ## perform simulations
-            if MCH.is_alone() and self.verbose:
-                pass_info("Simulating axons in fascicle " + str(self.ID))
             for k in this_core_mask:
-                if MCH.is_alone() and self.verbose:
-                    pass_info("\t Axon " + f"{k+1}" + "/" + str(self.N), end="\r")
                 axon_sim = self.__sim_axon(k, is_master_slave)
                 # postprocessing and data reduction
                 # (cannot be added to __sim.axon beceause nrv would not be global anymore)
                 if self.postproc_script.lower() in OTF_PP_library:
                     self.postproc_script = OTF_PP_path + self.postproc_script.lower()
                 elif self.postproc_script.lower() + ".py" in OTF_PP_library:
                     self.postproc_script = (
@@ -1654,19 +1530,26 @@
                 ## store results
                 if self.save_results:
                     ax_fname = "sim_axon_" + str(k) + ".json"
                     # save_axon_results_as_json(axon_sim, folder_name + "/" + ax_fname)
                     axon_sim.save(save=True, fname=folder_name + "/" + ax_fname)
                 if not self.return_parameters_only:
                     fasc_sim.update({"axon" + str(k): axon_sim})
+                if has_pbar:
+                    _pbar.update()
             # sum up all recorded extracellular potential if applicable
             synchronize_processes()
             if self.record:
                 self.recorder.gather_all_recordings()
         if not self.return_parameters_only:
             synchronize_processes()
             fasc_sim = MCH.gather_jobs(fasc_sim)
+            if MCH.do_master_only_work():
+                if "extra_stim" in fasc_sim:
+                    fasc_sim['extra_stim'] = load_any(fasc_sim['extra_stim']) #dirty hack to force NRV_class instead of dict
+                if self.record:
+                    fasc_sim['recorder'] = load_any(fasc_sim['recorder'])   #idem
         if MCH.is_alone() and self.verbose:
             pass_info("... Simulation done")
             fasc_sim["is_simulated"] = True
         self.is_simulated = True
         return fasc_sim
```

### Comparing `nrv-py-1.0.1/nrv/nmod/myelinated.py` & `nrv_py-1.1.0/nrv/nmod/myelinated.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,22 +58,25 @@
     else:
         # create fiting polynomyals
         g_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_g, 3))
         axonD_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_axonD, 3))
         nodeD_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_nodeD, 3))
         paraD1_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_paraD1, 3))
         paraD2_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_paraD2, 3))
-        deltax_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_deltax, 4))
-        if diameter < 1.0 or diameter > 16.0:
+        
+        if diameter < 1.0 or diameter > 14.0:
             # outside of the MRG originla limit, take 1st order approx,
-            paralength2_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_paralength2, 1))
+            paralength2_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_paralength2, 3))
+            deltax_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_deltax, 2))        
         else:
             # try to fit a bit better
             paralength2_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_paralength2, 5))
+            deltax_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_deltax, 5))
         nl_poly = np.poly1d(np.polyfit(MRG_fiberD, MRG_nl, 3))
+
         # evaluate for the requested diameter
         g = g_poly(diameter)
         axonD = axonD_poly(diameter)
         nodeD = nodeD_poly(diameter)
         paraD1 = paraD1_poly(diameter)
         paraD2 = paraD2_poly(diameter)
         deltax = deltax_poly(diameter)
@@ -183,15 +186,15 @@
         y=0,
         z=0,
         d=10,
         L=10000,
         model="MRG",
         dt=0.001,
         node_shift=0,
-        Nseg_per_sec=0,
+        Nseg_per_sec=1,
         freq=100,
         freq_min=0,
         mesh_shape="plateau_sigmoid",
         alpha_max=0.3,
         d_lambda=0.1,
         rec="nodes",
         v_init=None,
@@ -595,14 +598,28 @@
             fname=fname,
             extracel_context=extracel_context,
             intracel_context=intracel_context,
             rec_context=rec_context,
             blacklist=blacklist,
         )
 
+    def plot(self, axes: plt.axes, color: str="red", node_color: str="lightgray", elec_color="gold", **kwgs) -> None:
+        super().plot(axes, color, elec_color,**kwgs)
+        alpha = 1
+        if "alpha" in kwgs:
+            alpha = kwgs["alpha"]
+
+        axes.add_patch(plt.Circle(
+            (self.y, self.z),
+            self.nodeD / 2,
+            fc=node_color,
+            fill=True,
+            alpha = alpha,
+        ))
+
     def __set_model(self, model):
         """
         Set the double cable model. For internal use only.
 
         Parameters
         ----------
         model           : str
@@ -777,23 +794,23 @@
             if self.freq_min == 0:
                 # uniform meshing
                 for n in self.node:
                     Nseg = d_lambda_rule(n.L, self.d_lambda, self.freq, n)
                     n.nseg = Nseg
                     self.node_Nseg += Nseg
                 for m in self.MYSA:
-                    Nseg = Nseg = d_lambda_rule(m.L, self.d_lambda, self.freq, m)
+                    Nseg = d_lambda_rule(m.L, self.d_lambda, self.freq, m)
                     m.nseg = Nseg
                     self.MYSA_Nseg += Nseg
                 for f in self.FLUT:
-                    Nseg = Nseg = d_lambda_rule(f.L, self.d_lambda, self.freq, f)
+                    Nseg = d_lambda_rule(f.L, self.d_lambda, self.freq, f)
                     f.nseg = Nseg
                     self.FLUT_Nseg += Nseg
                 for s in self.STIN:
-                    Nseg = Nseg = d_lambda_rule(s.L, self.d_lambda, self.freq, s)
+                    Nseg = d_lambda_rule(s.L, self.d_lambda, self.freq, s)
                     s.nseg = Nseg
                     self.STIN_Nseg += Nseg
             else:
                 # non-uniform meshing
                 freqs = create_Nseg_freq_shape(
                     self.Nsec, self.mesh_shape, self.freq, self.freq_min, self.alpha_max
                 )
```

### Comparing `nrv-py-1.0.1/nrv/nmod/nerve.py` & `nrv_py-1.1.0/nrv/nmod/nerve.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,74 +22,61 @@
     A nerve can be instrumented by adding couples of electrodes+stimulus
 
     The extracellular context of the nerve is automatically generated from the context of its
     fascicles and an optional context added directly to the nerve.
 
     Parameters
     ----------
-    dt              : float
-        simulation time stem for Neuron (ms), by default 1us
-    Nseg_per_sec    : float
-        number of segment per section in Neuron. If set to 0, the number of segment per section is calculated with the d-lambda rule
-    freq            : float
-        frequency of the d-lambda rule (Hz), by default 100Hz
-    freq_min        : float
-        minimum frequency for the d-lambda rule when meshing is irregular, 0 for regular meshing
-    v_init          : float
-        initial value for the membrane voltage (mV), specify None for automatic model choice of v_init
-    T               : float
-        temperature (C), specify None for automatic model choice of temperature
-    ID              : int
-        axon ID, by default set to 0
-    threshold       : int
-        membrane voltage threshold for spike detection (mV), by default -40mV
-    Adelta_limit    : float
-        limit diameter between A-delta models (thin myelinated) and myelinated models for axons
+    length              : float
+        Nerve length, in um
+    diameter    : float
+        Nerve diameter, in um
+    Outer_D            : float
+        Outer saline box diameter, in mm
+    ID        : int
+        Nerve unique identifier 
     """
 
-    def __init__(self, Length=10000, Diameter=100, Outer_D=5, ID=0, **kwargs):
+    def __init__(self, length=10_000, diameter=100, Outer_D=5, ID=0, **kwargs):
         """
         Instanciates an empty nerve.
         """
-        super().__init__()
+        super().__init__(**kwargs)
 
         # to add to a fascicle/nerve common mother class
         self.save_path = ""
-        self.verbose = False
+        self.verbose = True
         self.postproc_script = "default"
         self.return_parameters_only = True
+        self.save_results = True
         self.loaded_footprints = True
 
         self.type = "nerve"
-        self.L = Length
-        self.D = Diameter
+        self.L = length
+        self.D =  None
         self.y_grav_center = 0
         self.z_grav_center = 0
         self.Outer_D = Outer_D
         self.ID = ID
 
         # geometric properties
         self.y_grav_center = 0
         self.z_grav_center = 0
-        self.N_vertices = 0
-        self.y_vertices = np.array([])
-        self.z_vertices = np.array([])
 
         # Fascicular content
-        self.N_ax = 0
         self.fascicles_IDs = []
         self.fascicles = {}
 
         # Axons objects default parameters
         self.unmyelinated_param = {
             "model": "Rattay_Aberham",
             "dt": 0.001,
             "Nrec": 0,
             "Nsec": 1,
-            "Nseg_per_sec": 100,
+            "Nseg_per_sec": length//25,
             "freq": 100,
             "freq_min": 0,
             "mesh_shape": "plateau_sigmoid",
             "alpha_max": 0.3,
             "d_lambda": 0.1,
             "v_init": None,
             "T": None,
@@ -116,28 +103,32 @@
         # extra-cellular stimulation
         self.extra_stim = None
         self.is_extra_stim = False
         self.added_extra_stims = []
         self.footprints = {}
         self.is_footprinted = False
         self.myelinated_nseg_per_sec = 3
-        self.unmyelinated_nseg = 100
+        self.unmyelinated_nseg = length//25
         # intra-cellular stimulation
         self.N_intra = 0
         self.intra_stim_position = []
         self.intra_stim_t_start = []
         self.intra_stim_duration = []
         self.intra_stim_amplitude = []
         self.intra_stim_ON = []
         ## recording mechanism
         self.record = False
         self.recorder = None
         self.is_simulated = False
         # Simulation status
 
+
+        self.define_circular_contour(diameter)
+
+
     ## save/load methods
     def save(
         self,
         fname="nerve.json",
         extracel_context=False,
         intracel_context=False,
         rec_context=False,
@@ -259,33 +250,50 @@
             blacklist=bl,
             extracel_context=extracel_context,
             intracel_context=intracel_context,
             rec_context=rec_context,
         )
 
     ## Nerve property method
+    @property
+    def n_fasc(self):
+        return len(self.fascicles)
+
+    def get_n_ax(self, id_fasc=None):
+        n = 0
+        if id_fasc is None:
+            id_fasc = self.fascicles.keys()
+        elif not np.iterable(id_fasc):
+            id_fasc = [id_fasc]
+        for i_fasc in id_fasc:
+            if i_fasc in self.fascicles:
+                fasc = self.fascicles[i_fasc]
+                n += fasc.n_ax
+        return n
+    n_ax = property(get_n_ax)
+
     def set_ID(self, ID):
         """
-        set the ID of the fascicle
+        set the ID of the nerve
 
         Parameters
         ----------
         ID : int
-            ID number of the fascicle
+            ID number of the nerve
         """
         self.ID = ID
 
     def define_length(self, L):
         """
-        set the length over the x axis of the fascicle
+        set the length over the x axis of the nerve
 
         Parameters
         ----------
         L   : float
-            length of the fascicle in um
+            length of the nerve in um
         """
         if self.extra_stim is not None or self.N_intra > 0:
             rise_warning(
                 "Modifying length of a fascicle with extra or intra cellular context can lead to error"
             )
         self.L = L
         self.set_axons_parameters(unmyelinated_nseg=self.L // 25)
@@ -294,109 +302,95 @@
                 Nerve_D=self.D,
                 Length=self.L,
                 y_c=self.y_grav_center,
                 z_c=self.z_grav_center,
             )
 
     ## generate stereotypic Nerve
-    def define_circular_contour(self, D, y_c=None, z_c=None, N_vertices=100):
+    def define_circular_contour(self, D, y_c=None, z_c=None):
         """
-        Define a circular countour to the fascicle
+        Define a circular countour to the nerve
 
         Parameters
         ----------
         D           : float
-            diameter of the circular fascicle contour, in um
+            diameter of the circular nerve contour, in um
         y_c         : float
             y coordinate of the circular contour center, in um
         z_c         : float
             z coordinate of the circular contour center, in um
-        N_vertices  : int
-            Number of vertice in the compute the contour
         """
         self.type = "Circular"
         self.D = D
         if y_c is not None:
             self.y_grav_center = y_c
         if z_c is not None:
             self.z_grav_center = z_c
-        self.N_vertices = N_vertices
-        theta = np.linspace(-np.pi, np.pi, num=N_vertices)
-        self.y_vertices = self.y_grav_center + (D / 2) * np.cos(theta)
-        self.z_vertices = self.z_grav_center + (D / 2) * np.sin(theta)
         self.A = np.pi * (D / 2) ** 2
         if self.is_extra_stim:
+            pass_info("FEM nerve resized!")
             self.extra_stim.reshape_nerve(
                 Nerve_D=self.D,
                 Length=self.L,
                 y_c=self.y_grav_center,
                 z_c=self.z_grav_center,
             )
 
     def get_circular_contour(self):
         """
-        Returns the properties of the fascicle contour considered as a circle (y and z center and diameter)
+        Returns the properties of the nerve contour considered as a circle (y and z center and diameter)
 
         Returns
         -------
         D : float
             diameter of the contour, in um. Set to 0 if not applicable
         y : float
             y position of the contour center, in um
         z : float
             z position of the contour center, in um
         """
         y = self.y_grav_center
         z = self.z_grav_center
-        if self.y_vertices == np.array([]) and self.D is None:
-            D = 0
-        elif self.D is not None:
-            D = self.D
-        else:
-            y = (np.amax(self.y_vertices) - np.amin(self.y_vertices)) / 2
-            z = (np.amax(self.z_vertices) - np.amin(self.z_vertices)) / 2
-            D = np.abs(np.amax(self.y_vertices) - np.amin(self.y_vertices))
+        D = self.D
         return D, y, z
 
-    def fit_circular_contour(self, y_c=None, z_c=None, Delta=20, N_vertices=100):
+    def fit_circular_contour(self, y_c=None, z_c=None, Delta=20):
         """
-        Define a circular countour to the fascicle
+        Define a circular countour to the nerve
 
         Parameters
         ----------
         y_c         : float
             y coordinate of the circular contour center, in um
         z_c         : float
             z coordinate of the circular contour center, in um
         Delta       : float
             distance between farest axon and contour, in um
-        N_vertices  : int
-            Number of vertice in the compute the contour
         """
         N_fasc = len(self.fascicles)
         D = 2 * Delta
 
         if y_c is not None:
             self.y_grav_center = y_c
         if z_c is not None:
             self.z_grav_center = z_c
         if N_fasc == 0:
-            pass_info("No fascicles to fit fascicul diameter set to " + str(D) + "um")
+            pass_info("No fascicles to fit - Nerve diameter set to " + str(D) + "um")
         else:
             for fasc in self.fascicles.values():
                 dist_max = (
                     fasc.D / 2
                     + (
                         (self.y_grav_center - fasc.y_grav_center) ** 2
                         + (self.z_grav_center - fasc.z_grav_center) ** 2
                     )
                     ** 0.5
                 )
                 D = max(D, 2 * (dist_max + Delta))
-        self.define_circular_contour(D, y_c=None, z_c=None, N_vertices=N_vertices)
+        self.define_circular_contour(D, y_c=None, z_c=None)
 
     def define_ellipsoid_contour(self, a, b, y_c=0, z_c=0, rotate=0):
         """
         Define ellipsoidal contour
         """
         pass
 
@@ -451,15 +445,15 @@
                 else:
                     self.fascicles_IDs += [fasc.ID]
                     self.fascicles[fasc.ID] = fasc
 
                 self.__merge_fascicular_context(self.fascicles[fasc.ID])
                 self.fascicles[fasc.ID].define_length(self.L)
 
-    def __check_fascicle_overlap(self, fasc):
+    def __check_fascicle_overlap(self, fasc:fascicle):
         for fasc_i in self.fascicles.values():
             dist_yz = (fasc.y_grav_center - fasc_i.y_grav_center) ** 2 + (
                 fasc.z_grav_center - fasc_i.z_grav_center
             ) ** 2
             len_min_yz = ((fasc.D + fasc_i.D) / 2) ** 2
             if dist_yz < len_min_yz:
                 return True
@@ -479,15 +473,15 @@
         fasc.clear_context(intracel_context=False)
 
     ## Axons handling method
     def set_axons_parameters(
         self, unmyelinated_only=False, myelinated_only=False, **kwargs
     ):
         """
-        set parameters of axons in the fascicle
+        set parameters of axons in the nerve
 
         Parameters
         ----------
         unmyelinated_only:      bool
             if true modification only done for unmyelinated axons parameters, by default False
         myelinated_only:        bool
             if true modification only done for myelinated axons parameters, by default False
@@ -501,17 +495,17 @@
                     self.unmyelinated_param["model"] = kwargs[key]
                 elif not unmyelinated_only and kwargs[key] in myelinated_models:
                     self.myelinated_param["model"] = kwargs[key]
                 else:
                     rise_warning(kwargs[key], " is not an implemented axon model")
             else:
                 if not myelinated_only and key in self.unmyelinated_param:
-                    self.unmyelinated_param["model"] = kwargs[key]
+                    self.unmyelinated_param[key] = kwargs[key]
                 if not unmyelinated_only and key in self.myelinated_param:
-                    self.myelinated_param["model"] = kwargs[key]
+                    self.myelinated_param[key] = kwargs[key]
 
         ## Specific keys
         if "unmyelinated_nseg" in kwargs:
             self.unmyelinated_param["Nseg_per_sec"] = kwargs["unmyelinated_nseg"]
         if "myelinated_nseg_per_sec" in kwargs:
             self.myelinated_param["Nseg_per_sec"] = kwargs["myelinated_nseg_per_sec"]
         if "Adelta_limit" in kwargs:
@@ -536,49 +530,56 @@
             return self.unmyelinated_param
         if myelinated_only:
             return self.myelinated_param
         return self.unmyelinated_param, self.myelinated_param
 
     ## Representation methods
     def plot(
-        self, fig, axes, contour_color="k", myel_color="r", unmyel_color="b", num=False
+        self, axes:plt.axes, contour_color:str="k", myel_color:str="r", unmyel_color:str="b", elec_color:str="gold",num:bool=False, **kwgs
     ):
         """
         plot the nerve in the Y-Z plane (transverse section)
 
         Parameters
         ----------
-        fig     : matplotlib.figure
-            figure to display the fascicle
         axes    : matplotlib.axes
             axes of the figure to display the fascicle
         contour_color   : str
             matplotlib color string applied to the contour. Black by default
         myel_color      : str
             matplotlib color string applied to the myelinated axons. Red by default
         unmyel_color    : str
             matplotlib color string applied to the myelinated axons. Blue by default
+        elec_color    : str
+            matplotlib color string applied to the electrodes axons. Blue by default
         num             : bool
             if True, the index of each axon is displayed on top of the circle
         """
         if MCH.do_master_only_work():
             ## plot contour
-            axes.plot(
-                self.y_vertices, self.z_vertices, linewidth=4, color=contour_color
-            )
+            axes.add_patch(plt.Circle(
+                (self.y_grav_center, self.z_grav_center),
+                self.D/2,
+                color=contour_color,
+                fill=False,
+                linewidth=4,
+            ))
             for i in self.fascicles:
                 fasc = self.fascicles[i]
                 fasc.plot(
-                    fig=fig,
                     axes=axes,
-                    contour_color=contour_color,
+                    contour_color="grey",
                     myel_color=myel_color,
                     unmyel_color=unmyel_color,
                     num=num,
                 )
+            if self.extra_stim is not None:
+                self.extra_stim.plot(axes=axes, color=elec_color, nerve_d=self.D)
+            axes.set_xlim((-1.1*self.D/2, 1.1*self.D/2))
+            axes.set_ylim((-1.1*self.D/2, 1.1*self.D/2))
 
     ## Context handling methods
     def clear_context(
         self, extracel_context=True, intracel_context=True, rec_context=True
     ):
         """
         Clear all stimulation and recording mecanism
@@ -601,15 +602,14 @@
         if rec_context:
             ## recording mechanism
             self.record = False
             self.recorder = None
         self.is_simulated = False
 
     # Intra cellular
-
     def insert_I_Clamp(self, position, t_start, duration, amplitude, ax_list=None):
         """
         Insert a IC clamp stimulation
 
         Parameters
         ----------
         position    : float
@@ -631,15 +631,14 @@
                 duration=duration,
                 amplitude=amplitude,
                 ax_list=ax_list,
             )
         self.N_intra += 1
 
     # Extracellular
-
     def attach_extracellular_stimulation(self, stimulation: FEM_stimulation):
         """
         attach a extracellular context of simulation for an axon.
 
         Parameters
         ----------
             stimulation  : stimulation object, see Extracellular.stimulation help for more details
@@ -666,32 +665,69 @@
                     y_c=fasc.y_grav_center,
                     z_c=fasc.z_grav_center,
                     ID=fasc.ID,
                 )
             self.is_extra_stim = True
 
         for i, elec in enumerate(stimulation.electrodes):
-            self.extra_stim.add_electrode(elec, stimulation.stimuli[i])
+            _overlap = self.__check_perineurium_electrode_overlap(elec)
+            if _overlap == -1:
+                self.extra_stim.add_electrode(elec, stimulation.stimuli[i])
+                for fasc in self.fascicles.values():
+                        fasc.remove_axons_electrode_overlap(elec)
+            else:
+                rise_warning(f"Electrode {i} ovelerlap with the perineurium the fascicle {_overlap}")
+
 
-    def change_stimulus_from_elecrode(self, ID_elec, stimulus):
+    def change_stimulus_from_electrode(self, ID_elec, stimulus):
         """
         Change the stimulus of the ID_elec electrods
 
         Parameters
         ----------
             ID_elec  : int
                 ID of the electrode which should be changed
             stimulus  : stimulus
                 New stimulus to set
         """
         if self.extra_stim is not None:
-            self.extra_stim.change_stimulus_from_elecrode(ID_elec, stimulus)
+            self.extra_stim.change_stimulus_from_electrode(ID_elec, stimulus)
         else:
             rise_warning("Cannot be changed: no extrastim in the nerve")
 
+    def __check_perineurium_electrode_overlap(self, electrode:electrode)->int:
+        """
+        Check if an electrode overlap with one fascicle perineurium of the nerve.
+
+        Paramters
+        ---------
+        electrode   : electrode
+            electrode to check
+        
+        Returns
+        -------
+        int
+            ID of the fascicle overlapping, -1 if no overlap
+        """
+        y, z, D = 0, 0, 0
+        # CUFF electrodes do not affect intrafascicular state
+        if not is_CUFF_electrode(electrode):
+            y = electrode.y
+            z = electrode.z
+            if is_LIFE_electrode(electrode):
+                D = electrode.D
+            for fasc in self.fascicles.values():
+                dist = np.sqrt((fasc.y_grav_center - y) ** 2 + (fasc.z_grav_center - z) ** 2) - (
+                    fasc.D / 2
+                )
+                if abs(dist) < D:
+                    return fasc.ID
+        return -1
+
+
     # RECORDING MECHANIMS
     def attach_extracellular_recorder(self, rec: recorder):
         """
         attach an extracellular recorder to the axon
 
         Parameters
         ----------
@@ -728,15 +764,20 @@
             fasc.record_V_mem = self.record_V_mem
             fasc.record_I_mem = (self.record_I_mem,)
             fasc.record_I_ions = self.record_I_ions
             fasc.record_g_mem = self.record_g_mem
             fasc.record_g_ions = self.record_g_ions
             fasc.record_particles = self.record_particles
             fasc.postproc_script = self.postproc_script
+            fasc.save_results = self.save_results,
+            fasc.return_parameters_only = self.return_parameters_only
+            fasc.verbose = self.verbose
 
+
+    # Footprint and mesh
     def compute_electrodes_footprints(self, **kwargs):
         """
         compute electrodes footprints
         """
         if not self.is_footprinted:
             self.__set_fascicles_context()
             self.set_axons_parameters(**kwargs)
@@ -749,14 +790,15 @@
                     )
                     if MCH.do_master_only_work() or mp_computation:
                         self.extra_stim.run_model()
                 for fasc in self.fascicles.values():
                     fasc.compute_electrodes_footprints()
             self.is_footprinted = True
 
+
     ## SIMULATION
     def simulate(
         self,
         **kwargs,
     ):
         """
         Simulate the nerve with the proposed extracellular context. Top level method for large
@@ -766,34 +808,54 @@
         ----------
 
         Warning
         -------
         calling this method can result in long processing time, even with large computational ressources.
         Keep aware of what is really implemented, ensure configuration and simulation protocol is correctly designed.
         """
-        pass_info("Starting nerve simulation")
+        if self.verbose:
+            pass_info("Starting nerve simulation")
         nerve_sim = super().simulate(**kwargs)
         self.__set_fascicles_simulation_parameters()
         if not MCH.do_master_only_work():
-            nerve_sim = {}
-        folder_name = self.save_path + "Nerve_" + str(self.ID) + "/"
-        if MCH.do_master_only_work():
-            create_folder(folder_name)
-            config_filename = folder_name + "/00_Nerve_config.json"
-            self.save(config_filename, fascicles_context=False)
-        else:
-            pass
+            nerve_sim = sim_results({"dummy_res":1})
+        if self.save_results:
+            folder_name = self.save_path + "Nerve_" + str(self.ID) + "/"
+            if MCH.do_master_only_work():
+                create_folder(folder_name)
+                config_filename = folder_name + "/00_Nerve_config.json"
+                self.save(config_filename, fascicles_context=False)
+            else:
+                pass
         # run FEM model
-        pass_info("...computing electrodes footprint")
+        if self.verbose:
+            pass_info("...computing electrodes footprint")
         self.compute_electrodes_footprints(**kwargs)
         synchronize_processes()
         # Simulate all fascicles
         fasc_kwargs = kwargs
-        fasc_kwargs["save_path"] = folder_name
+        if self.save_results:
+            fasc_kwargs["save_path"] = folder_name
+        has_pbar = False
+        if self.verbose:
+            i_pbar = 1
+            _pbar = pbar(n_tot=self.n_fasc, label="fasc")
+            has_pbar = True
         for fasc in self.fascicles.values():
-            pass_info("...simulating fascicle " + str(fasc.ID))
+            if has_pbar:
+                _pbar.set_label(f"fascicle {i_pbar}/{self.n_fasc}")
+                i_pbar += 1
+                fasc_kwargs["pbar"] = _pbar
             nerve_sim["fascicle" + str(fasc.ID)] = fasc.simulate(
-                in_nerve=True,
-                **fasc_kwargs,
+                in_nerve=True, **fasc_kwargs,
             )
+        if has_pbar:
+            del _pbar
+        if self.verbose:
+            pass_info("...Done!")
+        #dirty hack to force NRV_class type when saved
+        if "extra_stim" in nerve_sim:
+            nerve_sim["extra_stim"] = load_any(nerve_sim["extra_stim"])
+        if self.record:     # recorder not saved in result !!BUG
+            nerve_sim["recorder"] = self.recorder
         self.is_simulated = True
         return nerve_sim
```

### Comparing `nrv-py-1.0.1/nrv/nmod/unmyelinated.py` & `nrv_py-1.1.0/nrv/nmod/unmyelinated.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,25 +608,25 @@
         setup the ionic currents recording. For internal use only.
         """
         if self.model in ["HH", "Rattay_Aberham", "Sundt"]:
             self.i_na_reclist = neuron.h.List()
             self.i_k_reclist = neuron.h.List()
             self.i_l_reclist = neuron.h.List()
             self.__set_recorders_with_key(
-                (self.i_na_reclist, "_ref_nai"),
-                (self.i_k_reclist, "_ref_ki"),
+                (self.i_na_reclist, "_ref_ina"),
+                (self.i_k_reclist, "_ref_ik"),
                 (self.i_l_reclist, "_ref_i_pas"),
             )
         else:
             self.i_na_reclist = neuron.h.List()
             self.i_k_reclist = neuron.h.List()
             self.i_ca_reclist = neuron.h.List()
             self.__set_recorders_with_key(
-                (self.i_na_reclist, "_ref_nai"),
-                (self.i_k_reclist, "_ref_ki"),
+                (self.i_na_reclist, "_ref_ina"),
+                (self.i_k_reclist, "_ref_ik"),
                 (self.i_ca_reclist, "_ref_cai"),
             )
 
     def get_ionic_current(self):
         """
         get the ionic currents at the end of simulation. For internal use only.
         """
```

### Comparing `nrv-py-1.0.1/nrv/nrv2calm` & `nrv_py-1.1.0/nrv/nrv2calm`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/optim/Optimizers.py` & `nrv_py-1.1.0/nrv/optim/Optimizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,42 +30,134 @@
 class Optimizer(NRV_class, metaclass=ABCMeta):
     @abstractmethod
     def __init__(self, method=None):
         super().__init__()
         self._method = method
         self.swarm_optimizer = False
 
-    def minimize(self, f, **kwargs):
+    def minimize(self, f:callable, **kwargs)->optim_results:
+        """
+        Minimze the function ``f`` using the `optimzer`'s parameters
+
+        Parameters
+        ----------
+        f : callable
+            function to minimize
+        kwargs                  : dict
+            containing parameters to change in the class (:class:``PSO_optimizer``)
+
+        Returns
+        -------
+        optim_results
+            results of the optimization
+        """
         self.set_parameters(**kwargs)
         results = optim_results(self.save(save=False))
         results["date"] = asctime(localtime())
         results["status"] = "Processing"
         return results
 
-    def __call__(self, f, **kwargs: Any) -> optim_results:
+    def __call__(self, f:callable, **kwargs: Any) -> optim_results:
         return self.minimize(f, **kwargs)
 
 
 class scipy_optimizer(Optimizer):
+
+    """
+    
+
+    Parameters
+    ----------
+    method : str | callable, optional
+        Type of solver.  Should be one of
+            - 'Nelder-Mead'
+            - 'Powell'
+            - 'CG'
+            - 'BFGS'
+            - 'Newton-CG'
+            - 'L-BFGS-B'
+            - 'TNC'
+            - 'COBYLA'
+            - 'SLSQP'
+            - 'trust-constr'
+            - 'dogleg'
+            - 'trust-ncg'
+            - 'trust-exact'
+            - 'trust-krylov'
+            - custom - a callable object
+
+    x0 : np.ndarray, optional
+        Initial guess. Array of real elements of size (n,), where n is the number of independent variables,. by default None
+    args : tuple, optional
+        Extra arguments passed to the objective function and its derivatives (fun, jac and hess functions), by default ()
+    jac : {callable,  '2-point', '3-point', 'cs', bool}, optional
+        Method for computing the gradient vector, optional
+        _description_, by default None
+    hess : {callable, '2-point', '3-point', 'cs', HessianUpdateStrategy}, optional
+        Method for computing the Hessian matrix, by default None
+    hessp : callable, optional
+        Hessian of objective function times an arbitrary vector p. Only for
+        Newton-CG, trust-ncg, trust-krylov, trust-constr, by default None
+    bounds : sequence or `Bounds`, optional
+        Bounds on variables for Nelder-Mead, L-BFGS-B, TNC, SLSQP, Powell,
+        trust-constr, and COBYLA methods., by default None
+    constraints : {Constraint, dict} or List of {Constraint, dict}, optional
+        Constraints definition. Only for COBYLA, SLSQP and trust-constr, by default ()
+    tol : float, optional
+        Tolerance for termination, by default None
+    callback : callable, optional
+        A callable called after each iteration, by default None
+    maxiter : int, optional
+        _description_, by default None
+    options : dict, optional
+        A dictionary of solver options, by default None
+    dimension : int, optional
+        _description_, by default None
+    normalize : bool, optional
+        _description_, by default False
+
+    Note
+    ----
+    The following arguments are those used in scipy.optimize.minimize (see scipy documentation [2] for more informations): ``x0``, ``args``, ``jac``, ``hess``, ``hessp``, ``bounds``, ``constraints``, ``tol``, ``callback``, ``options``
+
+    Examples
+    --------
+    The following lines shows how `scipy_optimizer` can be used to minimze a 2D sphere function.
+
+    >>> import nrv
+    >>> my_cost1 = nrv.sphere()
+    >>> my_opt = nrv.scipy_optimizer(dimension=2, x0= [100, 10], maxiter=10)
+    >>> res = my_opt.minimize(my_cost1)
+    >>> print("best position",res.x, "best cost", res.best_cost)
+
+        best position [-1.52666570e-08 -1.32835147e-07] best cost 1.337095622502969e-07
+
+
+    References
+    ----------
+    [1] `scipy <https://docs.scipy.org/doc/scipy/>`_
+
+    [2] `scipy.optimize.minimize <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html#scipy.optimize.minimize>`_
+    """
     def __init__(
         self,
-        method=None,
-        x0=None,
-        args=(),
-        jac=None,
-        hess=None,
-        hessp=None,
-        bounds=None,
-        constraints=(),
-        tol=None,
-        callback=None,
-        maxiter=None,
-        options=None,
-        dimension=None,
-        normalize=False,
+        method:str=None,
+        x0:np.ndarray=None,
+        args:tuple=(),
+        jac:callable=None,
+        hess:callable=None,
+        hessp:callable=None,
+        bounds:tuple=None,
+        constraints:dict=(),
+        tol:float=None,
+        callback:callable=None,
+        maxiter:int=None,
+        options:dict=None,
+        dimension:int=None,
+        normalize:bool=False,
     ):
         if method is None:
             super().__init__("scipy_default")
         else:
             super().__init__("scipy_" + method)
         self.x0 = x0
         self.args = args
@@ -122,15 +214,15 @@
                 self.scaled_bounds += [(0, 1)]
                 self.scale_translation[i] = bd[0]
                 self.scale_homothety[i] = bd[1] - bd[0]
         results["scale_translation"] = self.scale_translation
         results["scale_homothety"] = self.scale_homothety
         results["scaled_bounds"] = self.scaled_bounds
 
-    def minimize(self, f, **kwargs):
+    def minimize(self, f:callable, **kwargs)->optim_results:
         results = super().minimize(f, **kwargs)
         if self.maxiter is not None:
             self.options["maxiter"] = self.maxiter
         self.__update_dimensions(results)
         self.__normalize_bound(results)
         results["cost_history"] = []
         results["position_history"] = []
@@ -169,101 +261,108 @@
         if "hess_inv" in results:
             del results["hess_inv"]
         results["status"] = "Completed"
         return results
 
 
 class PSO_optimizer(Optimizer):
+    """
+    Perform a Particle swarm optimization (PSO) on with a defined cost function using pyswarms
+    library[1]
+
+    Parameters
+    ----------
+    n_particles           	: int
+        number of particle of the swarm, by default 5
+    dimensions              : int
+        number of dimensions of each particle
+    options                 : dict
+        hyperparameter of the PSO
+    maxiter                    : int
+        number of iteration of the PSO
+    n_processes             : int
+        number of process used to parallelize cost calculation, by default None
+    bounds                  : tupple
+        bounds of the particle, if equal no bounds, by default (0, 0)
+    init_pos                : array
+        initial position of the particles if None random, by default None
+    print_time              : bool
+        if True, print the optimisation time, by default True
+    opt_type                : str
+        Neightboorhood type, by default "global"
+        type possibly:
+
+            - "global"                : Global best PSO (star topology)
+            - "local"                 : Local best PSO (ring topology)
+
+    static      : bool
+        if False and opt_type is local, update the neigthboorhood of each particle every iterations
+    bh_strategy             : str
+        out of bound position strategy for pyswarms optimizer [2]:
+
+            - "nearest"               : Round the value to the nearest bound (default)
+            - "periodic"              : set to the modulus of the value between the two bounds
+            - "random"                : set to a random value
+            - "shrink"                : reduce the velocity to finish land on the bound
+            - "reflective"            : mirror the position form inside to ouside the bounds
+            - "intermediate"          : set to intermediate value between previous pos and bound
+
+    oh_strategy             : dict (like {"w":str, "c1":str, "c2":str})
+        Dynamic options strategy for pyswarms optimizer [3], if None static options,
+        by default None:
+
+            - "exp_decay"             : Decreases the parameter exponentially between limits
+            - "lin_variation"         : Decreases/increases the parameter linearly between limits
+            - "nonlin_mod"            : Decreases/increases the parameter between limits
+                                    according to a nonlinear modulation index
+            - "rand"                  : takes a uniform random value between limits
+
+    ftol                    : float
+        relative error in objective_func(best_pos) acceptable for convergence, if None -np.inf
+        default None
+    ftol                    : int
+        number of iterations over which the relative error in objective_func(best_pos) is
+        acceptable for convergence, by default 1
+    save_results            : bool
+        save or not the output in a .json file, by default False
+    saving_file             : str
+        name of the file on wich the output should be saved, by default "pso_results.json"
+
+    Returns
+    -------
+    results     : optim_results
+        contains all the parameters and outputs of the PSO
+
+    References
+    ----------
+    links to pyswarms doc:
+        [1] `Pyswams <https://pyswarms.readthedocs.io/en/latest/index.html>`_
+
+        [2] `Pyswams handlers <https://pyswarms.readthedocs.io/en/latest/api/pyswarms.handlers.html>`_
+    """
     def __init__(
         self,
         n_particles=5,
+        bounds=(0, 0),
         dimensions=50,
         options=None,
         maxiter=1,
         n_processes=None,
-        bounds=(0, 0),
         init_pos=None,
         print_time=False,
         opt_type="global",
         static=False,
         ftol=None,
         ftol_iter=1,
         bh_strategy="nearest",
         oh_strategy=None,
         save_results=False,
         saving_file="pso_results.json",
         comment=None,
     ):
-        """
-        Perform a Particle swarm optimization (PSO) on with a defined cost function using pyswarms
-        library[1]
-
-        Parameters
-        ----------
-        n_particles           	: int
-            number of particle of the swarm, by default 5
-        dimensions              : int
-            number of dimensions of each particle
-        options                 : dict
-            hyperparameter of the PSO
-        maxiter                    : int
-            number of iteration of the PSO
-        n_processes             : int
-            number of process used to parallelize cost calculation, by default None
-        bounds                  : tupple
-            bounds of the particle, if equal no bounds, by default (0, 0)
-        init_pos                : array
-            initial position of the particles if None random, by default None
-        print_time              : bool
-            if True, print the optimisation time, by default True
-        opt_type                : str
-            Neightboorhood type, by default "global"
-            type possibly:
-                    "global"                : Global best PSO (star topology)
-                    "local"                 : Local best PSO (ring topology)
-        static      : bool
-            if False and opt_type is local, update the neigthboorhood of each particle every iterations
-        bh_strategy             : str
-            out of bound position strategy for pyswarms optimizer [2]:
-                    "nearest"               : Round the value to the nearest bound (default)
-                    "periodic"              : set to the modulus of the value between the two bounds
-                    "random"                : set to a random value
-                    "shrink"                : reduce the velocity to finish land on the bound
-                    "reflective"            : mirror the position form inside to ouside the bounds
-                    "intermediate"          : set to intermediate value between previous pos and bound
-        oh_strategy             : dict (like {"w":str, "c1":str, "c2":str})
-            Dynamic options strategy for pyswarms optimizer [3], if None static options,
-            by default None:
-                    "exp_decay"             : Decreases the parameter exponentially between limits
-                    "lin_variation"         : Decreases/increases the parameter linearly between limits
-                    "nonlin_mod"            : Decreases/increases the parameter between limits
-                                            according to a nonlinear modulation index
-                    "rand"                  : takes a uniform random value between limits
-        ftol                    : float
-            relative error in objective_func(best_pos) acceptable for convergence, if None -np.inf
-            default None
-        ftol                    : int
-            number of iterations over which the relative error in objective_func(best_pos) is
-            acceptable for convergence, by default 1
-        save_results            : bool
-            save or not the output in a .json file, by default False
-        saving_file             : str
-            name of the file on wich the output should be saved, by default "pso_results.json"
-
-        Returns
-        -------
-        results     : optim_results
-            contains all the parameters and outputs of the PSO
-
-        Note
-        ----
-        links to pyswarms doc:
-        [1] https://pyswarms.readthedocs.io/en/latest/index.html
-        [2] https://pyswarms.readthedocs.io/en/latest/api/pyswarms.handlers.html
-        """
         super().__init__("PSO")
         self.swarm_optimizer = True
         self.n_particles = n_particles
         self.dimensions = dimensions
         self.options = options
         self.maxiter = maxiter
         self.n_processes = n_processes
@@ -318,25 +417,30 @@
             )
             if answer == "Y":
                 self.n_processes = None
             else:
                 print("Terminated")
                 return False
 
-    def minimize(self, f_swarm, **kwargs):
+    def minimize(self, f_swarm:callable, **kwargs)-> optim_results:
         """
         Perform a Particle swarm optimization
 
         Parameters
         ----------
-        cost_function_swarm     : func
+        f_swarm     : callable
             function taking in parameter a swarm (dim-dimensions array) and returning the cost for each
             particle (1-dimensionnal array)
         kwargs                  : dict
-            containing parameters to change to class (PSO_optimizer.__init__)
+            containing parameters to change in the class (:class:``PSO_optimizer``)
+
+        Returns
+        -------
+        optim_results
+            results of the optimization
         """
         self.__mproc_handling()
         results = super().minimize(f_swarm, **kwargs)
 
         verbose = parameters.get_nrv_verbosity() > 2
         # initial position
         if not np.iterable(self.init_pos):
@@ -434,16 +538,15 @@
                 with open(self.saving_file, "w") as outfile:
                     json.dump(results, outfile)
         except KeyboardInterrupt:
             results["status"] = "Interrupted"
             if self.save_results:
                 with open(self.saving_file, "w") as outfile:
                     json.dump(results, outfile)
-            raise KeyboardInterrupt
-            sys.exit(1)
+            rise_error(KeyboardInterrupt, "Interuption raised during PSO")
         except:
             results["status"] = "Failed"
             results["Error_from_prompt"] = traceback.format_exc()
             print(results["Error_from_prompt"])
             if self.save_results:
                 with open(self.saving_file, "w") as outfile:
                     json.dump(results, outfile)
```

### Comparing `nrv-py-1.0.1/nrv/optim/Problems.py` & `nrv_py-1.1.0/nrv/optim/Problems.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import numpy as np
 import faulthandler
 import traceback
 
 from ..backend.NRV_Class import NRV_class
 from ..backend.MCore import MCH, synchronize_processes
 from ..backend.log_interface import rise_error, pass_debug_info, set_log_level
-from .CostFunctions import CostFunction
+from .optim_utils.optim_results import optim_results
+from .CostFunctions import cost_function
 from .Optimizers import Optimizer
 
 import sys
 
 # enable faulthandler to ease 'segmentation faults' debug
 faulthandler.enable()
 
@@ -48,49 +49,50 @@
 
 class Problem(NRV_class):
     """
     Problem Class
 
     A class to describe problems that should be optimized with the NRV Framework.
     The problem should be described with a simulation and a cost, using the object
-    CostFunction, and various optimization algorithms can be used to find optimal solution.
+    cost_function, and various optimization algorithms can be used to find optimal solution.
 
     This class is abstract and is not supposed to be used directly by the end user. NRV can
     handle two types of problems:
     - problems where a geometric parameter can be optimized: please refer to ...
     - problems where the waveform can be optimized: please refer to ...
     """
 
     def __init__(
         self,
-        cost_function: CostFunction = None,
+        cost_function: cost_function = None,
         optimizer: Optimizer = None,
         save_problem_results=False,
         problem_fname="optim.json",
     ):
         super().__init__()
         self._CostFunction = cost_function
         self._Optimizer = optimizer
         # For cases where optimisation is done on a swarm(groupe) of particle
         self.swarm_optimizer = False
         self._SwarmCostFunction = None
         self.save_problem_results = save_problem_results
         self.problem_fname = problem_fname
 
-    # Handling the CostFunction attribute
+    # Handling the cost_function attribute
     @property
     def costfunction(self):
         """
         Cost function of a Problem,
         the cost function should be a CosFunction object, it should return a scalar.
-        NRV function should be prefered"""
+        NRV function should be prefered
+        """
         return self._CostFunction
 
     @costfunction.setter
-    def costfunction(self, cf: CostFunction):
+    def costfunction(self, cf: cost_function):
         # need to add a verification that the cost function is a scallar and so on
         self._CostFunction = cf
 
     @costfunction.deleter
     def costfunction(self):
         self._CostFunction = None
 
@@ -114,15 +116,35 @@
 
     @optimizer.deleter
     def optmizer(self):
         # self._Optimizer = None
         pass
 
     # Call method is where the magic happens
-    def __call__(self, **kwargs):
+    def __call__(self, **kwargs)->optim_results:
+        """
+        Perform the optimization: minimze the `cost_function` using `optmizer`
+
+        Parameters
+        ----------
+
+        kwargs
+            containing parameters of the optimizer to change
+
+        Returns
+        -------
+        optim_results
+            results of the optimization
+
+
+        Raises
+        ------
+        KeyboardInterrupt
+            _description_
+        """
         if MCH.do_master_only_work():
             try:
                 kwargs = self.__update_saving_parameters(**kwargs)
                 if not self.swarm_optimizer:
                     results = self._Optimizer(self._CostFunction, **kwargs)
                 else:
                     self._SwarmCostFunction = cost_function_swarm_from_particle(
@@ -146,14 +168,18 @@
                 results.save(save=True, fname=self.problem_fname)
             return results
         else:
             return None
 
     # Mcore handling
     def __check_MCore_CostFunction(self):
+        """
+
+        ch
+        """
         return getattr(self._CostFunction, "_MCore_CostFunction", False)
 
     def __wait_for_simulation(self):
         slave_status = {"status": "Wait"}
         try:
             set_log_level("WARNING")
             while slave_status["status"] == "Wait":
@@ -176,11 +202,11 @@
         if "save_problem_results" in kwargs:
             self.save_problem_results = kwargs.pop("save_problem_results")
         if "problem_fname" in kwargs:
             self.problem_fname = kwargs.pop("problem_fname")
         return kwargs
 
     def context_and_cost(self, context_func, cost_func, residual):
-        self.CostFunction = CostFunction(context_func, cost_func, residual)
+        self.cost_function = cost_function(context_func, cost_func, residual)
 
     def autoset_optimizer(self):
         pass
```

### Comparing `nrv-py-1.0.1/nrv/optim/optim_utils/CostEvaluation.py` & `nrv_py-1.1.0/nrv/optim/optim_utils/CostEvaluation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,24 @@
 import numpy as np
 
 from ...fmod.stimulus import stimulus, set_common_time_series
 from ...fmod.extracellular import extracellular_context
 
 from ...backend.NRV_Class import NRV_class, load_any, abstractmethod
 from ...backend.NRV_Simulable import sim_results
-from ...utils.nrv_function import CostEvaluation
+from ...utils.nrv_function import cost_evaluation
 from ...utils.cell.CL_postprocessing import *
 
 
-class raster_count_CE(CostEvaluation):
+class raster_count_CE(cost_evaluation):
+    """
+    Create a callable object which returne the number of spike from the result
+    of a simulation
+    """
     def __init__(self):
-        """
-        Create a callable object which returne the number of spike from the result
-        of a simulation
-
-        Parameters
-        ----------
-        results     : dict
-            output of an axon simulation using Markov model for at least a node
-
-        Returns
-        -------
-        cost        :int
-            number of spike in the v_mem part
-        """
         super().__init__()
 
     def call_method(self, results: sim_results, **kwargs) -> float:
         """
         Returns the spike number from a simulation result
         """
         if "V_mem_raster_position" not in results:
@@ -37,142 +27,162 @@
         M = len(results["x_rec"]) - 1  # pos starts at 0
         i_first_pos = np.where(pos == 0)
         i_last_pos = np.where(pos == M)
         cost = (len(i_first_pos[0]) + len(i_last_pos[0])) / 2
         return cost
 
 
-class charge_quantity_CE(CostEvaluation):
-    def __init__(self, id_elec=None, dt_res=0.0001):
+class recrutement_count_CE(cost_evaluation):
+    r"""
+    Callable object which returns the number of triggered fibre in the results
+
+    Parameters
+    ----------
+    reverse     : bool
+        if True, the final cost is the difference between the number total of fibre and the number of activate fibre
+
+    Note
+    ----
+    if reverse is false:
+
+    .. math::
+
+        cost = N_{recruited}
+
+    else:
+
+    .. math::
+
+        cost = N_{total} - N_{recruited}
+    """
+
+    def __init__(self, reverse=False):
+        super().__init__()
+        self.reverse = reverse
+
+    def count_axon_activation(self, results: sim_results):
+        if "V_mem_raster_position" not in results:
+            rasterize(results, "V_mem")
+        if len(results["V_mem_raster_position"]) == 0:
+            # no spike
+            cpt = 0
+        else:
+            cpt = 1
+        if self.reverse:
+            cpt = int(not cpt)
+        return cpt
+
+    def count_fascicle_activation(self, results: sim_results):
+        cpt = 0
+        for i in range(len(results["axons_diameter"])):
+            if self.reverse:
+                cpt += 1 - results["axon" + str(i)]["spike"]
+            else:
+                cpt += results["axon" + str(i)]["spike"]
+        return cpt
+
+    def call_method(self, results: sim_results, **kwargs) -> float:
         """
-        Create a callable object which return the charge injected
+        Returns the spike number from a simulation result
 
         Parameters
         ----------
+        results     : dict
+            output of an axon simulation using Markov model for at least a node
 
         Returns
         -------
-
+        cost        :int
+            number of spike in the v_mem part
         """
+        cost = 0
+        if "myelinated" in results["result_type"]:
+            cost = self.count_axon_activation(results)
+        elif results["result_type"] == "fascicle":
+            cost = self.count_fascicle_activation(results)
+        else:
+            # nerve simulation
+            for i in results["fascicles_IDs"]:
+                cost += self.count_fascicle_activation(results["fascicle" + str(i)])
+        return cost
+
+
+
+class charge_quantity_CE(cost_evaluation):
+    r"""
+    Create a callable object which return a value proportionnal to the charge quantity injected by stimulus.
+
+    .. math::
+
+        cost = \sum_{e}\sum_{t_k}{i_{e,stim}(t_k)}
+
+    with :math:`t_k` is the discrete time step of the simulation
+    """
+    def __init__(self, id_elec=None, dt_res=0.0001):
         super().__init__()
         self.id_elec = id_elec
         self.dt_res = dt_res
 
     def compute_stimulus_cost(self, stim: stimulus):
         stim_ = stimulus()
         t_min, t_max = stim.t[0], stim.t[-1]
         N_pts = int((t_max - t_min) // self.dt_res)
         stim_.t = np.linspace(t_min, t_max, N_pts)
         set_common_time_series(stim, stim_)
         return abs(stim).integrate()
 
     def call_method(self, results: sim_results, **kwargs) -> float:
-        """ """
         extra_stim = load_any(results["extra_stim"])
         N_elec = len(extra_stim.stimuli)
         cost = 0
         if self.id_elec is None:
             self.id_elec = [k for k in range(N_elec)]
         elif isinstance(self.id_elec, int):
             self.id_elec = [self.id_elec]
         for i in self.id_elec:
             cost += self.compute_stimulus_cost(extra_stim.stimuli[i])
         return cost
 
 
-class stim_energy_CE(CostEvaluation):
-    def __init__(self, id_elec=None, dt_res=0.0001):
-        """
-        Create a callable object which return a value proportionnal to the stimulus energy, assuming Zelec is a constant
+class stim_energy_CE(cost_evaluation):
+    r"""
+    Create a callable object which return a value proportionnal to the stimulus energy, assuming the electrode impedance is a constant.
 
-        Parameters
-        ----------
+    .. math::
 
-        Returns
-        -------
+        cost = \sum_{e}\sum_{t_k}{i_{e,stim}^2(t_k)}
 
-        """
+    with :math:`t_k` is the discrete time step of the simulation
+
+    Parameters
+    ----------
+    id_elec : None | int | list[int]
+        id or list id of the electrode of the to from which the energy should be computed. If None, 
+    dt_res  : float
+        resolotion time step use to compute the cost value
+    """
+    def __init__(self, id_elec:None|int|list[int]=None, dt_res:float=0.0001):
         super().__init__()
         self.id_elec = id_elec
         self.dt_res = dt_res
 
     def compute_stimulus_cost(self, stim: stimulus):
         stim_ = stimulus()
         t_min, t_max = stim.t[0], stim.t[-1]
         N_pts = int((t_max - t_min) // self.dt_res)
         stim_.t = np.linspace(t_min, t_max, N_pts)
         set_common_time_series(stim, stim_)
         stim.s = stim.s * stim.s
         return abs(stim).integrate()
 
     def call_method(self, results: sim_results, **kwargs) -> float:
-        """ """
         extra_stim = load_any(results["extra_stim"])
         N_elec = len(extra_stim.stimuli)
         cost = 0
         if self.id_elec is None:
             self.id_elec = [k for k in range(N_elec)]
         elif isinstance(self.id_elec, int):
             self.id_elec = [self.id_elec]
         for i in self.id_elec:
             cost += self.compute_stimulus_cost(extra_stim.stimuli[i])
         return cost
 
-
-class recrutement_count_CE(CostEvaluation):
-    """
-    Callable object which returns the number of activated fibre in the results
-
-    Parameters
-    ----------
-    results     : dict
-        output of an axon simulation using Markov model for at least a node
-
-    Returns
-    -------
-    cost        :int
-        number of spike in the v_mem part
-    """
-
-    def __init__(self, reverse=False):
-        """
-        Create a callable object which returns the number of activated fibre in the results
-
-        Parameters
-        ----------
-        reverse     : bool
-            output of an axon simulation using Markov model for at least a node
-
-        """
-        super().__init__()
-        self.reverse = reverse
-
-    def count_axon_activation(self, results: sim_results):
-        if len(results["V_mem_raster_position"]) == 0:
-            # no spike
-            return 0
-        else:
-            return 1
-
-    def count_fascicle_activation(self, results: sim_results):
-        cpt = 0
-        for i in range(results["N"]):
-            if self.reverse:
-                cpt += 1 - results["axon" + str(i)]["spike"]
-            else:
-                cpt += results["axon" + str(i)]["spike"]
-        return cpt
-
-    def call_method(self, results: sim_results, **kwargs) -> float:
-        """
-        Returns the spike number from a simulation result
-        """
-        cost = 0
-        if "myelinated" in results["result_type"]:
-            cost = self.count_axon_activation(results)
-        elif results["result_type"] == "fascicle":
-            cost = self.count_fascicle_activation(results)
-        else:
-            # nerve simulation
-            for i in range(len(results["fascicles_IDs"])):
-                cost += self.count_fascicle_activation(results["fascicle" + str(i)])
-        return cost
```

### Comparing `nrv-py-1.0.1/nrv/optim/optim_utils/OptimFunctions.py` & `nrv_py-1.1.0/nrv/optim/optim_utils/OptimFunctions.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,54 @@
 ####################################################################
 ################# generate waveform functions ######################
 ####################################################################
 
 
 ## interpolation
 def interpolate(
-    y,
-    x=[],
+    y:np.ndarray,
+    x:np.ndarray=[],
     scale=4,
     intertype="Spline",
     bounds=(0, 0),
     save=False,
     filename="interpolate.dat",
     save_scale=False,
     kwargs_interp={},
 ):
+    """
+    :meta private:
+
+    Parameters
+    ----------
+    y : np.ndarray
+        _description_
+    x : np.ndarray, optional
+        _description_, by default []
+    scale : int, optional
+        _description_, by default 4
+    intertype : str, optional
+        _description_, by default "Spline"
+    bounds : tuple, optional
+        _description_, by default (0, 0)
+    save : bool, optional
+        _description_, by default False
+    filename : str, optional
+        _description_, by default "interpolate.dat"
+    save_scale : bool, optional
+        _description_, by default False
+    kwargs_interp : dict, optional
+        _description_, by default {}
+
+    Returns
+    -------
+    _type_
+        _description_
+    """
+
     y_scale = []
 
     if len(x) == 0:
         x = [i + 1 for i in range(len(y))]
 
     if type(scale) == float or type(scale) == int:
         x_scale = np.linspace(x[0], x[-1], int(scale))
@@ -61,40 +91,40 @@
             file.write(y_str[1:-2])
             file.close()
         np.set_printoptions(threshold=10)
     return y_scale
 
 
 def interpolate_amp(
-    position,
-    t_sim=100,
-    t_end=None,
-    dt=0.005,
-    intertype="Spline",
-    bounds=(0, 0),
-    save=False,
-    filename="interpolate_part.dat",
-    save_scale=False,
-):
+    position:np.ndarray,
+    t_sim:float=100,
+    t_end:float=None,
+    dt:float=0.005,
+    intertype:str="Spline",
+    bounds:tuple[float]=(0, 0),
+    save:bool=False,
+    filename:str="interpolate_part.dat",
+    save_scale:bool=False,
+)->np.ndarray:
     """
-    genarte a waveform from a particle position using interpolate where the position
-    values are the output waveform amplitudes at regular times
+    genarte a waveform from a particle position using interpolate where the position values are the output waveform amplitudes at constant sample rate
 
     Parameters
     ----------
     position    : array
         particle position in n dimension output waveform amplitudes at regular times
     t_sim       : float
         simulation time (ms), by default 100
     dt       	: float
         time step of the simulation (ms), by default 0.005
     intertype   : str
         type of interpolation perform, by default 'Spline'
         type possibly:
-                'Spline'                : Cubic spline interpolation
+            
+            - 'Spline'                : Cubic spline interpolation
     bounds      : tupple
         limit range of the interpolation, if both equal no limit,by default (0,0)
     save        : bool
         save or not the output in a .dat file, by default False
     filename    : str
         name of the file on wich the output should be saved, by default 'interpolate_part.dat'
 
@@ -128,57 +158,78 @@
         waveform = waveform[: int(t_sim / dt) + 1]
 
     return waveform
 
 
 def interpolate_Npts(
     position,
-    t_sim=100,
-    dt=0.005,
-    amp_start=0,
-    amp_stop=1,
-    intertype="Spline",
-    bounds=(0, 0),
-    fixed_order=False,
-    t_end=None,
-    t_shift=None,
-    save=False,
-    fname="interpolate_2pts.dat",
-    plot=False,
-    save_scale=False,
-    generatefigure=True,
-    strict_bounds=True,
-    kwargs_interp={},
+    t_sim:float=100,
+    dt:float=0.005,
+    amp_start:float=0,
+    amp_stop:float=1,
+    intertype:str="Spline",
+    bounds:tuple[float]=(0, 0),
+    fixed_order:bool=False,
+    t_end:float=None,
+    t_shift:float=None,
+    save:bool=False,
+    fname:str="interpolate_2pts.dat",
+    plot:bool=False,
+    save_scale:bool=False,
+    generatefigure:bool=True,
+    strict_bounds:bool=True,
+    kwargs_interp:dict={},
     **kwargs
 ):
-    """
+    r"""
     genarte a waveform from a particle position using interpolate where the position
-    values are the coordonnate of two points which should be reached by the output waveform
+    values are the coordonnate of N points which should be reached by the output waveform
+
+    Note
+    ----
+    If :math:`I_{i}` and :math:`t_{i}` are the time and amplitude of the :math:`ith` point the position vector :math:`\mathcal{X}` should be:
+
+    .. math::
+
+        \mathcal{X} = \begin{pmatrix} I_{1} & t_{1} & I_{2} & t_{2} & ... & I_{N} & t_{N}   \end{pmatrix}
 
     Parameters
     ----------
-    position    : array
-        particle position in 4 dimensions where the first two are the coordonate of the first point
-        the last two are the coordonate of the second, syntax: X = (time, amplitude)
+    position    : np.ndarray
+        particle position in 2N dimensions with the coordonnate of the N points to interpolate.
     t_sim       : float
         simulation time (ms), by default 100
     dt          : float
         time step of the simulation (ms), by default 0.005
+    amp_start   : float
+        amplitude at the beginning of the interpolation
+    amp_stop    : float
+        amplitude at the end of the interpolation
     intertype   : str
         type of interpolation perform, by default 'Spline'
         type possibly:
-                'Spline'                : Cubic spline interpolation
+
+            - 'Spline'                : Cubic spline interpolation
+            - 'linear'
     bounds      : tupple
         limit range of the interpolation, if both equal no limit, by default (0,0)
+    fixed_order         :bool
+        fix the order of the points to interpolate
+    t_end           :float
+        optionnal, if not None, time of the stimulation at which the interpollation should reach amp_stop
+    t_shift         :float
+        optionnal, if not None, interpolation will be shifted of this time
     save        : bool
         save or not the output in a .dat file, by default False
-    filename    : str
+    fname    : str
         name of the file on wich the output should be saved, by default 'interpolate_2pts.dat'
     strict_bounds    :bool
         if True values out of bound will be set to closer bound
+    kwargs_interp   : dict
+        kwargs to add to the interpollation 
 
     Returns
     -------
     waveform     : np.ndarray
         waveform generated from position
     """
 
@@ -259,16 +310,16 @@
 ####################################################################
 ########################### savers #################################
 ####################################################################
 
 
 def cost_position_saver(data, file_name="document.csv"):
     """
-    Simple saver which can be used in a CostFunction to save the cost
-    and position in a .csv file (see .Optim.CostFunction)
+    Simple saver which can be used in a cost_function to save the cost
+    and position in a .csv file (see .Optim.cost_function)
 
     Parameters
     ----------
     data        : dict
         dict containing the keys 'cost' and 'position'
     file_name:
         name of the saving file.
```

### Comparing `nrv-py-1.0.1/nrv/optim/optim_utils/optim_results.py` & `nrv_py-1.1.0/nrv/optim/optim_utils/optim_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import matplotlib.pyplot as plt
 from matplotlib.animation import FuncAnimation, PillowWriter, FFMpegWriter
 from .OptimFunctions import interpolate_Npts
+from ..CostFunctions import cost_function
 import numpy as np
 
 from ...backend.NRV_Results import NRV_results
 from ...backend.log_interface import pass_info, rise_warning
 
 
 class optim_results(NRV_results):
@@ -89,21 +90,22 @@
                         print("it=", j)
                     return i
 
         if verbose:
             pass_info("not found with decimals =", decimals)
         return self.findbestpart(decimals - 1, verbose=verbose, lim_it=lim_it)
 
+    def compute_best_pos(self, cost_function:cost_function, **kwrgs):
+        return cost_function.get_sim_results(self.x)
+
     ############################
     ##    plotting methods    ##
     ############################
     def plot_cost_history(
-        self, nitstop=-1, generatefigure=True, xlog=False, ylog=False, **fig_kwgs
+        self, ax:plt.axes, nitstop:int=-1, xlog:bool=False, ylog:bool=False,**ax_kwargs
     ):
         cost = self["cost_history"]
-        if generatefigure:
-            plt.figure()
-        plt.plot(cost[0:nitstop], **fig_kwgs)
+        ax.plot(cost[0:nitstop], **ax_kwargs)
         if xlog:
-            plt.xscale("log")
+            ax.set_xscale("log")
         if ylog:
-            plt.yscale("log")
+            ax.set_yscale("log")
```

### Comparing `nrv-py-1.0.1/nrv/utils/cell/CL_postprocessing.py` & `nrv_py-1.1.0/nrv/utils/cell/CL_postprocessing.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,72 +6,25 @@
 
 import numpy as np
 from numba import jit
 from scipy import signal
 
 from ...backend.file_handler import is_iterable, json_dump, json_load
 from ...backend.log_interface import pass_info, rise_warning, rise_error
-from ..units import *
+from ...backend.NRV_Class import load_any
+from ..units import MHz
+from ..misc import distance_point2line
 from ...nmod.unmyelinated import unmyelinated
 from ...nmod.myelinated import myelinated
-from ...backend.NRV_Class import load_any
+
 
 # enable faulthandler to ease 'segmentation faults' debug
 faulthandler.enable()
 
 
-#############################
-## miscellaneous functions ##
-#############################
-def distance_point2point(x_1, y_1, x_2=0, y_2=0):
-    """
-    Computes the distance between a point (x_p,y_p) and a line defined as y=a*x+b
-
-    Parameters
-    ----------
-    x_1 : float
-        first point x coordinate,
-    y_1 : float
-        firstpoint y coordinate,
-    x_2 : float
-        second point x coordinate, by default 0
-    y_2 : float
-        second point y coordinate, , by default 0
-
-    Returns
-    --------
-    d : float
-        distance between the point and the orthogonal projection of (x_p,y_p) on it
-    """
-    d = ((x_1 - x_2) ** 2 + (y_1 - y_2) ** 2) ** 0.5
-    return d
-
-
-def distance_point2line(x_p, y_p, a, b):
-    """
-    Computes the distance between a point (x_p,y_p) and a line defined as y=a*x+b
-
-    Parameters
-    ----------
-    x_p : float
-        point x coordinate,
-    y_p : float
-        point y coordinate,
-    a   : float
-        line direction coeefficient
-    b   : float
-        line y for x = 0
-
-    Returns
-    --------
-    d : float
-        distance between the point and the orthogonal projection of (x_p,y_p) on it
-    """
-    d = np.abs(a * x_p - y_p + b) / (np.sqrt(a**2 + 1))
-    return d
 
 
 #####################################
 ## SAVE AND LOAD RESULTS FUNCTIONS ##
 #####################################
 
 
@@ -1054,15 +1007,15 @@
 
     Parameters:
     -----------
     ax      : matplotlib axis object
         axes of the figure to work on
     values  : list, array, numpy array
     """
-    states = ["$I_1$", "$I_2$", "$C_1$", "$C_2$", "$O_1$", "$O_2$"]
+    states = [r"$I_1$", r"$I_2$", r"$C_1$", r"$C_2$", r"$O_1$", r"$O_2$"]
 
     X = [-1, -3, 0, 1, 0, 3]
     Y = [0, 0, 1, 0, -1, 0]
     c = ["r", "r", "b", "b", "g", "g"]
 
     ax.set_xlim(-3.4, 3.4)
     ax.set_ylim(-1.5, 1.5)
```

### Comparing `nrv-py-1.0.1/nrv/utils/cell/CL_simulations.py` & `nrv_py-1.1.0/nrv/utils/cell/CL_simulations.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ...fmod.extracellular import *
 from ...fmod.materials import *
 from ...fmod.stimulus import *
 from ...nmod.axons import *
 from ...nmod.myelinated import *
 from ...nmod.unmyelinated import *
 from ..saving_handler import *
-from .CL_discretization import *
 from .CL_postprocessing import *
 
 unmyelinated_models = [
     "HH",
     "Rattay_Aberham",
     "Sundt",
     "Tigerholm",
@@ -31,14 +30,15 @@
     diameter,
     L,
     dist_elec,
     cath_time=100e-3,
     model="MRG",
     amp_max=2000,
     amp_tol=1,
+    dt = 0.005,
     verbose=True,
     **kwargs,
 ):
     """
     Find the firing threshold with point source approximation using binary search.
 
     Parameters
@@ -53,14 +53,16 @@
             cathodic pulse width in ms
     model           : str
             Axon model
     amp_max         : float
             Maximum tested blocking amplitude for the binary search in uA
     amp_tol         : float
             Threshold tolerance in % for the binary search
+    dt              : float
+        Set the dt to a specific value in ms
     verbose         : bool
             set the verbosity of the search
     **kwargs:
             See below
 
     Keyword Arguments:
             material       :   str
@@ -86,18 +88,14 @@
                     Specify the cathodic/anodic ratio
             dt              : float
                     Set the dt to a specific value in ms
             cath_an_ratio          : float
                     Set the tolorance for dt in %
             nseg            : int
                     Set the number of segment for the axon
-            nseg_tol        : float
-                    Set the nseg tolerance in %
-            dt_tol        : float
-                    Set the dt tolerance in %
             amp_tol_abs     : float
                     Set the absolute tolerance for the binary search in uA.
             node_shift      : float between -1 and 1
                     Align electrode with Node of Ranvier. When Shift = 0, Electrode is aligned with node
             n_nodes         : integer
                     Specify the number of Node of Ranvier for myelinated models. Overwrite L when specified.
 
@@ -146,39 +144,24 @@
         amp_min = 0
 
     if "f_dlambda" in kwargs:
         f_dlambda = kwargs.get("f_dlambda")
     else:
         f_dlambda = 0
 
-    if "dt" in kwargs:
-        dt = kwargs.get("dt")
-    else:
-        dt = 0
-
-    if "dt_tol" in kwargs:
-        dt_tol = kwargs.get("dt_tol")
-    else:
-        dt_tol = amp_tol
-
     if "nseg" in kwargs:
         nseg = kwargs.get("nseg")
     else:
         nseg = 0
 
     if "Nseg_per_sec" in kwargs:
         Nseg_per_sec = kwargs.get("Nseg_per_sec")
     else:
         Nseg_per_sec = 0
 
-    if "nseg_tol" in kwargs:
-        nseg_tol = kwargs.get("nseg_tol")
-    else:
-        nseg_tol = amp_tol
-
     if "amp_tol_abs" in kwargs:
         amp_tol_abs = kwargs.get("amp_tol_abs")
     else:
         amp_tol_abs = 0
 
     if "node_shift" in kwargs:
         node_shift = kwargs.get("node_shift")
@@ -193,37 +176,14 @@
     amplitude_max_th = amp_max
     amplitude_min_th = amp_min
     amplitude_tol = amp_tol
     # axon
     y = 0
     z = 0
 
-    if dt == 0:
-        if cath_an_ratio > 0 and cath_an_ratio < 1:
-            dt = Get_dt(
-                dt_tol,
-                model,
-                simulation_category="Spike_threshold",
-                stim_pw=cath_time / cath_an_ratio,
-            )
-        else:
-            dt = Get_dt(
-                dt_tol, model, simulation_category="Spike_threshold", stim_pw=cath_time
-            )
-
-    if (nseg == 0) and (f_dlambda == 0) and (Nseg_per_sec == 0):
-        if model in unmyelinated_models:
-            Nseg_per_sec = Get_nseg(
-                nseg_tol, model, simulation_category="Spike_threshold", d=diameter, L=L
-            )
-        else:
-            Nseg_per_sec = Get_nseg(
-                nseg_tol, model, simulation_category="Spike_threshold"
-            )
-
     # extra cellular
     extra_material = load_material(material)
     # Dichotomy initialization
     previous_amp = amp_min
     delta_amp = np.abs(amp_max - amp_min)
     current_amp = amp_max
     Niter = 1
@@ -385,42 +345,45 @@
             Threshold tolerance in % for the binary search
     verbose         : bool
             set the verbosity of the search
     **kwargs:
             See below
 
     Keyword Arguments:
-            amp_min        : float
-                    minimum amplitude for the binary search
-            t_sim          : float
-                    Duration of the simulation in ms
-            amp_tol_abs    : float
-                    Specify an absolute amplitude tolerance for the binary search
-                    in uA
-            dt             : float
-                    Set the dt to a specific value in ms
-            anod_first  : bool
-                    Set the anodic phase before the cathodic phase
-            t_inter : float
-                    Specify the interphase delay in ms
-            cath_an_ratio: float
-                    Specify the cathodic/anodic ratio
-            cath_an_ratio          : float
-                    Set the tolorance for dt in %
-            amp_tol_abs     : float
-                    Set the absolute tolerance for the binary search in uA.
-            dt_tol        : float
-                    Set the dt tolerance in %
+    elec_id        : int
+            elec_id where to change stimulus
+    amp_min        : float
+            minimum amplitude for the binary search
+    t_sim          : float
+            Duration of the simulation in ms
+    amp_tol_abs    : float
+            Specify an absolute amplitude tolerance for the binary search
+            in uA
+    anod_first  : bool
+            Set the anodic phase before the cathodic phase
+    t_inter : float
+            Specify the interphase delay in ms
+    cath_an_ratio: float
+            Specify the cathodic/anodic ratio
+    cath_an_ratio          : float
+            Set the tolorance for dt in %
+    amp_tol_abs     : float
+            Set the absolute tolerance for the binary search in uA.
 
     Returns
     -------
     threshold       : float
             estimated firing threshold in uA
     """
 
+    if "elec_id" in kwargs:
+        elec_id = kwargs.get("elec_id")
+    else:
+        elec_id = 0
+
     if "t_sim" in kwargs:
         t_sim = kwargs.get("t_sim")
     else:
         t_sim = 10
 
     if "anod_first" in kwargs:
         anod_first = kwargs.get("anod_first")
@@ -443,40 +406,14 @@
         amp_min = 0
 
     if "amp_tol_abs" in kwargs:
         amp_tol_abs = kwargs.get("amp_tol_abs")
     else:
         amp_tol_abs = 0
 
-    if "dt" in kwargs:
-        dt = kwargs.get("dt")
-    else:
-        dt = 0
-
-    if "dt_tol" in kwargs:
-        dt_tol = kwargs.get("dt_tol")
-    else:
-        dt_tol = amp_tol
-
-    if dt == 0:
-        if cath_an_ratio > 0 and cath_an_ratio < 1:
-            dt = Get_dt(
-                dt_tol,
-                axon.model,
-                simulation_category="Spike_threshold",
-                stim_pw=cath_time / cath_an_ratio,
-            )
-        else:
-            dt = Get_dt(
-                dt_tol,
-                axon.model,
-                simulation_category="Spike_threshold",
-                stim_pw=cath_time,
-            )
-
     amplitude_max_th = amp_max
     amplitude_min_th = amp_min
     amplitude_tol = amp_tol
 
     # Dichotomy initialization
     previous_amp = amp_min
     delta_amp = np.abs(amp_max - amp_min)
@@ -508,16 +445,15 @@
             )
         else:
             stim_1.biphasic_pulse(
                 start, I_cathod, cath_time, 0, 0, anod_first=anod_first
             )
         # axon_load = load_any_axon(axon, extracel_context=True)
         # axon_th = copy.deepcopy(axon)
-        axon.dt = dt
-        axon.change_stimulus_from_elecrode(0, stim_1)
+        axon.change_stimulus_from_electrode(elec_id, stim_1)
 
         # simulate axon activity
         results = axon.simulate(t_sim=t_sim, loaded_footprints=True)
         # del (axon)
         if verbose:
             pass_info(
                 "... Iteration simulation performed in "
@@ -994,50 +930,31 @@
     axon, block_freq=10, amp_max=2000, amp_tol=1, dt=0.005, verbose=True, **kwargs
 ):
     """
     Find the blocking threshold with point source approximation using binary search.
 
     Parameters
     ----------
-    diameter        : float
-            axon diameter in um
-    L               : float
-            axon length in um
-    dist_elec       : float
-            y coordinate of the point source electrode in um
+    axon       : axon
+            axon to stimulation
     block_freq      : float
             Blocking frequency in kHz
-    model           : str
-            Axon model
     amp_max         : float
             Maximum tested blocking amplitude for the binary search in uA
     amp_tol         : float
             Threshold tolerance in % for the binary search
-    dt              : float
-            time discretization in ms
-    Nseg_per_sec    : int
-            Number of segment per section (myelinated axons)
-            Number of segment per mm of length (unmyelinated axons)
     verbose         : bool
             set the verbosity of the search
 
     **kwargs:
             See below
 
     Keyword Arguments:
-            material       :   str
-                    material used to compute the extracellular field
-            position_elect : float
-                    x location of the electrode, between 0 and 1
-            z_elect        : float
-                    z coordinate of the electrode
             amp_min        : float
                     minimum amplitude for the binary search
-            f_dlambda      : float
-                    To set the number of segment with the d_dlambda rule (Hz)
             t_sim          : float
                     Duration of the simulation in ms
             amp_tol_abs    : float
                     Specify an absolute amplitude tolerance for the binary search
                     in uA
             t_position     : float
                     Positition on the test electrode.
@@ -1049,35 +966,26 @@
                     duration of the test pulse, in ms
             t_amplitude    : float
                     Amplitude of the test pulse, in nA
             b_start        : float
                     start of the blocking stimulation in ms
             b_duration     : float
                     duration of the blocking stimulation in ms
-            node_shift      : float between -1 and 1
-                    Align electrode with Node of Ranvier. When Shift = 0, Electrode is aligned with node
-            n_nodes         : integer
-                    Specify the number of Node of Ranvier for myelinated models. Overwrite L when specified.
 
     Returns
     -------
     threshold       : float
             estimated threshold in uA
     """
 
     if "amp_min" in kwargs:
         amp_min = kwargs.get("amp_min")
     else:
         amp_min = 0
 
-    if "f_dlambda" in kwargs:
-        f_dlambda = kwargs.get("f_dlambda")
-    else:
-        f_dlambda = 100
-
     if "t_sim" in kwargs:
         t_sim = kwargs.get("t_sim")
     else:
         t_sim = 40
 
     if "amp_tol_abs" in kwargs:
         amp_tol_abs = kwargs.get("amp_tol_abs")
@@ -1098,15 +1006,15 @@
         t_duration = kwargs.get("t_duration")
     else:
         t_duration = 1
 
     if "t_amplitude" in kwargs:
         t_amplitude = kwargs.get("t_amplitude")
     else:
-        t_amplitude = 2
+        t_amplitude = 5
 
     if "b_start" in kwargs:
         b_start = kwargs.get("b_start")
     else:
         b_start = 3
 
     if "b_duration" in kwargs:
@@ -1139,16 +1047,15 @@
         # extra-cellular stimulation
 
         stim_1 = stimulus()
         stim_1.sinus(
             b_start, b_duration, current_amp, block_freq, dt=1 / (block_freq * 20)
         )
 
-        axon.dt = dt
-        axon.change_stimulus_from_elecrode(0, stim_1)
+        axon.change_stimulus_from_electrode(0, stim_1)
 
         # simulate axon activity
         results = axon.simulate(t_sim=t_sim, loaded_footprints=True)
 
         if verbose:
             pass_info(
                 "... Iteration simulation performed in "
```

### Comparing `nrv-py-1.0.1/nrv/utils/fascicle/FL_postprocessing.py` & `nrv_py-1.1.0/nrv/utils/fascicle/FL_postprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     Returns
     -------
     facsicular_state       : dict
     """
 
     fascicular = json_load(dir_path + "00_Fascicle_config.json")
     facsicular_state = {"-1": fascicular}
-    N_ax = fascicular["N"]
+    N_ax = len(fascicular["axons_diameter"])
     for i in range(N_ax):
         file = "sim_axon_"+ str(i) + ".json"
         if "extra_stim" not in facsicular_state["-1"]:
             facsicular_state["-1"]["extra_stim"] = extra_stim_properties(
                 dir_path + file
             )
 
@@ -235,28 +235,25 @@
 #############################
 ## VISUALIZATION FUNCTIONS ##
 #############################
 
 
 def plot_fasc_state(
     facsicular_state,
-    fig,
     axes,
     contour_color="k",
     myel_color="r",
     unmyel_color="b",
     num=False,
 ):
     """
     plot the fascicle in the Y-Z plane (transverse section)
 
     Parameters
     ----------
-    fig     : matplotlib.figure
-        figure to display the fascicle
     axes    : matplotlib.axes
         axes of the figure to display the fascicle
     contour_color   : str
         matplotlib color string applied to the contour. Black by default
     myel_color      : str
         matplotlib color string applied to the myelinated axons. Red by default
     unmyel_color    : str
@@ -288,15 +285,20 @@
                 colors += ["lightgray"]
                 alpha += [0]
         N += 1
 
     alpha = [1 - (i / (1 + max(alpha))) for i in alpha]
 
     ## plot contour
-    axes.plot(fasc["y_vertices"], fasc["z_vertices"], linewidth=2, color=contour_color)
+    axes.add_patch(plt.Circle(
+                (fasc["y_grav_center"], fasc["z_grav_center"]),
+                fasc["D"]/2,
+                color=contour_color,
+                fill=False,
+                linewidth=2,))
     ## plot axons
     circles = []
     for k in range(N):
         if fasc["axons_type"][k] == 1:  # myelinated
             circles.append(
                 plt.Circle(
                     (fasc["axons_y"][k], fasc["axons_z"][k]),
```

### Comparing `nrv-py-1.0.1/nrv/utils/nrv_function.py` & `nrv_py-1.1.0/nrv/utils/nrv_function.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from abc import abstractmethod
 
 import numpy as np
 from scipy.interpolate import CubicHermiteSpline, interp1d
 from scipy.special import erf
 
 from ..backend.file_handler import json_dump, json_load
-from ..backend.log_interface import rise_warning
+from ..backend.log_interface import rise_warning, rise_error
 from ..backend.NRV_Class import NRV_class, is_empty_iterable
 
 #############################
 ## sigma functions classes ##
 #############################
 spy_interp1D_kind = [
     "linear",
@@ -387,20 +387,20 @@
             else:
                 xc = 0
             res += (xi - xc) ** 2
         return res**0.5
 
 
 ###########################################################
-####################  CostEvaluation  #####################
+####################  cost_evaluation  #####################
 ###########################################################
-class CostEvaluation(nrv_function):
+class cost_evaluation(nrv_function):
     def __init__(self):
         super().__init__()
-        self.f_type = "CostEvaluation"
+        self.f_type = "cost_evaluation"
 
     @staticmethod
     def call_method(self, static_sim) -> float:
         return 1
 
     def __call__(self, results, **kwargs) -> float:
         return self.call_method(results)
@@ -451,15 +451,15 @@
 
         Returns
         -------
         output  :  tuple(3)
             (domain, cell_tag, facet_tag)
         """
         super().__init__()
-        self.f_type = "interp"
+        self.f_type = "nrv_interp"
         # General parameters
         self.X_values = X_values
         self.Y_values = Y_values
         self.N_pts = len(Y_values)
         self.interpolator = interpolator
         self.kind = kind
         self.dx = dx
@@ -530,14 +530,122 @@
             if self.kind.lower() == "cardinal" and scale is not None:
                 self.scale = scale
 
             self.interpolator = CubicHermiteSpline(
                 self.X_values, self.Y_values, self.scale * self.dxdy
             )
 
+    # Mathematical operations
+    def __add__(self, b):
+        if isinstance(b, nrv_interp):
+            if np.allclose(b.X_values, self.X_values):
+                Y = b.Y_values + self.Y_values
+                # TO ADD: computation of dxdy when both are set
+            else:
+                rise_error(
+                    "Not implemented: operations of nrv_iterp with different X_scale"
+                )
+        else: 
+            Y = self.Y_values+b
+        return nrv_interp(
+            X_values = self.X_values,
+            Y_values = Y,
+            interpolator = self.interpolator,
+            kind = self.kind,
+            dx = self.dx,
+            dxdy = None,
+            scale = self.scale,
+            columns = self.columns,
+        )
+
+    def __mul__(self, b):
+        if isinstance(b, nrv_interp):
+            if np.allclose(b.X_values, self.X_values):
+                Y =  self.Y_values*b.Y_values
+                # TO ADD: computation of dxdy when both are set
+            else:
+                rise_error(
+                    "Not implemented: operations of nrv_iterp with different X_scale"
+                )
+        else: 
+            Y = self.Y_values*b
+        return nrv_interp(
+            X_values = self.X_values,
+            Y_values = Y,
+            interpolator = self.interpolator,
+            kind = self.kind,
+            dx = self.dx,
+            dxdy = None,
+            scale = self.scale,
+            columns = self.columns,
+        )
+
+    def __truediv__(self, b):
+        if isinstance(b, nrv_interp):
+            if np.allclose(b.X_values, self.X_values):
+                if np.isclose(b.Y_values, 0).any():
+                    rise_error(ZeroDivisionError, "float division by zero in Python")
+                Y = self.Y_values / b.Y_values
+                # TO ADD: computation of dxdy when both are set
+            else:
+                rise_error(
+                    NotImplementedError,
+                    "operations of nrv_iterp with different X_scale",
+                )
+        else:
+            Y = self.Y_values/b
+        return nrv_interp(
+            X_values = self.X_values,
+            Y_values = Y,
+            interpolator = self.interpolator,
+            kind = self.kind,
+            dx = self.dx,
+            dxdy = None,
+            scale = self.scale,
+            columns = self.columns,
+        )
+
+    def __rtruediv__(self, b):
+        if np.isclose(self.Y_values, 0).any():
+            rise_error(ZeroDivisionError, " float division by zero in Python")
+        if isinstance(b, nrv_interp):
+            if np.allclose(b.X_values, self.X_values):
+                Y = b.Y_values/self.Y_values
+                # TO ADD: computation of dxdy when both are set
+            else:
+                rise_error(
+                    NotImplementedError,
+                    "operations of nrv_iterp with different X_scale",
+                )
+        else:
+            Y = b/self.Y_values
+        return nrv_interp(
+            X_values = self.X_values,
+            Y_values = Y,
+            interpolator = self.interpolator,
+            kind = self.kind,
+            dx = self.dx,
+            dxdy = self.dxdy,
+            scale = self.scale,
+            columns = self.columns,
+        )
+
+
+    def __radd__(self, b):
+        return self.__add__(b)
+
+    def __rmul__(self, b):
+        return self.__mul__(b)
+    
+    def __sub__(self, b):
+        return self.__add__(-b)
+    
+    def __rsub__(self, b):
+        return self.__sub__(b)
+
     def __call__(self, X):
         if is_empty_iterable(self.columns):
             return self.interpolator(X)
         try:
             return self.interpolator(X[self.columns])
         except:
             rise_warning(
```

### Comparing `nrv-py-1.0.1/nrv/utils/saving_handler.py` & `nrv_py-1.1.0/nrv/utils/saving_handler.py`

 * *Files identical despite different names*

### Comparing `nrv-py-1.0.1/nrv/utils/units.py` & `nrv_py-1.1.0/nrv/utils/units.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             - mV
             - uV, V
         *   - Time
             - ms
             - us, s, minute, hour, day
         *   - Length
             - um
-            - mm, cm, dm, m
+            - nm, mm, cm, dm, m
         *   - Currents
             - uA
             - nA, mA, A
         *   - Conductance
             - S
             - kS, mS, uS
         *   - Frequency
@@ -69,14 +69,15 @@
 Hz = 1e-3 * kHz
 MHz = 1e3 * kHz
 GHz = 1e6 * kHz
 
 #####################
 ## length prefixes ##
 #####################
+nm = 1e-3 * um
 mm = 1e3 * um
 cm = 1e1 * mm
 dm = 1e1 * cm
 m = 1e1 * dm
 
 ######################
 ## current prefixes ##
@@ -207,15 +208,49 @@
         cp_value = deepcopy(value)
         for i, num in enumerate(value):
             cp_value[i] = to_nrv_unit(num, unit)
         return cp_value
     else:
         return value * unit
 
+def convert(value, unitin, unitout):
+    """
+    Convert a quantity ``value`` from ``unitin`` to ``unitout``.
+
+    Parameters
+    ----------
+    value:      int, float, list or np.ndarray
+        value or values wich should be converted.
+    unit:     int or str
+        unit to which value should be converted, see examples.
+
+    Returns
+    -------
+    int, float, list or np.ndarray
+        rounded value or values, with the same type and shape than ``value``.)
+
+    Example
+    -------
+    Here are two ways of converting 0.2 S/m^{2} into S/cm^{2}:
 
+        >>> import nrv
+        >>> val_S_m = 0.2 # S/m**2
+        >>> nrv.convert(val_S_m, nrv.S/nrv.m**2, nrv.S/nrv.cm**2)
+        2e-05
+        >>> nrv.convert(val_S_m, "S/m**2", "S/cm**2")
+        2e-05
+    """
+    if np.iterable(value) and not isinstance(value, np.ndarray):
+        cp_value = deepcopy(value)
+        for i, num in enumerate(value):
+            cp_value[i] = convert(num, unitin, unitout)
+        return cp_value
+    else:
+        return from_nrv_unit(to_nrv_unit(value, unitin), unitout)
+    
 def sci_round(value, digits=3):
     """
     Rounds one or several values to ``digits`` significant digits.
 
     Parameters
     ----------
     value:      int, float, list or np.ndarray
```

### Comparing `nrv-py-1.0.1/nrv_py.egg-info/PKG-INFO` & `nrv_py-1.1.0/nrv_py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: nrv-py
-Version: 1.0.1
+Version: 1.1.0
 Summary: NeuRon Virtualizer (NRV)
 Home-page: https://github.com/fkolbl/NRV
 Author: Florian Kolbl, Roland Giraud, Louis Regnacq, Thomas Couppey
 Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Natural Language :: English
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: gmsh
 Requires-Dist: mph
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: neuron
 Requires-Dist: matplotlib
 Requires-Dist: numba
 Requires-Dist: ezdxf
 Requires-Dist: icecream
 Requires-Dist: pyswarms
+Requires-Dist: tqdm
 
 [![PyPI version](https://badge.fury.io/py/nrv-py.svg)](https://badge.fury.io/py/nrv-py)
 [![Documentation Status](https://readthedocs.org/projects/nrv/badge/?version=latest)](https://nrv.readthedocs.io/en/latest/?badge=latest)
 [![License: CeCill](https://img.shields.io/badge/Licence-CeCill-blue )](https://github.com/fkolbl/NRV/blob/master/Licence.txt)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10497741.svg)](https://doi.org/10.5281/zenodo.10497741)
 <!---[![DOI](xxxx)](xxx)-->
 <!---[![Build Status](xxxx)](xxx)-->
```

### Comparing `nrv-py-1.0.1/nrv_py.egg-info/SOURCES.txt` & `nrv_py-1.1.0/nrv_py.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,44 @@
 ReadMe.md
 setup.py
 ./nrv/nrv2calm
 ./tests/NRV_test
 nrv/__init__.py
 nrv/nrv2calm
 nrv/_misc/NRV.ini
+nrv/_misc/OTF_PP/ap_detection.py
 nrv/_misc/OTF_PP/default.py
 nrv/_misc/OTF_PP/is_blocked.py
 nrv/_misc/OTF_PP/is_excited.py
 nrv/_misc/OTF_PP/is_onset.py
 nrv/_misc/OTF_PP/raster_plot.py
 nrv/_misc/OTF_PP/rmv_keys.py
+nrv/_misc/OTF_PP/save_gmem.py
 nrv/_misc/OTF_PP/vmem_plot.py
 nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_CUFF.mph
 nrv/_misc/comsol_templates/Nerve_1_Fascicle_1_LIFE.mph
 nrv/_misc/comsol_templates/Nerve_1_Fascicle_2_LIFE.mph
 nrv/_misc/geom/smoothed_edges_white.dxf
 nrv/_misc/geom/smoothed_edges_white.png
 nrv/_misc/log/NRV.log
+nrv/_misc/materials/axoplasmic_mrg.mat
 nrv/_misc/materials/bone.mat
 nrv/_misc/materials/cerebrospinal_fluid.mat
 nrv/_misc/materials/dura.mat
 nrv/_misc/materials/endoneurium_bhadra.mat
+nrv/_misc/materials/endoneurium_horn.mat
 nrv/_misc/materials/endoneurium_ranck.mat
 nrv/_misc/materials/epidural_space.mat
 nrv/_misc/materials/epineurium.mat
+nrv/_misc/materials/epineurium_horn.mat
 nrv/_misc/materials/material_1.mat
 nrv/_misc/materials/material_2.mat
 nrv/_misc/materials/muscle.mat
 nrv/_misc/materials/perineurium.mat
+nrv/_misc/materials/perineurium_horn.mat
 nrv/_misc/materials/platinum.mat
 nrv/_misc/materials/saline.mat
 nrv/_misc/materials/silicone.mat
 nrv/_misc/mods/AXNODE.mod
 nrv/_misc/mods/CaPump.mod
 nrv/_misc/mods/DNav18.mod
 nrv/_misc/mods/KCa.mod
@@ -151,14 +157,15 @@
 nrv/_misc/ppops/Placed_population_of_5000_axons_F.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_A.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_B.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_C.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_D.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_E.ppop
 nrv/_misc/ppops/Placed_population_of_500_axons_F.ppop
+nrv/_misc/stats/Fugleholm.csv
 nrv/_misc/stats/Jacobs_11_A.csv
 nrv/_misc/stats/Jacobs_11_B.csv
 nrv/_misc/stats/Jacobs_11_C.csv
 nrv/_misc/stats/Jacobs_11_D.csv
 nrv/_misc/stats/Jacobs_9_A.csv
 nrv/_misc/stats/Jacobs_9_B.csv
 nrv/_misc/stats/Jacobs_9_C.csv
@@ -174,53 +181,68 @@
 nrv/backend/NRV_Singleton.py
 nrv/backend/__init__.py
 nrv/backend/compileMods.py
 nrv/backend/file_handler.py
 nrv/backend/inouts.py
 nrv/backend/log_interface.py
 nrv/backend/parameters.py
+nrv/backend/wrappers.py
+nrv/eit/Protocol.py
+nrv/eit/eit_forward.py
+nrv/eit/eit_inverse.py
+nrv/eit/eit_utils.py
 nrv/fmod/__init__.py
 nrv/fmod/electrodes.py
 nrv/fmod/extracellular.py
 nrv/fmod/materials.py
 nrv/fmod/recording.py
 nrv/fmod/stimulus.py
 nrv/fmod/FEM/COMSOL_model.py
 nrv/fmod/FEM/FEM.py
+nrv/fmod/FEM/FENICS_lumped_impedance_model.py
 nrv/fmod/FEM/FENICS_model.py
 nrv/fmod/FEM/__init__.py
+nrv/fmod/FEM/fenics_utils/FEMParameters.py
+nrv/fmod/FEM/fenics_utils/FEMResults.py
 nrv/fmod/FEM/fenics_utils/FEMSimulation.py
-nrv/fmod/FEM/fenics_utils/SimParameters.py
-nrv/fmod/FEM/fenics_utils/SimResult.py
 nrv/fmod/FEM/fenics_utils/__init__.py
+nrv/fmod/FEM/fenics_utils/f_materials.py
 nrv/fmod/FEM/fenics_utils/fenics_materials.py
+nrv/fmod/FEM/fenics_utils/layered_materials.py
 nrv/fmod/FEM/mesh_creator/MshCreator.py
 nrv/fmod/FEM/mesh_creator/NRV_Msh.py
 nrv/fmod/FEM/mesh_creator/NerveMshCreator.py
 nrv/fmod/FEM/mesh_creator/__init__.py
 nrv/nmod/__init__.py
+nrv/nmod/axon_pop_generator.py
 nrv/nmod/axons.py
-nrv/nmod/fascicle_generator.py
 nrv/nmod/fascicles.py
 nrv/nmod/myelinated.py
 nrv/nmod/nerve.py
 nrv/nmod/unmyelinated.py
+nrv/nmod/results/__init__.py
+nrv/nmod/results/axons_results.py
+nrv/nmod/results/fascicles_results.py
+nrv/nmod/results/myelinated_results.py
+nrv/nmod/results/nerve_results.py
+nrv/nmod/results/unmyelinated_results.py
 nrv/optim/CostFunctions.py
 nrv/optim/Optimizers.py
 nrv/optim/Problems.py
 nrv/optim/__init__.py
-nrv/optim/optim_utils/ContextModifier.py
+nrv/optim/optim_utils/ContextModifiers.py
 nrv/optim/optim_utils/CostEvaluation.py
 nrv/optim/optim_utils/OptimFunctions.py
+nrv/optim/optim_utils/__init__.py
 nrv/optim/optim_utils/optim_results.py
 nrv/utils/__init__.py
+nrv/utils/misc.py
 nrv/utils/nrv_function.py
 nrv/utils/saving_handler.py
 nrv/utils/units.py
-nrv/utils/cell/CL_discretization.py
 nrv/utils/cell/CL_postprocessing.py
 nrv/utils/cell/CL_simulations.py
 nrv/utils/cell/__init__.py
 nrv/utils/fascicle/FL_postprocessing.py
 nrv/utils/fascicle/__init__.py
 nrv_py.egg-info/PKG-INFO
 nrv_py.egg-info/SOURCES.txt
```

### Comparing `nrv-py-1.0.1/setup.py` & `nrv_py-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,19 +17,17 @@
     "mph",
     "neuron",
     "icecream",
     "numba",
     "mpi4py",
     "scipy",
     "numpy",
-    "ezdxf",
     "dolfinx",
     "petsc4py",
     "ufl",
-    "gmsh",
     "dolfinx.io",
     "petsc4py.PETSc",
     "dolfinx.fem",
     "dolfinx.fem.petsc",
     "dolfinx.io.utils",
     "scipy.interpolate",
     "scipy.special",
@@ -56,15 +54,15 @@
 
 setup(
     # meta infos
     name=PACKAGE_NAME,
     author=AUTHOR_NAME,
     description=DESCRIPTION,
     url=PROJECT_URL,
-    version="1.0.1",
+    version="1.1.0",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # architecture
     packages=[
         "nrv",
         "nrv._misc",
         "nrv._misc.OTF_PP",
@@ -73,19 +71,21 @@
         "nrv._misc.log",
         "nrv._misc.materials",
         "nrv._misc.mods",
         "nrv._misc.pops",
         "nrv._misc.ppops",
         "nrv._misc.stats",
         "nrv.backend",
+        "nrv.eit",
         "nrv.fmod",
         "nrv.fmod.FEM",
         "nrv.fmod.FEM.fenics_utils",
         "nrv.fmod.FEM.mesh_creator",
         "nrv.nmod",
+        "nrv.nmod.results",
         "nrv.optim",
         "nrv.optim.optim_utils",
         "nrv.utils",
         "nrv.utils.cell",
         "nrv.utils.fascicle",
     ],
     
@@ -103,19 +103,17 @@
         "nrv._misc.stats": ["*.csv"],
     },
     include_package_data=True,
     # classifiers
     classifiers=[
         'License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)',
         'Development Status :: 5 - Production/Stable',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX :: Linux',
         'Operating System :: MacOS :: MacOS X',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
@@ -129,11 +127,12 @@
         "scipy",
         "neuron",
         "matplotlib",
         "numba",
         "ezdxf",
         "icecream",
         "pyswarms",
+        "tqdm",
     ],  # external packages as dependencies
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     scripts=['./nrv/nrv2calm',"./tests/NRV_test"]        #script
 )
```

### Comparing `nrv-py-1.0.1/tests/NRV_test` & `nrv_py-1.1.0/tests/NRV_test`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                         old_argt = new_argt
                         new_argt = []
                         for arg in old_argt:
                             new_argt += [arg[:-3]+str(i)+arg[-2:] for i in range(10)]
                         arg_offset *= 10
                 args.TARGET = args.TARGET[:i+offset] + new_argt + args.TARGET[i+offset+1:]
                 offset += arg_offset
-
+        args.TARGET.sort()
         print("TARGETED:", *args.TARGET)
         for argt in args.TARGET:
             target_script_key = f"{int(argt):03}"
             ###################################
             ## clean the test/figures folder ##
             ###################################
             if os.path.exists(unit_test_figures):
```

