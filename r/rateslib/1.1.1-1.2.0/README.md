# Comparing `tmp/rateslib-1.1.1.tar.gz` & `tmp/rateslib-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateslib-1.1.1.tar", last modified: Thu Mar 21 06:28:46 2024, max compression
+gzip compressed data
```

## Comparing `rateslib-1.1.1.tar` & `rateslib-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,333 @@
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.877133 rateslib-1.1.1/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    19126 2022-10-15 05:18:28.000000 rateslib-1.1.1/LICENSE
--rw-r--r--   0 Darbyshire   (501) staff       (20)      675 2024-03-21 06:26:10.000000 rateslib-1.1.1/MANIFEST.in
--rw-r--r--   0 Darbyshire   (501) staff       (20)    25648 2024-03-21 06:28:46.876427 rateslib-1.1.1/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)     2656 2023-10-11 19:26:08.000000 rateslib-1.1.1/README.md
--rw-r--r--   0 Darbyshire   (501) staff       (20)      758 2024-03-21 06:28:08.000000 rateslib-1.1.1/pyproject.toml
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.688894 rateslib-1.1.1/rateslib/
--rw-r--r--   0 Darbyshire   (501) staff       (20)     4373 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    40145 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/_spec_loader.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    38857 2024-03-20 18:27:00.000000 rateslib-1.1.1/rateslib/calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   106209 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/curves.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.706793 rateslib-1.1.1/rateslib/data/
--rw-r--r--   0 Darbyshire   (501) staff       (20)   113962 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/cad_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17413 2023-11-30 06:38:11.000000 rateslib-1.1.1/rateslib/data/chf_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)   113962 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/corra.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17413 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/estr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)       36 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/eur_ibor_12m.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)       36 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/eur_ibor_1m.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)       36 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/eur_ibor_3m.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)       36 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/eur_ibor_6m.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17413 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/eur_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    47818 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/gbp_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    13423 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/nok_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    13423 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/nowa.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8438 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/sek_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    21159 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/sofr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    47818 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/sonia.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8438 2023-11-18 12:54:45.000000 rateslib-1.1.1/rateslib/data/swestr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)    21159 2023-11-24 18:08:11.000000 rateslib-1.1.1/rateslib/data/usd_rfr.csv
--rw-r--r--   0 Darbyshire   (501) staff       (20)     8591 2024-02-04 15:26:34.000000 rateslib-1.1.1/rateslib/default.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.714096 rateslib-1.1.1/rateslib/dual/
--rw-r--r--   0 Darbyshire   (501) staff       (20)      392 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/dual/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    29034 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/dual/dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    67174 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   327827 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    89067 2024-03-20 18:27:00.000000 rateslib-1.1.1/rateslib/legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    92182 2024-03-20 18:27:00.000000 rateslib-1.1.1/rateslib/periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    52186 2023-11-24 18:08:12.000000 rateslib-1.1.1/rateslib/scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    77617 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/solver.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.740599 rateslib-1.1.1/rateslib/splines/
--rw-r--r--   0 Darbyshire   (501) staff       (20)      326 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/splines/__init__.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    17050 2024-03-21 06:13:48.000000 rateslib-1.1.1/rateslib/splines/splines.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.874595 rateslib-1.1.1/rateslib.egg-info/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    25648 2024-03-21 06:28:46.000000 rateslib-1.1.1/rateslib.egg-info/PKG-INFO
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1257 2024-03-21 06:28:46.000000 rateslib-1.1.1/rateslib.egg-info/SOURCES.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        1 2024-03-21 06:28:46.000000 rateslib-1.1.1/rateslib.egg-info/dependency_links.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)      115 2024-03-21 06:28:46.000000 rateslib-1.1.1/rateslib.egg-info/requires.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)        9 2024-03-21 06:28:46.000000 rateslib-1.1.1/rateslib.egg-info/top_level.txt
--rw-r--r--   0 Darbyshire   (501) staff       (20)       38 2024-03-21 06:28:46.877225 rateslib-1.1.1/setup.cfg
--rw-r--r--   0 Darbyshire   (501) staff       (20)      104 2024-03-21 06:18:10.000000 rateslib-1.1.1/setup.py
-drwxr-xr-x   0 Darbyshire   (501) staff       (20)        0 2024-03-21 06:28:46.862085 rateslib-1.1.1/tests/
--rw-r--r--   0 Darbyshire   (501) staff       (20)    12346 2023-11-24 18:08:12.000000 rateslib-1.1.1/tests/test_calendars.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    50304 2024-03-21 06:13:48.000000 rateslib-1.1.1/tests/test_curves.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     1268 2024-03-21 06:13:48.000000 rateslib-1.1.1/tests/test_default.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    24504 2024-03-21 06:13:48.000000 rateslib-1.1.1/tests/test_dual.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    36607 2024-03-21 06:13:48.000000 rateslib-1.1.1/tests/test_fx.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)   107440 2024-03-20 18:27:00.000000 rateslib-1.1.1/tests/test_instruments.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    76039 2024-03-20 18:27:00.000000 rateslib-1.1.1/tests/test_instruments_bonds.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    59196 2024-02-04 15:26:34.000000 rateslib-1.1.1/tests/test_legs.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    67292 2024-03-20 18:27:00.000000 rateslib-1.1.1/tests/test_periods.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    31745 2023-10-11 19:26:08.000000 rateslib-1.1.1/tests/test_scheduling.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)    56581 2024-03-20 18:27:00.000000 rateslib-1.1.1/tests/test_solver.py
--rw-r--r--   0 Darbyshire   (501) staff       (20)     5839 2024-03-21 06:13:48.000000 rateslib-1.1.1/tests/test_splines.py
+-rw-r--r--   0        0        0     1124 1970-01-01 00:00:00.000000 rateslib-1.2.0/Cargo.toml
+-rw-r--r--   0      501       20     8196 2024-05-11 18:05:09.000000 rateslib-1.2.0/.DS_Store
+-rw-r--r--   0      501       20      482 2024-04-27 12:14:32.000000 rateslib-1.2.0/.flake8
+-rw-r--r--   0      501       20      948 2024-04-10 05:36:38.000000 rateslib-1.2.0/.github/workflows/ubuntu-latest.yml
+-rw-r--r--   0      501       20      948 2024-04-10 05:36:38.000000 rateslib-1.2.0/.github/workflows/ubuntu-minimum.yml
+-rw-r--r--   0      501       20      907 2024-04-10 05:36:38.000000 rateslib-1.2.0/.github/workflows/windows-latest.yml
+-rw-r--r--   0      501       20      950 2024-04-10 05:36:38.000000 rateslib-1.2.0/.github/workflows/windows-minimum.yml
+-rw-r--r--   0      501       20     1948 2024-04-10 05:36:38.000000 rateslib-1.2.0/.gitignore
+-rw-r--r--   0      501       20      791 2024-04-10 05:36:38.000000 rateslib-1.2.0/.readthedocs.yaml
+-rw-r--r--   0      501       20    27793 2024-04-11 15:36:35.000000 rateslib-1.2.0/Cargo.lock
+-rw-r--r--   0      501       20    19126 2022-10-15 05:18:28.000000 rateslib-1.2.0/LICENSE
+-rw-r--r--   0      501       20      676 2024-05-27 15:45:33.000000 rateslib-1.2.0/MANIFEST.in
+-rw-r--r--   0      501       20     1727 2024-04-10 05:36:38.000000 rateslib-1.2.0/PACKAGING.md
+-rw-r--r--   0      501       20     2656 2023-10-11 19:26:08.000000 rateslib-1.2.0/README.md
+-rw-r--r--   0      501       20       73 2024-04-10 05:36:38.000000 rateslib-1.2.0/benches/_README.txt
+-rw-r--r--   0      501       20     2785 2024-04-10 05:36:38.000000 rateslib-1.2.0/benches/my_benchmark.rs
+-rw-r--r--   0      501       20     8196 2023-08-08 06:55:14.000000 rateslib-1.2.0/docs/.DS_Store
+-rw-r--r--   0      501       20      656 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/Makefile
+-rw-r--r--   0      501       20       68 2024-05-26 19:35:23.000000 rateslib-1.2.0/docs/gbpusd.csv
+-rw-r--r--   0      501       20      804 2022-08-20 08:43:43.000000 rateslib-1.2.0/docs/make.bat
+-rw-r--r--   0      501       20       52 2024-05-26 19:35:23.000000 rateslib-1.2.0/docs/sek_ibor_3m.csv
+-rw-r--r--   0      501       20     6511 2023-09-23 05:38:42.000000 rateslib-1.2.0/docs/source/__cookbook.rst
+-rw-r--r--   0      501       20    72569 2023-01-16 21:36:39.000000 rateslib-1.2.0/docs/source/_static/1998-ISDA-memo-EMU-and-Market-Conventions-Recent-Developments.pdf
+-rw-r--r--   0      501       20   511773 2022-08-09 19:45:14.000000 rateslib-1.2.0/docs/source/_static/2006_isda_definitions.pdf
+-rw-r--r--   0      501       20   213504 2022-08-09 20:08:14.000000 rateslib-1.2.0/docs/source/_static/30360isda_2006_example.xls
+-rw-r--r--   0      501       20   883374 2023-03-21 16:36:11.000000 rateslib-1.2.0/docs/source/_static/ICMA-Repo-FAQs.pdf
+-rw-r--r--   0      501       20      171 2024-05-27 15:43:56.000000 rateslib-1.2.0/docs/source/_static/badges.json
+-rw-r--r--   0      501       20    50493 2023-08-27 20:52:17.000000 rateslib-1.2.0/docs/source/_static/base_inherit.png
+-rw-r--r--   0      501       20   155704 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/source/_static/bondbasis.png
+-rw-r--r--   0      501       20     1182 2024-05-08 12:50:48.000000 rateslib-1.2.0/docs/source/_static/css/overwrites.css
+-rw-r--r--   0      501       20    16670 2023-09-05 17:31:23.000000 rateslib-1.2.0/docs/source/_static/depchain_1.png
+-rw-r--r--   0      501       20     9215 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/_static/eurex_bond_conversion_factors.csv
+-rw-r--r--   0      501       20    34494 2023-04-23 13:30:08.000000 rateslib-1.2.0/docs/source/_static/favicon.ico
+-rw-r--r--   0      501       20      325 2023-04-23 13:27:19.000000 rateslib-1.2.0/docs/source/_static/favicon.png
+-rw-r--r--   0      501       20    22754 2024-05-08 12:50:48.000000 rateslib-1.2.0/docs/source/_static/fx_eurusd_3m_surf.PNG
+-rw-r--r--   0      501       20    14069 2024-05-08 12:50:48.000000 rateslib-1.2.0/docs/source/_static/fx_eurusd_3w_smile.PNG
+-rw-r--r--   0      501       20   531466 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/_static/fx_opt_bbg_eurusd.png
+-rw-r--r--   0      501       20    61962 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/source/_static/index_sofr.png
+-rw-r--r--   0      501       20   163191 2023-01-24 20:41:07.000000 rateslib-1.2.0/docs/source/_static/isda-compounding-memo.pdf
+-rw-r--r--   0      501       20   332087 2023-01-24 20:46:01.000000 rateslib-1.2.0/docs/source/_static/isda-memo-rfrs-2006.pdf
+-rw-r--r--   0      501       20   112885 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/_static/long_gilt_initial_jun23.pdf
+-rw-r--r--   0      501       20    14181 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/_static/ofcalc6decTbill.pdf
+-rw-r--r--   0      501       20    13336 2023-09-05 17:31:23.000000 rateslib-1.2.0/docs/source/_static/p2l2i.png
+-rw-r--r--   0      501       20    32680 2023-09-18 20:39:32.000000 rateslib-1.2.0/docs/source/_static/rateslib_github_social.png
+-rw-r--r--   0      501       20     1878 2023-09-12 16:19:32.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo2.png
+-rw-r--r--   0      501       20     1818 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo2a.png
+-rw-r--r--   0      501       20     8250 2023-01-17 20:11:30.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo4.gif
+-rw-r--r--   0      501       20     5454 2023-02-19 06:54:45.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo_big.gif
+-rw-r--r--   0      501       20     4115 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo_big2.png
+-rw-r--r--   0      501       20     5792 2023-11-26 16:05:11.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo_corner.png
+-rw-r--r--   0      501       20   187948 2023-09-12 20:04:16.000000 rateslib-1.2.0/docs/source/_static/rateslib_logo_cropped.psd
+-rw-r--r--   0      501       20    58626 2023-09-05 17:31:23.000000 rateslib-1.2.0/docs/source/_static/sofr_swpm_1.PNG
+-rw-r--r--   0      501       20    43233 2023-09-05 17:31:23.000000 rateslib-1.2.0/docs/source/_static/sofr_swpm_2.PNG
+-rw-r--r--   0      501       20    21856 2023-09-05 17:31:23.000000 rateslib-1.2.0/docs/source/_static/sofr_swpm_3.PNG
+-rw-r--r--   0      501       20    38187 2023-01-16 21:36:39.000000 rateslib-1.2.0/docs/source/_static/spline_note_cs_tau.pdf
+-rw-r--r--   0      501       20    29685 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/_static/swestr_turn.png
+-rw-r--r--   0      501       20    32954 2023-04-18 05:25:30.000000 rateslib-1.2.0/docs/source/_static/thumb_coding1.png
+-rw-r--r--   0      501       20   375725 2023-09-09 07:16:43.000000 rateslib-1.2.0/docs/source/_static/thumb_coding_2.png
+-rw-r--r--   0      501       20   204304 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/_static/thumb_coding_3.png
+-rw-r--r--   0      501       20    93489 2023-02-19 15:17:20.000000 rateslib-1.2.0/docs/source/_static/thumb_ptirds3.png
+-rw-r--r--   0      501       20   197394 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/_static/thumb_ptirds4.png
+-rw-r--r--   0      501       20    30894 2023-04-18 05:25:30.000000 rateslib-1.2.0/docs/source/_static/thumb_trading1.png
+-rw-r--r--   0      501       20    23869 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/_static/ukdmoyldconv.pdf
+-rw-r--r--   0      501       20   126749 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/source/_static/us-treasury-cfs.pdf
+-rw-r--r--   0      501       20    16081 2023-09-09 07:16:43.000000 rateslib-1.2.0/docs/source/_static/ust_10y.gif
+-rw-r--r--   0      501       20    34820 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/_static/usz3ctd.png
+-rw-r--r--   0      501       20    40973 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/_static/usz3dlv.png
+-rw-r--r--   0      501       20    72569 2023-01-16 21:36:39.000000 rateslib-1.2.0/docs/source/api/_static/1998-ISDA-memo-EMU-and-Market-Conventions-Recent-Developments.pdf
+-rw-r--r--   0      501       20   511773 2022-08-09 19:45:14.000000 rateslib-1.2.0/docs/source/api/_static/2006_isda_definitions.pdf
+-rw-r--r--   0      501       20   213504 2022-08-09 20:08:14.000000 rateslib-1.2.0/docs/source/api/_static/30360isda_2006_example.xls
+-rw-r--r--   0      501       20     9215 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/api/_static/eurex_bond_conversion_factors.csv
+-rw-r--r--   0      501       20   163191 2023-01-24 20:41:07.000000 rateslib-1.2.0/docs/source/api/_static/isda-compounding-memo.pdf
+-rw-r--r--   0      501       20   332087 2023-01-24 20:46:01.000000 rateslib-1.2.0/docs/source/api/_static/isda-memo-rfrs-2006.pdf
+-rw-r--r--   0      501       20   112885 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/api/_static/long_gilt_initial_jun23.pdf
+-rw-r--r--   0      501       20    14181 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/api/_static/ofcalc6decTbill.pdf
+-rw-r--r--   0      501       20    38187 2023-01-16 21:36:39.000000 rateslib-1.2.0/docs/source/api/_static/spline_note_cs_tau.pdf
+-rw-r--r--   0      501       20    23869 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/api/_static/ukdmoyldconv.pdf
+-rw-r--r--   0      501       20   126749 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/source/api/_static/us-treasury-cfs.pdf
+-rw-r--r--   0      501       20       88 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.calendars.add_tenor.rst
+-rw-r--r--   0      501       20      106 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.calendars.create_calendar.rst
+-rw-r--r--   0      501       20       70 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.calendars.dcf.rst
+-rw-r--r--   0      501       20       97 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.calendars.get_calendar.rst
+-rw-r--r--   0      501       20      996 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.CompositeCurve.rst
+-rw-r--r--   0      501       20      751 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.Curve.rst
+-rw-r--r--   0      501       20      936 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.IndexCurve.rst
+-rw-r--r--   0      501       20      803 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.LineCurve.rst
+-rw-r--r--   0      501       20      981 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.MultiCsaCurve.rst
+-rw-r--r--   0      501       20      816 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.ProxyCurve.rst
+-rw-r--r--   0      501       20       94 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.average_rate.rst
+-rw-r--r--   0      501       20       88 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.index_left.rst
+-rw-r--r--   0      501       20       91 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.curves.interpolate.rst
+-rw-r--r--   0      501       20     2668 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.default.Defaults.rst
+-rw-r--r--   0      501       20       99 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.default.Fixings.rst
+-rw-r--r--   0      501       20      351 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.default.NoInput.rst
+-rw-r--r--   0      501       20     1204 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.Dual.rst
+-rw-r--r--   0      501       20     1504 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.Dual.vars_from.rst
+-rw-r--r--   0      501       20     1558 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.Dual2.rst
+-rw-r--r--   0      501       20     1829 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.Dual2.vars_from.rst
+-rw-r--r--   0      501       20       80 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_exp.rst
+-rw-r--r--   0      501       20      107 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_inv_norm_cdf.rst
+-rw-r--r--   0      501       20       80 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_log.rst
+-rw-r--r--   0      501       20       95 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_norm_cdf.rst
+-rw-r--r--   0      501       20       95 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_norm_pdf.rst
+-rw-r--r--   0      501       20       86 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.dual_solve.rst
+-rw-r--r--   0      501       20       80 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.gradient.rst
+-rw-r--r--   0      501       20       83 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.set_order.rst
+-rw-r--r--   0      501       20      107 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.dual.set_order_convert.rst
+-rw-r--r--   0      501       20      777 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.fx.FXForwards.rst
+-rw-r--r--   0      501       20      709 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.fx.FXRates.rst
+-rw-r--r--   0      501       20       84 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.fx.forward_fx.rst
+-rw-r--r--   0      501       20      454 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.fx_volatility.FXDeltaVolSmile.rst
+-rw-r--r--   0      501       20      368 2024-05-20 17:48:06.000000 rateslib-1.2.0/docs/source/api/rateslib.fx_volatility.FXDeltaVolSurface.rst
+-rw-r--r--   0      501       20     1161 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.BaseDerivative.rst
+-rw-r--r--   0      501       20      917 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.BaseMixin.rst
+-rw-r--r--   0      501       20     1598 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Bill.rst
+-rw-r--r--   0      501       20     1154 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.BondFuture.rst
+-rw-r--r--   0      501       20      600 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.BondMixin.rst
+-rw-r--r--   0      501       20     1033 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FRA.rst
+-rw-r--r--   0      501       20      894 2024-05-20 17:48:06.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXBrokerFly.rst
+-rw-r--r--   0      501       20      701 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXCall.rst
+-rw-r--r--   0      501       20     1153 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXExchange.rst
+-rw-r--r--   0      501       20      723 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXOption.rst
+-rw-r--r--   0      501       20      384 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXOptionStrat.rst
+-rw-r--r--   0      501       20      690 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXPut.rst
+-rw-r--r--   0      501       20      933 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXRiskReversal.rst
+-rw-r--r--   0      501       20      881 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXStraddle.rst
+-rw-r--r--   0      501       20      881 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXStrangle.rst
+-rw-r--r--   0      501       20     1188 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FXSwap.rst
+-rw-r--r--   0      501       20     1667 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FixedRateBond.rst
+-rw-r--r--   0      501       20     1449 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.FloatRateNote.rst
+-rw-r--r--   0      501       20      458 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Fly.rst
+-rw-r--r--   0      501       20     1046 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.IIRS.rst
+-rw-r--r--   0      501       20     1029 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.IRS.rst
+-rw-r--r--   0      501       20     1861 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.IndexFixedRateBond.rst
+-rw-r--r--   0      501       20      466 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Portfolio.rst
+-rw-r--r--   0      501       20     1029 2024-05-06 18:33:40.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.SBS.rst
+-rw-r--r--   0      501       20     1148 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.STIRFuture.rst
+-rw-r--r--   0      501       20      390 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Sensitivities.rst
+-rw-r--r--   0      501       20      485 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Spread.rst
+-rw-r--r--   0      501       20      865 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.Value.rst
+-rw-r--r--   0      501       20      904 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.VolValue.rst
+-rw-r--r--   0      501       20     1084 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.XCS.rst
+-rw-r--r--   0      501       20     1001 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.ZCIS.rst
+-rw-r--r--   0      501       20      985 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.instruments.ZCS.rst
+-rw-r--r--   0      501       20      566 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.BaseLeg.rst
+-rw-r--r--   0      501       20      586 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.BaseLegMtm.rst
+-rw-r--r--   0      501       20      361 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.CustomLeg.rst
+-rw-r--r--   0      501       20      355 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FixedLeg.rst
+-rw-r--r--   0      501       20      278 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FixedLegMixin.rst
+-rw-r--r--   0      501       20      108 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FixedLegMtm.rst
+-rw-r--r--   0      501       20      418 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FloatLeg.rst
+-rw-r--r--   0      501       20      282 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FloatLegMixin.rst
+-rw-r--r--   0      501       20      108 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.FloatLegMtm.rst
+-rw-r--r--   0      501       20      385 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.IndexFixedLeg.rst
+-rw-r--r--   0      501       20      479 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.IndexLegMixin.rst
+-rw-r--r--   0      501       20      592 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.ZeroFixedLeg.rst
+-rw-r--r--   0      501       20      644 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.ZeroFloatLeg.rst
+-rw-r--r--   0      501       20      436 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.legs.ZeroIndexLeg.rst
+-rw-r--r--   0      501       20      517 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.BasePeriod.rst
+-rw-r--r--   0      501       20      558 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.Cashflow.rst
+-rw-r--r--   0      501       20      315 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.FXCallPeriod.rst
+-rw-r--r--   0      501       20      712 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.FXOptionPeriod.rst
+-rw-r--r--   0      501       20      310 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.FXPutPeriod.rst
+-rw-r--r--   0      501       20      534 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.FixedPeriod.rst
+-rw-r--r--   0      501       20      546 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.FloatPeriod.rst
+-rw-r--r--   0      501       20      558 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.IndexCashflow.rst
+-rw-r--r--   0      501       20      579 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.IndexFixedPeriod.rst
+-rw-r--r--   0      501       20      899 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.periods.IndexMixin.rst
+-rw-r--r--   0      501       20      312 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.scheduling.Schedule.rst
+-rw-r--r--   0      501       20      119 2023-03-05 18:52:56.000000 rateslib-1.2.0/docs/source/api/rateslib.scheduling._check_regular_swap.rst
+-rw-r--r--   0      501       20      110 2023-02-17 17:49:54.000000 rateslib-1.2.0/docs/source/api/rateslib.scheduling._infer_stub_date.rst
+-rw-r--r--   0      501       20     2324 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.solver.Gradients.rst
+-rw-r--r--   0      501       20      800 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.solver.Solver.rst
+-rw-r--r--   0      501       20       91 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.solver.newton_1dim.rst
+-rw-r--r--   0      501       20       91 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.solver.newton_ndim.rst
+-rw-r--r--   0      501       20       97 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.solver.quadratic_eqn.rst
+-rw-r--r--   0      501       20      918 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineDual.rst
+-rw-r--r--   0      501       20      921 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineDual2.rst
+-rw-r--r--   0      501       20      692 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.bspldnev.rst
+-rw-r--r--   0      501       20      590 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.bsplev.rst
+-rw-r--r--   0      501       20     1160 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.bsplmatrix.rst
+-rw-r--r--   0      501       20      733 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.csolve.rst
+-rw-r--r--   0      501       20      620 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppdnev.rst
+-rw-r--r--   0      501       20      843 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppdnev_single.rst
+-rw-r--r--   0      501       20      495 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppdnev_single_dual.rst
+-rw-r--r--   0      501       20      499 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppdnev_single_dual2.rst
+-rw-r--r--   0      501       20      926 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppev.rst
+-rw-r--r--   0      501       20      541 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppev_single.rst
+-rw-r--r--   0      501       20      392 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppev_single_dual.rst
+-rw-r--r--   0      501       20      396 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.ppev_single_dual2.rst
+-rw-r--r--   0      501       20     2056 2024-04-20 09:04:46.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.PPSplineF64.rst
+-rw-r--r--   0      501       20     2642 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.bspldnev_single.rst
+-rw-r--r--   0      501       20     1295 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.bsplev_single.rst
+-rw-r--r--   0      501       20       83 2024-05-06 18:33:41.000000 rateslib-1.2.0/docs/source/api/rateslib.splines.evaluate.rst
+-rw-r--r--   0      501       20    16820 2024-05-26 19:40:45.000000 rateslib-1.2.0/docs/source/c_curves.rst
+-rw-r--r--   0      501       20    16656 2024-05-27 15:35:16.000000 rateslib-1.2.0/docs/source/c_fx_smile.rst
+-rw-r--r--   0      501       20    21200 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/c_solver.rst
+-rw-r--r--   0      501       20     2597 2024-05-27 15:48:05.000000 rateslib-1.2.0/docs/source/conf.py
+-rw-r--r--   0      501       20     7521 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/d_legs.rst
+-rw-r--r--   0      501       20     2741 2024-05-25 12:04:18.000000 rateslib-1.2.0/docs/source/d_periods.rst
+-rw-r--r--   0      501       20      795 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/e_combinations.rst
+-rw-r--r--   0      501       20    16476 2024-05-26 19:36:53.000000 rateslib-1.2.0/docs/source/e_fx_volatility.rst
+-rw-r--r--   0      501       20      592 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/e_multicurrency.rst
+-rw-r--r--   0      501       20     2033 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/e_securities.rst
+-rw-r--r--   0      501       20      806 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/e_singlecurrency.rst
+-rw-r--r--   0      501       20     9706 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/f_fxf.rst
+-rw-r--r--   0      501       20     5124 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/f_fxr.rst
+-rw-r--r--   0      501       20      499 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/g_cookbook.rst
+-rw-r--r--   0      501       20     1639 2023-08-13 15:37:01.000000 rateslib-1.2.0/docs/source/g_coverage.rst
+-rw-r--r--   0      501       20     4145 2024-05-06 20:04:42.000000 rateslib-1.2.0/docs/source/g_curves.rst
+-rw-r--r--   0      501       20     2941 2024-05-26 07:42:17.000000 rateslib-1.2.0/docs/source/g_fx.rst
+-rw-r--r--   0      501       20     2160 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/g_instruments.rst
+-rw-r--r--   0      501       20    22031 2023-11-11 12:17:16.000000 rateslib-1.2.0/docs/source/g_mechanisms.rst
+-rw-r--r--   0      501       20      782 2023-04-24 05:10:57.000000 rateslib-1.2.0/docs/source/g_risk.rst
+-rw-r--r--   0      501       20      351 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/g_utilities.rst
+-rw-r--r--   0      501       20     5413 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/i_about.rst
+-rw-r--r--   0      501       20     6833 2024-05-21 15:32:54.000000 rateslib-1.2.0/docs/source/i_api.rst
+-rw-r--r--   0      501       20     7699 2024-05-25 08:50:44.000000 rateslib-1.2.0/docs/source/i_get_started.rst
+-rw-r--r--   0      501       20    11726 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/i_guide.rst
+-rw-r--r--   0      501       20    17869 2024-05-18 11:15:54.000000 rateslib-1.2.0/docs/source/i_licence.rst
+-rw-r--r--   0      501       20    15360 2024-05-27 15:43:56.000000 rateslib-1.2.0/docs/source/i_whatsnew.rst
+-rw-r--r--   0      501       20     7450 2024-05-18 11:15:54.000000 rateslib-1.2.0/docs/source/index.rst
+-rw-r--r--   0      501       20     2217 2024-05-24 16:32:59.000000 rateslib-1.2.0/docs/source/j_delta.rst
+-rw-r--r--   0      501       20     3803 2023-04-24 05:04:24.000000 rateslib-1.2.0/docs/source/j_gamma.rst
+-rw-r--r--   0      501       20     3165 2023-09-09 07:16:43.000000 rateslib-1.2.0/docs/source/u_calendars.rst
+-rw-r--r--   0      501       20     5425 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/u_defaults.rst
+-rw-r--r--   0      501       20     6631 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/u_dual.rst
+-rw-r--r--   0      501       20     4281 2023-09-09 07:16:43.000000 rateslib-1.2.0/docs/source/u_scheduling.rst
+-rw-r--r--   0      501       20    21644 2024-04-27 12:14:32.000000 rateslib-1.2.0/docs/source/u_splines.rst
+-rw-r--r--   0      501       20     4857 2024-02-04 15:26:34.000000 rateslib-1.2.0/docs/source/z_bondbasis.rst
+-rw-r--r--   0      501       20    16237 2024-04-10 05:36:38.000000 rateslib-1.2.0/docs/source/z_bondctd.rst
+-rw-r--r--   0      501       20     8413 2023-11-11 12:17:16.000000 rateslib-1.2.0/docs/source/z_convexityrisk.rst
+-rw-r--r--   0      501       20     5408 2023-09-09 07:16:43.000000 rateslib-1.2.0/docs/source/z_dependencychain.rst
+-rw-r--r--   0      501       20     5007 2024-05-21 15:32:54.000000 rateslib-1.2.0/docs/source/z_fixings.rst
+-rw-r--r--   0      501       20    10238 2023-11-24 18:08:11.000000 rateslib-1.2.0/docs/source/z_quantlib.rst
+-rw-r--r--   0      501       20     3491 2023-11-11 12:17:16.000000 rateslib-1.2.0/docs/source/z_stubs.rst
+-rw-r--r--   0      501       20     3360 2023-10-11 19:26:08.000000 rateslib-1.2.0/docs/source/z_swpm.rst
+-rw-r--r--   0      501       20     8258 2024-05-06 16:08:22.000000 rateslib-1.2.0/docs/source/z_turns.rst
+-rw-r--r--   0      501       20   980274 2023-07-22 12:01:54.000000 rateslib-1.2.0/notebooks/100swaps.csv
+-rw-r--r--   0      501       20    47588 2023-04-27 19:01:32.000000 rateslib-1.2.0/notebooks/Ch12-AdvancedCurve.ipynb
+-rw-r--r--   0      501       20    32150 2023-08-12 15:26:52.000000 rateslib-1.2.0/notebooks/MultiCSA.ipynb
+-rw-r--r--   0      501       20    11361 2024-03-09 11:19:46.000000 rateslib-1.2.0/notebooks/PerformanceCSV.ipynb
+-rw-r--r--   0      501       20   109981 2023-08-12 15:26:52.000000 rateslib-1.2.0/notebooks/Untitled.ipynb
+-rw-r--r--   0      501       20    83864 2024-05-26 14:36:47.000000 rateslib-1.2.0/notebooks/Untitled1.ipynb
+-rw-r--r--   0      501       20    27186 2023-08-16 19:01:54.000000 rateslib-1.2.0/notebooks/coding/BloombergReplicate.ipynb
+-rw-r--r--   0      501       20    67961 2023-07-08 19:36:50.000000 rateslib-1.2.0/notebooks/coding/Untitled.ipynb
+-rw-r--r--   0      501       20    16106 2023-08-13 15:37:01.000000 rateslib-1.2.0/notebooks/coding/ch5_fx.ipynb
+-rw-r--r--   0      501       20    15613 2023-07-05 20:12:32.000000 rateslib-1.2.0/notebooks/coding/cookbook.ipynb
+-rw-r--r--   0      501       20    10553 2023-08-13 15:37:01.000000 rateslib-1.2.0/notebooks/coding/curves.ipynb
+-rw-r--r--   0      501       20    10861 2023-08-13 15:37:01.000000 rateslib-1.2.0/notebooks/coding/scheduling.ipynb
+-rw-r--r--   0      501       20      145 2024-03-04 20:23:00.000000 rateslib-1.2.0/notebooks/context.py
+-rw-r--r--   0      501       20     4969 2024-05-21 18:13:33.000000 rateslib-1.2.0/rateslib/__init__.py
+-rw-r--r--   0      501       20    40115 2024-05-27 15:50:39.000000 rateslib-1.2.0/rateslib/_spec_loader.py
+-rw-r--r--   0      501       20    39561 2024-05-02 16:56:29.000000 rateslib-1.2.0/rateslib/calendars.py
+-rw-r--r--   0      501       20   108892 2024-05-21 18:13:33.000000 rateslib-1.2.0/rateslib/curves.py
+-rw-r--r--   0      501       20     6148 2023-11-18 11:00:09.000000 rateslib-1.2.0/rateslib/data/.DS_Store
+-rw-r--r--   0      501       20     9027 2024-03-08 18:48:06.000000 rateslib-1.2.0/rateslib/data/__instrument_spec.csv
+-rw-r--r--   0      501       20   113962 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/cad_rfr.csv
+-rw-r--r--   0      501       20    17413 2023-11-30 06:38:11.000000 rateslib-1.2.0/rateslib/data/chf_rfr.csv
+-rw-r--r--   0      501       20   113962 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/corra.csv
+-rw-r--r--   0      501       20    17413 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/estr.csv
+-rw-r--r--   0      501       20       36 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/eur_ibor_12m.csv
+-rw-r--r--   0      501       20       36 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/eur_ibor_1m.csv
+-rw-r--r--   0      501       20       36 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/eur_ibor_3m.csv
+-rw-r--r--   0      501       20       36 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/eur_ibor_6m.csv
+-rw-r--r--   0      501       20    17413 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/eur_rfr.csv
+-rw-r--r--   0      501       20    47818 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/gbp_rfr.csv
+-rw-r--r--   0      501       20    13423 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/nok_rfr.csv
+-rw-r--r--   0      501       20    13423 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/nowa.csv
+-rw-r--r--   0      501       20    17413 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/saron.csv
+-rw-r--r--   0      501       20     8438 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/sek_rfr.csv
+-rw-r--r--   0      501       20    21159 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/sofr.csv
+-rw-r--r--   0      501       20    47818 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/sonia.csv
+-rw-r--r--   0      501       20     8438 2023-11-18 12:54:45.000000 rateslib-1.2.0/rateslib/data/swestr.csv
+-rw-r--r--   0      501       20    21159 2023-11-24 18:08:11.000000 rateslib-1.2.0/rateslib/data/usd_rfr.csv
+-rw-r--r--   0      501       20     8888 2024-05-20 16:00:35.000000 rateslib-1.2.0/rateslib/default.py
+-rw-r--r--   0      501       20     7593 2024-04-29 16:04:56.000000 rateslib-1.2.0/rateslib/dual/__init__.py
+-rw-r--r--   0      501       20    26805 2024-04-27 12:14:32.000000 rateslib-1.2.0/rateslib/dual/dual.py
+-rw-r--r--   0      501       20      297 2024-04-10 05:36:39.000000 rateslib-1.2.0/rateslib/dual/dualrs.py
+-rw-r--r--   0      501       20    67204 2024-04-10 05:36:39.000000 rateslib-1.2.0/rateslib/fx.py
+-rw-r--r--   0      501       20    48215 2024-05-27 15:35:16.000000 rateslib-1.2.0/rateslib/fx_volatility.py
+-rw-r--r--   0      501       20   387947 2024-05-27 15:35:16.000000 rateslib-1.2.0/rateslib/instruments.py
+-rw-r--r--   0      501       20    89067 2024-03-28 15:38:51.000000 rateslib-1.2.0/rateslib/legs.py
+-rw-r--r--   0      501       20   148587 2024-05-26 11:20:41.000000 rateslib-1.2.0/rateslib/periods.py
+-rw-r--r--   0      501       20    52433 2024-04-27 12:14:32.000000 rateslib-1.2.0/rateslib/scheduling.py
+-rw-r--r--   0      501       20    90302 2024-05-21 18:13:33.000000 rateslib-1.2.0/rateslib/solver.py
+-rw-r--r--   0      501       20     1680 2024-05-05 13:59:59.000000 rateslib-1.2.0/rateslib/splines/__init__.py
+-rw-r--r--   0      501       20    17108 2024-04-10 05:36:39.000000 rateslib-1.2.0/rateslib/splines/splines.py
+-rw-r--r--   0      501       20      468 2024-04-10 05:36:39.000000 rateslib-1.2.0/rateslib/splines/splinesrs.py
+-rw-r--r--   0      501       20      223 2023-11-24 18:08:12.000000 rateslib-1.2.0/requirements-latest.txt
+-rw-r--r--   0      501       20      246 2023-08-27 20:52:17.000000 rateslib-1.2.0/requirements-minimum.txt
+-rw-r--r--   0      501       20      487 2023-11-24 18:08:12.000000 rateslib-1.2.0/requirements.txt
+-rw-r--r--   0      501       20     1635 2024-03-10 16:22:16.000000 rateslib-1.2.0/scratch2.py
+-rw-r--r--   0      501       20     1869 2024-05-26 14:40:40.000000 rateslib-1.2.0/scratch3.py
+-rw-r--r--   0      501       20      614 2024-05-25 10:49:09.000000 rateslib-1.2.0/scratch4.py
+-rw-r--r--   0      501       20      104 2024-03-28 15:38:51.000000 rateslib-1.2.0/setup.py
+-rw-r--r--   0      501       20      389 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/_README.txt
+-rw-r--r--   0      501       20      971 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/curves/interpolation.rs
+-rw-r--r--   0      501       20      379 2024-05-19 08:41:12.000000 rateslib-1.2.0/src/curves/interpolation_py.rs
+-rw-r--r--   0      501       20       49 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/curves/mod.rs
+-rw-r--r--   0      501       20    41466 2024-04-20 09:04:46.000000 rateslib-1.2.0/src/dual/dual1.rs
+-rw-r--r--   0      501       20    37845 2024-04-20 09:04:46.000000 rateslib-1.2.0/src/dual/dual2.rs
+-rw-r--r--   0      501       20    15647 2024-04-20 09:04:46.000000 rateslib-1.2.0/src/dual/dual_py.rs
+-rw-r--r--   0      501       20    15502 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/dual/linalg.rs
+-rw-r--r--   0      501       20     7222 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/dual/linalg_f64.rs
+-rw-r--r--   0      501       20     2516 2024-04-11 15:36:27.000000 rateslib-1.2.0/src/dual/linalg_py.rs
+-rw-r--r--   0      501       20      102 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/dual/mod.rs
+-rw-r--r--   0      501       20     1190 2024-04-11 15:36:27.000000 rateslib-1.2.0/src/lib.rs
+-rw-r--r--   0      501       20      386 2024-05-18 21:00:21.000000 rateslib-1.2.0/src/main.rs
+-rw-r--r--   0      501       20       39 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/splines/mod.rs
+-rw-r--r--   0      501       20    19976 2024-04-27 12:14:32.000000 rateslib-1.2.0/src/splines/spline_f64.rs
+-rw-r--r--   0      501       20     6177 2024-04-20 09:07:47.000000 rateslib-1.2.0/src/splines/spline_py.rs
+-rw-r--r--   0      501       20      231 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/tests/dual1.rs
+-rw-r--r--   0      501       20       14 2024-04-10 05:36:39.000000 rateslib-1.2.0/src/tests/mod.rs
+-rw-r--r--   0      501       20      147 2023-08-27 20:52:17.000000 rateslib-1.2.0/tests/context.py
+-rw-r--r--   0      501       20      396 2023-09-09 07:16:43.000000 rateslib-1.2.0/tests/pytest.ini
+-rw-r--r--   0      501       20    12908 2024-04-19 15:12:59.000000 rateslib-1.2.0/tests/test_calendars.py
+-rw-r--r--   0      501       20    50375 2024-05-18 21:00:21.000000 rateslib-1.2.0/tests/test_curves.py
+-rw-r--r--   0      501       20     1337 2024-04-10 05:36:39.000000 rateslib-1.2.0/tests/test_default.py
+-rw-r--r--   0      501       20    26467 2024-04-10 05:36:39.000000 rateslib-1.2.0/tests/test_dual.py
+-rw-r--r--   0      501       20    22890 2024-04-10 05:36:39.000000 rateslib-1.2.0/tests/test_dualpy.py
+-rw-r--r--   0      501       20     8571 2024-04-10 05:36:39.000000 rateslib-1.2.0/tests/test_dualrs.py
+-rw-r--r--   0      501       20    36607 2024-04-10 05:36:39.000000 rateslib-1.2.0/tests/test_fx.py
+-rw-r--r--   0      501       20    18814 2024-05-20 16:00:35.000000 rateslib-1.2.0/tests/test_fx_volatility.py
+-rw-r--r--   0      501       20   154267 2024-05-27 15:35:16.000000 rateslib-1.2.0/tests/test_instruments.py
+-rw-r--r--   0      501       20    76328 2024-05-20 21:07:17.000000 rateslib-1.2.0/tests/test_instruments_bonds.py
+-rw-r--r--   0      501       20    59196 2024-02-04 15:26:34.000000 rateslib-1.2.0/tests/test_legs.py
+-rw-r--r--   0      501       20    95749 2024-05-26 08:48:54.000000 rateslib-1.2.0/tests/test_periods.py
+-rw-r--r--   0      501       20    31805 2024-04-19 15:12:59.000000 rateslib-1.2.0/tests/test_scheduling.py
+-rw-r--r--   0      501       20    64793 2024-05-24 16:32:59.000000 rateslib-1.2.0/tests/test_solver.py
+-rw-r--r--   0      501       20     9108 2024-04-20 09:04:46.000000 rateslib-1.2.0/tests/test_splines.py
+-rw-r--r--   0      501       20     1231 2024-04-10 05:36:38.000000 rateslib-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3638 1970-01-01 00:00:00.000000 rateslib-1.2.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `rateslib-1.1.1/LICENSE` & `rateslib-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/MANIFEST.in` & `rateslib-1.2.0/MANIFEST.in`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 include rateslib/data/corra.csv
 include rateslib/data/estr.csv
-include rateslib/data/instrument_spec.csv
+include rateslib/data/__instrument_spec.csv
 include rateslib/data/nowa.csv
 include rateslib/data/sofr.csv
 include rateslib/data/sonia.csv
 include rateslib/data/swestr.csv
 include rateslib/data/eur_ibor_1m.csv
 include rateslib/data/eur_ibor_3m.csv
 include rateslib/data/eur_ibor_6m.csv
@@ -14,8 +14,8 @@
 include rateslib/data/cad_rfr.csv
 include rateslib/data/chf_rfr.csv
 include rateslib/data/nok_rfr.csv
 include rateslib/data/sek_rfr.csv
 include rateslib/data/usd_rfr.csv
 
 include rateslib/dual/*
-include rateslib/splines/*
+include rateslib/splines/*
```

### Comparing `rateslib-1.1.1/PKG-INFO` & `rateslib-1.2.0/docs/source/i_licence.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,1603 +1,1117 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 7261 7465  : 2.1.Name: rate
-00000020: 736c 6962 0a56 6572 7369 6f6e 3a20 312e  slib.Version: 1.
-00000030: 312e 310a 5375 6d6d 6172 793a 2041 2066  1.1.Summary: A f
-00000040: 6978 6564 2069 6e63 6f6d 6520 6c69 6272  ixed income libr
-00000050: 6172 7920 666f 7220 7472 6164 696e 6720  ary for trading 
-00000060: 696e 7465 7265 7374 2072 6174 6573 0a41  interest rates.A
-00000070: 7574 686f 723a 204a 2048 204d 2044 6172  uthor: J H M Dar
-00000080: 6279 7368 6972 650a 4c69 6365 6e73 653a  byshire.License:
-00000090: 2041 7474 7269 6275 7469 6f6e 2d4e 6f6e   Attribution-Non
-000000a0: 436f 6d6d 6572 6369 616c 2d4e 6f44 6572  Commercial-NoDer
-000000b0: 6976 6174 6976 6573 2034 2e30 2049 6e74  ivatives 4.0 Int
-000000c0: 6572 6e61 7469 6f6e 616c 0a20 2020 2020  ernational.     
-000000d0: 2020 200a 2020 2020 2020 2020 3d3d 3d3d     .        ====
-000000e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000000f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000120: 3d3d 3d0a 2020 2020 2020 2020 0a20 2020  ===.        .   
-00000130: 2020 2020 2043 7265 6174 6976 6520 436f       Creative Co
-00000140: 6d6d 6f6e 7320 436f 7270 6f72 6174 696f  mmons Corporatio
-00000150: 6e20 2822 4372 6561 7469 7665 2043 6f6d  n ("Creative Com
-00000160: 6d6f 6e73 2229 2069 7320 6e6f 7420 6120  mons") is not a 
-00000170: 6c61 7720 6669 726d 2061 6e64 0a20 2020  law firm and.   
-00000180: 2020 2020 2064 6f65 7320 6e6f 7420 7072       does not pr
-00000190: 6f76 6964 6520 6c65 6761 6c20 7365 7276  ovide legal serv
-000001a0: 6963 6573 206f 7220 6c65 6761 6c20 6164  ices or legal ad
-000001b0: 7669 6365 2e20 4469 7374 7269 6275 7469  vice. Distributi
-000001c0: 6f6e 206f 660a 2020 2020 2020 2020 4372  on of.        Cr
-000001d0: 6561 7469 7665 2043 6f6d 6d6f 6e73 2070  eative Commons p
-000001e0: 7562 6c69 6320 6c69 6365 6e73 6573 2064  ublic licenses d
-000001f0: 6f65 7320 6e6f 7420 6372 6561 7465 2061  oes not create a
-00000200: 206c 6177 7965 722d 636c 6965 6e74 206f   lawyer-client o
-00000210: 720a 2020 2020 2020 2020 6f74 6865 7220  r.        other 
-00000220: 7265 6c61 7469 6f6e 7368 6970 2e20 4372  relationship. Cr
-00000230: 6561 7469 7665 2043 6f6d 6d6f 6e73 206d  eative Commons m
-00000240: 616b 6573 2069 7473 206c 6963 656e 7365  akes its license
-00000250: 7320 616e 6420 7265 6c61 7465 640a 2020  s and related.  
-00000260: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-00000270: 6e20 6176 6169 6c61 626c 6520 6f6e 2061  n available on a
-00000280: 6e20 2261 732d 6973 2220 6261 7369 732e  n "as-is" basis.
-00000290: 2043 7265 6174 6976 6520 436f 6d6d 6f6e   Creative Common
-000002a0: 7320 6769 7665 7320 6e6f 0a20 2020 2020  s gives no.     
-000002b0: 2020 2077 6172 7261 6e74 6965 7320 7265     warranties re
-000002c0: 6761 7264 696e 6720 6974 7320 6c69 6365  garding its lice
-000002d0: 6e73 6573 2c20 616e 7920 6d61 7465 7269  nses, any materi
-000002e0: 616c 206c 6963 656e 7365 6420 756e 6465  al licensed unde
-000002f0: 7220 7468 6569 720a 2020 2020 2020 2020  r their.        
-00000300: 7465 726d 7320 616e 6420 636f 6e64 6974  terms and condit
-00000310: 696f 6e73 2c20 6f72 2061 6e79 2072 656c  ions, or any rel
-00000320: 6174 6564 2069 6e66 6f72 6d61 7469 6f6e  ated information
-00000330: 2e20 4372 6561 7469 7665 2043 6f6d 6d6f  . Creative Commo
-00000340: 6e73 0a20 2020 2020 2020 2064 6973 636c  ns.        discl
-00000350: 6169 6d73 2061 6c6c 206c 6961 6269 6c69  aims all liabili
-00000360: 7479 2066 6f72 2064 616d 6167 6573 2072  ty for damages r
-00000370: 6573 756c 7469 6e67 2066 726f 6d20 7468  esulting from th
-00000380: 6569 7220 7573 6520 746f 2074 6865 0a20  eir use to the. 
-00000390: 2020 2020 2020 2066 756c 6c65 7374 2065         fullest e
-000003a0: 7874 656e 7420 706f 7373 6962 6c65 2e0a  xtent possible..
-000003b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000003c0: 2055 7369 6e67 2043 7265 6174 6976 6520   Using Creative 
-000003d0: 436f 6d6d 6f6e 7320 5075 626c 6963 204c  Commons Public L
-000003e0: 6963 656e 7365 730a 2020 2020 2020 2020  icenses.        
-000003f0: 0a20 2020 2020 2020 2043 7265 6174 6976  .        Creativ
-00000400: 6520 436f 6d6d 6f6e 7320 7075 626c 6963  e Commons public
-00000410: 206c 6963 656e 7365 7320 7072 6f76 6964   licenses provid
-00000420: 6520 6120 7374 616e 6461 7264 2073 6574  e a standard set
-00000430: 206f 6620 7465 726d 7320 616e 640a 2020   of terms and.  
-00000440: 2020 2020 2020 636f 6e64 6974 696f 6e73        conditions
-00000450: 2074 6861 7420 6372 6561 746f 7273 2061   that creators a
-00000460: 6e64 206f 7468 6572 2072 6967 6874 7320  nd other rights 
-00000470: 686f 6c64 6572 7320 6d61 7920 7573 6520  holders may use 
-00000480: 746f 2073 6861 7265 0a20 2020 2020 2020  to share.       
-00000490: 206f 7269 6769 6e61 6c20 776f 726b 7320   original works 
-000004a0: 6f66 2061 7574 686f 7273 6869 7020 616e  of authorship an
-000004b0: 6420 6f74 6865 7220 6d61 7465 7269 616c  d other material
-000004c0: 2073 7562 6a65 6374 2074 6f20 636f 7079   subject to copy
-000004d0: 7269 6768 740a 2020 2020 2020 2020 616e  right.        an
-000004e0: 6420 6365 7274 6169 6e20 6f74 6865 7220  d certain other 
-000004f0: 7269 6768 7473 2073 7065 6369 6669 6564  rights specified
-00000500: 2069 6e20 7468 6520 7075 626c 6963 206c   in the public l
-00000510: 6963 656e 7365 2062 656c 6f77 2e20 5468  icense below. Th
-00000520: 650a 2020 2020 2020 2020 666f 6c6c 6f77  e.        follow
-00000530: 696e 6720 636f 6e73 6964 6572 6174 696f  ing consideratio
-00000540: 6e73 2061 7265 2066 6f72 2069 6e66 6f72  ns are for infor
-00000550: 6d61 7469 6f6e 616c 2070 7572 706f 7365  mational purpose
-00000560: 7320 6f6e 6c79 2c20 6172 6520 6e6f 740a  s only, are not.
-00000570: 2020 2020 2020 2020 6578 6861 7573 7469          exhausti
-00000580: 7665 2c20 616e 6420 646f 206e 6f74 2066  ve, and do not f
-00000590: 6f72 6d20 7061 7274 206f 6620 6f75 7220  orm part of our 
-000005a0: 6c69 6365 6e73 6573 2e0a 2020 2020 2020  licenses..      
-000005b0: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-000005c0: 436f 6e73 6964 6572 6174 696f 6e73 2066  Considerations f
-000005d0: 6f72 206c 6963 656e 736f 7273 3a20 4f75  or licensors: Ou
-000005e0: 7220 7075 626c 6963 206c 6963 656e 7365  r public license
-000005f0: 7320 6172 650a 2020 2020 2020 2020 2020  s are.          
-00000600: 2020 2069 6e74 656e 6465 6420 666f 7220     intended for 
-00000610: 7573 6520 6279 2074 686f 7365 2061 7574  use by those aut
-00000620: 686f 7269 7a65 6420 746f 2067 6976 6520  horized to give 
-00000630: 7468 6520 7075 626c 6963 0a20 2020 2020  the public.     
-00000640: 2020 2020 2020 2020 7065 726d 6973 7369          permissi
-00000650: 6f6e 2074 6f20 7573 6520 6d61 7465 7269  on to use materi
-00000660: 616c 2069 6e20 7761 7973 206f 7468 6572  al in ways other
-00000670: 7769 7365 2072 6573 7472 6963 7465 6420  wise restricted 
-00000680: 6279 0a20 2020 2020 2020 2020 2020 2020  by.             
-00000690: 636f 7079 7269 6768 7420 616e 6420 6365  copyright and ce
-000006a0: 7274 6169 6e20 6f74 6865 7220 7269 6768  rtain other righ
-000006b0: 7473 2e20 4f75 7220 6c69 6365 6e73 6573  ts. Our licenses
-000006c0: 2061 7265 0a20 2020 2020 2020 2020 2020   are.           
-000006d0: 2020 6972 7265 766f 6361 626c 652e 204c    irrevocable. L
-000006e0: 6963 656e 736f 7273 2073 686f 756c 6420  icensors should 
-000006f0: 7265 6164 2061 6e64 2075 6e64 6572 7374  read and underst
-00000700: 616e 6420 7468 6520 7465 726d 730a 2020  and the terms.  
-00000710: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
-00000720: 6f6e 6469 7469 6f6e 7320 6f66 2074 6865  onditions of the
-00000730: 206c 6963 656e 7365 2074 6865 7920 6368   license they ch
-00000740: 6f6f 7365 2062 6566 6f72 6520 6170 706c  oose before appl
-00000750: 7969 6e67 2069 742e 0a20 2020 2020 2020  ying it..       
-00000760: 2020 2020 2020 4c69 6365 6e73 6f72 7320        Licensors 
-00000770: 7368 6f75 6c64 2061 6c73 6f20 7365 6375  should also secu
-00000780: 7265 2061 6c6c 2072 6967 6874 7320 6e65  re all rights ne
-00000790: 6365 7373 6172 7920 6265 666f 7265 0a20  cessary before. 
-000007a0: 2020 2020 2020 2020 2020 2020 6170 706c              appl
-000007b0: 7969 6e67 206f 7572 206c 6963 656e 7365  ying our license
-000007c0: 7320 736f 2074 6861 7420 7468 6520 7075  s so that the pu
-000007d0: 626c 6963 2063 616e 2072 6575 7365 2074  blic can reuse t
-000007e0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-000007f0: 6d61 7465 7269 616c 2061 7320 6578 7065  material as expe
-00000800: 6374 6564 2e20 4c69 6365 6e73 6f72 7320  cted. Licensors 
-00000810: 7368 6f75 6c64 2063 6c65 6172 6c79 206d  should clearly m
-00000820: 6172 6b20 616e 790a 2020 2020 2020 2020  ark any.        
-00000830: 2020 2020 206d 6174 6572 6961 6c20 6e6f       material no
-00000840: 7420 7375 626a 6563 7420 746f 2074 6865  t subject to the
-00000850: 206c 6963 656e 7365 2e20 5468 6973 2069   license. This i
-00000860: 6e63 6c75 6465 7320 6f74 6865 7220 4343  ncludes other CC
-00000870: 2d0a 2020 2020 2020 2020 2020 2020 206c  -.             l
-00000880: 6963 656e 7365 6420 6d61 7465 7269 616c  icensed material
-00000890: 2c20 6f72 206d 6174 6572 6961 6c20 7573  , or material us
-000008a0: 6564 2075 6e64 6572 2061 6e20 6578 6365  ed under an exce
-000008b0: 7074 696f 6e20 6f72 0a20 2020 2020 2020  ption or.       
-000008c0: 2020 2020 2020 6c69 6d69 7461 7469 6f6e        limitation
-000008d0: 2074 6f20 636f 7079 7269 6768 742e 204d   to copyright. M
-000008e0: 6f72 6520 636f 6e73 6964 6572 6174 696f  ore consideratio
-000008f0: 6e73 2066 6f72 206c 6963 656e 736f 7273  ns for licensors
-00000900: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00000910: 6b69 2e63 7265 6174 6976 6563 6f6d 6d6f  ki.creativecommo
-00000920: 6e73 2e6f 7267 2f43 6f6e 7369 6465 7261  ns.org/Considera
-00000930: 7469 6f6e 735f 666f 725f 6c69 6365 6e73  tions_for_licens
-00000940: 6f72 730a 2020 2020 2020 2020 0a20 2020  ors.        .   
-00000950: 2020 2020 2020 2020 2020 436f 6e73 6964            Consid
-00000960: 6572 6174 696f 6e73 2066 6f72 2074 6865  erations for the
-00000970: 2070 7562 6c69 633a 2042 7920 7573 696e   public: By usin
-00000980: 6720 6f6e 6520 6f66 206f 7572 2070 7562  g one of our pub
-00000990: 6c69 630a 2020 2020 2020 2020 2020 2020  lic.            
-000009a0: 206c 6963 656e 7365 732c 2061 206c 6963   licenses, a lic
-000009b0: 656e 736f 7220 6772 616e 7473 2074 6865  ensor grants the
-000009c0: 2070 7562 6c69 6320 7065 726d 6973 7369   public permissi
-000009d0: 6f6e 2074 6f20 7573 6520 7468 650a 2020  on to use the.  
-000009e0: 2020 2020 2020 2020 2020 206c 6963 656e             licen
-000009f0: 7365 6420 6d61 7465 7269 616c 2075 6e64  sed material und
-00000a00: 6572 2073 7065 6369 6669 6564 2074 6572  er specified ter
-00000a10: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
-00000a20: 732e 2049 660a 2020 2020 2020 2020 2020  s. If.          
-00000a30: 2020 2074 6865 206c 6963 656e 736f 7227     the licensor'
-00000a40: 7320 7065 726d 6973 7369 6f6e 2069 7320  s permission is 
-00000a50: 6e6f 7420 6e65 6365 7373 6172 7920 666f  not necessary fo
-00000a60: 7220 616e 7920 7265 6173 6f6e 2d2d 666f  r any reason--fo
-00000a70: 720a 2020 2020 2020 2020 2020 2020 2065  r.             e
-00000a80: 7861 6d70 6c65 2c20 6265 6361 7573 6520  xample, because 
-00000a90: 6f66 2061 6e79 2061 7070 6c69 6361 626c  of any applicabl
-00000aa0: 6520 6578 6365 7074 696f 6e20 6f72 206c  e exception or l
-00000ab0: 696d 6974 6174 696f 6e20 746f 0a20 2020  imitation to.   
-00000ac0: 2020 2020 2020 2020 2020 636f 7079 7269            copyri
-00000ad0: 6768 742d 2d74 6865 6e20 7468 6174 2075  ght--then that u
-00000ae0: 7365 2069 7320 6e6f 7420 7265 6775 6c61  se is not regula
-00000af0: 7465 6420 6279 2074 6865 206c 6963 656e  ted by the licen
-00000b00: 7365 2e20 4f75 720a 2020 2020 2020 2020  se. Our.        
-00000b10: 2020 2020 206c 6963 656e 7365 7320 6772       licenses gr
-00000b20: 616e 7420 6f6e 6c79 2070 6572 6d69 7373  ant only permiss
-00000b30: 696f 6e73 2075 6e64 6572 2063 6f70 7972  ions under copyr
-00000b40: 6967 6874 2061 6e64 2063 6572 7461 696e  ight and certain
-00000b50: 0a20 2020 2020 2020 2020 2020 2020 6f74  .             ot
-00000b60: 6865 7220 7269 6768 7473 2074 6861 7420  her rights that 
-00000b70: 6120 6c69 6365 6e73 6f72 2068 6173 2061  a licensor has a
-00000b80: 7574 686f 7269 7479 2074 6f20 6772 616e  uthority to gran
-00000b90: 742e 2055 7365 206f 660a 2020 2020 2020  t. Use of.      
-00000ba0: 2020 2020 2020 2074 6865 206c 6963 656e         the licen
-00000bb0: 7365 6420 6d61 7465 7269 616c 206d 6179  sed material may
-00000bc0: 2073 7469 6c6c 2062 6520 7265 7374 7269   still be restri
-00000bd0: 6374 6564 2066 6f72 206f 7468 6572 0a20  cted for other. 
-00000be0: 2020 2020 2020 2020 2020 2020 7265 6173              reas
-00000bf0: 6f6e 732c 2069 6e63 6c75 6469 6e67 2062  ons, including b
-00000c00: 6563 6175 7365 206f 7468 6572 7320 6861  ecause others ha
-00000c10: 7665 2063 6f70 7972 6967 6874 206f 7220  ve copyright or 
-00000c20: 6f74 6865 720a 2020 2020 2020 2020 2020  other.          
-00000c30: 2020 2072 6967 6874 7320 696e 2074 6865     rights in the
-00000c40: 206d 6174 6572 6961 6c2e 2041 206c 6963   material. A lic
-00000c50: 656e 736f 7220 6d61 7920 6d61 6b65 2073  ensor may make s
-00000c60: 7065 6369 616c 2072 6571 7565 7374 732c  pecial requests,
-00000c70: 0a20 2020 2020 2020 2020 2020 2020 7375  .             su
-00000c80: 6368 2061 7320 6173 6b69 6e67 2074 6861  ch as asking tha
-00000c90: 7420 616c 6c20 6368 616e 6765 7320 6265  t all changes be
-00000ca0: 206d 6172 6b65 6420 6f72 2064 6573 6372   marked or descr
-00000cb0: 6962 6564 2e0a 2020 2020 2020 2020 2020  ibed..          
-00000cc0: 2020 2041 6c74 686f 7567 6820 6e6f 7420     Although not 
-00000cd0: 7265 7175 6972 6564 2062 7920 6f75 7220  required by our 
-00000ce0: 6c69 6365 6e73 6573 2c20 796f 7520 6172  licenses, you ar
-00000cf0: 6520 656e 636f 7572 6167 6564 2074 6f0a  e encouraged to.
-00000d00: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00000d10: 7065 6374 2074 686f 7365 2072 6571 7565  pect those reque
-00000d20: 7374 7320 7768 6572 6520 7265 6173 6f6e  sts where reason
-00000d30: 6162 6c65 2e20 4d6f 7265 2063 6f6e 7369  able. More consi
-00000d40: 6465 7261 7469 6f6e 730a 2020 2020 2020  derations.      
-00000d50: 2020 2020 2020 2066 6f72 2074 6865 2070         for the p
-00000d60: 7562 6c69 633a 0a20 2020 2020 2020 2020  ublic:.         
-00000d70: 2020 2077 696b 692e 6372 6561 7469 7665     wiki.creative
-00000d80: 636f 6d6d 6f6e 732e 6f72 672f 436f 6e73  commons.org/Cons
-00000d90: 6964 6572 6174 696f 6e73 5f66 6f72 5f6c  iderations_for_l
-00000da0: 6963 656e 7365 6573 0a20 2020 2020 2020  icensees.       
-00000db0: 200a 2020 2020 2020 2020 3d3d 3d3d 3d3d   .        ======
-00000dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000de0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000e00: 3d0a 2020 2020 2020 2020 0a20 2020 2020  =.        .     
-00000e10: 2020 2043 7265 6174 6976 6520 436f 6d6d     Creative Comm
-00000e20: 6f6e 7320 4174 7472 6962 7574 696f 6e2d  ons Attribution-
-00000e30: 4e6f 6e43 6f6d 6d65 7263 6961 6c2d 4e6f  NonCommercial-No
-00000e40: 4465 7269 7661 7469 7665 7320 342e 300a  Derivatives 4.0.
-00000e50: 2020 2020 2020 2020 496e 7465 726e 6174          Internat
-00000e60: 696f 6e61 6c20 5075 626c 6963 204c 6963  ional Public Lic
-00000e70: 656e 7365 0a20 2020 2020 2020 200a 2020  ense.        .  
-00000e80: 2020 2020 2020 4279 2065 7865 7263 6973        By exercis
-00000e90: 696e 6720 7468 6520 4c69 6365 6e73 6564  ing the Licensed
-00000ea0: 2052 6967 6874 7320 2864 6566 696e 6564   Rights (defined
-00000eb0: 2062 656c 6f77 292c 2059 6f75 2061 6363   below), You acc
-00000ec0: 6570 7420 616e 6420 6167 7265 650a 2020  ept and agree.  
-00000ed0: 2020 2020 2020 746f 2062 6520 626f 756e        to be boun
-00000ee0: 6420 6279 2074 6865 2074 6572 6d73 2061  d by the terms a
-00000ef0: 6e64 2063 6f6e 6469 7469 6f6e 7320 6f66  nd conditions of
-00000f00: 2074 6869 7320 4372 6561 7469 7665 2043   this Creative C
-00000f10: 6f6d 6d6f 6e73 0a20 2020 2020 2020 2041  ommons.        A
-00000f20: 7474 7269 6275 7469 6f6e 2d4e 6f6e 436f  ttribution-NonCo
-00000f30: 6d6d 6572 6369 616c 2d4e 6f44 6572 6976  mmercial-NoDeriv
-00000f40: 6174 6976 6573 2034 2e30 2049 6e74 6572  atives 4.0 Inter
-00000f50: 6e61 7469 6f6e 616c 2050 7562 6c69 630a  national Public.
-00000f60: 2020 2020 2020 2020 4c69 6365 6e73 6520          License 
-00000f70: 2822 5075 626c 6963 204c 6963 656e 7365  ("Public License
-00000f80: 2229 2e20 546f 2074 6865 2065 7874 656e  "). To the exten
-00000f90: 7420 7468 6973 2050 7562 6c69 6320 4c69  t this Public Li
-00000fa0: 6365 6e73 6520 6d61 7920 6265 0a20 2020  cense may be.   
-00000fb0: 2020 2020 2069 6e74 6572 7072 6574 6564       interpreted
-00000fc0: 2061 7320 6120 636f 6e74 7261 6374 2c20   as a contract, 
-00000fd0: 596f 7520 6172 6520 6772 616e 7465 6420  You are granted 
-00000fe0: 7468 6520 4c69 6365 6e73 6564 2052 6967  the Licensed Rig
-00000ff0: 6874 7320 696e 0a20 2020 2020 2020 2063  hts in.        c
-00001000: 6f6e 7369 6465 7261 7469 6f6e 206f 6620  onsideration of 
-00001010: 596f 7572 2061 6363 6570 7461 6e63 6520  Your acceptance 
-00001020: 6f66 2074 6865 7365 2074 6572 6d73 2061  of these terms a
-00001030: 6e64 2063 6f6e 6469 7469 6f6e 732c 2061  nd conditions, a
-00001040: 6e64 2074 6865 0a20 2020 2020 2020 204c  nd the.        L
-00001050: 6963 656e 736f 7220 6772 616e 7473 2059  icensor grants Y
-00001060: 6f75 2073 7563 6820 7269 6768 7473 2069  ou such rights i
-00001070: 6e20 636f 6e73 6964 6572 6174 696f 6e20  n consideration 
-00001080: 6f66 2062 656e 6566 6974 7320 7468 650a  of benefits the.
-00001090: 2020 2020 2020 2020 4c69 6365 6e73 6f72          Licensor
-000010a0: 2072 6563 6569 7665 7320 6672 6f6d 206d   receives from m
-000010b0: 616b 696e 6720 7468 6520 4c69 6365 6e73  aking the Licens
-000010c0: 6564 204d 6174 6572 6961 6c20 6176 6169  ed Material avai
-000010d0: 6c61 626c 6520 756e 6465 720a 2020 2020  lable under.    
-000010e0: 2020 2020 7468 6573 6520 7465 726d 7320      these terms 
-000010f0: 616e 6420 636f 6e64 6974 696f 6e73 2e0a  and conditions..
-00001100: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001110: 200a 2020 2020 2020 2020 5365 6374 696f   .        Sectio
-00001120: 6e20 3120 2d2d 2044 6566 696e 6974 696f  n 1 -- Definitio
-00001130: 6e73 2e0a 2020 2020 2020 2020 0a20 2020  ns..        .   
-00001140: 2020 2020 2020 2061 2e20 4164 6170 7465         a. Adapte
-00001150: 6420 4d61 7465 7269 616c 206d 6561 6e73  d Material means
-00001160: 206d 6174 6572 6961 6c20 7375 626a 6563   material subjec
-00001170: 7420 746f 2043 6f70 7972 6967 6874 2061  t to Copyright a
-00001180: 6e64 2053 696d 696c 6172 0a20 2020 2020  nd Similar.     
-00001190: 2020 2020 2020 2020 5269 6768 7473 2074          Rights t
-000011a0: 6861 7420 6973 2064 6572 6976 6564 2066  hat is derived f
-000011b0: 726f 6d20 6f72 2062 6173 6564 2075 706f  rom or based upo
-000011c0: 6e20 7468 6520 4c69 6365 6e73 6564 204d  n the Licensed M
-000011d0: 6174 6572 6961 6c0a 2020 2020 2020 2020  aterial.        
-000011e0: 2020 2020 2061 6e64 2069 6e20 7768 6963       and in whic
-000011f0: 6820 7468 6520 4c69 6365 6e73 6564 204d  h the Licensed M
-00001200: 6174 6572 6961 6c20 6973 2074 7261 6e73  aterial is trans
-00001210: 6c61 7465 642c 2061 6c74 6572 6564 2c0a  lated, altered,.
-00001220: 2020 2020 2020 2020 2020 2020 2061 7272               arr
-00001230: 616e 6765 642c 2074 7261 6e73 666f 726d  anged, transform
-00001240: 6564 2c20 6f72 206f 7468 6572 7769 7365  ed, or otherwise
-00001250: 206d 6f64 6966 6965 6420 696e 2061 206d   modified in a m
-00001260: 616e 6e65 7220 7265 7175 6972 696e 670a  anner requiring.
-00001270: 2020 2020 2020 2020 2020 2020 2070 6572               per
-00001280: 6d69 7373 696f 6e20 756e 6465 7220 7468  mission under th
-00001290: 6520 436f 7079 7269 6768 7420 616e 6420  e Copyright and 
-000012a0: 5369 6d69 6c61 7220 5269 6768 7473 2068  Similar Rights h
-000012b0: 656c 6420 6279 2074 6865 0a20 2020 2020  eld by the.     
-000012c0: 2020 2020 2020 2020 4c69 6365 6e73 6f72          Licensor
-000012d0: 2e20 466f 7220 7075 7270 6f73 6573 206f  . For purposes o
-000012e0: 6620 7468 6973 2050 7562 6c69 6320 4c69  f this Public Li
-000012f0: 6365 6e73 652c 2077 6865 7265 2074 6865  cense, where the
-00001300: 204c 6963 656e 7365 640a 2020 2020 2020   Licensed.      
-00001310: 2020 2020 2020 204d 6174 6572 6961 6c20         Material 
-00001320: 6973 2061 206d 7573 6963 616c 2077 6f72  is a musical wor
-00001330: 6b2c 2070 6572 666f 726d 616e 6365 2c20  k, performance, 
-00001340: 6f72 2073 6f75 6e64 2072 6563 6f72 6469  or sound recordi
-00001350: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-00001360: 2041 6461 7074 6564 204d 6174 6572 6961   Adapted Materia
-00001370: 6c20 6973 2061 6c77 6179 7320 7072 6f64  l is always prod
-00001380: 7563 6564 2077 6865 7265 2074 6865 204c  uced where the L
-00001390: 6963 656e 7365 6420 4d61 7465 7269 616c  icensed Material
-000013a0: 2069 730a 2020 2020 2020 2020 2020 2020   is.            
-000013b0: 2073 796e 6368 6564 2069 6e20 7469 6d65   synched in time
-000013c0: 6420 7265 6c61 7469 6f6e 2077 6974 6820  d relation with 
-000013d0: 6120 6d6f 7669 6e67 2069 6d61 6765 2e0a  a moving image..
-000013e0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-000013f0: 2020 2062 2e20 436f 7079 7269 6768 7420     b. Copyright 
-00001400: 616e 6420 5369 6d69 6c61 7220 5269 6768  and Similar Righ
-00001410: 7473 206d 6561 6e73 2063 6f70 7972 6967  ts means copyrig
-00001420: 6874 2061 6e64 2f6f 7220 7369 6d69 6c61  ht and/or simila
-00001430: 7220 7269 6768 7473 0a20 2020 2020 2020  r rights.       
-00001440: 2020 2020 2020 636c 6f73 656c 7920 7265        closely re
-00001450: 6c61 7465 6420 746f 2063 6f70 7972 6967  lated to copyrig
-00001460: 6874 2069 6e63 6c75 6469 6e67 2c20 7769  ht including, wi
-00001470: 7468 6f75 7420 6c69 6d69 7461 7469 6f6e  thout limitation
-00001480: 2c0a 2020 2020 2020 2020 2020 2020 2070  ,.             p
-00001490: 6572 666f 726d 616e 6365 2c20 6272 6f61  erformance, broa
-000014a0: 6463 6173 742c 2073 6f75 6e64 2072 6563  dcast, sound rec
-000014b0: 6f72 6469 6e67 2c20 616e 6420 5375 6920  ording, and Sui 
-000014c0: 4765 6e65 7269 7320 4461 7461 6261 7365  Generis Database
-000014d0: 0a20 2020 2020 2020 2020 2020 2020 5269  .             Ri
-000014e0: 6768 7473 2c20 7769 7468 6f75 7420 7265  ghts, without re
-000014f0: 6761 7264 2074 6f20 686f 7720 7468 6520  gard to how the 
-00001500: 7269 6768 7473 2061 7265 206c 6162 656c  rights are label
-00001510: 6564 206f 720a 2020 2020 2020 2020 2020  ed or.          
-00001520: 2020 2063 6174 6567 6f72 697a 6564 2e20     categorized. 
-00001530: 466f 7220 7075 7270 6f73 6573 206f 6620  For purposes of 
-00001540: 7468 6973 2050 7562 6c69 6320 4c69 6365  this Public Lice
-00001550: 6e73 652c 2074 6865 2072 6967 6874 730a  nse, the rights.
-00001560: 2020 2020 2020 2020 2020 2020 2073 7065               spe
-00001570: 6369 6669 6564 2069 6e20 5365 6374 696f  cified in Sectio
-00001580: 6e20 3228 6229 2831 292d 2832 2920 6172  n 2(b)(1)-(2) ar
-00001590: 6520 6e6f 7420 436f 7079 7269 6768 7420  e not Copyright 
-000015a0: 616e 6420 5369 6d69 6c61 720a 2020 2020  and Similar.    
-000015b0: 2020 2020 2020 2020 2052 6967 6874 732e           Rights.
-000015c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015d0: 2020 2020 632e 2045 6666 6563 7469 7665      c. Effective
-000015e0: 2054 6563 686e 6f6c 6f67 6963 616c 204d   Technological M
-000015f0: 6561 7375 7265 7320 6d65 616e 7320 7468  easures means th
-00001600: 6f73 6520 6d65 6173 7572 6573 2074 6861  ose measures tha
-00001610: 742c 2069 6e20 7468 650a 2020 2020 2020  t, in the.      
-00001620: 2020 2020 2020 2061 6273 656e 6365 206f         absence o
-00001630: 6620 7072 6f70 6572 2061 7574 686f 7269  f proper authori
-00001640: 7479 2c20 6d61 7920 6e6f 7420 6265 2063  ty, may not be c
-00001650: 6972 6375 6d76 656e 7465 6420 756e 6465  ircumvented unde
-00001660: 7220 6c61 7773 0a20 2020 2020 2020 2020  r laws.         
-00001670: 2020 2020 6675 6c66 696c 6c69 6e67 206f      fulfilling o
-00001680: 626c 6967 6174 696f 6e73 2075 6e64 6572  bligations under
-00001690: 2041 7274 6963 6c65 2031 3120 6f66 2074   Article 11 of t
-000016a0: 6865 2057 4950 4f20 436f 7079 7269 6768  he WIPO Copyrigh
-000016b0: 740a 2020 2020 2020 2020 2020 2020 2054  t.             T
-000016c0: 7265 6174 7920 6164 6f70 7465 6420 6f6e  reaty adopted on
-000016d0: 2044 6563 656d 6265 7220 3230 2c20 3139   December 20, 19
-000016e0: 3936 2c20 616e 642f 6f72 2073 696d 696c  96, and/or simil
-000016f0: 6172 2069 6e74 6572 6e61 7469 6f6e 616c  ar international
-00001700: 0a20 2020 2020 2020 2020 2020 2020 6167  .             ag
-00001710: 7265 656d 656e 7473 2e0a 2020 2020 2020  reements..      
-00001720: 2020 0a20 2020 2020 2020 2020 2064 2e20    .          d. 
-00001730: 4578 6365 7074 696f 6e73 2061 6e64 204c  Exceptions and L
-00001740: 696d 6974 6174 696f 6e73 206d 6561 6e73  imitations means
-00001750: 2066 6169 7220 7573 652c 2066 6169 7220   fair use, fair 
-00001760: 6465 616c 696e 672c 2061 6e64 2f6f 720a  dealing, and/or.
-00001770: 2020 2020 2020 2020 2020 2020 2061 6e79               any
-00001780: 206f 7468 6572 2065 7863 6570 7469 6f6e   other exception
-00001790: 206f 7220 6c69 6d69 7461 7469 6f6e 2074   or limitation t
-000017a0: 6f20 436f 7079 7269 6768 7420 616e 6420  o Copyright and 
-000017b0: 5369 6d69 6c61 7220 5269 6768 7473 0a20  Similar Rights. 
-000017c0: 2020 2020 2020 2020 2020 2020 7468 6174              that
-000017d0: 2061 7070 6c69 6573 2074 6f20 596f 7572   applies to Your
-000017e0: 2075 7365 206f 6620 7468 6520 4c69 6365   use of the Lice
-000017f0: 6e73 6564 204d 6174 6572 6961 6c2e 0a20  nsed Material.. 
-00001800: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001810: 2020 652e 204c 6963 656e 7365 6420 4d61    e. Licensed Ma
-00001820: 7465 7269 616c 206d 6561 6e73 2074 6865  terial means the
-00001830: 2061 7274 6973 7469 6320 6f72 206c 6974   artistic or lit
-00001840: 6572 6172 7920 776f 726b 2c20 6461 7461  erary work, data
-00001850: 6261 7365 2c0a 2020 2020 2020 2020 2020  base,.          
-00001860: 2020 206f 7220 6f74 6865 7220 6d61 7465     or other mate
-00001870: 7269 616c 2074 6f20 7768 6963 6820 7468  rial to which th
-00001880: 6520 4c69 6365 6e73 6f72 2061 7070 6c69  e Licensor appli
-00001890: 6564 2074 6869 7320 5075 626c 6963 0a20  ed this Public. 
-000018a0: 2020 2020 2020 2020 2020 2020 4c69 6365              Lice
-000018b0: 6e73 652e 0a20 2020 2020 2020 200a 2020  nse..        .  
-000018c0: 2020 2020 2020 2020 662e 204c 6963 656e          f. Licen
-000018d0: 7365 6420 5269 6768 7473 206d 6561 6e73  sed Rights means
-000018e0: 2074 6865 2072 6967 6874 7320 6772 616e   the rights gran
-000018f0: 7465 6420 746f 2059 6f75 2073 7562 6a65  ted to You subje
-00001900: 6374 2074 6f20 7468 650a 2020 2020 2020  ct to the.      
-00001910: 2020 2020 2020 2074 6572 6d73 2061 6e64         terms and
-00001920: 2063 6f6e 6469 7469 6f6e 7320 6f66 2074   conditions of t
-00001930: 6869 7320 5075 626c 6963 204c 6963 656e  his Public Licen
-00001940: 7365 2c20 7768 6963 6820 6172 6520 6c69  se, which are li
-00001950: 6d69 7465 6420 746f 0a20 2020 2020 2020  mited to.       
-00001960: 2020 2020 2020 616c 6c20 436f 7079 7269        all Copyri
-00001970: 6768 7420 616e 6420 5369 6d69 6c61 7220  ght and Similar 
-00001980: 5269 6768 7473 2074 6861 7420 6170 706c  Rights that appl
-00001990: 7920 746f 2059 6f75 7220 7573 6520 6f66  y to Your use of
-000019a0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-000019b0: 2020 4c69 6365 6e73 6564 204d 6174 6572    Licensed Mater
-000019c0: 6961 6c20 616e 6420 7468 6174 2074 6865  ial and that the
-000019d0: 204c 6963 656e 736f 7220 6861 7320 6175   Licensor has au
-000019e0: 7468 6f72 6974 7920 746f 206c 6963 656e  thority to licen
-000019f0: 7365 2e0a 2020 2020 2020 2020 0a20 2020  se..        .   
-00001a00: 2020 2020 2020 2067 2e20 4c69 6365 6e73         g. Licens
-00001a10: 6f72 206d 6561 6e73 2074 6865 2069 6e64  or means the ind
-00001a20: 6976 6964 7561 6c28 7329 206f 7220 656e  ividual(s) or en
-00001a30: 7469 7479 2869 6573 2920 6772 616e 7469  tity(ies) granti
-00001a40: 6e67 2072 6967 6874 730a 2020 2020 2020  ng rights.      
-00001a50: 2020 2020 2020 2075 6e64 6572 2074 6869         under thi
-00001a60: 7320 5075 626c 6963 204c 6963 656e 7365  s Public License
-00001a70: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00001a80: 2020 2020 2068 2e20 4e6f 6e43 6f6d 6d65       h. NonComme
-00001a90: 7263 6961 6c20 6d65 616e 7320 6e6f 7420  rcial means not 
-00001aa0: 7072 696d 6172 696c 7920 696e 7465 6e64  primarily intend
-00001ab0: 6564 2066 6f72 206f 7220 6469 7265 6374  ed for or direct
-00001ac0: 6564 2074 6f77 6172 6473 0a20 2020 2020  ed towards.     
-00001ad0: 2020 2020 2020 2020 636f 6d6d 6572 6369          commerci
-00001ae0: 616c 2061 6476 616e 7461 6765 206f 7220  al advantage or 
-00001af0: 6d6f 6e65 7461 7279 2063 6f6d 7065 6e73  monetary compens
-00001b00: 6174 696f 6e2e 2046 6f72 2070 7572 706f  ation. For purpo
-00001b10: 7365 7320 6f66 0a20 2020 2020 2020 2020  ses of.         
-00001b20: 2020 2020 7468 6973 2050 7562 6c69 6320      this Public 
-00001b30: 4c69 6365 6e73 652c 2074 6865 2065 7863  License, the exc
-00001b40: 6861 6e67 6520 6f66 2074 6865 204c 6963  hange of the Lic
-00001b50: 656e 7365 6420 4d61 7465 7269 616c 2066  ensed Material f
-00001b60: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00001b70: 6f74 6865 7220 6d61 7465 7269 616c 2073  other material s
-00001b80: 7562 6a65 6374 2074 6f20 436f 7079 7269  ubject to Copyri
-00001b90: 6768 7420 616e 6420 5369 6d69 6c61 7220  ght and Similar 
-00001ba0: 5269 6768 7473 2062 7920 6469 6769 7461  Rights by digita
-00001bb0: 6c0a 2020 2020 2020 2020 2020 2020 2066  l.             f
-00001bc0: 696c 652d 7368 6172 696e 6720 6f72 2073  ile-sharing or s
-00001bd0: 696d 696c 6172 206d 6561 6e73 2069 7320  imilar means is 
-00001be0: 4e6f 6e43 6f6d 6d65 7263 6961 6c20 7072  NonCommercial pr
-00001bf0: 6f76 6964 6564 2074 6865 7265 2069 730a  ovided there is.
-00001c00: 2020 2020 2020 2020 2020 2020 206e 6f20               no 
-00001c10: 7061 796d 656e 7420 6f66 206d 6f6e 6574  payment of monet
-00001c20: 6172 7920 636f 6d70 656e 7361 7469 6f6e  ary compensation
-00001c30: 2069 6e20 636f 6e6e 6563 7469 6f6e 2077   in connection w
-00001c40: 6974 6820 7468 650a 2020 2020 2020 2020  ith the.        
-00001c50: 2020 2020 2065 7863 6861 6e67 652e 0a20       exchange.. 
-00001c60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001c70: 2020 692e 2053 6861 7265 206d 6561 6e73    i. Share means
-00001c80: 2074 6f20 7072 6f76 6964 6520 6d61 7465   to provide mate
-00001c90: 7269 616c 2074 6f20 7468 6520 7075 626c  rial to the publ
-00001ca0: 6963 2062 7920 616e 7920 6d65 616e 7320  ic by any means 
-00001cb0: 6f72 0a20 2020 2020 2020 2020 2020 2020  or.             
-00001cc0: 7072 6f63 6573 7320 7468 6174 2072 6571  process that req
-00001cd0: 7569 7265 7320 7065 726d 6973 7369 6f6e  uires permission
-00001ce0: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
-00001cf0: 7365 6420 5269 6768 7473 2c20 7375 6368  sed Rights, such
-00001d00: 0a20 2020 2020 2020 2020 2020 2020 6173  .             as
-00001d10: 2072 6570 726f 6475 6374 696f 6e2c 2070   reproduction, p
-00001d20: 7562 6c69 6320 6469 7370 6c61 792c 2070  ublic display, p
-00001d30: 7562 6c69 6320 7065 7266 6f72 6d61 6e63  ublic performanc
-00001d40: 652c 2064 6973 7472 6962 7574 696f 6e2c  e, distribution,
-00001d50: 0a20 2020 2020 2020 2020 2020 2020 6469  .             di
-00001d60: 7373 656d 696e 6174 696f 6e2c 2063 6f6d  ssemination, com
-00001d70: 6d75 6e69 6361 7469 6f6e 2c20 6f72 2069  munication, or i
-00001d80: 6d70 6f72 7461 7469 6f6e 2c20 616e 6420  mportation, and 
-00001d90: 746f 206d 616b 6520 6d61 7465 7269 616c  to make material
-00001da0: 0a20 2020 2020 2020 2020 2020 2020 6176  .             av
-00001db0: 6169 6c61 626c 6520 746f 2074 6865 2070  ailable to the p
-00001dc0: 7562 6c69 6320 696e 636c 7564 696e 6720  ublic including 
-00001dd0: 696e 2077 6179 7320 7468 6174 206d 656d  in ways that mem
-00001de0: 6265 7273 206f 6620 7468 650a 2020 2020  bers of the.    
-00001df0: 2020 2020 2020 2020 2070 7562 6c69 6320           public 
-00001e00: 6d61 7920 6163 6365 7373 2074 6865 206d  may access the m
-00001e10: 6174 6572 6961 6c20 6672 6f6d 2061 2070  aterial from a p
-00001e20: 6c61 6365 2061 6e64 2061 7420 6120 7469  lace and at a ti
-00001e30: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
-00001e40: 696e 6469 7669 6475 616c 6c79 2063 686f  individually cho
-00001e50: 7365 6e20 6279 2074 6865 6d2e 0a20 2020  sen by them..   
-00001e60: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001e70: 6a2e 2053 7569 2047 656e 6572 6973 2044  j. Sui Generis D
-00001e80: 6174 6162 6173 6520 5269 6768 7473 206d  atabase Rights m
-00001e90: 6561 6e73 2072 6967 6874 7320 6f74 6865  eans rights othe
-00001ea0: 7220 7468 616e 2063 6f70 7972 6967 6874  r than copyright
-00001eb0: 0a20 2020 2020 2020 2020 2020 2020 7265  .             re
-00001ec0: 7375 6c74 696e 6720 6672 6f6d 2044 6972  sulting from Dir
-00001ed0: 6563 7469 7665 2039 362f 392f 4543 206f  ective 96/9/EC o
-00001ee0: 6620 7468 6520 4575 726f 7065 616e 2050  f the European P
-00001ef0: 6172 6c69 616d 656e 7420 616e 6420 6f66  arliament and of
-00001f00: 0a20 2020 2020 2020 2020 2020 2020 7468  .             th
-00001f10: 6520 436f 756e 6369 6c20 6f66 2031 3120  e Council of 11 
-00001f20: 4d61 7263 6820 3139 3936 206f 6e20 7468  March 1996 on th
-00001f30: 6520 6c65 6761 6c20 7072 6f74 6563 7469  e legal protecti
-00001f40: 6f6e 206f 6620 6461 7461 6261 7365 732c  on of databases,
-00001f50: 0a20 2020 2020 2020 2020 2020 2020 6173  .             as
-00001f60: 2061 6d65 6e64 6564 2061 6e64 2f6f 7220   amended and/or 
-00001f70: 7375 6363 6565 6465 642c 2061 7320 7765  succeeded, as we
-00001f80: 6c6c 2061 7320 6f74 6865 7220 6573 7365  ll as other esse
-00001f90: 6e74 6961 6c6c 790a 2020 2020 2020 2020  ntially.        
-00001fa0: 2020 2020 2065 7175 6976 616c 656e 7420       equivalent 
-00001fb0: 7269 6768 7473 2061 6e79 7768 6572 6520  rights anywhere 
-00001fc0: 696e 2074 6865 2077 6f72 6c64 2e0a 2020  in the world..  
-00001fd0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001fe0: 206b 2e20 596f 7520 6d65 616e 7320 7468   k. You means th
-00001ff0: 6520 696e 6469 7669 6475 616c 206f 7220  e individual or 
-00002000: 656e 7469 7479 2065 7865 7263 6973 696e  entity exercisin
-00002010: 6720 7468 6520 4c69 6365 6e73 6564 2052  g the Licensed R
-00002020: 6967 6874 730a 2020 2020 2020 2020 2020  ights.          
-00002030: 2020 2075 6e64 6572 2074 6869 7320 5075     under this Pu
-00002040: 626c 6963 204c 6963 656e 7365 2e20 596f  blic License. Yo
-00002050: 7572 2068 6173 2061 2063 6f72 7265 7370  ur has a corresp
-00002060: 6f6e 6469 6e67 206d 6561 6e69 6e67 2e0a  onding meaning..
-00002070: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00002080: 200a 2020 2020 2020 2020 5365 6374 696f   .        Sectio
-00002090: 6e20 3220 2d2d 2053 636f 7065 2e0a 2020  n 2 -- Scope..  
-000020a0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-000020b0: 2061 2e20 4c69 6365 6e73 6520 6772 616e   a. License gran
-000020c0: 742e 0a20 2020 2020 2020 200a 2020 2020  t..        .    
-000020d0: 2020 2020 2020 2020 2020 2031 2e20 5375             1. Su
-000020e0: 626a 6563 7420 746f 2074 6865 2074 6572  bject to the ter
-000020f0: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
-00002100: 7320 6f66 2074 6869 7320 5075 626c 6963  s of this Public
-00002110: 204c 6963 656e 7365 2c0a 2020 2020 2020   License,.      
-00002120: 2020 2020 2020 2020 2020 2020 7468 6520              the 
-00002130: 4c69 6365 6e73 6f72 2068 6572 6562 7920  Licensor hereby 
-00002140: 6772 616e 7473 2059 6f75 2061 2077 6f72  grants You a wor
-00002150: 6c64 7769 6465 2c20 726f 7961 6c74 792d  ldwide, royalty-
-00002160: 6672 6565 2c0a 2020 2020 2020 2020 2020  free,.          
-00002170: 2020 2020 2020 2020 6e6f 6e2d 7375 626c          non-subl
-00002180: 6963 656e 7361 626c 652c 206e 6f6e 2d65  icensable, non-e
-00002190: 7863 6c75 7369 7665 2c20 6972 7265 766f  xclusive, irrevo
-000021a0: 6361 626c 6520 6c69 6365 6e73 6520 746f  cable license to
-000021b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021c0: 2020 2065 7865 7263 6973 6520 7468 6520     exercise the 
-000021d0: 4c69 6365 6e73 6564 2052 6967 6874 7320  Licensed Rights 
-000021e0: 696e 2074 6865 204c 6963 656e 7365 6420  in the Licensed 
-000021f0: 4d61 7465 7269 616c 2074 6f3a 0a20 2020  Material to:.   
-00002200: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00002210: 2020 2020 2020 2020 2020 612e 2072 6570            a. rep
-00002220: 726f 6475 6365 2061 6e64 2053 6861 7265  roduce and Share
-00002230: 2074 6865 204c 6963 656e 7365 6420 4d61   the Licensed Ma
-00002240: 7465 7269 616c 2c20 696e 2077 686f 6c65  terial, in whole
-00002250: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-00002260: 2020 2020 2020 2020 2020 2069 6e20 7061             in pa
-00002270: 7274 2c20 666f 7220 4e6f 6e43 6f6d 6d65  rt, for NonComme
-00002280: 7263 6961 6c20 7075 7270 6f73 6573 206f  rcial purposes o
-00002290: 6e6c 793b 2061 6e64 0a20 2020 2020 2020  nly; and.       
-000022a0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000022b0: 2020 2020 2020 622e 2070 726f 6475 6365        b. produce
-000022c0: 2061 6e64 2072 6570 726f 6475 6365 2c20   and reproduce, 
-000022d0: 6275 7420 6e6f 7420 5368 6172 652c 2041  but not Share, A
-000022e0: 6461 7074 6564 204d 6174 6572 6961 6c0a  dapted Material.
-000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002300: 2020 2020 2020 2066 6f72 204e 6f6e 436f         for NonCo
-00002310: 6d6d 6572 6369 616c 2070 7572 706f 7365  mmercial purpose
-00002320: 7320 6f6e 6c79 2e0a 2020 2020 2020 2020  s only..        
-00002330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002340: 322e 2045 7863 6570 7469 6f6e 7320 616e  2. Exceptions an
-00002350: 6420 4c69 6d69 7461 7469 6f6e 732e 2046  d Limitations. F
-00002360: 6f72 2074 6865 2061 766f 6964 616e 6365  or the avoidance
-00002370: 206f 6620 646f 7562 742c 2077 6865 7265   of doubt, where
-00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002390: 2020 2045 7863 6570 7469 6f6e 7320 616e     Exceptions an
-000023a0: 6420 4c69 6d69 7461 7469 6f6e 7320 6170  d Limitations ap
-000023b0: 706c 7920 746f 2059 6f75 7220 7573 652c  ply to Your use,
-000023c0: 2074 6869 7320 5075 626c 6963 0a20 2020   this Public.   
-000023d0: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-000023e0: 6963 656e 7365 2064 6f65 7320 6e6f 7420  icense does not 
-000023f0: 6170 706c 792c 2061 6e64 2059 6f75 2064  apply, and You d
-00002400: 6f20 6e6f 7420 6e65 6564 2074 6f20 636f  o not need to co
-00002410: 6d70 6c79 2077 6974 680a 2020 2020 2020  mply with.      
-00002420: 2020 2020 2020 2020 2020 2020 6974 7320              its 
-00002430: 7465 726d 7320 616e 6420 636f 6e64 6974  terms and condit
-00002440: 696f 6e73 2e0a 2020 2020 2020 2020 0a20  ions..        . 
-00002450: 2020 2020 2020 2020 2020 2020 2020 332e                3.
-00002460: 2054 6572 6d2e 2054 6865 2074 6572 6d20   Term. The term 
-00002470: 6f66 2074 6869 7320 5075 626c 6963 204c  of this Public L
-00002480: 6963 656e 7365 2069 7320 7370 6563 6966  icense is specif
-00002490: 6965 6420 696e 2053 6563 7469 6f6e 0a20  ied in Section. 
-000024a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024b0: 2036 2861 292e 0a20 2020 2020 2020 200a   6(a)..        .
-000024c0: 2020 2020 2020 2020 2020 2020 2020 2034                 4
-000024d0: 2e20 4d65 6469 6120 616e 6420 666f 726d  . Media and form
-000024e0: 6174 733b 2074 6563 686e 6963 616c 206d  ats; technical m
-000024f0: 6f64 6966 6963 6174 696f 6e73 2061 6c6c  odifications all
-00002500: 6f77 6564 2e20 5468 650a 2020 2020 2020  owed. The.      
-00002510: 2020 2020 2020 2020 2020 2020 4c69 6365              Lice
-00002520: 6e73 6f72 2061 7574 686f 7269 7a65 7320  nsor authorizes 
-00002530: 596f 7520 746f 2065 7865 7263 6973 6520  You to exercise 
-00002540: 7468 6520 4c69 6365 6e73 6564 2052 6967  the Licensed Rig
-00002550: 6874 7320 696e 0a20 2020 2020 2020 2020  hts in.         
-00002560: 2020 2020 2020 2020 2061 6c6c 206d 6564           all med
-00002570: 6961 2061 6e64 2066 6f72 6d61 7473 2077  ia and formats w
-00002580: 6865 7468 6572 206e 6f77 206b 6e6f 776e  hether now known
-00002590: 206f 7220 6865 7265 6166 7465 7220 6372   or hereafter cr
-000025a0: 6561 7465 642c 0a20 2020 2020 2020 2020  eated,.         
-000025b0: 2020 2020 2020 2020 2061 6e64 2074 6f20           and to 
-000025c0: 6d61 6b65 2074 6563 686e 6963 616c 206d  make technical m
-000025d0: 6f64 6966 6963 6174 696f 6e73 206e 6563  odifications nec
-000025e0: 6573 7361 7279 2074 6f20 646f 2073 6f2e  essary to do so.
-000025f0: 2054 6865 0a20 2020 2020 2020 2020 2020   The.           
-00002600: 2020 2020 2020 204c 6963 656e 736f 7220         Licensor 
-00002610: 7761 6976 6573 2061 6e64 2f6f 7220 6167  waives and/or ag
-00002620: 7265 6573 206e 6f74 2074 6f20 6173 7365  rees not to asse
-00002630: 7274 2061 6e79 2072 6967 6874 206f 720a  rt any right or.
-00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 2020 6175 7468 6f72 6974 7920 746f 2066    authority to f
-00002660: 6f72 6269 6420 596f 7520 6672 6f6d 206d  orbid You from m
-00002670: 616b 696e 6720 7465 6368 6e69 6361 6c20  aking technical 
-00002680: 6d6f 6469 6669 6361 7469 6f6e 730a 2020  modifications.  
-00002690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026a0: 6e65 6365 7373 6172 7920 746f 2065 7865  necessary to exe
-000026b0: 7263 6973 6520 7468 6520 4c69 6365 6e73  rcise the Licens
-000026c0: 6564 2052 6967 6874 732c 2069 6e63 6c75  ed Rights, inclu
-000026d0: 6469 6e67 0a20 2020 2020 2020 2020 2020  ding.           
-000026e0: 2020 2020 2020 2074 6563 686e 6963 616c         technical
-000026f0: 206d 6f64 6966 6963 6174 696f 6e73 206e   modifications n
-00002700: 6563 6573 7361 7279 2074 6f20 6369 7263  ecessary to circ
-00002710: 756d 7665 6e74 2045 6666 6563 7469 7665  umvent Effective
-00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002730: 2020 2054 6563 686e 6f6c 6f67 6963 616c     Technological
-00002740: 204d 6561 7375 7265 732e 2046 6f72 2070   Measures. For p
-00002750: 7572 706f 7365 7320 6f66 2074 6869 7320  urposes of this 
-00002760: 5075 626c 6963 204c 6963 656e 7365 2c0a  Public License,.
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 7369 6d70 6c79 206d 616b 696e 6720    simply making 
-00002790: 6d6f 6469 6669 6361 7469 6f6e 7320 6175  modifications au
-000027a0: 7468 6f72 697a 6564 2062 7920 7468 6973  thorized by this
-000027b0: 2053 6563 7469 6f6e 2032 2861 290a 2020   Section 2(a).  
-000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027d0: 2834 2920 6e65 7665 7220 7072 6f64 7563  (4) never produc
-000027e0: 6573 2041 6461 7074 6564 204d 6174 6572  es Adapted Mater
-000027f0: 6961 6c2e 0a20 2020 2020 2020 200a 2020  ial..        .  
-00002800: 2020 2020 2020 2020 2020 2020 2035 2e20               5. 
-00002810: 446f 776e 7374 7265 616d 2072 6563 6970  Downstream recip
-00002820: 6965 6e74 732e 0a20 2020 2020 2020 200a  ients..        .
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 612e 204f 6666 6572 2066 726f      a. Offer fro
-00002850: 6d20 7468 6520 4c69 6365 6e73 6f72 202d  m the Licensor -
-00002860: 2d20 4c69 6365 6e73 6564 204d 6174 6572  - Licensed Mater
-00002870: 6961 6c2e 2045 7665 7279 0a20 2020 2020  ial. Every.     
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 7265 6369 7069 656e 7420 6f66 2074    recipient of t
-000028a0: 6865 204c 6963 656e 7365 6420 4d61 7465  he Licensed Mate
-000028b0: 7269 616c 2061 7574 6f6d 6174 6963 616c  rial automatical
-000028c0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-000028d0: 2020 2020 2020 2020 2020 7265 6365 6976            receiv
-000028e0: 6573 2061 6e20 6f66 6665 7220 6672 6f6d  es an offer from
-000028f0: 2074 6865 204c 6963 656e 736f 7220 746f   the Licensor to
-00002900: 2065 7865 7263 6973 6520 7468 650a 2020   exercise the.  
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 2020 204c 6963 656e 7365 6420 5269       Licensed Ri
-00002930: 6768 7473 2075 6e64 6572 2074 6865 2074  ghts under the t
-00002940: 6572 6d73 2061 6e64 2063 6f6e 6469 7469  erms and conditi
-00002950: 6f6e 7320 6f66 2074 6869 730a 2020 2020  ons of this.    
-00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002970: 2020 2050 7562 6c69 6320 4c69 6365 6e73     Public Licens
-00002980: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 622e 204e 6f20 646f 776e 7374 7265 616d  b. No downstream
-000029b0: 2072 6573 7472 6963 7469 6f6e 732e 2059   restrictions. Y
-000029c0: 6f75 206d 6179 206e 6f74 206f 6666 6572  ou may not offer
-000029d0: 206f 7220 696d 706f 7365 0a20 2020 2020   or impose.     
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 616e 7920 6164 6469 7469 6f6e 616c    any additional
-00002a00: 206f 7220 6469 6666 6572 656e 7420 7465   or different te
-00002a10: 726d 7320 6f72 2063 6f6e 6469 7469 6f6e  rms or condition
-00002a20: 7320 6f6e 2c20 6f72 0a20 2020 2020 2020  s on, or.       
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 6170 706c 7920 616e 7920 4566 6665 6374  apply any Effect
-00002a50: 6976 6520 5465 6368 6e6f 6c6f 6769 6361  ive Technologica
-00002a60: 6c20 4d65 6173 7572 6573 2074 6f2c 2074  l Measures to, t
-00002a70: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
-00002a80: 2020 2020 2020 2020 2020 4c69 6365 6e73            Licens
-00002a90: 6564 204d 6174 6572 6961 6c20 6966 2064  ed Material if d
-00002aa0: 6f69 6e67 2073 6f20 7265 7374 7269 6374  oing so restrict
-00002ab0: 7320 6578 6572 6369 7365 206f 6620 7468  s exercise of th
-00002ac0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00002ad0: 2020 2020 2020 2020 204c 6963 656e 7365           License
-00002ae0: 6420 5269 6768 7473 2062 7920 616e 7920  d Rights by any 
-00002af0: 7265 6369 7069 656e 7420 6f66 2074 6865  recipient of the
-00002b00: 204c 6963 656e 7365 640a 2020 2020 2020   Licensed.      
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 204d 6174 6572 6961 6c2e 0a20 2020 2020   Material..     
-00002b30: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00002b40: 2020 2036 2e20 4e6f 2065 6e64 6f72 7365     6. No endorse
-00002b50: 6d65 6e74 2e20 4e6f 7468 696e 6720 696e  ment. Nothing in
-00002b60: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
-00002b70: 656e 7365 2063 6f6e 7374 6974 7574 6573  ense constitutes
-00002b80: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-00002b90: 2020 2020 2020 6d61 7920 6265 2063 6f6e        may be con
-00002ba0: 7374 7275 6564 2061 7320 7065 726d 6973  strued as permis
-00002bb0: 7369 6f6e 2074 6f20 6173 7365 7274 206f  sion to assert o
-00002bc0: 7220 696d 706c 7920 7468 6174 2059 6f75  r imply that You
-00002bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002be0: 2020 2061 7265 2c20 6f72 2074 6861 7420     are, or that 
-00002bf0: 596f 7572 2075 7365 206f 6620 7468 6520  Your use of the 
-00002c00: 4c69 6365 6e73 6564 204d 6174 6572 6961  Licensed Materia
-00002c10: 6c20 6973 2c20 636f 6e6e 6563 7465 640a  l is, connected.
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 7769 7468 2c20 6f72 2073 706f 6e73    with, or spons
-00002c40: 6f72 6564 2c20 656e 646f 7273 6564 2c20  ored, endorsed, 
-00002c50: 6f72 2067 7261 6e74 6564 206f 6666 6963  or granted offic
-00002c60: 6961 6c20 7374 6174 7573 2062 792c 0a20  ial status by,. 
-00002c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c80: 2074 6865 204c 6963 656e 736f 7220 6f72   the Licensor or
-00002c90: 206f 7468 6572 7320 6465 7369 676e 6174   others designat
-00002ca0: 6564 2074 6f20 7265 6365 6976 6520 6174  ed to receive at
-00002cb0: 7472 6962 7574 696f 6e20 6173 0a20 2020  tribution as.   
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002cd0: 726f 7669 6465 6420 696e 2053 6563 7469  rovided in Secti
-00002ce0: 6f6e 2033 2861 2928 3129 2841 2928 6929  on 3(a)(1)(A)(i)
-00002cf0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00002d00: 2020 2020 2062 2e20 4f74 6865 7220 7269       b. Other ri
-00002d10: 6768 7473 2e0a 2020 2020 2020 2020 0a20  ghts..        . 
-00002d20: 2020 2020 2020 2020 2020 2020 2020 312e                1.
-00002d30: 204d 6f72 616c 2072 6967 6874 732c 2073   Moral rights, s
-00002d40: 7563 6820 6173 2074 6865 2072 6967 6874  uch as the right
-00002d50: 206f 6620 696e 7465 6772 6974 792c 2061   of integrity, a
-00002d60: 7265 206e 6f74 0a20 2020 2020 2020 2020  re not.         
-00002d70: 2020 2020 2020 2020 206c 6963 656e 7365           license
-00002d80: 6420 756e 6465 7220 7468 6973 2050 7562  d under this Pub
-00002d90: 6c69 6320 4c69 6365 6e73 652c 206e 6f72  lic License, nor
-00002da0: 2061 7265 2070 7562 6c69 6369 7479 2c0a   are publicity,.
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 7072 6976 6163 792c 2061 6e64 2f6f    privacy, and/o
-00002dd0: 7220 6f74 6865 7220 7369 6d69 6c61 7220  r other similar 
-00002de0: 7065 7273 6f6e 616c 6974 7920 7269 6768  personality righ
-00002df0: 7473 3b20 686f 7765 7665 722c 2074 6f0a  ts; however, to.
-00002e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e10: 2020 7468 6520 6578 7465 6e74 2070 6f73    the extent pos
-00002e20: 7369 626c 652c 2074 6865 204c 6963 656e  sible, the Licen
-00002e30: 736f 7220 7761 6976 6573 2061 6e64 2f6f  sor waives and/o
-00002e40: 7220 6167 7265 6573 206e 6f74 2074 6f0a  r agrees not to.
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 6173 7365 7274 2061 6e79 2073 7563    assert any suc
-00002e70: 6820 7269 6768 7473 2068 656c 6420 6279  h rights held by
-00002e80: 2074 6865 204c 6963 656e 736f 7220 746f   the Licensor to
-00002e90: 2074 6865 206c 696d 6974 6564 0a20 2020   the limited.   
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00002eb0: 7874 656e 7420 6e65 6365 7373 6172 7920  xtent necessary 
-00002ec0: 746f 2061 6c6c 6f77 2059 6f75 2074 6f20  to allow You to 
-00002ed0: 6578 6572 6369 7365 2074 6865 204c 6963  exercise the Lic
-00002ee0: 656e 7365 640a 2020 2020 2020 2020 2020  ensed.          
-00002ef0: 2020 2020 2020 2020 5269 6768 7473 2c20          Rights, 
-00002f00: 6275 7420 6e6f 7420 6f74 6865 7277 6973  but not otherwis
-00002f10: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
-00002f20: 2020 2020 2020 2020 2020 2032 2e20 5061             2. Pa
-00002f30: 7465 6e74 2061 6e64 2074 7261 6465 6d61  tent and tradema
-00002f40: 726b 2072 6967 6874 7320 6172 6520 6e6f  rk rights are no
-00002f50: 7420 6c69 6365 6e73 6564 2075 6e64 6572  t licensed under
-00002f60: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
-00002f70: 2020 2020 2020 2020 5075 626c 6963 204c          Public L
-00002f80: 6963 656e 7365 2e0a 2020 2020 2020 2020  icense..        
-00002f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002fa0: 332e 2054 6f20 7468 6520 6578 7465 6e74  3. To the extent
-00002fb0: 2070 6f73 7369 626c 652c 2074 6865 204c   possible, the L
-00002fc0: 6963 656e 736f 7220 7761 6976 6573 2061  icensor waives a
-00002fd0: 6e79 2072 6967 6874 2074 6f0a 2020 2020  ny right to.    
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002ff0: 6c6c 6563 7420 726f 7961 6c74 6965 7320  llect royalties 
-00003000: 6672 6f6d 2059 6f75 2066 6f72 2074 6865  from You for the
-00003010: 2065 7865 7263 6973 6520 6f66 2074 6865   exercise of the
-00003020: 204c 6963 656e 7365 640a 2020 2020 2020   Licensed.      
-00003030: 2020 2020 2020 2020 2020 2020 5269 6768              Righ
-00003040: 7473 2c20 7768 6574 6865 7220 6469 7265  ts, whether dire
-00003050: 6374 6c79 206f 7220 7468 726f 7567 6820  ctly or through 
-00003060: 6120 636f 6c6c 6563 7469 6e67 2073 6f63  a collecting soc
-00003070: 6965 7479 0a20 2020 2020 2020 2020 2020  iety.           
-00003080: 2020 2020 2020 2075 6e64 6572 2061 6e79         under any
-00003090: 2076 6f6c 756e 7461 7279 206f 7220 7761   voluntary or wa
-000030a0: 6976 6162 6c65 2073 7461 7475 746f 7279  ivable statutory
-000030b0: 206f 7220 636f 6d70 756c 736f 7279 0a20   or compulsory. 
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 206c 6963 656e 7369 6e67 2073 6368 656d   licensing schem
-000030e0: 652e 2049 6e20 616c 6c20 6f74 6865 7220  e. In all other 
-000030f0: 6361 7365 7320 7468 6520 4c69 6365 6e73  cases the Licens
-00003100: 6f72 2065 7870 7265 7373 6c79 0a20 2020  or expressly.   
-00003110: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003120: 6573 6572 7665 7320 616e 7920 7269 6768  eserves any righ
-00003130: 7420 746f 2063 6f6c 6c65 6374 2073 7563  t to collect suc
-00003140: 6820 726f 7961 6c74 6965 732c 2069 6e63  h royalties, inc
-00003150: 6c75 6469 6e67 2077 6865 6e0a 2020 2020  luding when.    
-00003160: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00003170: 6520 4c69 6365 6e73 6564 204d 6174 6572  e Licensed Mater
-00003180: 6961 6c20 6973 2075 7365 6420 6f74 6865  ial is used othe
-00003190: 7220 7468 616e 2066 6f72 204e 6f6e 436f  r than for NonCo
-000031a0: 6d6d 6572 6369 616c 0a20 2020 2020 2020  mmercial.       
-000031b0: 2020 2020 2020 2020 2020 2070 7572 706f             purpo
-000031c0: 7365 732e 0a20 2020 2020 2020 200a 2020  ses..        .  
-000031d0: 2020 2020 2020 0a20 2020 2020 2020 2053        .        S
-000031e0: 6563 7469 6f6e 2033 202d 2d20 4c69 6365  ection 3 -- Lice
-000031f0: 6e73 6520 436f 6e64 6974 696f 6e73 2e0a  nse Conditions..
-00003200: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003210: 2059 6f75 7220 6578 6572 6369 7365 206f   Your exercise o
-00003220: 6620 7468 6520 4c69 6365 6e73 6564 2052  f the Licensed R
-00003230: 6967 6874 7320 6973 2065 7870 7265 7373  ights is express
-00003240: 6c79 206d 6164 6520 7375 626a 6563 7420  ly made subject 
-00003250: 746f 2074 6865 0a20 2020 2020 2020 2066  to the.        f
-00003260: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
-00003270: 6f6e 732e 0a20 2020 2020 2020 200a 2020  ons..        .  
-00003280: 2020 2020 2020 2020 612e 2041 7474 7269          a. Attri
-00003290: 6275 7469 6f6e 2e0a 2020 2020 2020 2020  bution..        
-000032a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032b0: 312e 2049 6620 596f 7520 5368 6172 6520  1. If You Share 
-000032c0: 7468 6520 4c69 6365 6e73 6564 204d 6174  the Licensed Mat
-000032d0: 6572 6961 6c2c 2059 6f75 206d 7573 743a  erial, You must:
-000032e0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000032f0: 2020 2020 2020 2020 2020 2020 2020 612e                a.
-00003300: 2072 6574 6169 6e20 7468 6520 666f 6c6c   retain the foll
-00003310: 6f77 696e 6720 6966 2069 7420 6973 2073  owing if it is s
-00003320: 7570 706c 6965 6420 6279 2074 6865 204c  upplied by the L
-00003330: 6963 656e 736f 720a 2020 2020 2020 2020  icensor.        
-00003340: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00003350: 6974 6820 7468 6520 4c69 6365 6e73 6564  ith the Licensed
-00003360: 204d 6174 6572 6961 6c3a 0a20 2020 2020   Material:.     
-00003370: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00003380: 2020 2020 2020 2020 2020 2020 2069 2e20               i. 
-00003390: 6964 656e 7469 6669 6361 7469 6f6e 206f  identification o
-000033a0: 6620 7468 6520 6372 6561 746f 7228 7329  f the creator(s)
-000033b0: 206f 6620 7468 6520 4c69 6365 6e73 6564   of the Licensed
-000033c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033d0: 2020 2020 2020 2020 2020 2020 204d 6174               Mat
-000033e0: 6572 6961 6c20 616e 6420 616e 7920 6f74  erial and any ot
-000033f0: 6865 7273 2064 6573 6967 6e61 7465 6420  hers designated 
-00003400: 746f 2072 6563 6569 7665 0a20 2020 2020  to receive.     
-00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 2020 2020 2020 2061 7474 7269 6275 7469         attributi
-00003430: 6f6e 2c20 696e 2061 6e79 2072 6561 736f  on, in any reaso
-00003440: 6e61 626c 6520 6d61 6e6e 6572 2072 6571  nable manner req
-00003450: 7565 7374 6564 2062 790a 2020 2020 2020  uested by.      
-00003460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003470: 2020 2020 2020 7468 6520 4c69 6365 6e73        the Licens
-00003480: 6f72 2028 696e 636c 7564 696e 6720 6279  or (including by
-00003490: 2070 7365 7564 6f6e 796d 2069 660a 2020   pseudonym if.  
-000034a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034b0: 2020 2020 2020 2020 2020 6465 7369 676e            design
-000034c0: 6174 6564 293b 0a20 2020 2020 2020 200a  ated);.        .
-000034d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034e0: 2020 2020 2020 2020 6969 2e20 6120 636f          ii. a co
-000034f0: 7079 7269 6768 7420 6e6f 7469 6365 3b0a  pyright notice;.
-00003500: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 6969 692e 2061 206e 6f74 6963 6520 7468  iii. a notice th
-00003530: 6174 2072 6566 6572 7320 746f 2074 6869  at refers to thi
-00003540: 7320 5075 626c 6963 204c 6963 656e 7365  s Public License
-00003550: 3b0a 2020 2020 2020 2020 0a20 2020 2020  ;.        .     
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2069 762e 2061 206e 6f74 6963 6520     iv. a notice 
-00003580: 7468 6174 2072 6566 6572 7320 746f 2074  that refers to t
-00003590: 6865 2064 6973 636c 6169 6d65 7220 6f66  he disclaimer of
-000035a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035b0: 2020 2020 2020 2020 2020 2020 2077 6172               war
-000035c0: 7261 6e74 6965 733b 0a20 2020 2020 2020  ranties;.       
-000035d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-000035e0: 2020 2020 2020 2020 2020 2076 2e20 6120             v. a 
-000035f0: 5552 4920 6f72 2068 7970 6572 6c69 6e6b  URI or hyperlink
-00003600: 2074 6f20 7468 6520 4c69 6365 6e73 6564   to the Licensed
-00003610: 204d 6174 6572 6961 6c20 746f 2074 6865   Material to the
-00003620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003630: 2020 2020 2020 2020 2020 2020 2065 7874               ext
-00003640: 656e 7420 7265 6173 6f6e 6162 6c79 2070  ent reasonably p
-00003650: 7261 6374 6963 6162 6c65 3b0a 2020 2020  racticable;.    
-00003660: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00003670: 2020 2020 2020 2020 2062 2e20 696e 6469           b. indi
-00003680: 6361 7465 2069 6620 596f 7520 6d6f 6469  cate if You modi
-00003690: 6669 6564 2074 6865 204c 6963 656e 7365  fied the License
-000036a0: 6420 4d61 7465 7269 616c 2061 6e64 0a20  d Material and. 
-000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036c0: 2020 2020 2020 7265 7461 696e 2061 6e20        retain an 
-000036d0: 696e 6469 6361 7469 6f6e 206f 6620 616e  indication of an
-000036e0: 7920 7072 6576 696f 7573 206d 6f64 6966  y previous modif
-000036f0: 6963 6174 696f 6e73 3b20 616e 640a 2020  ications; and.  
-00003700: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00003710: 2020 2020 2020 2020 2020 2063 2e20 696e             c. in
-00003720: 6469 6361 7465 2074 6865 204c 6963 656e  dicate the Licen
-00003730: 7365 6420 4d61 7465 7269 616c 2069 7320  sed Material is 
-00003740: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
-00003750: 6869 730a 2020 2020 2020 2020 2020 2020  his.            
-00003760: 2020 2020 2020 2020 2020 2050 7562 6c69             Publi
-00003770: 6320 4c69 6365 6e73 652c 2061 6e64 2069  c License, and i
-00003780: 6e63 6c75 6465 2074 6865 2074 6578 7420  nclude the text 
-00003790: 6f66 2c20 6f72 2074 6865 2055 5249 206f  of, or the URI o
-000037a0: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-000037b0: 2020 2020 2020 2020 2068 7970 6572 6c69           hyperli
-000037c0: 6e6b 2074 6f2c 2074 6869 7320 5075 626c  nk to, this Publ
-000037d0: 6963 204c 6963 656e 7365 2e0a 2020 2020  ic License..    
-000037e0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-000037f0: 2020 2020 2020 2046 6f72 2074 6865 2061         For the a
-00003800: 766f 6964 616e 6365 206f 6620 646f 7562  voidance of doub
-00003810: 742c 2059 6f75 2064 6f20 6e6f 7420 6861  t, You do not ha
-00003820: 7665 2070 6572 6d69 7373 696f 6e20 756e  ve permission un
-00003830: 6465 720a 2020 2020 2020 2020 2020 2020  der.            
-00003840: 2020 2020 2020 7468 6973 2050 7562 6c69        this Publi
-00003850: 6320 4c69 6365 6e73 6520 746f 2053 6861  c License to Sha
-00003860: 7265 2041 6461 7074 6564 204d 6174 6572  re Adapted Mater
-00003870: 6961 6c2e 0a20 2020 2020 2020 200a 2020  ial..        .  
-00003880: 2020 2020 2020 2020 2020 2020 2032 2e20               2. 
-00003890: 596f 7520 6d61 7920 7361 7469 7366 7920  You may satisfy 
-000038a0: 7468 6520 636f 6e64 6974 696f 6e73 2069  the conditions i
-000038b0: 6e20 5365 6374 696f 6e20 3328 6129 2831  n Section 3(a)(1
-000038c0: 2920 696e 2061 6e79 0a20 2020 2020 2020  ) in any.       
-000038d0: 2020 2020 2020 2020 2020 2072 6561 736f             reaso
-000038e0: 6e61 626c 6520 6d61 6e6e 6572 2062 6173  nable manner bas
-000038f0: 6564 206f 6e20 7468 6520 6d65 6469 756d  ed on the medium
-00003900: 2c20 6d65 616e 732c 2061 6e64 2063 6f6e  , means, and con
-00003910: 7465 7874 2069 6e0a 2020 2020 2020 2020  text in.        
-00003920: 2020 2020 2020 2020 2020 7768 6963 6820            which 
-00003930: 596f 7520 5368 6172 6520 7468 6520 4c69  You Share the Li
-00003940: 6365 6e73 6564 204d 6174 6572 6961 6c2e  censed Material.
-00003950: 2046 6f72 2065 7861 6d70 6c65 2c20 6974   For example, it
-00003960: 206d 6179 2062 650a 2020 2020 2020 2020   may be.        
-00003970: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-00003980: 6162 6c65 2074 6f20 7361 7469 7366 7920  able to satisfy 
-00003990: 7468 6520 636f 6e64 6974 696f 6e73 2062  the conditions b
-000039a0: 7920 7072 6f76 6964 696e 6720 6120 5552  y providing a UR
-000039b0: 4920 6f72 0a20 2020 2020 2020 2020 2020  I or.           
-000039c0: 2020 2020 2020 2068 7970 6572 6c69 6e6b         hyperlink
-000039d0: 2074 6f20 6120 7265 736f 7572 6365 2074   to a resource t
-000039e0: 6861 7420 696e 636c 7564 6573 2074 6865  hat includes the
-000039f0: 2072 6571 7569 7265 640a 2020 2020 2020   required.      
-00003a00: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00003a10: 726d 6174 696f 6e2e 0a20 2020 2020 2020  rmation..       
-00003a20: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00003a30: 2033 2e20 4966 2072 6571 7565 7374 6564   3. If requested
-00003a40: 2062 7920 7468 6520 4c69 6365 6e73 6f72   by the Licensor
-00003a50: 2c20 596f 7520 6d75 7374 2072 656d 6f76  , You must remov
-00003a60: 6520 616e 7920 6f66 2074 6865 0a20 2020  e any of the.   
-00003a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003a80: 6e66 6f72 6d61 7469 6f6e 2072 6571 7569  nformation requi
-00003a90: 7265 6420 6279 2053 6563 7469 6f6e 2033  red by Section 3
-00003aa0: 2861 2928 3129 2841 2920 746f 2074 6865  (a)(1)(A) to the
-00003ab0: 2065 7874 656e 740a 2020 2020 2020 2020   extent.        
-00003ac0: 2020 2020 2020 2020 2020 7265 6173 6f6e            reason
-00003ad0: 6162 6c79 2070 7261 6374 6963 6162 6c65  ably practicable
-00003ae0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00003af0: 2020 200a 2020 2020 2020 2020 5365 6374     .        Sect
-00003b00: 696f 6e20 3420 2d2d 2053 7569 2047 656e  ion 4 -- Sui Gen
-00003b10: 6572 6973 2044 6174 6162 6173 6520 5269  eris Database Ri
-00003b20: 6768 7473 2e0a 2020 2020 2020 2020 0a20  ghts..        . 
-00003b30: 2020 2020 2020 2057 6865 7265 2074 6865         Where the
-00003b40: 204c 6963 656e 7365 6420 5269 6768 7473   Licensed Rights
-00003b50: 2069 6e63 6c75 6465 2053 7569 2047 656e   include Sui Gen
-00003b60: 6572 6973 2044 6174 6162 6173 6520 5269  eris Database Ri
-00003b70: 6768 7473 2074 6861 740a 2020 2020 2020  ghts that.      
-00003b80: 2020 6170 706c 7920 746f 2059 6f75 7220    apply to Your 
-00003b90: 7573 6520 6f66 2074 6865 204c 6963 656e  use of the Licen
-00003ba0: 7365 6420 4d61 7465 7269 616c 3a0a 2020  sed Material:.  
-00003bb0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00003bc0: 2061 2e20 666f 7220 7468 6520 6176 6f69   a. for the avoi
-00003bd0: 6461 6e63 6520 6f66 2064 6f75 6274 2c20  dance of doubt, 
-00003be0: 5365 6374 696f 6e20 3228 6129 2831 2920  Section 2(a)(1) 
-00003bf0: 6772 616e 7473 2059 6f75 2074 6865 2072  grants You the r
-00003c00: 6967 6874 0a20 2020 2020 2020 2020 2020  ight.           
-00003c10: 2020 746f 2065 7874 7261 6374 2c20 7265    to extract, re
-00003c20: 7573 652c 2072 6570 726f 6475 6365 2c20  use, reproduce, 
-00003c30: 616e 6420 5368 6172 6520 616c 6c20 6f72  and Share all or
-00003c40: 2061 2073 7562 7374 616e 7469 616c 0a20   a substantial. 
-00003c50: 2020 2020 2020 2020 2020 2020 706f 7274              port
-00003c60: 696f 6e20 6f66 2074 6865 2063 6f6e 7465  ion of the conte
-00003c70: 6e74 7320 6f66 2074 6865 2064 6174 6162  nts of the datab
-00003c80: 6173 6520 666f 7220 4e6f 6e43 6f6d 6d65  ase for NonComme
-00003c90: 7263 6961 6c20 7075 7270 6f73 6573 0a20  rcial purposes. 
-00003ca0: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
-00003cb0: 2061 6e64 2070 726f 7669 6465 6420 596f   and provided Yo
-00003cc0: 7520 646f 206e 6f74 2053 6861 7265 2041  u do not Share A
-00003cd0: 6461 7074 6564 204d 6174 6572 6961 6c3b  dapted Material;
-00003ce0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003cf0: 2020 2020 622e 2069 6620 596f 7520 696e      b. if You in
-00003d00: 636c 7564 6520 616c 6c20 6f72 2061 2073  clude all or a s
-00003d10: 7562 7374 616e 7469 616c 2070 6f72 7469  ubstantial porti
-00003d20: 6f6e 206f 6620 7468 6520 6461 7461 6261  on of the databa
-00003d30: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
-00003d40: 636f 6e74 656e 7473 2069 6e20 6120 6461  contents in a da
-00003d50: 7461 6261 7365 2069 6e20 7768 6963 6820  tabase in which 
-00003d60: 596f 7520 6861 7665 2053 7569 2047 656e  You have Sui Gen
-00003d70: 6572 6973 2044 6174 6162 6173 650a 2020  eris Database.  
-00003d80: 2020 2020 2020 2020 2020 2052 6967 6874             Right
-00003d90: 732c 2074 6865 6e20 7468 6520 6461 7461  s, then the data
-00003da0: 6261 7365 2069 6e20 7768 6963 6820 596f  base in which Yo
-00003db0: 7520 6861 7665 2053 7569 2047 656e 6572  u have Sui Gener
-00003dc0: 6973 2044 6174 6162 6173 650a 2020 2020  is Database.    
-00003dd0: 2020 2020 2020 2020 2052 6967 6874 7320           Rights 
-00003de0: 2862 7574 206e 6f74 2069 7473 2069 6e64  (but not its ind
-00003df0: 6976 6964 7561 6c20 636f 6e74 656e 7473  ividual contents
-00003e00: 2920 6973 2041 6461 7074 6564 204d 6174  ) is Adapted Mat
-00003e10: 6572 6961 6c3b 2061 6e64 0a20 2020 2020  erial; and.     
-00003e20: 2020 200a 2020 2020 2020 2020 2020 632e     .          c.
-00003e30: 2059 6f75 206d 7573 7420 636f 6d70 6c79   You must comply
-00003e40: 2077 6974 6820 7468 6520 636f 6e64 6974   with the condit
-00003e50: 696f 6e73 2069 6e20 5365 6374 696f 6e20  ions in Section 
-00003e60: 3328 6129 2069 6620 596f 7520 5368 6172  3(a) if You Shar
-00003e70: 650a 2020 2020 2020 2020 2020 2020 2061  e.             a
-00003e80: 6c6c 206f 7220 6120 7375 6273 7461 6e74  ll or a substant
-00003e90: 6961 6c20 706f 7274 696f 6e20 6f66 2074  ial portion of t
-00003ea0: 6865 2063 6f6e 7465 6e74 7320 6f66 2074  he contents of t
-00003eb0: 6865 2064 6174 6162 6173 652e 0a20 2020  he database..   
-00003ec0: 2020 2020 200a 2020 2020 2020 2020 466f       .        Fo
-00003ed0: 7220 7468 6520 6176 6f69 6461 6e63 6520  r the avoidance 
-00003ee0: 6f66 2064 6f75 6274 2c20 7468 6973 2053  of doubt, this S
-00003ef0: 6563 7469 6f6e 2034 2073 7570 706c 656d  ection 4 supplem
-00003f00: 656e 7473 2061 6e64 2064 6f65 7320 6e6f  ents and does no
-00003f10: 740a 2020 2020 2020 2020 7265 706c 6163  t.        replac
-00003f20: 6520 596f 7572 206f 626c 6967 6174 696f  e Your obligatio
-00003f30: 6e73 2075 6e64 6572 2074 6869 7320 5075  ns under this Pu
-00003f40: 626c 6963 204c 6963 656e 7365 2077 6865  blic License whe
-00003f50: 7265 2074 6865 204c 6963 656e 7365 640a  re the Licensed.
-00003f60: 2020 2020 2020 2020 5269 6768 7473 2069          Rights i
-00003f70: 6e63 6c75 6465 206f 7468 6572 2043 6f70  nclude other Cop
-00003f80: 7972 6967 6874 2061 6e64 2053 696d 696c  yright and Simil
-00003f90: 6172 2052 6967 6874 732e 0a20 2020 2020  ar Rights..     
-00003fa0: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
-00003fb0: 2020 2020 2053 6563 7469 6f6e 2035 202d       Section 5 -
-00003fc0: 2d20 4469 7363 6c61 696d 6572 206f 6620  - Disclaimer of 
-00003fd0: 5761 7272 616e 7469 6573 2061 6e64 204c  Warranties and L
-00003fe0: 696d 6974 6174 696f 6e20 6f66 204c 6961  imitation of Lia
-00003ff0: 6269 6c69 7479 2e0a 2020 2020 2020 2020  bility..        
-00004000: 0a20 2020 2020 2020 2020 2061 2e20 554e  .          a. UN
-00004010: 4c45 5353 204f 5448 4552 5749 5345 2053  LESS OTHERWISE S
-00004020: 4550 4152 4154 454c 5920 554e 4445 5254  EPARATELY UNDERT
-00004030: 414b 454e 2042 5920 5448 4520 4c49 4345  AKEN BY THE LICE
-00004040: 4e53 4f52 2c20 544f 2054 4845 0a20 2020  NSOR, TO THE.   
-00004050: 2020 2020 2020 2020 2020 4558 5445 4e54            EXTENT
-00004060: 2050 4f53 5349 424c 452c 2054 4845 204c   POSSIBLE, THE L
-00004070: 4943 454e 534f 5220 4f46 4645 5253 2054  ICENSOR OFFERS T
-00004080: 4845 204c 4943 454e 5345 4420 4d41 5445  HE LICENSED MATE
-00004090: 5249 414c 2041 532d 4953 0a20 2020 2020  RIAL AS-IS.     
-000040a0: 2020 2020 2020 2020 414e 4420 4153 2d41          AND AS-A
-000040b0: 5641 494c 4142 4c45 2c20 414e 4420 4d41  VAILABLE, AND MA
-000040c0: 4b45 5320 4e4f 2052 4550 5245 5345 4e54  KES NO REPRESENT
-000040d0: 4154 494f 4e53 204f 5220 5741 5252 414e  ATIONS OR WARRAN
-000040e0: 5449 4553 204f 460a 2020 2020 2020 2020  TIES OF.        
-000040f0: 2020 2020 2041 4e59 204b 494e 4420 434f       ANY KIND CO
-00004100: 4e43 4552 4e49 4e47 2054 4845 204c 4943  NCERNING THE LIC
-00004110: 454e 5345 4420 4d41 5445 5249 414c 2c20  ENSED MATERIAL, 
-00004120: 5748 4554 4845 5220 4558 5052 4553 532c  WHETHER EXPRESS,
-00004130: 0a20 2020 2020 2020 2020 2020 2020 494d  .             IM
-00004140: 504c 4945 442c 2053 5441 5455 544f 5259  PLIED, STATUTORY
-00004150: 2c20 4f52 204f 5448 4552 2e20 5448 4953  , OR OTHER. THIS
-00004160: 2049 4e43 4c55 4445 532c 2057 4954 484f   INCLUDES, WITHO
-00004170: 5554 204c 494d 4954 4154 494f 4e2c 0a20  UT LIMITATION,. 
-00004180: 2020 2020 2020 2020 2020 2020 5741 5252              WARR
-00004190: 414e 5449 4553 204f 4620 5449 544c 452c  ANTIES OF TITLE,
-000041a0: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
-000041b0: 2c20 4649 544e 4553 5320 464f 5220 4120  , FITNESS FOR A 
-000041c0: 5041 5254 4943 554c 4152 0a20 2020 2020  PARTICULAR.     
-000041d0: 2020 2020 2020 2020 5055 5250 4f53 452c          PURPOSE,
-000041e0: 204e 4f4e 2d49 4e46 5249 4e47 454d 454e   NON-INFRINGEMEN
-000041f0: 542c 2041 4253 454e 4345 204f 4620 4c41  T, ABSENCE OF LA
-00004200: 5445 4e54 204f 5220 4f54 4845 5220 4445  TENT OR OTHER DE
-00004210: 4645 4354 532c 0a20 2020 2020 2020 2020  FECTS,.         
-00004220: 2020 2020 4143 4355 5241 4359 2c20 4f52      ACCURACY, OR
-00004230: 2054 4845 2050 5245 5345 4e43 4520 4f52   THE PRESENCE OR
-00004240: 2041 4253 454e 4345 204f 4620 4552 524f   ABSENCE OF ERRO
-00004250: 5253 2c20 5748 4554 4845 5220 4f52 204e  RS, WHETHER OR N
-00004260: 4f54 0a20 2020 2020 2020 2020 2020 2020  OT.             
-00004270: 4b4e 4f57 4e20 4f52 2044 4953 434f 5645  KNOWN OR DISCOVE
-00004280: 5241 424c 452e 2057 4845 5245 2044 4953  RABLE. WHERE DIS
-00004290: 434c 4149 4d45 5253 204f 4620 5741 5252  CLAIMERS OF WARR
-000042a0: 414e 5449 4553 2041 5245 204e 4f54 0a20  ANTIES ARE NOT. 
-000042b0: 2020 2020 2020 2020 2020 2020 414c 4c4f              ALLO
-000042c0: 5745 4420 494e 2046 554c 4c20 4f52 2049  WED IN FULL OR I
-000042d0: 4e20 5041 5254 2c20 5448 4953 2044 4953  N PART, THIS DIS
-000042e0: 434c 4149 4d45 5220 4d41 5920 4e4f 5420  CLAIMER MAY NOT 
-000042f0: 4150 504c 5920 544f 2059 4f55 2e0a 2020  APPLY TO YOU..  
-00004300: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00004310: 2062 2e20 544f 2054 4845 2045 5854 454e   b. TO THE EXTEN
-00004320: 5420 504f 5353 4942 4c45 2c20 494e 204e  T POSSIBLE, IN N
-00004330: 4f20 4556 454e 5420 5749 4c4c 2054 4845  O EVENT WILL THE
-00004340: 204c 4943 454e 534f 5220 4245 204c 4941   LICENSOR BE LIA
-00004350: 424c 450a 2020 2020 2020 2020 2020 2020  BLE.            
-00004360: 2054 4f20 594f 5520 4f4e 2041 4e59 204c   TO YOU ON ANY L
-00004370: 4547 414c 2054 4845 4f52 5920 2849 4e43  EGAL THEORY (INC
-00004380: 4c55 4449 4e47 2c20 5749 5448 4f55 5420  LUDING, WITHOUT 
-00004390: 4c49 4d49 5441 5449 4f4e 2c0a 2020 2020  LIMITATION,.    
-000043a0: 2020 2020 2020 2020 204e 4547 4c49 4745           NEGLIGE
-000043b0: 4e43 4529 204f 5220 4f54 4845 5257 4953  NCE) OR OTHERWIS
-000043c0: 4520 464f 5220 414e 5920 4449 5245 4354  E FOR ANY DIRECT
-000043d0: 2c20 5350 4543 4941 4c2c 2049 4e44 4952  , SPECIAL, INDIR
-000043e0: 4543 542c 0a20 2020 2020 2020 2020 2020  ECT,.           
-000043f0: 2020 494e 4349 4445 4e54 414c 2c20 434f    INCIDENTAL, CO
-00004400: 4e53 4551 5545 4e54 4941 4c2c 2050 554e  NSEQUENTIAL, PUN
-00004410: 4954 4956 452c 2045 5845 4d50 4c41 5259  ITIVE, EXEMPLARY
-00004420: 2c20 4f52 204f 5448 4552 204c 4f53 5345  , OR OTHER LOSSE
-00004430: 532c 0a20 2020 2020 2020 2020 2020 2020  S,.             
-00004440: 434f 5354 532c 2045 5850 454e 5345 532c  COSTS, EXPENSES,
-00004450: 204f 5220 4441 4d41 4745 5320 4152 4953   OR DAMAGES ARIS
-00004460: 494e 4720 4f55 5420 4f46 2054 4849 5320  ING OUT OF THIS 
-00004470: 5055 424c 4943 204c 4943 454e 5345 204f  PUBLIC LICENSE O
-00004480: 520a 2020 2020 2020 2020 2020 2020 2055  R.             U
-00004490: 5345 204f 4620 5448 4520 4c49 4345 4e53  SE OF THE LICENS
-000044a0: 4544 204d 4154 4552 4941 4c2c 2045 5645  ED MATERIAL, EVE
-000044b0: 4e20 4946 2054 4845 204c 4943 454e 534f  N IF THE LICENSO
-000044c0: 5220 4841 5320 4245 454e 0a20 2020 2020  R HAS BEEN.     
-000044d0: 2020 2020 2020 2020 4144 5649 5345 4420          ADVISED 
-000044e0: 4f46 2054 4845 2050 4f53 5349 4249 4c49  OF THE POSSIBILI
-000044f0: 5459 204f 4620 5355 4348 204c 4f53 5345  TY OF SUCH LOSSE
-00004500: 532c 2043 4f53 5453 2c20 4558 5045 4e53  S, COSTS, EXPENS
-00004510: 4553 2c20 4f52 0a20 2020 2020 2020 2020  ES, OR.         
-00004520: 2020 2020 4441 4d41 4745 532e 2057 4845      DAMAGES. WHE
-00004530: 5245 2041 204c 494d 4954 4154 494f 4e20  RE A LIMITATION 
-00004540: 4f46 204c 4941 4249 4c49 5459 2049 5320  OF LIABILITY IS 
-00004550: 4e4f 5420 414c 4c4f 5745 4420 494e 2046  NOT ALLOWED IN F
-00004560: 554c 4c20 4f52 0a20 2020 2020 2020 2020  ULL OR.         
-00004570: 2020 2020 494e 2050 4152 542c 2054 4849      IN PART, THI
-00004580: 5320 4c49 4d49 5441 5449 4f4e 204d 4159  S LIMITATION MAY
-00004590: 204e 4f54 2041 5050 4c59 2054 4f20 594f   NOT APPLY TO YO
-000045a0: 552e 0a20 2020 2020 2020 200a 2020 2020  U..        .    
-000045b0: 2020 2020 2020 632e 2054 6865 2064 6973        c. The dis
-000045c0: 636c 6169 6d65 7220 6f66 2077 6172 7261  claimer of warra
-000045d0: 6e74 6965 7320 616e 6420 6c69 6d69 7461  nties and limita
-000045e0: 7469 6f6e 206f 6620 6c69 6162 696c 6974  tion of liabilit
-000045f0: 7920 7072 6f76 6964 6564 0a20 2020 2020  y provided.     
-00004600: 2020 2020 2020 2020 6162 6f76 6520 7368          above sh
-00004610: 616c 6c20 6265 2069 6e74 6572 7072 6574  all be interpret
-00004620: 6564 2069 6e20 6120 6d61 6e6e 6572 2074  ed in a manner t
-00004630: 6861 742c 2074 6f20 7468 6520 6578 7465  hat, to the exte
-00004640: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
-00004650: 706f 7373 6962 6c65 2c20 6d6f 7374 2063  possible, most c
-00004660: 6c6f 7365 6c79 2061 7070 726f 7869 6d61  losely approxima
-00004670: 7465 7320 616e 2061 6273 6f6c 7574 6520  tes an absolute 
-00004680: 6469 7363 6c61 696d 6572 2061 6e64 0a20  disclaimer and. 
-00004690: 2020 2020 2020 2020 2020 2020 7761 6976              waiv
-000046a0: 6572 206f 6620 616c 6c20 6c69 6162 696c  er of all liabil
-000046b0: 6974 792e 0a20 2020 2020 2020 200a 2020  ity..        .  
-000046c0: 2020 2020 2020 0a20 2020 2020 2020 2053        .        S
-000046d0: 6563 7469 6f6e 2036 202d 2d20 5465 726d  ection 6 -- Term
-000046e0: 2061 6e64 2054 6572 6d69 6e61 7469 6f6e   and Termination
-000046f0: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00004700: 2020 2020 2061 2e20 5468 6973 2050 7562       a. This Pub
-00004710: 6c69 6320 4c69 6365 6e73 6520 6170 706c  lic License appl
-00004720: 6965 7320 666f 7220 7468 6520 7465 726d  ies for the term
-00004730: 206f 6620 7468 6520 436f 7079 7269 6768   of the Copyrigh
-00004740: 7420 616e 640a 2020 2020 2020 2020 2020  t and.          
-00004750: 2020 2053 696d 696c 6172 2052 6967 6874     Similar Right
-00004760: 7320 6c69 6365 6e73 6564 2068 6572 652e  s licensed here.
-00004770: 2048 6f77 6576 6572 2c20 6966 2059 6f75   However, if You
-00004780: 2066 6169 6c20 746f 2063 6f6d 706c 7920   fail to comply 
-00004790: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
-000047a0: 2020 7468 6973 2050 7562 6c69 6320 4c69    this Public Li
-000047b0: 6365 6e73 652c 2074 6865 6e20 596f 7572  cense, then Your
-000047c0: 2072 6967 6874 7320 756e 6465 7220 7468   rights under th
-000047d0: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
-000047e0: 650a 2020 2020 2020 2020 2020 2020 2074  e.             t
-000047f0: 6572 6d69 6e61 7465 2061 7574 6f6d 6174  erminate automat
-00004800: 6963 616c 6c79 2e0a 2020 2020 2020 2020  ically..        
-00004810: 0a20 2020 2020 2020 2020 2062 2e20 5768  .          b. Wh
-00004820: 6572 6520 596f 7572 2072 6967 6874 2074  ere Your right t
-00004830: 6f20 7573 6520 7468 6520 4c69 6365 6e73  o use the Licens
-00004840: 6564 204d 6174 6572 6961 6c20 6861 7320  ed Material has 
-00004850: 7465 726d 696e 6174 6564 2075 6e64 6572  terminated under
-00004860: 0a20 2020 2020 2020 2020 2020 2020 5365  .             Se
-00004870: 6374 696f 6e20 3628 6129 2c20 6974 2072  ction 6(a), it r
-00004880: 6569 6e73 7461 7465 733a 0a20 2020 2020  einstates:.     
-00004890: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-000048a0: 2020 2031 2e20 6175 746f 6d61 7469 6361     1. automatica
-000048b0: 6c6c 7920 6173 206f 6620 7468 6520 6461  lly as of the da
-000048c0: 7465 2074 6865 2076 696f 6c61 7469 6f6e  te the violation
-000048d0: 2069 7320 6375 7265 642c 2070 726f 7669   is cured, provi
-000048e0: 6465 640a 2020 2020 2020 2020 2020 2020  ded.            
-000048f0: 2020 2020 2020 6974 2069 7320 6375 7265        it is cure
-00004900: 6420 7769 7468 696e 2033 3020 6461 7973  d within 30 days
-00004910: 206f 6620 596f 7572 2064 6973 636f 7665   of Your discove
-00004920: 7279 206f 6620 7468 650a 2020 2020 2020  ry of the.      
-00004930: 2020 2020 2020 2020 2020 2020 7669 6f6c              viol
-00004940: 6174 696f 6e3b 206f 720a 2020 2020 2020  ation; or.      
-00004950: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-00004960: 2020 322e 2075 706f 6e20 6578 7072 6573    2. upon expres
-00004970: 7320 7265 696e 7374 6174 656d 656e 7420  s reinstatement 
-00004980: 6279 2074 6865 204c 6963 656e 736f 722e  by the Licensor.
-00004990: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000049a0: 2020 2020 2020 2046 6f72 2074 6865 2061         For the a
-000049b0: 766f 6964 616e 6365 206f 6620 646f 7562  voidance of doub
-000049c0: 742c 2074 6869 7320 5365 6374 696f 6e20  t, this Section 
-000049d0: 3628 6229 2064 6f65 7320 6e6f 7420 6166  6(b) does not af
-000049e0: 6665 6374 2061 6e79 0a20 2020 2020 2020  fect any.       
-000049f0: 2020 2020 2020 7269 6768 7420 7468 6520        right the 
-00004a00: 4c69 6365 6e73 6f72 206d 6179 2068 6176  Licensor may hav
-00004a10: 6520 746f 2073 6565 6b20 7265 6d65 6469  e to seek remedi
-00004a20: 6573 2066 6f72 2059 6f75 7220 7669 6f6c  es for Your viol
-00004a30: 6174 696f 6e73 0a20 2020 2020 2020 2020  ations.         
-00004a40: 2020 2020 6f66 2074 6869 7320 5075 626c      of this Publ
-00004a50: 6963 204c 6963 656e 7365 2e0a 2020 2020  ic License..    
-00004a60: 2020 2020 0a20 2020 2020 2020 2020 2063      .          c
-00004a70: 2e20 466f 7220 7468 6520 6176 6f69 6461  . For the avoida
-00004a80: 6e63 6520 6f66 2064 6f75 6274 2c20 7468  nce of doubt, th
-00004a90: 6520 4c69 6365 6e73 6f72 206d 6179 2061  e Licensor may a
-00004aa0: 6c73 6f20 6f66 6665 7220 7468 650a 2020  lso offer the.  
-00004ab0: 2020 2020 2020 2020 2020 204c 6963 656e             Licen
-00004ac0: 7365 6420 4d61 7465 7269 616c 2075 6e64  sed Material und
-00004ad0: 6572 2073 6570 6172 6174 6520 7465 726d  er separate term
-00004ae0: 7320 6f72 2063 6f6e 6469 7469 6f6e 7320  s or conditions 
-00004af0: 6f72 2073 746f 700a 2020 2020 2020 2020  or stop.        
-00004b00: 2020 2020 2064 6973 7472 6962 7574 696e       distributin
-00004b10: 6720 7468 6520 4c69 6365 6e73 6564 204d  g the Licensed M
-00004b20: 6174 6572 6961 6c20 6174 2061 6e79 2074  aterial at any t
-00004b30: 696d 653b 2068 6f77 6576 6572 2c20 646f  ime; however, do
-00004b40: 696e 6720 736f 0a20 2020 2020 2020 2020  ing so.         
-00004b50: 2020 2020 7769 6c6c 206e 6f74 2074 6572      will not ter
-00004b60: 6d69 6e61 7465 2074 6869 7320 5075 626c  minate this Publ
-00004b70: 6963 204c 6963 656e 7365 2e0a 2020 2020  ic License..    
-00004b80: 2020 2020 0a20 2020 2020 2020 2020 2064      .          d
-00004b90: 2e20 5365 6374 696f 6e73 2031 2c20 352c  . Sections 1, 5,
-00004ba0: 2036 2c20 372c 2061 6e64 2038 2073 7572   6, 7, and 8 sur
-00004bb0: 7669 7665 2074 6572 6d69 6e61 7469 6f6e  vive termination
-00004bc0: 206f 6620 7468 6973 2050 7562 6c69 630a   of this Public.
-00004bd0: 2020 2020 2020 2020 2020 2020 204c 6963               Lic
-00004be0: 656e 7365 2e0a 2020 2020 2020 2020 0a20  ense..        . 
-00004bf0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004c00: 5365 6374 696f 6e20 3720 2d2d 204f 7468  Section 7 -- Oth
-00004c10: 6572 2054 6572 6d73 2061 6e64 2043 6f6e  er Terms and Con
-00004c20: 6469 7469 6f6e 732e 0a20 2020 2020 2020  ditions..       
-00004c30: 200a 2020 2020 2020 2020 2020 612e 2054   .          a. T
-00004c40: 6865 204c 6963 656e 736f 7220 7368 616c  he Licensor shal
-00004c50: 6c20 6e6f 7420 6265 2062 6f75 6e64 2062  l not be bound b
-00004c60: 7920 616e 7920 6164 6469 7469 6f6e 616c  y any additional
-00004c70: 206f 7220 6469 6666 6572 656e 740a 2020   or different.  
-00004c80: 2020 2020 2020 2020 2020 2074 6572 6d73             terms
-00004c90: 206f 7220 636f 6e64 6974 696f 6e73 2063   or conditions c
-00004ca0: 6f6d 6d75 6e69 6361 7465 6420 6279 2059  ommunicated by Y
-00004cb0: 6f75 2075 6e6c 6573 7320 6578 7072 6573  ou unless expres
-00004cc0: 736c 7920 6167 7265 6564 2e0a 2020 2020  sly agreed..    
-00004cd0: 2020 2020 0a20 2020 2020 2020 2020 2062      .          b
-00004ce0: 2e20 416e 7920 6172 7261 6e67 656d 656e  . Any arrangemen
-00004cf0: 7473 2c20 756e 6465 7273 7461 6e64 696e  ts, understandin
-00004d00: 6773 2c20 6f72 2061 6772 6565 6d65 6e74  gs, or agreement
-00004d10: 7320 7265 6761 7264 696e 6720 7468 650a  s regarding the.
-00004d20: 2020 2020 2020 2020 2020 2020 204c 6963               Lic
-00004d30: 656e 7365 6420 4d61 7465 7269 616c 206e  ensed Material n
-00004d40: 6f74 2073 7461 7465 6420 6865 7265 696e  ot stated herein
-00004d50: 2061 7265 2073 6570 6172 6174 6520 6672   are separate fr
-00004d60: 6f6d 2061 6e64 0a20 2020 2020 2020 2020  om and.         
-00004d70: 2020 2020 696e 6465 7065 6e64 656e 7420      independent 
-00004d80: 6f66 2074 6865 2074 6572 6d73 2061 6e64  of the terms and
-00004d90: 2063 6f6e 6469 7469 6f6e 7320 6f66 2074   conditions of t
-00004da0: 6869 7320 5075 626c 6963 204c 6963 656e  his Public Licen
-00004db0: 7365 2e0a 2020 2020 2020 2020 0a20 2020  se..        .   
-00004dc0: 2020 2020 200a 2020 2020 2020 2020 5365       .        Se
-00004dd0: 6374 696f 6e20 3820 2d2d 2049 6e74 6572  ction 8 -- Inter
-00004de0: 7072 6574 6174 696f 6e2e 0a20 2020 2020  pretation..     
-00004df0: 2020 200a 2020 2020 2020 2020 2020 612e     .          a.
-00004e00: 2046 6f72 2074 6865 2061 766f 6964 616e   For the avoidan
-00004e10: 6365 206f 6620 646f 7562 742c 2074 6869  ce of doubt, thi
-00004e20: 7320 5075 626c 6963 204c 6963 656e 7365  s Public License
-00004e30: 2064 6f65 7320 6e6f 742c 2061 6e64 0a20   does not, and. 
-00004e40: 2020 2020 2020 2020 2020 2020 7368 616c              shal
-00004e50: 6c20 6e6f 7420 6265 2069 6e74 6572 7072  l not be interpr
-00004e60: 6574 6564 2074 6f2c 2072 6564 7563 652c  eted to, reduce,
-00004e70: 206c 696d 6974 2c20 7265 7374 7269 6374   limit, restrict
-00004e80: 2c20 6f72 2069 6d70 6f73 650a 2020 2020  , or impose.    
-00004e90: 2020 2020 2020 2020 2063 6f6e 6469 7469           conditi
-00004ea0: 6f6e 7320 6f6e 2061 6e79 2075 7365 206f  ons on any use o
-00004eb0: 6620 7468 6520 4c69 6365 6e73 6564 204d  f the Licensed M
-00004ec0: 6174 6572 6961 6c20 7468 6174 2063 6f75  aterial that cou
-00004ed0: 6c64 206c 6177 6675 6c6c 790a 2020 2020  ld lawfully.    
-00004ee0: 2020 2020 2020 2020 2062 6520 6d61 6465           be made
-00004ef0: 2077 6974 686f 7574 2070 6572 6d69 7373   without permiss
-00004f00: 696f 6e20 756e 6465 7220 7468 6973 2050  ion under this P
-00004f10: 7562 6c69 6320 4c69 6365 6e73 652e 0a20  ublic License.. 
-00004f20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00004f30: 2020 622e 2054 6f20 7468 6520 6578 7465    b. To the exte
-00004f40: 6e74 2070 6f73 7369 626c 652c 2069 6620  nt possible, if 
-00004f50: 616e 7920 7072 6f76 6973 696f 6e20 6f66  any provision of
-00004f60: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
-00004f70: 656e 7365 2069 730a 2020 2020 2020 2020  ense is.        
-00004f80: 2020 2020 2064 6565 6d65 6420 756e 656e       deemed unen
-00004f90: 666f 7263 6561 626c 652c 2069 7420 7368  forceable, it sh
-00004fa0: 616c 6c20 6265 2061 7574 6f6d 6174 6963  all be automatic
-00004fb0: 616c 6c79 2072 6566 6f72 6d65 6420 746f  ally reformed to
-00004fc0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-00004fd0: 2020 6d69 6e69 6d75 6d20 6578 7465 6e74    minimum extent
-00004fe0: 206e 6563 6573 7361 7279 2074 6f20 6d61   necessary to ma
-00004ff0: 6b65 2069 7420 656e 666f 7263 6561 626c  ke it enforceabl
-00005000: 652e 2049 6620 7468 6520 7072 6f76 6973  e. If the provis
-00005010: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00005020: 2063 616e 6e6f 7420 6265 2072 6566 6f72   cannot be refor
-00005030: 6d65 642c 2069 7420 7368 616c 6c20 6265  med, it shall be
-00005040: 2073 6576 6572 6564 2066 726f 6d20 7468   severed from th
-00005050: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
-00005060: 650a 2020 2020 2020 2020 2020 2020 2077  e.             w
-00005070: 6974 686f 7574 2061 6666 6563 7469 6e67  ithout affecting
-00005080: 2074 6865 2065 6e66 6f72 6365 6162 696c   the enforceabil
-00005090: 6974 7920 6f66 2074 6865 2072 656d 6169  ity of the remai
-000050a0: 6e69 6e67 2074 6572 6d73 2061 6e64 0a20  ning terms and. 
-000050b0: 2020 2020 2020 2020 2020 2020 636f 6e64              cond
-000050c0: 6974 696f 6e73 2e0a 2020 2020 2020 2020  itions..        
-000050d0: 0a20 2020 2020 2020 2020 2063 2e20 4e6f  .          c. No
-000050e0: 2074 6572 6d20 6f72 2063 6f6e 6469 7469   term or conditi
-000050f0: 6f6e 206f 6620 7468 6973 2050 7562 6c69  on of this Publi
-00005100: 6320 4c69 6365 6e73 6520 7769 6c6c 2062  c License will b
-00005110: 6520 7761 6976 6564 2061 6e64 206e 6f0a  e waived and no.
-00005120: 2020 2020 2020 2020 2020 2020 2066 6169               fai
-00005130: 6c75 7265 2074 6f20 636f 6d70 6c79 2063  lure to comply c
-00005140: 6f6e 7365 6e74 6564 2074 6f20 756e 6c65  onsented to unle
-00005150: 7373 2065 7870 7265 7373 6c79 2061 6772  ss expressly agr
-00005160: 6565 6420 746f 2062 7920 7468 650a 2020  eed to by the.  
-00005170: 2020 2020 2020 2020 2020 204c 6963 656e             Licen
-00005180: 736f 722e 0a20 2020 2020 2020 200a 2020  sor..        .  
-00005190: 2020 2020 2020 2020 642e 204e 6f74 6869          d. Nothi
-000051a0: 6e67 2069 6e20 7468 6973 2050 7562 6c69  ng in this Publi
-000051b0: 6320 4c69 6365 6e73 6520 636f 6e73 7469  c License consti
-000051c0: 7475 7465 7320 6f72 206d 6179 2062 6520  tutes or may be 
-000051d0: 696e 7465 7270 7265 7465 640a 2020 2020  interpreted.    
-000051e0: 2020 2020 2020 2020 2061 7320 6120 6c69           as a li
-000051f0: 6d69 7461 7469 6f6e 2075 706f 6e2c 206f  mitation upon, o
-00005200: 7220 7761 6976 6572 206f 662c 2061 6e79  r waiver of, any
-00005210: 2070 7269 7669 6c65 6765 7320 616e 6420   privileges and 
-00005220: 696d 6d75 6e69 7469 6573 0a20 2020 2020  immunities.     
-00005230: 2020 2020 2020 2020 7468 6174 2061 7070          that app
-00005240: 6c79 2074 6f20 7468 6520 4c69 6365 6e73  ly to the Licens
-00005250: 6f72 206f 7220 596f 752c 2069 6e63 6c75  or or You, inclu
-00005260: 6469 6e67 2066 726f 6d20 7468 6520 6c65  ding from the le
-00005270: 6761 6c0a 2020 2020 2020 2020 2020 2020  gal.            
-00005280: 2070 726f 6365 7373 6573 206f 6620 616e   processes of an
-00005290: 7920 6a75 7269 7364 6963 7469 6f6e 206f  y jurisdiction o
-000052a0: 7220 6175 7468 6f72 6974 792e 0a20 2020  r authority..   
-000052b0: 2020 2020 200a 2020 2020 2020 2020 3d3d       .        ==
-000052c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000052d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000052e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000052f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005300: 3d3d 3d3d 3d0a 2020 2020 2020 2020 0a20  =====.        . 
-00005310: 2020 2020 2020 2043 7265 6174 6976 6520         Creative 
-00005320: 436f 6d6d 6f6e 7320 6973 206e 6f74 2061  Commons is not a
-00005330: 2070 6172 7479 2074 6f20 6974 7320 7075   party to its pu
-00005340: 626c 6963 0a20 2020 2020 2020 206c 6963  blic.        lic
-00005350: 656e 7365 732e 204e 6f74 7769 7468 7374  enses. Notwithst
-00005360: 616e 6469 6e67 2c20 4372 6561 7469 7665  anding, Creative
-00005370: 2043 6f6d 6d6f 6e73 206d 6179 2065 6c65   Commons may ele
-00005380: 6374 2074 6f20 6170 706c 7920 6f6e 6520  ct to apply one 
-00005390: 6f66 0a20 2020 2020 2020 2069 7473 2070  of.        its p
-000053a0: 7562 6c69 6320 6c69 6365 6e73 6573 2074  ublic licenses t
-000053b0: 6f20 6d61 7465 7269 616c 2069 7420 7075  o material it pu
-000053c0: 626c 6973 6865 7320 616e 6420 696e 2074  blishes and in t
-000053d0: 686f 7365 2069 6e73 7461 6e63 6573 0a20  hose instances. 
-000053e0: 2020 2020 2020 2077 696c 6c20 6265 2063         will be c
-000053f0: 6f6e 7369 6465 7265 6420 7468 6520 e280  onsidered the ..
-00005400: 9c4c 6963 656e 736f 722e e280 9d20 5468  .Licensor.... Th
-00005410: 6520 7465 7874 206f 6620 7468 6520 4372  e text of the Cr
-00005420: 6561 7469 7665 2043 6f6d 6d6f 6e73 0a20  eative Commons. 
-00005430: 2020 2020 2020 2070 7562 6c69 6320 6c69         public li
-00005440: 6365 6e73 6573 2069 7320 6465 6469 6361  censes is dedica
-00005450: 7465 6420 746f 2074 6865 2070 7562 6c69  ted to the publi
-00005460: 6320 646f 6d61 696e 2075 6e64 6572 2074  c domain under t
-00005470: 6865 2043 4330 2050 7562 6c69 630a 2020  he CC0 Public.  
-00005480: 2020 2020 2020 446f 6d61 696e 2044 6564        Domain Ded
-00005490: 6963 6174 696f 6e2e 2045 7863 6570 7420  ication. Except 
-000054a0: 666f 7220 7468 6520 6c69 6d69 7465 6420  for the limited 
-000054b0: 7075 7270 6f73 6520 6f66 2069 6e64 6963  purpose of indic
-000054c0: 6174 696e 6720 7468 6174 0a20 2020 2020  ating that.     
-000054d0: 2020 206d 6174 6572 6961 6c20 6973 2073     material is s
-000054e0: 6861 7265 6420 756e 6465 7220 6120 4372  hared under a Cr
-000054f0: 6561 7469 7665 2043 6f6d 6d6f 6e73 2070  eative Commons p
-00005500: 7562 6c69 6320 6c69 6365 6e73 6520 6f72  ublic license or
-00005510: 2061 730a 2020 2020 2020 2020 6f74 6865   as.        othe
-00005520: 7277 6973 6520 7065 726d 6974 7465 6420  rwise permitted 
-00005530: 6279 2074 6865 2043 7265 6174 6976 6520  by the Creative 
-00005540: 436f 6d6d 6f6e 7320 706f 6c69 6369 6573  Commons policies
-00005550: 2070 7562 6c69 7368 6564 2061 740a 2020   published at.  
-00005560: 2020 2020 2020 6372 6561 7469 7665 636f        creativeco
-00005570: 6d6d 6f6e 732e 6f72 672f 706f 6c69 6369  mmons.org/polici
-00005580: 6573 2c20 4372 6561 7469 7665 2043 6f6d  es, Creative Com
-00005590: 6d6f 6e73 2064 6f65 7320 6e6f 7420 6175  mons does not au
-000055a0: 7468 6f72 697a 6520 7468 650a 2020 2020  thorize the.    
-000055b0: 2020 2020 7573 6520 6f66 2074 6865 2074      use of the t
-000055c0: 7261 6465 6d61 726b 2022 4372 6561 7469  rademark "Creati
-000055d0: 7665 2043 6f6d 6d6f 6e73 2220 6f72 2061  ve Commons" or a
-000055e0: 6e79 206f 7468 6572 2074 7261 6465 6d61  ny other tradema
-000055f0: 726b 206f 7220 6c6f 676f 0a20 2020 2020  rk or logo.     
-00005600: 2020 206f 6620 4372 6561 7469 7665 2043     of Creative C
-00005610: 6f6d 6d6f 6e73 2077 6974 686f 7574 2069  ommons without i
-00005620: 7473 2070 7269 6f72 2077 7269 7474 656e  ts prior written
-00005630: 2063 6f6e 7365 6e74 2069 6e63 6c75 6469   consent includi
-00005640: 6e67 2c0a 2020 2020 2020 2020 7769 7468  ng,.        with
-00005650: 6f75 7420 6c69 6d69 7461 7469 6f6e 2c20  out limitation, 
-00005660: 696e 2063 6f6e 6e65 6374 696f 6e20 7769  in connection wi
-00005670: 7468 2061 6e79 2075 6e61 7574 686f 7269  th any unauthori
-00005680: 7a65 6420 6d6f 6469 6669 6361 7469 6f6e  zed modification
-00005690: 730a 2020 2020 2020 2020 746f 2061 6e79  s.        to any
-000056a0: 206f 6620 6974 7320 7075 626c 6963 206c   of its public l
-000056b0: 6963 656e 7365 7320 6f72 2061 6e79 206f  icenses or any o
-000056c0: 7468 6572 2061 7272 616e 6765 6d65 6e74  ther arrangement
-000056d0: 732c 0a20 2020 2020 2020 2075 6e64 6572  s,.        under
-000056e0: 7374 616e 6469 6e67 732c 206f 7220 6167  standings, or ag
-000056f0: 7265 656d 656e 7473 2063 6f6e 6365 726e  reements concern
-00005700: 696e 6720 7573 6520 6f66 206c 6963 656e  ing use of licen
-00005710: 7365 6420 6d61 7465 7269 616c 2e20 466f  sed material. Fo
-00005720: 720a 2020 2020 2020 2020 7468 6520 6176  r.        the av
-00005730: 6f69 6461 6e63 6520 6f66 2064 6f75 6274  oidance of doubt
-00005740: 2c20 7468 6973 2070 6172 6167 7261 7068  , this paragraph
-00005750: 2064 6f65 7320 6e6f 7420 666f 726d 2070   does not form p
-00005760: 6172 7420 6f66 2074 6865 0a20 2020 2020  art of the.     
-00005770: 2020 2070 7562 6c69 6320 6c69 6365 6e73     public licens
-00005780: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00005790: 2020 2020 2043 7265 6174 6976 6520 436f       Creative Co
-000057a0: 6d6d 6f6e 7320 6d61 7920 6265 2063 6f6e  mmons may be con
-000057b0: 7461 6374 6564 2061 7420 6372 6561 7469  tacted at creati
-000057c0: 7665 636f 6d6d 6f6e 732e 6f72 672e 0a20  vecommons.org.. 
-000057d0: 2020 2020 2020 200a 5072 6f6a 6563 742d         .Project-
-000057e0: 5552 4c3a 2048 6f6d 6570 6167 652c 2068  URL: Homepage, h
-000057f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00005800: 6d2f 6174 7461 636b 3638 2f72 6174 6573  m/attack68/rates
-00005810: 6c69 620a 4b65 7977 6f72 6473 3a20 696e  lib.Keywords: in
-00005820: 7465 7265 7374 2072 6174 652c 6465 7269  terest rate,deri
-00005830: 7661 7469 7665 732c 7377 6170 732c 626f  vatives,swaps,bo
-00005840: 6e64 732c 6669 7865 6420 696e 636f 6d65  nds,fixed income
-00005850: 0a52 6571 7569 7265 732d 5079 7468 6f6e  .Requires-Python
-00005860: 3a20 3e3d 332e 390a 4465 7363 7269 7074  : >=3.9.Descript
-00005870: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00005880: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00005890: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
-000058a0: 4345 4e53 450a 5265 7175 6972 6573 2d44  CENSE.Requires-D
-000058b0: 6973 743a 206e 756d 7079 3e3d 312e 3231  ist: numpy>=1.21
-000058c0: 2e35 0a52 6571 7569 7265 732d 4469 7374  .5.Requires-Dist
-000058d0: 3a20 6d61 7470 6c6f 746c 6962 3e3d 332e  : matplotlib>=3.
-000058e0: 352e 310a 5265 7175 6972 6573 2d44 6973  5.1.Requires-Dis
-000058f0: 743a 2070 616e 6461 733e 3d31 2e34 2e31  t: pandas>=1.4.1
-00005900: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
-00005910: 2064 6576 0a52 6571 7569 7265 732d 4469   dev.Requires-Di
-00005920: 7374 3a20 7079 7465 7374 3e3d 372e 302e  st: pytest>=7.0.
-00005930: 313b 2065 7874 7261 203d 3d20 2264 6576  1; extra == "dev
-00005940: 220a 5265 7175 6972 6573 2d44 6973 743a  ".Requires-Dist:
-00005950: 206a 7570 7974 6572 6c61 623e 3d33 2e33   jupyterlab>=3.3
-00005960: 2e31 3b20 6578 7472 6120 3d3d 2022 6465  .1; extra == "de
-00005970: 7622 0a52 6571 7569 7265 732d 4469 7374  v".Requires-Dist
-00005980: 3a20 7370 6869 6e78 3e3d 352e 312e 313b  : sphinx>=5.1.1;
-00005990: 2065 7874 7261 203d 3d20 2264 6576 220a   extra == "dev".
-000059a0: 5265 7175 6972 6573 2d44 6973 743a 2063  Requires-Dist: c
-000059b0: 6f76 6572 6167 653e 3d37 2e31 2e30 3b20  overage>=7.1.0; 
-000059c0: 6578 7472 6120 3d3d 2022 6465 7622 0a0a  extra == "dev"..
-000059d0: 3c64 6976 2073 7479 6c65 3d22 7465 7874  <div style="text
-000059e0: 2d61 6c69 676e 3a20 6365 6e74 6572 3b20  -align: center; 
-000059f0: 7061 6464 696e 673a 2032 656d 2030 2032  padding: 2em 0 2
-00005a00: 656d 223e 0a20 2020 203c 696d 6720 7372  em">.    <img sr
-00005a10: 633d 2268 7474 7073 3a2f 2f72 6174 6573  c="https://rates
-00005a20: 6c69 622e 7265 6164 7468 6564 6f63 732e  lib.readthedocs.
-00005a30: 696f 2f65 6e2f 6c61 7465 7374 2f5f 7374  io/en/latest/_st
-00005a40: 6174 6963 2f72 6174 6573 6c69 625f 6c6f  atic/rateslib_lo
-00005a50: 676f 5f62 6967 322e 706e 6722 2061 6c74  go_big2.png" alt
-00005a60: 3d22 7261 7465 736c 6962 223e 0a3c 2f64  ="rateslib">.</d
-00005a70: 6976 3e0a 0a3c 6469 7620 7374 796c 653d  iv>..<div style=
-00005a80: 2274 6578 742d 616c 6967 6e3a 2063 656e  "text-align: cen
-00005a90: 7465 7222 3e0a 2020 3c69 6d67 2073 7263  ter">.  <img src
-00005aa0: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
-00005ab0: 6965 6c64 732e 696f 2f62 6164 6765 2f64  ields.io/badge/d
-00005ac0: 796e 616d 6963 2f6a 736f 6e3f 7572 6c3d  ynamic/json?url=
-00005ad0: 6874 7470 7325 3341 2532 4625 3246 7261  https%3A%2F%2Fra
-00005ae0: 7465 736c 6962 2e72 6561 6474 6865 646f  teslib.readthedo
-00005af0: 6373 2e69 6f25 3246 656e 2532 466c 6174  cs.io%2Fen%2Flat
-00005b00: 6573 7425 3246 5f73 7461 7469 6325 3246  est%2F_static%2F
-00005b10: 6261 6467 6573 2e6a 736f 6e26 7175 6572  badges.json&quer
-00005b20: 793d 2532 342e 7079 7468 6f6e 266c 6162  y=%24.python&lab
-00005b30: 656c 3d50 7974 686f 6e26 636f 6c6f 723d  el=Python&color=
-00005b40: 626c 7565 2220 616c 743d 2250 7974 686f  blue" alt="Pytho
-00005b50: 6e22 3e0a 2020 3c69 6d67 2073 7263 3d22  n">.  <img src="
-00005b60: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00005b70: 6c64 732e 696f 2f62 6164 6765 2f64 796e  lds.io/badge/dyn
-00005b80: 616d 6963 2f6a 736f 6e3f 7572 6c3d 6874  amic/json?url=ht
-00005b90: 7470 7325 3341 2532 4625 3246 7261 7465  tps%3A%2F%2Frate
-00005ba0: 736c 6962 2e72 6561 6474 6865 646f 6373  slib.readthedocs
-00005bb0: 2e69 6f25 3246 656e 2532 466c 6174 6573  .io%2Fen%2Flates
-00005bc0: 7425 3246 5f73 7461 7469 6325 3246 6261  t%2F_static%2Fba
-00005bd0: 6467 6573 2e6a 736f 6e26 7175 6572 793d  dges.json&query=
-00005be0: 2532 342e 7079 7069 266c 6162 656c 3d50  %24.pypi&label=P
-00005bf0: 7950 6926 636f 6c6f 723d 626c 7565 2220  yPi&color=blue" 
-00005c00: 616c 743d 2250 7950 6922 3e0a 2020 3c69  alt="PyPi">.  <i
-00005c10: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00005c20: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
-00005c30: 6164 6765 2f64 796e 616d 6963 2f6a 736f  adge/dynamic/jso
-00005c40: 6e3f 7572 6c3d 6874 7470 7325 3341 2532  n?url=https%3A%2
-00005c50: 4625 3246 7261 7465 736c 6962 2e72 6561  F%2Frateslib.rea
-00005c60: 6474 6865 646f 6373 2e69 6f25 3246 656e  dthedocs.io%2Fen
-00005c70: 2532 466c 6174 6573 7425 3246 5f73 7461  %2Flatest%2F_sta
-00005c80: 7469 6325 3246 6261 6467 6573 2e6a 736f  tic%2Fbadges.jso
-00005c90: 6e26 7175 6572 793d 2532 342e 636f 6e64  n&query=%24.cond
-00005ca0: 6126 6c61 6265 6c3d 436f 6e64 6126 636f  a&label=Conda&co
-00005cb0: 6c6f 723d 626c 7565 2220 616c 743d 2243  lor=blue" alt="C
-00005cc0: 6f6e 6461 223e 0a20 203c 696d 6720 7372  onda">.  <img sr
-00005cd0: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-00005ce0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00005cf0: 6479 6e61 6d69 632f 6a73 6f6e 3f75 726c  dynamic/json?url
-00005d00: 3d68 7474 7073 2533 4125 3246 2532 4672  =https%3A%2F%2Fr
-00005d10: 6174 6573 6c69 622e 7265 6164 7468 6564  ateslib.readthed
-00005d20: 6f63 732e 696f 2532 4665 6e25 3246 6c61  ocs.io%2Fen%2Fla
-00005d30: 7465 7374 2532 465f 7374 6174 6963 2532  test%2F_static%2
-00005d40: 4662 6164 6765 732e 6a73 6f6e 2671 7565  Fbadges.json&que
-00005d50: 7279 3d25 3234 2e6c 6963 656e 6365 266c  ry=%24.licence&l
-00005d60: 6162 656c 3d4c 6963 656e 6365 2663 6f6c  abel=Licence&col
-00005d70: 6f72 3d6f 7261 6e67 6522 2061 6c74 3d22  or=orange" alt="
-00005d80: 4c69 6365 6e63 6522 3e0a 2020 3c69 6d67  Licence">.  <img
-00005d90: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00005da0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00005db0: 6765 2f64 796e 616d 6963 2f6a 736f 6e3f  ge/dynamic/json?
-00005dc0: 7572 6c3d 6874 7470 7325 3341 2532 4625  url=https%3A%2F%
-00005dd0: 3246 7261 7465 736c 6962 2e72 6561 6474  2Frateslib.readt
-00005de0: 6865 646f 6373 2e69 6f25 3246 656e 2532  hedocs.io%2Fen%2
-00005df0: 466c 6174 6573 7425 3246 5f73 7461 7469  Flatest%2F_stati
-00005e00: 6325 3246 6261 6467 6573 2e6a 736f 6e26  c%2Fbadges.json&
-00005e10: 7175 6572 793d 2532 342e 7374 6174 7573  query=%24.status
-00005e20: 266c 6162 656c 3d53 7461 7475 7326 636f  &label=Status&co
-00005e30: 6c6f 723d 6f72 616e 6765 2220 616c 743d  lor=orange" alt=
-00005e40: 2253 7461 7475 7322 3e0a 2020 3c69 6d67  "Status">.  <img
-00005e50: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-00005e60: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-00005e70: 6765 2f64 796e 616d 6963 2f6a 736f 6e3f  ge/dynamic/json?
-00005e80: 7572 6c3d 6874 7470 7325 3341 2532 4625  url=https%3A%2F%
-00005e90: 3246 7261 7465 736c 6962 2e72 6561 6474  2Frateslib.readt
-00005ea0: 6865 646f 6373 2e69 6f25 3246 656e 2532  hedocs.io%2Fen%2
-00005eb0: 466c 6174 6573 7425 3246 5f73 7461 7469  Flatest%2F_stati
-00005ec0: 6325 3246 6261 6467 6573 2e6a 736f 6e26  c%2Fbadges.json&
-00005ed0: 7175 6572 793d 2532 342e 636f 7665 7261  query=%24.covera
-00005ee0: 6765 266c 6162 656c 3d43 6f76 6572 6167  ge&label=Coverag
-00005ef0: 6526 636f 6c6f 723d 6772 6565 6e22 2061  e&color=green" a
-00005f00: 6c74 3d22 436f 7665 7261 6765 223e 0a20  lt="Coverage">. 
-00005f10: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00005f20: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00005f30: 6f2f 6261 6467 652f 6479 6e61 6d69 632f  o/badge/dynamic/
-00005f40: 6a73 6f6e 3f75 726c 3d68 7474 7073 2533  json?url=https%3
-00005f50: 4125 3246 2532 4672 6174 6573 6c69 622e  A%2F%2Frateslib.
-00005f60: 7265 6164 7468 6564 6f63 732e 696f 2532  readthedocs.io%2
-00005f70: 4665 6e25 3246 6c61 7465 7374 2532 465f  Fen%2Flatest%2F_
-00005f80: 7374 6174 6963 2532 4662 6164 6765 732e  static%2Fbadges.
-00005f90: 6a73 6f6e 2671 7565 7279 3d25 3234 2e73  json&query=%24.s
-00005fa0: 7479 6c65 266c 6162 656c 3d43 6f64 6525  tyle&label=Code%
-00005fb0: 3230 5374 796c 6526 636f 6c6f 723d 626c  20Style&color=bl
-00005fc0: 6163 6b22 2061 6c74 3d22 436f 6465 2053  ack" alt="Code S
-00005fd0: 7479 6c65 223e 0a3c 2f64 6976 3e0a 0a23  tyle">.</div>..#
-00005fe0: 2052 6174 6573 6c69 620a 0a60 6052 6174   Rateslib..``Rat
-00005ff0: 6573 6c69 6260 6020 6973 2061 2073 7461  eslib`` is a sta
-00006000: 7465 2d6f 662d 7468 652d 6172 7420 2a2a  te-of-the-art **
-00006010: 6669 7865 6420 696e 636f 6d65 206c 6962  fixed income lib
-00006020: 7261 7279 2a2a 2064 6573 6967 6e65 6420  rary** designed 
-00006030: 666f 7220 5079 7468 6f6e 2e0a 4974 7320  for Python..Its 
-00006040: 7075 7270 6f73 6520 6973 2074 6f20 7072  purpose is to pr
-00006050: 6f76 6964 6520 6164 7661 6e63 6564 2c20  ovide advanced, 
-00006060: 666c 6578 6962 6c65 2061 6e64 2065 6666  flexible and eff
-00006070: 6963 6965 6e74 2066 6978 6564 2069 6e63  icient fixed inc
-00006080: 6f6d 6520 616e 616c 7973 6973 0a77 6974  ome analysis.wit
-00006090: 6820 6120 6869 6768 206c 6576 656c 2c20  h a high level, 
-000060a0: 7765 6c6c 2064 6f63 756d 656e 7465 6420  well documented 
-000060b0: 4150 492e 0a0a 4974 7320 6465 7369 676e  API...Its design
-000060c0: 206f 626a 6563 7469 7665 2069 7320 746f   objective is to
-000060d0: 2062 6520 6162 6c65 2074 6f20 6372 6561   be able to crea
-000060e0: 7465 2061 2073 656c 662d 636f 6e73 6973  te a self-consis
-000060f0: 7465 6e74 2c20 6172 6269 7472 6167 6520  tent, arbitrage 
-00006100: 6672 6565 0a66 7261 6d65 776f 726b 2066  free.framework f
-00006110: 6f72 2070 7269 6369 6e67 2061 6c6c 2061  or pricing all a
-00006120: 7370 6563 7473 206f 6620 6669 7865 6420  spects of fixed 
-00006130: 696e 636f 6d65 2074 7261 6469 6e67 2c20  income trading, 
-00006140: 7375 6368 2061 7320 7370 6f74 2046 582c  such as spot FX,
-00006150: 2046 5820 666f 7277 6172 6473 2c0a 7369   FX forwards,.si
-00006160: 6e67 6c65 2063 7572 7265 6e63 7920 7365  ngle currency se
-00006170: 6375 7269 7469 6573 2061 6e64 2064 6572  curities and der
-00006180: 6976 6174 6976 6573 206c 696b 6520 6669  ivatives like fi
-00006190: 7865 6420 7261 7465 2062 6f6e 6473 2061  xed rate bonds a
-000061a0: 6e64 2049 5253 732c 2061 6e64 2061 6c73  nd IRSs, and als
-000061b0: 6f0a 6d75 6c74 692d 6375 7272 656e 6379  o.multi-currency
-000061c0: 2064 6572 6976 6174 6976 6573 2073 7563   derivatives suc
-000061d0: 6820 6173 2046 5820 7377 6170 7320 616e  h as FX swaps an
-000061e0: 6420 6372 6f73 732d 6375 7272 656e 6379  d cross-currency
-000061f0: 2073 7761 7073 2e20 4f70 7469 6f6e 732c   swaps. Options,
-00006200: 0a73 7761 7074 696f 6e73 2061 6e64 2069  .swaptions and i
-00006210: 6e66 6c61 7469 6f6e 2061 7265 2061 6c73  nflation are als
-00006220: 6f20 756e 6465 7220 636f 6e73 6964 6572  o under consider
-00006230: 6174 696f 6e20 666f 7220 6675 7475 7265  ation for future
-00006240: 2064 6576 656c 6f70 6d65 6e74 2e0a 0a54   development...T
-00006250: 6865 2074 6563 686e 6971 7565 7320 616e  he techniques an
-00006260: 6420 6f62 6a65 6374 2069 6e74 6572 6163  d object interac
-00006270: 7469 6f6e 2077 6974 6869 6e20 2a72 6174  tion within *rat
-00006280: 6573 6c69 622a 2077 6572 6520 696e 7370  eslib* were insp
-00006290: 6972 6564 2062 790a 7468 6520 7265 7175  ired by.the requ
-000062a0: 6972 656d 656e 7473 206f 6620 6d75 6c74  irements of mult
-000062b0: 692d 6469 7363 6970 6c69 6e65 6420 6669  i-disciplined fi
-000062c0: 7865 6420 696e 636f 6d65 2074 6561 6d73  xed income teams
-000062d0: 2077 6f72 6b69 6e67 2c20 626f 7468 2063   working, both c
-000062e0: 6f6f 7065 7261 7469 7665 6c79 0a61 6e64  ooperatively.and
-000062f0: 2069 6e64 6570 656e 6465 6e74 6c79 2c20   independently, 
-00006300: 7769 7468 696e 2067 6c6f 6261 6c20 696e  within global in
-00006310: 7665 7374 6d65 6e74 2062 616e 6b73 2e0a  vestment banks..
-00006320: 0a0a 4c69 6365 6e63 650a 3d3d 3d3d 3d3d  ..Licence.======
-00006330: 3d0a 0a54 6869 7320 6c69 6272 6172 7920  =..This library 
-00006340: 6973 2072 656c 6561 7365 6420 756e 6465  is released unde
-00006350: 7220 6120 2a2a 4372 6561 7469 7665 2043  r a **Creative C
-00006360: 6f6d 6d6f 6e73 2041 7474 7269 6275 7469  ommons Attributi
-00006370: 6f6e 2c20 4e6f 6e2d 436f 6d6d 6572 6369  on, Non-Commerci
-00006380: 616c 2c0a 4e6f 2d44 6572 6976 6174 6976  al,.No-Derivativ
-00006390: 6573 2034 2e30 2049 6e74 6572 6e61 7469  es 4.0 Internati
-000063a0: 6f6e 616c 204c 6963 656e 6365 2a2a 2e0a  onal Licence**..
-000063b0: 0a0a 4765 7420 5374 6172 7465 640a 3d3d  ..Get Started.==
-000063c0: 3d3d 3d3d 3d3d 3d3d 3d0a 0a52 6561 6420  =========..Read 
-000063d0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
-000063e0: 6e20 6174 200a 5b52 6174 6573 6c69 6220  n at .[Rateslib 
-000063f0: 5265 6164 2d74 6865 2d44 6f63 735d 2868  Read-the-Docs](h
-00006400: 7474 7073 3a2f 2f72 6174 6573 6c69 622e  ttps://rateslib.
-00006410: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
-00006420: 6e2f 6c61 7465 7374 2f29 0a0a 0a0a 0a0a  n/latest/)......
+00000000: 2e2e 205f 6c69 6365 6e63 652d 646f 633a  .. _licence-doc:
+00000010: 0a0a 2a2a 2a2a 2a2a 2a0a 4c69 6365 6e63  ..*******.Licenc
+00000020: 650a 2a2a 2a2a 2a2a 2a0a 0a0a 5468 6973  e.*******...This
+00000030: 206c 6962 7261 7279 2069 7320 7265 6c65   library is rele
+00000040: 6173 6564 2075 6e64 6572 2061 202a 2a43  ased under a **C
+00000050: 7265 6174 6976 6520 436f 6d6d 6f6e 7320  reative Commons 
+00000060: 4174 7472 6962 7574 696f 6e2c 204e 6f6e  Attribution, Non
+00000070: 2d43 6f6d 6d65 7263 6961 6c2c 0a4e 6f2d  -Commercial,.No-
+00000080: 4465 7269 7661 7469 7665 7320 342e 3020  Derivatives 4.0 
+00000090: 496e 7465 726e 6174 696f 6e61 6c20 4c69  International Li
+000000a0: 6365 6e63 652a 2a2e 0a0a 2e2e 2072 6177  cence**..... raw
+000000b0: 3a3a 2068 746d 6c0a 0a20 2020 3c74 6162  :: html..   <tab
+000000c0: 6c65 2073 7479 6c65 3d22 7769 6474 683a  le style="width:
+000000d0: 3130 3025 3b20 7465 7874 2d61 6c69 676e  100%; text-align
+000000e0: 3a63 656e 7465 723b 2062 6f72 6465 722d  :center; border-
+000000f0: 636f 6c6c 6170 7365 3a20 7365 7061 7261  collapse: separa
+00000100: 7465 3b20 666f 6e74 2d73 697a 653a 302e  te; font-size:0.
+00000110: 3865 6d3b 2062 6f72 6465 723a 2031 7078  8em; border: 1px
+00000120: 2073 6f6c 6964 2023 6430 6437 6465 3b20   solid #d0d7de; 
+00000130: 626f 7264 6572 2d72 6164 6975 733a 2035  border-radius: 5
+00000140: 7074 3b22 3e0a 2020 2020 2020 3c74 6865  pt;">.      <the
+00000150: 6164 2073 7479 6c65 3d22 6261 636b 6772  ad style="backgr
+00000160: 6f75 6e64 2d63 6f6c 6f72 3a20 2365 6266  ound-color: #ebf
+00000170: 3066 343b 223e 0a20 2020 2020 2020 203c  0f4;">.        <
+00000180: 7472 3e0a 2020 2020 2020 2020 2020 3c74  tr>.          <t
+00000190: 6820 7374 796c 653d 2263 6f6c 6f72 3a23  h style="color:#
+000001a0: 3435 3964 6239 3b20 626f 7264 6572 2d62  459db9; border-b
+000001b0: 6f74 746f 6d3a 2031 7078 2073 6f6c 6964  ottom: 1px solid
+000001c0: 2023 6430 6437 6465 3b22 3e41 6361 6465   #d0d7de;">Acade
+000001d0: 6d69 632c 2050 6572 736f 6e61 6c2c 206f  mic, Personal, o
+000001e0: 7220 4564 7563 6174 696f 6e61 6c20 5573  r Educational Us
+000001f0: 653c 2f74 683e 0a20 2020 2020 2020 2020  e</th>.         
+00000200: 203c 7468 2073 7479 6c65 3d22 636f 6c6f   <th style="colo
+00000210: 723a 2334 3539 6462 393b 2062 6f72 6465  r:#459db9; borde
+00000220: 722d 626f 7474 6f6d 3a20 3170 7820 736f  r-bottom: 1px so
+00000230: 6c69 6420 2364 3064 3764 653b 223e 436f  lid #d0d7de;">Co
+00000240: 6d6d 6572 6369 616c 2055 7365 3a20 4261  mmercial Use: Ba
+00000250: 6e6b 732c 2046 756e 6473 2c20 4163 636f  nks, Funds, Acco
+00000260: 756e 7461 6e74 732c 2054 7265 6173 7572  untants, Treasur
+00000270: 6965 733c 2f74 683e 0a20 2020 2020 2020  ies</th>.       
+00000280: 203c 2f74 723e 0a20 2020 2020 203c 2f74   </tr>.      </t
+00000290: 6865 6164 3e0a 2020 2020 2020 3c74 626f  head>.      <tbo
+000002a0: 6479 3e0a 2020 2020 2020 2020 3c74 723e  dy>.        <tr>
+000002b0: 0a20 2020 2020 2020 2020 203c 7464 2073  .          <td s
+000002c0: 7479 6c65 3d22 636f 6c6f 723a 6772 6565  tyle="color:gree
+000002d0: 6e3b 2066 6f6e 742d 7369 7a65 3a20 312e  n; font-size: 1.
+000002e0: 3235 656d 3b20 666f 6e74 2d77 6569 6768  25em; font-weigh
+000002f0: 743a 626f 6c64 3b22 3e46 5245 4520 746f  t:bold;">FREE to
+00000300: 2075 7365 2061 6e64 206d 6f64 6966 792e   use and modify.
+00000310: 3c62 723e 3c2f 7464 3e0a 2020 2020 2020  <br></td>.      
+00000320: 2020 2020 3c74 6420 7374 796c 653d 2222      <td style=""
+00000330: 3e0a 2020 2020 2020 2020 2020 3c73 7061  >.          <spa
+00000340: 6e20 7374 796c 653d 2263 6f6c 6f72 3a20  n style="color: 
+00000350: 7265 643b 2066 6f6e 742d 7369 7a65 3a31  red; font-size:1
+00000360: 2e32 3565 6d3b 223e 4e6f 7420 4c69 6365  .25em;">Not Lice
+00000370: 6e63 6564 2e3c 2f73 7061 6e3e 3c62 723e  nced.</span><br>
+00000380: 0a20 2020 2020 2020 2020 2020 2020 3c73  .             <s
+00000390: 7061 6e20 7374 796c 653d 2274 6578 742d  pan style="text-
+000003a0: 616c 6967 6e3a 2063 656e 7465 723b 2066  align: center; f
+000003b0: 6f6e 742d 7374 796c 653a 6974 616c 6963  ont-style:italic
+000003c0: 3b22 3e0a 2020 2020 2020 2020 2020 2020  ;">.            
+000003d0: 2043 616e 2070 7572 6368 6173 6520 6120   Can purchase a 
+000003e0: 6c69 6365 6e63 6520 6578 7465 6e73 696f  licence extensio
+000003f0: 6e2e 2024 3330 3020 7065 7220 7965 6172  n. $300 per year
+00000400: 202f 2070 6572 2075 7365 722e 3c2f 7370   / per user.</sp
+00000410: 616e 3e3c 6272 3e0a 2020 2020 2020 2020  an><br>.        
+00000420: 2020 2020 203c 7370 616e 2073 7479 6c65       <span style
+00000430: 3d22 7465 7874 2d61 6c69 676e 3a20 6365  ="text-align: ce
+00000440: 6e74 6572 3b20 666f 6e74 2d73 7479 6c65  nter; font-style
+00000450: 3a69 7461 6c69 633b 223e 0a20 2020 2020  :italic;">.     
+00000460: 2020 2020 2020 2020 636f 6e74 6163 743a          contact:
+00000470: 2072 6174 6573 6c69 6240 676d 6169 6c2e   rateslib@gmail.
+00000480: 636f 6d0a 2020 2020 2020 2020 2020 2020  com.            
+00000490: 203c 2f73 7061 6e3e 0a20 2020 2020 2020   </span>.       
+000004a0: 2020 203c 2f74 643e 0a20 2020 2020 2020     </td>.       
+000004b0: 203c 2f74 723e 0a20 2020 2020 203c 2f74   </tr>.      </t
+000004c0: 626f 6479 3e0a 2020 203c 2f74 6162 6c65  body>.   </table
+000004d0: 3e0a 0a2e 2e20 6e6f 7465 3a3a 0a0a 2020  >.... note::..  
+000004e0: 2054 6869 7320 6d65 616e 7320 7468 6174   This means that
+000004f0: 2079 6f75 202a 2a63 616e 2a2a 3b0a 0a20   you **can**;.. 
+00000500: 2020 2d20 446f 776e 6c6f 6164 2061 6e64    - Download and
+00000510: 2075 7365 2074 6865 2063 6f64 6520 7072   use the code pr
+00000520: 6976 6174 656c 7920 696e 2061 206e 6f6e  ivately in a non
+00000530: 2d70 726f 6669 7420 6675 6e63 7469 6f6e  -profit function
+00000540: 2c20 7375 6368 2061 7320 6120 6c65 6172  , such as a lear
+00000550: 6e69 6e67 2065 6e76 6972 6f6e 6d65 6e74  ning environment
+00000560: 2e0a 2020 202d 204d 6f64 6966 7920 7468  ..   - Modify th
+00000570: 6520 636f 6465 2066 6f72 202a 2a70 7269  e code for **pri
+00000580: 7661 7465 2c20 6e6f 6e2d 636f 6d6d 6572  vate, non-commer
+00000590: 6963 616c 2075 7365 2a2a 206f 6e6c 792e  ical use** only.
+000005a0: 0a20 2020 2d20 5368 6172 6520 6f72 2072  .   - Share or r
+000005b0: 6564 6973 7472 6962 7574 6520 7468 6520  edistribute the 
+000005c0: 636f 6465 2c20 6275 7420 6f6e 6c79 2069  code, but only i
+000005d0: 6e20 6974 7320 2a2a 656e 7469 7265 7479  n its **entirety
+000005e0: 2077 6974 686f 7574 206d 6f64 6966 6963   without modific
+000005f0: 6174 696f 6e2a 2a2c 2061 6e64 202a 2a77  ation**, and **w
+00000600: 6974 6820 6174 7472 6962 7574 696f 6e2a  ith attribution*
+00000610: 2a2c 0a20 2020 2020 616e 6420 7375 6368  *,.     and such
+00000620: 2074 6861 7420 2a2a 656e 6420 7573 6520   that **end use 
+00000630: 6973 206e 6f6e 2d63 6f6d 6d65 7263 6961  is non-commercia
+00000640: 6c2a 2a20 616e 6420 696e 2061 206e 6f6e  l** and in a non
+00000650: 2d70 726f 6669 7420 6675 6e63 7469 6f6e  -profit function
+00000660: 2e0a 0a2e 2e20 7761 726e 696e 673a 3a0a  ..... warning::.
+00000670: 0a20 2020 5468 6973 206d 6561 6e73 2074  .   This means t
+00000680: 6861 7420 796f 7520 2a2a 6361 6e6e 6f74  hat you **cannot
+00000690: 2a2a 3b0a 0a20 2020 2d20 5573 6520 7468  **;..   - Use th
+000006a0: 6520 6c69 6272 6172 7920 6f72 2063 6f64  e library or cod
+000006b0: 6520 666f 7220 616e 7920 666f 726d 206f  e for any form o
+000006c0: 6620 636f 6d6d 6572 6369 616c 206f 7220  f commercial or 
+000006d0: 7072 6f66 6974 2062 6173 6564 2061 6374  profit based act
+000006e0: 6976 6974 792e 2059 6f75 2063 616e 6e6f  ivity. You canno
+000006f0: 7420 7573 6520 6974 0a20 2020 2020 696e  t use it.     in
+00000700: 7369 6465 2061 2062 616e 6b2c 2066 756e  side a bank, fun
+00000710: 6420 636f 6d70 616e 792c 2062 726f 6b65  d company, broke
+00000720: 7261 6765 2066 6972 6d2c 206f 7220 616e  rage firm, or an
+00000730: 7920 666f 726d 206f 6620 696e 7665 7374  y form of invest
+00000740: 6d65 6e74 2066 6972 6d20 7768 6572 650a  ment firm where.
+00000750: 2020 2020 2069 7473 2075 7365 2069 7320       its use is 
+00000760: 7061 7274 206f 6620 7468 6520 6f70 6572  part of the oper
+00000770: 6174 696f 6e2c 206f 7220 6465 6369 7369  ation, or decisi
+00000780: 6f6e 206d 616b 696e 6720 7072 6f63 6573  on making proces
+00000790: 732c 206f 6620 7468 6174 2065 6e74 6974  s, of that entit
+000007a0: 792e 0a20 2020 2d20 436f 7079 206f 7220  y..   - Copy or 
+000007b0: 6d6f 6469 6679 2074 6865 2063 6f64 6520  modify the code 
+000007c0: 616e 6420 7573 6520 6974 2069 6e20 616e  and use it in an
+000007d0: 7920 6465 7269 7661 7469 7665 2070 726f  y derivative pro
+000007e0: 6475 6374 206f 7220 636f 6d6d 6572 6369  duct or commerci
+000007f0: 616c 2061 6374 6976 6974 792c 0a20 2020  al activity,.   
+00000800: 2020 7375 6368 2061 7320 696e 2061 2074    such as in a t
+00000810: 7261 6469 6e67 2061 7070 6c69 6361 7469  rading applicati
+00000820: 6f6e 2c20 4150 4920 6f72 206f 7468 6572  on, API or other
+00000830: 2066 6f72 6d20 6f66 2070 7562 6c69 6361   form of publica
+00000840: 7469 6f6e 2e0a 2020 202d 2053 6861 7265  tion..   - Share
+00000850: 206f 7220 7265 6469 7374 7269 6275 7465   or redistribute
+00000860: 2061 6e79 202a 2a73 7562 2d70 6172 742a   any **sub-part*
+00000870: 2a20 6f66 2074 6865 2063 6f64 652c 206f  * of the code, o
+00000880: 7220 2a2a 6d6f 6469 6669 6564 2a2a 2063  r **modified** c
+00000890: 6f64 652c 2065 7665 6e20 7769 7468 2061  ode, even with a
+000008a0: 7474 7269 6275 7469 6f6e 2e0a 2020 202d  ttribution..   -
+000008b0: 2053 6861 7265 206f 7220 7265 6469 7374   Share or redist
+000008c0: 7269 6275 7465 2074 6865 2063 6f64 6520  ribute the code 
+000008d0: 696e 2069 7473 2065 6e74 6972 6574 7920  in its entirety 
+000008e0: 2a2a 7769 7468 6f75 7420 6174 7472 6962  **without attrib
+000008f0: 7574 696f 6e2a 2a2e 0a20 2020 2d20 496e  ution**..   - In
+00000900: 636c 7564 6520 7468 6973 2063 6f64 652c  clude this code,
+00000910: 206f 7220 7061 636b 6167 652c 2061 7320   or package, as 
+00000920: 6120 2a2a 6465 7065 6e64 656e 6379 2a2a  a **dependency**
+00000930: 206f 6620 616e 7920 6f74 6865 7220 7061   of any other pa
+00000940: 636b 6167 652e 0a20 2020 2d20 5573 6520  ckage..   - Use 
+00000950: 7468 6973 2063 6f64 6520 6173 2061 2062  this code as a b
+00000960: 656e 6368 6d61 726b 206f 7220 6173 2061  enchmark or as a
+00000970: 2076 616c 6964 6174 6f72 2066 6f72 2064   validator for d
+00000980: 6576 656c 6f70 696e 6720 796f 7572 206f  eveloping your o
+00000990: 776e 2063 6f64 650a 2020 2020 2077 6869  wn code.     whi
+000009a0: 6368 2077 696c 6c20 6265 2075 7365 6420  ch will be used 
+000009b0: 696e 2061 2063 6f6d 6d65 7263 6961 6c20  in a commercial 
+000009c0: 6361 7061 6369 7479 2e0a 0a0a 4372 6561  capacity....Crea
+000009d0: 7469 7665 2043 6f6d 6d6f 6e73 2041 7474  tive Commons Att
+000009e0: 7269 6275 7469 6f6e 2c20 4e6f 6e2d 436f  ribution, Non-Co
+000009f0: 6d6d 6572 6369 616c 2c20 4e6f 2d44 6572  mmercial, No-Der
+00000a00: 6976 6174 6976 6573 2034 2e30 2049 6e74  ivatives 4.0 Int
+00000a10: 6572 6e61 7469 6f6e 616c 2050 7562 6c69  ernational Publi
+00000a20: 6320 4c69 6365 6e73 650a 3d3d 3d3d 3d3d  c License.======
+00000a30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000a80: 3d3d 3d3d 3d3d 3d0a 0a42 7920 6578 6572  =======..By exer
+00000a90: 6369 7369 6e67 2074 6865 204c 6963 656e  cising the Licen
+00000aa0: 7365 6420 5269 6768 7473 2028 6465 6669  sed Rights (defi
+00000ab0: 6e65 6420 6265 6c6f 7729 2c20 596f 7520  ned below), You 
+00000ac0: 6163 6365 7074 2061 6e64 2061 6772 6565  accept and agree
+00000ad0: 0a74 6f20 6265 2062 6f75 6e64 2062 7920  .to be bound by 
+00000ae0: 7468 6520 7465 726d 7320 616e 6420 636f  the terms and co
+00000af0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
+00000b00: 2043 7265 6174 6976 6520 436f 6d6d 6f6e   Creative Common
+00000b10: 730a 4174 7472 6962 7574 696f 6e2d 4e6f  s.Attribution-No
+00000b20: 6e43 6f6d 6d65 7263 6961 6c2d 4e6f 4465  nCommercial-NoDe
+00000b30: 7269 7661 7469 7665 7320 342e 3020 496e  rivatives 4.0 In
+00000b40: 7465 726e 6174 696f 6e61 6c20 5075 626c  ternational Publ
+00000b50: 6963 0a4c 6963 656e 7365 2028 2250 7562  ic.License ("Pub
+00000b60: 6c69 6320 4c69 6365 6e73 6522 292e 2054  lic License"). T
+00000b70: 6f20 7468 6520 6578 7465 6e74 2074 6869  o the extent thi
+00000b80: 7320 5075 626c 6963 204c 6963 656e 7365  s Public License
+00000b90: 206d 6179 2062 650a 696e 7465 7270 7265   may be.interpre
+00000ba0: 7465 6420 6173 2061 2063 6f6e 7472 6163  ted as a contrac
+00000bb0: 742c 2059 6f75 2061 7265 2067 7261 6e74  t, You are grant
+00000bc0: 6564 2074 6865 204c 6963 656e 7365 6420  ed the Licensed 
+00000bd0: 5269 6768 7473 2069 6e0a 636f 6e73 6964  Rights in.consid
+00000be0: 6572 6174 696f 6e20 6f66 2059 6f75 7220  eration of Your 
+00000bf0: 6163 6365 7074 616e 6365 206f 6620 7468  acceptance of th
+00000c00: 6573 6520 7465 726d 7320 616e 6420 636f  ese terms and co
+00000c10: 6e64 6974 696f 6e73 2c20 616e 6420 7468  nditions, and th
+00000c20: 650a 4c69 6365 6e73 6f72 2067 7261 6e74  e.Licensor grant
+00000c30: 7320 596f 7520 7375 6368 2072 6967 6874  s You such right
+00000c40: 7320 696e 2063 6f6e 7369 6465 7261 7469  s in considerati
+00000c50: 6f6e 206f 6620 6265 6e65 6669 7473 2074  on of benefits t
+00000c60: 6865 0a4c 6963 656e 736f 7220 7265 6365  he.Licensor rece
+00000c70: 6976 6573 2066 726f 6d20 6d61 6b69 6e67  ives from making
+00000c80: 2074 6865 204c 6963 656e 7365 6420 4d61   the Licensed Ma
+00000c90: 7465 7269 616c 2061 7661 696c 6162 6c65  terial available
+00000ca0: 2075 6e64 6572 0a74 6865 7365 2074 6572   under.these ter
+00000cb0: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
+00000cc0: 732e 0a0a 0a53 6563 7469 6f6e 2031 202d  s....Section 1 -
+00000cd0: 2d20 4465 6669 6e69 7469 6f6e 732e 0a2d  - Definitions..-
+00000ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000cf0: 2d2d 2d2d 2d2d 2d2d 0a0a 2020 612e 2041  --------..  a. A
+00000d00: 6461 7074 6564 204d 6174 6572 6961 6c20  dapted Material 
+00000d10: 6d65 616e 7320 6d61 7465 7269 616c 2073  means material s
+00000d20: 7562 6a65 6374 2074 6f20 436f 7079 7269  ubject to Copyri
+00000d30: 6768 7420 616e 6420 5369 6d69 6c61 720a  ght and Similar.
+00000d40: 2020 2020 2052 6967 6874 7320 7468 6174       Rights that
+00000d50: 2069 7320 6465 7269 7665 6420 6672 6f6d   is derived from
+00000d60: 206f 7220 6261 7365 6420 7570 6f6e 2074   or based upon t
+00000d70: 6865 204c 6963 656e 7365 6420 4d61 7465  he Licensed Mate
+00000d80: 7269 616c 0a20 2020 2020 616e 6420 696e  rial.     and in
+00000d90: 2077 6869 6368 2074 6865 204c 6963 656e   which the Licen
+00000da0: 7365 6420 4d61 7465 7269 616c 2069 7320  sed Material is 
+00000db0: 7472 616e 736c 6174 6564 2c20 616c 7465  translated, alte
+00000dc0: 7265 642c 0a20 2020 2020 6172 7261 6e67  red,.     arrang
+00000dd0: 6564 2c20 7472 616e 7366 6f72 6d65 642c  ed, transformed,
+00000de0: 206f 7220 6f74 6865 7277 6973 6520 6d6f   or otherwise mo
+00000df0: 6469 6669 6564 2069 6e20 6120 6d61 6e6e  dified in a mann
+00000e00: 6572 2072 6571 7569 7269 6e67 0a20 2020  er requiring.   
+00000e10: 2020 7065 726d 6973 7369 6f6e 2075 6e64    permission und
+00000e20: 6572 2074 6865 2043 6f70 7972 6967 6874  er the Copyright
+00000e30: 2061 6e64 2053 696d 696c 6172 2052 6967   and Similar Rig
+00000e40: 6874 7320 6865 6c64 2062 7920 7468 650a  hts held by the.
+00000e50: 2020 2020 204c 6963 656e 736f 722e 2046       Licensor. F
+00000e60: 6f72 2070 7572 706f 7365 7320 6f66 2074  or purposes of t
+00000e70: 6869 7320 5075 626c 6963 204c 6963 656e  his Public Licen
+00000e80: 7365 2c20 7768 6572 6520 7468 6520 4c69  se, where the Li
+00000e90: 6365 6e73 6564 0a20 2020 2020 4d61 7465  censed.     Mate
+00000ea0: 7269 616c 2069 7320 6120 6d75 7369 6361  rial is a musica
+00000eb0: 6c20 776f 726b 2c20 7065 7266 6f72 6d61  l work, performa
+00000ec0: 6e63 652c 206f 7220 736f 756e 6420 7265  nce, or sound re
+00000ed0: 636f 7264 696e 672c 0a20 2020 2020 4164  cording,.     Ad
+00000ee0: 6170 7465 6420 4d61 7465 7269 616c 2069  apted Material i
+00000ef0: 7320 616c 7761 7973 2070 726f 6475 6365  s always produce
+00000f00: 6420 7768 6572 6520 7468 6520 4c69 6365  d where the Lice
+00000f10: 6e73 6564 204d 6174 6572 6961 6c20 6973  nsed Material is
+00000f20: 0a20 2020 2020 7379 6e63 6865 6420 696e  .     synched in
+00000f30: 2074 696d 6564 2072 656c 6174 696f 6e20   timed relation 
+00000f40: 7769 7468 2061 206d 6f76 696e 6720 696d  with a moving im
+00000f50: 6167 652e 0a0a 2020 622e 2043 6f70 7972  age...  b. Copyr
+00000f60: 6967 6874 2061 6e64 2053 696d 696c 6172  ight and Similar
+00000f70: 2052 6967 6874 7320 6d65 616e 7320 636f   Rights means co
+00000f80: 7079 7269 6768 7420 616e 642f 6f72 2073  pyright and/or s
+00000f90: 696d 696c 6172 2072 6967 6874 730a 2020  imilar rights.  
+00000fa0: 2020 2063 6c6f 7365 6c79 2072 656c 6174     closely relat
+00000fb0: 6564 2074 6f20 636f 7079 7269 6768 7420  ed to copyright 
+00000fc0: 696e 636c 7564 696e 672c 2077 6974 686f  including, witho
+00000fd0: 7574 206c 696d 6974 6174 696f 6e2c 0a20  ut limitation,. 
+00000fe0: 2020 2020 7065 7266 6f72 6d61 6e63 652c      performance,
+00000ff0: 2062 726f 6164 6361 7374 2c20 736f 756e   broadcast, soun
+00001000: 6420 7265 636f 7264 696e 672c 2061 6e64  d recording, and
+00001010: 2053 7569 2047 656e 6572 6973 2044 6174   Sui Generis Dat
+00001020: 6162 6173 650a 2020 2020 2052 6967 6874  abase.     Right
+00001030: 732c 2077 6974 686f 7574 2072 6567 6172  s, without regar
+00001040: 6420 746f 2068 6f77 2074 6865 2072 6967  d to how the rig
+00001050: 6874 7320 6172 6520 6c61 6265 6c65 6420  hts are labeled 
+00001060: 6f72 0a20 2020 2020 6361 7465 676f 7269  or.     categori
+00001070: 7a65 642e 2046 6f72 2070 7572 706f 7365  zed. For purpose
+00001080: 7320 6f66 2074 6869 7320 5075 626c 6963  s of this Public
+00001090: 204c 6963 656e 7365 2c20 7468 6520 7269   License, the ri
+000010a0: 6768 7473 0a20 2020 2020 7370 6563 6966  ghts.     specif
+000010b0: 6965 6420 696e 2053 6563 7469 6f6e 2032  ied in Section 2
+000010c0: 2862 2928 3129 2d28 3229 2061 7265 206e  (b)(1)-(2) are n
+000010d0: 6f74 2043 6f70 7972 6967 6874 2061 6e64  ot Copyright and
+000010e0: 2053 696d 696c 6172 0a20 2020 2020 5269   Similar.     Ri
+000010f0: 6768 7473 2e0a 0a20 2063 2e20 4566 6665  ghts...  c. Effe
+00001100: 6374 6976 6520 5465 6368 6e6f 6c6f 6769  ctive Technologi
+00001110: 6361 6c20 4d65 6173 7572 6573 206d 6561  cal Measures mea
+00001120: 6e73 2074 686f 7365 206d 6561 7375 7265  ns those measure
+00001130: 7320 7468 6174 2c20 696e 2074 6865 0a20  s that, in the. 
+00001140: 2020 2020 6162 7365 6e63 6520 6f66 2070      absence of p
+00001150: 726f 7065 7220 6175 7468 6f72 6974 792c  roper authority,
+00001160: 206d 6179 206e 6f74 2062 6520 6369 7263   may not be circ
+00001170: 756d 7665 6e74 6564 2075 6e64 6572 206c  umvented under l
+00001180: 6177 730a 2020 2020 2066 756c 6669 6c6c  aws.     fulfill
+00001190: 696e 6720 6f62 6c69 6761 7469 6f6e 7320  ing obligations 
+000011a0: 756e 6465 7220 4172 7469 636c 6520 3131  under Article 11
+000011b0: 206f 6620 7468 6520 5749 504f 2043 6f70   of the WIPO Cop
+000011c0: 7972 6967 6874 0a20 2020 2020 5472 6561  yright.     Trea
+000011d0: 7479 2061 646f 7074 6564 206f 6e20 4465  ty adopted on De
+000011e0: 6365 6d62 6572 2032 302c 2031 3939 362c  cember 20, 1996,
+000011f0: 2061 6e64 2f6f 7220 7369 6d69 6c61 7220   and/or similar 
+00001200: 696e 7465 726e 6174 696f 6e61 6c0a 2020  international.  
+00001210: 2020 2061 6772 6565 6d65 6e74 732e 0a0a     agreements...
+00001220: 2020 642e 2045 7863 6570 7469 6f6e 7320    d. Exceptions 
+00001230: 616e 6420 4c69 6d69 7461 7469 6f6e 7320  and Limitations 
+00001240: 6d65 616e 7320 6661 6972 2075 7365 2c20  means fair use, 
+00001250: 6661 6972 2064 6561 6c69 6e67 2c20 616e  fair dealing, an
+00001260: 642f 6f72 0a20 2020 2020 616e 7920 6f74  d/or.     any ot
+00001270: 6865 7220 6578 6365 7074 696f 6e20 6f72  her exception or
+00001280: 206c 696d 6974 6174 696f 6e20 746f 2043   limitation to C
+00001290: 6f70 7972 6967 6874 2061 6e64 2053 696d  opyright and Sim
+000012a0: 696c 6172 2052 6967 6874 730a 2020 2020  ilar Rights.    
+000012b0: 2074 6861 7420 6170 706c 6965 7320 746f   that applies to
+000012c0: 2059 6f75 7220 7573 6520 6f66 2074 6865   Your use of the
+000012d0: 204c 6963 656e 7365 6420 4d61 7465 7269   Licensed Materi
+000012e0: 616c 2e0a 0a20 2065 2e20 4c69 6365 6e73  al...  e. Licens
+000012f0: 6564 204d 6174 6572 6961 6c20 6d65 616e  ed Material mean
+00001300: 7320 7468 6520 6172 7469 7374 6963 206f  s the artistic o
+00001310: 7220 6c69 7465 7261 7279 2077 6f72 6b2c  r literary work,
+00001320: 2064 6174 6162 6173 652c 0a20 2020 2020   database,.     
+00001330: 6f72 206f 7468 6572 206d 6174 6572 6961  or other materia
+00001340: 6c20 746f 2077 6869 6368 2074 6865 204c  l to which the L
+00001350: 6963 656e 736f 7220 6170 706c 6965 6420  icensor applied 
+00001360: 7468 6973 2050 7562 6c69 630a 2020 2020  this Public.    
+00001370: 204c 6963 656e 7365 2e0a 0a20 2066 2e20   License...  f. 
+00001380: 4c69 6365 6e73 6564 2052 6967 6874 7320  Licensed Rights 
+00001390: 6d65 616e 7320 7468 6520 7269 6768 7473  means the rights
+000013a0: 2067 7261 6e74 6564 2074 6f20 596f 7520   granted to You 
+000013b0: 7375 626a 6563 7420 746f 2074 6865 0a20  subject to the. 
+000013c0: 2020 2020 7465 726d 7320 616e 6420 636f      terms and co
+000013d0: 6e64 6974 696f 6e73 206f 6620 7468 6973  nditions of this
+000013e0: 2050 7562 6c69 6320 4c69 6365 6e73 652c   Public License,
+000013f0: 2077 6869 6368 2061 7265 206c 696d 6974   which are limit
+00001400: 6564 2074 6f0a 2020 2020 2061 6c6c 2043  ed to.     all C
+00001410: 6f70 7972 6967 6874 2061 6e64 2053 696d  opyright and Sim
+00001420: 696c 6172 2052 6967 6874 7320 7468 6174  ilar Rights that
+00001430: 2061 7070 6c79 2074 6f20 596f 7572 2075   apply to Your u
+00001440: 7365 206f 6620 7468 650a 2020 2020 204c  se of the.     L
+00001450: 6963 656e 7365 6420 4d61 7465 7269 616c  icensed Material
+00001460: 2061 6e64 2074 6861 7420 7468 6520 4c69   and that the Li
+00001470: 6365 6e73 6f72 2068 6173 2061 7574 686f  censor has autho
+00001480: 7269 7479 2074 6f20 6c69 6365 6e73 652e  rity to license.
+00001490: 0a0a 2020 672e 204c 6963 656e 736f 7220  ..  g. Licensor 
+000014a0: 6d65 616e 7320 7468 6520 696e 6469 7669  means the indivi
+000014b0: 6475 616c 2873 2920 6f72 2065 6e74 6974  dual(s) or entit
+000014c0: 7928 6965 7329 2067 7261 6e74 696e 6720  y(ies) granting 
+000014d0: 7269 6768 7473 0a20 2020 2020 756e 6465  rights.     unde
+000014e0: 7220 7468 6973 2050 7562 6c69 6320 4c69  r this Public Li
+000014f0: 6365 6e73 652e 0a0a 2020 682e 204e 6f6e  cense...  h. Non
+00001500: 436f 6d6d 6572 6369 616c 206d 6561 6e73  Commercial means
+00001510: 206e 6f74 2070 7269 6d61 7269 6c79 2069   not primarily i
+00001520: 6e74 656e 6465 6420 666f 7220 6f72 2064  ntended for or d
+00001530: 6972 6563 7465 6420 746f 7761 7264 730a  irected towards.
+00001540: 2020 2020 2063 6f6d 6d65 7263 6961 6c20       commercial 
+00001550: 6164 7661 6e74 6167 6520 6f72 206d 6f6e  advantage or mon
+00001560: 6574 6172 7920 636f 6d70 656e 7361 7469  etary compensati
+00001570: 6f6e 2e20 466f 7220 7075 7270 6f73 6573  on. For purposes
+00001580: 206f 660a 2020 2020 2074 6869 7320 5075   of.     this Pu
+00001590: 626c 6963 204c 6963 656e 7365 2c20 7468  blic License, th
+000015a0: 6520 6578 6368 616e 6765 206f 6620 7468  e exchange of th
+000015b0: 6520 4c69 6365 6e73 6564 204d 6174 6572  e Licensed Mater
+000015c0: 6961 6c20 666f 720a 2020 2020 206f 7468  ial for.     oth
+000015d0: 6572 206d 6174 6572 6961 6c20 7375 626a  er material subj
+000015e0: 6563 7420 746f 2043 6f70 7972 6967 6874  ect to Copyright
+000015f0: 2061 6e64 2053 696d 696c 6172 2052 6967   and Similar Rig
+00001600: 6874 7320 6279 2064 6967 6974 616c 0a20  hts by digital. 
+00001610: 2020 2020 6669 6c65 2d73 6861 7269 6e67      file-sharing
+00001620: 206f 7220 7369 6d69 6c61 7220 6d65 616e   or similar mean
+00001630: 7320 6973 204e 6f6e 436f 6d6d 6572 6369  s is NonCommerci
+00001640: 616c 2070 726f 7669 6465 6420 7468 6572  al provided ther
+00001650: 6520 6973 0a20 2020 2020 6e6f 2070 6179  e is.     no pay
+00001660: 6d65 6e74 206f 6620 6d6f 6e65 7461 7279  ment of monetary
+00001670: 2063 6f6d 7065 6e73 6174 696f 6e20 696e   compensation in
+00001680: 2063 6f6e 6e65 6374 696f 6e20 7769 7468   connection with
+00001690: 2074 6865 0a20 2020 2020 6578 6368 616e   the.     exchan
+000016a0: 6765 2e0a 0a20 2069 2e20 5368 6172 6520  ge...  i. Share 
+000016b0: 6d65 616e 7320 746f 2070 726f 7669 6465  means to provide
+000016c0: 206d 6174 6572 6961 6c20 746f 2074 6865   material to the
+000016d0: 2070 7562 6c69 6320 6279 2061 6e79 206d   public by any m
+000016e0: 6561 6e73 206f 720a 2020 2020 2070 726f  eans or.     pro
+000016f0: 6365 7373 2074 6861 7420 7265 7175 6972  cess that requir
+00001700: 6573 2070 6572 6d69 7373 696f 6e20 756e  es permission un
+00001710: 6465 7220 7468 6520 4c69 6365 6e73 6564  der the Licensed
+00001720: 2052 6967 6874 732c 2073 7563 680a 2020   Rights, such.  
+00001730: 2020 2061 7320 7265 7072 6f64 7563 7469     as reproducti
+00001740: 6f6e 2c20 7075 626c 6963 2064 6973 706c  on, public displ
+00001750: 6179 2c20 7075 626c 6963 2070 6572 666f  ay, public perfo
+00001760: 726d 616e 6365 2c20 6469 7374 7269 6275  rmance, distribu
+00001770: 7469 6f6e 2c0a 2020 2020 2064 6973 7365  tion,.     disse
+00001780: 6d69 6e61 7469 6f6e 2c20 636f 6d6d 756e  mination, commun
+00001790: 6963 6174 696f 6e2c 206f 7220 696d 706f  ication, or impo
+000017a0: 7274 6174 696f 6e2c 2061 6e64 2074 6f20  rtation, and to 
+000017b0: 6d61 6b65 206d 6174 6572 6961 6c0a 2020  make material.  
+000017c0: 2020 2061 7661 696c 6162 6c65 2074 6f20     available to 
+000017d0: 7468 6520 7075 626c 6963 2069 6e63 6c75  the public inclu
+000017e0: 6469 6e67 2069 6e20 7761 7973 2074 6861  ding in ways tha
+000017f0: 7420 6d65 6d62 6572 7320 6f66 2074 6865  t members of the
+00001800: 0a20 2020 2020 7075 626c 6963 206d 6179  .     public may
+00001810: 2061 6363 6573 7320 7468 6520 6d61 7465   access the mate
+00001820: 7269 616c 2066 726f 6d20 6120 706c 6163  rial from a plac
+00001830: 6520 616e 6420 6174 2061 2074 696d 650a  e and at a time.
+00001840: 2020 2020 2069 6e64 6976 6964 7561 6c6c       individuall
+00001850: 7920 6368 6f73 656e 2062 7920 7468 656d  y chosen by them
+00001860: 2e0a 0a20 206a 2e20 5375 6920 4765 6e65  ...  j. Sui Gene
+00001870: 7269 7320 4461 7461 6261 7365 2052 6967  ris Database Rig
+00001880: 6874 7320 6d65 616e 7320 7269 6768 7473  hts means rights
+00001890: 206f 7468 6572 2074 6861 6e20 636f 7079   other than copy
+000018a0: 7269 6768 740a 2020 2020 2072 6573 756c  right.     resul
+000018b0: 7469 6e67 2066 726f 6d20 4469 7265 6374  ting from Direct
+000018c0: 6976 6520 3936 2f39 2f45 4320 6f66 2074  ive 96/9/EC of t
+000018d0: 6865 2045 7572 6f70 6561 6e20 5061 726c  he European Parl
+000018e0: 6961 6d65 6e74 2061 6e64 206f 660a 2020  iament and of.  
+000018f0: 2020 2074 6865 2043 6f75 6e63 696c 206f     the Council o
+00001900: 6620 3131 204d 6172 6368 2031 3939 3620  f 11 March 1996 
+00001910: 6f6e 2074 6865 206c 6567 616c 2070 726f  on the legal pro
+00001920: 7465 6374 696f 6e20 6f66 2064 6174 6162  tection of datab
+00001930: 6173 6573 2c0a 2020 2020 2061 7320 616d  ases,.     as am
+00001940: 656e 6465 6420 616e 642f 6f72 2073 7563  ended and/or suc
+00001950: 6365 6564 6564 2c20 6173 2077 656c 6c20  ceeded, as well 
+00001960: 6173 206f 7468 6572 2065 7373 656e 7469  as other essenti
+00001970: 616c 6c79 0a20 2020 2020 6571 7569 7661  ally.     equiva
+00001980: 6c65 6e74 2072 6967 6874 7320 616e 7977  lent rights anyw
+00001990: 6865 7265 2069 6e20 7468 6520 776f 726c  here in the worl
+000019a0: 642e 0a0a 2020 6b2e 2059 6f75 206d 6561  d...  k. You mea
+000019b0: 6e73 2074 6865 2069 6e64 6976 6964 7561  ns the individua
+000019c0: 6c20 6f72 2065 6e74 6974 7920 6578 6572  l or entity exer
+000019d0: 6369 7369 6e67 2074 6865 204c 6963 656e  cising the Licen
+000019e0: 7365 6420 5269 6768 7473 0a20 2020 2020  sed Rights.     
+000019f0: 756e 6465 7220 7468 6973 2050 7562 6c69  under this Publi
+00001a00: 6320 4c69 6365 6e73 652e 2059 6f75 7220  c License. Your 
+00001a10: 6861 7320 6120 636f 7272 6573 706f 6e64  has a correspond
+00001a20: 696e 6720 6d65 616e 696e 672e 0a0a 0a53  ing meaning....S
+00001a30: 6563 7469 6f6e 2032 202d 2d20 5363 6f70  ection 2 -- Scop
+00001a40: 652e 0a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  e..-------------
+00001a50: 2d2d 2d2d 2d2d 0a0a 2020 612e 204c 6963  ------..  a. Lic
+00001a60: 656e 7365 2067 7261 6e74 2e0a 0a20 2020  ense grant...   
+00001a70: 2020 2020 312e 2053 7562 6a65 6374 2074      1. Subject t
+00001a80: 6f20 7468 6520 7465 726d 7320 616e 6420  o the terms and 
+00001a90: 636f 6e64 6974 696f 6e73 206f 6620 7468  conditions of th
+00001aa0: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
+00001ab0: 652c 0a20 2020 2020 2020 2020 2074 6865  e,.          the
+00001ac0: 204c 6963 656e 736f 7220 6865 7265 6279   Licensor hereby
+00001ad0: 2067 7261 6e74 7320 596f 7520 6120 776f   grants You a wo
+00001ae0: 726c 6477 6964 652c 2072 6f79 616c 7479  rldwide, royalty
+00001af0: 2d66 7265 652c 0a20 2020 2020 2020 2020  -free,.         
+00001b00: 206e 6f6e 2d73 7562 6c69 6365 6e73 6162   non-sublicensab
+00001b10: 6c65 2c20 6e6f 6e2d 6578 636c 7573 6976  le, non-exclusiv
+00001b20: 652c 2069 7272 6576 6f63 6162 6c65 206c  e, irrevocable l
+00001b30: 6963 656e 7365 2074 6f0a 2020 2020 2020  icense to.      
+00001b40: 2020 2020 6578 6572 6369 7365 2074 6865      exercise the
+00001b50: 204c 6963 656e 7365 6420 5269 6768 7473   Licensed Rights
+00001b60: 2069 6e20 7468 6520 4c69 6365 6e73 6564   in the Licensed
+00001b70: 204d 6174 6572 6961 6c20 746f 3a0a 0a20   Material to:.. 
+00001b80: 2020 2020 2020 2020 2020 2061 2e20 7265             a. re
+00001b90: 7072 6f64 7563 6520 616e 6420 5368 6172  produce and Shar
+00001ba0: 6520 7468 6520 4c69 6365 6e73 6564 204d  e the Licensed M
+00001bb0: 6174 6572 6961 6c2c 2069 6e20 7768 6f6c  aterial, in whol
+00001bc0: 6520 6f72 0a20 2020 2020 2020 2020 2020  e or.           
+00001bd0: 2020 2020 696e 2070 6172 742c 2066 6f72      in part, for
+00001be0: 204e 6f6e 436f 6d6d 6572 6369 616c 2070   NonCommercial p
+00001bf0: 7572 706f 7365 7320 6f6e 6c79 3b20 616e  urposes only; an
+00001c00: 640a 0a20 2020 2020 2020 2020 2020 2062  d..            b
+00001c10: 2e20 7072 6f64 7563 6520 616e 6420 7265  . produce and re
+00001c20: 7072 6f64 7563 652c 2062 7574 206e 6f74  produce, but not
+00001c30: 2053 6861 7265 2c20 4164 6170 7465 6420   Share, Adapted 
+00001c40: 4d61 7465 7269 616c 0a20 2020 2020 2020  Material.       
+00001c50: 2020 2020 2020 2020 666f 7220 4e6f 6e43          for NonC
+00001c60: 6f6d 6d65 7263 6961 6c20 7075 7270 6f73  ommercial purpos
+00001c70: 6573 206f 6e6c 792e 0a0a 2020 2020 2020  es only...      
+00001c80: 2032 2e20 4578 6365 7074 696f 6e73 2061   2. Exceptions a
+00001c90: 6e64 204c 696d 6974 6174 696f 6e73 2e20  nd Limitations. 
+00001ca0: 466f 7220 7468 6520 6176 6f69 6461 6e63  For the avoidanc
+00001cb0: 6520 6f66 2064 6f75 6274 2c20 7768 6572  e of doubt, wher
+00001cc0: 650a 2020 2020 2020 2020 2020 4578 6365  e.          Exce
+00001cd0: 7074 696f 6e73 2061 6e64 204c 696d 6974  ptions and Limit
+00001ce0: 6174 696f 6e73 2061 7070 6c79 2074 6f20  ations apply to 
+00001cf0: 596f 7572 2075 7365 2c20 7468 6973 2050  Your use, this P
+00001d00: 7562 6c69 630a 2020 2020 2020 2020 2020  ublic.          
+00001d10: 4c69 6365 6e73 6520 646f 6573 206e 6f74  License does not
+00001d20: 2061 7070 6c79 2c20 616e 6420 596f 7520   apply, and You 
+00001d30: 646f 206e 6f74 206e 6565 6420 746f 2063  do not need to c
+00001d40: 6f6d 706c 7920 7769 7468 0a20 2020 2020  omply with.     
+00001d50: 2020 2020 2069 7473 2074 6572 6d73 2061       its terms a
+00001d60: 6e64 2063 6f6e 6469 7469 6f6e 732e 0a0a  nd conditions...
+00001d70: 2020 2020 2020 2033 2e20 5465 726d 2e20         3. Term. 
+00001d80: 5468 6520 7465 726d 206f 6620 7468 6973  The term of this
+00001d90: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00001da0: 6973 2073 7065 6369 6669 6564 2069 6e20  is specified in 
+00001db0: 5365 6374 696f 6e0a 2020 2020 2020 2020  Section.        
+00001dc0: 2020 3628 6129 2e0a 0a20 2020 2020 2020    6(a)...       
+00001dd0: 342e 204d 6564 6961 2061 6e64 2066 6f72  4. Media and for
+00001de0: 6d61 7473 3b20 7465 6368 6e69 6361 6c20  mats; technical 
+00001df0: 6d6f 6469 6669 6361 7469 6f6e 7320 616c  modifications al
+00001e00: 6c6f 7765 642e 2054 6865 0a20 2020 2020  lowed. The.     
+00001e10: 2020 2020 204c 6963 656e 736f 7220 6175       Licensor au
+00001e20: 7468 6f72 697a 6573 2059 6f75 2074 6f20  thorizes You to 
+00001e30: 6578 6572 6369 7365 2074 6865 204c 6963  exercise the Lic
+00001e40: 656e 7365 6420 5269 6768 7473 2069 6e0a  ensed Rights in.
+00001e50: 2020 2020 2020 2020 2020 616c 6c20 6d65            all me
+00001e60: 6469 6120 616e 6420 666f 726d 6174 7320  dia and formats 
+00001e70: 7768 6574 6865 7220 6e6f 7720 6b6e 6f77  whether now know
+00001e80: 6e20 6f72 2068 6572 6561 6674 6572 2063  n or hereafter c
+00001e90: 7265 6174 6564 2c0a 2020 2020 2020 2020  reated,.        
+00001ea0: 2020 616e 6420 746f 206d 616b 6520 7465    and to make te
+00001eb0: 6368 6e69 6361 6c20 6d6f 6469 6669 6361  chnical modifica
+00001ec0: 7469 6f6e 7320 6e65 6365 7373 6172 7920  tions necessary 
+00001ed0: 746f 2064 6f20 736f 2e20 5468 650a 2020  to do so. The.  
+00001ee0: 2020 2020 2020 2020 4c69 6365 6e73 6f72          Licensor
+00001ef0: 2077 6169 7665 7320 616e 642f 6f72 2061   waives and/or a
+00001f00: 6772 6565 7320 6e6f 7420 746f 2061 7373  grees not to ass
+00001f10: 6572 7420 616e 7920 7269 6768 7420 6f72  ert any right or
+00001f20: 0a20 2020 2020 2020 2020 2061 7574 686f  .          autho
+00001f30: 7269 7479 2074 6f20 666f 7262 6964 2059  rity to forbid Y
+00001f40: 6f75 2066 726f 6d20 6d61 6b69 6e67 2074  ou from making t
+00001f50: 6563 686e 6963 616c 206d 6f64 6966 6963  echnical modific
+00001f60: 6174 696f 6e73 0a20 2020 2020 2020 2020  ations.         
+00001f70: 206e 6563 6573 7361 7279 2074 6f20 6578   necessary to ex
+00001f80: 6572 6369 7365 2074 6865 204c 6963 656e  ercise the Licen
+00001f90: 7365 6420 5269 6768 7473 2c20 696e 636c  sed Rights, incl
+00001fa0: 7564 696e 670a 2020 2020 2020 2020 2020  uding.          
+00001fb0: 7465 6368 6e69 6361 6c20 6d6f 6469 6669  technical modifi
+00001fc0: 6361 7469 6f6e 7320 6e65 6365 7373 6172  cations necessar
+00001fd0: 7920 746f 2063 6972 6375 6d76 656e 7420  y to circumvent 
+00001fe0: 4566 6665 6374 6976 650a 2020 2020 2020  Effective.      
+00001ff0: 2020 2020 5465 6368 6e6f 6c6f 6769 6361      Technologica
+00002000: 6c20 4d65 6173 7572 6573 2e20 466f 7220  l Measures. For 
+00002010: 7075 7270 6f73 6573 206f 6620 7468 6973  purposes of this
+00002020: 2050 7562 6c69 6320 4c69 6365 6e73 652c   Public License,
+00002030: 0a20 2020 2020 2020 2020 2073 696d 706c  .          simpl
+00002040: 7920 6d61 6b69 6e67 206d 6f64 6966 6963  y making modific
+00002050: 6174 696f 6e73 2061 7574 686f 7269 7a65  ations authorize
+00002060: 6420 6279 2074 6869 7320 5365 6374 696f  d by this Sectio
+00002070: 6e20 3228 6129 0a20 2020 2020 2020 2020  n 2(a).         
+00002080: 2028 3429 206e 6576 6572 2070 726f 6475   (4) never produ
+00002090: 6365 7320 4164 6170 7465 6420 4d61 7465  ces Adapted Mate
+000020a0: 7269 616c 2e0a 0a20 2020 2020 2020 352e  rial...       5.
+000020b0: 2044 6f77 6e73 7472 6561 6d20 7265 6369   Downstream reci
+000020c0: 7069 656e 7473 2e0a 0a20 2020 2020 2020  pients...       
+000020d0: 2020 2020 2061 2e20 4f66 6665 7220 6672       a. Offer fr
+000020e0: 6f6d 2074 6865 204c 6963 656e 736f 7220  om the Licensor 
+000020f0: 2d2d 204c 6963 656e 7365 6420 4d61 7465  -- Licensed Mate
+00002100: 7269 616c 2e20 4576 6572 790a 2020 2020  rial. Every.    
+00002110: 2020 2020 2020 2020 2020 2072 6563 6970             recip
+00002120: 6965 6e74 206f 6620 7468 6520 4c69 6365  ient of the Lice
+00002130: 6e73 6564 204d 6174 6572 6961 6c20 6175  nsed Material au
+00002140: 746f 6d61 7469 6361 6c6c 790a 2020 2020  tomatically.    
+00002150: 2020 2020 2020 2020 2020 2072 6563 6569             recei
+00002160: 7665 7320 616e 206f 6666 6572 2066 726f  ves an offer fro
+00002170: 6d20 7468 6520 4c69 6365 6e73 6f72 2074  m the Licensor t
+00002180: 6f20 6578 6572 6369 7365 2074 6865 0a20  o exercise the. 
+00002190: 2020 2020 2020 2020 2020 2020 2020 4c69                Li
+000021a0: 6365 6e73 6564 2052 6967 6874 7320 756e  censed Rights un
+000021b0: 6465 7220 7468 6520 7465 726d 7320 616e  der the terms an
+000021c0: 6420 636f 6e64 6974 696f 6e73 206f 6620  d conditions of 
+000021d0: 7468 6973 0a20 2020 2020 2020 2020 2020  this.           
+000021e0: 2020 2020 5075 626c 6963 204c 6963 656e      Public Licen
+000021f0: 7365 2e0a 0a20 2020 2020 2020 2020 2020  se...           
+00002200: 2062 2e20 4e6f 2064 6f77 6e73 7472 6561   b. No downstrea
+00002210: 6d20 7265 7374 7269 6374 696f 6e73 2e20  m restrictions. 
+00002220: 596f 7520 6d61 7920 6e6f 7420 6f66 6665  You may not offe
+00002230: 7220 6f72 2069 6d70 6f73 650a 2020 2020  r or impose.    
+00002240: 2020 2020 2020 2020 2020 2061 6e79 2061             any a
+00002250: 6464 6974 696f 6e61 6c20 6f72 2064 6966  dditional or dif
+00002260: 6665 7265 6e74 2074 6572 6d73 206f 7220  ferent terms or 
+00002270: 636f 6e64 6974 696f 6e73 206f 6e2c 206f  conditions on, o
+00002280: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00002290: 2061 7070 6c79 2061 6e79 2045 6666 6563   apply any Effec
+000022a0: 7469 7665 2054 6563 686e 6f6c 6f67 6963  tive Technologic
+000022b0: 616c 204d 6561 7375 7265 7320 746f 2c20  al Measures to, 
+000022c0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+000022d0: 2020 204c 6963 656e 7365 6420 4d61 7465     Licensed Mate
+000022e0: 7269 616c 2069 6620 646f 696e 6720 736f  rial if doing so
+000022f0: 2072 6573 7472 6963 7473 2065 7865 7263   restricts exerc
+00002300: 6973 6520 6f66 2074 6865 0a20 2020 2020  ise of the.     
+00002310: 2020 2020 2020 2020 2020 4c69 6365 6e73            Licens
+00002320: 6564 2052 6967 6874 7320 6279 2061 6e79  ed Rights by any
+00002330: 2072 6563 6970 6965 6e74 206f 6620 7468   recipient of th
+00002340: 6520 4c69 6365 6e73 6564 0a20 2020 2020  e Licensed.     
+00002350: 2020 2020 2020 2020 2020 4d61 7465 7269            Materi
+00002360: 616c 2e0a 0a20 2020 2020 2020 362e 204e  al...       6. N
+00002370: 6f20 656e 646f 7273 656d 656e 742e 204e  o endorsement. N
+00002380: 6f74 6869 6e67 2069 6e20 7468 6973 2050  othing in this P
+00002390: 7562 6c69 6320 4c69 6365 6e73 6520 636f  ublic License co
+000023a0: 6e73 7469 7475 7465 7320 6f72 0a20 2020  nstitutes or.   
+000023b0: 2020 2020 2020 206d 6179 2062 6520 636f         may be co
+000023c0: 6e73 7472 7565 6420 6173 2070 6572 6d69  nstrued as permi
+000023d0: 7373 696f 6e20 746f 2061 7373 6572 7420  ssion to assert 
+000023e0: 6f72 2069 6d70 6c79 2074 6861 7420 596f  or imply that Yo
+000023f0: 750a 2020 2020 2020 2020 2020 6172 652c  u.          are,
+00002400: 206f 7220 7468 6174 2059 6f75 7220 7573   or that Your us
+00002410: 6520 6f66 2074 6865 204c 6963 656e 7365  e of the License
+00002420: 6420 4d61 7465 7269 616c 2069 732c 2063  d Material is, c
+00002430: 6f6e 6e65 6374 6564 0a20 2020 2020 2020  onnected.       
+00002440: 2020 2077 6974 682c 206f 7220 7370 6f6e     with, or spon
+00002450: 736f 7265 642c 2065 6e64 6f72 7365 642c  sored, endorsed,
+00002460: 206f 7220 6772 616e 7465 6420 6f66 6669   or granted offi
+00002470: 6369 616c 2073 7461 7475 7320 6279 2c0a  cial status by,.
+00002480: 2020 2020 2020 2020 2020 7468 6520 4c69            the Li
+00002490: 6365 6e73 6f72 206f 7220 6f74 6865 7273  censor or others
+000024a0: 2064 6573 6967 6e61 7465 6420 746f 2072   designated to r
+000024b0: 6563 6569 7665 2061 7474 7269 6275 7469  eceive attributi
+000024c0: 6f6e 2061 730a 2020 2020 2020 2020 2020  on as.          
+000024d0: 7072 6f76 6964 6564 2069 6e20 5365 6374  provided in Sect
+000024e0: 696f 6e20 3328 6129 2831 2928 4129 2869  ion 3(a)(1)(A)(i
+000024f0: 292e 0a0a 2020 622e 204f 7468 6572 2072  )...  b. Other r
+00002500: 6967 6874 732e 0a0a 2020 2020 2020 2031  ights...       1
+00002510: 2e20 4d6f 7261 6c20 7269 6768 7473 2c20  . Moral rights, 
+00002520: 7375 6368 2061 7320 7468 6520 7269 6768  such as the righ
+00002530: 7420 6f66 2069 6e74 6567 7269 7479 2c20  t of integrity, 
+00002540: 6172 6520 6e6f 740a 2020 2020 2020 2020  are not.        
+00002550: 2020 6c69 6365 6e73 6564 2075 6e64 6572    licensed under
+00002560: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
+00002570: 656e 7365 2c20 6e6f 7220 6172 6520 7075  ense, nor are pu
+00002580: 626c 6963 6974 792c 0a20 2020 2020 2020  blicity,.       
+00002590: 2020 2070 7269 7661 6379 2c20 616e 642f     privacy, and/
+000025a0: 6f72 206f 7468 6572 2073 696d 696c 6172  or other similar
+000025b0: 2070 6572 736f 6e61 6c69 7479 2072 6967   personality rig
+000025c0: 6874 733b 2068 6f77 6576 6572 2c20 746f  hts; however, to
+000025d0: 0a20 2020 2020 2020 2020 2074 6865 2065  .          the e
+000025e0: 7874 656e 7420 706f 7373 6962 6c65 2c20  xtent possible, 
+000025f0: 7468 6520 4c69 6365 6e73 6f72 2077 6169  the Licensor wai
+00002600: 7665 7320 616e 642f 6f72 2061 6772 6565  ves and/or agree
+00002610: 7320 6e6f 7420 746f 0a20 2020 2020 2020  s not to.       
+00002620: 2020 2061 7373 6572 7420 616e 7920 7375     assert any su
+00002630: 6368 2072 6967 6874 7320 6865 6c64 2062  ch rights held b
+00002640: 7920 7468 6520 4c69 6365 6e73 6f72 2074  y the Licensor t
+00002650: 6f20 7468 6520 6c69 6d69 7465 640a 2020  o the limited.  
+00002660: 2020 2020 2020 2020 6578 7465 6e74 206e          extent n
+00002670: 6563 6573 7361 7279 2074 6f20 616c 6c6f  ecessary to allo
+00002680: 7720 596f 7520 746f 2065 7865 7263 6973  w You to exercis
+00002690: 6520 7468 6520 4c69 6365 6e73 6564 0a20  e the Licensed. 
+000026a0: 2020 2020 2020 2020 2052 6967 6874 732c           Rights,
+000026b0: 2062 7574 206e 6f74 206f 7468 6572 7769   but not otherwi
+000026c0: 7365 2e0a 0a20 2020 2020 2020 322e 2050  se...       2. P
+000026d0: 6174 656e 7420 616e 6420 7472 6164 656d  atent and tradem
+000026e0: 6172 6b20 7269 6768 7473 2061 7265 206e  ark rights are n
+000026f0: 6f74 206c 6963 656e 7365 6420 756e 6465  ot licensed unde
+00002700: 7220 7468 6973 0a20 2020 2020 2020 2020  r this.         
+00002710: 2050 7562 6c69 6320 4c69 6365 6e73 652e   Public License.
+00002720: 0a0a 2020 2020 2020 2033 2e20 546f 2074  ..       3. To t
+00002730: 6865 2065 7874 656e 7420 706f 7373 6962  he extent possib
+00002740: 6c65 2c20 7468 6520 4c69 6365 6e73 6f72  le, the Licensor
+00002750: 2077 6169 7665 7320 616e 7920 7269 6768   waives any righ
+00002760: 7420 746f 0a20 2020 2020 2020 2020 2063  t to.          c
+00002770: 6f6c 6c65 6374 2072 6f79 616c 7469 6573  ollect royalties
+00002780: 2066 726f 6d20 596f 7520 666f 7220 7468   from You for th
+00002790: 6520 6578 6572 6369 7365 206f 6620 7468  e exercise of th
+000027a0: 6520 4c69 6365 6e73 6564 0a20 2020 2020  e Licensed.     
+000027b0: 2020 2020 2052 6967 6874 732c 2077 6865       Rights, whe
+000027c0: 7468 6572 2064 6972 6563 746c 7920 6f72  ther directly or
+000027d0: 2074 6872 6f75 6768 2061 2063 6f6c 6c65   through a colle
+000027e0: 6374 696e 6720 736f 6369 6574 790a 2020  cting society.  
+000027f0: 2020 2020 2020 2020 756e 6465 7220 616e          under an
+00002800: 7920 766f 6c75 6e74 6172 7920 6f72 2077  y voluntary or w
+00002810: 6169 7661 626c 6520 7374 6174 7574 6f72  aivable statutor
+00002820: 7920 6f72 2063 6f6d 7075 6c73 6f72 790a  y or compulsory.
+00002830: 2020 2020 2020 2020 2020 6c69 6365 6e73            licens
+00002840: 696e 6720 7363 6865 6d65 2e20 496e 2061  ing scheme. In a
+00002850: 6c6c 206f 7468 6572 2063 6173 6573 2074  ll other cases t
+00002860: 6865 204c 6963 656e 736f 7220 6578 7072  he Licensor expr
+00002870: 6573 736c 790a 2020 2020 2020 2020 2020  essly.          
+00002880: 7265 7365 7276 6573 2061 6e79 2072 6967  reserves any rig
+00002890: 6874 2074 6f20 636f 6c6c 6563 7420 7375  ht to collect su
+000028a0: 6368 2072 6f79 616c 7469 6573 2c20 696e  ch royalties, in
+000028b0: 636c 7564 696e 6720 7768 656e 0a20 2020  cluding when.   
+000028c0: 2020 2020 2020 2074 6865 204c 6963 656e         the Licen
+000028d0: 7365 6420 4d61 7465 7269 616c 2069 7320  sed Material is 
+000028e0: 7573 6564 206f 7468 6572 2074 6861 6e20  used other than 
+000028f0: 666f 7220 4e6f 6e43 6f6d 6d65 7263 6961  for NonCommercia
+00002900: 6c0a 2020 2020 2020 2020 2020 7075 7270  l.          purp
+00002910: 6f73 6573 2e0a 0a0a 5365 6374 696f 6e20  oses....Section 
+00002920: 3320 2d2d 204c 6963 656e 7365 2043 6f6e  3 -- License Con
+00002930: 6469 7469 6f6e 732e 0a2d 2d2d 2d2d 2d2d  ditions..-------
+00002940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00002950: 2d2d 2d2d 2d2d 2d2d 2d0a 0a59 6f75 7220  ---------..Your 
+00002960: 6578 6572 6369 7365 206f 6620 7468 6520  exercise of the 
+00002970: 4c69 6365 6e73 6564 2052 6967 6874 7320  Licensed Rights 
+00002980: 6973 2065 7870 7265 7373 6c79 206d 6164  is expressly mad
+00002990: 6520 7375 626a 6563 7420 746f 2074 6865  e subject to the
+000029a0: 0a66 6f6c 6c6f 7769 6e67 2063 6f6e 6469  .following condi
+000029b0: 7469 6f6e 732e 0a0a 2020 612e 2041 7474  tions...  a. Att
+000029c0: 7269 6275 7469 6f6e 2e0a 0a20 2020 2020  ribution...     
+000029d0: 2020 312e 2049 6620 596f 7520 5368 6172    1. If You Shar
+000029e0: 6520 7468 6520 4c69 6365 6e73 6564 204d  e the Licensed M
+000029f0: 6174 6572 6961 6c2c 2059 6f75 206d 7573  aterial, You mus
+00002a00: 743a 0a0a 2020 2020 2020 2020 2020 2020  t:..            
+00002a10: 612e 2072 6574 6169 6e20 7468 6520 666f  a. retain the fo
+00002a20: 6c6c 6f77 696e 6720 6966 2069 7420 6973  llowing if it is
+00002a30: 2073 7570 706c 6965 6420 6279 2074 6865   supplied by the
+00002a40: 204c 6963 656e 736f 720a 2020 2020 2020   Licensor.      
+00002a50: 2020 2020 2020 2020 2077 6974 6820 7468           with th
+00002a60: 6520 4c69 6365 6e73 6564 204d 6174 6572  e Licensed Mater
+00002a70: 6961 6c3a 0a0a 2020 2020 2020 2020 2020  ial:..          
+00002a80: 2020 2020 2020 2069 2e20 6964 656e 7469         i. identi
+00002a90: 6669 6361 7469 6f6e 206f 6620 7468 6520  fication of the 
+00002aa0: 6372 6561 746f 7228 7329 206f 6620 7468  creator(s) of th
+00002ab0: 6520 4c69 6365 6e73 6564 0a20 2020 2020  e Licensed.     
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 204d                 M
+00002ad0: 6174 6572 6961 6c20 616e 6420 616e 7920  aterial and any 
+00002ae0: 6f74 6865 7273 2064 6573 6967 6e61 7465  others designate
+00002af0: 6420 746f 2072 6563 6569 7665 0a20 2020  d to receive.   
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2061 7474 7269 6275 7469 6f6e 2c20 696e   attribution, in
+00002b20: 2061 6e79 2072 6561 736f 6e61 626c 6520   any reasonable 
+00002b30: 6d61 6e6e 6572 2072 6571 7565 7374 6564  manner requested
+00002b40: 2062 790a 2020 2020 2020 2020 2020 2020   by.            
+00002b50: 2020 2020 2020 2020 7468 6520 4c69 6365          the Lice
+00002b60: 6e73 6f72 2028 696e 636c 7564 696e 6720  nsor (including 
+00002b70: 6279 2070 7365 7564 6f6e 796d 2069 660a  by pseudonym if.
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b90: 2020 2020 6465 7369 676e 6174 6564 293b      designated);
+00002ba0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002bb0: 2020 6969 2e20 6120 636f 7079 7269 6768    ii. a copyrigh
+00002bc0: 7420 6e6f 7469 6365 3b0a 0a20 2020 2020  t notice;..     
+00002bd0: 2020 2020 2020 2020 2020 6969 692e 2061            iii. a
+00002be0: 206e 6f74 6963 6520 7468 6174 2072 6566   notice that ref
+00002bf0: 6572 7320 746f 2074 6869 7320 5075 626c  ers to this Publ
+00002c00: 6963 204c 6963 656e 7365 3b0a 0a20 2020  ic License;..   
+00002c10: 2020 2020 2020 2020 2020 2020 2069 762e               iv.
+00002c20: 2061 206e 6f74 6963 6520 7468 6174 2072   a notice that r
+00002c30: 6566 6572 7320 746f 2074 6865 2064 6973  efers to the dis
+00002c40: 636c 6169 6d65 7220 6f66 0a20 2020 2020  claimer of.     
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00002c60: 6172 7261 6e74 6965 733b 0a0a 2020 2020  arranties;..    
+00002c70: 2020 2020 2020 2020 2020 2020 2076 2e20               v. 
+00002c80: 6120 5552 4920 6f72 2068 7970 6572 6c69  a URI or hyperli
+00002c90: 6e6b 2074 6f20 7468 6520 4c69 6365 6e73  nk to the Licens
+00002ca0: 6564 204d 6174 6572 6961 6c20 746f 2074  ed Material to t
+00002cb0: 6865 0a20 2020 2020 2020 2020 2020 2020  he.             
+00002cc0: 2020 2020 2020 2065 7874 656e 7420 7265         extent re
+00002cd0: 6173 6f6e 6162 6c79 2070 7261 6374 6963  asonably practic
+00002ce0: 6162 6c65 3b0a 0a20 2020 2020 2020 2020  able;..         
+00002cf0: 2020 2062 2e20 696e 6469 6361 7465 2069     b. indicate i
+00002d00: 6620 596f 7520 6d6f 6469 6669 6564 2074  f You modified t
+00002d10: 6865 204c 6963 656e 7365 6420 4d61 7465  he Licensed Mate
+00002d20: 7269 616c 2061 6e64 0a20 2020 2020 2020  rial and.       
+00002d30: 2020 2020 2020 2020 7265 7461 696e 2061          retain a
+00002d40: 6e20 696e 6469 6361 7469 6f6e 206f 6620  n indication of 
+00002d50: 616e 7920 7072 6576 696f 7573 206d 6f64  any previous mod
+00002d60: 6966 6963 6174 696f 6e73 3b20 616e 640a  ifications; and.
+00002d70: 0a20 2020 2020 2020 2020 2020 2063 2e20  .            c. 
+00002d80: 696e 6469 6361 7465 2074 6865 204c 6963  indicate the Lic
+00002d90: 656e 7365 6420 4d61 7465 7269 616c 2069  ensed Material i
+00002da0: 7320 6c69 6365 6e73 6564 2075 6e64 6572  s licensed under
+00002db0: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
+00002dc0: 2020 2020 2050 7562 6c69 6320 4c69 6365       Public Lice
+00002dd0: 6e73 652c 2061 6e64 2069 6e63 6c75 6465  nse, and include
+00002de0: 2074 6865 2074 6578 7420 6f66 2c20 6f72   the text of, or
+00002df0: 2074 6865 2055 5249 206f 720a 2020 2020   the URI or.    
+00002e00: 2020 2020 2020 2020 2020 2068 7970 6572             hyper
+00002e10: 6c69 6e6b 2074 6f2c 2074 6869 7320 5075  link to, this Pu
+00002e20: 626c 6963 204c 6963 656e 7365 2e0a 0a20  blic License... 
+00002e30: 2020 2020 2020 2020 2046 6f72 2074 6865           For the
+00002e40: 2061 766f 6964 616e 6365 206f 6620 646f   avoidance of do
+00002e50: 7562 742c 2059 6f75 2064 6f20 6e6f 7420  ubt, You do not 
+00002e60: 6861 7665 2070 6572 6d69 7373 696f 6e20  have permission 
+00002e70: 756e 6465 720a 2020 2020 2020 2020 2020  under.          
+00002e80: 7468 6973 2050 7562 6c69 6320 4c69 6365  this Public Lice
+00002e90: 6e73 6520 746f 2053 6861 7265 2041 6461  nse to Share Ada
+00002ea0: 7074 6564 204d 6174 6572 6961 6c2e 0a0a  pted Material...
+00002eb0: 2020 2020 2020 2032 2e20 596f 7520 6d61         2. You ma
+00002ec0: 7920 7361 7469 7366 7920 7468 6520 636f  y satisfy the co
+00002ed0: 6e64 6974 696f 6e73 2069 6e20 5365 6374  nditions in Sect
+00002ee0: 696f 6e20 3328 6129 2831 2920 696e 2061  ion 3(a)(1) in a
+00002ef0: 6e79 0a20 2020 2020 2020 2020 2072 6561  ny.          rea
+00002f00: 736f 6e61 626c 6520 6d61 6e6e 6572 2062  sonable manner b
+00002f10: 6173 6564 206f 6e20 7468 6520 6d65 6469  ased on the medi
+00002f20: 756d 2c20 6d65 616e 732c 2061 6e64 2063  um, means, and c
+00002f30: 6f6e 7465 7874 2069 6e0a 2020 2020 2020  ontext in.      
+00002f40: 2020 2020 7768 6963 6820 596f 7520 5368      which You Sh
+00002f50: 6172 6520 7468 6520 4c69 6365 6e73 6564  are the Licensed
+00002f60: 204d 6174 6572 6961 6c2e 2046 6f72 2065   Material. For e
+00002f70: 7861 6d70 6c65 2c20 6974 206d 6179 2062  xample, it may b
+00002f80: 650a 2020 2020 2020 2020 2020 7265 6173  e.          reas
+00002f90: 6f6e 6162 6c65 2074 6f20 7361 7469 7366  onable to satisf
+00002fa0: 7920 7468 6520 636f 6e64 6974 696f 6e73  y the conditions
+00002fb0: 2062 7920 7072 6f76 6964 696e 6720 6120   by providing a 
+00002fc0: 5552 4920 6f72 0a20 2020 2020 2020 2020  URI or.         
+00002fd0: 2068 7970 6572 6c69 6e6b 2074 6f20 6120   hyperlink to a 
+00002fe0: 7265 736f 7572 6365 2074 6861 7420 696e  resource that in
+00002ff0: 636c 7564 6573 2074 6865 2072 6571 7569  cludes the requi
+00003000: 7265 640a 2020 2020 2020 2020 2020 696e  red.          in
+00003010: 666f 726d 6174 696f 6e2e 0a0a 2020 2020  formation...    
+00003020: 2020 2033 2e20 4966 2072 6571 7565 7374     3. If request
+00003030: 6564 2062 7920 7468 6520 4c69 6365 6e73  ed by the Licens
+00003040: 6f72 2c20 596f 7520 6d75 7374 2072 656d  or, You must rem
+00003050: 6f76 6520 616e 7920 6f66 2074 6865 0a20  ove any of the. 
+00003060: 2020 2020 2020 2020 2069 6e66 6f72 6d61           informa
+00003070: 7469 6f6e 2072 6571 7569 7265 6420 6279  tion required by
+00003080: 2053 6563 7469 6f6e 2033 2861 2928 3129   Section 3(a)(1)
+00003090: 2841 2920 746f 2074 6865 2065 7874 656e  (A) to the exten
+000030a0: 740a 2020 2020 2020 2020 2020 7265 6173  t.          reas
+000030b0: 6f6e 6162 6c79 2070 7261 6374 6963 6162  onably practicab
+000030c0: 6c65 2e0a 0a0a 5365 6374 696f 6e20 3420  le....Section 4 
+000030d0: 2d2d 2053 7569 2047 656e 6572 6973 2044  -- Sui Generis D
+000030e0: 6174 6162 6173 6520 5269 6768 7473 2e0a  atabase Rights..
+000030f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003110: 2d2d 2d2d 2d2d 2d2d 2d0a 0a57 6865 7265  ---------..Where
+00003120: 2074 6865 204c 6963 656e 7365 6420 5269   the Licensed Ri
+00003130: 6768 7473 2069 6e63 6c75 6465 2053 7569  ghts include Sui
+00003140: 2047 656e 6572 6973 2044 6174 6162 6173   Generis Databas
+00003150: 6520 5269 6768 7473 2074 6861 740a 6170  e Rights that.ap
+00003160: 706c 7920 746f 2059 6f75 7220 7573 6520  ply to Your use 
+00003170: 6f66 2074 6865 204c 6963 656e 7365 6420  of the Licensed 
+00003180: 4d61 7465 7269 616c 3a0a 0a20 2061 2e20  Material:..  a. 
+00003190: 666f 7220 7468 6520 6176 6f69 6461 6e63  for the avoidanc
+000031a0: 6520 6f66 2064 6f75 6274 2c20 5365 6374  e of doubt, Sect
+000031b0: 696f 6e20 3228 6129 2831 2920 6772 616e  ion 2(a)(1) gran
+000031c0: 7473 2059 6f75 2074 6865 2072 6967 6874  ts You the right
+000031d0: 0a20 2020 2020 746f 2065 7874 7261 6374  .     to extract
+000031e0: 2c20 7265 7573 652c 2072 6570 726f 6475  , reuse, reprodu
+000031f0: 6365 2c20 616e 6420 5368 6172 6520 616c  ce, and Share al
+00003200: 6c20 6f72 2061 2073 7562 7374 616e 7469  l or a substanti
+00003210: 616c 0a20 2020 2020 706f 7274 696f 6e20  al.     portion 
+00003220: 6f66 2074 6865 2063 6f6e 7465 6e74 7320  of the contents 
+00003230: 6f66 2074 6865 2064 6174 6162 6173 6520  of the database 
+00003240: 666f 7220 4e6f 6e43 6f6d 6d65 7263 6961  for NonCommercia
+00003250: 6c20 7075 7270 6f73 6573 0a20 2020 2020  l purposes.     
+00003260: 6f6e 6c79 2061 6e64 2070 726f 7669 6465  only and provide
+00003270: 6420 596f 7520 646f 206e 6f74 2053 6861  d You do not Sha
+00003280: 7265 2041 6461 7074 6564 204d 6174 6572  re Adapted Mater
+00003290: 6961 6c3b 0a0a 2020 622e 2069 6620 596f  ial;..  b. if Yo
+000032a0: 7520 696e 636c 7564 6520 616c 6c20 6f72  u include all or
+000032b0: 2061 2073 7562 7374 616e 7469 616c 2070   a substantial p
+000032c0: 6f72 7469 6f6e 206f 6620 7468 6520 6461  ortion of the da
+000032d0: 7461 6261 7365 0a20 2020 2020 636f 6e74  tabase.     cont
+000032e0: 656e 7473 2069 6e20 6120 6461 7461 6261  ents in a databa
+000032f0: 7365 2069 6e20 7768 6963 6820 596f 7520  se in which You 
+00003300: 6861 7665 2053 7569 2047 656e 6572 6973  have Sui Generis
+00003310: 2044 6174 6162 6173 650a 2020 2020 2052   Database.     R
+00003320: 6967 6874 732c 2074 6865 6e20 7468 6520  ights, then the 
+00003330: 6461 7461 6261 7365 2069 6e20 7768 6963  database in whic
+00003340: 6820 596f 7520 6861 7665 2053 7569 2047  h You have Sui G
+00003350: 656e 6572 6973 2044 6174 6162 6173 650a  eneris Database.
+00003360: 2020 2020 2052 6967 6874 7320 2862 7574       Rights (but
+00003370: 206e 6f74 2069 7473 2069 6e64 6976 6964   not its individ
+00003380: 7561 6c20 636f 6e74 656e 7473 2920 6973  ual contents) is
+00003390: 2041 6461 7074 6564 204d 6174 6572 6961   Adapted Materia
+000033a0: 6c3b 2061 6e64 0a0a 2020 632e 2059 6f75  l; and..  c. You
+000033b0: 206d 7573 7420 636f 6d70 6c79 2077 6974   must comply wit
+000033c0: 6820 7468 6520 636f 6e64 6974 696f 6e73  h the conditions
+000033d0: 2069 6e20 5365 6374 696f 6e20 3328 6129   in Section 3(a)
+000033e0: 2069 6620 596f 7520 5368 6172 650a 2020   if You Share.  
+000033f0: 2020 2061 6c6c 206f 7220 6120 7375 6273     all or a subs
+00003400: 7461 6e74 6961 6c20 706f 7274 696f 6e20  tantial portion 
+00003410: 6f66 2074 6865 2063 6f6e 7465 6e74 7320  of the contents 
+00003420: 6f66 2074 6865 2064 6174 6162 6173 652e  of the database.
+00003430: 0a0a 466f 7220 7468 6520 6176 6f69 6461  ..For the avoida
+00003440: 6e63 6520 6f66 2064 6f75 6274 2c20 7468  nce of doubt, th
+00003450: 6973 2053 6563 7469 6f6e 2034 2073 7570  is Section 4 sup
+00003460: 706c 656d 656e 7473 2061 6e64 2064 6f65  plements and doe
+00003470: 7320 6e6f 740a 7265 706c 6163 6520 596f  s not.replace Yo
+00003480: 7572 206f 626c 6967 6174 696f 6e73 2075  ur obligations u
+00003490: 6e64 6572 2074 6869 7320 5075 626c 6963  nder this Public
+000034a0: 204c 6963 656e 7365 2077 6865 7265 2074   License where t
+000034b0: 6865 204c 6963 656e 7365 640a 5269 6768  he Licensed.Righ
+000034c0: 7473 2069 6e63 6c75 6465 206f 7468 6572  ts include other
+000034d0: 2043 6f70 7972 6967 6874 2061 6e64 2053   Copyright and S
+000034e0: 696d 696c 6172 2052 6967 6874 732e 0a0a  imilar Rights...
+000034f0: 0a53 6563 7469 6f6e 2035 202d 2d20 4469  .Section 5 -- Di
+00003500: 7363 6c61 696d 6572 206f 6620 5761 7272  sclaimer of Warr
+00003510: 616e 7469 6573 2061 6e64 204c 696d 6974  anties and Limit
+00003520: 6174 696f 6e20 6f66 204c 6961 6269 6c69  ation of Liabili
+00003530: 7479 2e0a 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ty..------------
+00003540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003570: 2d2d 2d2d 2d2d 0a0a 2020 612e 2055 4e4c  ------..  a. UNL
+00003580: 4553 5320 4f54 4845 5257 4953 4520 5345  ESS OTHERWISE SE
+00003590: 5041 5241 5445 4c59 2055 4e44 4552 5441  PARATELY UNDERTA
+000035a0: 4b45 4e20 4259 2054 4845 204c 4943 454e  KEN BY THE LICEN
+000035b0: 534f 522c 2054 4f20 5448 450a 2020 2020  SOR, TO THE.    
+000035c0: 2045 5854 454e 5420 504f 5353 4942 4c45   EXTENT POSSIBLE
+000035d0: 2c20 5448 4520 4c49 4345 4e53 4f52 204f  , THE LICENSOR O
+000035e0: 4646 4552 5320 5448 4520 4c49 4345 4e53  FFERS THE LICENS
+000035f0: 4544 204d 4154 4552 4941 4c20 4153 2d49  ED MATERIAL AS-I
+00003600: 530a 2020 2020 2041 4e44 2041 532d 4156  S.     AND AS-AV
+00003610: 4149 4c41 424c 452c 2041 4e44 204d 414b  AILABLE, AND MAK
+00003620: 4553 204e 4f20 5245 5052 4553 454e 5441  ES NO REPRESENTA
+00003630: 5449 4f4e 5320 4f52 2057 4152 5241 4e54  TIONS OR WARRANT
+00003640: 4945 5320 4f46 0a20 2020 2020 414e 5920  IES OF.     ANY 
+00003650: 4b49 4e44 2043 4f4e 4345 524e 494e 4720  KIND CONCERNING 
+00003660: 5448 4520 4c49 4345 4e53 4544 204d 4154  THE LICENSED MAT
+00003670: 4552 4941 4c2c 2057 4845 5448 4552 2045  ERIAL, WHETHER E
+00003680: 5850 5245 5353 2c0a 2020 2020 2049 4d50  XPRESS,.     IMP
+00003690: 4c49 4544 2c20 5354 4154 5554 4f52 592c  LIED, STATUTORY,
+000036a0: 204f 5220 4f54 4845 522e 2054 4849 5320   OR OTHER. THIS 
+000036b0: 494e 434c 5544 4553 2c20 5749 5448 4f55  INCLUDES, WITHOU
+000036c0: 5420 4c49 4d49 5441 5449 4f4e 2c0a 2020  T LIMITATION,.  
+000036d0: 2020 2057 4152 5241 4e54 4945 5320 4f46     WARRANTIES OF
+000036e0: 2054 4954 4c45 2c20 4d45 5243 4841 4e54   TITLE, MERCHANT
+000036f0: 4142 494c 4954 592c 2046 4954 4e45 5353  ABILITY, FITNESS
+00003700: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
+00003710: 520a 2020 2020 2050 5552 504f 5345 2c20  R.     PURPOSE, 
+00003720: 4e4f 4e2d 494e 4652 494e 4745 4d45 4e54  NON-INFRINGEMENT
+00003730: 2c20 4142 5345 4e43 4520 4f46 204c 4154  , ABSENCE OF LAT
+00003740: 454e 5420 4f52 204f 5448 4552 2044 4546  ENT OR OTHER DEF
+00003750: 4543 5453 2c0a 2020 2020 2041 4343 5552  ECTS,.     ACCUR
+00003760: 4143 592c 204f 5220 5448 4520 5052 4553  ACY, OR THE PRES
+00003770: 454e 4345 204f 5220 4142 5345 4e43 4520  ENCE OR ABSENCE 
+00003780: 4f46 2045 5252 4f52 532c 2057 4845 5448  OF ERRORS, WHETH
+00003790: 4552 204f 5220 4e4f 540a 2020 2020 204b  ER OR NOT.     K
+000037a0: 4e4f 574e 204f 5220 4449 5343 4f56 4552  NOWN OR DISCOVER
+000037b0: 4142 4c45 2e20 5748 4552 4520 4449 5343  ABLE. WHERE DISC
+000037c0: 4c41 494d 4552 5320 4f46 2057 4152 5241  LAIMERS OF WARRA
+000037d0: 4e54 4945 5320 4152 4520 4e4f 540a 2020  NTIES ARE NOT.  
+000037e0: 2020 2041 4c4c 4f57 4544 2049 4e20 4655     ALLOWED IN FU
+000037f0: 4c4c 204f 5220 494e 2050 4152 542c 2054  LL OR IN PART, T
+00003800: 4849 5320 4449 5343 4c41 494d 4552 204d  HIS DISCLAIMER M
+00003810: 4159 204e 4f54 2041 5050 4c59 2054 4f20  AY NOT APPLY TO 
+00003820: 594f 552e 0a0a 2020 622e 2054 4f20 5448  YOU...  b. TO TH
+00003830: 4520 4558 5445 4e54 2050 4f53 5349 424c  E EXTENT POSSIBL
+00003840: 452c 2049 4e20 4e4f 2045 5645 4e54 2057  E, IN NO EVENT W
+00003850: 494c 4c20 5448 4520 4c49 4345 4e53 4f52  ILL THE LICENSOR
+00003860: 2042 4520 4c49 4142 4c45 0a20 2020 2020   BE LIABLE.     
+00003870: 544f 2059 4f55 204f 4e20 414e 5920 4c45  TO YOU ON ANY LE
+00003880: 4741 4c20 5448 454f 5259 2028 494e 434c  GAL THEORY (INCL
+00003890: 5544 494e 472c 2057 4954 484f 5554 204c  UDING, WITHOUT L
+000038a0: 494d 4954 4154 494f 4e2c 0a20 2020 2020  IMITATION,.     
+000038b0: 4e45 474c 4947 454e 4345 2920 4f52 204f  NEGLIGENCE) OR O
+000038c0: 5448 4552 5749 5345 2046 4f52 2041 4e59  THERWISE FOR ANY
+000038d0: 2044 4952 4543 542c 2053 5045 4349 414c   DIRECT, SPECIAL
+000038e0: 2c20 494e 4449 5245 4354 2c0a 2020 2020  , INDIRECT,.    
+000038f0: 2049 4e43 4944 454e 5441 4c2c 2043 4f4e   INCIDENTAL, CON
+00003900: 5345 5155 454e 5449 414c 2c20 5055 4e49  SEQUENTIAL, PUNI
+00003910: 5449 5645 2c20 4558 454d 504c 4152 592c  TIVE, EXEMPLARY,
+00003920: 204f 5220 4f54 4845 5220 4c4f 5353 4553   OR OTHER LOSSES
+00003930: 2c0a 2020 2020 2043 4f53 5453 2c20 4558  ,.     COSTS, EX
+00003940: 5045 4e53 4553 2c20 4f52 2044 414d 4147  PENSES, OR DAMAG
+00003950: 4553 2041 5249 5349 4e47 204f 5554 204f  ES ARISING OUT O
+00003960: 4620 5448 4953 2050 5542 4c49 4320 4c49  F THIS PUBLIC LI
+00003970: 4345 4e53 4520 4f52 0a20 2020 2020 5553  CENSE OR.     US
+00003980: 4520 4f46 2054 4845 204c 4943 454e 5345  E OF THE LICENSE
+00003990: 4420 4d41 5445 5249 414c 2c20 4556 454e  D MATERIAL, EVEN
+000039a0: 2049 4620 5448 4520 4c49 4345 4e53 4f52   IF THE LICENSOR
+000039b0: 2048 4153 2042 4545 4e0a 2020 2020 2041   HAS BEEN.     A
+000039c0: 4456 4953 4544 204f 4620 5448 4520 504f  DVISED OF THE PO
+000039d0: 5353 4942 494c 4954 5920 4f46 2053 5543  SSIBILITY OF SUC
+000039e0: 4820 4c4f 5353 4553 2c20 434f 5354 532c  H LOSSES, COSTS,
+000039f0: 2045 5850 454e 5345 532c 204f 520a 2020   EXPENSES, OR.  
+00003a00: 2020 2044 414d 4147 4553 2e20 5748 4552     DAMAGES. WHER
+00003a10: 4520 4120 4c49 4d49 5441 5449 4f4e 204f  E A LIMITATION O
+00003a20: 4620 4c49 4142 494c 4954 5920 4953 204e  F LIABILITY IS N
+00003a30: 4f54 2041 4c4c 4f57 4544 2049 4e20 4655  OT ALLOWED IN FU
+00003a40: 4c4c 204f 520a 2020 2020 2049 4e20 5041  LL OR.     IN PA
+00003a50: 5254 2c20 5448 4953 204c 494d 4954 4154  RT, THIS LIMITAT
+00003a60: 494f 4e20 4d41 5920 4e4f 5420 4150 504c  ION MAY NOT APPL
+00003a70: 5920 544f 2059 4f55 2e0a 0a20 2063 2e20  Y TO YOU...  c. 
+00003a80: 5468 6520 6469 7363 6c61 696d 6572 206f  The disclaimer o
+00003a90: 6620 7761 7272 616e 7469 6573 2061 6e64  f warranties and
+00003aa0: 206c 696d 6974 6174 696f 6e20 6f66 206c   limitation of l
+00003ab0: 6961 6269 6c69 7479 2070 726f 7669 6465  iability provide
+00003ac0: 640a 2020 2020 2061 626f 7665 2073 6861  d.     above sha
+00003ad0: 6c6c 2062 6520 696e 7465 7270 7265 7465  ll be interprete
+00003ae0: 6420 696e 2061 206d 616e 6e65 7220 7468  d in a manner th
+00003af0: 6174 2c20 746f 2074 6865 2065 7874 656e  at, to the exten
+00003b00: 740a 2020 2020 2070 6f73 7369 626c 652c  t.     possible,
+00003b10: 206d 6f73 7420 636c 6f73 656c 7920 6170   most closely ap
+00003b20: 7072 6f78 696d 6174 6573 2061 6e20 6162  proximates an ab
+00003b30: 736f 6c75 7465 2064 6973 636c 6169 6d65  solute disclaime
+00003b40: 7220 616e 640a 2020 2020 2077 6169 7665  r and.     waive
+00003b50: 7220 6f66 2061 6c6c 206c 6961 6269 6c69  r of all liabili
+00003b60: 7479 2e0a 0a0a 5365 6374 696f 6e20 3620  ty....Section 6 
+00003b70: 2d2d 2054 6572 6d20 616e 6420 5465 726d  -- Term and Term
+00003b80: 696e 6174 696f 6e2e 0a2d 2d2d 2d2d 2d2d  ination..-------
+00003b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00003ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a20 2061  -----------..  a
+00003bb0: 2e20 5468 6973 2050 7562 6c69 6320 4c69  . This Public Li
+00003bc0: 6365 6e73 6520 6170 706c 6965 7320 666f  cense applies fo
+00003bd0: 7220 7468 6520 7465 726d 206f 6620 7468  r the term of th
+00003be0: 6520 436f 7079 7269 6768 7420 616e 640a  e Copyright and.
+00003bf0: 2020 2020 2053 696d 696c 6172 2052 6967       Similar Rig
+00003c00: 6874 7320 6c69 6365 6e73 6564 2068 6572  hts licensed her
+00003c10: 652e 2048 6f77 6576 6572 2c20 6966 2059  e. However, if Y
+00003c20: 6f75 2066 6169 6c20 746f 2063 6f6d 706c  ou fail to compl
+00003c30: 7920 7769 7468 0a20 2020 2020 7468 6973  y with.     this
+00003c40: 2050 7562 6c69 6320 4c69 6365 6e73 652c   Public License,
+00003c50: 2074 6865 6e20 596f 7572 2072 6967 6874   then Your right
+00003c60: 7320 756e 6465 7220 7468 6973 2050 7562  s under this Pub
+00003c70: 6c69 6320 4c69 6365 6e73 650a 2020 2020  lic License.    
+00003c80: 2074 6572 6d69 6e61 7465 2061 7574 6f6d   terminate autom
+00003c90: 6174 6963 616c 6c79 2e0a 0a20 2062 2e20  atically...  b. 
+00003ca0: 5768 6572 6520 596f 7572 2072 6967 6874  Where Your right
+00003cb0: 2074 6f20 7573 6520 7468 6520 4c69 6365   to use the Lice
+00003cc0: 6e73 6564 204d 6174 6572 6961 6c20 6861  nsed Material ha
+00003cd0: 7320 7465 726d 696e 6174 6564 2075 6e64  s terminated und
+00003ce0: 6572 0a20 2020 2020 5365 6374 696f 6e20  er.     Section 
+00003cf0: 3628 6129 2c20 6974 2072 6569 6e73 7461  6(a), it reinsta
+00003d00: 7465 733a 0a0a 2020 2020 2020 2031 2e20  tes:..       1. 
+00003d10: 6175 746f 6d61 7469 6361 6c6c 7920 6173  automatically as
+00003d20: 206f 6620 7468 6520 6461 7465 2074 6865   of the date the
+00003d30: 2076 696f 6c61 7469 6f6e 2069 7320 6375   violation is cu
+00003d40: 7265 642c 2070 726f 7669 6465 640a 2020  red, provided.  
+00003d50: 2020 2020 2020 2020 6974 2069 7320 6375          it is cu
+00003d60: 7265 6420 7769 7468 696e 2033 3020 6461  red within 30 da
+00003d70: 7973 206f 6620 596f 7572 2064 6973 636f  ys of Your disco
+00003d80: 7665 7279 206f 6620 7468 650a 2020 2020  very of the.    
+00003d90: 2020 2020 2020 7669 6f6c 6174 696f 6e3b        violation;
+00003da0: 206f 720a 0a20 2020 2020 2020 322e 2075   or..       2. u
+00003db0: 706f 6e20 6578 7072 6573 7320 7265 696e  pon express rein
+00003dc0: 7374 6174 656d 656e 7420 6279 2074 6865  statement by the
+00003dd0: 204c 6963 656e 736f 722e 0a0a 2020 2020   Licensor...    
+00003de0: 2046 6f72 2074 6865 2061 766f 6964 616e   For the avoidan
+00003df0: 6365 206f 6620 646f 7562 742c 2074 6869  ce of doubt, thi
+00003e00: 7320 5365 6374 696f 6e20 3628 6229 2064  s Section 6(b) d
+00003e10: 6f65 7320 6e6f 7420 6166 6665 6374 2061  oes not affect a
+00003e20: 6e79 0a20 2020 2020 7269 6768 7420 7468  ny.     right th
+00003e30: 6520 4c69 6365 6e73 6f72 206d 6179 2068  e Licensor may h
+00003e40: 6176 6520 746f 2073 6565 6b20 7265 6d65  ave to seek reme
+00003e50: 6469 6573 2066 6f72 2059 6f75 7220 7669  dies for Your vi
+00003e60: 6f6c 6174 696f 6e73 0a20 2020 2020 6f66  olations.     of
+00003e70: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
+00003e80: 656e 7365 2e0a 0a20 2063 2e20 466f 7220  ense...  c. For 
+00003e90: 7468 6520 6176 6f69 6461 6e63 6520 6f66  the avoidance of
+00003ea0: 2064 6f75 6274 2c20 7468 6520 4c69 6365   doubt, the Lice
+00003eb0: 6e73 6f72 206d 6179 2061 6c73 6f20 6f66  nsor may also of
+00003ec0: 6665 7220 7468 650a 2020 2020 204c 6963  fer the.     Lic
+00003ed0: 656e 7365 6420 4d61 7465 7269 616c 2075  ensed Material u
+00003ee0: 6e64 6572 2073 6570 6172 6174 6520 7465  nder separate te
+00003ef0: 726d 7320 6f72 2063 6f6e 6469 7469 6f6e  rms or condition
+00003f00: 7320 6f72 2073 746f 700a 2020 2020 2064  s or stop.     d
+00003f10: 6973 7472 6962 7574 696e 6720 7468 6520  istributing the 
+00003f20: 4c69 6365 6e73 6564 204d 6174 6572 6961  Licensed Materia
+00003f30: 6c20 6174 2061 6e79 2074 696d 653b 2068  l at any time; h
+00003f40: 6f77 6576 6572 2c20 646f 696e 6720 736f  owever, doing so
+00003f50: 0a20 2020 2020 7769 6c6c 206e 6f74 2074  .     will not t
+00003f60: 6572 6d69 6e61 7465 2074 6869 7320 5075  erminate this Pu
+00003f70: 626c 6963 204c 6963 656e 7365 2e0a 0a20  blic License... 
+00003f80: 2064 2e20 5365 6374 696f 6e73 2031 2c20   d. Sections 1, 
+00003f90: 352c 2036 2c20 372c 2061 6e64 2038 2073  5, 6, 7, and 8 s
+00003fa0: 7572 7669 7665 2074 6572 6d69 6e61 7469  urvive terminati
+00003fb0: 6f6e 206f 6620 7468 6973 2050 7562 6c69  on of this Publi
+00003fc0: 630a 2020 2020 204c 6963 656e 7365 2e0a  c.     License..
+00003fd0: 0a0a 5365 6374 696f 6e20 3720 2d2d 204f  ..Section 7 -- O
+00003fe0: 7468 6572 2054 6572 6d73 2061 6e64 2043  ther Terms and C
+00003ff0: 6f6e 6469 7469 6f6e 732e 0a2d 2d2d 2d2d  onditions..-----
+00004000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00004020: 2d2d 2d0a 0a20 2061 2e20 5468 6520 4c69  ---..  a. The Li
+00004030: 6365 6e73 6f72 2073 6861 6c6c 206e 6f74  censor shall not
+00004040: 2062 6520 626f 756e 6420 6279 2061 6e79   be bound by any
+00004050: 2061 6464 6974 696f 6e61 6c20 6f72 2064   additional or d
+00004060: 6966 6665 7265 6e74 0a20 2020 2020 7465  ifferent.     te
+00004070: 726d 7320 6f72 2063 6f6e 6469 7469 6f6e  rms or condition
+00004080: 7320 636f 6d6d 756e 6963 6174 6564 2062  s communicated b
+00004090: 7920 596f 7520 756e 6c65 7373 2065 7870  y You unless exp
+000040a0: 7265 7373 6c79 2061 6772 6565 642e 0a0a  ressly agreed...
+000040b0: 2020 622e 2041 6e79 2061 7272 616e 6765    b. Any arrange
+000040c0: 6d65 6e74 732c 2075 6e64 6572 7374 616e  ments, understan
+000040d0: 6469 6e67 732c 206f 7220 6167 7265 656d  dings, or agreem
+000040e0: 656e 7473 2072 6567 6172 6469 6e67 2074  ents regarding t
+000040f0: 6865 0a20 2020 2020 4c69 6365 6e73 6564  he.     Licensed
+00004100: 204d 6174 6572 6961 6c20 6e6f 7420 7374   Material not st
+00004110: 6174 6564 2068 6572 6569 6e20 6172 6520  ated herein are 
+00004120: 7365 7061 7261 7465 2066 726f 6d20 616e  separate from an
+00004130: 640a 2020 2020 2069 6e64 6570 656e 6465  d.     independe
+00004140: 6e74 206f 6620 7468 6520 7465 726d 7320  nt of the terms 
+00004150: 616e 6420 636f 6e64 6974 696f 6e73 206f  and conditions o
+00004160: 6620 7468 6973 2050 7562 6c69 6320 4c69  f this Public Li
+00004170: 6365 6e73 652e 0a0a 0a53 6563 7469 6f6e  cense....Section
+00004180: 2038 202d 2d20 496e 7465 7270 7265 7461   8 -- Interpreta
+00004190: 7469 6f6e 2e0a 2d2d 2d2d 2d2d 2d2d 2d2d  tion..----------
+000041a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000041b0: 2d2d 0a0a 2020 612e 2046 6f72 2074 6865  --..  a. For the
+000041c0: 2061 766f 6964 616e 6365 206f 6620 646f   avoidance of do
+000041d0: 7562 742c 2074 6869 7320 5075 626c 6963  ubt, this Public
+000041e0: 204c 6963 656e 7365 2064 6f65 7320 6e6f   License does no
+000041f0: 742c 2061 6e64 0a20 2020 2020 7368 616c  t, and.     shal
+00004200: 6c20 6e6f 7420 6265 2069 6e74 6572 7072  l not be interpr
+00004210: 6574 6564 2074 6f2c 2072 6564 7563 652c  eted to, reduce,
+00004220: 206c 696d 6974 2c20 7265 7374 7269 6374   limit, restrict
+00004230: 2c20 6f72 2069 6d70 6f73 650a 2020 2020  , or impose.    
+00004240: 2063 6f6e 6469 7469 6f6e 7320 6f6e 2061   conditions on a
+00004250: 6e79 2075 7365 206f 6620 7468 6520 4c69  ny use of the Li
+00004260: 6365 6e73 6564 204d 6174 6572 6961 6c20  censed Material 
+00004270: 7468 6174 2063 6f75 6c64 206c 6177 6675  that could lawfu
+00004280: 6c6c 790a 2020 2020 2062 6520 6d61 6465  lly.     be made
+00004290: 2077 6974 686f 7574 2070 6572 6d69 7373   without permiss
+000042a0: 696f 6e20 756e 6465 7220 7468 6973 2050  ion under this P
+000042b0: 7562 6c69 6320 4c69 6365 6e73 652e 0a0a  ublic License...
+000042c0: 2020 622e 2054 6f20 7468 6520 6578 7465    b. To the exte
+000042d0: 6e74 2070 6f73 7369 626c 652c 2069 6620  nt possible, if 
+000042e0: 616e 7920 7072 6f76 6973 696f 6e20 6f66  any provision of
+000042f0: 2074 6869 7320 5075 626c 6963 204c 6963   this Public Lic
+00004300: 656e 7365 2069 730a 2020 2020 2064 6565  ense is.     dee
+00004310: 6d65 6420 756e 656e 666f 7263 6561 626c  med unenforceabl
+00004320: 652c 2069 7420 7368 616c 6c20 6265 2061  e, it shall be a
+00004330: 7574 6f6d 6174 6963 616c 6c79 2072 6566  utomatically ref
+00004340: 6f72 6d65 6420 746f 2074 6865 0a20 2020  ormed to the.   
+00004350: 2020 6d69 6e69 6d75 6d20 6578 7465 6e74    minimum extent
+00004360: 206e 6563 6573 7361 7279 2074 6f20 6d61   necessary to ma
+00004370: 6b65 2069 7420 656e 666f 7263 6561 626c  ke it enforceabl
+00004380: 652e 2049 6620 7468 6520 7072 6f76 6973  e. If the provis
+00004390: 696f 6e0a 2020 2020 2063 616e 6e6f 7420  ion.     cannot 
+000043a0: 6265 2072 6566 6f72 6d65 642c 2069 7420  be reformed, it 
+000043b0: 7368 616c 6c20 6265 2073 6576 6572 6564  shall be severed
+000043c0: 2066 726f 6d20 7468 6973 2050 7562 6c69   from this Publi
+000043d0: 6320 4c69 6365 6e73 650a 2020 2020 2077  c License.     w
+000043e0: 6974 686f 7574 2061 6666 6563 7469 6e67  ithout affecting
+000043f0: 2074 6865 2065 6e66 6f72 6365 6162 696c   the enforceabil
+00004400: 6974 7920 6f66 2074 6865 2072 656d 6169  ity of the remai
+00004410: 6e69 6e67 2074 6572 6d73 2061 6e64 0a20  ning terms and. 
+00004420: 2020 2020 636f 6e64 6974 696f 6e73 2e0a      conditions..
+00004430: 0a20 2063 2e20 4e6f 2074 6572 6d20 6f72  .  c. No term or
+00004440: 2063 6f6e 6469 7469 6f6e 206f 6620 7468   condition of th
+00004450: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
+00004460: 6520 7769 6c6c 2062 6520 7761 6976 6564  e will be waived
+00004470: 2061 6e64 206e 6f0a 2020 2020 2066 6169   and no.     fai
+00004480: 6c75 7265 2074 6f20 636f 6d70 6c79 2063  lure to comply c
+00004490: 6f6e 7365 6e74 6564 2074 6f20 756e 6c65  onsented to unle
+000044a0: 7373 2065 7870 7265 7373 6c79 2061 6772  ss expressly agr
+000044b0: 6565 6420 746f 2062 7920 7468 650a 2020  eed to by the.  
+000044c0: 2020 204c 6963 656e 736f 722e 0a0a 2020     Licensor...  
+000044d0: 642e 204e 6f74 6869 6e67 2069 6e20 7468  d. Nothing in th
+000044e0: 6973 2050 7562 6c69 6320 4c69 6365 6e73  is Public Licens
+000044f0: 6520 636f 6e73 7469 7475 7465 7320 6f72  e constitutes or
+00004500: 206d 6179 2062 6520 696e 7465 7270 7265   may be interpre
+00004510: 7465 640a 2020 2020 2061 7320 6120 6c69  ted.     as a li
+00004520: 6d69 7461 7469 6f6e 2075 706f 6e2c 206f  mitation upon, o
+00004530: 7220 7761 6976 6572 206f 662c 2061 6e79  r waiver of, any
+00004540: 2070 7269 7669 6c65 6765 7320 616e 6420   privileges and 
+00004550: 696d 6d75 6e69 7469 6573 0a20 2020 2020  immunities.     
+00004560: 7468 6174 2061 7070 6c79 2074 6f20 7468  that apply to th
+00004570: 6520 4c69 6365 6e73 6f72 206f 7220 596f  e Licensor or Yo
+00004580: 752c 2069 6e63 6c75 6469 6e67 2066 726f  u, including fro
+00004590: 6d20 7468 6520 6c65 6761 6c0a 2020 2020  m the legal.    
+000045a0: 2070 726f 6365 7373 6573 206f 6620 616e   processes of an
+000045b0: 7920 6a75 7269 7364 6963 7469 6f6e 206f  y jurisdiction o
+000045c0: 7220 6175 7468 6f72 6974 792e 0a         r authority..
```

### Comparing `rateslib-1.1.1/README.md` & `rateslib-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/pyproject.toml` & `rateslib-1.2.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 # pyproject.toml
 
+#[build-system]
+#requires      = ["setuptools>=61.0.0", "wheel"]
+#build-backend = "setuptools.build_meta"
+
 [build-system]
-requires      = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+requires = ["maturin>=1.0,<2.0"]
+build-backend = "maturin"
+
+[tool.maturin]
+bindings = "pyo3"
+compatibility = "linux"
+# rustc --print target-list
+# https://doc.rust-lang.org/rustc/platform-support.html
 
 [project]
 name = "rateslib"
-version = "1.1.1"
+version = "1.2.0"
 description = "A fixed income library for trading interest rates"
 readme = "README.md"
 authors = [{ name = "J H M Darbyshire"}]
 license = { file = "LICENSE" }
 keywords = ["interest rate", "derivatives", "swaps", "bonds", "fixed income"]
 dependencies = [
     "numpy>=1.21.5",
     "matplotlib>=3.5.1",
     "pandas>=1.4.1",
 ]
 requires-python = ">=3.9"
+classifiers = [
+    "Programming Language :: Rust",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.0.1",
     "jupyterlab>=3.3.1",
-    "sphinx>=5.1.1",
+    "sphinx>=7.1.0",
     "coverage>=7.1.0",
+    "sphinx-automodapi==0.16.0",
+    "pydata-sphinx-theme==0.14.3",
 ]
 
 [tool.setuptools]
 packages = ["rateslib"]
 
 [project.urls]
 Homepage = "https://github.com/attack68/rateslib"
```

### Comparing `rateslib-1.1.1/rateslib/__init__.py` & `rateslib-1.2.0/rateslib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,41 +49,52 @@
                 setattr(defaults, pat, val)
 
 
 from rateslib.dual import Dual, Dual2, dual_log, dual_exp, dual_solve
 
 from rateslib.calendars import create_calendar, get_calendar, add_tenor, dcf
 
-from rateslib.splines import bsplev_single, bspldnev_single, PPSpline
+from rateslib.splines import (
+    bsplev_single,
+    bspldnev_single,
+    PPSpline,
+    PPSplineF64,
+    PPSplineDual,
+    PPSplineDual2,
+)
 
 from rateslib.scheduling import Schedule
 
 from rateslib.curves import (
     Curve,
     LineCurve,
     interpolate,
     index_left,
     IndexCurve,
     CompositeCurve,
     ProxyCurve,
 )
 
+from rateslib.fx_volatility import FXDeltaVolSmile, FXDeltaVolSurface
+
 from rateslib.fx import (
     FXRates,
     FXForwards,
 )
 
 from rateslib.solver import Solver
 
 from rateslib.periods import (
     FixedPeriod,
     FloatPeriod,
     Cashflow,
     IndexFixedPeriod,
     IndexCashflow,
+    FXPutPeriod,
+    FXCallPeriod,
 )
 
 from rateslib.legs import (
     FixedLeg,
     FixedLegMtm,
     FloatLeg,
     FloatLegMtm,
@@ -92,14 +103,15 @@
     ZeroIndexLeg,
     IndexFixedLeg,
     CustomLeg,
 )
 
 from rateslib.instruments import (
     Value,
+    VolValue,
     Bill,
     FixedRateBond,
     IndexFixedRateBond,
     FloatRateNote,
     BondFuture,
     IRS,
     STIRFuture,
@@ -110,14 +122,20 @@
     SBS,
     FXSwap,
     FXExchange,
     XCS,
     Spread,
     Fly,
     Portfolio,
+    FXCall,
+    FXPut,
+    FXRiskReversal,
+    FXStraddle,
+    FXStrangle,
+    FXBrokerFly,
 )
 
 # module level doc-string
 __doc__ = """
 RatesLib - An efficient and interconnected fixed income library for Python
 ==========================================================================
 
@@ -141,14 +159,17 @@
     "dual_log",
     "dual_exp",
     "dual_solve",
     # splines.py
     "bsplev_single",
     "bspldnev_single",
     "PPSpline",
+    "PPSplineF64",
+    "PPSplineDual",
+    "PPSplineDual2",
     # calendars.py
     "create_calendar",
     "get_calendar",
     "add_tenor",
     "dcf",
     # scheduling.py
     "Schedule",
@@ -156,25 +177,30 @@
     "Curve",
     "LineCurve",
     "IndexCurve",
     "CompositeCurve",
     "ProxyCurve",
     "interpolate",
     "index_left",
+    # fx_volatility.py
+    "FXDeltaVolSmile",
+    "FXDeltaVolSurface",
     # solver.py
     "Solver",
     # fx.py
     "FXRates",
     "FXForwards",
     # periods.py,
     "FixedPeriod",
     "FloatPeriod",
     "Cashflow",
     "IndexCashflow",
     "IndexFixedPeriod",
+    "FXCallPeriod",
+    "FXPutPeriod",
     # legs.py
     "FixedLeg",
     "FloatLeg",
     "ZeroFloatLeg",
     "ZeroFixedLeg",
     "FixedLegMtm",
     "FloatLegMtm",
@@ -184,21 +210,30 @@
     # instruments.py
     "FixedRateBond",
     "IndexFixedRateBond",
     "FloatRateNote",
     "BondFuture",
     "FRA",
     "Value",
+    "VolValue",
     "Bill",
     "IRS",
     "STIRFuture",
     "IIRS",
     "ZCS",
     "ZCIS",
     "SBS",
     "FXSwap",
     "FXExchange",
     "XCS",
     "Spread",
     "Fly",
     "Portfolio",
+    "FXCall",
+    "FXPut",
+    "FXRiskReversal",
+    "FXStraddle",
+    "FXStrangle",
+    "FXBrokerFly",
 ]
+
+__version__ = "1.2.0"
```

### Comparing `rateslib-1.1.1/rateslib/_spec_loader.py` & `rateslib-1.2.0/rateslib/_spec_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,15 @@
                 return None
 
         if version.parse(pd.__version__) >= version.parse("2.1.0"):
             # applymap issues a deprecation warning with version <2.1.0
             # TODO (low): clean this up when setting a minimum pandas version at 2.1.0
             df[df["dtype"] == "bool"] = df[df["dtype"] == "bool"].map(_map_true_false)
         else:
-            df[df["dtype"] == "bool"] = df[df["dtype"] == "bool"].applymap(
-                _map_true_false
-            )
+            df[df["dtype"] == "bool"] = df[df["dtype"] == "bool"].applymap(_map_true_false)
         return df
 
     path = "data/__instrument_spec.csv"
     abspath = os.path.dirname(os.path.abspath(__file__))
     target = os.path.join(abspath, path)
     df = pd.read_csv(target)
     df = _append_kwargs_name(df)
```

### Comparing `rateslib-1.1.1/rateslib/calendars.py` & `rateslib-1.2.0/rateslib/calendars.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Union, Dict, Any
 from math import floor
 from datetime import datetime, timedelta
 import calendar as calendar_mod
+import warnings
 
 from dateutil.relativedelta import MO, TH, FR
 
 from pandas.tseries.holiday import (
     AbstractHolidayCalendar,
     Holiday,
     next_monday,
@@ -1132,42 +1133,53 @@
 ):
     if frequency_months is NoInput.blank:
         raise ValueError("`frequency_months` must be supplied with specified `convention`.")
     if termination is NoInput.blank:
         raise ValueError("`termination` must be supplied with specified `convention`.")
     if stub is NoInput.blank:
         raise ValueError("`stub` must be supplied with specified `convention`.")
-    if not stub:
+    if not stub and frequency_months < 13:  # This is a well defined period that is NOT zero coupon
         return frequency_months / 12.0
     else:
+        # Perform stub and zero coupon calculation. Zero coupons handled with an Annual frequency.
+        if frequency_months >= 13:
+            warnings.warn(
+                "Using `convention` 'ActActICMA' with a Period having `frequency` 'Z' is undefined, and "
+                "should be avoided.\nFor calculation purposes here the `frequency` is set to 'A'.",
+                UserWarning,
+            )
+            frequency_months = 12  # Will handle Z frequency as a stub period see GH:144
+
         # roll is used here to roll a negative months forward eg, 30 sep minus 6M = 30/31 March.
         if end == termination:  # stub is a BACK stub:
-            fwd_end = _add_months(start, frequency_months, "NONE", calendar, roll)
-            fraction = 0.0
-            if end > fwd_end:  # stub is LONG
+            fwd_end_0, fwd_end_1, fraction = start, start, -1.0
+            while (
+                end > fwd_end_1
+            ):  # Handle Long Stubs which require repeated periods, and Zero frequencies.
+                fwd_end_0 = fwd_end_1
                 fraction += 1.0
-                fraction += (end - fwd_end) / (
-                    _add_months(start, 2 * frequency_months, "NONE", calendar, roll) - fwd_end
+                fwd_end_1 = _add_months(
+                    start, (int(fraction) + 1) * frequency_months, "NONE", calendar, roll
                 )
-            else:
-                fraction += (end - start) / (fwd_end - start)
+
+            fraction += (end - fwd_end_0) / (fwd_end_1 - fwd_end_0)
             return fraction * frequency_months / 12.0
         else:  # stub is a FRONT stub
-            prev_start = _add_months(end, -frequency_months, "NONE", calendar, roll)
-            fraction = 0
-            if start < prev_start:  # stub is LONG
-                fraction += 1
-                r = prev_start - start
-                s = prev_start - _add_months(end, -2 * frequency_months, "NONE", calendar, roll)
-                fraction += r / s
-            else:
-                r = end - start
-                s = end - prev_start
-                fraction += r / s
-            return fraction * frequency_months / 12
+            prev_start_0, prev_start_1, fraction = end, end, -1.0
+            while (
+                start < prev_start_1
+            ):  # Handle Long Stubs which require repeated periods, and Zero frequencies.
+                prev_start_0 = prev_start_1
+                fraction += 1.0
+                prev_start_1 = _add_months(
+                    end, -(int(fraction) + 1) * frequency_months, "NONE", calendar, roll
+                )
+
+            fraction += (prev_start_0 - start) / (prev_start_0 - prev_start_1)
+            return fraction * frequency_months / 12.0
 
 
 def _dcf_actacticma_stub365f(
     start: datetime,
     end: datetime,
     termination: Union[datetime, NoInput],
     frequency_months: Union[int, NoInput],
@@ -1233,15 +1245,15 @@
     "30360": _dcf_30360,
     "360360": _dcf_30360,
     "BONDBASIS": _dcf_30360,
     "30E360": _dcf_30e360,
     "EUROBONDBASIS": _dcf_30e360,
     "30E360ISDA": _dcf_30e360isda,
     "ACTACT": _dcf_actactisda,
-    "ACTACTISDA": _dcf_30e360isda,
+    "ACTACTISDA": _dcf_actactisda,
     "ACTACTICMA": _dcf_actacticma,
     "ACTACTICMA_STUB365F": _dcf_actacticma_stub365f,
     "ACTACTISMA": _dcf_actacticma,
     "ACTACTBOND": _dcf_actacticma,
     "1": _dcf_1,
     "1+": _dcf_1plus,
 }
```

### Comparing `rateslib-1.1.1/rateslib/curves.py` & `rateslib-1.2.0/rateslib/curves.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,37 +7,34 @@
 """
 
 from __future__ import annotations
 
 from datetime import datetime, timedelta
 from pytz import UTC
 from typing import Optional, Union, Callable, Any
+import numpy as np
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas.tseries.holiday import Holiday
 from uuid import uuid4
-import numpy as np
 import warnings
 import json
 from math import floor, comb
 from rateslib import defaults
-from rateslib.dual import Dual, dual_log, dual_exp, set_order_convert
-from rateslib.splines import (
-    PPSplineF64,
-    PPSplineDual,
-    PPSplineDual2
-)
+from rateslib.dual import Dual, dual_log, dual_exp, set_order_convert, DualTypes, Dual2
+from rateslib.splines import PPSplineF64, PPSplineDual, PPSplineDual2
 from rateslib.default import plot, NoInput
 from rateslib.calendars import (
     create_calendar,
     get_calendar,
     add_tenor,
     dcf,
     CalInput,
     _DCF1d,
 )
+from rateslibrs import index_left_f64
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from rateslib.fx import FXForwards  # pragma: no cover
 
 
@@ -165,15 +162,15 @@
         if order == getattr(self, "ad", None):
             return None
         elif order not in [0, 1, 2]:
             raise ValueError("`order` can only be in {0, 1, 2} for auto diff calcs.")
 
         self.ad = order
         self.nodes = {
-            k: set_order_convert(v, order, f"{self.id}{i}")
+            k: set_order_convert(v, order, [f"{self.id}{i}"])
             for i, (k, v) in enumerate(self.nodes.items())
         }
         self.csolve()
         return None
 
 
 class Curve(_Serialize):
@@ -308,19 +305,23 @@
         modifier: Union[str, NoInput] = NoInput(0),
         calendar: Union[CustomBusinessDay, str, NoInput] = NoInput(0),
         ad: int = 0,
         **kwargs,
     ):
         self.id = uuid4().hex[:5] + "_" if id is NoInput.blank else id  # 1 in a million clash
         self.nodes = nodes  # nodes.copy()
-        self.node_dates = list(self.nodes.keys())
+        self.node_keys = list(self.nodes.keys())
+        self.node_dates = self.node_keys
+        self.node_dates_posix = [_.replace(tzinfo=UTC).timestamp() for _ in self.node_dates]
         self.n = len(self.node_dates)
         for idx in range(1, self.n):
-            if self.node_dates[idx-1] >= self.node_dates[idx]:
-                raise ValueError("Curve node dates are not sorted or contain duplicates. To sort directly use: `dict(sorted(nodes.items()))`")
+            if self.node_dates[idx - 1] >= self.node_dates[idx]:
+                raise ValueError(
+                    "Curve node dates are not sorted or contain duplicates. To sort directly use: `dict(sorted(nodes.items()))`"
+                )
         self.interpolation = (
             defaults.interpolation[type(self).__name__]
             if interpolation is NoInput.blank
             else interpolation
         )
         if isinstance(self.interpolation, str):
             self.interpolation = self.interpolation.lower()
@@ -340,58 +341,62 @@
         else:
             self.spline_endpoints = [_.lower() for _ in endpoints]
 
         self.t = t
         self.c_init = False if c is NoInput.blank else True
         if t is not NoInput.blank:
             self.t_posix = [_.replace(tzinfo=UTC).timestamp() for _ in t]
-            self.spline = PPSplineF64(4, self.t_posix, c)
+            self.spline = PPSplineF64(4, self.t_posix, None if c is NoInput.blank else c)
             if len(self.t) < 10 and "not_a_knot" in self.spline_endpoints:
                 raise ValueError(
                     "`endpoints` cannot be 'not_a_knot' with only 1 interior breakpoint"
                 )
         else:
             self.t_posix = None
             self.spline = None
 
         self._set_ad_order(order=ad)
 
     def __getitem__(self, date: datetime):
+        date_posix = date.replace(tzinfo=UTC).timestamp()
         if self.spline is None or date <= self.t[0]:
             if isinstance(self.interpolation, Callable):
                 return self.interpolation(date, self.nodes.copy())
-            return self._local_interp_(date)
+            return self._local_interp_(date_posix)
         else:
             if date > self.t[-1]:
                 warnings.warn(
                     "Evaluating points on a curve beyond the endpoint of the basic "
                     "spline interval is undefined.\n"
                     f"date: {date.strftime('%Y-%m-%d')}, spline end: {self.t[-1].strftime('%Y-%m-%d')}",
                     UserWarning,
                 )
-            date_posix = date.replace(tzinfo=UTC).timestamp()
             return self._op_exp(self.spline.ppev_single(date_posix))
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-    def _local_interp_(self, date: datetime):
-        if date < self.node_dates[0]:
+    def _local_interp_(self, date_posix: float):
+        if date_posix < self.node_dates_posix[0]:
             return 0  # then date is in the past and DF is zero
-        l_index = index_left(self.node_dates, self.n, date)
+        l_index = index_left_f64(self.node_dates_posix, date_posix, None)
+        node_left_posix, node_right_posix = (
+            self.node_dates_posix[l_index],
+            self.node_dates_posix[l_index + 1],
+        )
         node_left, node_right = self.node_dates[l_index], self.node_dates[l_index + 1]
         return interpolate(
-            date,
-            node_left,
+            date_posix,
+            node_left_posix,
             self.nodes[node_left],
-            node_right,
+            node_right_posix,
             self.nodes[node_right],
             self.interpolation,
-            self.node_dates[0],
+            self.node_dates_posix[0],
         )
 
     # def plot(self, *args, **kwargs):
     #     return super().plot(*args, **kwargs)
 
     def rate(
         self,
@@ -486,26 +491,34 @@
             )
             curve_act360.rate(dt(2022, 2, 1), dt(2022, 3, 1))
         """
         modifier = self.modifier if modifier is NoInput.blank else modifier
         # calendar = self.calendar if calendar is False else calendar
         # convention = self.convention if convention is None else convention
 
+        # Alternative solution to PR 172.
+        # if effective < self.node_dates[0]:
+        #     raise ValueError(
+        #         "`effective` date for rate period is before the initial node date of the Curve.\n"
+        #         "If you are trying to calculate a rate for an historical FloatPeriod have you "
+        #         "neglected to supply appropriate `fixings`?\n"
+        #         "See Documentation > Cookbook > Working with Fixings."
+        #     )
         if isinstance(termination, str):
             termination = add_tenor(effective, termination, modifier, self.calendar)
         try:
             n_, d_ = self[effective], self[termination]
             df_ratio = n_ / d_
         except ZeroDivisionError:
             return None
 
         if termination == effective:
             raise ZeroDivisionError(f"effective: {effective}, termination: {termination}")
         n_, d_ = (df_ratio - 1), dcf(effective, termination, self.convention)
-        _ =  n_ / d_ * 100
+        _ = n_ / d_ * 100
 
         if float_spread is not None and abs(float_spread) > 1e-9:
             if spread_compound_method == "none_simple":
                 return _ + float_spread / 100
             elif spread_compound_method == "isda_compounding":
                 # this provides an approximated rate
                 r_bar, d, n = average_rate(effective, termination, self.convention, _)
@@ -552,22 +565,22 @@
         if self.ad == 0:
             Spline = PPSplineF64
         elif self.ad == 1:
             Spline = PPSplineDual
         else:
             Spline = PPSplineDual2
 
-        t_posix = [_.replace(tzinfo=UTC).timestamp() for _ in self.t]
+        t_posix = self.t_posix.copy()
         tau_posix = [k.replace(tzinfo=UTC).timestamp() for k in self.nodes.keys() if k >= self.t[0]]
         y = [self._op_log(v) for k, v in self.nodes.items() if k >= self.t[0]]
 
         # Left side constraint
         if self.spline_endpoints[0].lower() == "natural":
             tau_posix.insert(0, self.t_posix[0])
-            y.insert(0, set_order_convert(0., self.ad, None))
+            y.insert(0, set_order_convert(0.0, self.ad, None))
             left_n = 2
         elif self.spline_endpoints[0].lower() == "not_a_knot":
             t_posix.pop(4)
             left_n = 0
         else:
             raise NotImplementedError(
                 f"Endpoint method '{self.spline_endpoints[0]}' not implemented."
@@ -583,15 +596,15 @@
             right_n = 0
         else:
             raise NotImplementedError(
                 f"Endpoint method '{self.spline_endpoints[0]}' not implemented."
             )
 
         self.spline = Spline(4, t_posix, None)
-        self.spline.csolve(np.array(tau_posix), np.array(y), left_n, right_n)
+        self.spline.csolve(tau_posix, y, left_n, right_n, False)
         return None
 
     def shift(
         self,
         spread: float,
         id: Optional[str] = None,
         composite: bool = True,
@@ -1171,14 +1184,50 @@
 
         left, right = self.node_dates[0], self.node_dates[-1]
         points = (right - left).days
         x = [left + timedelta(days=i) for i in range(points)]
         rates = [forward_fx(_, self, curve_foreign, fx_rate, fx_settlement) for _ in x]
         return plot(x, [rates])
 
+    def _set_node_vector(self, vector: list[DualTypes], ad):
+        """Used to update curve values during a Solver iteration. ``ad`` in {1, 2}."""
+        DualType = Dual if ad == 1 else Dual2
+        DualArgs = ([],) if ad == 1 else ([], [])
+        base_obj = DualType(0.0, [f"{self.id}{i}" for i in range(self.n)], *DualArgs)
+        ident = np.eye(self.n)
+
+        if self._ini_solve == 1:
+            # then the first node on the Curve is not updated but
+            # set it as a dual type with consistent vars.
+            self.nodes[self.node_keys[0]] = DualType.vars_from(
+                base_obj,
+                self.nodes[self.node_keys[0]].real,
+                base_obj.vars,
+                ident[0, :].tolist(),
+                *DualArgs[1:],
+            )
+
+        for i, k in enumerate(self.node_keys[self._ini_solve :]):
+            self.nodes[k] = DualType.vars_from(
+                base_obj,
+                vector[i].real,
+                base_obj.vars,
+                ident[i + self._ini_solve, :].tolist(),
+                *DualArgs[1:],
+            )
+        self.csolve()
+
+    def _get_node_vector(self):
+        """Get a 1d array of variables associated with nodes of this object updated by Solver"""
+        return np.array(list(self.nodes.values())[self._ini_solve:])
+
+    def _get_node_vars(self):
+        """Get the variable names of elements updated by a Solver"""
+        return tuple((f"{self.id}{i}" for i in range(self._ini_solve, self.n)))
+
 
 class LineCurve(Curve):
     """
     Curve based on value parametrisation at given node dates with interpolation.
 
     Parameters
     ----------
@@ -2277,14 +2326,17 @@
 
         See :meth:`IndexCurve.index_value()<rateslib.curves.IndexCurve.index_value>`
         """
         if not isinstance(self.curves[0], IndexCurve):
             raise TypeError("`index_value` not available on non `IndexCurve` types.")
         return super().index_value(date, interpolation)
 
+    def _get_node_vector(self):
+        return NotImplementedError("Instances of CompositeCurve do not have solvable variables.")
+
 
 class MultiCsaCurve(CompositeCurve):
     """
     A dynamic composition of a sequence of other curves.
 
     .. note::
        Can only combine curves of the type: :class:`Curve`. Other curve parameters such as
@@ -2361,16 +2413,16 @@
         _ = (df_num / df_den - 1) * 100 / (d * n)
         return _
 
     def __getitem__(self, date: datetime):
         # will return a composited discount factor
         if date == self.curves[0].node_dates[0]:
             return 1.0  # TODO (low:?) this is not variable but maybe should be tagged as "id0"?
-        days = (date - self.curves[0].node_dates[0]).days
-        d = _DCF1d[self.convention.upper()]
+        # days = (date - self.curves[0].node_dates[0]).days
+        # d = _DCF1d[self.convention.upper()]
 
         # method uses the step and picks the highest (cheapest rate)
         # in each period
         _ = 1.0
         d1 = self.curves[0].node_dates[0]
 
         def _get_step(step):
@@ -2621,14 +2673,17 @@
 
     def _set_ad_order(self):  # pragma: no cover
         """
         Not implemented for :class:`~rateslib.fx.ProxyCurve` s.
         """
         return NotImplementedError("`set_ad_order` not available on proxy curve.")
 
+    def _get_node_vector(self):
+        return NotImplementedError("Instances of ProxyCurve do not have solvable variables.")
+
 
 def average_rate(effective, termination, convention, rate):
     """
     Return the geometric, 1 calendar day, average rate for the rate in a period.
 
     This is used for approximations usually in combination with floating periods.
 
@@ -2703,22 +2758,23 @@
             return 1 / z
 
         y_1, y_2 = 1 / y_1, 1 / y_2
     elif interpolation == "log_linear":
         op, y_1, y_2 = dual_exp, dual_log(y_1), dual_log(y_2)
     elif interpolation == "linear_zero_rate":
         # convention not used here since we just determine linear rate interpolation
-        y_2 = dual_log(y_2) / ((start - x_2) / timedelta(days=365))
+        # 86400. scalar relates to using posix timestamp conversion
+        y_2 = dual_log(y_2) / ((start - x_2) / (365.0 * 86400.0))
         if start == x_1:
             y_1 = y_2
         else:
-            y_1 = dual_log(y_1) / ((start - x_1) / timedelta(days=365))
+            y_1 = dual_log(y_1) / ((start - x_1) / (365.0 * 86400.0))
 
         def op(z):
-            return dual_exp((start - x) / timedelta(days=365) * z)
+            return dual_exp((start - x) / (365.0 * 86400.0) * z)
 
     elif interpolation == "flat_forward":
         if x >= x_2:
             return y_2
         return y_1
     elif interpolation == "flat_backward":
         if x <= x_1:
```

### Comparing `rateslib-1.1.1/rateslib/data/cad_rfr.csv` & `rateslib-1.2.0/rateslib/data/cad_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/chf_rfr.csv` & `rateslib-1.2.0/rateslib/data/chf_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/corra.csv` & `rateslib-1.2.0/rateslib/data/corra.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/estr.csv` & `rateslib-1.2.0/rateslib/data/estr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/eur_rfr.csv` & `rateslib-1.2.0/rateslib/data/eur_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/gbp_rfr.csv` & `rateslib-1.2.0/rateslib/data/gbp_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/nok_rfr.csv` & `rateslib-1.2.0/rateslib/data/nok_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/nowa.csv` & `rateslib-1.2.0/rateslib/data/nowa.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/sek_rfr.csv` & `rateslib-1.2.0/rateslib/data/sek_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/sofr.csv` & `rateslib-1.2.0/rateslib/data/sofr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/sonia.csv` & `rateslib-1.2.0/rateslib/data/sonia.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/swestr.csv` & `rateslib-1.2.0/rateslib/data/swestr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/data/usd_rfr.csv` & `rateslib-1.2.0/rateslib/data/usd_rfr.csv`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/default.py` & `rateslib-1.2.0/rateslib/default.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 class NoInput(Enum):
     """
     Enumerable type to handle setting default values.
 
     See :ref:`default values <defaults-doc>`.
     """
+
     blank = 0
     inherit = 1
     negate = -1
 
 
 class Fixings:
     """
@@ -141,14 +142,18 @@
         "rfr_lockout_avg": 2,
         "rfr_lookback_avg": 2,
         "ibor": 2,
     }
     spread_compound_method = "none_simple"
     base_currency = "usd"
 
+    fx_delivery_lag = 2
+    fx_delta_type = "spot"
+    fx_option_metric = "pips"
+
     # Curves
 
     interpolation = {
         "Curve": "log_linear",
         "LineCurve": "linear",
         "IndexCurve": "linear_index",
     }
@@ -287,16 +292,24 @@
     fig, ax = plt.subplots(1, 1)
     lines = []
     for _y in y:
         (line,) = ax.plot(x, _y)
         lines.append(line)
     if labels and len(labels) == len(lines):
         ax.legend(lines, labels)
-    years = mdates.YearLocator()  # every year
-    months = mdates.MonthLocator()  # every month
-    yearsFmt = mdates.DateFormatter("%Y")
-    ax.xaxis.set_major_locator(years)
-    ax.xaxis.set_major_formatter(yearsFmt)
-    ax.xaxis.set_minor_locator(months)
+
     ax.grid(True)
-    fig.autofmt_xdate()
+
+    if isinstance(x[0], datetime):
+        years = mdates.YearLocator()  # every year
+        months = mdates.MonthLocator()  # every month
+        yearsFmt = mdates.DateFormatter("%Y")
+        ax.xaxis.set_major_locator(years)
+        ax.xaxis.set_major_formatter(yearsFmt)
+        ax.xaxis.set_minor_locator(months)
+        fig.autofmt_xdate()
     return fig, ax, lines
+
+
+def _drb(default, possible_blank):
+    """(D)efault (r)eplaces (b)lank"""
+    return default if possible_blank is NoInput.blank else possible_blank
```

### Comparing `rateslib-1.1.1/rateslib/dual/dual.py` & `rateslib-1.2.0/rateslib/dual/dual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,24 @@
 from math import isclose
 from abc import abstractmethod, ABCMeta
-from typing import Union, Optional
+from typing import Optional
+from statistics import NormalDist
 import math
 import numpy as np
+from rateslib.default import NoInput
 
 PRECISION = 1e-14
 FLOATS = (float, np.float16, np.float32, np.float64, np.longdouble)
 INTS = (int, np.int8, np.int16, np.int32, np.int32, np.int64)
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-def gradient(dual, vars: Optional[list[str]] = None, order: int = 1, keep_manifold: bool = False):
-    """
-    Return derivatives of a dual number.
-
-    Parameters
-    ----------
-    dual : Dual or Dual2
-        The dual variable from which to derive derivatives.
-    vars : str, tuple, list optional
-        Name of the variables which to return gradients for. If not given
-        defaults to all vars attributed to the instance.
-    order : {1, 2}
-        Whether to return the first or second derivative of the dual number.
-        Second order will raise if applied to a ``Dual`` and not ``Dual2`` instance.
-    keep_manifold : bool
-        If ``order`` is 1 and the type is ``Dual2`` one can return a ``Dual2``
-        where the ``dual2`` values are converted to ``dual`` values to represent
-        a first order manifold of the first derivative (and the ``dual2`` values
-        set to zero). Useful for propagation in iterations.
-
-    Returns
-    -------
-    float, ndarray, Dual2
-    """
-    if not isinstance(dual, (Dual, Dual2)):
-        raise TypeError("Must call `gradient` on dual-type variables")
-    return dual.grad(vars, order, keep_manifold)
-
-
 class DualBase(metaclass=ABCMeta):
     """
     Base class for dual number implementation.
     """
 
     dual: np.ndarray = np.zeros(0)
     dual2: np.ndarray = np.zeros(0)
@@ -80,15 +53,17 @@
         if float(self) > float(argument):
             return True
         return False
 
     def __eq__(self, argument):
         """Compare an argument with a Dual number for equality."""
         if not isinstance(argument, type(self)):
-            if not isinstance(argument, (*FLOATS, *INTS)):
+            if isinstance(argument, NoInput):
+                return False
+            elif not isinstance(argument, (*FLOATS, *INTS)):
                 raise TypeError(f"Cannot compare {type(self)} with incompatible type.")
             argument = type(self)(float(argument))
         if self.vars == argument.vars:
             return self.__eq_coeffs__(argument, PRECISION)
         else:
             self_, argument = self.__upcast_combined__(argument)
             return self_.__eq__(argument)
@@ -158,14 +133,23 @@
             return _.dual[ix_]
         else:
             ret = np.array([Dual2(v, vars) for v in _.dual[ix_]])
             for ix, du in zip(ix_, ret):
                 du.dual = 2 * _.dual2[ix, ix_]
             return ret
 
+    def grad1(self, vars=None):
+        return self.grad(vars, order=1, keep_manifold=False)
+
+    def grad1_manifold(self, vars=None):
+        return self.grad(vars, order=1, keep_manifold=True)
+
+    def grad2(self, vars=None, keep_manifold=False):
+        return self.grad(vars, order=2, keep_manifold=keep_manifold)
+
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
 class Dual2(DualBase):
@@ -218,19 +202,19 @@
         elif dual2 is not None:
             self.dual2 = np.asarray(dual2.copy())
         else:
             self.dual2 = np.zeros((n, n))
 
     def __repr__(self):
         name, final = "Dual2", ", [[...]]"
-        vars = ', '.join(self.vars[:3])
-        dual = ', '.join([f"{_:.1f}" for _ in self.dual[:3]])
+        vars = ", ".join(self.vars[:3])
+        dual = ", ".join([f"{_:.1f}" for _ in self.dual[:3]])
         if len(self.vars) > 3:
-            vars += ',...'
-            dual += ',...'
+            vars += ",..."
+            dual += ",..."
         return f"<{name}: {self.real:,.6f}, ({vars}), [{dual}]{final}>"
 
     def __str__(self):
         output = f" val = {self.real:.8f}\n"
         for i, tag in enumerate(self.vars):
             output += f"  d{tag} = {self.dual[i]:.6f}\n"
         for i, ltag in enumerate(self.vars):
@@ -361,19 +345,41 @@
         return Dual2(
             math.log(self.real),
             self.vars,
             self.dual / self.real,
             self.dual2 / self.real - np.einsum("i,j", self.dual, self.dual) * 0.5 / self.real**2,
         )
 
+    def __norm_cdf__(self):
+        base = NormalDist().cdf(self.real)
+        scalar = 1 / math.sqrt(2 * math.pi) * math.exp(-0.5 * self.real**2)
+        scalar2 = scalar * -self.real
+        return Dual2(
+            base,
+            self.vars,
+            scalar * self.dual,
+            scalar * self.dual2 + 0.5 * scalar2 * np.einsum("i,j", self.dual, self.dual),
+        )
+
+    def __norm_inv_cdf__(self):
+        base = NormalDist().inv_cdf(self.real)
+        scalar = math.sqrt(2 * math.pi) * math.exp(0.5 * base**2)
+        scalar2 = base * scalar**2
+        return Dual2(
+            base,
+            self.vars,
+            scalar * self.dual,
+            scalar * self.dual2 + 0.5 * scalar2 * np.einsum("i,j", self.dual, self.dual),
+        )
+
     def __upcast_vars__(self, new_vars):
         n = len(new_vars)
         dual, dual2 = np.zeros(n), np.zeros((n, n))
         ix_ = list(map(lambda x: new_vars.index(x), self.vars))
-        dual[ix_] = self.dual,
+        dual[ix_] = (self.dual,)
         dual2[np.ix_(ix_, ix_)] = self.dual2
         return Dual2(self.real, new_vars, dual, dual2)
 
     def __downcast_vars__(self):
         """removes variables where first and second order sensitivity is zero"""
         ix_ = np.where(~np.isclose(self.dual, 0, atol=PRECISION))[0]
         ix2_ = np.where(~np.isclose(self.dual2.sum(axis=0), 0, atol=PRECISION))[0]
@@ -448,19 +454,19 @@
 
     @property
     def dual2(self):
         raise ValueError("`Dual` variable cannot possess `dual2` attribute")
 
     def __repr__(self):
         name, final = "Dual", ""
-        vars = ', '.join(self.vars[:3])
-        dual = ', '.join([f"{_:.1f}" for _ in self.dual[:3]])
+        vars = ", ".join(self.vars[:3])
+        dual = ", ".join([f"{_:.1f}" for _ in self.dual[:3]])
         if len(self.vars) > 3:
-            vars += ',...'
-            dual += ',...'
+            vars += ",..."
+            dual += ",..."
         return f"<{name}: {self.real:,.6f}, ({vars}), [{dual}]{final}>"
 
     def __str__(self):
         output = f" val = {self.real:.8f}\n"
         for i, tag in enumerate(self.vars):
             output += f"  d{tag} = {self.dual[i]:.6f}\n"
         return output
@@ -546,14 +552,24 @@
     def __exp__(self):
         const = math.exp(self.real)
         return Dual(const, self.vars, self.dual * const)
 
     def __log__(self):
         return Dual(math.log(self.real), self.vars, self.dual / self.real)
 
+    def __norm_cdf__(self):
+        base = NormalDist().cdf(self.real)
+        scalar = 1 / math.sqrt(2 * math.pi) * math.exp(-0.5 * self.real**2)
+        return Dual(base, self.vars, scalar * self.dual)
+
+    def __norm_inv_cdf__(self):
+        base = NormalDist().inv_cdf(self.real)
+        scalar = math.sqrt(2 * math.pi) * math.exp(0.5 * base**2)
+        return Dual(base, self.vars, scalar * self.dual)
+
     def __upcast_vars__(self, new_vars):
         n = len(new_vars)
         dual = np.zeros(n)
         ix_ = list(map(lambda x: new_vars.index(x), self.vars))
         dual[ix_] = self.dual
         return Dual(self.real, new_vars, dual)
 
@@ -564,15 +580,15 @@
         new_vars = tuple(self.vars[i] for i in ix_)
         return Dual(self.real, new_vars, self.dual[ix_])
 
     def _set_order(self, order):
         if order == 1:
             return self
         if order == 2:
-            return Dual2(self.real, self.vars, self.dual)
+            return Dual2(self.real, self.vars, self.dual, [])
         if order == 0:
             return float(self)
 
     @staticmethod
     def vars_from(other, real, vars=(), dual=None):
         if other.vars == vars:
             return Dual(real, vars, dual)
@@ -582,64 +598,19 @@
     # def __str__(self):
     #     output = f"    f = {self.real:.8f}\n"
     #     for i, tag in enumerate(self.vars):
     #         output += f"df/d{tag} = {self.dual[i]:.6f}\n"
     #     return output
 
 
-def dual_exp(x):
-    """
-    Calculate the exponential value of a regular int or float or a dual number.
-
-    Parameters
-    ----------
-    x : int, float, Dual, Dual2
-        Value to calculate exponent of.
-
-    Returns
-    -------
-    float, Dual, Dual2
-    """
-    if isinstance(x, (Dual, Dual2)):
-        return x.__exp__()
-    return math.exp(x)
-
-
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-def dual_log(x, base=None):
-    """
-    Calculate the logarithm of a regular int or float or a dual number.
-
-    Parameters
-    ----------
-    x : int, float, Dual, Dual2
-        Value to calculate exponent of.
-    base : int, float, optional
-        Base of the logarithm. Defaults to e to compute natural logarithm
-
-    Returns
-    -------
-    float, Dual, Dual2
-    """
-    if isinstance(x, (Dual, Dual2)):
-        val = x.__log__()
-        if base is None:
-            return val
-        else:
-            return val * (1 / math.log(base))
-    elif base is None:
-        return math.log(x)
-    else:
-        return math.log(x, base)
-
-
 def _pivot_matrix(A, method=1):
     """
     Returns the pivoting matrix for P, used in Doolittle's method.
 
     Notes
     -----
     Partial pivoting can fail. If the solution detects that it has failed
@@ -654,15 +625,15 @@
     # Pivot P such that the largest element of each column of A is on diagonal
     for j in range(n):
         # row = np.argmax(np.abs(_[j:, j]))  <- alternative but seems slower
         row = max(range(j, n), key=lambda i: abs(_[i][j]))
         if j != row:
             P[[j, row]] = P[[row, j]]  # Define a row swap in P
             PA[[j, row]] = PA[[row, j]]
-            if method == 2:
+            if method == 1:
                 _[[j, row]] = _[[row, j]]  # alters the pivoting by updating underlying
     return P, PA
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
@@ -680,32 +651,31 @@
     # Create zero matrices for L and U
     L, U = np.zeros((n, n), dtype="object"), np.zeros((n, n), dtype="object")
 
     # Create the pivot matrix P and the multipled matrix PA
     P, PA = _pivot_matrix(A, method=method)
 
     # Perform the LU Decomposition
-    try:
-        for j in range(n):
-            # All diagonal entries of L are set to unity
-            L[j, j] = 1.0
-
-            # LaTeX: u_{ij} = a_{ij} - \sum_{k=1}^{i-1} u_{kj} l_{ik}
-            for i in range(j + 1):
-                sx = np.matmul(L[i, :i], U[:i, j])
-                # s1 = sum(U[k][j] * L[i][k] for k in range(i))
-                U[i, j] = PA[i, j] - sx
-
-            # LaTeX: l_{ij} = \frac{1}{u_{jj}} (a_{ij} - \sum_{k=1}^{j-1} u_{kj} l_{ik})
-            for i in range(j, n):
-                sy = np.matmul(L[i, :j], U[:j, j])
-                # s2 = sum(U[k][j] * L[i][k] for k in range(j))
-                L[i, j] = (PA[i, j] - sy) / U[j, j]
-    except ZeroDivisionError:
-        return _plu_decomp(A, method + 1)  # retry with altered pivoting technique
+    for j in range(n):
+        # All diagonal entries of L are set to unity
+        L[j, j] = 1.0
+
+        # LaTeX: u_{ij} = a_{ij} - \sum_{k=1}^{i-1} u_{kj} l_{ik}
+        for i in range(j + 1):
+            sx = np.matmul(L[i, :i], U[:i, j])
+            # s1 = sum(U[k][j] * L[i][k] for k in range(i))
+            U[i, j] = PA[i, j] - sx
+
+        # LaTeX: l_{ij} = \frac{1}{u_{jj}} (a_{ij} - \sum_{k=1}^{j-1} u_{kj} l_{ik})
+        for i in range(j, n):
+            sy = np.matmul(L[i, :j], U[:j, j])
+            # s2 = sum(U[k][j] * L[i][k] for k in range(j))
+            if abs(U[j, j]) < 1e-16:
+                return _plu_decomp(A, method + 1)  # retry with altered pivoting technique
+            L[i, j] = (PA[i, j] - sy) / U[j, j]
 
     return P, L, U
 
 
 def _solve_lower_triangular_1d(L, b):
     """dual_solve the equation Lx = b, for L lower diagonal matrix, b is 1 dimension"""
     n = L.shape[0]
@@ -726,15 +696,15 @@
 
 
 def _solve_upper_triangular(U, b):
     """dual_solve the equation Ux = b, for U upper diagonal matrix"""
     return _solve_lower_triangular(U[::-1, ::-1], b[::-1, ::-1])[::-1, ::-1]
 
 
-def dual_solve(A, b, allow_lsq=False):
+def _dsolve(A, b, allow_lsq=False):
     """
     Solve the linear system Ax=b.
 
     Parameters
     ----------
     A : ndarray of object dtype
         Array which can contain dual number data types.
@@ -761,69 +731,10 @@
 
     P, L, U = _plu_decomp(A)
     y = _solve_lower_triangular(L, np.matmul(P, b))
     x = _solve_upper_triangular(U, y)
     return x
 
 
-def set_order(val, order):
-    """
-    Changes the order of a :class:`Dual` or :class:`Dual2` leaving floats and ints
-    unchanged.
-
-    Parameters
-    ----------
-    val : float, int, Dual or Dual2
-        The value to convert the order of.
-    order : int in [0, 1, 2]
-        The AD order to convert to. If ``val`` is float or int 0 will be used.
-
-    Returns
-    -------
-    float, int, Dual or Dual2
-    """
-    if order == 2 and isinstance(val, Dual):
-        return Dual2(val.real, val.vars, val.dual.tolist(), [])
-    elif order == 1 and isinstance(val, Dual2):
-        return Dual(val.real, val.vars, val.dual.tolist())
-    elif order == 0:
-        return float(val)
-    # otherwise:
-    #  - val is a Float or an Int
-    #  - val is a Dual and order == 1 OR val is Dual2 and order == 2
-    return val
-
-
-def set_order_convert(val, order, tag):
-    """
-    Convert a float, :class:`Dual` or :class:`Dual2` type to a specified alternate type.
-
-    Parameters
-    ----------
-    val : float, Dual or Dual2
-        The value to convert.
-    order : int
-        The AD order to convert the value to if necessary.
-    tag : list of str, optional
-        The variable name(s) if upcasting a float to a Dual or Dual2
-
-    Returns
-    -------
-    float, Dual, Dual2
-    """
-    if isinstance(val, (*FLOATS, *INTS)):
-        _ = [] if tag is None else tag
-        if order == 0:
-            return val
-        elif order == 1:
-            return Dual(val, _, [])
-        elif order == 2:
-            return Dual2(val, _, [], [])
-    # else val is Dual or Dual2 so convert directly
-    return set_order(val, order)
-
-
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
-
-DualTypes = Union[float, Dual, Dual2]
```

### Comparing `rateslib-1.1.1/rateslib/fx.py` & `rateslib-1.2.0/rateslib/fx.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,24 +152,24 @@
             raise ValueError(
                 f"`fx_rates` is underspecified: {self.q} currencies needs "
                 f"{self.q - 1} FX pairs, not {len(self.pairs)}."
             )
 
         # solve FX vector in linear system
         A = np.zeros((self.q, self.q), dtype="object")
-        b = np.ones(self.q, dtype="object")
         A[0, 0] = 1.0
+        b = np.zeros(self.q, dtype="object")
+        b[0] = 1.0
         for i, pair in enumerate(self.pairs):
             domestic_idx = self.currencies[pair[:3]]
             foreign_idx = self.currencies[pair[3:]]
             A[i + 1, domestic_idx] = -1.0
             A[i + 1, foreign_idx] = 1 / self.fx_rates[pair]
-            b[i + 1] = 0
         try:
-            x = dual_solve(A, b[:, np.newaxis])[:, 0]
+            x = dual_solve(A, b[:, np.newaxis], types=(Dual, Dual))[:, 0]  # TODO: (Dual, float)
         except ArithmeticError:
             return self._solve_error()
         if math.isnan(x[0].real):
             return self._solve_error()
 
         self.fx_vector = x
 
@@ -366,15 +366,15 @@
         Series
 
         Examples
         --------
         .. ipython:: python
 
            fxr = FXRates({"usdnok": 8.0})
-           fxr.positions(Dual(125000, "fx_usdnok", np.array([-15625])), "usd")
+           fxr.positions(Dual(125000, ["fx_usdnok"], [-15625]), "usd")
            fxr.positions(100, base="nok")
 
         """
         if isinstance(value, (float, int)):
             value = Dual(value, [], [])
         base = self.base if base is NoInput.blank else base.lower()
         _ = np.array([0 if ccy != base else float(value) for ccy in self.currencies_list])
```

### Comparing `rateslib-1.1.1/rateslib/instruments.py` & `rateslib-1.2.0/rateslib/instruments.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,39 +32,48 @@
 import numpy as np
 
 # from scipy.optimize import brentq
 from pandas.tseries.offsets import CustomBusinessDay
 from pandas import DataFrame, concat, Series, MultiIndex, isna
 
 from rateslib import defaults
-from rateslib.default import NoInput
-from rateslib.calendars import add_tenor, get_calendar, dcf, _get_years_and_months, _DCF1d
+from rateslib.calendars import add_tenor, get_calendar, dcf, _get_years_and_months
+from rateslib.default import NoInput, plot, _drb
 
-from rateslib.curves import Curve, index_left, LineCurve, CompositeCurve, IndexCurve, average_rate
-from rateslib.solver import Solver
+from rateslib.curves import Curve, index_left, LineCurve, IndexCurve, average_rate
+from rateslib.solver import Solver, quadratic_eqn
 from rateslib.periods import (
     Cashflow,
     FloatPeriod,
     _get_fx_and_base,
     IndexMixin,
     _disc_from_curve,
     _disc_maybe_from_curve,
+    FXCallPeriod,
+    FXPutPeriod,
 )
 from rateslib.legs import (
     FixedLeg,
     FloatLeg,
     FloatLegMtm,
     FixedLegMtm,
     ZeroFloatLeg,
     ZeroFixedLeg,
     ZeroIndexLeg,
     IndexFixedLeg,
 )
-from rateslib.dual import Dual, Dual2, DualTypes, dual_log, gradient
+from rateslib.dual import (
+    Dual,
+    Dual2,
+    DualTypes,
+    dual_log,
+    gradient,
+)
 from rateslib.fx import FXForwards, FXRates, forward_fx
+from rateslib.fx_volatility import FXDeltaVolSmile, FXVolObj
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
@@ -114,64 +123,35 @@
             elif defaults.curve_not_in_solver == "warn":
                 warnings.warn("`curve` not found in `solver`.", UserWarning)
                 return curve
             else:
                 raise ValueError("`curve` must be in `solver`.")
 
 
-def _get_curves_fx_and_base_maybe_from_solver(
-    curves_attr: Optional[Union[Curve, str, list]],
-    solver: Optional[Solver],
-    curves: Optional[Union[Curve, str, list]],
-    fx: Optional[Union[float, FXRates, FXForwards]],
-    base: Optional[str],
-    local_ccy: Optional[str],
-) -> tuple:
-    """
-    Parses the ``solver``, ``curves``, ``fx`` and ``base`` arguments in combination.
-
-    Parameters
-    ----------
-    curves_attr
-        The curves attribute attached to the class.
-    solver
-        The solver argument passed in the outer method.
-    curves
-        The curves argument passed in the outer method.
-    fx
-        The fx argument agrument passed in the outer method.
-
-    Returns
-    -------
-    tuple : (leg1 forecasting, leg1 discounting, leg2 forecasting, leg2 discounting), fx, base
-
-    Notes
-    -----
-    If only one curve is given this is used as all four curves.
-
-    If two curves are given the forecasting curve is used as the forecasting
-    curve on both legs and the discounting curve is used as the discounting
-    curve for both legs.
-
-    If three curves are given the single discounting curve is used as the
-    discounting curve for both legs.
-    """
-
-    # First process `base`.
+def _get_base_maybe_from_fx(
+    fx: Union[float, FXRates, FXForwards, NoInput],
+    base: Union[str, NoInput],
+    local_ccy: Union[str, NoInput],
+) -> Union[str, NoInput]:
     if fx is NoInput.blank and base is NoInput.blank:
         # base will not be inherited from a 2nd level inherited object, i.e.
         # from solver.fx, to preserve single currency instruments being defaulted
         # to their local currency.
         base_ = local_ccy
     elif isinstance(fx, (FXRates, FXForwards)) and base is NoInput.blank:
         base_ = fx.base
     else:
         base_ = base
+    return base_
 
-    # Second process `fx`
+
+def _get_fx_maybe_from_solver(
+    solver: Union[Solver, NoInput],
+    fx: Union[float, FXRates, FXForwards, NoInput],
+) -> Union[float, FXRates, FXForwards, NoInput]:
     if fx is NoInput.blank:
         if solver is NoInput.blank:
             fx_ = NoInput(0)
             # fx_ = 1.0
         elif solver is not NoInput.blank:
             if solver.fx is NoInput.blank:
                 fx_ = NoInput(0)
@@ -188,21 +168,31 @@
             warnings.warn(
                 "Solver contains an `fx` attribute but an `fx` argument has been "
                 "supplied which will be used but is not the same. This can lead "
                 "to calculation inconsistencies, mathematically.",
                 UserWarning,
             )
 
+    return fx_
+
+
+def _get_curves_maybe_from_solver(
+    curves_attr: Union[Curve, str, list, NoInput],
+    solver: Union[Solver, NoInput],
+    curves: Union[Curve, str, list, NoInput],
+) -> tuple:
     if curves is NoInput.blank and curves_attr is NoInput.blank:
-        return (NoInput(0), NoInput(0), NoInput(0), NoInput(0)), fx_, base_
+        return (NoInput(0), NoInput(0), NoInput(0), NoInput(0))
     elif curves is NoInput.blank:
         curves = curves_attr
 
-    if isinstance(curves, (Curve, str, CompositeCurve, dict)):
+    # if isinstance(curves, (Curve, str, dict)):  # All Curve types are sub-classes of Curve
+    if not isinstance(curves, (list, tuple)):
         curves = [curves]
+
     if solver is NoInput.blank:
 
         def check_curve(curve):
             if isinstance(curve, str):
                 raise ValueError("`curves` must contain Curve, not str, if `solver` not given.")
             elif curve is None or curve is NoInput(0):
                 return NoInput(0)
@@ -225,86 +215,129 @@
     elif len(curves_) == 2:
         curves_ *= 2
     elif len(curves_) == 3:
         curves_ += (curves_[1],)
     elif len(curves_) > 4:
         raise ValueError("Can only supply a maximum of 4 `curves`.")
 
+    return curves_
+
+
+def _get_curves_fx_and_base_maybe_from_solver(
+    curves_attr: Optional[Union[Curve, str, list]],
+    solver: Optional[Solver],
+    curves: Optional[Union[Curve, str, list]],
+    fx: Optional[Union[float, FXRates, FXForwards]],
+    base: Optional[str],
+    local_ccy: Optional[str],
+) -> tuple:
+    """
+    Parses the ``solver``, ``curves``, ``fx`` and ``base`` arguments in combination.
+
+    Parameters
+    ----------
+    curves_attr
+        The curves attribute attached to the class.
+    solver
+        The solver argument passed in the outer method.
+    curves
+        The curves argument passed in the outer method.
+    fx
+        The fx argument agrument passed in the outer method.
+
+    Returns
+    -------
+    tuple : (leg1 forecasting, leg1 discounting, leg2 forecasting, leg2 discounting), fx, base
+
+    Notes
+    -----
+    If only one curve is given this is used as all four curves.
+
+    If two curves are given the forecasting curve is used as the forecasting
+    curve on both legs and the discounting curve is used as the discounting
+    curve for both legs.
+
+    If three curves are given the single discounting curve is used as the
+    discounting curve for both legs.
+    """
+    # First process `base`.
+    base_ = _get_base_maybe_from_fx(fx, base, local_ccy)
+    # Second process `fx`
+    fx_ = _get_fx_maybe_from_solver(solver, fx)
+    # Third process `curves`
+    curves_ = _get_curves_maybe_from_solver(curves_attr, solver, curves)
     return curves_, fx_, base_
 
 
-# def _get_curves_and_fx_maybe_from_solver(
-#     solver: Optional[Solver],
-#     curves: Union[Curve, str, list],
-#     fx: Optional[Union[float, FXRates, FXForwards]],
-# ):
-#     """
-#     Parses the ``solver``, ``curves`` and ``fx`` arguments in combination.
-#
-#     Returns
-#     -------
-#     tuple : (leg1 forecasting, leg1 discounting, leg2 forecasting, leg2 discounting), fx
-#
-#     Notes
-#     -----
-#     If only one curve is given this is used as all four curves.
-#
-#     If two curves are given the forecasting curve is used as the forecasting
-#     curve on both legs and the discounting curve is used as the discounting
-#     curve for both legs.
-#
-#     If three curves are given the single discounting curve is used as the
-#     discounting curve for both legs.
-#     """
-#
-#     if fx is NoInput.blank:
-#         if solver is NoInput.blank:
-#             fx_ = None
-#             # fx_ = 1.0
-#         elif solver is not NoInput.blank:
-#             if solver.fx is NoInput.blank:
-#                 fx_ = None
-#                 # fx_ = 1.0
-#             else:
-#                 fx_ = solver.fx
-#     else:
-#         fx_ = fx
-#
-#     if curves is NoInput.blank:
-#         return (None, None, None, None), fx_
-#
-#     if isinstance(curves, (Curve, str)):
-#         curves = [curves]
-#     if solver is NoInput.blank:
-#         def check_curve(curve):
-#             if isinstance(curve, str):
-#                 raise ValueError(
-#                     "`curves` must contain Curve, not str, if `solver` not given."
-#                 )
-#             return curve
-#         curves_ = tuple(check_curve(curve) for curve in curves)
-#     else:
-#         try:
-#             curves_ = tuple(_get_curve_from_solver(curve, solver) for curve in curves)
-#         except KeyError:
-#             raise ValueError(
-#                 "`curves` must contain str curve `id` s existing in `solver` "
-#                 "(or its associated `pre_solvers`)"
-#             )
-#
-#     if len(curves_) == 1:
-#         curves_ *= 4
-#     elif len(curves_) == 2:
-#         curves_ *= 2
-#     elif len(curves_) == 3:
-#         curves_ += (curves_[1],)
-#     elif len(curves_) > 4:
-#         raise ValueError("Can only supply a maximum of 4 `curves`.")
-#
-#     return curves_, fx_
+def _get_vol_maybe_from_solver(
+    vol_attr: Union[DualTypes, str, FXDeltaVolSmile, NoInput],
+    vol: Union[DualTypes, str, FXDeltaVolSmile, NoInput],
+    solver: Union[Solver, NoInput],
+):
+    """
+    Try to retrieve a general vol input from a solver or the default vol object associated with instrument.
+
+    Parameters
+    ----------
+    vol_attr: DualTypes, str or FXDeltaVolSmile
+        The vol attribute associated with the object at initialisation.
+    vol: DualTypes, str of FXDeltaVolSMile
+        The specific vol argument supplied at price time. Will take precendence.
+    solver: Solver, optional
+        A solver object
+
+    Returns
+    -------
+    DualTypes, FXDeltaVolSmile or NoInput.blank
+    """
+    if vol is None:  # capture blank user input and reset
+        vol = NoInput(0)
+
+    if vol is NoInput.blank and vol_attr is NoInput.blank:
+        return NoInput(0)
+    elif vol is NoInput.blank:
+        vol = vol_attr
+
+    if solver is NoInput.blank:
+        if isinstance(vol, str):
+            raise ValueError(
+                "String `vol` ids require a `solver` to be mapped. No `solver` provided."
+            )
+        return vol
+    elif isinstance(vol, (float, Dual, Dual2)):
+        return vol
+    elif isinstance(vol, str):
+        return solver.pre_curves[vol]
+    else:  # vol is a Smile or Surface - check that it is in the Solver
+        try:
+            # it is a safeguard to load curves from solvers when a solver is
+            # provided and multiple curves might have the same id
+            _ = solver.pre_curves[vol.id]
+            if id(_) != id(vol):  # Python id() is a memory id, not a string label id.
+                raise ValueError(
+                    "A ``vol`` object has been supplied which has the same "
+                    f"`id` ('{vol.id}'),\nas one of those available as part of the "
+                    "Solver's collection but is not the same object.\n"
+                    "This is ambiguous and may lead to erroneous prices.\n"
+                )
+            return _
+        except AttributeError:
+            raise AttributeError(
+                "`vol` has no attribute `id`, likely it not a valid object, got: "
+                f"{vol}.\nSince a solver is provided have you missed labelling the `vol` "
+                f"of the instrument or supplying `vol` directly?"
+            )
+        except KeyError:
+            if defaults.curve_not_in_solver == "ignore":
+                return vol
+            elif defaults.curve_not_in_solver == "warn":
+                warnings.warn("`vol` not found in `solver`.", UserWarning)
+                return vol
+            else:
+                raise ValueError("`vol` must be in `solver`.")
 
 
 class Sensitivities:
     """
     Base class to add risk sensitivity calculations to an object with an ``npv()``
     method.
     """
@@ -312,14 +345,15 @@
     def delta(
         self,
         curves: Union[Curve, str, list, NoInput] = NoInput(0),
         solver: Union[Solver, NoInput] = NoInput(0),
         fx: Union[FXRates, FXForwards, NoInput] = NoInput(0),
         base: Union[str, NoInput] = NoInput(0),
         local: bool = False,
+        **kwargs,
     ):
         """
         Calculate delta risk of an *Instrument* against the calibrating instruments in a
         :class:`~rateslib.curves.Solver`.
 
         Parameters
         ----------
@@ -349,29 +383,30 @@
 
         Returns
         -------
         DataFrame
         """
         if solver is NoInput.blank:
             raise ValueError("`solver` is required for delta/gamma methods.")
-        npv = self.npv(curves, solver, fx, base, local=True)
+        npv = self.npv(curves, solver, fx, base, local=True, **kwargs)
         _, fx_, base_ = _get_curves_fx_and_base_maybe_from_solver(
             NoInput(0), solver, NoInput(0), fx, base, NoInput(0)
         )
         if local:
             base_ = NoInput(0)
         return solver.delta(npv, base_, fx_)
 
     def gamma(
         self,
         curves: Union[Curve, str, list, NoInput] = NoInput(0),
         solver: Union[Solver, NoInput] = NoInput(0),
         fx: Union[FXRates, FXForwards, NoInput] = NoInput(0),
         base: Union[str, NoInput] = NoInput(0),
         local: bool = False,
+        **kwargs,
     ):
         """
         Calculate cross-gamma risk of an *Instrument* against the calibrating instruments of a
         :class:`~rateslib.curves.Solver`.
 
         Parameters
         ----------
@@ -415,15 +450,15 @@
         if fx_ is not NoInput.blank:
             _ad2 = fx_._ad
             fx_._set_ad_order(2)
 
         _ad1 = solver._ad
         solver._set_ad_order(2)
 
-        npv = self.npv(curves, solver, fx_, base_, local=True)
+        npv = self.npv(curves, solver, fx_, base_, local=True, **kwargs)
         grad_s_sT_P = solver.gamma(npv, base_, fx_)
 
         # reset original order
         if fx_ is not NoInput.blank:
             fx_._set_ad_order(_ad2)
         solver._set_ad_order(_ad1)
 
@@ -820,15 +855,15 @@
     The below :class:`~rateslib.curves.Curve` is solved directly
     from a calibrating DF value on 1st Nov 2022.
 
     .. ipython:: python
 
        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="v")
        instruments = [(Value(dt(2022, 11, 1)), (curve,), {})]
-       solver = Solver([curve], instruments, [0.99])
+       solver = Solver([curve], [], instruments, [0.99])
        curve[dt(2022, 1, 1)]
        curve[dt(2022, 11, 1)]
        curve[dt(2023, 1, 1)]
     """
 
     def __init__(
         self,
@@ -876,15 +911,17 @@
             self.curves, solver, curves, NoInput(0), NoInput(0), "_"
         )
         metric = self.metric if metric is NoInput.blank else metric.lower()
         if metric == "curve_value":
             return curves[0][self.effective]
         elif metric == "cc_zero_rate":
             if curves[0]._base_type != "dfs":
-                raise TypeError("`curve` used with `metric`='cc_zero_rate' must be discount factor based.")
+                raise TypeError(
+                    "`curve` used with `metric`='cc_zero_rate' must be discount factor based."
+                )
             dcf_ = dcf(curves[0].node_dates[0], self.effective, self.convention)
             _ = (dual_log(curves[0][self.effective]) / -dcf_) * 100
             return _
         elif metric == "index_value":
             if not isinstance(curves[0], IndexCurve):
                 raise TypeError("`curve` used with `metric`='index_value' must be type IndexCurve.")
             _ = curves[0].index_value(self.effective)
@@ -897,65 +934,167 @@
     def cashflows(self, *args, **kwargs):
         raise NotImplementedError("`Value` instrument has no concept of cashflows.")
 
     def analytic_delta(self, *args, **kwargs):
         raise NotImplementedError("`Value` instrument has no concept of analytic delta.")
 
 
+class VolValue(BaseMixin):
+    """
+    A null *Instrument* which can be used within a :class:`~rateslib.solver.Solver`
+    to directly parametrise a *Vol* node, via some calculated metric.
+
+    Parameters
+    ----------
+    index_value : float, Dual, Dual2
+        The value of some index to the *VolSmile* or *VolSurface*.
+    metric: str, optional
+        The default metric to return from the ``rate`` method.
+    vol: str, FXDeltaVolSmile, optional
+        The associated object from which to determine the ``rate``.
+
+    Examples
+    --------
+    The below :class:`~rateslib.fx_volatility.FXDeltaVolSmile` is solved directly
+    from calibrating volatility values.
+
+    .. ipython:: python
+       :suppress:
+
+       from rateslib.fx_volatility import FXDeltaVolSmile
+       from rateslib.instruments import VolValue
+       from rateslib.solver import Solver
+
+    .. ipython:: python
+
+       smile = FXDeltaVolSmile(
+           nodes={0.25: 10.0, 0.5: 10.0, 0.75: 10.0},
+           eval_date=dt(2023, 3, 16),
+           expiry=dt(2023, 6, 16),
+           delta_type="forward",
+           id="VolSmile",
+       )
+       instruments = [
+           VolValue(0.25, vol="VolSmile"),
+           VolValue(0.5, vol="VolSmile"),
+           VolValue(0.75, vol=smile)
+       ]
+       solver = Solver(curves=[smile], instruments=instruments, s=[8.9, 7.8, 9.9])
+       smile[0.25]
+       smile[0.5]
+       smile[0.75]
+    """
+
+    def __init__(
+        self,
+        index_value: DualTypes,
+        # index_type: str = "delta",
+        # delta_type: str = NoInput(0),
+        metric: str = "vol",
+        vol: Union[NoInput, str, FXDeltaVolSmile] = NoInput(0),
+    ):
+        self.index_value = index_value
+        # self.index_type = index_type
+        # self.delta_type = delta_type
+        self.vol = vol
+        self.curves = NoInput(0)
+        self.metric = metric.lower()
+
+    def rate(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        vol: Union[DualTypes, FXDeltaVolSmile] = NoInput(0),
+        metric: str = "vol",
+    ):
+        """
+        Return a value derived from a *Curve*.
+
+        Parameters
+        ----------
+        curves : Curve, LineCurve, str or list of such
+            Uses only one *Curve*, the one given or the first in the list.
+        solver : Solver, optional
+            The numerical :class:`~rateslib.solver.Solver` that constructs
+            ``Curves`` from calibrating instruments.
+        fx : float, FXRates, FXForwards, optional
+            Not used.
+        base : str, optional
+            Not used.
+        metric: str in {"curve_value", "index_value", "cc_zero_rate"}, optional
+            Configures which type of value to return from the applicable *Curve*.
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        """
+        curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+            self.curves, solver, curves, fx, base, "_"
+        )
+        vol = _get_vol_maybe_from_solver(self.vol, vol, solver)
+        metric = self.metric if metric is NoInput.blank else metric.lower()
+
+        if metric == "vol":
+            return vol[self.index_value]
+
+        raise ValueError("`metric` must be in {'vol'}.")
+
+    def npv(self, *args, **kwargs):
+        raise NotImplementedError("`VolValue` instrument has no concept of NPV.")
+
+    def cashflows(self, *args, **kwargs):
+        raise NotImplementedError("`VolValue` instrument has no concept of cashflows.")
+
+    def analytic_delta(self, *args, **kwargs):
+        raise NotImplementedError("`VolValue` instrument has no concept of analytic delta.")
+
+
 class FXExchange(Sensitivities, BaseMixin):
     """
     Create a simple exchange of two currencies.
 
     Parameters
     ----------
     settlement : datetime
         The date of the currency exchange.
-    currency : str
-        The currency of the cashflow for which ``notional`` is applicable (3-digit code).
-    leg2_currency : str
-        The currency of the cashflow on the alternate *Leg*.
+    pair: str
+        The curreny pair of the exchange, e.g. "eurusd", using 3-digit iso codes.
     fx_rate : float, optional
         The FX rate used to derive the notional exchange on *Leg2*.
     notional : float
-        The cashflow amount for the initial currency.
+        The cashflow amount of the LHS currency.
     curves : Curve, LineCurve, str or list of such, optional
-        A single :class:`~rateslib.curves.Curve`,
-        :class:`~rateslib.curves.LineCurve` or id or a
-        list of such. A list defines the following curves in the order:
-
-        - Forecasting :class:`~rateslib.curves.Curve` or
-          :class:`~rateslib.curves.LineCurve` for ``leg1``.
-        - Discounting :class:`~rateslib.curves.Curve` for ``leg1``.
-        - Forecasting :class:`~rateslib.curves.Curve` or
-          :class:`~rateslib.curves.LineCurve` for ``leg2``.
-        - Discounting :class:`~rateslib.curves.Curve` for ``leg2``.
+        For *FXExchange* only discounting curves are required in each currency and not rate forecasting curves.
+        The signature should be: `[None, eur_curve, None, usd_curve]` for a "eurusd" pair.
     """
 
     def __init__(
         self,
         settlement: datetime,
-        currency: str,
-        leg2_currency: str,
+        pair: str,
         fx_rate: Union[float, NoInput] = NoInput(0),
         notional: Union[float, NoInput] = NoInput(0),
         curves: Union[list, str, Curve, NoInput] = NoInput(0),
     ):
         self.curves = curves
         self.settlement = settlement
-        self.pair = f"{currency.lower()}{leg2_currency.lower()}"
+        self.pair = pair.lower()
         self.leg1 = Cashflow(
-            notional=defaults.notional if notional is NoInput.blank else notional,
-            currency=currency.lower(),
+            notional=-defaults.notional if notional is NoInput.blank else -notional,
+            currency=self.pair[0:3],
             payment=settlement,
             stub_type="Exchange",
             rate=NoInput(0),
         )
         self.leg2 = Cashflow(
             notional=1.0,  # will be determined by setting fx_rate
-            currency=leg2_currency.lower(),
+            currency=self.pair[3:6],
             payment=settlement,
             stub_type="Exchange",
             rate=fx_rate,
         )
         self.fx_rate = fx_rate
 
     @property
@@ -1453,15 +1592,15 @@
         self,
         price: Union[float, Dual, Dual2],
         settlement: datetime,
         forward_settlement: datetime,
         repo_rate: Union[float, Dual, Dual2],
         convention: Union[str, NoInput] = NoInput(0),
         dirty: bool = False,
-        method: str = "proceeds"
+        method: str = "proceeds",
     ):
         """
         Return a forward price implied by a given repo rate.
 
         Parameters
         ----------
         price : float, Dual, or Dual2
@@ -1905,23 +2044,24 @@
         c = float(npv_price) - float(price)
         z_hat = -c / b
 
         # shift the curve to the first order approximation and fine tune with 2nd order approxim.
         curves[1]._set_ad_order(2)
         disc_curve = curves[1].shift(Dual2(z_hat, ["z_spread"], [], []), composite=False)
         npv_price = self.rate(curves=[curves[0], disc_curve], metric=metric)
-        a, b = (
+        a, b, c = (
             0.5 * gradient(npv_price, ["z_spread"], 2)[0][0],
             gradient(npv_price, ["z_spread"], 1)[0],
+            float(npv_price) - float(price),
         )
-        z_hat2 = _quadratic_equation(a, b, float(npv_price) - float(price))
+        z_hat2 = quadratic_eqn(a, b, c, x0=-c / b)["g"]
 
         # perform one final approximation albeit the additional price calculation slows calc time
         curves[1]._set_ad_order(0)
-        disc_curve = curves[1].shift(z_hat+z_hat2, composite=False)
+        disc_curve = curves[1].shift(z_hat + z_hat2, composite=False)
         npv_price = self.rate(curves=[curves[0], disc_curve], metric=metric)
         b = b + 2 * a * z_hat2  # forecast the new gradient
         c = float(npv_price) - float(price)
         z_hat3 = -c / b
 
         z = z_hat + z_hat2 + z_hat3
         curves[1]._set_ad_order(ad_)
@@ -2502,15 +2642,15 @@
            )
            gilt.ytm(
                price=141.0701315,
                settlement=dt(1999,5,27),
                dirty=True
            )
            gilt.ytm(Dual(141.0701315, ["price", "a", "b"], [1, -0.5, 2]), dt(1999, 5, 27), True)
-           gilt.ytm(Dual2(141.0701315, ["price", "a", "b"], [1, -0.5, 2]), dt(1999, 5, 27), True)
+           gilt.ytm(Dual2(141.0701315, ["price", "a", "b"], [1, -0.5, 2], []), dt(1999, 5, 27), True)
 
         """
 
         def root(y):
             # we set this to work in float arithmetic for efficiency. Dual is added
             # back below, see PR GH3
             return self._price_from_ytm(y, settlement, self.calc_mode, dirty) - float(price)
@@ -4302,19 +4442,19 @@
             settlement,
             f"-{self.basket[0].kwargs['settle']}B",
             None,
             self.basket[0].leg1.schedule.calendar,
         )
         unsorted_nodes = {
             today: 1.0,
-            **{_.leg1.schedule.termination: 1.0 for _ in self.basket}
+            **{_.leg1.schedule.termination: 1.0 for _ in self.basket},
         }
         bcurve = Curve(
             nodes=dict(sorted(unsorted_nodes.items(), key=lambda _: _[0])),
-            convention="act365f"  # use the most natural DCF without scaling
+            convention="act365f",  # use the most natural DCF without scaling
         )
         if dirty:
             metric = "dirty_price"
         else:
             metric = "clean_price"
         solver = Solver(
             curves=[bcurve],
@@ -4430,21 +4570,26 @@
         if not isinstance(repo_rate, (list, tuple)):
             r_ = (repo_rate,) * len(self.basket)
         else:
             r_ = repo_rate
 
         if dirty:
             net_basis_ = tuple(
-                bond.fwd_from_repo(prices[i], settlement, f_settlement, r_[i], convention, dirty=dirty)
-                - self.cfs[i] * future_price - bond.accrued(f_settlement)
+                bond.fwd_from_repo(
+                    prices[i], settlement, f_settlement, r_[i], convention, dirty=dirty
+                )
+                - self.cfs[i] * future_price
+                - bond.accrued(f_settlement)
                 for i, bond in enumerate(self.basket)
             )
         else:
             net_basis_ = tuple(
-                bond.fwd_from_repo(prices[i], settlement, f_settlement, r_[i], convention, dirty=dirty)
+                bond.fwd_from_repo(
+                    prices[i], settlement, f_settlement, r_[i], convention, dirty=dirty
+                )
                 - self.cfs[i] * future_price
                 for i, bond in enumerate(self.basket)
             )
         return net_basis_
 
     def implied_repo(
         self,
@@ -7328,16 +7473,17 @@
         """
         if self._is_mtm:
             self.leg2._set_periods(fx_arg)
             self.leg2_notional = self.leg2.notional
         else:
             self.leg2_notional = self.leg1.notional * -fx_arg
             self.leg2.notional = self.leg2_notional
-            self.leg2_amortization = self.leg1.amortization * -fx_arg
-            self.leg2.amortization = self.leg2_amortization
+            if self.kwargs["amortization"] is not NoInput.blank:
+                self.leg2_amortization = self.leg1.amortization * -fx_arg
+                self.leg2.amortization = self.leg2_amortization
 
     @property
     def _is_unpriced(self):
         if getattr(self, "_unpriced", None) is True:
             return True
         if self._fixed_rate_mixin and self._leg2_fixed_rate_mixin:
             # Fixed/Fixed where one leg is unpriced.
@@ -7490,17 +7636,22 @@
                 "`fixed_rate` on the non-solvable leg is NoInput.blank."
             )
 
         # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
         # Commercial use of this code, and/or copying and redistribution is prohibited.
         # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-        if not _is_float_tgt_leg and getattr(tgt_leg, "fixed_rate") is NoInput.blank:
-            # set the target fixed leg to a null fixed rate for calculation
-            tgt_leg.fixed_rate = 0.0
+        if not _is_float_tgt_leg:
+            tgt_leg_fixed_rate = getattr(tgt_leg, "fixed_rate")
+            if tgt_leg_fixed_rate is NoInput.blank:
+                # set the target fixed leg to a null fixed rate for calculation
+                tgt_leg.fixed_rate = 0.0
+            else:
+                # set the fixed rate to a float for calculation and no Dual Type crossing PR: XXX
+                tgt_leg.fixed_rate = float(tgt_leg_fixed_rate)
 
         self._set_fx_fixings(fx_)
         if self._is_mtm:
             self.leg2._do_not_repeat_set_periods = True
 
         tgt_leg_npv = tgt_leg.npv(tgt_fore_curve, tgt_disc_curve, fx_, base_)
         alt_leg_npv = alt_leg.npv(alt_fore_curve, alt_disc_curve, fx_, base_)
@@ -7556,14 +7707,18 @@
     """
     Create an FX swap simulated via a *Fixed-Fixed* :class:`XCS`.
 
     Parameters
     ----------
     args : dict
         Required positional args to :class:`XCS`.
+    pair : str, optional
+        The FX pair, e.g. "eurusd" as 3-digit ISO codes. If not given, fallsback to the base implementation of
+        *XCS* which defines separate inputs as ``currency`` and ``leg2_currency``. If overspecified, ``pair`` will
+        dominate.
     fx_fixings : float, FXForwards or None
         The initial FX fixing where leg 1 is considered the domestic currency. For
         example for an ESTR/SOFR XCS in 100mm EUR notional a value of 1.10 for `fx0`
         implies the notional on leg 2 is 110m USD. If `None` determines this
         dynamically.
     points : float, optional
         The pricing parameter for the FX Swap, which will determine the implicit
@@ -7662,18 +7817,17 @@
     Then we define the *FXSwap*. This in an unpriced instrument.
 
     .. ipython:: python
 
        fxs = FXSwap(
            effective=dt(2022, 1, 18),
            termination=dt(2022, 4, 19),
+           pair="usdeur",
            calendar="nyc",
-           currency="usd",
            notional=1000000,
-           leg2_currency="eur",
            curves=["usd", "usd", "eur", "eurusd"],
        )
 
     Now demonstrate the :meth:`~rateslib.instruments.FXSwap.npv` and
     :meth:`~rateslib.instruments.FXSwap.rate` methods:
 
     .. ipython:: python
@@ -7692,18 +7846,17 @@
     The following is an example of a fully priced *FXSwap* with split notionals.
 
     .. ipython:: python
 
        fxs = FXSwap(
            effective=dt(2022, 1, 18),
            termination=dt(2022, 4, 19),
+           pair="usdeur",
            calendar="nyc",
-           currency="usd",
            notional=1000000,
-           leg2_currency="eur",
            curves=["usd", "usd", "eur", "eurusd"],
            fx_fixings=0.90,
            split_notional=1001500,
            points=-49.0
        )
        fxs.npv(curves=[None, usd, None, eurusd], fx=fxf)
        fxs.cashflows(curves=[None, usd, None, eurusd], fx=fxf)
@@ -7748,20 +7901,24 @@
         Will set the fixed rate, if not zero, for leg1, given provided split not or forecast splnot.
 
         self._split_notional is used as a temporary storage when mid market price is determined.
         """
         if not self._is_split:
             self._split_notional = self.kwargs["notional"]
             # fixed rate at zero remains
+
+        # a split notional is given by a user and then this is set and never updated.
         elif self.kwargs["split_notional"] is not NoInput.blank:
             if at_init:  # this will be run for one time only at initialisation
                 self._split_notional = self.kwargs["split_notional"]
                 self._set_leg1_fixed_rate()
             else:
                 return None
+
+        # else new pricing parameters will affect and unpriced split notional
         else:
             if at_init:
                 self._split_notional = None
             else:
                 dt1, dt2 = self.leg1.periods[0].payment, self.leg1.periods[2].payment
                 self._split_notional = self.kwargs["notional"] * curve[dt1] / curve[dt2]
                 self._set_leg1_fixed_rate()
@@ -7771,32 +7928,37 @@
             -self.leg1.notional * self.leg1.periods[1].dcf
         )
         self.leg1.fixed_rate = fixed_rate * 100
 
     def __init__(
         self,
         *args,
+        pair: Union[str, NoInput] = NoInput(0),
         fx_fixings: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
         points: Union[float, NoInput] = NoInput(0),
         split_notional: Union[float, NoInput] = NoInput(0),
         **kwargs,
     ):
         self._parse_split_flag(fx_fixings, points, split_notional)
+        currencies = {}
+        if isinstance(pair, str):
+            # TODO for version 2.0 should look to deprecate 'currency' and 'leg2_currency' as allowable inputs.
+            currencies = {"currency": pair.lower()[0:3], "leg2_currency": pair.lower()[3:6]}
 
         kwargs_overrides = dict(  # specific args for FXSwap passed to the Base XCS
             fixed=True,
             leg2_fixed=True,
             leg2_mtm=False,
             fixed_rate=0.0,
             frequency="Z",
             leg2_frequency="Z",
             leg2_fixed_rate=NoInput(0),
             fx_fixings=fx_fixings,
         )
-        super().__init__(*args, **{**kwargs, **kwargs_overrides})
+        super().__init__(*args, **{**kwargs, **kwargs_overrides, **currencies})
 
         self.kwargs["split_notional"] = split_notional
         self._set_split_notional(curve=None, at_init=True)
         # self._initialise_fx_fixings(fx_fixings)
         self.points = points
 
     @property
@@ -7900,14 +8062,1463 @@
     ):
         if self._is_unpriced:
             self._set_pricing_mid(curves, solver, fx)
         ret = super().cashflows(curves, solver, fx, base)
         return ret
 
 
+# FX Options
+
+
+class FXOption(Sensitivities, metaclass=ABCMeta):
+    """
+    Create an *FX Option*.
+
+    Parameters
+    ----------
+    pair: str
+        The currency pair for the FX rate which the option is settled. 3-digit code, e.g. "eurusd".
+    expiry: datetime, str
+        The expiry of the option.
+    notional: float
+        The amount in ccy1 (left side of `pair`) on which the option is based.
+    strike: float, Dual, Dual2, str in {"atm_forward", "atm_spot", "atm_delta", "[float]d"}
+        The strike value of the option.
+        If str there are four possibilities as above. If giving a specific delta should end
+        with a 'd' for delta e.g. "-25d". Put deltas should be input including negative sign.
+    eval_date: datetime, optional
+        The date from which to evaluate a string tenor expiry.
+    modifier : str, optional
+        The modification rule, in {"F", "MF", "P", "MP"} for date evaluation.
+    calendar : calendar or str, optional
+        The holiday calendar object to use. If str, looks up named calendar from
+        static data.
+    delivery_lag: int, optional
+        The number of business days after expiry that the physical settlement of the FX exchange occurs.
+    payment_lag: int or datetime, optional
+        The number of business days after expiry to pay premium. If a *datetime* is given this will
+        set the premium date explicitly.
+    premium: float
+        The amount paid for the option.
+    premium_ccy: str
+        The currency in which the premium is paid. Can *only* be one of the two currencies in `pair`.
+    option_fixing: float
+        The value determined at expiry to set the moneyness of the option.
+    delta_type: str in {"spot", "forward"}
+        When deriving strike from delta use the equation associated with spot or forward delta.
+        If premium currency is ccy1 (left side of `pair`) then this will produce **premium adjusted**
+        delta values. If the `premium_ccy` is ccy2 (right side of `pair`) then delta values are
+        **unadjusted**.
+    metric: str in {"pips_or_%", "vol", "premium"}, optional
+        The pricing metric returned by the ``rate`` method.
+    curves : Curve, LineCurve, str or list of such, optional
+        For *FXOptions* curves should be expressed as a list with the discount curves
+        entered either as *Curve* or str for discounting cashflows in the appropriate currency
+        with a consistent collateral on each side. E.g. *[None, "eurusd", None, "usdusd"]*.
+        Forecasting curves are not relevant.
+    spec : str, optional
+        An identifier to pre-populate many field with conventional values. See
+        :ref:`here<defaults-doc>` for more info and available values.
+
+    """
+
+    style = "european"
+    _pricing = None
+    _rate_scalar = 1.0
+
+    def __init__(
+        self,
+        pair: str,
+        expiry: Union[datetime, str],
+        notional: float = NoInput(0),
+        eval_date: Union[datetime, NoInput] = NoInput(0),
+        calendar: Union[CustomBusinessDay, str, NoInput] = NoInput(0),
+        modifier: Union[str, NoInput] = NoInput(0),
+        delivery_lag: Union[int, NoInput] = NoInput(0),
+        strike: Union[DualTypes, str, NoInput] = NoInput(0),
+        premium: Union[float, NoInput] = NoInput(0),
+        premium_ccy: Union[str, NoInput] = NoInput(0),
+        payment_lag: Union[str, datetime, NoInput] = NoInput(0),
+        option_fixing: Union[float, NoInput] = NoInput(0),
+        delta_type: Union[float, NoInput] = NoInput(0),
+        metric: Union[str, NoInput] = NoInput(0),
+        curves: Union[list, str, Curve, NoInput] = NoInput(0),
+        vol: Union[str, FXDeltaVolSmile, NoInput] = NoInput(0),
+        spec: Union[str, NoInput] = NoInput(0),
+    ):
+        self.kwargs = dict(
+            pair=pair,
+            expiry=expiry,
+            notional=notional,
+            strike=strike,
+            premium=premium,
+            premium_ccy=premium_ccy,
+            option_fixing=option_fixing,
+            payment_lag=payment_lag,
+            delivery_lag=delivery_lag,
+            calendar=calendar,
+            modifier=modifier,
+            delta_type=delta_type,
+            metric=metric,
+        )
+        self.kwargs = _push(spec, self.kwargs)
+
+        self.kwargs = _update_with_defaults(
+            self.kwargs,
+            {
+                "delta_type": defaults.fx_delta_type,
+                "notional": defaults.notional,
+                "modifier": defaults.modifier,
+                "metric": "pips_or_%",
+                "delivery_lag": defaults.fx_delivery_lag,
+                "payment_lag": defaults.payment_lag,
+                "premium_ccy": self.kwargs["pair"][3:],
+            },
+        )
+
+        if isinstance(self.kwargs["expiry"], str):
+            if not isinstance(eval_date, datetime):
+                raise ValueError("`expiry` as string tenor requires `eval_date`.")
+            self.kwargs["expiry"] = add_tenor(
+                eval_date,
+                self.kwargs["expiry"],
+                self.kwargs["modifier"],
+                self.kwargs["calendar"],
+                NoInput(0),
+            )
+
+        if isinstance(self.kwargs["delivery_lag"], datetime):
+            self.kwargs["delivery"] = self.kwargs["delivery_lag"]
+        else:
+            self.kwargs["delivery"] = add_tenor(
+                self.kwargs["expiry"],
+                f"{self.kwargs['delivery_lag']}b",
+                "F",
+                self.kwargs["calendar"],
+                NoInput(0),
+            )
+
+        if isinstance(self.kwargs["payment_lag"], datetime):
+            self.kwargs["payment"] = self.kwargs["payment_lag"]
+        else:
+            self.kwargs["payment"] = add_tenor(
+                self.kwargs["expiry"],
+                f"{self.kwargs['payment_lag']}b",
+                "F",
+                self.kwargs["calendar"],
+                NoInput(0),
+            )
+
+        if self.kwargs["premium_ccy"] not in [
+            self.kwargs["pair"][:3],
+            self.kwargs["pair"][3:],
+        ]:
+            raise ValueError(
+                f"`premium_ccy`: '{self.kwargs['premium_ccy']}' must be one of option "
+                f"currency pair: '{self.kwargs['pair']}'."
+            )
+        elif self.kwargs["premium_ccy"] == self.kwargs["pair"][3:]:
+            self.kwargs["metric_period"] = (
+                "pips" if self.kwargs["metric"] == "pips_or_%" else self.kwargs["metric"]
+            )
+            self.kwargs["delta_adjustment"] = ""
+        else:
+            self.kwargs["metric_period"] = (
+                "percent" if self.kwargs["metric"] == "pips_or_%" else self.kwargs["metric"]
+            )
+            self.kwargs["delta_adjustment"] = "_pa"
+
+        # nothing to inherit or negate.
+        # self.kwargs = _inherit_or_negate(self.kwargs)  # inherit or negate the complete arg list
+
+        self._validate_strike_and_premiums()
+
+        self.vol = vol
+        self.curves = curves
+        self.spec = spec
+
+    def _validate_strike_and_premiums(self):
+        if self.kwargs["strike"] is NoInput.blank:
+            raise ValueError("`strike` for FXOption must be set to numeric or string value.")
+        if isinstance(self.kwargs["strike"], str) and self.kwargs["premium"] is not NoInput.blank:
+            raise ValueError(
+                "FXOption with string delta as `strike` cannot be initialised with a known `premium`.\n"
+                "Either set `strike` as a defined numeric value, or remove the `premium`."
+            )
+
+    def _set_strike_and_vol(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        vol: float = NoInput(0),
+    ):
+        # If the strike for the option is not set directly it must be inferred
+        # and some of the pricing elements associated with this strike definition must
+        # be captured for use in subsequent formulae.
+
+        if fx is NoInput.blank:
+            raise ValueError(
+                "An FXForwards object for `fx` is required for FXOption pricing.\n"
+                "If this instrument is part of a Solver, have you omitted the `fx` input?"
+            )
+
+        self._pricing = {
+            "vol": vol,
+            "k": self.kwargs["strike"],
+            "delta_index": None,
+            "spot": fx.pairs_settlement[self.kwargs["pair"]],
+            "t_e": self.periods[0]._t_to_expiry(curves[3].node_dates[0]),
+            "f_d": fx.rate(self.kwargs["pair"], self.kwargs["delivery"]),
+        }
+        w_deli = curves[1][self.kwargs["delivery"]]
+        w_spot = curves[1][self._pricing["spot"]]
+
+        if isinstance(self.kwargs["strike"], str):
+            method = self.kwargs["strike"].lower()
+
+            if method == "atm_forward":
+                self._pricing["k"] = fx.rate(self.kwargs["pair"], self.kwargs["delivery"])
+
+            elif method == "atm_spot":
+                self._pricing["k"] = fx.rate(self.kwargs["pair"], self._pricing["spot"])
+
+            elif method == "atm_delta":
+                self._pricing["k"], self._pricing["delta_index"] = self.periods[
+                    0
+                ]._strike_and_index_from_atm(
+                    delta_type=self.periods[0].delta_type,
+                    vol=vol,
+                    w_deli=w_deli,
+                    w_spot=w_spot,
+                    f=self._pricing["f_d"],
+                    t_e=self._pricing["t_e"],
+                )
+
+            elif method[-1] == "d":  # representing delta
+                # then strike is commanded by delta
+                self._pricing["k"], self._pricing["delta_index"] = self.periods[
+                    0
+                ]._strike_and_index_from_delta(
+                    delta=float(self.kwargs["strike"][:-1]) / 100.0,
+                    delta_type=self.kwargs["delta_type"] + self.kwargs["delta_adjustment"],
+                    vol=vol,
+                    w_deli=w_deli,
+                    w_spot=w_spot,
+                    f=self._pricing["f_d"],
+                    t_e=self._pricing["t_e"],
+                )
+
+            # TODO: this may affect solvers dependent upon sensitivity to vol for changing strikes.
+            # set the strike as a float without any sensitivity. Trade definition is a fixed quantity
+            # at this stage. Similar to setting a fixed rate as a float on an unpriced IRS for mid-market.
+            self.periods[0].strike = float(self._pricing["k"])
+
+        if isinstance(vol, FXVolObj):
+            if self._pricing["delta_index"] is None:
+                self._pricing["delta_index"], self._pricing["vol"], _ = vol.get_from_strike(
+                    k=self._pricing["k"],
+                    phi=self.periods[0].phi,
+                    f=self._pricing["f_d"],
+                    w_deli=w_deli,
+                    w_spot=w_spot,
+                    expiry=self.kwargs["expiry"]
+                )
+            else:
+                self._pricing["vol"] = vol._get_index(self._pricing["delta_index"], self.kwargs["expiry"])
+
+    def _set_premium(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+    ):
+        if self.kwargs["premium"] is NoInput.blank:
+            # then set the CashFlow to mid-market
+            try:
+                npv = self.periods[0].npv(curves[1], curves[3], fx, vol=self._pricing["vol"])
+            except AttributeError:
+                raise ValueError(
+                    "`premium` has not been configured for the specified FXOption.\nThis is "
+                    "normally determined at mid-market from the given `curves` and `vol` but "
+                    "in this case these values do not provide a valid calculation. "
+                    "If not required, initialise the "
+                    "FXOption with a `premium` of 0.0, and this will be avoided."
+                )
+            m_p = self.kwargs["payment"]
+            if self.kwargs["premium_ccy"] == self.kwargs["pair"][:3]:
+                premium = npv / (curves[3][m_p] * fx.rate("eurusd", m_p))
+            else:
+                premium = npv / curves[3][m_p]
+
+            self.periods[1].notional = float(premium)
+
+    def _get_vol_curves_fx_and_base_maybe_from_solver(self, solver, curves, fx, base, vol):
+        """
+        Parses the inputs including the instrument's attributes and also validates them
+        """
+        curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+            self.curves, solver, curves, fx, base, self.kwargs["pair"][3:]
+        )
+        vol = _get_vol_maybe_from_solver(self.vol, vol, solver)
+        if isinstance(vol, FXDeltaVolSmile) and vol.eval_date != curves[1].node_dates[0]:
+            raise ValueError(
+                "The `eval_date` on the FXDeltaVolSmile and the Curve do not align.\n"
+                "Aborting calculation to avoid pricing errors."
+            )
+        return curves, fx, base, vol
+
+    def rate(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        vol: Union[float, FXDeltaVolSmile, NoInput] = NoInput(0),
+        metric: Union[str, NoInput] = NoInput(0),
+    ):
+        """
+        Return various pricing metrics of the *FX Option*.
+
+        Parameters
+        ----------
+        curves : list of Curve
+            Curves for discounting cashflows. List follows the structure used by IRDs and
+            should be given as:
+            `[None, Curve for domestic ccy, None, Curve for foreign ccy]`
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx: FXForwards
+            The object to project the relevant forward and spot FX rates.
+        base: str, optional
+            Not used by `rate`.
+        vol: float, Dual, Dual2 or FXDeltaVolSmile
+            The volatility used in calculation.
+        metric: str in {"pips_or_%", "vol", "premium"}, optional
+            The pricing metric type to return. See notes.
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        Notes
+        -----
+        The available choices for the pricing ``metric`` that can be used are:
+
+        - *"pips_or_%"*: if the ``premium_ccy`` is the foreign (RHS) currency then *pips* will be returned, else
+          if the premium is the domestic (LHS) currency then % of notional will be returned.
+
+        - *"vol"*: the volatility used to price the option at that strike / delta is returned.
+
+        - *"premium"*: the monetary amount in ``premium_ccy`` payable at the payment date is returned.
+
+        If calculating the *rate* of an *FXOptionStrat* then the attributes ``rate_weight`` and ``rate_weight_vol``
+        will be used to combine the output for each individual *FXOption* within the strategy.
+
+        *FXStrangle* and *FXBrokerFly* have the additional ``metric`` *'single_vol'* which is a more complex and
+        integrated calculation.
+        """
+        curves, fx, _base, vol = self._get_vol_curves_fx_and_base_maybe_from_solver(
+            solver, curves, fx, base, vol
+        )
+        self._set_strike_and_vol(curves, fx, vol)
+        # self._set_premium(curves, fx)
+
+        metric = _drb(self.kwargs["metric"], metric)
+        if metric == "vol":
+            return self._pricing["vol"]
+
+        _ = self.periods[0].rate(curves[1], curves[3], fx, NoInput(0), False, self._pricing["vol"])
+        if metric == "premium":
+            if self.periods[0].metric == "pips":
+                _ *= self.periods[0].notional / 10000
+            else:  # == "percent"
+                _ *= self.periods[0].notional / 100
+        return _
+
+    def npv(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        curves, fx, base, vol = self._get_vol_curves_fx_and_base_maybe_from_solver(
+            solver, curves, fx, base, vol
+        )
+        self._set_strike_and_vol(curves, fx, vol)
+        self._set_premium(curves, fx)
+
+        opt_npv = self.periods[0].npv(curves[1], curves[3], fx, base, local, vol)
+        if self.kwargs["premium_ccy"] == self.kwargs["pair"][:3]:
+            disc_curve = curves[1]
+        else:
+            disc_curve = curves[3]
+        prem_npv = self.periods[1].npv(NoInput(0), disc_curve, fx, base, local)
+        if local:
+            return {k: opt_npv.get(k, 0) + prem_npv.get(k, 0) for k in set(opt_npv) | set(prem_npv)}
+        else:
+            return opt_npv + prem_npv
+
+    def analytic_greeks(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        """
+        Return various pricing metrics of the *FX Option*.
+
+        Parameters
+        ----------
+        curves : list of Curve
+            Curves for discounting cashflows. List follows the structure used by IRDs and
+            should be given as:
+            `[None, Curve for domestic ccy, None, Curve for foreign ccy]`
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx: FXForwards
+            The object to project the relevant forward and spot FX rates.
+        base: str, optional
+            Not used by `analytic_greeks`.
+        local: bool,
+            Not used by `analytic_greeks`.
+        vol: float, or FXDeltaVolSmile
+            The volatility used in calculation.
+
+        Returns
+        -------
+        float, Dual, Dual2
+        """
+        curves, fx, base, vol = self._get_vol_curves_fx_and_base_maybe_from_solver(
+            solver, curves, fx, base, vol
+        )
+        self._set_strike_and_vol(curves, fx, vol)
+        # self._set_premium(curves, fx)
+
+        return self.periods[0].analytic_greeks(
+            curves[1],
+            curves[3],
+            fx,
+            base,
+            local,
+            vol,
+            premium=NoInput(0),
+        )
+
+    def _plot_payoff(
+        self,
+        range: Union[list[float], NoInput] = NoInput(0),
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        """
+        Mechanics to determine (x,y) coordinates for payoff at expiry plot.
+        """
+        curves, fx, base, vol = self._get_vol_curves_fx_and_base_maybe_from_solver(
+            solver, curves, fx, base, vol
+        )
+        self._set_strike_and_vol(curves, fx, vol)
+        # self._set_premium(curves, fx)
+
+        x, y = self.periods[0]._payoff_at_expiry(range)
+        return x, y
+
+    def plot_payoff(
+        self,
+        range: Union[list[float], NoInput] = NoInput(0),
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        x, y = self._plot_payoff(range, curves, solver, fx, base, local, vol)
+        return plot(x, [y])
+
+
+class FXCall(FXOption):
+    """
+    Create an *FX Call* option.
+
+    For parameters see :class:`~rateslib.instruments.FXOption`.
+    """
+
+    style = "european"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.periods = [
+            FXCallPeriod(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery=self.kwargs["delivery"],
+                payment=self.kwargs["payment"],
+                strike=NoInput(0)
+                if isinstance(self.kwargs["strike"], str)
+                else self.kwargs["strike"],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"] + self.kwargs["delta_adjustment"],
+                metric=self.kwargs["metric_period"],
+            ),
+            Cashflow(
+                notional=self.kwargs["premium"],
+                payment=self.kwargs["payment"],
+                currency=self.kwargs["premium_ccy"],
+                stub_type="Premium",
+            ),
+        ]
+
+
+class FXPut(FXOption):
+    """
+    Create an *FX Put* option.
+
+    For parameters see :class:`~rateslib.instruments.FXOption`.
+    """
+
+    style = "european"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.periods = [
+            FXPutPeriod(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery=self.kwargs["delivery"],
+                payment=self.kwargs["payment"],
+                strike=NoInput(0)
+                if isinstance(self.kwargs["strike"], str)
+                else self.kwargs["strike"],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"] + self.kwargs["delta_adjustment"],
+                metric=self.kwargs["metric_period"],
+            ),
+            Cashflow(
+                notional=self.kwargs["premium"],
+                payment=self.kwargs["payment"],
+                currency=self.kwargs["premium_ccy"],
+                stub_type="Premium",
+            ),
+        ]
+
+
+class FXOptionStrat:
+    """
+    Create a custom option strategy composed of a list of :class:`~rateslib.instruments.FXOption`.
+
+    Parameters
+    ----------
+    options: list
+        The *FXOptions* which make up the strategy.
+    rate_weight: list
+        The multiplier for the *'pips_or_%'* metric that sums the options to a final *rate*.
+    rate_weight_vol: list
+        The multiplier for the *'vol'* metric that sums the options to a final *rate*.
+    """
+
+    _pricing = {}
+
+    def __init__(
+        self,
+        options: list[FXOption],
+        rate_weight: list[float],
+        rate_weight_vol: list[float],
+    ):
+        self.periods = options
+        self.rate_weight = rate_weight
+        self.rate_weight_vol = rate_weight_vol
+        if len(self.periods) != len(self.rate_weight) or len(self.periods) != len(
+            self.rate_weight_vol
+        ):
+            raise ValueError(
+                "`rate_weight` and `rate_weight_vol` must have same length as `options`."
+            )
+
+    def _vol_as_list(self, vol, solver):
+        """Standardise a vol input over the list of periods"""
+        if not isinstance(vol, (list, tuple)):
+            vol = [vol] * len(self.periods)
+        return [_get_vol_maybe_from_solver(self.vol, _, solver) for _ in vol]
+
+    def rate(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        vol: Union[list[float], float] = NoInput(0),
+        metric: Union[str, NoInput] = NoInput(0),  # "pips_or_%",
+    ):
+        """
+        Return the mid-market rate of an option strategy.
+
+        See :meth:`~rateslib.instruments.FXOption.rate`.
+        """
+        curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+            self.curves, solver, curves, fx, base, self.kwargs["pair"][3:]
+        )
+        vol = self._vol_as_list(vol, solver)
+
+        metric = metric if metric is not NoInput.blank else self.kwargs["metric"]
+        map_ = {
+            "pips_or_%": self.rate_weight,
+            "vol": self.rate_weight_vol,
+            "premium": [1.0] * len(self.periods),
+        }
+        weights = map_[metric]
+
+        _ = 0.0
+        for option, vol_, weight in zip(self.periods, vol, weights):
+            _ += option.rate(curves, solver, fx, base, vol_, metric) * weight
+        return _
+
+    def npv(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: Union[list[float], float] = NoInput(0),
+    ):
+        if not isinstance(vol, list):
+            vol = [vol] * len(self.periods)
+
+        results = [
+            option.npv(curves, solver, fx, base, local, vol_)
+            for (option, vol_) in zip(self.periods, vol)
+        ]
+
+        if local:
+            _ = DataFrame(results).fillna(0.0)
+            _ = _.sum()
+            _ = _.to_dict()
+        else:
+            _ = sum(results)
+        return _
+
+    def _plot_payoff(
+        self,
+        range: Union[list[float], NoInput] = NoInput(0),
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: Union[list[float], float] = NoInput(0),
+    ):
+        if not isinstance(vol, list):
+            vol = [vol] * len(self.periods)
+
+        y = None
+        for option, vol_ in zip(self.periods, vol):
+            x, y_ = option._plot_payoff(range, curves, solver, fx, base, local, vol_)
+            if y is None:
+                y = y_
+            else:
+                y += y_
+
+        return x, y
+
+    def _set_notionals(self, notional):
+        """Set the notionals on each option period. Mainly used by Brokerfly for vega neutral strangle and straddle."""
+        for option in self.periods:
+            option.periods[0].notional = notional
+
+    def analytic_greeks(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        """
+        Return various pricing metrics of the *FX Option*.
+
+        Parameters
+        ----------
+        curves : list of Curve
+            Curves for discounting cashflows. List follows the structure used by IRDs and should be given as:
+            `[None, Curve for domestic ccy, None, Curve for foreign ccy]`
+        solver : Solver, optional
+            The numerical :class:`Solver` that constructs ``Curves`` from calibrating
+            instruments.
+        fx : float, FXRates, FXForwards, optional
+            The immediate settlement FX rate that will be used to convert values
+            into another currency. A given `float` is used directly. If giving a
+            ``FXRates`` or ``FXForwards`` object, converts from local currency
+            into ``base``.
+        base : str, optional
+            The base currency to convert cashflows into (3-digit code), set by default.
+            Only used if ``fx`` is an ``FXRates`` or ``FXForwards`` object.
+
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        Notes
+        ------
+
+        """
+
+        # implicitly call set_pricing_mid for unpriced parameters
+        # this is important for Strategies whose options are
+        # dependent upon each other, e.g. Strangle. (RR and Straddle do not have
+        # interdependent options)
+        self.rate(curves, solver, fx, base, vol)
+
+        curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+            self.curves, solver, curves, fx, base, self.kwargs["pair"][3:]
+        )
+        vol = self._vol_as_list(vol, solver)
+
+        gks = []
+        for option, _vol in zip(self.periods, vol):
+            # by calling on the OptionPeriod directly the strike is maintained from rate call.
+            gks.append(
+                option.periods[0].analytic_greeks(
+                    curves[1],
+                    curves[3],
+                    fx,
+                    base,
+                    local,
+                    _vol,
+                    option.kwargs["premium"],
+                )
+            )
+
+        _unit_attrs = ["delta", "gamma", "vega", "vomma", "vanna", "_kega", "_kappa", "__bs76"]
+        _ = {}
+        for attr in _unit_attrs:
+            _[attr] = sum(gk[attr] * self.rate_weight[i] for i, gk in enumerate(gks))
+
+        _notional_attrs = [
+            f"delta_{self.kwargs['pair'][:3]}",
+            f"gamma_{self.kwargs['pair'][:3]}_1%",
+            f"vega_{self.kwargs['pair'][3:]}",
+        ]
+        for attr in _notional_attrs:
+            _[attr] = sum(gk[attr] * self.rate_weight[i] for i, gk in enumerate(gks))
+
+        _.update(
+            {
+                "__class": "FXOptionStrat",
+                "__options": gks,
+                "__delta_type": gks[0]["__delta_type"],
+                "__notional": self.kwargs["notional"],
+            }
+        )
+        return _
+
+
+class FXRiskReversal(FXOptionStrat, FXOption):
+    """
+    Create an *FX Risk Reversal* option strategy.
+
+    For additional arguments see :class:`~rateslib.instruments.FXOption`.
+
+    Parameters
+    ----------
+    args: tuple
+        Positional arguments to :class:`~rateslib.instruments.FXOption`.
+    strike: 2-element sequence
+        The first element is applied to the lower strike put and the
+        second element applied to the higher strike call, e.g. `["-25d", "25d"]`.
+    premium: 2-element sequence, optional
+        The premiums associated with each option of the risk reversal.
+    metric: str, optional
+        The default metric to apply in the method :meth:`~rateslib.instruments.FXOptionStrat.rate`
+    kwargs: tuple
+        Keyword arguments to :class:`~rateslib.instruments.FXOption`.
+
+    Notes
+    -----
+    When supplying ``strike`` as a string delta the strike will be determined at price time from
+    the provided volatility.
+
+    Buying a *Risk Reversal* equates to selling a lower strike :class:`~rateslib.instruments.FXPut`
+    and buying a higher strike :class:`~rateslib.instruments.FXCall`.
+
+    This class is essentially an alias constructor for an
+    :class:`~rateslib.instruments.FXOptionStrat` where the number
+    of options and their definitions and nominals have been specifically set.
+    """
+
+    rate_weight = [-1.0, 1.0]
+    rate_weight_vol = [-1.0, 1.0]
+    _rate_scalar = 100.0
+
+    def __init__(
+        self,
+        *args,
+        strike=[NoInput(0), NoInput(0)],
+        premium=[NoInput(0), NoInput(0)],
+        metric: str = "vol",
+        **kwargs,
+    ):
+        super(FXOptionStrat, self).__init__(
+            *args,
+            strike=strike,
+            premium=premium,
+            **kwargs,
+        )
+        self.kwargs["metric"] = metric
+        self.periods = [
+            FXPut(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"][0],
+                notional=-self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][0],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+            FXCall(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"][1],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][1],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+        ]
+
+    def _validate_strike_and_premiums(self):
+        """called as part of init, specific validation rules for straddle"""
+        if any(_ is NoInput.blank for _ in self.kwargs["strike"]):
+            raise ValueError(
+                "`strike` for FXRiskReversal must be set to list of 2 numeric or string values."
+            )
+        for k, p in zip(self.kwargs["strike"], self.kwargs["premium"]):
+            if isinstance(k, str) and p != NoInput.blank:
+                raise ValueError(
+                    "FXRiskReversal with string delta as `strike` cannot be initialised with a known `premium`.\n"
+                    "Either set `strike` as a defined numeric value, or remove the `premium`."
+                )
+
+
+class FXStraddle(FXOptionStrat, FXOption):
+    """
+    Create an *FX Straddle* option strategy.
+
+    For additional arguments see :class:`~rateslib.instruments.FXOption`.
+
+    Parameters
+    ----------
+    args: tuple
+        Positional arguments to :class:`~rateslib.instruments.FXOption`.
+    premium: 2-element sequence, optional
+        The premiums associated with each option of the straddle.
+    metric: str, optional
+        The default metric to apply in the method :meth:`~rateslib.instruments.FXOptionStrat.rate`
+    kwargs: tuple
+        Keyword arguments to :class:`~rateslib.instruments.FXOption`.
+
+    Notes
+    -----
+    When supplying ``strike`` as a string delta the strike will be determined at price time from
+    the provided volatility and FX forward market.
+
+    Buying a *Straddle* equates to buying an :class:`~rateslib.instruments.FXCall`
+    and an :class:`~rateslib.instruments.FXPut` at the same strike.
+
+    This class is essentially an alias constructor for an
+    :class:`~rateslib.instruments.FXOptionStrat` where the number
+    of options and their definitions and nominals have been specifically set.
+    """
+
+    rate_weight = [1.0, 1.0]
+    rate_weight_vol = [0.5, 0.5]
+    _rate_scalar = 100.0
+
+    def __init__(self, *args, premium=[NoInput(0), NoInput(0)], metric="vol", **kwargs):
+        super(FXOptionStrat, self).__init__(*args, premium=premium, **kwargs)
+        self.kwargs["metric"] = metric
+        self.periods = [
+            FXPut(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][0],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+            FXCall(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][1],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+        ]
+
+    def _validate_strike_and_premiums(self):
+        """called as part of init, specific validation rules for straddle"""
+        if self.kwargs["strike"] is NoInput.blank:
+            raise ValueError("`strike` for FXStraddle must be set to numeric or string value.")
+        if isinstance(self.kwargs["strike"], str) and self.kwargs["premium"] != [
+            NoInput.blank,
+            NoInput.blank,
+        ]:
+            raise ValueError(
+                "FXStraddle with string delta as `strike` cannot be initialised with a known `premium`.\n"
+                "Either set `strike` as a defined numeric value, or remove the `premium`."
+            )
+
+
+class FXStrangle(FXOptionStrat, FXOption):
+    """
+    Create an *FX Strangle* option strategy.
+
+    For additional arguments see :class:`~rateslib.instruments.FXOption`.
+
+    Parameters
+    ----------
+    args: tuple
+        Positional arguments to :class:`~rateslib.instruments.FXOption`.
+    strike: 2-element sequence
+        The first element is applied to the lower strike put and the
+        second element applied to the higher strike call, e.g. `["-25d", "25d"]`.
+    premium: 2-element sequence, optional
+        The premiums associated with each option of the strangle.
+    metric: str, optional
+        The default metric to apply in the method :meth:`~rateslib.instruments.FXOptionStrat.rate`
+    kwargs: tuple
+        Keyword arguments to :class:`~rateslib.instruments.FXOption`.
+
+    Notes
+    -----
+    When supplying ``strike`` as a string delta the strike will be determined at price time from
+    the provided volatility.
+
+    Buying a *Strangle* equates to buying a lower strike :class:`~rateslib.instruments.FXPut`
+    and buying a higher strike :class:`~rateslib.instruments.FXCall`.
+
+    This class is essentially an alias constructor for an
+    :class:`~rateslib.instruments.FXOptionStrat` where the number
+    of options and their definitions and nominals have been specifically set.
+
+    .. warning::
+
+       The default ``metric`` for an *FXStraddle* is *'single_vol'*, which requires an iterative algorithm to solve.
+       For defined strikes it is usually very accurate but for strikes defined by delta it
+       will return a solution within 0.1 pips. This means it is both slower than other instruments and inexact.
+
+    """
+
+    rate_weight = [1.0, 1.0]
+    rate_weight_vol = [0.5, 0.5]
+    _rate_scalar = 100.0
+
+    def __init__(
+        self,
+        *args,
+        strike=[NoInput(0), NoInput(0)],
+        premium=[NoInput(0), NoInput(0)],
+        metric="single_vol",
+        **kwargs,
+    ):
+        super(FXOptionStrat, self).__init__(*args, strike=strike, premium=premium, **kwargs)
+        self.kwargs["metric"] = metric
+        self._is_fixed_delta = [
+            isinstance(self.kwargs["strike"][0], str)
+            and self.kwargs["strike"][0][-1].lower() == "d"
+            and self.kwargs["strike"][0] != "atm_forward",
+            isinstance(self.kwargs["strike"][1], str)
+            and self.kwargs["strike"][1][-1].lower() == "d"
+            and self.kwargs["strike"][1] != "atm_forward",
+        ]
+        self.periods = [
+            FXPut(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"][0],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][0],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+            FXCall(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"][1],
+                notional=self.kwargs["notional"],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][1],
+                premium_ccy=self.kwargs["premium_ccy"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+        ]
+
+    def _validate_strike_and_premiums(self):
+        """called as part of init, specific validation rules for strangle"""
+        if any(_ is NoInput.blank for _ in self.kwargs["strike"]):
+            raise ValueError(
+                "`strike` for FXStrangle must be set to list of 2 numeric or string values."
+            )
+        for k, p in zip(self.kwargs["strike"], self.kwargs["premium"]):
+            if isinstance(k, str) and p != NoInput.blank:
+                raise ValueError(
+                    "FXStrangle with string delta as `strike` cannot be initialised with a known `premium`.\n"
+                    "Either set `strike` as a defined numeric value, or remove the `premium`."
+                )
+
+    def rate(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        vol: Union[list[float], float] = NoInput(0),
+        metric: Union[str, NoInput] = NoInput(0),  # "pips_or_%",
+    ):
+        """
+        Returns the rate of the *FXStraddle* according to a pricing metric.
+
+        Notes
+        ------
+
+        .. warning::
+
+           The default ``metric`` for an *FXStraddle* is *'single_vol'*, which requires an iterative algorithm to solve.
+           For defined strikes it is usually very accurate but for strikes defined by delta it
+           will return a solution within 0.01 pips. This means it is both slower than other instruments and inexact.
+
+        For parameters see :meth:`~rateslib.instruments.FXOption.rate`.
+
+        The ``metric`` *'vol'* is not sensible to use with an *FXStraddle*, although it will return the arithmetic
+        average volatility across both options, *'single_vol'* is the more standardised choice.
+        """
+        return self._rate(curves, solver, fx, base, vol, metric)
+
+    def _rate(self, curves, solver, fx, base, vol, metric, record_greeks=False):
+        metric = _drb(self.kwargs["metric"], metric).lower()
+        if metric != "single_vol" and not any(self._is_fixed_delta):
+            # the strikes are explicitly defined and independent across options.
+            # can evaluate separately
+            return super().rate(curves, solver, fx, base, vol, metric)
+        else:
+            # must perform single vol evaluation to determine mkt convention strikes
+            single_vol = self._rate_single_vol(curves, solver, fx, base, vol, record_greeks)
+            if metric == "single_vol":
+                return single_vol
+            else:
+                # return the premiums using the single_vol as the volatility
+                return super().rate(curves, solver, fx, base, vol=single_vol, metric=metric)
+
+    def _rate_single_vol(self, curves, solver, fx, base, vol, record_greeks):
+        """
+        Solve the single vol rate metric for a strangle using iterative market convergence routine.
+        """
+        # Get curves and vol
+        curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+            self.curves, solver, curves, fx, base, self.kwargs["pair"][3:]
+        )
+        vol = self._vol_as_list(vol, solver)
+
+        # first start by evaluating the individual swaptions given their strikes with the smile - delta or fixed
+        gks = [
+            self.periods[0].analytic_greeks(curves, solver, fx, base, vol=vol[0]),
+            self.periods[1].analytic_greeks(curves, solver, fx, base, vol=vol[1]),
+        ]
+
+        tgt_vol = (gks[0]["__vol"] * gks[0]["vega"] + gks[1]["__vol"] * gks[1]["vega"]) * 100.0
+        tgt_vol /= gks[0]["vega"] + gks[1]["vega"]
+        f0, iters = 100e6, 1
+        while abs(f0) > 1e-6 and iters < 10:
+            gks = [
+                self.periods[0].analytic_greeks(curves, solver, fx, base, vol=tgt_vol),
+                self.periods[1].analytic_greeks(curves, solver, fx, base, vol=tgt_vol),
+            ]
+            smile_gks = [  # note the strikes have been set at price time by previous call, call OptionPeriods direct
+                self.periods[0]
+                .periods[0]
+                .analytic_greeks(curves[1], curves[3], fx, base, vol=vol[0]),
+                self.periods[1]
+                .periods[0]
+                .analytic_greeks(curves[1], curves[3], fx, base, vol=vol[1]),
+            ]
+
+            # Apply ad hoc Newton 1d algorithm
+            f0 = (
+                smile_gks[0]["__bs76"]
+                + smile_gks[1]["__bs76"]
+                - gks[0]["__bs76"]
+                - gks[1]["__bs76"]
+            )
+
+            kega1 = gks[0]["_kega"] if self._is_fixed_delta[0] else 0.0
+            kega2 = gks[1]["_kega"] if self._is_fixed_delta[1] else 0.0
+            f1 = smile_gks[0]["_kappa"] * kega1 + smile_gks[1]["_kappa"] * kega2
+            f1 -= (
+                gks[0]["vega"]
+                + gks[1]["vega"]
+                + gks[0]["_kappa"] * kega1
+                + gks[1]["_kappa"] * kega2
+            )
+
+            tgt_vol = tgt_vol - (f0 / f1) * 100.0
+            iters += 1
+
+        if record_greeks:  # this needs to be explicitly called since it degrades performance
+            self._pricing["strangle_greeks"] = {
+                "single_vol": {
+                    "FXPut": self.periods[0].analytic_greeks(curves, solver, fx, base, vol=tgt_vol),
+                    "FXCall": self.periods[1].analytic_greeks(
+                        curves, solver, fx, base, vol=tgt_vol
+                    ),
+                },
+                "market_vol": {
+                    "FXPut": self.periods[0]
+                    .periods[0]
+                    .analytic_greeks(curves[1], curves[3], fx, base, vol=vol[0]),
+                    "FXCall": self.periods[1]
+                    .periods[0]
+                    .analytic_greeks(curves[1], curves[3], fx, base, vol=vol[1]),
+                },
+            }
+
+        return tgt_vol
+
+    # def _single_vol_rate_known_strikes(
+    #     self,
+    #     imm_prem,
+    #     f_d,
+    #     t_e,
+    #     v_deli,
+    #     g0,
+    # ):
+    #     k1 = self.kwargs["strike"][0]
+    #     k2 = self.kwargs["strike"][1]
+    #     sqrt_t = t_e ** 0.5
+    #
+    #     def root(g, imm_prem, k1, k2, f_d, sqrt_t, v_deli):
+    #         vol_sqrt_t = g * sqrt_t
+    #         d_plus_1 = _d_plus_min(k1, f_d, vol_sqrt_t, 0.5)
+    #         d_min_1 = _d_plus_min(k1, f_d, vol_sqrt_t, -0.5)
+    #         d_plus_2 = _d_plus_min(k2, f_d, vol_sqrt_t, 0.5)
+    #         d_min_2 = _d_plus_min(k2, f_d, vol_sqrt_t, -0.5)
+    #         f0 = -(f_d * dual_norm_cdf(-d_plus_1) - k1 * dual_norm_cdf(-d_min_1))
+    #         f0 += (f_d * dual_norm_cdf(d_plus_2) - k2 * dual_norm_cdf(d_min_2))
+    #         f0 = f0 * v_deli - imm_prem
+    #         f1 = v_deli * f_d * sqrt_t * (dual_norm_pdf(-d_plus_1) + dual_norm_pdf(d_plus_2))
+    #         return f0, f1
+    #
+    #     result = newton_1dim(root, g0=g0, args=(imm_prem, k1, k2, f_d, sqrt_t, v_deli))
+    #     return result["g"]
+
+
+class FXBrokerFly(FXOptionStrat, FXOption):
+    """
+    Create an *FX BrokerFly* option strategy.
+
+    For additional arguments see :class:`~rateslib.instruments.FXOption`.
+
+    Parameters
+    ----------
+    args: tuple
+        Positional arguments to :class:`~rateslib.instruments.FXOption`.
+    strike: 3-element sequence
+        The first element is applied to the lower strike put, the
+        second element to the straddle strike and the third element to the higher strike
+        call, e.g. `["-25d", "atm_delta", "25d"]`.
+    premium: 4-element sequence, optional
+        The premiums associated with each option of the strategy; lower strike put, straddle put,
+        straddle call, higher strike call.
+    metric: str, optional
+        The default metric to apply in the method :meth:`~rateslib.instruments.FXOptionStrat.rate`
+    kwargs: tuple
+        Keyword arguments to :class:`~rateslib.instruments.FXOption`.
+
+    Notes
+    -----
+    When supplying ``strike`` as a string delta the strike will be determined at price time from
+    the provided volatility.
+
+    Buying a *BrokerFly* equates to buying an :class:`~rateslib.instruments.FXStrangle` and
+    selling a :class:`~rateslib.instruments.FXStraddle`, where the convention is to set the
+    notional on the *Straddle* such that the entire strategy is *vega* neutral at inception.
+
+    .. warning::
+
+       The default ``metric`` for an *FXBrokerFly* is *'single_vol'*, which requires an iterative algorithm to solve.
+       For defined strikes it is usually very accurate but for strikes defined by delta it
+       will return a solution within 0.1 pips. This means it is both slower than other instruments and inexact.
+
+    """
+
+    rate_weight = [1.0, 1.0]
+    rate_weight_vol = [1.0, -1.0]
+    _rate_scalar = 100.0
+
+    def __init__(
+        self,
+        *args,
+        strike=[NoInput(0), NoInput(0), NoInput(0)],
+        premium=[NoInput(0), NoInput(0), NoInput(0), NoInput(0)],
+        notional=[NoInput(0), NoInput(0)],
+        metric="single_vol",
+        **kwargs,
+    ):
+        super(FXOptionStrat, self).__init__(
+            *args, premium=premium, strike=strike, notional=notional, **kwargs
+        )
+        self.kwargs["notional"][1] = (
+            NoInput(0) if self.kwargs["notional"][1] is None else self.kwargs["notional"][1]
+        )
+        self.kwargs["metric"] = metric
+        self.periods = [
+            FXStrangle(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=[self.kwargs["strike"][0], self.kwargs["strike"][2]],
+                notional=self.kwargs["notional"][0],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=[self.kwargs["premium"][0], self.kwargs["premium"][3]],
+                premium_ccy=self.kwargs["premium_ccy"],
+                metric=self.kwargs["metric"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+            FXStraddle(
+                pair=self.kwargs["pair"],
+                expiry=self.kwargs["expiry"],
+                delivery_lag=self.kwargs["delivery"],
+                payment_lag=self.kwargs["payment"],
+                calendar=self.kwargs["calendar"],
+                modifier=self.kwargs["modifier"],
+                strike=self.kwargs["strike"][1],
+                notional=self.kwargs["notional"][1],
+                option_fixing=self.kwargs["option_fixing"],
+                delta_type=self.kwargs["delta_type"],
+                premium=self.kwargs["premium"][1:3],
+                premium_ccy=self.kwargs["premium_ccy"],
+                metric="vol" if self.kwargs["metric"] == "single_vol" else self.kwargs["metric"],
+                curves=self.curves,
+                vol=self.vol,
+            ),
+        ]
+
+    def _maybe_set_vega_neutral_notional(self, curves, solver, fx, base, vol, metric):
+        if self.kwargs["notional"][1] is NoInput.blank and metric in ["pips_or_%", "premium"]:
+            self.periods[0]._rate(
+                curves, solver, fx, base, vol=vol[0], metric="single_vol", record_greeks=True
+            )
+            self._pricing["straddle_greeks"] = self.periods[1].analytic_greeks(
+                curves, solver, fx, base, vol=vol[1]
+            )
+            strangle_vega = self._pricing["strangle_greeks"]["market_vol"]["FXPut"]["vega"]
+            strangle_vega += self._pricing["strangle_greeks"]["market_vol"]["FXCall"]["vega"]
+            straddle_vega = self._pricing["straddle_greeks"]["vega"]
+            scalar = strangle_vega / straddle_vega
+            self.periods[1].kwargs["notional"] = float(
+                self.periods[0].periods[0].periods[0].notional * -scalar
+            )
+            self.periods[1]._set_notionals(self.periods[1].kwargs["notional"])
+            # BrokerFly -> Strangle -> FXPut -> FXPutPeriod
+
+    def rate(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        vol: Union[list[float], float] = NoInput(0),
+        metric: Union[str, NoInput] = NoInput(0),
+    ):
+        """
+        Return the mid-market rate of an option strategy.
+
+        Parameters
+        ----------
+        curves
+        solver
+        fx
+        base
+        vol
+        metric
+
+        Returns
+        -------
+        float, Dual, Dual2
+
+        Notes
+        -----
+
+        The different types of ``metric`` return different quotation conventions.
+
+        - *'single_vol'*: the default type for a :class:`~rateslib.instruments.FXStrangle`
+
+        - *'vol'*: sums the mid-market volatilities of each option multiplied by their respective ``rate_weight_vol``
+          parameter. For example this is the default pricing convention for
+          a :class:`~rateslib.instruments.FXRiskReversal` where the price is the vol of the call minus the vol of the
+          put and the ``rate_weight_vol`` parameters are [-1.0, 1.0].
+
+        - *'pips_or_%'*: sums the mid-market pips or percent price of each option multiplied by their respective
+          ``rate_weight`` parameter. For example for a :class:`~rateslib.instruments.FXStraddle` the total premium
+          is the sum of two premiums and the ``rate_weight`` parameters are [1.0, 1.0].
+        """
+        if not isinstance(vol, list):
+            vol = [[vol, vol], vol]
+        else:
+            vol = [
+                [vol[0], vol[2]],
+                vol[1],
+            ]  # restructure to pass to Strangle and Straddle separately
+
+        temp_metric = _drb(self.kwargs["metric"], metric)
+        self._maybe_set_vega_neutral_notional(curves, solver, fx, base, vol, temp_metric.lower())
+
+        if temp_metric == "pips_or_%":
+            straddle_scalar = (
+                self.periods[1].periods[0].periods[0].notional
+                / self.periods[0].periods[0].periods[0].notional
+            )
+            weights = [1.0, straddle_scalar]
+        elif temp_metric == "premium":
+            weights = self.rate_weight
+        else:
+            weights = self.rate_weight_vol
+        _ = 0.0
+        for option_strat, vol_, weight in zip(self.periods, vol, weights):
+            _ += option_strat.rate(curves, solver, fx, base, vol_, metric) * weight
+        return _
+
+    def analytic_greeks(
+        self,
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: float = NoInput(0),
+    ):
+        """ """
+        # implicitly call set_pricing_mid for unpriced parameters
+        self.rate(curves, solver, fx, base, vol, metric="pips_or_%")
+        # curves, fx, base = _get_curves_fx_and_base_maybe_from_solver(
+        #     self.curves, solver, curves, fx, base, self.kwargs["pair"][3:]
+        # )
+        if not isinstance(vol, list):
+            vol = [[vol, vol], vol]
+        else:
+            vol = [[vol[0], vol[2]], vol[1]]  # restructure for strangle / straddle
+
+        # TODO: this method can be optimised because it calculates greeks at multiple times within frames
+        g_grks = self.periods[0].analytic_greeks(curves, solver, fx, base, local, vol[0])
+        d_grks = self.periods[1].analytic_greeks(curves, solver, fx, base, local, vol[1])
+        sclr = abs(
+            self.periods[1].periods[0].periods[0].notional
+            / self.periods[0].periods[0].periods[0].notional
+        )
+
+        _unit_attrs = ["delta", "gamma", "vega", "vomma", "vanna", "_kega", "_kappa", "__bs76"]
+        _ = {}
+        for attr in _unit_attrs:
+            _[attr] = g_grks[attr] - sclr * d_grks[attr]
+
+        _notional_attrs = [
+            f"delta_{self.kwargs['pair'][:3]}",
+            f"gamma_{self.kwargs['pair'][:3]}_1%",
+            f"vega_{self.kwargs['pair'][3:]}",
+        ]
+        for attr in _notional_attrs:
+            _[attr] = g_grks[attr] - d_grks[attr]
+
+        _.update(
+            {
+                "__class": "FXOptionStrat",
+                "__strategies": {"FXStrangle": g_grks, "FXStraddle": d_grks},
+                "__delta_type": g_grks["__delta_type"],
+                "__notional": self.kwargs["notional"],
+            }
+        )
+        return _
+
+    def _plot_payoff(
+        self,
+        range: Union[list[float], NoInput] = NoInput(0),
+        curves: Union[Curve, str, list, NoInput] = NoInput(0),
+        solver: Union[Solver, NoInput] = NoInput(0),
+        fx: Union[FXForwards, NoInput] = NoInput(0),
+        base: Union[str, NoInput] = NoInput(0),
+        local: bool = False,
+        vol: Union[list[float], float] = NoInput(0),
+    ):
+        vol = self._vol_as_list(vol, solver)
+        self._maybe_set_vega_neutral_notional(curves, solver, fx, base, vol, metric="pips_or_%")
+        return super()._plot_payoff(range, curves, solver, fx, base, local, vol)
+
+
 # Generic Instruments
 
 
 class Spread(Sensitivities):
     """
     A spread instrument defined as the difference in rate between two *Instruments*.
 
@@ -8055,18 +9666,14 @@
         Calculate the gamma of the *Instrument*.
 
         For arguments see :meth:`Sensitivities.gamma()<rateslib.instruments.Sensitivities.gamma>`.
         """
         return super().gamma(*args, **kwargs)
 
 
-# class SpreadX:
-#     pass
-
-
 class Fly(Sensitivities):
     """
     A butterfly instrument which is, mechanically, the spread of two spread instruments.
 
     Parameters
     ----------
     instrument1 : Instrument
@@ -8168,46 +9775,14 @@
         Calculate the gamma of the *Instrument*.
 
         For arguments see :meth:`Sensitivities.gamma()<rateslib.instruments.Sensitivities.gamma>`.
         """
         return super().gamma(*args, **kwargs)
 
 
-# class FlyX:
-#     """
-#     A butterly instrument which is the spread of two spread instruments
-#     """
-#     def __init__(self, instrument1, instrument2, instrument3):
-#         self.instrument1 = instrument1
-#         self.instrument2 = instrument2
-#         self.instrument3 = instrument3
-#
-#     def npv(self, *args, **kwargs):
-#         if len(args) == 0:
-#             args1 = (kwargs.get("curve1", None), kwargs.get("disc_curve1", None))
-#             args2 = (kwargs.get("curve2", None), kwargs.get("disc_curve2", None))
-#             args3 = (kwargs.get("curve3", None), kwargs.get("disc_curve3", None))
-#         else:
-#             args1 = args
-#             args2 = args
-#             args3 = args
-#         return self.instrument1.npv(*args1) + self.instrument2.npv(*args2) + self.instrument3.npv(*args3)
-#
-#     def rate(self, *args, **kwargs):
-#         if len(args) == 0:
-#             args1 = (kwargs.get("curve1", None), kwargs.get("disc_curve1", None))
-#             args2 = (kwargs.get("curve2", None), kwargs.get("disc_curve2", None))
-#             args3 = (kwargs.get("curve3", None), kwargs.get("disc_curve3", None))
-#         else:
-#             args1 = args
-#             args2 = args
-#             args3 = args
-#         return 2 * self.instrument2.rate(*args2) - self.instrument1.rate(*args1) - self.instrument3.rate(*args3)
-
-
 def _instrument_npv(instrument, *args, **kwargs):  # pragma: no cover
     # this function is captured by TestPortfolio pooling but is not registered as a parallel process
     # used for parallel processing with Portfolio.npv
     return instrument.npv(*args, **kwargs)
 
 
 class Portfolio(Sensitivities):
@@ -8428,102 +10003,14 @@
     else:  # y2 < y:
         # line not hit due to reassessment of initial vars?
         return _ytm_quadratic_converger2(
             f, y2 - pad, y, 2 * y - y2 + pad, None, f_, None, tol
         )  # pragma: no cover
 
 
-# def _brents(f, x0, x1, max_iter=50, tolerance=1e-9):  # pragma: no cover
-#     """
-#     Alternative yield converger as an alternative to ytm_converger
-#
-#     Unused currently within the library
-#     """
-#     fx0 = f(x0)
-#     fx1 = f(x1)
-#
-#     if float(fx0 * fx1) > 0:
-#         raise ValueError(
-#             "`brents` must initiate from function values with opposite signs."
-#         )
-#
-#     if abs(fx0) < abs(fx1):
-#         x0, x1 = x1, x0
-#         fx0, fx1 = fx1, fx0
-#
-#     x2, fx2 = x0, fx0
-#
-#     mflag = True
-#     steps_taken = 0
-#
-#     while steps_taken < max_iter and abs(x1 - x0) > tolerance:
-#         fx0 = f(x0)
-#         fx1 = f(x1)
-#         fx2 = f(x2)
-#
-#         if fx0 != fx2 and fx1 != fx2:
-#             L0 = (x0 * fx1 * fx2) / ((fx0 - fx1) * (fx0 - fx2))
-#             L1 = (x1 * fx0 * fx2) / ((fx1 - fx0) * (fx1 - fx2))
-#             L2 = (x2 * fx1 * fx0) / ((fx2 - fx0) * (fx2 - fx1))
-#             new = L0 + L1 + L2
-#
-#         else:
-#             new = x1 - ((fx1 * (x1 - x0)) / (fx1 - fx0))
-#
-#         if (
-#             (float(new) < float((3 * x0 + x1) / 4) or float(new) > float(x1))
-#             or (mflag is True and (abs(new - x1)) >= (abs(x1 - x2) / 2))
-#             or (mflag is False and (abs(new - x1)) >= (abs(x2 - d) / 2))
-#             or (mflag is True and (abs(x1 - x2)) < tolerance)
-#             or (mflag is False and (abs(x2 - d)) < tolerance)
-#         ):
-#             new = (x0 + x1) / 2
-#             mflag = True
-#
-#         else:
-#             mflag = False
-#
-#         fnew = f(new)
-#         d, x2 = x2, x1
-#
-#         if float(fx0 * fnew) < 0:
-#             x1 = new
-#         else:
-#             x0 = new
-#
-#         if abs(fx0) < abs(fx1):
-#             x0, x1 = x1, x0
-#
-#         steps_taken += 1
-#
-#     return x1, steps_taken
-
-
-def _quadratic_equation(a: float, b: float, c: float):
-    """
-    solver the equation ax^2 + bx + c = 0, via the quadratic formula.
-    """
-    # perform the quadratic solution
-    _1 = -c / b  # approximate linear solution: applicable for most situations.
-    discriminant = b**2 - 4 * a * c
-    if abs(a) > 1e-14:
-        _2a = (-b - discriminant**0.5) / (2 * a)
-        _2b = (-b + discriminant**0.5) / (2 * a)  # alt quadratic soln
-        if abs(_1 - _2a) < abs(_1 - _2b):
-            _ = _2a
-        else:
-            _ = _2b  # select quadratic soln
-    else:
-        # this is to avoid divide by zero errors and return an approximation
-        # also isda_flat_compounding has a=0
-        _ = _1
-
-    return _
-
-
 def _get(kwargs: dict, leg: int = 1, filter=[]):
     """
     A parser to return kwarg dicts for relevant legs.
     Internal structuring only.
     Will return kwargs relevant to leg1 OR leg2.
     Does not return keys that are specified in the filter.
     """
@@ -8608,7 +10095,10 @@
     return val
 
 
 def _upper(val: Union[str, NoInput]):
     if isinstance(val, str):
         return val.upper()
     return val
+
+
+
```

### Comparing `rateslib-1.1.1/rateslib/legs.py` & `rateslib-1.2.0/rateslib/legs.py`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/rateslib/periods.py` & `rateslib-1.2.0/rateslib/solver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,2392 +1,2335 @@
-# This module is a dependent of legs.py
-
-"""
-.. ipython:: python
-   :suppress:
-
-   from rateslib.periods import *
-   from rateslib.curves import Curve
-   from datetime import datetime as dt
-   curve = Curve(
-       nodes={
-           dt(2022,1,1): 1.0,
-           dt(2023,1,1): 0.99,
-           dt(2024,1,1): 0.965,
-           dt(2025,1,1): 0.93,
-       },
-       interpolation="log_linear",
-   )
-"""
-
-from abc import abstractmethod, ABCMeta
-from datetime import datetime
-from typing import Optional, Union
-import warnings
-from math import comb, log
+from __future__ import annotations
 
+from typing import Optional, Union, Callable
+from itertools import combinations
+from uuid import uuid4
+from time import time
 import numpy as np
-
-# from pandas.tseries.offsets import CustomBusinessDay
-from pandas import DataFrame, date_range, Series, NA, isna, notna
+import warnings
+from pandas import DataFrame, MultiIndex, concat, Series
 
 from rateslib import defaults
 from rateslib.default import NoInput
-from rateslib.calendars import add_tenor, dcf, _get_eom, _is_holiday, CalInput
-from rateslib.curves import (
-    Curve,
-    LineCurve,
-    IndexCurve,
-    average_rate,
-    CompositeCurve,
-    index_left,
-)
-from rateslib.dual import Dual, Dual2, DualTypes, gradient
-from rateslib.fx import FXForwards, FXRates
+from rateslib.dual import Dual, Dual2, dual_log, dual_solve, gradient
+from rateslib.curves import CompositeCurve, ProxyCurve, MultiCsaCurve
+from rateslib.fx import FXRates, FXForwards
 
 
 # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
 # Commercial use of this code, and/or copying and redistribution is prohibited.
 # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
 
-def _get_fx_and_base(
-    currency: str,
-    fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-    base: Union[str, NoInput] = NoInput(0),
-):
-    if fx is None:
-        raise NotImplementedError("TraceBack for NoInput")
-    if base is None:
-        raise NotImplementedError("TraceBack for NoInput")
-
-    if isinstance(fx, (FXRates, FXForwards)):
-        base = fx.base if base is NoInput.blank else base.lower()
-        if base == currency:
-            fx = 1.0
-        else:
-            fx = fx.rate(pair=f"{currency}{base}")
-    elif base is not NoInput.blank:  # and fx is then a float or None
-        if fx is NoInput.blank:
-            if base.lower() != currency.lower():
-                raise ValueError(
-                    f"`base` ({base}) cannot be requested without supplying `fx` as a "
-                    "valid FXRates or FXForwards object to convert to "
-                    f"currency ({currency}).\n"
-                    "If you are using a `Solver` with multi-currency instruments have you "
-                    "forgotten to attach the FXForwards in the solver's `fx` argument?"
-                )
-            fx = 1.0
-        else:
-            if abs(fx - 1.0) < 1e-10:
-                pass  # no warning when fx == 1.0
-            else:
-                warnings.warn(
-                    f"`base` ({base}) should not be given when supplying `fx` as numeric "
-                    f"since it will not be used.\nIt may also be interpreted as giving "
-                    f"wrong results.\nBest practice is to instead supply `fx` as an "
-                    f"FXRates (or FXForwards) object.\n"
-                    f"Reformulate: [fx={fx}, base='{base}'] -> "
-                    f"[fx=FXRates({{'{currency}{base}': {fx}}}), base='{base}'].",
-                    UserWarning,
-                )
-            fx = fx
-    else:  # base is None and fx is float or None.
-        if fx is NoInput.blank:
-            fx = 1.0
-        else:
-            if abs(fx - 1.0) < 1e-10:
-                pass  # no warning when fx == 1.0
-            else:
-                warnings.warn(
-                    "It is not best practice to provide `fx` as numeric since this can "
-                    "cause errors of output when dealing with multi-currency derivatives,\n"
-                    "and it also fails to preserve FX rate sensitivity in calculations.\n"
-                    "Instead, supply a 'base' currency and use an "
-                    "FXRates or FXForwards object.\n"
-                    f"Reformulate: [fx={fx}, base=None] -> "
-                    f"[fx=FXRates({{'{currency}bas': {fx}}}), base='bas'].",
-                    UserWarning,
-                )
-            fx = fx
-
-    return fx, base
-
-
-class BasePeriod(metaclass=ABCMeta):
+class Gradients:
+    """
+    A catalogue of all the gradients used in optimisation routines and risk
+    sensitivties.
     """
-    Abstract base class with common parameters for all ``Period`` subclasses.
 
-    See also: :ref:`User guide for Periods <periods-doc>`.
+    @property
+    def J(self):
+        """
+        2d Jacobian array of calibrating instrument rates with respect to curve
+        variables, of size (n, m);
 
-    Parameters
-    ----------
-    start : Datetime
-        The adjusted start date of the calculation period.
-    end: Datetime
-        The adjusted end date of the calculation period.
-    payment : Datetime
-        The adjusted payment date of the period.
-    frequency : str
-        The frequency of the corresponding leg. Also used
-        with specific values for ``convention``, or floating rate calculation.
-    notional : float, optional, set by Default
-        The notional amount of the period (positive implies paying a cashflow).
-    currency : str, optional
-        The currency of the cashflow (3-digit code), set by default.
-    convention : str, optional, set by Default
-        The day count convention of the calculation period accrual.
-        See :meth:`~rateslib.scheduling.dcf`.
-    termination : Datetime, optional
-        The termination date of the corresponding leg. Required only with
-        specific values for ``convention``.
-    stub : bool, optional
-        Records whether the period is a stub or regular. Used by certain day count
-        convention calculations.
-    roll : int, str, optional
-        Used only by ``stub`` periods and for specific values of ``convention``.
-    calendar : CustomBusinessDay, str, optional
-        Used only by ``stub`` periods and for specific values of ``convention``.
+        .. math::
 
-    """
+           [J]_{i,j} = [\\nabla_\\mathbf{v} \\mathbf{r^T}]_{i,j} = \\frac{\\partial r_j}{\\partial v_i}
 
-    @abstractmethod
-    def __init__(
-        self,
-        start: datetime,
-        end: datetime,
-        payment: datetime,
-        frequency: str,
-        notional: Union[float, NoInput] = NoInput(0),
-        currency: Union[str, NoInput] = NoInput(0),
-        convention: Union[str, NoInput] = NoInput(0),
-        termination: Union[datetime, NoInput] = NoInput(0),
-        stub: bool = False,
-        roll: Union[int, str, NoInput] = NoInput(0),
-        calendar: CalInput = NoInput(0),
-    ):
-        if end < start:
-            raise ValueError("`end` cannot be before `start`.")
-        self.start, self.end, self.payment = start, end, payment
-        self.frequency = frequency.upper()
-        self.notional = defaults.notional if notional is NoInput.blank else notional
-        self.currency = defaults.base_currency if currency is NoInput.blank else currency.lower()
-        self.convention = defaults.convention if convention is NoInput.blank else convention
-        self.termination = termination
-        self.freq_months = defaults.frequency_months[self.frequency]
-        self.stub = stub
-        self.roll = roll
-        self.calendar = calendar
-
-    def __repr__(self):
-        return (
-            f"<{type(self).__name__}: {self.start.strftime('%Y-%m-%d')}->"
-            f"{self.end.strftime('%Y-%m-%d')},{self.notional},{self.convention}>"
-        )
+        Depends on ``self.r``.
+        """
+        if self._J is None:
+            self._J = np.array([gradient(rate, self.variables) for rate in self.r]).T
+        return self._J
 
     @property
-    def dcf(self):
+    def grad_v_rT(self):
         """
-        float : Calculated with appropriate ``convention`` over the period.
+        Alias of ``J``.
         """
-        return dcf(
-            self.start,
-            self.end,
-            self.convention,
-            self.termination,
-            self.freq_months,
-            self.stub,
-            self.roll,
-            self.calendar,
-        )
+        return self.J
 
-    @abstractmethod
-    def analytic_delta(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ) -> DualTypes:
+    @property
+    def J2(self):
         """
-        Return the analytic delta of the period object.
-
-        Parameters
-        ----------
-        curve : Curve
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``, or if a rate in a :class:`FloatPeriod` is required.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object.
+        3d array of second derivatives of calibrating instrument rates with
+        respect to curve variables, of size (n, n, m);
 
-        Returns
-        -------
-        float, Dual, Dual2
-
-        Examples
-        --------
-        .. ipython:: python
+        .. math::
 
-           curve = Curve({dt(2021,1,1): 1.00, dt(2025,1,1): 0.83}, interpolation="log_linear", id="SONIA")
-           fxr = FXRates({"gbpusd": 1.25}, base="usd")
+           [J2]_{i,j,k} = [\\nabla_\\mathbf{v} \\nabla_\\mathbf{v} \\mathbf{r^T}]_{i,j,k} = \\frac{\\partial^2 r_k}{\\partial v_i \\partial v_j}
 
-        .. ipython:: python
+        Depends on ``self.r``.
+        """
+        if self._J2 is None:
+            if self._ad != 2:
+                raise ValueError(
+                    "Cannot perform second derivative calculations when ad mode is " f"{self._ad}."
+                )
 
-           period = FixedPeriod(
-               start=dt(2022, 1, 1),
-               end=dt(2022, 7, 1),
-               payment=dt(2022, 7, 1),
-               frequency="S",
-               currency="gbp",
-               fixed_rate=4.00,
-           )
-           period.analytic_delta(curve, curve)
-           period.analytic_delta(curve, curve, fxr)
-           period.analytic_delta(curve, curve, fxr, "gbp")
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        fx, base = _get_fx_and_base(self.currency, fx, base)
-        _ = fx * self.notional * self.dcf * disc_curve_[self.payment] / 10000
-        return _
+            rates = np.array([_[0].rate(*_[1], **_[2]) for _ in self.instruments])
+            # solver is passed in order to extract curves as string
+            _ = np.array([gradient(rate, self.variables, order=2) for rate in rates])
+            self._J2 = np.transpose(_, (1, 2, 0))
+        return self._J2
 
-    @abstractmethod
-    def cashflows(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ) -> dict:
+    @property
+    def grad_v_v_rT(self):
         """
-        Return the properties of the period used in calculating cashflows.
+        Alias of ``J2``.
+        """
+        return self.J2  # pragma: no cover
 
-        Parameters
-        ----------
-        curve : Curve, optional
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``, or if a rate in a :class:`FloatPeriod` is required.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code).
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object. If not given defaults to
-            ``fx.base``.
+    @property
+    def grad_s_vT(self):
+        """
+        2d Jacobian array of curve variables with respect to calibrating instruments,
+        of size (m, n);
 
-        Returns
-        -------
-        dict
+        .. math::
 
-        Examples
-        --------
-        .. ipython:: python
+           [\\nabla_\\mathbf{s}\\mathbf{v^T}]_{i,j} = \\frac{\\partial v_j}{\\partial s_i} = \\mathbf{J^+}
+        """
+        if self._grad_s_vT is None:
+            self._grad_s_vT = getattr(self, self._grad_s_vT_method)()
+        return self._grad_s_vT
+
+    def _grad_s_vT_final_iteration_dual(self, algorithm: Optional[str] = None):
+        """
+        This is not the ideal method since it requires reset_properties to reassess.
+        """
+        algorithm = algorithm or self._grad_s_vT_final_iteration_algo
+        _s = self.s
+        self.s = np.array([Dual(v, [f"s{i}"], []) for i, v in enumerate(self.s)])
+        self._reset_properties_()
+        v_1 = self._update_step_(algorithm)
+        s_vars = [f"s{i}" for i in range(self.m)]
+        grad_s_vT = np.array([gradient(v, s_vars) for v in v_1]).T
+        self.s = _s
+        return grad_s_vT
+
+    def _grad_s_vT_final_iteration_analytical(self):
+        """Uses a pseudoinverse algorithm on floats"""
+        grad_s_vT = np.linalg.pinv(self.J)
+        return grad_s_vT
+
+    def _grad_s_vT_fixed_point_iteration(self):
+        """
+        This is not the ideal method because it requires second order and reset props.
+        """
+        self._set_ad_order(2)
+        self._reset_properties_()
+        _s = self.s
+        self.s = np.array([Dual2(v, [f"s{i}"], [], []) for i, v in enumerate(self.s)])
+        s_vars = tuple(f"s{i}" for i in range(self.m))
+        grad2 = gradient(self.g, self.variables + s_vars, order=2)
+        grad_v_vT_f = grad2[: self.n, : self.n]
+        grad_s_vT_f = grad2[self.n :, : self.n]
+        grad_s_vT = np.linalg.solve(grad_v_vT_f, -grad_s_vT_f.T).T
+
+        # The following are alternative representations. Actually faster to calculate and
+        # do not require sensitivity against S variables to be measured.
+        # See 'coding interest rates' equation 12.38
+        # _1 = np.einsum("iy, yz, jz", self.J, self.W, self.J)
+        # _2 = np.einsum("z, zy, ijy", self.x.astype(float), self.W, self.J2)
+        # _3 = 2* (_1 + _2)
+        # _11 = -2 * np.einsum("iz,zj->ji", self.J, self.W)
+
+        self.s = _s
+        self._set_ad_order(1)
+        self._reset_properties_()
+        return grad_s_vT
 
-           period.cashflows(curve, curve, fxr)
+    @property
+    def grad_s_s_vT(self):
         """
-        disc_curve: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        if disc_curve is NoInput.blank:
-            df, collateral = None, None
-        else:
-            df, collateral = float(disc_curve[self.payment]), disc_curve.collateral
+        3d array of second derivatives of curve variables with respect to
+        calibrating instruments, of size (m, m, n);
 
-        return {
-            defaults.headers["type"]: type(self).__name__,
-            defaults.headers["stub_type"]: "Stub" if self.stub else "Regular",
-            defaults.headers["currency"]: self.currency.upper(),
-            defaults.headers["a_acc_start"]: self.start,
-            defaults.headers["a_acc_end"]: self.end,
-            defaults.headers["payment"]: self.payment,
-            defaults.headers["convention"]: self.convention,
-            defaults.headers["dcf"]: self.dcf,
-            defaults.headers["notional"]: float(self.notional),
-            defaults.headers["df"]: df,
-            defaults.headers["collateral"]: collateral,
-        }
+        .. math::
 
-    @abstractmethod
-    def npv(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-        local: bool = False,
-    ) -> Union[DualTypes, dict[str, DualTypes]]:
+           [\\nabla_\\mathbf{s} \\nabla_\\mathbf{s} \\mathbf{v^T}]_{i,j,k} = \\frac{\\partial^2 v_k}{\\partial s_i \\partial s_j}
         """
-        Return the NPV of the period object.
+        if self._grad_s_s_vT is None:
+            self._grad_s_s_vT = self._grad_s_s_vT_final_iteration_analytical()
+        return self._grad_s_s_vT
 
-        Calculates the cashflow for the period and multiplies it by the DF associated
-        with the payment date.
+    def _grad_s_s_vT_fwd_difference_method(self):
+        """Use a numerical method, iterating through changes in s to calculate."""
+        ds = 10 ** (int(dual_log(self.func_tol, 10) / 2))
+        grad_s_vT_0 = np.copy(self.grad_s_vT)
+        grad_s_s_vT = np.zeros(shape=(self.m, self.m, self.n))
 
-        Parameters
-        ----------
-        curve : Curve, optional
-            The forecasting curve object. Not used unless it is set equal to
-            ``disc_curve``, or if a rate in a :class:`FloatPeriod` is required.
-        disc_curve : Curve, optional
-            The discounting curve object used in calculations.
-            Set equal to ``curve`` if not given.
-        fx : float, FXRates, FXForwards, optional
-            The immediate settlement FX rate that will be used to convert values
-            into another currency. A given `float` is used directly. If giving a
-            :class:`~rateslib.fx.FXRates` or :class:`~rateslib.fx.FXForwards`
-            object, converts from local currency into ``base``.
-        base : str, optional
-            The base currency to convert cashflows into (3-digit code), set by default.
-            Only used if ``fx`` is an :class:`~rateslib.fx.FXRates` or
-            :class:`~rateslib.fx.FXForwards` object.
-        local : bool, optional
-            If `True` will ignore the ``base`` request and return a dict identifying
-            local currency NPV.
+        for i in range(self.m):
+            self.s[i] += ds
+            self.iterate()
+            grad_s_s_vT[:, i, :] = (self.grad_s_vT - grad_s_vT_0) / ds
+            self.s[i] -= ds
 
-        Returns
-        -------
-        float, Dual, Dual2, or dict of such
+        # ensure exact symmetry (maybe redundant)
+        grad_s_s_vT = (grad_s_s_vT + np.swapaxes(grad_s_s_vT, 0, 1)) / 2
+        self.iterate()
+        # self._grad_s_vT_fixed_point_iteration()  # TODO: returns nothing: what is purpose
+        return grad_s_s_vT
 
-        Examples
-        --------
-        .. ipython:: python
+    def _grad_s_s_vT_final_iteration_analytical(self, use_pre=False):
+        """
+        Use an analytical formula and second order AD to calculate.
 
-           period.npv(curve, curve)
-           period.npv(curve, curve, fxr)
-           period.npv(curve, curve, fxr, "gbp")
-           period.npv(curve, curve, fxr, local=True)
+        Not: must have 2nd order AD set to function, and valid properties set to
+        function
         """
-        pass  # pragma: no cover
+        if use_pre:
+            J2, grad_s_vT = self.J2_pre, self.grad_s_vT_pre
+        else:
+            J2, grad_s_vT = self.J2, self.grad_s_vT
 
+        _ = np.tensordot(J2, grad_s_vT, (2, 0))  # dv/dr_l * d2r_l / dvdv
+        _ = np.tensordot(grad_s_vT, _, (1, 0))  # dv_z /ds * d2v / dv_zdv
+        _ = -np.tensordot(grad_s_vT, _, (1, 1))  # dv_h /ds * d2v /dvdv_h
+        grad_s_s_vT = _
+        return grad_s_s_vT
+        # _ = np.matmul(grad_s_vT, np.matmul(J2, grad_s_vT))
+        # grad_s_s_vT = -np.tensordot(grad_s_vT, _, (1, 0))
+        # return grad_s_s_vT
 
-class FixedPeriod(BasePeriod):
-    """
-    Create a period defined with a fixed rate.
+    # _pre versions incorporate all variables of solver and pre_solvers
 
-    Parameters
-    ----------
-    args : dict
-        Required positional args to :class:`BasePeriod`.
-    fixed_rate : float or None, optional
-        The rate applied to determine the cashflow. If `None`, can be set later,
-        typically after a mid-market rate for all periods has been calculated.
-    kwargs : dict
-        Required keyword arguments to :class:`BasePeriod`.
+    def grad_f_rT_pre(self, fx_vars):
+        """
+        2d Jacobian array of calibrating instrument rates with respect to FX rate
+        variables, of size (len(fx_vars), pre_m);
 
-    Notes
-    -----
-    The ``cashflow`` is defined as follows;
+        .. math::
 
-    .. math::
+           [\\nabla_\\mathbf{f}\\mathbf{r^T}]_{i,j} = \\frac{\\partial r_j}{\\partial f_i}
 
-       C = -NdR
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities.
+        """
+        grad_f_rT = np.array([gradient(rate, fx_vars) for rate in self.r_pre]).T
+        return grad_f_rT
 
-    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+    @property
+    def J2_pre(self):
+        """
+        3d array of second derivatives of calibrating instrument rates with
+        respect to curve variables for all ``Solvers`` including ``pre_solvers``,
+        of size (pre_n, pre_n, pre_m);
 
-    .. math::
+        .. math::
 
-       P = Cv = -NdRv(m)
+           [J2]_{i,j,k} = [\\nabla_\\mathbf{v} \\nabla_\\mathbf{v} \\mathbf{r^T}]_{i,j,k} = \\frac{\\partial^2 r_k}{\\partial v_i \\partial v_j}
 
-    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+        Depends on ``self.r`` and ``pre_solvers.J2``.
+        """
+        if len(self.pre_solvers) == 0:
+            return self.J2
 
-    .. math::
+        if self._J2_pre is None:
+            if self._ad != 2:
+                raise ValueError(
+                    "Cannot perform second derivative calculations when ad mode is " f"{self._ad}."
+                )
 
-       A = - \\frac{\\partial P}{\\partial R} = Ndv(m)
+            J2 = np.zeros(shape=(self.pre_n, self.pre_n, self.pre_m))
+            i, j = 0, 0
+            for pre_slvr in self.pre_solvers:
+                J2[
+                    i : i + pre_slvr.pre_n,
+                    i : i + pre_slvr.pre_n,
+                    j : j + pre_slvr.pre_m,
+                ] = pre_slvr.J2_pre
+                i, j = i + pre_slvr.pre_n, j + pre_slvr.pre_m
+
+            rates = np.array([_[0].rate(*_[1], **_[2]) for _ in self.instruments])
+            # solver is passed in order to extract curves as string
+            _ = np.array([gradient(r, self.pre_variables, order=2) for r in rates])
+            J2[:, :, -self.m :] = np.transpose(_, (1, 2, 0))
+            self._J2_pre = J2
+        return self._J2_pre
 
-    Examples
-    --------
-    .. ipython:: python
+    def grad_f_v_rT_pre(self, fx_vars):
+        """
+        3d array of second derivatives of calibrating instrument rates with respect to
+        FX rates and curve variables, of size (len(fx_vars), pre_n, pre_m);
+
+        .. math::
 
-       fp = FixedPeriod(
-           start=dt(2022, 2, 1),
-           end=dt(2022, 8, 1),
-           payment=dt(2022, 8, 2),
-           frequency="S",
-           notional=1e6,
-           currency="eur",
-           convention="30e360",
-           fixed_rate=5.0,
-       )
-       fp.cashflows(curve=Curve({dt(2022, 1, 1):1.0, dt(2022, 12, 31): 0.98}))
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{v} \\mathbf{r^T}]_{i,j,k} = \\frac{\\partial^2 r_k}{\\partial f_i \\partial v_j}
 
-    """
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities.
+        """
+        # FX sensitivity requires reverting through all pre-solvers rates.
+        all_gradients = np.array(
+            [gradient(rate, self.pre_variables + tuple(fx_vars), order=2) for rate in self.r_pre]
+        ).swapaxes(0, 2)
 
-    def __init__(self, *args, fixed_rate: Union[float, NoInput] = NoInput(0), **kwargs):
-        self.fixed_rate = fixed_rate
-        super().__init__(*args, **kwargs)
+        grad_f_v_rT = all_gradients[self.pre_n :, : self.pre_n, :]
+        return grad_f_v_rT
 
-    def analytic_delta(self, *args, **kwargs) -> DualTypes:
+    def grad_f_f_rT_pre(self, fx_vars):
         """
-        Return the analytic delta of the *FixedPeriod*.
-        See
-        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
+        3d array of second derivatives of calibrating instrument rates with respect to
+        FX rates, of size (len(fx_vars), len(fx_vars), pre_m);
+
+        .. math::
+
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{f} \\mathbf{r^T}]_{i,j,k} = \\frac{\\partial^2 r_k}{\\partial f_i \\partial f_j}
+
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities.
         """
-        return super().analytic_delta(*args, **kwargs)
+        # FX sensitivity requires reverting through all pre-solvers rates.
+        grad_f_f_rT = np.array([gradient(rate, fx_vars, order=2) for rate in self.r_pre]).swapaxes(
+            0, 2
+        )
+        return grad_f_f_rT
 
     @property
-    def cashflow(self) -> Union[float, None]:
+    def grad_s_s_vT_pre(self):
         """
-        float, Dual or Dual2 : The calculated value from rate, dcf and notional.
-        """
-        if self.fixed_rate is NoInput.blank:
-            return None
-        else:
-            return -self.notional * self.dcf * self.fixed_rate / 100
+        3d array of second derivatives of curve variables with respect to
+        calibrating instruments, of size (pre_m, pre_m, pre_n);
 
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-    # Commercial use of this code, and/or copying and redistribution is prohibited.
-    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+        .. math::
 
-    def npv(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-        local: bool = False,
-    ) -> DualTypes:
-        """
-        Return the NPV of the *FixedPeriod*.
-        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
-        """
-        disc_curve_: Curve = _disc_from_curve(curve, disc_curve)
-        if not isinstance(disc_curve, Curve) and curve is NoInput.blank:
-            raise TypeError("`curves` have not been supplied correctly.")
-        value = self.cashflow * disc_curve_[self.payment]
-        if local:
-            return {self.currency: value}
-        else:
-            fx, _ = _get_fx_and_base(self.currency, fx, base)
-            return fx * value
+           [\\nabla_\\mathbf{s} \\nabla_\\mathbf{s} \\mathbf{v^T}]_{i,j,k} = \\frac{\\partial^2 v_k}{\\partial s_i \\partial s_j}
+        """
+        if len(self.pre_solvers) == 0:
+            return self.grad_s_s_vT
 
-    def cashflows(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ) -> dict:
-        """
-        Return the cashflows of the *FixedPeriod*.
-        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        fx, base = _get_fx_and_base(self.currency, fx, base)
-
-        if disc_curve_ is NoInput.blank or self.fixed_rate is NoInput.blank:
-            npv = None
-            npv_fx = None
-        else:
-            npv = float(self.npv(curve, disc_curve_))
-            npv_fx = npv * float(fx)
+        if self._grad_s_s_vT_pre is None:
+            self._grad_s_s_vT_pre = self._grad_s_s_vT_final_iteration_analytical(use_pre=True)
+        return self._grad_s_s_vT_pre
 
-        cashflow = None if self.cashflow is None else float(self.cashflow)
-        return {
-            **super().cashflows(curve, disc_curve_, fx, base),
-            defaults.headers["rate"]: self.fixed_rate,
-            defaults.headers["spread"]: None,
-            defaults.headers["cashflow"]: cashflow,
-            defaults.headers["npv"]: npv,
-            defaults.headers["fx"]: float(fx),
-            defaults.headers["npv_fx"]: npv_fx,
-        }
+    @property
+    def grad_v_v_rT_pre(self):
+        """
+        Alias of ``J2_pre``.
+        """
+        return self.J2_pre  # pragma: no cover
 
+    def grad_f_s_vT_pre(self, fx_vars):
+        """
+        3d array of second derivatives of curve variables with respect to
+        FX rates and calibrating instrument rates, of size (len(fx_vars), pre_m, pre_n);
 
-def _validate_float_args(
-    fixing_method: Union[str, NoInput],
-    method_param: Union[int, NoInput],
-    spread_compound_method: Union[str, NoInput],
-):
-    """
-    Validate the argument input to float periods.
+        .. math::
 
-    Returns
-    -------
-    tuple
-    """
-    if fixing_method is NoInput.blank:
-        fixing_method_: str = defaults.fixing_method
-    else:
-        fixing_method_ = fixing_method.lower()
-    if fixing_method_ not in [
-        "ibor",
-        "rfr_payment_delay",
-        "rfr_observation_shift",
-        "rfr_lockout",
-        "rfr_lookback",
-        "rfr_payment_delay_avg",
-        "rfr_observation_shift_avg",
-        "rfr_lockout_avg",
-        "rfr_lookback_avg",
-    ]:
-        raise ValueError(
-            "`fixing_method` must be in {'rfr_payment_delay', "
-            "'rfr_observation_shift', 'rfr_lockout', 'rfr_lookback', 'ibor'}, "
-            f"got '{fixing_method_}'."
-        )
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{s} \\mathbf{v^T}]_{i,j,k} = \\frac{\\partial^2 v_k}{\\partial f_i \\partial s_j}
 
-    if method_param is NoInput.blank:
-        method_param_: int = defaults.fixing_method_param[fixing_method_]
-    else:
-        method_param_ = method_param
-    if method_param_ != 0 and fixing_method_ == "rfr_payment_delay":
-        raise ValueError(
-            "`method_param` should not be used (or a value other than 0) when "
-            f"using a `fixing_method` of 'rfr_payment_delay', got {method_param_}. "
-            f"Configure the `payment_lag` option instead to have the "
-            f"appropriate effect."
-        )
-    elif fixing_method_ == "rfr_lockout" and method_param_ < 1:
-        raise ValueError(
-            f'`method_param` must be >0 for "rfr_lockout" `fixing_method`, ' f"got {method_param_}"
-        )
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities.
+        """
+        # FX sensitivity requires reverting through all pre-solvers rates.
+        _ = -np.tensordot(self.grad_f_v_rT_pre(fx_vars), self.grad_s_vT_pre, (1, 1)).swapaxes(1, 2)
+        _ = np.tensordot(_, self.grad_s_vT_pre, (2, 0))
+        grad_f_s_vT = _
+        return grad_f_s_vT
 
-    if spread_compound_method is NoInput.blank:
-        spread_compound_method_: str = defaults.spread_compound_method
-    else:
-        spread_compound_method_ = spread_compound_method.lower()
-    if spread_compound_method_ not in [
-        "none_simple",
-        "isda_compounding",
-        "isda_flat_compounding",
-    ]:
-        raise ValueError(
-            "`spread_compound_method` must be in {'none_simple', "
-            "'isda_compounding', 'isda_flat_compounding'}, "
-            f"got {spread_compound_method_}"
-        )
-    return fixing_method_, method_param_, spread_compound_method_
+    def grad_f_f_vT_pre(self, fx_vars):
+        """
+        3d array of second derivatives of curve variables with respect to
+        FX rates, of size (len(fx_vars), len(fx_vars), pre_n);
 
+        .. math::
 
-class FloatPeriod(BasePeriod):
-    """
-    Create a period defined with a floating rate index.
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{f} \\mathbf{v^T}]_{i,j,k} = \\frac{\\partial^2 v_k}{\\partial f_i \\partial f_j}
 
-    Parameters
-    ----------
-    args : dict
-        Required positional args to :class:`BasePeriod`.
-    float_spread : float or None, optional
-        The float spread applied to determine the cashflow. Can be set to `None` and
-        set later, typically after a mid-market float spread for all periods
-        has been calculated. **Expressed in basis points (bps).**
-    spread_compound_method : str, optional
-        The method to use for adding a floating rate to compounded rates. Available
-        options are `{"none_simple", "isda_compounding", "isda_flat_compounding"}`.
-    fixings : float, list, or Series, optional
-        If a float scalar, will be applied as the determined fixing for the whole
-        period. If a list of *n* fixings will be used as the first *n* RFR fixings
-        in the period and the remaining fixings will be forecast from the curve and
-        composed into the overall rate. If a datetime indexed ``Series`` will use the
-        fixings that are available in that object, and derive the rest from the
-        ``curve``. **Must be input excluding** ``float_spread``.
-    fixing_method : str, optional
-        The method by which floating rates are determined, set by default. See notes.
-    method_param : int, optional
-        A parameter that is used for the various ``fixing_method`` s. See notes.
-    kwargs : dict
-        Required keyword arguments to :class:`BasePeriod`.
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities.
+        """
+        # FX sensitivity requires reverting through all pre-solvers rates.
+        _ = -np.tensordot(self.grad_f_f_rT_pre(fx_vars), self.grad_s_vT_pre, (2, 0))
+        _ -= np.tensordot(self.grad_f_rT_pre(fx_vars), self.grad_f_s_vT_pre(fx_vars), (1, 1))
+        grad_f_f_vT = _
+        return grad_f_f_vT
 
-    Notes
-    -----
-    The ``cashflow`` is defined as follows;
+    def grad_f_vT_pre(self, fx_vars):
+        """
+        2d array of the derivatives of curve variables with respect to FX rates, of
+        size (len(fx_vars), pre_n).
 
-    .. math::
+        .. math::
 
-       C = -Ndr(r_i, z)
+           [\\nabla_\\mathbf{f}\\mathbf{v^T}]_{i,j} = \\frac{\\partial v_j}{\\partial f_i} = -\\frac{\\partial r_z}{\\partial f_i} \\frac{\\partial v_j}{\\partial s_z}
 
-    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+        Parameters
+        ----------
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities
+        """
+        # FX sensitivity requires reverting through all pre-solvers rates.
+        grad_f_rT = np.array([gradient(rate, fx_vars) for rate in self.r_pre]).T
+        return -np.matmul(grad_f_rT, self.grad_s_vT_pre)
 
-    .. math::
+    def grad_f_f(self, f, fx_vars):
+        """
+        1d array of total derivatives of FX conversion rate with respect to
+        FX rate variables, of size (len(fx_vars));
 
-       P = Cv(m) = -Ndr(r_i, z)v(m)
+        .. math::
 
-    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+           [\\nabla_\\mathbf{f} f_{loc:bas}]_{i} = \\frac{d f}{d f_i}
 
-    .. math::
+        Parameters
+        ----------
+        f : Dual or Dual2
+            The value of the local to base FX conversion rate.
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities
+        """
+        grad_f_f = gradient(f, fx_vars)
+        grad_f_f += np.matmul(self.grad_f_vT_pre(fx_vars), gradient(f, self.pre_variables))
+        return grad_f_f
 
-       A = - \\frac{\\partial P}{\\partial z} = Ndv(m) \\frac{\\partial r}{\\partial z}
+    @property
+    def grad_s_vT_pre(self):
+        """
+        2d Jacobian array of curve variables with respect to calibrating instruments
+        including all pre solvers attached to the Solver, of size (pre_m, pre_n).
 
-    **Fixing Methods**
+        .. math::
 
-    Floating period rates depend on different ``fixing_method`` to determine their
-    rates. For further info see
-    :download:`ISDA RFR Compounding Memo (2006)<_static/isda-memo-rfrs-2006.pdf>`.
-    The available options provided here are:
+           [\\nabla_\\mathbf{s}\\mathbf{v^T}]_{i,j} = \\frac{\\partial v_j}{\\partial s_i} = \\mathbf{J^+}
+        """
+        if len(self.pre_solvers) == 0:
+            return self.grad_s_vT
 
-    - **"rfr_payment_delay"**: this is the standard convention adopted by interbank
-      RFR derivative trades, such as SOFR, SONIA, and ESTR OIS etc. ``method_param``
-      is not used for this method and defaults to zero, ``payment_lag`` serves as the
-      appropriate parameter for this method.
-    - **"rfr_observation_shift"**: typical conventions of FRNs. The ``method_param``
-      is the integer number of business days by which both the observation
-      rates and the DCFs are shifted.
-    - **"rfr_lockout"**: this is a convention typically used on floating rate notes
-      (FRNs), the ``method_param`` as integer number of business days is
-      the number of locked-out days. E.g. SOFR based FRNs generally have 4.
-    - **"rfr_lookback"**: this is also a convention typically used on FRNs. The
-      ``method_param`` as integer number of business days defines the
-      observation offset, the DCFs remain static, measured between the start and end
-      dates.
-    - **"rfr_payment_delay_avg", "rfr_observation_shift_avg", "rfr_lockout_avg",
-      "rfr_lookback_avg"**: these are the same as the previous conventions except that
-      the period rate is defined as the arithmetic average of the individual fixings,
-      weighted by the relevant DCF depending upon the method.
-    - **"ibor"**: this the convention for determining IBOR rates from a curve. The
-      ``method_param`` is the number of fixing lag days before the accrual start when
-      the fixing is published. For example, Euribor or Stibor have 2.
+        if self._grad_s_vT_pre is None:
+            grad_s_vT = np.zeros(shape=(self.pre_m, self.pre_n))
 
-    The first two are the only methods recommended by Alternative Reference Rates
-    Comittee (AARC), although other methods have been implemented in
-    financial instruments previously.
+            i, j = 0, 0
+            for pre_solver in self.pre_solvers:
+                # create the left side block matrix
+                m, n = pre_solver.pre_m, pre_solver.pre_n
+                grad_s_vT[i : i + m, j : j + n] = pre_solver.grad_s_vT_pre
 
-    **Spread Compounding Methods**
+                # create the right column dependencies
+                grad_v_r = np.array([gradient(r, pre_solver.pre_variables) for r in self.r]).T
+                block = np.matmul(grad_v_r, self.grad_s_vT)
+                block = -1 * np.matmul(pre_solver.grad_s_vT_pre, block)
+                grad_s_vT[i : i + m, -self.m :] = block
 
-    The spread compounding methods operate as follows:
+                i, j = i + m, j + n
 
-    - **"none_simple"**: the float spread added in a simple way to the determined
-      compounded period rate.
-    - **"isda_compounding"**: the float spread is added to each individual rate
-      and then everything is compounded.
-    - **"isda_flat_compounding"**: the spread is added to each rate but is not used
-      when compounding each previously calculated component.
+            # create bottom right block
+            grad_s_vT[-self.m :, -self.m :] = self.grad_s_vT
+            self._grad_s_vT_pre = grad_s_vT
+        return self._grad_s_vT_pre
 
-    The first is the most efficient and most encountered. The second and third are
-    rarely encountered in modern financial instruments.
-    For further info see
-    :download:`ISDA Compounding Memo (2009)<_static/isda-compounding-memo.pdf>`.
+    def grad_s_f_pre(self, f):
+        """
+        1d array of FX conversion rate with respect to calibrating instruments,
+        of size (pre_m);
 
-    .. _float fixings:
+        .. math::
 
-    **Fixings**
+           [\\nabla_\\mathbf{s} f_{loc:bas}]_{i} = \\frac{\\partial f}{\\partial s_i}
 
-    .. warning::
+        Parameters
+        ----------
+        f : Dual or Dual2
+            The value of the local to base FX conversion rate.
+        """
+        _ = np.tensordot(self.grad_s_vT_pre, gradient(f, self.pre_variables), (1, 0))
+        grad_s_f = _
+        return grad_s_f
 
-       Providing ``fixings`` as a ``Series`` is **best practice**.
+    def grad_s_sT_f_pre(self, f):
+        """
+        2d array of derivatives of FX conversion rate with respect to
+        calibrating instruments, of size (pre_m, pre_m);
 
-       But, **RFR** and **IBOR** fixings provided as datetime indexed ``Series`` require
-       **different formats**:
+        .. math::
 
-       - IBOR fixings are indexed by publication date and fixing value.
-       - RFR fixings are indexed by reference value date and fixing value.
+           [\\nabla_\\mathbf{s} \\nabla_\\mathbf{s}^\\mathbf{T} f_{loc:bas}]_{i,j} = \\frac{\\partial^2 f}{\\partial s_i \\partial s_j}
 
-    If an *"ibor"* ``fixing
-    method`` is given the series should index the published IBOR rates by
-    **publication date**, which usually lags the reference value dates.
-    For example, EURIBOR lags its
-    value dates by two business days. 3M EURIBOR was published on Thu-2-Mar-2023 as
-    2.801%, which is applicable to the start date of Mon-6-Mar-2023 with value end
-    date of Tue-6-Jun-2023.
+        Parameters
+        ----------
+        f : Dual or Dual2
+            The value of the local to base FX conversion rate.
+        """
+        grad_s_vT = self.grad_s_vT_pre
+        grad_v_vT_f = gradient(f, self.pre_variables, order=2)
 
-    .. ipython:: python
+        _ = np.tensordot(grad_s_vT, grad_v_vT_f, (1, 0))
+        _ = np.tensordot(_, grad_s_vT, (1, 1))
 
-       ibor_curve = Curve(
-           nodes={dt(2023, 3, 6): 1.0, dt(2024, 3, 6): 0.96},
-           calendar="bus"
-       )
-       fixings = Series(
-           [1.00, 2.801, 1.00, 1.00],
-           index=[dt(2023, 3, 1), dt(2023, 3, 2), dt(2023, 3, 3), dt(2023, 3, 6)]
-       )
-       float_period = FloatPeriod(
-           start=dt(2023, 3, 6),
-           end=dt(2023, 6, 6),
-           payment=dt(2023, 6, 6),
-           frequency="Q",
-           fixing_method="ibor",
-           method_param=2,
-           fixings=fixings
-       )
-       float_period.rate(ibor_curve)  # this will return the fixing published 2-Mar-23
-       float_period.fixings_table(ibor_curve)
-
-    RFR rates tend to be maintained by central banks. The modern tendency seems to be
-    to present historical RFR data indexed by **reference value date** and not
-    publication date, which is usually 1 business day in arrears. If the
-    ``fixing_method`` is *"rfr"* based then the given series should be indexed in a
-    similar manner. ESTR was published as 2.399% on Fri-3-Mar-2023 for the reference
-    value start date of Thu-2-Mar-2023 (and end date of Fri-3-Mar-2023).
+        grad_s_sT_f = _
+        return grad_s_sT_f
 
-    .. ipython:: python
+    def grad_f_sT_f_pre(self, f, fx_vars):
+        """
+        2d array of derivatives of FX conversion rate with respect to
+        calibrating instruments, of size (pre_m, pre_m);
 
-       rfr_curve = Curve(
-           nodes={dt(2023, 3, 3): 1.0, dt(2024, 3, 3): 0.96},
-           calendar="bus"
-       )
-       fixings = Series(
-           [1.00, 1.00, 2.399],
-           index=[dt(2023, 2, 28), dt(2023, 3, 1), dt(2023, 3, 2)]
-       )
-       float_period = FloatPeriod(
-           start=dt(2023, 3, 2),
-           end=dt(2023, 3, 3),
-           payment=dt(2023, 3, 3),
-           frequency="A",
-           fixing_method="rfr_payment_delay",
-           fixings=fixings
-       )
-       float_period.rate(rfr_curve)  # this will return the fixing for reference 2-Mar-23
-       float_period.fixings_table(rfr_curve)
+        .. math::
 
-    Examples
-    --------
-    Create a stepped (log-linear interpolated) curve with 2 relevant steps:
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{s}^\\mathbf{T} f_{loc:bas}(\\mathbf{v(s, f), f)})]_{i,j} = \\frac{d^2 f}{d f_i \\partial s_j}
 
-    .. ipython:: python
+        Parameters
+        ----------
+        f : Dual or Dual2
+            The value of the local to base FX conversion rate.
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities
+        """
+        grad_s_vT = self.grad_s_vT_pre
+        grad_v_f = gradient(f, self.pre_variables)
+        grad_f_sT_v = self.grad_f_s_vT_pre(fx_vars)
+        _ = gradient(f, self.pre_variables + tuple(fx_vars), order=2)
+        grad_v_vT_f = _[: self.pre_n, : self.pre_n]
+        grad_f_vT_f = _[self.pre_n :, : self.pre_n]
+        # grad_f_fT_f = _[self.pre_n :, self.pre_n :]
+        grad_f_vT = self.grad_f_vT_pre(fx_vars)
+
+        _ = np.tensordot(grad_f_sT_v, grad_v_f, (2, 0))
+        _ += np.tensordot(grad_f_vT_f, grad_s_vT, (1, 1))
+
+        __ = np.tensordot(grad_f_vT, grad_v_vT_f, (1, 0))
+        __ = np.tensordot(__, grad_s_vT, (1, 1))
 
-       curve = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.999, dt(2022, 3, 1): 0.997})
-       curve.rate(dt(2022, 1, 1), "1D")
-       curve.rate(dt(2022, 2, 1), "1D")
+        grad_f_sT_f = _ + __
+        return grad_f_sT_f
 
-    A standard `"rfr_payment_delay"` period, which is the default for this library.
+    def grad_f_fT_f_pre(self, f, fx_vars):
+        """
+        2d array of derivatives of FX conversion rate with respect to
+        calibrating instruments, of size (pre_m, pre_m);
 
-    .. ipython:: python
+        .. math::
 
-       period = FloatPeriod(
-           start=dt(2022, 1, 1),
-           end=dt(2022, 3, 1),
-           payment=dt(2022, 3, 1),
-           frequency="M",
-       )
-       period.fixing_method
-       period.rate(curve)
-
-    An `"rfr_lockout"` period, here with 28 business days lockout (under a curve
-    with a no holidays) meaning the observation period
-    ends on the 1st Feb 2022 and the 1D rate between 31st Jan 2022 and 1st Feb is used
-    consistently as the fixing for the remaining fixing dates.
+           [\\nabla_\\mathbf{f} \\nabla_\\mathbf{f}^\\mathbf{T} f_{loc:bas}(\\mathbf{v(s, f), f)})]_{i,j} = \\frac{d^2 f}{d f_i d f_j}
 
-    .. ipython:: python
+        Parameters
+        ----------
+        f : Dual or Dual2
+            The value of the local to base FX conversion rate.
+        fx_vars : list or tuple of str
+            The variable name tags for the FX rate sensitivities
+        """
+        # grad_s_vT = self.grad_s_vT_pre
+        grad_v_f = gradient(f, self.pre_variables)
+        # grad_f_sT_v = self.grad_f_s_vT_pre(fx_vars)
+        _ = gradient(f, self.pre_variables + tuple(fx_vars), order=2)
+        grad_v_vT_f = _[: self.pre_n, : self.pre_n]
+        grad_f_vT_f = _[self.pre_n :, : self.pre_n]
+        grad_f_fT_f = _[self.pre_n :, self.pre_n :]
+        grad_f_vT = self.grad_f_vT_pre(fx_vars)
+        grad_f_fT_v = self.grad_f_f_vT_pre(fx_vars)
+
+        _ = grad_f_fT_f
+        _ += 2.0 * np.tensordot(grad_f_vT_f, grad_f_vT, (1, 1))
+        _ += np.tensordot(grad_f_fT_v, grad_v_f, (2, 0))
+
+        __ = np.tensordot(grad_f_vT, grad_v_vT_f, (1, 0))
+        __ = np.tensordot(__, grad_f_vT, (1, 1))
+
+        grad_f_fT_f = _ + __
+        return grad_f_fT_f
 
-       period = FloatPeriod(
-           start=dt(2022, 1, 1),
-           end=dt(2022, 3, 1),
-           payment=dt(2022, 3, 1),
-           frequency="M",
-           fixing_method="rfr_lockout",
-           method_param=28,
-       )
-       period.rate(curve)
+    # grad_v_v_f: calculated within grad_s_vT_fixed_point_iteration
 
-    An `"rfr_lookback"` period, here with 5 days offset meaning the observation period
-    starts on 27th Jan and ends on 6th Feb.
+    # delta and gamma calculations require all solver and pre_solver variables
 
-    .. ipython:: python
+    def grad_s_Ploc(self, npv):
+        """
+        1d array of derivatives of local currency PV with respect to calibrating
+        instruments, of size (pre_m).
 
-       period = FloatPeriod(
-           start=dt(2022, 2, 1),
-           end=dt(2022, 2, 11),
-           payment=dt(2022, 2, 11),
-           frequency="M",
-           fixing_method="rfr_lookback",
-           method_param=5,
-       )
-       period.rate(curve)
+        .. math::
 
-    An `"ibor"` period, with a 2 day fixing lag
+           \\nabla_\\mathbf{s} P^{loc} = \\frac{\\partial P^{loc}}{\\partial s_i}
 
-    .. ipython:: python
-       :okexcept:
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+        """
+        grad_s_P = np.matmul(self.grad_s_vT_pre, gradient(npv, self.pre_variables))
+        return grad_s_P
 
-       period = FloatPeriod(
-           start=dt(2022, 1, 3),
-           end=dt(2022, 3, 3),
-           payment=dt(2022, 3, 3),
-           frequency="B",
-           fixing_method="ibor",
-           method_param=2,
-       )
-       period.rate(curve)
-       curve.rate(dt(2022, 1, 3), "2M")
-    """
+    def grad_f_Ploc(self, npv, fx_vars):
+        """
+        1d array of derivatives of local currency PV with respect to FX rate variable,
+        of size (len(fx_vars)).
 
-    def __init__(
-        self,
-        *args,
-        float_spread: Union[float, NoInput] = NoInput(0),
-        fixings: Union[float, list, Series, NoInput] = NoInput(0),
-        fixing_method: Union[str, NoInput] = NoInput(0),
-        method_param: Union[int, NoInput] = NoInput(0),
-        spread_compound_method: Union[str, NoInput] = NoInput(0),
-        **kwargs,
-    ):
-        self.float_spread = 0.0 if float_spread is NoInput.blank else float_spread
+        .. math::
 
-        (
-            self.fixing_method,
-            self.method_param,
-            self.spread_compound_method,
-        ) = _validate_float_args(fixing_method, method_param, spread_compound_method)
-
-        self.fixings = fixings
-        if isinstance(self.fixings, list) and self.fixing_method == "ibor":
-            raise ValueError("`fixings` cannot be supplied as list, under 'ibor' `fixing_method`.")
-
-        # self.calendar = get_calendar(calendar)
-        # self.modifier = modifier
-        super().__init__(*args, **kwargs)
+           \\nabla_\\mathbf{f} P^{loc}(\\mathbf{v(s, f), f}) = \\frac{\\partial P^{loc}}{\\partial f_i}+  \\frac{\partial v_z}{\\partial f_i} \\frac{\\partial P^{loc}}{\\partial v_z}
 
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-    # Commercial use of this code, and/or copying and redistribution is prohibited.
-    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        grad_f_P = gradient(npv, fx_vars)
+        grad_f_P += np.matmul(self.grad_f_vT_pre(fx_vars), gradient(npv, self.pre_variables))
+        return grad_f_P
 
-    def analytic_delta(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ):
+    def grad_s_Pbase(self, npv, grad_s_P, f):
         """
-        Return the analytic delta of the *FloatPeriod*.
-        See
-        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
-        """
-        if self.spread_compound_method == "none_simple" or self.float_spread == 0:
-            # then analytic_delta is not impacted by float_spread compounding
-            dr_dz = 1.0
-        elif isinstance(curve, Curve):
-            _ = self.float_spread
-            DualType = Dual if curve.ad in [0, 1] else Dual2
-            DualArgs = ([],) if curve.ad in [0, 1] else ([], [])
-            self.float_spread = DualType(float(_), ["z_float_spread"], *DualArgs)
-            rate = self.rate(curve)
-            dr_dz = gradient(rate, ["z_float_spread"])[0] * 100
-            self.float_spread = _
-        else:
-            raise TypeError("`curve` must be supplied for given `spread_compound_method`")
+        1d array of derivatives of base currency PV with respect to calibrating
+        instruments, of size (pre_m).
 
-        return dr_dz * super().analytic_delta(curve, disc_curve, fx, base)
+        .. math::
 
-    def cashflows(
-        self,
-        curve: Union[Curve, dict, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ):
-        """
-        Return the cashflows of the *FloatPeriod*.
-        See
-        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
-        """
-        fx, base = _get_fx_and_base(self.currency, fx, base)
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-
-        if curve is not NoInput.blank:
-            cashflow = float(self.cashflow(curve))
-            rate = float(100 * cashflow / (-self.notional * self.dcf))
-            npv = float(self.npv(curve, disc_curve_))
-            npv_fx = npv * float(fx)
-        else:
-            cashflow, rate, npv, npv_fx = None, None, None, None
+           \\nabla_\\mathbf{s} P^{bas}(\\mathbf{v(s, f)}) = \\nabla_\\mathbf{s} P^{loc}(\\mathbf{v(s, f)})  f_{loc:bas} + P^{loc} \\nabla_\\mathbf{s} f_{loc:bas}
 
-        return {
-            **super().cashflows(curve, disc_curve_, fx, base),
-            defaults.headers["rate"]: rate,
-            defaults.headers["spread"]: float(self.float_spread),
-            defaults.headers["cashflow"]: cashflow,
-            defaults.headers["npv"]: npv,
-            defaults.headers["fx"]: float(fx),
-            defaults.headers["npv_fx"]: npv_fx,
-        }
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            grad_s_P : ndarray
+                The local currency delta risks w.r.t. calibrating instruments.
+            f : Dual or Dual2
+                The local:base FX rate.
+        """
+        grad_s_Pbas = float(npv) * np.matmul(self.grad_s_vT_pre, gradient(f, self.pre_variables))
+        grad_s_Pbas += grad_s_P * float(f)  # <- use float to cast float array not Dual
+        return grad_s_Pbas
 
-    def npv(
-        self,
-        curve: Union[Curve, dict, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-        local: bool = False,
-    ):
+    def grad_f_Pbase(self, npv, grad_f_P, f, fx_vars):
         """
-        Return the cashflows of the *FloatPeriod*.
-        See
-        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        if not isinstance(disc_curve_, Curve) or curve is NoInput.blank:
-            raise TypeError("`curves` have not been supplied correctly.")
-        if self.payment < disc_curve_.node_dates[0]:
-            if local:
-                return {self.currency: 0.0}
-            else:
-                return 0.0  # payment date is in the past avoid issues with fixings or rates
-        value = self.rate(curve) / 100 * self.dcf * disc_curve_[self.payment] * -self.notional
-        if local:
-            return {self.currency: value}
-        else:
-            fx, _ = _get_fx_and_base(self.currency, fx, base)
-            return fx * value
+        1d array of derivatives of base currency PV with respect to FX rate variables,
+        of size (len(fx_vars)).
 
-    def cashflow(self, curve: Union[Curve, LineCurve, dict]) -> Union[None, DualTypes]:
-        if curve is None:
-            return None
-        else:
-            rate = None if curve is None else self.rate(curve)
-            _ = -self.notional * self.dcf * rate / 100
-            return _
+        .. math::
+
+           \\nabla_\\mathbf{s} P^{bas}(\\mathbf{v(s, f)}) = \\nabla_\\mathbf{s} P^{loc}(\\mathbf{v(s, f)})  f_{loc:bas} + P^{loc} \\nabla_\\mathbf{s} f_{loc:bas}
 
-    def rate(self, curve: Union[Curve, LineCurve, dict]):
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            grad_f_P : ndarray
+                The local currency delta risks w.r.t. FX pair variables.
+            f : Dual or Dual2
+                The local:base FX rate.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        ret = grad_f_P * float(f)  # <- use float here to cast float array not Dual
+        ret += float(npv) * self.grad_f_f(f, fx_vars)
+        return ret
+
+    def grad_s_sT_Ploc(self, npv):
         """
-        Calculating the floating rate for the period.
+        2d array of derivatives of local currency PV with respect to calibrating
+        instruments, of size (pre_m, pre_m).
 
-        Parameters
-        ----------
-        curve : Curve, LineCurve, IndexCurve, dict of curves
-            The forecasting curve object.
+        .. math::
 
-        Returns
-        -------
-        float, Dual, Dual2
+           \\nabla_\\mathbf{s} \\nabla_\\mathbf{s}^\\mathbf{T} P^{loc}(\\mathbf{v, f}) = \\frac{ \\partial^2 P^{loc}(\\mathbf{v(s, f)}) }{\\partial s_i \\partial s_j}
 
-        Examples
-        --------
-        Using a single forecast *Curve*.
+        Parameters:
+            npv : Dual2
+                A local currency NPV of a period of a leg.
+        """
+        # instrument-instrument cross gamma:
+        _ = np.tensordot(gradient(npv, self.pre_variables, order=2), self.grad_s_vT_pre, (1, 1))
+        _ = np.tensordot(self.grad_s_vT_pre, _, (1, 0))
+
+        _ += np.tensordot(self.grad_s_s_vT_pre, gradient(npv, self.pre_variables), (2, 0))
+        grad_s_sT_P = _
+        return grad_s_sT_P
+        # grad_s_sT_P = np.matmul(
+        #     self.grad_s_vT_pre,
+        #     np.matmul(
+        #         npv.gradient(self.pre_variables, order=2), self.grad_s_vT_pre.T
+        #     ),
+        # )
+        # grad_s_sT_P += np.matmul(
+        #     self.grad_s_s_vT_pre, npv.gradient(self.pre_variables)[:, None]
+        # )[:, :, 0]
 
-        .. ipython:: python
+    def gradp_f_vT_Ploc(self, npv, fx_vars):
+        """
+        2d array of (partial) derivatives of local currency PV with respect to
+        FX rate variables and curve variables, of size (len(fx_vars), pre_n).
 
-           period.rate(curve)
+        .. math::
 
-        Using a dict of *Curves* for stub periods calculable under an *"ibor"* ``fixing_method``.
+           \\nabla_\\mathbf{f} \\nabla_\\mathbf{v}^\\mathbf{T} P^{loc}(\\mathbf{v, f}) = \\frac{ \\partial ^2 P^{loc}(\\mathbf{v, f)}) }{\\partial f_i \\partial v_j}
 
-        .. ipython:: python
+        Parameters:
+            npv : Dual2
+                A local currency NPV of a period of a leg.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        grad_x_xT_Ploc = gradient(npv, self.pre_variables + tuple(fx_vars), order=2)
+        grad_f_vT_Ploc = grad_x_xT_Ploc[self.pre_n :, : self.pre_n]
+        return grad_f_vT_Ploc
 
-           period.rate({"1m": curve, "3m": curve, "6m": curve, "12m": curve})
+    def grad_f_sT_Ploc(self, npv, fx_vars):
         """
-        if isinstance(self.fixings, (float, Dual, Dual2)):
-            # if fixings is a single value then return that value (curve unused)
-            if (
-                self.spread_compound_method in ["isda_compounding", "isda_flat_compounding"]
-                and self.float_spread != 0
-                and "rfr" in self.fixing_method
-            ):
-                warnings.warn(
-                    "Unless the RFR period is a 1-day tenor, "
-                    "a single scalar fixing will not be compounded correctly"
-                    "with the given `spread_compound_method`, and "
-                    "`float_spread`",
-                    UserWarning,
-                )
+        2d array of derivatives of local currency PV with respect to calibrating
+        instruments, of size (pre_m, pre_m).
 
-            # this ignores spread_compound_type
-            return self.fixings + self.float_spread / 100
+        .. math::
 
-        # else next calculations made based on fixings in (None, list, Series)
+           \\nabla_\\mathbf{f} \\nabla_\\mathbf{s}^\\mathbf{T} P^{loc}(\\mathbf{v(s, f), f}) = \\frac{ d^2 P^{loc}(\\mathbf{v(s, f), f)}) }{d f_i \\partial s_j}
 
-        if "rfr" in self.fixing_method:
-            method = {
-                "dfs": self._rfr_rate_from_df_curve,
-                "values": self._rfr_rate_from_line_curve,
-            }
-            try:
-                return method[curve._base_type](curve)
-            except AttributeError:
-                raise ValueError(
-                    "Must supply a valid curve for forecasting.\n"
-                    "Do not supply a dict of curves for RFR based methods."
-                )
-        elif "ibor" in self.fixing_method:
-            method = {
-                "dfs": self._ibor_rate_from_df_curve,
-                "values": self._ibor_rate_from_line_curve,
-            }
-            if not isinstance(curve, dict):
-                return method[curve._base_type](curve)
-            else:
-                if not self.stub:
-                    curve = curve[f"{self.freq_months}m"]
-                    return method[curve._base_type](curve)
-                else:
-                    return self._interpolated_ibor_from_curve_dict(curve)
-        else:
-            raise ValueError("`fixing_method` not valid for the FloatPeriod.")  # pragma: no cover
+        Parameters:
+            npv : Dual2
+                A local currency NPV of a period of a leg.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        # fx_rate-instrument cross gamma:
+        _ = np.tensordot(
+            self.grad_f_vT_pre(fx_vars),
+            gradient(npv, self.pre_variables, order=2),
+            (1, 0),
+        )
+        _ += self.gradp_f_vT_Ploc(npv, fx_vars)
+        _ = np.tensordot(_, self.grad_s_vT_pre, (1, 1))
+        _ += np.tensordot(self.grad_f_s_vT_pre(fx_vars), gradient(npv, self.pre_variables), (2, 0))
+        grad_f_sT_Ploc = _
+        return grad_f_sT_Ploc
 
-    def _interpolated_ibor_from_curve_dict(self, curve: dict):
-        """
-        Get the rate on all available curves in dict and then determine the ones to interpolate.
+    def grad_f_fT_Ploc(self, npv, fx_vars):
         """
-        calendar = next(iter(curve.values())).calendar  # note: ASSUMES all curve calendars are same
-        fixing_date = add_tenor(self.start, f"-{self.method_param}B", NoInput(0), calendar)
-
-        def _rate(c: Union[Curve, LineCurve, IndexCurve], tenor):
-            if c._base_type == "dfs":
-                return c.rate(self.start, tenor)
-            else:  # values
-                return c.rate(fixing_date)
-
-        values = {add_tenor(self.start, k, "MF", calendar): _rate(v, k) for k, v in curve.items()}
-        values = dict(sorted(values.items()))
-        dates, rates = list(values.keys()), list(values.values())
-        if self.end > dates[-1]:
-            warnings.warn(
-                "Interpolated stub period has a length longer than the provided "
-                "IBOR curve tenors: using the longest IBOR value.",
-                UserWarning,
-            )
-            return rates[-1]
-        elif self.end < dates[0]:
-            warnings.warn(
-                "Interpolated stub period has a length shorter than the provided "
-                "IBOR curve tenors: using the shortest IBOR value.",
-                UserWarning,
-            )
-            return rates[0]
-        else:
-            i = index_left(dates, len(dates), self.end)
-            _ = rates[i] + (rates[i + 1] - rates[i]) * (
-                (self.end - dates[i]) / (dates[i + 1] - dates[i])
-            )
-            return _
+        2d array of derivatives of local currency PV with respect to FX rate variables,
+        of size (len(fx_vars), len(fx_vars)).
 
-    def _ibor_rate_from_df_curve(self, curve: Curve):
-        # the compounding method has no effect on single rate (ibor) fixings.
-        if isinstance(self.fixings, Series):
-            # check if we return published IBOR rate
-            fixing_date = add_tenor(self.start, f"-{self.method_param}B", None, curve.calendar)
-            try:
-                return self.fixings[fixing_date] + self.float_spread / 100
-            except KeyError:
-                # TODO warn if Series contains close dates but cannot find a value for exact date.
-                # fixing not available: use curve
-                pass
-        elif isinstance(self.fixings, list):  # this is also validated in __init__
-            raise ValueError("`fixings` cannot be supplied as list, under 'ibor' `fixing_method`.")
+        .. math::
 
-        if self.stub:
-            r = curve.rate(self.start, self.end) + self.float_spread / 100
-        else:
-            r = curve.rate(self.start, f"{self.freq_months}m") + self.float_spread / 100
-        return r
+           \\nabla_\\mathbf{f} \\nabla_\\mathbf{s}^\\mathbf{T} P^{loc}(\\mathbf{v(s, f), f}) = \\frac{ d^2 P^{loc}(\\mathbf{v(s, f), f)}) }{d f_i d f_j}
 
-    def _ibor_rate_from_line_curve(self, curve: LineCurve):
-        # the compounding method has no effect on single rate (ibor) fixings.
-        fixing_date = add_tenor(self.start, f"-{self.method_param}B", NoInput(0), curve.calendar)
-        if isinstance(self.fixings, Series):
-            try:
-                return self.fixings[fixing_date] + self.float_spread / 100
-            except KeyError:
-                # TODO warn if Series contains close dates but cannot find a value for exact date.
-                # fixing not available: use curve
-                pass
-        elif isinstance(self.fixings, list):  # this is also validated in __init__
-            raise ValueError("`fixings` cannot be supplied as list, under 'ibor' `fixing_method`.")
-
-        return curve[fixing_date] + self.float_spread / 100
-
-    def _rfr_rate_from_df_curve(self, curve: Curve):
-        if self.fixing_method == "rfr_payment_delay" and not self._is_inefficient:
-            return curve.rate(self.start, self.end) + self.float_spread / 100
-
-        elif self.fixing_method == "rfr_observation_shift" and not self._is_inefficient:
-            start = add_tenor(self.start, f"-{self.method_param}b", "P", curve.calendar)
-            end = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
-            return curve.rate(start, end) + self.float_spread / 100
-            # TODO: (low:perf) semi-efficient method for lockout under certain conditions
-        else:
-            # return inefficient calculation
-            # this is also the path for all averaging methods
-            return self._rfr_fixings_array(curve, fixing_exposure=False)[0]
+        Parameters:
+            npv : Dual2
+                A local currency NPV of a period of a leg.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        # fx_rate-instrument cross gamma:
+        gradp_f_vT_Ploc = self.gradp_f_vT_Ploc(npv, fx_vars)
+        grad_f_vT_pre = self.grad_f_vT_pre(fx_vars)
+        grad_v_Ploc = gradient(npv, self.pre_variables)
+        grad_v_vT_Ploc = gradient(npv, self.pre_variables, order=2)
+
+        _ = gradient(npv, fx_vars, order=2)
+        _ += np.tensordot(self.grad_f_f_vT_pre(fx_vars), grad_v_Ploc, (2, 0))
+        _ += np.tensordot(grad_f_vT_pre, gradp_f_vT_Ploc, (1, 1))
+        _ += np.tensordot(gradp_f_vT_Ploc, grad_f_vT_pre, (1, 1))
+
+        __ = np.tensordot(grad_f_vT_pre, grad_v_vT_Ploc, (1, 0))
+        __ = np.tensordot(__, grad_f_vT_pre, (1, 1))
 
-    def _rfr_rate_from_line_curve(self, curve: LineCurve):
-        return self._rfr_fixings_array(curve, fixing_exposure=False)[0]
+        grad_f_f_Ploc = _ + __
+        return grad_f_f_Ploc
 
-    def _avg_rate_with_spread(self, rates, dcf_vals):
+    def grad_s_sT_Pbase(self, npv, grad_s_sT_P, f):
         """
-        Calculate all in rate with float spread under averaging.
+        2d array of derivatives of base currency PV with respect to calibrating
+        instrument rate variables, of size (pre_m, pre_m).
 
-        Parameters
-        ----------
-        rates : Series
-            The rates which are expected for each daily period.
-        dcf_vals : Series
-            The weightings which are used for each rate in the compounding formula.
+        .. math::
 
-        Returns
-        -------
-        float, Dual, Dual2
-        """
-        dcf_vals = dcf_vals.set_axis(rates.index)
-        if self.spread_compound_method != "none_simple":
-            raise ValueError(
-                "`spread_compound` method must be 'none_simple' in an RFR averaging " "period."
-            )
-        else:
-            return (dcf_vals * rates).sum() / dcf_vals.sum() + self.float_spread / 100
+           \\nabla_\\mathbf{s} \\nabla_\\mathbf{s}^\\mathbf{T} P^{bas}(\\mathbf{v(s, f), f})
 
-    def _isda_compounded_rate_with_spread(self, rates, dcf_vals):
-        """
-        Calculate all in rates with float spread under different compounding methods.
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            grad_s_sT_P : ndarray
+                The local currency gamma risks w.r.t. calibrating instrument variables.
+            f : Dual or Dual2
+                The local:base FX rate.
+        """
+        grad_s_f = self.grad_s_f_pre(f)
+        grad_s_sT_f = self.grad_s_sT_f_pre(f)
+        grad_s_P = self.grad_s_Ploc(npv)
+
+        _ = float(f) * grad_s_sT_P
+        _ += np.tensordot(grad_s_f[:, None], grad_s_P[None, :], (1, 0))
+        _ += np.tensordot(grad_s_P[:, None], grad_s_f[None, :], (1, 0))
+        _ += float(npv) * grad_s_sT_f  # <- use float to cast float array not Dual
 
-        Parameters
-        ----------
-        rates : Series
-            The rates which are expected for each daily period.
-        dcf_vals : Series
-            The weightings which are used for each rate in the compounding formula.
+        grad_s_sT_Pbas = _
+        return grad_s_sT_Pbas
 
-        Returns
-        -------
-        float, Dual, Dual2
+    def grad_f_sT_Pbase(self, npv, grad_f_sT_P, f, fx_vars):
         """
-        dcf_vals = dcf_vals.set_axis(rates.index)
-        if self.float_spread == 0 or self.spread_compound_method == "none_simple":
-            return (
-                (1 + dcf_vals * rates / 100).prod() - 1
-            ) * 100 / dcf_vals.sum() + self.float_spread / 100
-        elif self.spread_compound_method == "isda_compounding":
-            return (
-                ((1 + dcf_vals * (rates / 100 + self.float_spread / 10000)).prod() - 1)
-                * 100
-                / dcf_vals.sum()
-            )
-        elif self.spread_compound_method == "isda_flat_compounding":
-            sub_cashflows = (rates / 100 + self.float_spread / 10000) * dcf_vals
-            C_i = 0.0
-            for i in range(1, len(sub_cashflows)):
-                C_i += sub_cashflows.iloc[i - 1]
-                sub_cashflows.iloc[i] += C_i * rates.iloc[i] / 100 * dcf_vals.iloc[i]
-            total_cashflow = sub_cashflows.sum()
-            return total_cashflow * 100 / dcf_vals.sum()
-        else:
-            # this path not generally hit due to validation at initialisation
-            raise ValueError(
-                "`spread_compound_method` must be in {'none_simple', "
-                "'isda_compounding', 'isda_flat_compounding'}."
-            )
+        2d array of derivatives of base currency PV with respect to FX variables and
+        calibrating instrument rate variables, of size (len(fx_vars), pre_m).
 
-    def fixings_table(
-        self,
-        curve: Union[Curve, LineCurve, dict],
-        approximate: bool = False,
-        disc_curve: Curve = NoInput(0),
-    ):
-        """
-        Return a DataFrame of fixing exposures.
+        .. math::
 
-        Parameters
-        ----------
-        curve : Curve, LineCurve, IndexCurve dict of such
-            The forecast needed to calculate rates which affect compounding and
-            dependent notional exposure.
-        approximate : bool, optional
-            Perform a calculation that is broadly 10x faster but potentially loses
-            precision upto 0.1%.
-        disc_curve : Curve
-            A curve to make appropriate DF scalings. If *None* and ``curve`` contains
-            DFs that will be used instead, otherwise errors are raised.
+           \\nabla_\\mathbf{f} \\nabla_\\mathbf{s}^\\mathbf{T} P^{bas}(\\mathbf{v(s, f), f})
 
-        Returns
-        -------
-        DataFrame
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            grad_f_sT_P : ndarray
+                The local currency gamma risks w.r.t. FX rate variables and
+                calibrating instrument variables.
+            f : Dual or Dual2
+                The local:base FX rate.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        grad_s_f = self.grad_s_f_pre(f)
+        grad_f_f = self.grad_f_f(f, fx_vars)
+        grad_s_P = self.grad_s_Ploc(npv)
+        grad_f_P = self.grad_f_Ploc(npv, fx_vars)
+        grad_f_sT_f = self.grad_f_sT_f_pre(f, fx_vars)
+
+        _ = float(f) * grad_f_sT_P
+        _ += np.tensordot(grad_f_f[:, None], grad_s_P[None, :], (1, 0))
+        _ += np.tensordot(grad_f_P[:, None], grad_s_f[None, :], (1, 0))
+        _ += float(npv) * grad_f_sT_f  # <- use float to cast float array not Dual
 
-        Notes
-        -----
-        **IBOR** and **RFR** ``fixing_method`` have different representations under
-        this method.
+        grad_s_sT_Pbas = _
+        return grad_s_sT_Pbas
 
-        For *"ibor"* based floating rates the fixing exposures are indexed by
-        **publication date** and not by reference value date. IBOR fixings tend to
-        occur either in advance, or the same day.
-
-        For *"rfr"* based floating rates the fixing exposures are indexed by the
-        **reference value date** and not by publication date. RFR fixings tend to
-        publish in arrears, usually at 9am the following business day. Central banks
-        tend to publish data aligning the fixing rate with the reference value date
-        and not by the publication date which is why this format is chosen. It also
-        has practical application when constructing curves.
+    def grad_f_fT_Pbase(self, npv, grad_f_fT_P, f, fx_vars):
+        """
+        2d array of derivatives of base currency PV with respect to calibrating
+        instrument rate variables, of size (pre_m, pre_m).
 
-        Examples
-        --------
-        .. ipython:: python
+        .. math::
 
-           rfr_curve = Curve(
-               nodes={dt(2022, 1, 1): 1.00, dt(2022, 1, 13): 0.9995},
-               calendar="bus"
-           )
+           \\nabla_\\mathbf{s} \\nabla_\\mathbf{s}^\\mathbf{T} P^{bas}(\\mathbf{v(s, f), f})
 
-        A regular `rfr_payment_delay` period.
+        Parameters:
+            npv : Dual or Dual2
+                A local currency NPV of a period of a leg.
+            grad_f_fT_P : ndarray
+                The local currency gamma risks w.r.t. FX rate variables.
+            f : Dual or Dual2
+                The local:base FX rate.
+            fx_vars : list or tuple of str
+                The variable tags for automatic differentiation of FX rate sensitivity
+        """
+        # grad_s_f = self.grad_s_f_pre(f)
+        grad_f_f = self.grad_f_f(f, fx_vars)
+        # grad_s_P = self.grad_s_Ploc(npv)
+        grad_f_P = self.grad_f_Ploc(npv, fx_vars)
+        grad_f_fT_f = self.grad_f_fT_f_pre(f, fx_vars)
+
+        _ = float(f) * grad_f_fT_P
+        _ += np.tensordot(grad_f_f[:, None], grad_f_P[None, :], (1, 0))
+        _ += np.tensordot(grad_f_P[:, None], grad_f_f[None, :], (1, 0))
+        _ += float(npv) * grad_f_fT_f  # <- use float to cast float array not Dual
 
-        .. ipython:: python
+        grad_s_sT_Pbas = _
+        return grad_s_sT_Pbas
 
-           constants = {
-               "start": dt(2022, 1, 5),
-               "end": dt(2022, 1, 11),
-               "payment": dt(2022, 1, 11),
-               "frequency": "Q",
-               "notional": -1000000,
-               "currency": "gbp",
-           }
-           period = FloatPeriod(**{
-               **constants,
-               "fixing_method": "rfr_payment_delay"
-           })
-           period.fixings_table(rfr_curve)
-
-        A 2 business day `rfr_observation_shift` period. Notice how the above had
-        4 fixings spanning 6 calendar days, but the observation shift here attributes
-        4 fixings spanning 4 calendar days so the notional exposure to those dates
-        is increased by effectively 6/4.
 
-        .. ipython:: python
+class Solver(Gradients):
+    """
+    A numerical solver to determine node values on multiple curves simultaneously.
 
-           period = FloatPeriod(**{
-               **constants,
-               "fixing_method": "rfr_observation_shift",
-               "method_param": 2,
-            })
-           period.fixings_table(rfr_curve)
-
-        A 2 business day `rfr_lookback` period. Notice how the lookback period adjusts
-        the weightings on the 6th January fixing by 3, and thus increases the notional
-        exposure.
+    Parameters
+    ----------
+    curves : sequence
+        Sequence of :class:`Curve` or :class:`FXDeltaVolSmile` objects where each *curve*
+        has been individually configured for its node dates and interpolation structures,
+        and has a unique ``id``. Each *curve* will be dynamically updated by the Solver.
+    surfaces : sequence
+        Sequence of :class:`FXDeltaVolSurface` objects where each *surface* has been configured
+        with a unique ``id``. Each *surface* will be dynamically updated. *Surfaces* are appended
+        to ``curves`` and just provide a distinct keyword for organisational distinction.
+    instruments : sequence
+        Sequence of calibrating instrument specifications that will be used by
+        the solver to determine the solved curves. See notes.
+    s : sequence
+        Sequence of objective rates that each solved calibrating instrument will solve
+        to. Must have the same length and order as ``instruments``.
+    weights : sequence, optional
+        The weights that should be used within the objective function when determining
+        the loss function associated with each calibrating instrument. Should be of
+        same length as ``instruments``. If not given defaults to all ones.
+    algorithm : str in {"levenberg_marquardt", "gauss_newton", "gradient_descent"}
+        The optimisation algorithm to use when solving curves via :meth:`iterate`.
+    fx : FXForwards, optional
+        The ``FXForwards`` object used in FX rate calculations for ``instruments``.
+    instrument_labels : list of str, optional
+        The names of the calibrating instruments which will be used in delta risk
+        outputs.
+    id : str, optional
+        The identifier used to denote the instance and attribute risk factors.
+    pre_solvers : list,
+        A collection of ``Solver`` s that have already determined curves to which this
+        instance has a dependency. Used for aggregation of risk sensitivities.
+    max_iter : int
+        The maximum number of iterations to perform.
+    func_tol : float
+        The tolerance to determine convergence if the objective function is lower
+        than a specific value. Defaults to 1e-12.
+    conv_tol : float
+        The tolerance to determine convergence if successive objective function
+        values are similar. Defaults to 1e-17.
+    ini_lambda : 3-tuple of float, optional
+        Parameters to control the Levenberg-Marquardt algorithm, defined as the
+        initial lambda value, the scaling factor for a successful iteration and the
+        scaling factor for an unsuccessful iteration. Defaults to (1000, 0.25, 2).
+    callback : callable, optional
+        Is called after each iteration. Used for debugging or optimisation.
 
-        .. ipython:: python
+    Notes
+    -----
+    Once initialised the ``Solver`` will numerically determine and set all of the
+    relevant DF node values on each *Curve* simultaneously by calling :meth:`iterate`.
 
-           period = FloatPeriod(**{
-               **constants,
-               "fixing_method": "rfr_lookback",
-               "method_param": 2,
-            })
-           period.fixings_table(rfr_curve)
+    Each instrument provided to ``instruments`` must have its ``curves`` and ``metric``
+    preset at initialisation, and can then be used directly (as shown in some examples).
 
-        A 2 business day `rfr_lockout` period. Notice how the exposure to the final
-        fixing which then spans multiple days is increased.
+    If the *Curves* and/or *metric* are not preset then the *Solver* ``instruments`` can be
+    given as a tuple where the second and third items are a tuple and dict representing positional
+    and keyword arguments passed to the *instrument's*
+    :meth:`~rateslib.instruments.FixedRateBond.rate`` method. Usually using the keyword arguments
+    is more explicit. An example is:
 
-        .. ipython:: python
+    - (FixedRateBond([args]), (), {"curves": bond_curve, "metric": "ytm"}),
 
-           period = FloatPeriod(**{
-               **constants,
-               "fixing_method": "rfr_lockout",
-               "method_param": 2,
-            })
-           period.fixings_table(rfr_curve)
+    Examples
+    --------
 
-        An IBOR fixing table
+    See the documentation user guide :ref:`here <c-solver-doc>`.
 
-        .. ipython:: python
+    Attributes
+    ----------
+    curves : dict
+    instruments : sequence
+    weights : sequence
+    s : sequence
+    algorithm : str
+    fx : FXForwards
+    id : str
+    tol : float
+    max_iter : int
+    n : int
+        The total number of curve variables to solve for.
+    m : int
+        The total number of calibrating instruments provided to the Solver.
+    W : 2d array
+        A diagonal array constructed from ``weights``.
+    variables : list[str]
+        List of variable name tags used in extracting derivatives automatically.
+    instrument_labels : list[str]
+        List of calibrating instrument names for delta risk visualization.
+    pre_solvers : list
+    pre_variables : list[str]
+        List of variable name tags used in extracting derivatives automatically.
+    pre_m : int
+        The total number of calibrating instruments provided to the Solver including
+        those in pre-solvers
+    pre_n : int
+        The total number of curve variables solved for, including those in pre-solvers.
+    """
 
-            ibor_curve = Curve(
-               nodes={dt(2022, 1, 1): 1.00, dt(2023, 1, 1): 0.99},
-               calendar="bus",
-           )
-           period = FloatPeriod(**{
-               **constants,
-               "fixing_method": "ibor",
-               "method_param": 2,
-            })
-           period.fixings_table(ibor_curve)
-        """
-        if disc_curve is NoInput.blank and isinstance(curve, dict):
-            raise ValueError("Cannot infer `disc_curve` from a dict of curves.")
-        elif disc_curve is NoInput.blank and curve._base_type == "dfs":
-            disc_curve = curve
+    _grad_s_vT_method = "_grad_s_vT_final_iteration_analytical"
+    _grad_s_vT_final_iteration_algo = "gauss_newton_final"
 
-        if approximate:
-            if self.fixings is not NoInput.blank:
-                warnings.warn(
-                    "Cannot approximate a fixings table when some published fixings "
-                    f"are given within the period {self.start.strftime('%d-%b-%Y')}->"
-                    f"{self.end.strftime('%d-%b-%Y')}. Switching to exact mode for this "
-                    f"period.",
-                    UserWarning,
-                )
-            else:
-                return self._fixings_table_fast(curve, disc_curve)
+    def __init__(
+        self,
+        curves: Union[list, tuple] = (),
+        surfaces: Union[list, tuple] = (),
+        instruments: Union[tuple[tuple], list[tuple]] = (),
+        s: list[float] = [],
+        weights: Optional[list] = NoInput(0),
+        algorithm: Optional[str] = NoInput(0),
+        fx: Union[FXForwards, FXRates, NoInput] = NoInput(0),
+        instrument_labels: Optional[tuple[str], list[str]] = NoInput(0),
+        id: Optional[str] = NoInput(0),
+        pre_solvers: Union[tuple[Solver], list[Solver]] = (),
+        max_iter: int = 100,
+        func_tol: float = 1e-11,
+        conv_tol: float = 1e-14,
+        ini_lambda: Union[tuple[float, float, float], NoInput] = NoInput(0),
+        callback: Union[Callable, NoInput] = NoInput(0),
+    ) -> None:
+        self.callback = callback
+        self.algorithm = defaults.algorithm if algorithm is NoInput.blank else algorithm
+        if ini_lambda is NoInput.blank:
+            self.ini_lambda = defaults.ini_lambda
+        else:
+            self.ini_lambda = ini_lambda
+        self.m = len(instruments)
+        self.func_tol, self.conv_tol, self.max_iter = func_tol, conv_tol, max_iter
+        self.id = uuid4().hex[:5] + "_" if id is NoInput.blank else id  # 1 in a million clash
+        self.pre_solvers = tuple(pre_solvers)
 
-        if "rfr" in self.fixing_method:
-            rate, table = self._rfr_fixings_array(
-                curve,
-                fixing_exposure=True,
-                disc_curve=disc_curve,
+        # validate `id`s so that DataFrame indexing does not share duplicated keys.
+        if len(set([self.id] + [p.id for p in self.pre_solvers])) < 1 + len(self.pre_solvers):
+            raise ValueError(
+                "Solver `id`s must be unique when supplying `pre_solvers`, "
+                f"got ids: {[self.id] + [p.id for p in self.pre_solvers]}"
             )
-            table = table.iloc[:-1]
-            return table[["obs_dates", "notional", "dcf", "rates"]].set_index("obs_dates")
-        elif "ibor" in self.fixing_method:
-            if isinstance(curve, dict):
-                calendar = next(iter(curve.values())).calendar
+
+        # validate `s` and `instruments` with a naive length comparison
+        if len(s) != len(instruments):
+            raise ValueError("`instrument_rates` must be same length as `instruments`.")
+        self.s = np.asarray(s)
+
+        # validate `instrument_labels` if given is same length as `m`
+        if instrument_labels is not NoInput.blank:
+            if self.m != len(instrument_labels):
+                raise ValueError("`instrument_labels` must have length `instruments`.")
             else:
-                calendar = curve.calendar
-            fixing_date = add_tenor(self.start, f"-{self.method_param}b", "P", calendar)
-            return DataFrame(
-                {
-                    "obs_dates": [fixing_date],
-                    "notional": -self.notional,
-                    "dcf": [None],
-                    "rates": [self.rate(curve)],
-                }
-            ).set_index("obs_dates")
+                self.instrument_labels = tuple(instrument_labels)
+        else:
+            self.instrument_labels = tuple(f"{self.id}{i}" for i in range(self.m))
 
-    def _rfr_fixings_array(
-        self,
-        curve: Union[Curve, LineCurve],
-        fixing_exposure: bool = False,
-        disc_curve: Curve = None,
-    ):
-        """
-        Calculate the rate of a period via extraction and combination of every fixing.
+        if weights is NoInput.blank:
+            self.weights = np.ones(len(instruments))
+        else:
+            if len(weights) != self.m:
+                raise ValueError("`weights` must be same length as `instruments`.")
+            self.weights = np.asarray(weights)
+        self.W = np.diag(self.weights)
+
+        # `surfaces` are treated identically to `curves`. Introduced in PR
+        self.curves = {
+            curve.id: curve
+            for curve in list(curves) + list(surfaces)
+            if not type(curve) in [ProxyCurve, CompositeCurve, MultiCsaCurve]
+            # Proxy and Composite curves have no parameters of their own
+        }
+        self.variables = ()
+        for curve in self.curves.values():
+            curve._set_ad_order(1)  # solver uses gradients in optimisation
+            self.variables += curve._get_node_vars()
+        self.n = len(self.variables)
+
+        # aggregate and organise variables and labels including pre_solvers
+        self.pre_curves = {}
+        self.pre_variables = ()
+        self.pre_instrument_labels = ()
+        self.pre_instruments = ()
+        self.pre_rate_scalars = []
+        self.pre_m, self.pre_n = self.m, self.n
+        curve_collection = []
+        for pre_solver in self.pre_solvers:
+            self.pre_variables += pre_solver.pre_variables
+            self.pre_instrument_labels += pre_solver.pre_instrument_labels
+            self.pre_instruments += pre_solver.pre_instruments
+            self.pre_rate_scalars.extend(pre_solver.pre_rate_scalars)
+            self.pre_m += pre_solver.pre_m
+            self.pre_n += pre_solver.pre_n
+            self.pre_curves.update(pre_solver.pre_curves)
+            curve_collection.extend(pre_solver.pre_curves.values())
+        self.pre_curves.update(self.curves)
+        self.pre_curves.update(
+            {
+                curve.id: curve
+                for curve in curves
+                if type(curve) in [ProxyCurve, CompositeCurve, MultiCsaCurve]
+                # Proxy and Composite curves added to the collection without variables
+            }
+        )
+        curve_collection.extend(curves)
+        for curve1, curve2 in combinations(curve_collection, 2):
+            if curve1.id == curve2.id:
+                raise ValueError(
+                    "`curves` must each have their own unique `id`. If using "
+                    "pre-solvers as part of a dependency chain a curve can only be "
+                    "specified as a variable in one solver."
+                )
+        self.pre_variables += self.variables
+        self.pre_instrument_labels += tuple((self.id, lbl) for lbl in self.instrument_labels)
 
-        This method of calculation is inefficient and used when either:
+        # Final elements
+        self._ad = 1
+        self.fx = fx
+        self.instruments = tuple((self._parse_instrument(inst) for inst in instruments))
+        self.pre_instruments += self.instruments
+        self.rate_scalars = tuple((inst[0]._rate_scalar for inst in self.instruments))
+        self.pre_rate_scalars += self.rate_scalars
+
+        # TODO need to check curves associated with fx object and set order.
+        # self._reset_properties_()  performed in iterate
+        self.result = {
+            "status": "INITIALISED",
+            "state": 0,
+            "g": None,
+            "iterations": 0,
+            "time": None,
+        }
+        self.iterate()
 
-        - known fixings needs to be combined with unknown fixings,
-        - the fixing_method is of a type that needs individual fixing data,
-        - the spread compound method is of a type that needs individual fixing data.
+    def _parse_instrument(self, value):
+        """
+        Parses different input formats for an instrument given to the ``Solver``.
 
         Parameters
         ----------
-        curve : Curve or LineCurve
-            The forecasting curve used to extract the fixing data.
-        fixing_exposure : bool
-            Whether to calculate sensitivities to the fixings additionally.
-        fixing_exposure_approx : bool
-            Whether to use an approximation, if available, for fixing exposure calcs.
+        value : Instrument or 3-tuple.
+            If a 3-tuple then it must have the following items:
+
+            - The ``Instrument``.
+            - Positional args supplied to the ``rate`` method as a tuple, or None.
+            - Keyword args supplied to the ``rate`` method as a dict, or None.
 
         Returns
         -------
-        tuple
-            The compounded rate, DataFrame of the calculation data.
+        tuple :
+            A 3-tuple attaching the self solver and self fx object as pricing params.
 
-        Notes
-        -----
-        ``start_obs`` and ``end_obs`` define the observation period for fixing rates.
-        ``start_dcf`` and ``end_dcf`` define the period for day count fractions.
-        Unless *"lookback"* is used which mis-aligns the obs and dcf periods these
-        will be aligned.
+        Examples
+        --------
+        ``value=Instrument()``
 
-        The ``fixing_exposure_approx`` is available only for ``spread_compound_method``
-        that is either *"none_simple"* or *"isda_compounding"*.
-        """
+        ``value=(Instrument(), (curve, None, fx), {"other_arg": 10.0})``
 
-        obs_dates, dcf_dates = self._get_method_dcf_markers(curve)
+        ``value=(Instrument(), None, {"other_arg": 10.0})``
 
-        dcf_vals = Series(
-            [  # calculate the dcf values from the dcf dates
-                dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
-                for i in range(len(dcf_dates.index) - 1)
-            ]
-        )
+        ``value=(Instrument(), (curve, None, fx), None)``
 
-        rates = Series(NA, index=obs_dates[:-1])
-        if self.fixings is not NoInput.blank:
-            # then fixings will be a list or Series, scalars are already processed.
-            if isinstance(self.fixings, list):
-                rates.iloc[: len(self.fixings)] = self.fixings
-            elif isinstance(self.fixings, Series):
-                if not self.fixings.index.is_monotonic_increasing:
-                    raise ValueError(
-                        "`fixings` as a Series must have a monotonically increasing "
-                        "datetimeindex."
-                    )
-                # [-2] is used because the last rfr fixing is 1 day before the end
-                fixing_rates = self.fixings.loc[obs_dates.iloc[0] : obs_dates.iloc[-2]]  # type: ignore[misc]
+        ``value=(Instrument(), (curve,), {})``
+        """
+        if not isinstance(value, tuple):
+            # is a direct Instrument so convert to tuple with pricing params
+            return (value, tuple(), {"solver": self, "fx": self.fx})
+        else:
+            # object is tuple
+            if len(value) != 3:
+                raise ValueError(
+                    "`Instrument` supplied to `Solver` as tuple must be a 3-tuple of "
+                    "signature: (Instrument, positional args[tuple], keyword "
+                    "args[dict])."
+                )
+            ret0, ret1, ret2 = value[0], tuple(), {"solver": self, "fx": self.fx}
+            if not (value[1] is None or value[1] == ()):
+                ret1 = value[1]
+            if not (value[2] is None or value[2] == {}):
+                ret2 = {**ret2, **value[2]}
+            return (ret0, ret1, ret2)
 
-                try:
-                    rates.loc[fixing_rates.index] = fixing_rates
-                except KeyError as e:
-                    raise ValueError(
-                        "The supplied `fixings` contain more fixings than were "
-                        "expected by the holiday calendar of the `curve`.\nThe "
-                        "additional fixing dates are shown in the underlying "
-                        "KeyError message below.\nIf the Series you are providing "
-                        "contains valid fixings the fault probably lies with "
-                        "Rateslib calendar definitions and should be reported.\n"
-                        "This error can avoided by excluding these fixings using "
-                        f"Series.pop().\n{e}"
-                    )
+    def _reset_properties_(self, dual2_only=False):
+        """
+        Set all calculated attributes to `None` requiring re-evaluation.
 
-                # basic error checking for missing fixings and provide warning.
-                try:
-                    first_forecast_date = rates[isna(rates)].index[0]
-                    if rates[~isna(rates)].index[-1] > first_forecast_date:
-                        # then a missing fixing exists
-                        warnings.warn(
-                            f"`fixings` has missed a calendar value "
-                            f"({first_forecast_date}) which "
-                            "has been inferred from the curve. Subsequent "
-                            "fixings have been detected",
-                            UserWarning,
-                        )
-                except (KeyError, IndexError):
-                    pass
-            else:
-                raise TypeError(
-                    "`fixings` should be of type scalar, None, list or Series."
-                )  # pragma: no cover
-
-        # reindex the rates series getting missing values from the curves
-        # TODO (low) the next two lines could probably be vectorised and made more efficient.
-        fixed = ~isna(rates)
-        rates = Series({k: v if notna(v) else curve.rate(k, "1b", "F") for k, v in rates.items()})
-
-        if fixing_exposure:
-            # need to calculate the dcfs associated with the rates (unshifted)
-            if self.fixing_method in [
-                "rfr_payment_delay",
-                "rfr_observation_shift",
-                "rfr_lockout",
-                "rfr_payment_delay_avg",
-                "rfr_observation_shift_avg",
-                "rfr_lockout_avg",
-            ]:  # for all these methods there is no shift
-                dcf_of_r = dcf_vals.copy()
-            elif self.fixing_method in ["rfr_lookback", "rfr_lookback_avg"]:
-                dcf_of_r = Series(
-                    [
-                        dcf(obs_dates[i], obs_dates[i + 1], curve.convention)
-                        for i in range(len(dcf_dates.index) - 1)
-                    ]
-                )
-            v_with_r = Series([disc_curve[obs_dates[i]] for i in range(1, len(dcf_dates.index))])
+        Parameters
+        ----------
+        dual2_only : bool
+            Choose whether to reset properties only for the calculation of the
+            properties whose derivation **requires** Dual2 datatypes. Since the
+            ``Solver`` iterates ``Curve`` s by default it necessarily uses Dual
+            datatypes and first order derivatives. For the calculation of:
+
+              - ``J2`` and ``J2_pre``:
+                :math:`\frac{\\partial^2 r_i}{\\partial v_j \\partial v_k}`
+              - ``grad_s_s_vT`` and ``grad_s_s_vT_pre``:
+                :math:`\frac{\\partial^2 v_i}{\\partial s_j \\partial s_k}`
 
-        if self.fixing_method in ["rfr_lockout", "rfr_lockout_avg"]:
-            # adjust the final rates values of the lockout arrays according to param
-            try:
-                rates.iloc[-self.method_param :] = rates.iloc[-self.method_param - 1]
-            except IndexError:
-                raise ValueError("period has too few dates for `rfr_lockout` param to function.")
-
-        if fixing_exposure:
-            rates_dual = Series(
-                [Dual(float(r), [f"fixing_{i}"], []) for i, (k, r) in enumerate(rates.items())],
-                index=rates.index,
-            )
-            if self.fixing_method in ["rfr_lockout", "rfr_lockout_avg"]:
-                rates_dual.iloc[-self.method_param :] = rates_dual.iloc[-self.method_param - 1]
-            if "avg" in self.fixing_method:
-                rate = self._avg_rate_with_spread(rates_dual, dcf_vals)
-            else:
-                rate = self._isda_compounded_rate_with_spread(rates_dual, dcf_vals)
-            notional_exposure = Series(
-                [gradient(rate, [f"fixing_{i}"])[0] for i in range(len(dcf_dates.index) - 1)]
-            ).astype(float)
-            v = disc_curve[self.payment]
-            mask = ~fixed.to_numpy()  # exclude fixings that are already fixed
-
-            notional_exposure[mask] *= -self.notional * (self.dcf / dcf_of_r[mask]) * float(v)
-            notional_exposure[mask] /= v_with_r[mask].astype(float)
-            # notional_exposure[mask] *= (-self.notional * (self.dcf / dcf_of_r[mask]) * v / v_with_r[mask])
-            # notional_exposure[fixed.drop_index(drop=True)] = 0.0
-            notional_exposure[fixed.to_numpy()] = 0.0
-            extra_cols = {
-                "obs_dcf": dcf_of_r,
-                "notional": notional_exposure.astype(float),  # apply(float, convert_dtype=float),
-            }
-        else:
-            if "avg" in self.fixing_method:
-                rate = self._avg_rate_with_spread(rates, dcf_vals)
-            else:
-                rate = self._isda_compounded_rate_with_spread(rates, dcf_vals)
-            extra_cols = {}
+        Returns
+        -------
+        None
+        """
+        if not dual2_only:
+            self._v = None  # depends on self.curves
+            self._r = None  # depends on self.pre_curves and self.instruments
+            self._r_pre = None  # depends on pre_solvers and self.r
+            self._x = None  # depends on self.r, self.s
+            self._g = None  # depends on self.x, self.weights
+            self._J = None  # depends on self.r
+            self._grad_s_vT = None  # final_iter_dual: depends on self.s and iteration
+            # fixed_point_iter: depends on self.f
+            # final_iter_anal: depends on self.J
+            self._grad_s_vT_pre = None  # depends on self.grad_s_vT and pre_solvers.
+
+        self._J2 = None  # defines its own self.r under dual2
+        self._J2_pre = None  # depends on self.r and pre_solvers
+        self._grad_s_s_vT = None  # final_iter: depends on self.J2 and self.grad_s_vT
+        # finite_diff: TODO update comment
+        self._grad_s_s_vT_pre = None  # final_iter: depends on pre versions of above
+        # finite_diff: TODO update comment
 
-        if rates.isna().any():
-            raise ValueError(
-                "RFRs could not be calculated, have you missed providing `fixings` or "
-                "does the `Curve` begin after the start of a `FloatPeriod` including"
-                "the `method_param` adjustment?"
-            )
+        # self._grad_v_v_f = None
+        # self._Jkm = None  # keep manifold originally used for exploring J2 calc method
 
-        return rate, DataFrame(
-            {
-                "obs_dates": obs_dates,
-                "dcf_dates": dcf_dates,
-                "dcf": dcf_vals,
-                "rates": rates.astype(float).reset_index(drop=True),
-                **extra_cols,
-            }
-        )
+    @property
+    def v(self):
+        """
+        1d array of curve node variables for each ordered curve, size (n,).
 
-    def _fixings_table_fast(self, curve: Union[Curve, LineCurve], disc_curve: Curve):
+        Depends on ``self.curves``.
         """
-        Return a DataFrame of **approximate** fixing exposures.
+        if self._v is None:
+            self._v = np.block([_._get_node_vector() for _ in self.curves.values()])
+        return self._v
 
-        For arguments see :meth:`~rateslib.periods.FloatPeriod.fixings_table`.
+    @property
+    def r(self):
         """
-        if "rfr" in self.fixing_method:
-            # Depending upon method get the observation dates and dcf dates
-            obs_dates, dcf_dates = self._get_method_dcf_markers(curve)
+        1d array of mid-market rates of each calibrating instrument with given curves,
+        size (m,).
 
-            # TODO (low) this calculation could be vectorised by a 360 or 365 multiplier
-            dcf_vals = Series(
-                [  # calculate the dcf values from the dcf dates
-                    dcf(dcf_dates[i], dcf_dates[i + 1], curve.convention)
-                    for i in range(len(dcf_dates.index) - 1)
-                ]
-            )
-            obs_vals = Series(
-                [  # calculate the dcf values from the dcf dates
-                    dcf(obs_dates[i], obs_dates[i + 1], curve.convention)
-                    for i in range(len(obs_dates.index) - 1)
-                ]
-            )
+        Depends on ``self.pre_curves`` and ``self.instruments``.
+        """
+        if self._r is None:
+            self._r = np.array([_[0].rate(*_[1], **_[2]) for _ in self.instruments])
+            # solver and fx are passed by default via parse_args to get string curves
+        return self._r
 
-            # approximate DFs
-            v_vals = Series(np.nan, index=obs_dates.iloc[1:])
-            v_vals.iloc[0] = log(float(disc_curve[obs_dates.iloc[1]]))
-            v_vals.iloc[-1] = log(float(disc_curve[obs_dates.iloc[-1]]))
-            v_vals = v_vals.interpolate(method="time")
-            v_vals = Series(np.exp(v_vals.to_numpy()), index=obs_vals.index)
-
-            scalar = dcf_vals.values / obs_vals.values
-            if self.fixing_method in ["rfr_lockout", "rfr_lockout_avg"]:
-                scalar[-self.method_param :] = 0.0
-                scalar[-(self.method_param + 1)] = (
-                    obs_vals.iloc[-(self.method_param + 1) :].sum()
-                    / obs_vals.iloc[-(self.method_param + 1)]
-                )
-            # perform an efficient rate approximation
-            rate = curve.rate(
-                effective=obs_dates.iloc[0],
-                termination=obs_dates.iloc[-1],
-            )
-            r_bar, d, n = average_rate(
-                obs_dates.iloc[0], obs_dates.iloc[-1], curve.convention, rate
-            )
-            # approximate sensitivity to each fixing
-            z = self.float_spread / 10000
-            if "avg" in self.fixing_method:
-                drdri = 1 / n
-            elif self.spread_compound_method == "none_simple":
-                drdri = (1 / n) * (1 + (r_bar / 100) * d) ** (n - 1)
-            elif self.spread_compound_method == "isda_compounding":
-                drdri = (1 / n) * (1 + (r_bar / 100 + z) * d) ** (n - 1)
-            elif self.spread_compound_method == "isda_flat_compounding":
-                dr = d * r_bar / 100
-                drdri = (1 / n) * (
-                    ((1 / n) * (comb(n, 1) + comb(n, 2) * dr + comb(n, 3) * dr**2))
-                    + ((r_bar / 100 + z) / n) * (comb(n, 2) * d + 2 * comb(n, 3) * dr * d)
-                )
+    @property
+    def r_pre(self):
+        if len(self.pre_solvers) == 0:
+            return self.r
+
+        if self._r_pre is None:
+            r_pre = np.empty(self.pre_m, dtype="object")
+
+            i = 0
+            for pre_solver in self.pre_solvers:
+                m = pre_solver.pre_m
+                r_pre[i : i + m] = pre_solver.r_pre
+                i = i + m
+
+            # create bottom right block
+            r_pre[-self.m :] = self.r
+            self._r_pre = r_pre
+        return self._r_pre
 
-            v = float(disc_curve[self.payment])
-            v_vals /= v
-            notional_exposure = Series(
-                (-self.notional * self.dcf * float(drdri) / d * scalar) / v_vals,
-                index=obs_vals.index,
-            )
+    @property
+    def x(self):
+        """
+        1d array of error in each calibrating instrument rate, of size (m,).
 
-            table = DataFrame(
-                {
-                    "obs_dates": obs_dates,
-                    "obs_dcf": obs_vals,
-                    "dcf_dates": dcf_dates,
-                    "dcf": dcf_vals,
-                    "notional": notional_exposure,
-                    "rates": Series(rate, index=obs_dates.index).astype(
-                        float
-                    ),  # .apply(float, convert_dtype=float),
-                }
-            )
+        .. math::
 
-            table = table.iloc[:-1]
-            return table[["obs_dates", "notional", "dcf", "rates"]].set_index("obs_dates")
-        elif "ibor" in self.fixing_method:
-            fixing_date = add_tenor(self.start, f"-{self.method_param}b", "P", curve.calendar)
-            return DataFrame(
-                {
-                    "obs_dates": [fixing_date],
-                    "notional": -self.notional,
-                    "dcf": [None],
-                    "rates": [self.rate(curve)],
-                }
-            ).set_index("obs_dates")
+           \\mathbf{x} = \\mathbf{r-S}
 
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-    # Commercial use of this code, and/or copying and redistribution is prohibited.
-    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+        Depends on ``self.r`` and ``self.s``.
+        """
+        if self._x is None:
+            self._x = self.r - self.s
+        return self._x
 
     @property
-    def _is_inefficient(self):
+    def error(self):
         """
-        An inefficient float period is one which is RFR based and for which each individual
-        RFR fixing is required is order to calculate correctly. This occurs in the
-        following cases:
-
-        1) The ``fixing_method`` is lookback - since fixing have arbitrary weightings
-           misaligned with their standard weightings due to arbitrary shifts.
-        2) The ``spread_compound_method`` is not *"none_simple"* - this is because the
-           float spread is compounded alongside the rates so there is a non-linear
-           relationship. Note if spread is zero this is negated and can be ignored.
-        3) The ``fixing_method`` is lockout - technically this could be made semi
-           efficient by splitting calculations into two parts. As of now it
-           remains within the inefficient section.
-        4) ``fixings`` are given which need to be incorporated into the calculation
-        """
-        if self.fixing_method in ["rfr_payment_delay", "rfr_observation_shift"]:
-            if self.fixings is not NoInput.blank:
-                return True
-            elif self.float_spread == 0 or self.spread_compound_method == "none_simple":
-                return False
+        Return the error in calibrating instruments, including ``pre_solvers``, scaled
+        to the risk representation factor.
+
+        Returns
+        -------
+        Series
+        """
+        s = None
+        for pre_solver in self.pre_solvers:
+            if s is None:
+                s = pre_solver.error
             else:
-                return True
-        elif self.fixing_method == "ibor":
-            return False
-        # else fixing method in ["rfr_lookback", "rfr_lockout"]
-        return True
-
-    def _get_method_dcf_markers(self, curve: Union[Curve, LineCurve], endpoints=False):
-        # Depending upon method get the observation dates and dcf dates
-        if self.fixing_method in [
-            "rfr_payment_delay",
-            "rfr_lockout",
-            "rfr_payment_delay_avg",
-            "rfr_lockout_avg",
-        ]:
-            start_obs, end_obs = self.start, self.end
-            start_dcf, end_dcf = self.start, self.end
-        elif self.fixing_method in [
-            "rfr_observation_shift",
-            "rfr_observation_shift_avg",
-        ]:
-            start_obs = add_tenor(self.start, f"-{self.method_param}b", "P", curve.calendar)
-            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
-            start_dcf, end_dcf = start_obs, end_obs
-        elif self.fixing_method in ["rfr_lookback", "rfr_lookback_avg"]:
-            start_obs = add_tenor(self.start, f"-{self.method_param}b", "P", curve.calendar)
-            end_obs = add_tenor(self.end, f"-{self.method_param}b", "P", curve.calendar)
-            start_dcf, end_dcf = self.start, self.end
+                s = concat([pre_solver.error, s])
+
+        _ = Series(
+            self.x.astype(float) * 100 / self.rate_scalars,
+            index=MultiIndex.from_tuples([(self.id, inst) for inst in self.instrument_labels]),
+        )
+        if s is None:
+            s = _
         else:
-            raise NotImplementedError(
-                "`fixing_method` should be in {'rfr_payment_delay', 'rfr_lockout', "
-                "'rfr_lookback', 'rfr_observation_shift'} or the same with '_avg' as "
-                "a suffix for averaging methods."
-            )
+            s = concat([s, _])
+        return s
 
-        if endpoints:
-            # return just the edges without the computation of creating Series
-            return start_obs, end_obs, start_dcf, end_dcf
-
-        # dates of the fixing observation period
-        obs_dates = Series(date_range(start=start_obs, end=end_obs, freq=curve.calendar))
-        # dates for the dcf weight for each observation towards the calculation
-        dcf_dates = Series(date_range(start=start_dcf, end=end_dcf, freq=curve.calendar))
-        if len(dcf_dates) != len(obs_dates):
-            # this might only be true with lookback when obs dates are adjusted
-            # but DCF dates are not, and if starting on holiday causes problems.
-            raise ValueError(
-                "RFR Observation and Accrual DCF dates do not align.\n"
-                "This is usually the result of a 'rfr_lookback' Period which does "
-                "not adhere to the holiday calendar of the `curve`.\n"
-                f"start date: {self.start.strftime('%d-%m-%Y')} is curve holiday? "
-                f"{_is_holiday(self.start, curve.calendar)}\n"
-                f"end date: {self.end.strftime('%d-%m-%Y')} is curve holiday? "
-                f"{_is_holiday(self.end, curve.calendar)}\n"
-            )
+    @property
+    def g(self):
+        """
+        Objective function scalar value of the solver;
+
+        .. math::
 
-        return obs_dates, dcf_dates
+           g = \\mathbf{(r-S)^{T}W(r-S)}
 
-    def _get_analytic_delta_quadratic_coeffs(self, fore_curve, disc_curve):
+        Depends on ``self.x`` and ``self.weights``.
         """
-        For use in the Leg._spread calculation get the 'a' and 'b' coefficients
+        if self._g is None:
+            self._g = np.dot(self.x, self.weights * self.x)
+        return self._g
+
+    # def Jkm(self, extra_vars=[]):
+    #     """
+    #     2d Jacobian array of rates with respect to discount factors, of size (n, m); :math:`[J]_{i,j} = \\frac{\\partial r_j}{\\partial v_i}`.
+    #     """
+    #     _Jkm = np.array([rate.gradient(self.variables + extra_vars, keep_manifold=True) for rate in self.r]).T
+    #     return _Jkm
+
+    def _update_step_(self, algorithm):
+        if algorithm == "gradient_descent":
+            grad_v_g = gradient(self.g, self.variables)
+            y = np.matmul(self.J.transpose(), grad_v_g[:, np.newaxis])[:, 0]
+            alpha = np.dot(y, self.weights * self.x) / np.dot(y, self.weights * y)
+            v_1 = self.v - grad_v_g * alpha.real
+        elif algorithm == "gauss_newton":
+            if self.J.shape[0] == self.J.shape[1]:  # square system
+                A = self.J.transpose()
+                b = -np.array([x.real for x in self.x])[:, np.newaxis]
+            else:
+                A = np.matmul(self.J, np.matmul(self.W, self.J.transpose()))
+                b = -0.5 * gradient(self.g, self.variables)[:, np.newaxis]
+            delta = np.linalg.solve(A, b)[:, 0]
+            v_1 = self.v + delta
+        elif algorithm == "levenberg_marquardt":
+            if self.g_list[-2] < self.g.real:
+                # reject previous iteration and rescale lambda:
+                self.lambd *= self.ini_lambda[2]
+                # self._update_curves_with_parameters(self.v_prev)
+            else:
+                self.lambd *= self.ini_lambda[1]
+            # self.lambd *= self.ini_lambda[2] if self.g_prev < self.g.real else self.ini_lambda[1]
+            A = np.matmul(self.J, np.matmul(self.W, self.J.transpose()))
+            A += self.lambd * np.eye(self.n)
+            b = -0.5 * gradient(self.g, self.variables)[:, np.newaxis]
+            delta = np.linalg.solve(A, b)[:, 0]
+            v_1 = self.v + delta
+        # elif algorithm == "gradient_descent_final":
+        #     _ = np.matmul(self.Jkm, np.matmul(self.W, self.x[:, np.newaxis]))
+        #     y = 2 * np.matmul(self.Jkm.transpose(), _)[:, 0]
+        #     alpha = np.dot(y, self.weights * self.x) / np.dot(y, self.weights * y)
+        #     v_1 = self.v - 2 * alpha * _[:, 0]
+        elif algorithm == "gauss_newton_final":
+            if self.J.shape[0] == self.J.shape[1]:  # square system
+                A = self.J.transpose()
+                b = -self.x[:, np.newaxis]
+            else:
+                A = np.matmul(self.J, np.matmul(self.W, self.J.transpose()))
+                b = -np.matmul(np.matmul(self.J, self.W), self.x[:, np.newaxis])
+
+            delta = dual_solve(A, b)[:, 0]
+            v_1 = self.v + delta
+        else:
+            raise NotImplementedError(f"`algorithm`: {algorithm} (spelled correctly?)")
+        return v_1
+
+    def _update_fx(self):
+        if self.fx is not NoInput.blank:
+            self.fx.update()  # note: with no variables this does nothing.
+
+    def iterate(self):
         """
-        os, oe, _, _ = self._get_method_dcf_markers(fore_curve, True)
-        rate = fore_curve.rate(
-            effective=os,
-            termination=oe,
-            float_spread=0.0,
-            spread_compound_method=self.spread_compound_method,
-        )
-        r, d, n = average_rate(os, oe, fore_curve.convention, rate)
-        # approximate sensitivity to each fixing
-        z = 0.0 if self.float_spread is None else self.float_spread
-        if self.spread_compound_method == "isda_compounding":
-            d2rdz2 = d * (n - 1) * (1 + (r / 100 + z / 10000) * d) ** (n - 2) / 1e8
-            drdz = (1 + (r / 100 + z / 10000) * d) ** (n - 1) / 1e4
-            Nvd = -self.notional * disc_curve[self.payment] * self.dcf
-            a, b = 0.5 * Nvd * d2rdz2, Nvd * drdz
-        elif self.spread_compound_method == "isda_flat_compounding":
-            # d2rdz2 = 0.0
-            drdz = (1 + comb(n, 2) / n * r / 100 * d + comb(n, 3) / n * (r / 100 * d) ** 2) / 1e4
-            Nvd = -self.notional * disc_curve[self.payment] * self.dcf
-            a, b = 0.0, Nvd * drdz
+        Solve the DF node values and update all the ``curves``.
 
-        return a, b
+        This method uses a gradient based optimisation routine, to solve for all
+        the curve variables, :math:`\\mathbf{v}`, as follows,
 
+        .. math::
 
-class Cashflow:
-    """
-    Create a single cashflow amount on a payment date (effectively a CustomPeriod).
+           \\mathbf{v} = \\underset{\\mathbf{v}}{\\mathrm{argmin}} \;\; f(\\mathbf{v}) = \\underset{\\mathbf{v}}{\\mathrm{argmin}} \;\; (\\mathbf{r(v)} - \\mathbf{S})\\mathbf{W}(\\mathbf{r(v)} - \\mathbf{S})^\\mathbf{T}
 
-    Parameters
-    ----------
-    notional : float
-        The notional amount of the period (positive assumes paying a cashflow).
-    payment : Datetime
-        The adjusted payment date of the period.
-    currency : str
-        The currency of the cashflow (3-digit code).
-    stub_type : str
-        Record of the type of cashflow.
-    rate : float
-        An associated rate to relate to the cashflow, e.g. an FX fixing.
+        where :math:`\\mathbf{r}` are the mid-market rates of the calibrating
+        instruments, :math:`\\mathbf{S}` are the observed and target rates, and
+        :math:`\\mathbf{W}` is the diagonal array of weights.
 
-    Attributes
-    ----------
-    notional : float
-    payment : Datetime
-    stub_type : str
+        Returns
+        -------
+        None
+        """
 
-    Notes
-    -----
-    Other common :class:`BasePeriod` parameters not required for single cashflows are
-    set to *None*.
+        # Initialise data and clear and caches
+        self.g_list, self.lambd = [1e10], self.ini_lambda[0]
+        self._reset_properties_()
+        self._update_fx()
+        t0 = time()
+
+        # Begin iteration
+        for i in range(self.max_iter):
+            self.g_list.append(self.g.real)
+            if self.g.real < self.g_list[i] and (self.g_list[i] - self.g.real) < self.conv_tol:
+                # condition is set to less than to avoid the case where a null update
+                # results in the same solution and this is erroneously categorised
+                # as a converged solution.
+                return self._solver_result(1, i, time() - t0)
+            elif self.g.real < self.func_tol:
+                return self._solver_result(2, i, time() - t0)
+
+            # v_0 = self.v.copy()
+            v_1 = self._update_step_(self.algorithm)
+            # self.v_prev = v_0
+            self._update_curves_with_parameters(v_1)
 
-    The ``cashflow`` is defined as follows;
+            if self.callback is not NoInput.blank:
+                self.callback(self, i, v_1)
 
-    .. math::
+        return self._solver_result(-1, self.max_iter, time() - t0)
 
-       C = -N
+    def _solver_result(self, state: int, i: int, time: float):
+        self.result = _solver_result(state, i, self.g.real, time, True, self.algorithm)
+        return None
 
-    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+    def _update_curves_with_parameters(self, v_new):
+        """Populate the variable curves with the new values"""
+        var_counter = 0
+        for curve in self.curves.values():
+            # this was amended in PR126 as performance improvement to keep consistent `vars`
+            # and was restructured in PR## to decouple methods to accomodate vol surfaces
+            vars = curve.n - curve._ini_solve
+            curve._set_node_vector(v_new[var_counter : var_counter + vars], self._ad)
+            var_counter += vars
+
+        self._reset_properties_()
+        self._update_fx()
+
+    def _set_ad_order(self, order):
+        """Defines the node DF in terms of float, Dual or Dual2 for AD order calcs."""
+        for pre_solver in self.pre_solvers:
+            pre_solver._set_ad_order(order=order)
+        self._ad = order
+        self._reset_properties_()
+        for _, curve in self.curves.items():
+            curve._set_ad_order(order)
+        if self.fx is not NoInput.blank:
+            self.fx._set_ad_order(order)
 
-    .. math::
+    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+    # Commercial use of this code, and/or copying and redistribution is prohibited.
+    # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-       P = Cv(m) = -Nv(m)
+    def delta(self, npv, base: Union[str, NoInput] = NoInput(0), fx=NoInput(0)):
+        """
+        Calculate the delta risk sensitivity of an instrument's NPV to the
+        calibrating instruments of the :class:`~rateslib.solver.Solver`, and to
+        FX rates.
 
-    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+        Parameters
+        ----------
+        npv : Dual,
+            The NPV of the instrument or composition of instruments to risk.
+        base : str, optional
+            The currency (3-digit code) to report risk metrics in. If not given will
+            default to the local currency of the cashflows.
+        fx : FXRates, FXForwards, optional
+            The FX object to use to convert risk metrics. If needed but not given
+            will default to the ``fx`` object associated with the
+            :class:`~rateslib.solver.Solver`. It is not recommended to use this
+            argument with multi-currency instruments, see notes.
 
-    .. math::
+        Returns
+        -------
+        DataFrame
 
-       A = 0
+        Notes
+        -----
 
-    Example
-    -------
-    .. ipython:: python
+        **Output Structure**
 
-       cf = Cashflow(
-           notional=1e6,
-           payment=dt(2022, 8, 3),
-           currency="usd",
-           stub_type="Loan Payment",
-       )
-       cf.cashflows(curve=Curve({dt(2022, 1, 1): 1.0, dt(2022, 12, 31): 0.98}))
-    """
+        .. note::
 
-    def __init__(
-        self,
-        notional: float,
-        payment: datetime,
-        currency: Union[str, NoInput] = NoInput(0),
-        stub_type: Union[str, NoInput] = NoInput(0),
-        rate: Union[float, NoInput] = NoInput(0),
-    ):
-        self.notional, self.payment = notional, payment
-        self.currency = defaults.base_currency if currency is NoInput.blank else currency.lower()
-        self.stub_type = stub_type
-        self._rate = rate if rate is NoInput.blank else float(rate)
+           *Instrument* values are scaled to 1bp (1/10000th of a unit) when they are
+           rate based. *FX* values are scaled to pips (1/10000th of an FX rate unit).
 
-    def rate(self):
-        """
-        Return the associated rate initialised with the *Cashflow*. Not used for calculations.
-        """
-        return self._rate
+        The output ``DataFrame`` has the following structure:
 
-    def npv(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-        local: bool = False,
-    ):
-        """
-        Return the NPV of the *Cashflow*.
-        See
-        :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        if not isinstance(disc_curve, Curve) and curve is NoInput.blank:
-            raise TypeError("`curves` have not been supplied correctly.")
-        value = self.cashflow * disc_curve_[self.payment]
-        if local:
-            return {self.currency: value}
-        else:
-            fx, _ = _get_fx_and_base(self.currency, fx, base)
-            return fx * value
+        - A 3-level index by *'type'*, *'solver'*, and *'label'*;
+
+          - **type** is either *'instruments'* or *'fx'*, and fx exposures are only
+            calculated and displayed in some cases where genuine FX exposure arises.
+          - **solver** lists the different solver ``id`` s to identify between
+            different instruments in dependency chains from ``pre_solvers``.
+          - **label** lists the given instrument names in each solver using the
+            ``instrument_labels``.
+
+        - A 2-level column header index by *'local_ccy'* and *'display_ccy'*;
+
+          - **local_ccy** displays the currency for which cashflows are payable, and
+            therefore the local currency risk sensitivity amount.
+          - **display_ccy** displays the currency which the local currency risk
+            sensitivity has been converted to via an FX transformation.
+
+        Converting a delta from a local currency to another ``base`` currency also
+        introduces FX risk to the NPV of the instrument, which is included in the
+        output.
+
+        **Best Practice**
+
+        The ``fx`` option is provided to allow tactical and fast conversion of
+        delta risks to ``Instruments``. When constructing and pricing multi-currency
+        instruments it is likely that the :class:`~rateslib.solver.Solver` used is
+        associated with an :class:`~rateslib.fx.FXForwards` object to consistently
+        produce FX forward rates within an aribitrage free framework. In that case
+        it is more consistent to re-use those FX associations. If such an
+        association exists and a direct ``fx`` object is supplied a warning may be
+        emitted if they are not the same object.
+        """
+        base, fx = self._get_base_and_fx(base, fx)
+        fx_vars = tuple() if fx is NoInput.blank else fx.variables
+
+        inst_scalar = np.array(self.pre_rate_scalars) / 100  # instruments scalar
+        fx_scalar = 0.0001
+        container = {}
+        for ccy in npv:
+            container[("instruments", ccy, ccy)] = self.grad_s_Ploc(npv[ccy]) * inst_scalar
+            container[("fx", ccy, ccy)] = self.grad_f_Ploc(npv[ccy], fx_vars) * fx_scalar
+
+            if base is not NoInput.blank and base != ccy:
+                # extend the derivatives
+                f = fx.rate(f"{ccy}{base}")
+                container[("instruments", ccy, base)] = (
+                    self.grad_s_Pbase(
+                        npv[ccy], container[("instruments", ccy, ccy)] / inst_scalar, f
+                    )
+                    * inst_scalar
+                )
+                container[("fx", ccy, base)] = (
+                    self.grad_f_Pbase(npv[ccy], container[("fx", ccy, ccy)] / fx_scalar, f, fx_vars)
+                    * fx_scalar
+                )
 
-    def cashflows(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ) -> dict:
-        """
-        Return the cashflows of the *Cashflow*.
-        See
-        :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        fx, base = _get_fx_and_base(self.currency, fx, base)
+        # construct the DataFrame from container with hierarchical indexes
+        inst_idx = MultiIndex.from_tuples(
+            [("instruments",) + label for label in self.pre_instrument_labels],
+            names=["type", "solver", "label"],
+        )
+        fx_idx = MultiIndex.from_tuples(
+            [("fx", "fx", f[3:]) for f in fx_vars], names=["type", "solver", "label"]
+        )
+        indexes = {"instruments": inst_idx, "fx": fx_idx}
+        r_idx = inst_idx.append(fx_idx)
+        c_idx = MultiIndex.from_tuples([], names=["local_ccy", "display_ccy"])
+        df = DataFrame(None, index=r_idx, columns=c_idx)
+        for key, array in container.items():
+            df.loc[indexes[key[0]], (key[1], key[2])] = array
 
-        if disc_curve_ is NoInput.blank:
-            npv, npv_fx, df, collateral = None, None, None, None
-        else:
-            npv = float(self.npv(curve, disc_curve_))
-            npv_fx = npv * float(fx)
-            df, collateral = float(disc_curve_[self.payment]), disc_curve_.collateral
-
-        try:
-            cashflow_ = float(self.cashflow)
-        except TypeError:  # cashflow in superclass not a property
-            cashflow_ = None
-
-        rate = None if self.rate() is NoInput.blank else self.rate()
-        stub_type = None if self.stub_type is NoInput.blank else self.stub_type
-        return {
-            defaults.headers["type"]: type(self).__name__,
-            defaults.headers["stub_type"]: stub_type,
-            defaults.headers["currency"]: self.currency.upper(),
-            defaults.headers["a_acc_start"]: None,
-            defaults.headers["a_acc_end"]: None,
-            defaults.headers["payment"]: self.payment,
-            defaults.headers["convention"]: None,
-            defaults.headers["dcf"]: None,
-            defaults.headers["notional"]: float(self.notional),
-            defaults.headers["df"]: df,
-            defaults.headers["rate"]: rate,
-            defaults.headers["spread"]: None,
-            defaults.headers["cashflow"]: cashflow_,
-            defaults.headers["npv"]: npv,
-            defaults.headers["fx"]: float(fx),
-            defaults.headers["npv_fx"]: npv_fx,
-            defaults.headers["collateral"]: collateral,
-        }
+        if base is not NoInput.blank:
+            df.loc[r_idx, ("all", base)] = df.loc[r_idx, (slice(None), base)].sum(axis=1)
 
-    @property
-    def cashflow(self):
-        return -self.notional
+        sorted_cols = df.columns.sort_values()
+        return df.loc[:, sorted_cols].astype("float64")
 
-    def analytic_delta(
-        self,
-        curve: Optional[Curve] = None,
-        disc_curve: Optional[Curve] = None,
-        fx: Optional[Union[float, FXRates, FXForwards]] = None,
-        base: Optional[str] = None,
+    def _get_base_and_fx(
+        self, base: Union[str, NoInput], fx: Union[FXForwards, FXRates, float, NoInput]
     ):
+        if base is not NoInput.blank and self.fx is NoInput.blank and fx is NoInput.blank:
+            raise ValueError(
+                "`base` is given but `fx` is not and Solver does not "
+                "contain an attached FXForwards object."
+            )
+        elif fx is NoInput.blank:
+            fx = self.fx
+        elif fx is not NoInput.blank and self.fx is not NoInput.blank:
+            if id(fx) != id(self.fx):
+                warnings.warn(
+                    "Solver contains an `fx` attribute but an `fx` argument has been "
+                    "supplied which is not the same. This can lead to risk sensitivity "
+                    "inconsistencies, mathematically.",
+                    UserWarning,
+                )
+        if base is not NoInput.blank:
+            base = base.lower()
+        return base, fx
+
+    def gamma(self, npv, base=NoInput(0), fx=NoInput(0)):
         """
-        Return the analytic delta of the *Cashflow*.
-        See
-        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
-        """
-        return 0
+        Calculate the cross-gamma risk sensitivity of an instrument's NPV to the
+        calibrating instruments of the :class:`~rateslib.solver.Solver`.
 
+        Parameters
+        ----------
+        npv : Dual2,
+            The NPV of the instrument or composition of instruments to risk.
+        base : str, optional
+            The currency (3-digit code) to report risk metrics in. If not given will
+            default to the local currency of the cashflows.
+        fx : FXRates, FXForwards, optional
+            The FX object to use to convert risk metrics. If needed but not given
+            will default to the ``fx`` object associated with the
+            :class:`~rateslib.solver.Solver`.
 
-# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-# Commercial use of this code, and/or copying and redistribution is prohibited.
-# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
+        Returns
+        -------
+        DataFrame
+
+        Notes
+        -----
+        .. note::
 
+           *Instrument* values are scaled to 1bp (1/10000th of a unit) when they are
+           rate based.
 
-class IndexMixin(metaclass=ABCMeta):
-    """
-    Abstract base class to include methods and properties related to indexed *Periods*.
-    """
+           *FX* values are scaled to pips (1/10000th of an FX unit).
 
-    index_base: Union[float, Series, NoInput] = NoInput(0)
-    index_method: str = ""
-    index_fixings: Union[float, Series, NoInput] = NoInput(0)
-    index_lag: Union[int, NoInput] = NoInput(0)
-    payment: datetime = datetime(1990, 1, 1)
-    currency: str = ""
-
-    def cashflow(self, curve: Union[IndexCurve, NoInput] = NoInput(0)) -> Optional[DualTypes]:
-        """
-        float, Dual or Dual2 : The calculated value from rate, dcf and notional,
-        adjusted for the index.
-        """
-        if self.real_cashflow is None:
-            return None
-        index_ratio, _, _ = self.index_ratio(curve)
-        if index_ratio is None:
-            return None
-        else:
-            if self.index_only:
-                _ = -1.0
-            else:
-                _ = 0.0
-            _ = self.real_cashflow * (index_ratio + _)
-        return _
+        The output ``DataFrame`` has the following structure:
 
-    def index_ratio(self, curve: Union[IndexCurve, NoInput] = NoInput(0)) -> tuple:
-        """
-        Calculate the index ratio for the end date of the *IndexPeriod*.
+        - A 5-level index by *'local_ccy'*, *'display_ccy'*, *'type'*, *'solver'*,
+          and *'label'*;
+
+          - **local_ccy** displays the currency for which cashflows are payable, and
+            therefore the local currency risk sensitivity amount.
+          - **display_ccy** displays the currency which the local currency risk
+            sensitivity has been converted to via an FX transformation.
+          - **type** is either *'instruments'* or *'fx'*, and fx exposures are only
+            calculated and displayed in some cases where genuine FX exposure arises.
+          - **solver** lists the different solver ``id`` s to identify between
+            different instruments in dependency chains from ``pre_solvers``.
+          - **label** lists the given instrument names in each solver using the
+            ``instrument_labels``.
+
+        - A 3-level column header index using the last three levels of the above;
+
+        Converting a gamma/delta from a local currency to another ``base`` currency also
+        introduces FX risk to the NPV of the instrument, which is included in the
+        output.
 
-        .. math::
+        Examples
+        --------
+        This example replicates the analytical calculations demonstrated in
+        *Pricing and Trading Interest Rate Derivatives (2022)*, derived from
+        first principles.
+        The results are stated in the cross-gamma grid in figure 22.1.
 
-           I(m) = \\frac{I_{val}(m)}{I_{base}}
+        .. ipython:: python
 
-        Parameters
-        ----------
-        curve : IndexCurve
-            The index curve from which index values are forecast.
+           curve_r = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="r"
+           )
+           curve_z = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="z"
+           )
+           curve_s = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 0.99,
+                   dt(2024, 1, 1): 0.98,
+                   dt(2025, 1, 1): 0.97,
+                   dt(2026, 1, 1): 0.96,
+                   dt(2027, 1, 1): 0.95,
+               },
+               id="s"
+           )
+           args = dict(termination="1Y", frequency="A", fixing_method="ibor", leg2_fixing_method="ibor")
+           instruments = [
+               SBS(dt(2022, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2023, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2024, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2025, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2026, 1, 1), curves=["r", "s", "s", "s"], **args),
+               SBS(dt(2022, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2023, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2024, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2025, 1, 1), curves=["r", "s", "z", "s"], **args),
+               SBS(dt(2026, 1, 1), curves=["r", "s", "z", "s"], **args),
+               IRS(dt(2022, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2023, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2024, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2025, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+               IRS(dt(2026, 1, 1), "1Y", "A", curves=["r", "s"], leg2_fixing_method="ibor"),
+           ]
+           solver = Solver(
+               curves=[curve_r, curve_s, curve_z],
+               instruments=instruments,
+               s=[0.]*5 + [0.]*5 + [1.5]*5,
+               id="sonia",
+               instrument_labels=[
+                   "s1", "s2", "s3", "s4", "s5",
+                   "z1", "z2", "z3", "z4", "z5",
+                   "r1", "r2", "r3", "r4", "r5",
+               ],
+           )
+           irs = IRS(dt(2022, 1, 1), "5Y", "A", notional=-8.3e8, curves=["z", "s"], leg2_fixing_method="ibor", fixed_rate=25.0)
+           irs.delta(solver=solver)
+           irs.gamma(solver=solver)
+        """
+        if self._ad != 2:
+            raise ValueError("`Solver` must be in ad order 2 to use `gamma` method.")
+
+        # new
+        base, fx = self._get_base_and_fx(base, fx)
+        fx_vars = tuple() if fx is NoInput.blank else fx.variables
+
+        inst_scalar = np.array(self.pre_rate_scalars) / 100  # instruments scalar
+        fx_scalar = np.ones(len(fx_vars)) * 0.0001
+        container = {}
+        for ccy in npv:
+            container[(ccy, ccy)] = {}
+            container[(ccy, ccy)]["instruments", "instruments"] = self.grad_s_sT_Ploc(
+                npv[ccy]
+            ) * np.matmul(inst_scalar[:, None], inst_scalar[None, :])
+            container[(ccy, ccy)]["fx", "instruments"] = self.grad_f_sT_Ploc(
+                npv[ccy], fx_vars
+            ) * np.matmul(fx_scalar[:, None], inst_scalar[None, :])
+            container[(ccy, ccy)]["instruments", "fx"] = container[(ccy, ccy)][
+                ("fx", "instruments")
+            ].T
+            container[(ccy, ccy)]["fx", "fx"] = self.grad_f_fT_Ploc(npv[ccy], fx_vars) * np.matmul(
+                fx_scalar[:, None], fx_scalar[None, :]
+            )
 
-        Returns
-        -------
-        float, Dual, Dual2
-        """
-        denominator = self._index_value(
-            i_fixings=self.index_base,
-            i_date=getattr(self, "start", None),  # IndexCashflow has no start
-            i_curve=curve,
-            i_lag=self.index_lag,
-            i_method=self.index_method,
+            if base is not NoInput.blank and base != ccy:
+                # extend the derivatives
+                f = fx.rate(f"{ccy}{base}")
+                container[(ccy, base)] = {}
+                container[(ccy, base)]["instruments", "instruments"] = self.grad_s_sT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["instruments", "instruments"]
+                    / np.matmul(inst_scalar[:, None], inst_scalar[None, :]),
+                    f,
+                ) * np.matmul(inst_scalar[:, None], inst_scalar[None, :])
+                container[(ccy, base)]["fx", "instruments"] = self.grad_f_sT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["fx", "instruments"]
+                    / np.matmul(fx_scalar[:, None], inst_scalar[None, :]),
+                    f,
+                    fx_vars,
+                ) * np.matmul(fx_scalar[:, None], inst_scalar[None, :])
+                container[(ccy, base)]["instruments", "fx"] = container[(ccy, base)][
+                    ("fx", "instruments")
+                ].T
+                container[(ccy, base)]["fx", "fx"] = self.grad_f_fT_Pbase(
+                    npv[ccy],
+                    container[(ccy, ccy)]["fx", "fx"]
+                    / np.matmul(fx_scalar[:, None], fx_scalar[None, :]),
+                    f,
+                    fx_vars,
+                ) * np.matmul(fx_scalar[:, None], fx_scalar[None, :])
+
+        # construct the DataFrame from container with hierarchical indexes
+        currencies = list(npv.keys())
+        local_keys = [(ccy, ccy) for ccy in currencies]
+        base_keys = [] if base is NoInput.blank else [(ccy, base) for ccy in currencies]
+        all_keys = sorted(list(set(local_keys + base_keys)))
+        inst_keys = [("instruments",) + label for label in self.pre_instrument_labels]
+        fx_keys = [("fx", "fx", f[3:]) for f in fx_vars]
+        idx_tuples = [c + _ for c in all_keys for _ in inst_keys + fx_keys]
+        ridx = MultiIndex.from_tuples(
+            [key for key in idx_tuples],
+            names=["local_ccy", "display_ccy", "type", "solver", "label"],
         )
-        numerator = self._index_value(
-            i_fixings=self.index_fixings,
-            i_date=self.end,
-            i_curve=curve,
-            i_lag=self.index_lag,
-            i_method=self.index_method,
+        if base is not NoInput.blank:
+            ridx = ridx.append(
+                MultiIndex.from_tuples(
+                    [("all", base) + _ for _ in inst_keys + fx_keys],
+                    names=["local_ccy", "display_ccy", "type", "solver", "label"],
+                )
+            )
+        cidx = MultiIndex.from_tuples(
+            [_ for _ in inst_keys + fx_keys], names=["type", "solver", "label"]
         )
-        if numerator is None or denominator is None:
-            return None, numerator, denominator
-        else:
-            return numerator / denominator, numerator, denominator
+        df = DataFrame(None, index=ridx, columns=cidx)
+        for key, d in container.items():
+            array = np.block(
+                [
+                    [d[("instruments", "instruments")], d[("instruments", "fx")]],
+                    [d[("fx", "instruments")], d[("fx", "fx")]],
+                ]
+            )
+            locator = key + (slice(None), slice(None), slice(None))
+            df.loc[locator, :] = array
 
-    @staticmethod
-    def _index_value_from_curve(
-        i_date: datetime,
-        i_curve: Union[IndexCurve, NoInput],
-        i_lag: int,
-        i_method: str,
-    ) -> Optional[DualTypes]:
-        if i_curve is NoInput.blank:
-            return None
-        elif (not isinstance(i_curve, IndexCurve) and not isinstance(i_curve, CompositeCurve)) or (
-            isinstance(i_curve, CompositeCurve) and not isinstance(i_curve.curves[0], IndexCurve)
-        ):
-            raise TypeError("`index_value` must be forecast from an `IndexCurve`.")
-        elif i_lag != i_curve.index_lag:
-            return None  # TODO decide if RolledCurve to correct index lag be attempted
-        else:
-            return i_curve.index_value(i_date, i_method)
+        if base is not NoInput.blank:
+            # sum over all the base rows to aggregate
+            gdf = (
+                df.loc[(currencies, base, slice(None), slice(None), slice(None)), :]
+                .groupby(level=[2, 3, 4])
+                .sum()
+            )
+            gdf.index = MultiIndex.from_tuples([("all", base) + _ for _ in gdf.index])
+            df.loc[("all", base, slice(None), slice(None), slice(None))] = gdf
 
-    @staticmethod
-    def _index_value(
-        i_fixings: Union[float, Series, NoInput],
-        i_date: datetime,
-        i_curve: Union[IndexCurve, NoInput],
-        i_lag: int,
-        i_method: str,
-    ) -> Union[DualTypes, NoInput]:
-        """
-        Project an index rate, or lookup from provided fixings, for a given date.
+        return df.astype("float64")
 
-        If ``index_fixings`` are set on the period this will be used instead of
-        the ``curve``.
+    def _pnl_explain(self, npv, ds, dfx=None, base=NoInput(0), fx=NoInput(0), order=1):
+        """
+        Calculate PnL from market movements over delta and, optionally, gamma.
 
         Parameters
         ----------
-        curve : IndexCurve
+        npv : Dual or Dual2,
+            The initial NPV of the instrument or composition of instruments to value.
+        ds : sequence of float
+            The projected market movements of calibrating instruments of the solver,
+            scaled to the appropriate value amount matching the delta representation.
+        dfx : sequence of float
+            The projected market movements of FX rates,
+            scaled to the appropriate value amount matching the delta representation.
+        base : str, optional
+            The currency (3-digit code) to report risk metrics in. If not given will
+            default to the local currency of the cashflows.
+        fx : FXRates, FXForwards, optional
+            The FX object to use to convert risk metrics. If needed but not given
+            will default to the ``fx`` object associated with the
+            :class:`~rateslib.solver.Solver`.
+        order : int in {1, 2}
+            Whether to return a first order delta PnL explain or a second order one
+            including gamma contribution.
 
         Returns
         -------
-        float, Dual, Dual2
+        DataFrame
         """
-        if i_fixings is NoInput.blank:
-            return IndexMixin._index_value_from_curve(i_date, i_curve, i_lag, i_method)
-        else:
-            if isinstance(i_fixings, Series):
-                if i_method == "daily":
-                    adj_date = i_date
-                    unavailable_date = i_fixings.index[-1]
-                else:
-                    adj_date = datetime(i_date.year, i_date.month, 1)
-                    _ = i_fixings.index[-1]
-                    unavailable_date = _get_eom(_.month, _.year)
-
-                if i_date > unavailable_date:
-                    if i_curve is NoInput.blank:
-                        return NoInput(0)
-                    else:
-                        return IndexMixin._index_value_from_curve(i_date, i_curve, i_lag, i_method)
-                    # raise ValueError(
-                    #     "`index_fixings` cannot forecast the index value. "
-                    #     f"There are no fixings available after date: {unavailable_date}"
-                    # )
-                else:
-                    try:
-                        return i_fixings[adj_date]
-                    except KeyError:
-                        s = i_fixings.copy()
-                        s.loc[adj_date] = np.NaN  # type: ignore[call-overload]
-                        _ = s.sort_index().interpolate("time")[adj_date]
-                        return _
-            else:
-                return i_fixings
+        raise NotImplementedError()
 
-    def npv(
-        self,
-        curve: Union[IndexCurve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-        local: bool = False,
-    ):
-        """
-        Return the cashflows of the *IndexPeriod*.
-        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
+    def market_movements(self, solver: Solver):
         """
-        disc_curve_: Curve = _disc_from_curve(curve, disc_curve)
-        if not isinstance(disc_curve, Curve) and curve is NoInput.blank:
-            raise TypeError("`curves` have not been supplied correctly.")
-        value = self.cashflow(curve) * disc_curve_[self.payment]
-        if local:
-            return {self.currency: value}
-        else:
-            fx, _ = _get_fx_and_base(self.currency, fx, base)
-            return fx * value
-
-    @property
-    @abstractmethod
-    def real_cashflow(self):
-        pass  # pragma: no cover
+        Determine market movements between the *Solver's* instrument rates and those rates priced
+        from a second *Solver*.
 
+        Parameters
+        ----------
+        solver: Solver
+            The other *Solver* whose *Curves* are to be used for measuring the final instrument
+            rates of the existing *Solver's* instruments.
 
-class IndexFixedPeriod(IndexMixin, FixedPeriod):  # type: ignore[misc]
-    """
-    Create a period defined with a real rate adjusted by an index.
+        Returns
+        -------
+        DataFrame
 
-    When used with an inflation index this defines a real coupon period with a
-    cashflow adjusted upwards by the inflation index.
+        Notes
+        -----
+        .. warning::
+           Market movement calculations are only possible between *Solvers* whose ``instruments``
+           are associated with *Curves* with string ID mappings (which is best practice and
+           demonstrated HERE XXX). This allows two different
+           *Solvers* to contain their own *Curves* (which may or may not be equivalent models),
+           and for the instrument rates of one *Solver* to be evaluated by the *Curves* present
+           in another *Solver*.
+        """
+        r_0 = self.r_pre
+        r_1 = np.array(
+            [
+                _[0].rate(*_[1], **{**_[2], **{"solver": solver, "fx": solver.fx}})
+                for _ in self.pre_instruments
+            ]
+        )
+        return DataFrame(
+            (r_1 - r_0) * 100 / np.array(self.pre_rate_scalars),
+            index=self.pre_instrument_labels,
+        )
 
-    Parameters
-    ----------
-    args : dict
-        Required positional args to :class:`FixedPeriod`.
-    index_base : float or None, optional
-        The base index to determine the cashflow.
-    index_fixings : float, or Series, optional
-        If a float scalar, will be applied as the index fixing for the settlement, or
-        payment, date.
-        If a datetime indexed ``Series`` will use the
-        fixings that are available in that object, using linear interpolation if
-        necessary.
-    index_method : str, optional
-        Whether the indexing uses a daily measure for settlement or the most recently
-        monthly data taken from the first day of month. Defined by default.
-    index_lag : int, optional
-        The number of months by which the index value is lagged. Used to ensure
-        consistency between curves and forecast values. Defined by default.
-    kwargs : dict
-        Required keyword arguments to :class:`FixedPeriod`.
+    def jacobian(self, solver: Solver):
+        """
+        Calculate the Jacobian with respect to another *Solver's* instruments.
 
-    Notes
-    -----
-    The ``real_cashflow`` is defined as follows;
+        Parameters
+        ----------
+        solver : Solver
+            The other ``Solver`` for which the Jacobian is to be determined.
 
-    .. math::
+        Returns
+        -------
+        DataFrame
 
-       C_{real} = -NdR
+        Notes
+        -----
+        This Jacobian converts risk sensitivities expressed in the underlying *Solver's*
+        instruments to the instruments in the other ``solver``.
 
-    The ``cashflow`` is defined as follows;
+        .. warning::
+           A Jacobian transformation is only possible between *Solvers* whose ``instruments``
+           are associated with *Curves* with string ID mappings (which is best practice and
+           demonstrated HERE XXX). This allows two different
+           *Solvers* to contain their own *Curves* (which may or may not be equivalent models),
+           and for the instrument rates of one *Solver* to be evaluated by the *Curves* present
+           in another *Solver*
 
-    .. math::
+        Examples
+        --------
+        This example creates a Jacobian transformation between par tenor IRS and forward tenor
+        IRS. These models are completely consistent and lossless.
 
-       C = C_{real}I(m) = -NdRI(m)
+        .. ipython:: python
 
-    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+           par_curve = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 1.0,
+                   dt(2024, 1, 1): 1.0,
+                   dt(2025, 1, 1): 1.0,
+               },
+               id="curve",
+           )
+           par_instruments = [
+               IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+               IRS(dt(2022, 1, 1), "2Y", "A", curves="curve"),
+               IRS(dt(2022, 1, 1), "3Y", "A", curves="curve"),
+           ]
+           par_solver = Solver(
+               curves=[par_curve],
+               instruments=par_instruments,
+               s=[1.21, 1.635, 1.99],
+               id="par_solver",
+               instrument_labels=["1Y", "2Y", "3Y"],
+           )
 
-    .. math::
+           fwd_curve = Curve(
+               nodes={
+                   dt(2022, 1, 1): 1.0,
+                   dt(2023, 1, 1): 1.0,
+                   dt(2024, 1, 1): 1.0,
+                   dt(2025, 1, 1): 1.0,
+               },
+               id="curve"
+           )
+           fwd_instruments = [
+               IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+               IRS(dt(2023, 1, 1), "1Y", "A", curves="curve"),
+               IRS(dt(2024, 1, 1), "1Y", "A", curves="curve"),
+           ]
+           s_fwd = [float(_.rate(solver=par_solver)) for _ in fwd_instruments]
+           fwd_solver = Solver(
+               curves=[fwd_curve],
+               instruments=fwd_instruments,
+               s=s_fwd,
+               id="fwd_solver",
+               instrument_labels=["1Y", "1Y1Y", "2Y1Y"],
+           )
 
-       P = Cv = -NdRv(m)I(m)
+           par_solver.jacobian(fwd_solver)
 
-    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+        """
+        # Get the instrument rates for self solver evaluated using the curves and links of other
+        r = np.array(
+            [
+                _[0].rate(*_[1], **{**_[2], **{"solver": solver, "fx": solver.fx}})
+                for _ in self.pre_instruments
+            ]
+        )
+        # Get the gradient of these rates with respect to the variable in other
+        grad_v_rT = np.array([gradient(_, solver.pre_variables) for _ in r]).T
+        return DataFrame(
+            np.matmul(solver.grad_s_vT_pre, grad_v_rT),
+            columns=self.pre_instrument_labels,
+            index=solver.pre_instrument_labels,
+        )
 
-    .. math::
 
-       A = - \\frac{\\partial P}{\\partial R} = Ndv(m)I(m)
+# Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
+# Commercial use of this code, and/or copying and redistribution is prohibited.
+# Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
-    Examples
-    --------
-    .. ipython:: python
 
-       ifp = IndexFixedPeriod(
-           start=dt(2022, 2, 1),
-           end=dt(2022, 8, 1),
-           payment=dt(2022, 8, 2),
-           frequency="S",
-           notional=1e6,
-           currency="eur",
-           convention="30e360",
-           fixed_rate=5.0,
-           index_lag=2,
-           index_base=100.25,
-       )
-       ifp.cashflows(
-           curve=IndexCurve({dt(2022, 1, 1):1.0, dt(2022, 12, 31): 0.99}, index_base=100.0, index_lag=2),
-           disc_curve=Curve({dt(2022, 1, 1):1.0, dt(2022, 12, 31): 0.98})
-       )
+def _float_if_not_string(x):
+    if not isinstance(x, str):
+        return float(x)
+    return x
+
+
+def newton_1dim(
+    f,
+    g0,
+    max_iter=50,
+    func_tol=1e-14,
+    conv_tol=1e-9,
+    args=(),
+    pre_args=(),
+    final_args=(),
+    raise_on_fail=True,
+):
     """
+    Use the Newton-Raphson algorithm to determine the root of a function searching **one** variable.
 
-    def __init__(
-        self,
-        *args,
-        index_base: Union[float, Series, NoInput] = NoInput(0),
-        index_fixings: Union[float, Series, NoInput] = NoInput(0),
-        index_method: Union[str, NoInput] = NoInput(0),
-        index_lag: Union[int, NoInput] = NoInput(0),
-        **kwargs,
-    ):
-        # if index_base is None:
-        #     raise ValueError("`index_base` cannot be None.")
-        self.index_base = index_base
-        self.index_fixings = index_fixings
-        self.index_only = False
-        self.index_method = (
-            defaults.index_method if index_method is NoInput.blank else index_method.lower()
-        )
-        self.index_lag = defaults.index_lag if index_lag is NoInput.blank else index_lag
-        if self.index_method not in ["daily", "monthly"]:
-            raise ValueError("`index_method` must be in {'daily', 'monthly'}.")
-        super(IndexMixin, self).__init__(*args, **kwargs)
-
-    def analytic_delta(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ):
-        """
-        Return the analytic delta of the *IndexFixedPeriod*.
-        See :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
-        """
-        real_a_delta = super().analytic_delta(curve, disc_curve, fx, base)
-        index_ratio, _, _ = self.index_ratio(curve)
-        _ = None if index_ratio is None else real_a_delta * index_ratio
-        return _
-
-    @property
-    def real_cashflow(self):
-        """
-        float, Dual or Dual2 : The calculated real value from rate, dcf and notional.
-        """
-        if self.fixed_rate is NoInput.blank:
-            return None
-        else:
-            return -self.notional * self.dcf * self.fixed_rate / 100
+    Solves the root equation :math:`f(g; s_i)=0` for *g*.
 
-    # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
-    # Commercial use of this code, and/or copying and redistribution is prohibited.
-    # Contact rateslib at gmail.com if this code is observed outside its intended sphere
+    Parameters
+    ----------
+    f: callable
+        The function, *f*, to find the root of. Of the signature: `f(g, *args)`.
+        Must return a tuple where the second value is the derivative of *f* with respect to *g*.
+    g0: DualTypes
+        Initial guess of the root. Should be reasonable to avoid failure.
+    max_iter: int
+        The maximum number of iterations to try before exiting.
+    func_tol: float, optional
+        The absolute function tolerance to reach before exiting.
+    conv_tol: float, optional
+        The convergence tolerance for subsequent iterations of *g*.
+    args: tuple of float, Dual or Dual2
+        Additional arguments passed to ``f``.
+    pre_args: tuple
+        Additional arguments passed to ``f`` used only in the float solve section of
+        the algorithm.
+        Functions are called with the signature `f(g, *(*args[as float], *pre_args))`.
+    final_args: tuple of float, Dual, Dual2
+        Additional arguments passed to ``f`` in the final iteration of the algorithm
+        to capture AD sensitivities.
+        Functions are called with the signature `f(g, *(*args, *final_args))`.
+    raise_on_fail: bool, optional
+        If *False* will return a solver result dict with state and message indicating failure.
 
-    def cashflows(
-        self,
-        curve: Union[IndexCurve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ):
-        """
-        Return the cashflows of the *IndexFixedPeriod*.
-        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
-        """
-        disc_curve_: Union[Curve, NoInput] = _disc_maybe_from_curve(curve, disc_curve)
-        fx, base = _get_fx_and_base(self.currency, fx, base)
+    Returns
+    -------
+    dict
 
-        if disc_curve_ is NoInput.blank or self.fixed_rate is NoInput.blank:
-            npv = None
-            npv_fx = None
-        else:
-            npv = float(self.npv(curve, disc_curve_))
-            npv_fx = npv * float(fx)
+    Examples
+    --------
+    Iteratively solve the equation: :math:`f(g, s) = g^2 - s = 0`.
 
-        index_ratio_, index_val_, index_base_ = self.index_ratio(curve)
+    .. ipython:: python
 
-        return {
-            **super(FixedPeriod, self).cashflows(curve, disc_curve_, fx, base),
-            defaults.headers["rate"]: self.fixed_rate,
-            defaults.headers["spread"]: None,
-            defaults.headers["real_cashflow"]: self.real_cashflow,
-            defaults.headers["index_base"]: _float_or_none(index_base_),
-            defaults.headers["index_value"]: _float_or_none(index_val_),
-            defaults.headers["index_ratio"]: _float_or_none(index_ratio_),
-            defaults.headers["cashflow"]: _float_or_none(self.cashflow(curve)),
-            defaults.headers["npv"]: npv,
-            defaults.headers["fx"]: float(fx),
-            defaults.headers["npv_fx"]: npv_fx,
-        }
+       from rateslib.solver import newton_1dim
 
-    def npv(self, *args, **kwargs):
-        """
-        Return the cashflows of the *IndexFixedPeriod*.
-        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
-        """
-        return super().npv(*args, **kwargs)
+       def f(g, s):
+           f0 = g**2 - s   # Function value
+           f1 = 2*g        # Analytical derivative is required
+           return f0, f1
 
+       s = Dual(2.0, ["s"], [])
+       newton_1dim(f, g0=1.0, args=(s,))
+    """
+    t0 = time()
+    i = 0
 
-class IndexCashflow(IndexMixin, Cashflow):  # type: ignore[misc]
+    # First attempt solution using faster float calculations
+    float_args = tuple(_float_if_not_string(_) for _ in args)
+    g0 = float(g0)
+    state = -1
+
+    while i < max_iter:
+        f0, f1 = f(g0, *(*float_args, *pre_args))
+        i += 1
+        g1 = g0 - f0 / f1
+        if abs(f0) < func_tol:
+            state = 2
+            break
+        elif abs(g1 - g0) < conv_tol:
+            state = 1
+            break
+        g0 = g1
+
+    if i == max_iter:
+        if raise_on_fail:
+            raise ValueError(f"`max_iter`: {max_iter} exceeded in 'newton_1dim' algorithm'.")
+        else:
+            return _solver_result(-1, i, g1, time() - t0, log=True, algo="newton_1dim")
+
+    # # Final iteration method to preserve AD
+    f0, f1 = f(g1, *(*args, *final_args))
+    if isinstance(f0, (Dual, Dual2)) or isinstance(f1, (Dual, Dual2)):
+        i += 1
+        g1 = g1 - f0 / f1
+    if isinstance(f0, Dual2) or isinstance(f1, Dual2):
+        f0, f1 = f(g1, *(*args, *final_args))
+        i += 1
+        g1 = g1 - f0 / f1
+
+    # # Analytical approach to capture AD sensitivities
+    # f0, f1 = f(g1, *(*args, *final_args))
+    # if isinstance(f0, Dual):
+    #     g1 = Dual.vars_from(f0, float(g1), f0.vars, float(f1) ** -1 * -gradient(f0))
+    # if isinstance(f0, Dual2):
+    #     g1 = Dual2.vars_from(f0, float(g1), f0.vars, float(f1) ** -1 * -gradient(f0), [])
+    #     f02, f1 = f(g1, *(*args, *final_args))
+    #
+    #     #f0_beta = gradient(f0, order=1, vars=f0.vars, keep_manifold=True)
+    #
+    #     f0_gamma = gradient(f02, order=2)
+    #     f0_beta = gradient(f0, order=1)
+    #     # f1 = set_order_convert(g1, tag=[], order=2)
+    #     f1_gamma = gradient(f1, f0.vars, order=2)
+    #     f1_beta = gradient(f1, f0.vars, order=1)
+    #
+    #     g1_beta = -float(f1) ** -1 * f0_beta
+    #     g1_gamma = (
+    #         -float(f1)**-1 * f0_gamma +
+    #         float(f1)**-2 * (
+    #                 np.matmul(f0_beta[:, None], f1_beta[None, :]) +
+    #                 np.matmul(f1_beta[:, None], f0_beta[None, :]) +
+    #                 float(f0) * f1_gamma
+    #         ) -
+    #         2 * float(f1)**-3 * float(f0) * np.matmul(f1_beta[:, None], f1_beta[None, :])
+    #     )
+    #     g1 = Dual2.vars_from(f0, float(g1), f0.vars, g1_beta, g1_gamma.flatten())
+
+    return _solver_result(state, i, g1, time() - t0, log=False, algo="newton_1dim")
+
+
+def newton_ndim(
+    f,
+    g0,
+    max_iter=50,
+    func_tol=1e-14,
+    conv_tol=1e-9,
+    args=(),
+    pre_args=(),
+    final_args=(),
+    raise_on_fail=True,
+) -> dict:
     """
-    Create a cashflow defined with a real rate adjusted by an index.
+    Use the Newton-Raphson algorithm to determine the root of a function searching **many** variables.
 
-    When used with an inflation index this defines a real redemption with a
-    cashflow adjusted upwards by the inflation index.
+    Solves the *n* root equations :math:`f_i(g_1, \hdots, g_n; s_k)=0` for each :math:`g_j`.
 
     Parameters
     ----------
-    args : dict
-        Required positional args to :class:`Cashflow`.
-    index_base : float or None, optional
-        The base index to determine the cashflow.
-    index_fixings : float, or Series, optional
-        If a float scalar, will be applied as the index fixing for the whole
-        period. If a datetime indexed ``Series`` will use the
-        fixings that are available in that object, and derive the rest from the
-        ``curve``.
-    index_method : str
-        Whether the indexing uses a daily measure for settlement or the most recently
-        monthly data taken from the first day of month. Defined by default.
-    index_lag : int
-        The number of months by which the index value is lagged. Used to ensure
-        consistency between curves and forecast values. Defined by default.
-    index_only : bool
-        If *True* deduct the real notional from the cashflow and produce only the
-        indexed component.
-    end : datetime, optional
-        The registered end of a period when the index value is measured. If *None*
-        is set equal to the payment date.
-    kwargs : dict
-        Required keyword arguments to :class:`Cashflow`.
+    f: callable
+        The function, *f*, to find the root of. Of the signature: `f([g_1, .., g_n], *args)`.
+        Must return a tuple where the second value is the Jacobian of *f* with respect to *g*.
+    g0: Sequence of DualTypes
+        Initial guess of the root values. Should be reasonable to avoid failure.
+    max_iter: int
+        The maximum number of iterations to try before exiting.
+    func_tol: float, optional
+        The absolute function tolerance to reach before exiting.
+    conv_tol: float, optional
+        The convergence tolerance for subsequent iterations of *g*.
+    args: tuple of float, Dual or Dual2
+        Additional arguments passed to ``f``.
+    pre_args: tuple
+        Additional arguments passed to ``f`` only in the float solve section
+        of the algorithm.
+        Functions are called with the signature `f(g, *(*args[as float], *pre_args))`.
+    final_args: tuple of float, Dual, Dual2
+        Additional arguments passed to ``f`` in the final iteration of the algorithm
+        to capture AD sensitivities.
+        Functions are called with the signature `f(g, *(*args, *final_args))`.
+    raise_on_fail: bool, optional
+        If *False* will return a solver result dict with state and message indicating failure.
 
-    Notes
-    -----
-    The ``real_cashflow`` is defined as follows;
-
-    .. math::
+    Returns
+    -------
+    dict
 
-       C_{real} = -N
+    Examples
+    --------
+    Iteratively solve the equation system:
 
-    The ``cashflow`` is defined as follows;
+    - :math:`f_0(\mathbf{g}, s) = g_1^2 + g_2^2 + s = 0`.
+    - :math:`f_1(\mathbf{g}, s) = g_1^2 - 2g_2^2 + s = 0`.
 
-    .. math::
+    .. ipython:: python
 
-       C = C_{real}I(m) = -NI(m)
+       from rateslib.solver import newton_ndim
 
-    The :meth:`~rateslib.periods.BasePeriod.npv` is defined as;
+       def f(g, s):
+           # Function value
+           f0 = g[0] ** 2 + g[1] ** 2 + s
+           f1 = g[0] ** 2 - 2 * g[1]**2 - s
+           # Analytical derivative as Jacobian matrix is required
+           f00 = 2 * g[0]
+           f01 = 2 * g[1]
+           f10 = 2 * g[0]
+           f11 = -4 * g[1]
+           return [f0, f1], [[f00, f01], [f10, f11]]
 
-    .. math::
+       s = Dual(-2.0, ["s"], [])
+       newton_ndim(f, g0=[1.0, 1.0], args=(s,))
+    """
+    t0 = time()
+    i = 0
+    n = len(g0)
+
+    # First attempt solution using faster float calculations
+    float_args = tuple(_float_if_not_string(_) for _ in args)
+    g0 = np.array([float(_) for _ in g0])
+    state = -1
+
+    while i < max_iter:
+        f0, f1 = f(g0, *(*float_args, *pre_args))
+        f0 = np.array(f0)[:, np.newaxis]
+        f1 = np.array(f1)
+
+        i += 1
+        g1 = g0 - np.matmul(np.linalg.inv(f1), f0)[:, 0]
+        if all(abs(_) < func_tol for _ in f0[:, 0]):
+            state = 2
+            break
+        elif all(abs(g1[_] - g0[_]) < conv_tol for _ in range(n)):
+            state = 1
+            break
+        g0 = g1
+
+    if i == max_iter:
+        if raise_on_fail:
+            raise ValueError(f"`max_iter`: {max_iter} exceeded in 'newton_ndim' algorithm'.")
+        else:
+            return _solver_result(-1, i, g1, time() - t0, log=True, algo="newton_ndim")
+
+    # Final iteration method to preserve AD
+    f0, f1 = f(g1, *(*args, *final_args))
+    f1, f0 = np.array(f1), np.array(f0)
+
+    # get AD type
+    ad = 0
+    if _is_any_dual(f0) or _is_any_dual(f1):
+        ad, DualType = 1, Dual
+    elif _is_any_dual2(f0) or _is_any_dual2(f1):
+        ad, DualType = 2, Dual2
+
+    if ad > 0:
+        i += 1
+        g1 = g0 - dual_solve(f1, f0[:, None], allow_lsq=False, types=(DualType, DualType))[:, 0]
+    if ad == 2:
+        f0, f1 = f(g1, *(*args, *final_args))
+        f1, f0 = np.array(f1), np.array(f0)
+        i += 1
+        g1 = g1 - dual_solve(f1, f0[:, None], allow_lsq=False, types=(DualType, DualType))[:, 0]
+
+    return _solver_result(state, i, g1, time() - t0, log=False, algo="newton_ndim")
+
+
+STATE_MAP = {
+    1: ["SUCCESS", "`conv_tol` reached"],
+    2: ["SUCCESS", "`func_tol` reached"],
+    3: ["SUCCESS", "closed form valid"],
+    -1: ["FAILURE", "`max_iter` breached"],
+}
+
+
+def _solver_result(state: int, i: int, func_val: float, time: float, log: bool, algo: str):
+    if log:
+        print(
+            f"{STATE_MAP[state][0]}: {STATE_MAP[state][1]} after {i} iterations "
+            f"({algo}), `f_val`: {func_val}, "
+            f"`time`: {time:.4f}s"
+        )
+    return {
+        "status": STATE_MAP[state][0],
+        "state": state,
+        "g": func_val,
+        "iterations": i,
+        "time": time,
+    }
 
-       P = Cv(m) = -Nv(m)I(m)
 
-    The :meth:`~rateslib.periods.BasePeriod.analytic_delta` is defined as;
+def _is_any_dual(arr):
+    return any([isinstance(_, Dual) for _ in arr.flatten()])
 
-    .. math::
 
-       A = 0
+def _is_any_dual2(arr):
+    return any([isinstance(_, Dual2) for _ in arr.flatten()])
 
-    Example
-    -------
-    .. ipython:: python
 
-       icf = IndexCashflow(
-           notional=1e6,
-           end=dt(2022, 8, 1),
-           payment=dt(2022, 8, 3),
-           currency="usd",
-           stub_type="Loan Payment",
-           index_base=100.25
-       )
-       icf.cashflows(
-           curve=IndexCurve({dt(2022, 1, 1): 1.0, dt(2022, 12, 31): 0.99}, index_base=100.0),
-           disc_curve=Curve({dt(2022, 1, 1): 1.0, dt(2022, 12, 31): 0.98}),
-       )
+def quadratic_eqn(a, b, c, x0, raise_on_fail=True):
     """
+    Solve the quadratic equation, :math:`ax^2 + bx +c = 0`, with error reporting.
 
-    def __init__(
-        self,
-        *args,
-        index_base: float,
-        index_fixings: Union[float, Series, NoInput] = NoInput(0),
-        index_method: Union[str, NoInput] = NoInput(0),
-        index_lag: Union[int, NoInput] = NoInput(0),
-        index_only: bool = False,
-        end: Union[datetime, NoInput] = NoInput(0),
-        **kwargs,
-    ):
-        self.index_base = index_base
-        self.index_fixings = index_fixings
-        self.index_method = (
-            defaults.index_method if index_method is NoInput.blank else index_method.lower()
-        )
-        self.index_lag = defaults.index_lag if index_lag is NoInput.blank else index_lag
-        self.index_only = index_only
-        super(IndexMixin, self).__init__(*args, **kwargs)
-        self.end = self.payment if end is NoInput.blank else end
-
-    @property
-    def real_cashflow(self):
-        return -self.notional
+    Parameters
+    ----------
+    a: float, Dual Dual2
+        The *a* coefficient value.
+    b: float, Dual Dual2
+        The *b* coefficient value.
+    c: float, Dual Dual2
+        The *c* coefficient value.
+    x0: float
+        The expected solution to discriminate between two possible solutions.
+    raise_on_fail: bool, optional
+        Whether to raise if unsolved or return a solver result in failed state.
 
-    def cashflows(
-        self,
-        curve: Union[Curve, NoInput] = NoInput(0),
-        disc_curve: Union[Curve, NoInput] = NoInput(0),
-        fx: Union[float, FXRates, FXForwards, NoInput] = NoInput(0),
-        base: Union[str, NoInput] = NoInput(0),
-    ) -> dict:
-        """
-        Return the cashflows of the *IndexCashflow*.
-        See :meth:`BasePeriod.cashflows()<rateslib.periods.BasePeriod.cashflows>`
-        """
-        index_ratio_, index_val_, index_base_ = self.index_ratio(curve)
-        return {
-            **super(IndexMixin, self).cashflows(curve, disc_curve, fx, base),
-            defaults.headers["a_acc_end"]: self.end,
-            defaults.headers["real_cashflow"]: self.real_cashflow,
-            defaults.headers["index_base"]: _float_or_none(index_base_),
-            defaults.headers["index_value"]: _float_or_none(index_val_),
-            defaults.headers["index_ratio"]: _float_or_none(index_ratio_),
-            defaults.headers["cashflow"]: _float_or_none(self.cashflow(curve)),
-        }
+    Returns
+    -------
+    dict
 
-    def npv(self, *args, **kwargs):
-        """
-        Return the NPV of the *IndexCashflow*.
-        See :meth:`BasePeriod.npv()<rateslib.periods.BasePeriod.npv>`
-        """
-        return super().npv(*args, **kwargs)
+    Notes
+    -----
+    If ``a`` is evaluated to be less that 1e-15 in absolute terms then it is treated as zero and the
+    equation is solved as a linear equation in ``b`` and ``c`` only.
 
-    def analytic_delta(self, *args, **kwargs):
-        """
-        Return the analytic delta of the *IndexCashflow*.
-        See
-        :meth:`BasePeriod.analytic_delta()<rateslib.periods.BasePeriod.analytic_delta>`
-        """
-        return 0.0
+    Examples
+    --------
+    .. ipython:: python
 
+       from rateslib.solver import quadratic_eqn
 
-def _float_or_none(val):
-    if val is None:
-        return None
-    else:
-        return float(val)
+       quadratic_eqn(a=1.0, b=1.0, c=Dual(-6.0, ["c"], []), x0=-2.9)
 
+    """
+    discriminant = b**2 - 4 * a * c
+    if discriminant < 0.0:
+        if raise_on_fail:
+            raise ValueError("`quadratic_eqn` has failed to solve: discriminant is less than zero.")
+        else:
+            return _solver_result(
+                state=-1, i=0, func_val=1e308, time=0.0, log=True, algo="quadratic_eqn"
+            )
 
-def _disc_from_curve(curve: Curve, disc_curve: Union[Curve, NoInput]) -> Curve:
-    if disc_curve is NoInput.blank:
-        _: Curve = curve
+    if abs(a) > 1e-15:  # machine tolerance on normal float64 is 2.22e-16
+        sqrt_d = discriminant**0.5
+        _1 = (-b + sqrt_d) / (2 * a)
+        _2 = (-b - sqrt_d) / (2 * a)
+        if abs(x0 - _1) < abs(x0 - _2):
+            return _solver_result(
+                state=3, i=1, func_val=_1, time=0.0, log=False, algo="quadratic_eqn"
+            )
+        else:
+            return _solver_result(
+                state=3, i=1, func_val=_2, time=0.0, log=False, algo="quadratic_eqn"
+            )
     else:
-        _ = disc_curve
-    return _
+        # 'a' is considered too close to zero for the quadratic eqn, solve the linear eqn
+        # to avoid division by zero errors
+        return _solver_result(
+            state=3, i=1, func_val=-c / b, time=0.0, log=False, algo="quadratic_eqn->linear_eqn"
+        )
 
 
-def _disc_maybe_from_curve(
-    curve: Union[Curve, NoInput, dict], disc_curve: Union[Curve, NoInput]
-) -> Union[Curve, NoInput]:
-    if disc_curve is NoInput.blank:
-        if isinstance(curve, dict):
-            raise ValueError("`disc_curve` cannot be inferred from a dictionary of curves.")
-        _: Curve = curve
-    else:
-        _ = disc_curve
-    return _
+# def _brents(f, x0, x1, max_iter=50, tolerance=1e-9):
+#     """
+#     Alternative root solver. Used for solving premium adjutsed option strikes from delta values.
+#     """
+#     fx0 = f(x0)
+#     fx1 = f(x1)
+#
+#     if float(fx0 * fx1) > 0:
+#         raise ValueError("`brents` must initiate from function values with opposite signs.")
+#
+#     if abs(fx0) < abs(fx1):
+#         x0, x1 = x1, x0
+#         fx0, fx1 = fx1, fx0
+#
+#     x2, fx2 = x0, fx0
+#
+#     mflag = True
+#     steps_taken = 0
+#
+#     while steps_taken < max_iter and abs(x1 - x0) > tolerance:
+#         fx0 = f(x0)
+#         fx1 = f(x1)
+#         fx2 = f(x2)
+#
+#         if fx0 != fx2 and fx1 != fx2:
+#             L0 = (x0 * fx1 * fx2) / ((fx0 - fx1) * (fx0 - fx2))
+#             L1 = (x1 * fx0 * fx2) / ((fx1 - fx0) * (fx1 - fx2))
+#             L2 = (x2 * fx1 * fx0) / ((fx2 - fx0) * (fx2 - fx1))
+#             new = L0 + L1 + L2
+#
+#         else:
+#             new = x1 - ((fx1 * (x1 - x0)) / (fx1 - fx0))
+#
+#         if (
+#             (float(new) < float((3 * x0 + x1) / 4) or float(new) > float(x1))
+#             or (mflag is True and (abs(new - x1)) >= (abs(x1 - x2) / 2))
+#             or (mflag is False and (abs(new - x1)) >= (abs(x2 - d) / 2))
+#             or (mflag is True and (abs(x1 - x2)) < tolerance)
+#             or (mflag is False and (abs(x2 - d)) < tolerance)
+#         ):
+#             new = (x0 + x1) / 2
+#             mflag = True
+#
+#         else:
+#             mflag = False
+#
+#         fnew = f(new)
+#         d, x2 = x2, x1
+#
+#         if float(fx0 * fnew) < 0:
+#             x1 = new
+#         else:
+#             x0 = new
+#
+#         if abs(fx0) < abs(fx1):
+#             x0, x1 = x1, x0
+#
+#         steps_taken += 1
+#
+#     return x1, steps_taken
```

### Comparing `rateslib-1.1.1/rateslib/scheduling.py` & `rateslib-1.2.0/rateslib/scheduling.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,20 +321,20 @@
             termination_ = termination
         self.termination: datetime = termination_
 
         if self.termination <= self.effective:
             raise ValueError("`termination` must be after `effective`.")
 
         if frequency == "Z":
-            self.ueffective = None
-            self.utermination = None
-            self.stub = None
-            self.front_stub = None
-            self.back_stub = None
-            self.roll = None
+            self.ueffective = NoInput(0)
+            self.utermination = NoInput(0)
+            self.stub = NoInput(0)
+            self.front_stub = NoInput(0)
+            self.back_stub = NoInput(0)
+            self.roll = NoInput(0)
             self.uschedule = [self.effective, self.termination]
             self._attribute_schedules()
             return None
 
         if stub is NoInput.blank:
             # if specific stub dates are given we cannot know if these are long or short
             if front_stub is NoInput.blank:
@@ -476,15 +476,15 @@
             if not valid:
                 raise ValueError("date, stub and roll inputs are invalid")
             else:
                 # stub inference is not required, no stubs are necessary
                 self.ueffective = self.effective
                 self.utermination = parsed_args["utermination"]
                 self.front_stub = parsed_args["ueffective"]
-                self.back_stub = None
+                self.back_stub = NoInput(0)
                 self.roll = parsed_args["roll"]
 
     def _back_sided_stub_parsing(self, front_stub, back_stub, roll):
         if front_stub is not NoInput.blank:
             raise ValueError("`stub` is only back sided but `front_stub` given.")
         if back_stub is NoInput.blank:
             valid, parsed_args = _infer_stub_date(
@@ -519,29 +519,29 @@
                 self.calendar,
             )
             if not valid:
                 raise ValueError("date, stub and roll inputs are invalid")
             else:
                 self.ueffective = parsed_args["ueffective"]
                 self.utermination = self.termination
-                self.front_stub = None
+                self.front_stub = NoInput(0)
                 self.back_stub = parsed_args["utermination"]
                 self.roll = parsed_args["roll"]
 
     def _attribute_schedules(self):
         """Attributes additional schedules according to date adjust and payment lag."""
         self.aschedule = [_adjust_date(dt, self.modifier, self.calendar) for dt in self.uschedule]
         self.pschedule = [
             add_tenor(dt, f"{self.payment_lag}B", "NONE", self.calendar, NoInput(0))
             for dt in self.aschedule
         ]
         self.stubs = [False] * (len(self.uschedule) - 1)
-        if self.front_stub is not None:
+        if self.front_stub is not NoInput(0):
             self.stubs[0] = True
-        if self.back_stub is not None:
+        if self.back_stub is not NoInput(0):
             self.stubs[-1] = True
 
     def __repr__(self):
         str = (
             f"freq: {self.frequency},  stub: {self.stub},  roll: {self.roll}"
             f",  pay lag: {self.payment_lag},  modifier: {self.modifier}\n"
         )
@@ -964,15 +964,15 @@
             valid, parsed_args = _check_regular_swap(
                 effective, back_stub, frequency, modifier, eom, roll, calendar
             )
             if valid:  # no front stub is required
                 return True, {
                     "ueffective": parsed_args["ueffective"],
                     "utermination": termination,
-                    "front_stub": None,
+                    "front_stub": NoInput(0),
                     "back_stub": parsed_args["utermination"],
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("FRONT", stub)
@@ -987,15 +987,15 @@
                 front_stub, termination, frequency, modifier, eom, roll, calendar
             )
             if valid:  # no back stub is required
                 return True, {
                     "ueffective": effective,
                     "utermination": parsed_args["utermination"],
                     "front_stub": parsed_args["ueffective"],
-                    "back_stub": None,
+                    "back_stub": NoInput(0),
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
             else:
                 stub_ = _get_default_stub("BACK", stub)
                 back_stub = _get_unadjusted_stub_date(
@@ -1009,30 +1009,30 @@
         )
         if not valid:
             return valid, parsed_args
         else:
             return True, {
                 "ueffective": effective if not dead_front_stub else parsed_args["ueffective"],
                 "utermination": termination if not dead_back_stub else parsed_args["utermination"],
-                "front_stub": parsed_args["ueffective"] if not dead_front_stub else None,
-                "back_stub": parsed_args["utermination"] if not dead_back_stub else None,
+                "front_stub": parsed_args["ueffective"] if not dead_front_stub else NoInput(0),
+                "back_stub": parsed_args["utermination"] if not dead_back_stub else NoInput(0),
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
                 "eom": parsed_args["eom"],
             }
     elif "FRONT" in stub:
         valid, parsed_args = _check_regular_swap(
             effective, termination, frequency, modifier, eom, roll, calendar
         )
         if valid:  # no front stub is required
             return True, {
                 "ueffective": parsed_args["ueffective"],
                 "utermination": parsed_args["utermination"],
-                "front_stub": None,
-                "back_stub": None,
+                "front_stub": NoInput(0),
+                "back_stub": NoInput(0),
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
                 "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("FRONT", stub)
             front_stub = _get_unadjusted_stub_date(
@@ -1048,30 +1048,30 @@
             )
             if not valid:
                 return valid, parsed_args
             else:
                 return True, {
                     "ueffective": effective if not dead_stub else parsed_args["ueffective"],
                     "utermination": parsed_args["utermination"],
-                    "front_stub": parsed_args["ueffective"] if not dead_stub else None,
-                    "back_stub": None,
+                    "front_stub": parsed_args["ueffective"] if not dead_stub else NoInput(0),
+                    "back_stub": NoInput(0),
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
     else:  # schedule is "BACK" sided
         valid, parsed_args = _check_regular_swap(
             effective, termination, frequency, modifier, eom, roll, calendar
         )
         if valid:  # no back stub is required
             return True, {
                 "ueffective": parsed_args["ueffective"],
                 "utermination": parsed_args["utermination"],
-                "front_stub": None,
-                "back_stub": None,
+                "front_stub": NoInput(0),
+                "back_stub": NoInput(0),
                 "roll": parsed_args["roll"],
                 "frequency": parsed_args["frequency"],
                 "eom": parsed_args["eom"],
             }
         else:
             stub_ = _get_default_stub("BACK", stub)
             back_stub = _get_unadjusted_stub_date(
@@ -1087,16 +1087,16 @@
             )
             if not valid:
                 return valid, parsed_args
             else:
                 return True, {
                     "ueffective": parsed_args["ueffective"],
                     "utermination": termination if not dead_stub else parsed_args["utermination"],
-                    "front_stub": None,
-                    "back_stub": parsed_args["utermination"] if not dead_stub else None,
+                    "front_stub": NoInput(0),
+                    "back_stub": parsed_args["utermination"] if not dead_stub else NoInput(0),
                     "roll": parsed_args["roll"],
                     "frequency": parsed_args["frequency"],
                     "eom": parsed_args["eom"],
                 }
 
 
 def _get_default_stub(side: str, stub: str) -> str:
@@ -1269,24 +1269,27 @@
     uback_stub : datetime, optional
         The unadjusted back stub date.
 
     Yields
     ------
     datetime
     """
-    if ufront_stub is None:
+    if ufront_stub is NoInput(0):
         yield from _generate_regular_schedule_unadjusted(
-            ueffective, uback_stub or utermination, frequency, roll
+            ueffective, utermination if uback_stub is NoInput.blank else uback_stub, frequency, roll
         )
     else:
         yield ueffective
         yield from _generate_regular_schedule_unadjusted(
-            ufront_stub, uback_stub or utermination, frequency, roll
+            ufront_stub,
+            utermination if uback_stub is NoInput.blank else uback_stub,
+            frequency,
+            roll,
         )
-    if uback_stub is not None:
+    if uback_stub is not NoInput(0):
         yield utermination
 
 
 def _generate_regular_schedule_unadjusted(
     ueffective: datetime, utermination: datetime, frequency: str, roll: Union[int, str]
 ) -> Iterator[datetime]:
     """
```

### Comparing `rateslib-1.1.1/rateslib/splines/splines.py` & `rateslib-1.2.0/rateslib/splines/splines.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,29 @@
 
        B_{i,1,\\mathbf{t}}(x) = \\left \{ \\begin{matrix} 1, & t_i \leq x < t_{i+1} \\\\ 0, & \\text{otherwise} \end{matrix} \\right .
 
     For continuity on the right boundary the rightmost basic b-spline is also set equal
     to 1 there: :math:`B_{n,1,\\mathbf{t}}(t_{n+k})=1`.
     """
     # Short circuit (positivity and support property)
-    if x < t[i] or x > t[i+k]:
-        return 0.
+    if x < t[i] or x > t[i + k]:
+        return 0.0
 
     org_k = org_k or k  # original_k adds support for derivative recursion
     # Right side endpoint support
     if x == t[-1] and i >= (len(t) - org_k - 1):
-        return 1.
+        return 1.0
 
     # Recursion
     if k == 1:
         if t[i] <= x < t[i + 1]:
-            return 1.
-        return 0.
+            return 1.0
+        return 0.0
     else:
-        left, right = 0., 0.
+        left, right = 0.0, 0.0
         if t[i] != t[i + k - 1]:
             left = (x - t[i]) / (t[i + k - 1] - t[i]) * bsplev_single(x, i, k - 1, t)
         if t[i + 1] != t[i + k]:
             right = (t[i + k] - x) / (t[i + k] - t[i + 1]) * bsplev_single(x, i + 1, k - 1, t)
         return left + right
 
 
@@ -235,20 +235,20 @@
             return False
         for i in range(len(self.t)):
             if self.t[i] != other.t[i]:
                 return False
         for attr in ["k", "n"]:
             if getattr(self, attr, None) != getattr(other, attr, None):
                 return False
-        if self.c is None and other.c is None:
-            return True
-        elif (self.c is None and other.c is not None) or (self.c is not None and other.c is None):
-            return False
-        elif not all(self.c == other.c):
+        if self.c is None or other.c is None:
             return False
+        else:
+            for i in range(len(self.c)):
+                if self.c[i] != other.c[i]:
+                    return False
         return True
 
     def bsplev(self, x, i, otypes=["float64"]):
         """
         Evaluate `x` coordinates on the `i` th B-Spline.
 
         Is the vectorised version of :meth:`bsplev_single`.
@@ -329,15 +329,15 @@
         B_ji = np.zeros(shape=(len(tau), self.n))
         for i in range(self.n):
             B_ji[0, i] = bspldnev_single(tau[0], i, self.k, self.t, left_n)
             B_ji[1:-1, i] = self.bsplev(tau[1:-1], i=i)
             B_ji[-1, i] = bspldnev_single(tau[-1], i, self.k, self.t, right_n)
         return B_ji
 
-    def csolve(self, tau, y, left_n, right_n, allow_lsq=False):
+    def csolve(self, tau, y, left_n, right_n, allow_lsq=False, **kwargs):
         """
         Evaluates and sets the b-spline coefficients, `c`, that parametrise the pp.
 
         Parameters
         ----------
         tau : sequence
             The data sites along the `x` axis which will instruct the pp spline.
@@ -352,14 +352,16 @@
         right_n : int
             The order of function derivative which is supplied for
             the last  value of ``y``. Use `0` if function value is given.
         allow_lsq : bool
             If the number of data sites is greater than the dimension of the pp spline
             this setting allows the coefficients to be solved as a least squares
             problem rather than raising dimensionality exceptions.
+        kwargs : dict
+            Additional keyword args passed to the `dual_solve` linear algebra function.
 
         Returns
         -------
         Sets the class attribute ``c`` : None
 
         Notes
         -----
@@ -383,15 +385,15 @@
                 )
         if len(tau) != len(y):
             raise ValueError(
                 f"`tau` and `y` must have the same length, " f"`tau`: {len(tau)}, `y`: {len(y)}"
             )
         y = np.asarray(y)
         B_ji = self.bsplmatrix(tau, left_n, right_n)
-        c = dual_solve(B_ji, y[:, np.newaxis], allow_lsq=allow_lsq)
+        c = dual_solve(B_ji, y[:, np.newaxis], allow_lsq=allow_lsq, **kwargs)
         self.c = c[:, 0]
         return None
 
     # Licence: Creative Commons - Attribution-NonCommercial-NoDerivatives 4.0 International
     # Commercial use of this code, and/or copying and redistribution is prohibited.
     # Contact rateslib at gmail.com if this code is observed outside its intended sphere.
 
@@ -414,17 +416,15 @@
         The value of the spline at *x* is the sum of the value of each b-spline
         evaluated at *x* multiplied by the spline coefficients, *c*.
 
         .. math::
 
            \\$(x) = \\sum_{i=1}^n c_i B_{(i,k,\\mathbf{t})}(x)
         """
-        _ = np.array([
-            bsplev_single(x, i, self.k, self.t) for i in range(self.n)
-        ])
+        _ = np.array([bsplev_single(x, i, self.k, self.t) for i in range(self.n)])
         return np.dot(_, self.c)
 
     def ppev(self, x):
         """
         Evaluate an array of `x` coordinates on the piecewise polynomial spline.
 
         Is a vectorisation of the :meth:`ppev_single` method.
```

### Comparing `rateslib-1.1.1/tests/test_calendars.py` & `rateslib-1.2.0/tests/test_calendars.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     _get_eom,
     _adjust_date,
     _is_eom,
     _is_imm,
     _is_som,
     _get_imm,
     _get_years_and_months,
+    _dcf_actacticma,
 )
 
 
 @pytest.fixture
 def cal_():
     rules = [Holiday("New Year", month=1, day=3)]
     return create_calendar(rules=rules)
@@ -402,7 +403,25 @@
         (dt(2008, 12, 1), dt(2038, 5, 15), (29, 5)),
     ],
 )
 def test_get_years_and_months(d1, d2, exp):
     result = _get_years_and_months(d1, d2)
     assert result == exp
 
+
+@pytest.mark.parametrize("s, e, t, exp", [
+    (dt(2024, 2, 29), dt(2024, 5, 29), dt(2024, 5, 29), 0.24657534),
+    (dt(2021, 2, 28), dt(2024, 5, 29), dt(2024, 5, 29), 3.24863387),
+    (dt(2021, 2, 28), dt(2024, 5, 29), dt(2026, 5, 28), 3.24657534),
+])
+def test_act_act_icma_z_freq(s, e, t, exp):
+    result = _dcf_actacticma(
+        start=s,
+        end=e,
+        termination=t,
+        frequency_months=1e8,  # Z Frequency
+        stub=False,
+        roll=NoInput(0),
+        calendar=NoInput(0),
+    )
+    assert abs(result-exp)<1e-6
+
```

### Comparing `rateslib-1.1.1/tests/test_curves.py` & `rateslib-1.2.0/tests/test_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from rateslib.default import NoInput
 from rateslib.fx import FXRates, FXForwards
 from rateslib import default_context
 from rateslib.dual import Dual, Dual2, gradient
 from rateslib.calendars import get_calendar
 from rateslib.solver import Solver
 from rateslib.instruments import IRS
+from rateslibrs import index_left_f64
 
 
 @pytest.fixture()
 def curve():
     return Curve(
         nodes={
             dt(2022, 3, 1): 1.00,
@@ -456,15 +457,16 @@
             dt(2026, 1, 1),
             dt(2026, 1, 1),
             dt(2026, 1, 1),
             dt(2026, 1, 1),
         ],
     )
     for i, date in enumerate([dt(2022, 1, 1), dt(2022, 7, 1), dt(2025, 7, 1), dt(2026, 1, 1)]):
-        assert curve[date] == expected[i]
+        result = curve[date]
+        assert (result - expected[i]) < 1e-12
 
 
 @pytest.mark.parametrize("endpoints", [("natural", "bad"), ("bad", "natural")])
 def test_spline_endpoints_raise(endpoints):
     with pytest.raises(NotImplementedError, match="Endpoint method"):
         Curve(
             nodes={
```

### Comparing `rateslib-1.1.1/tests/test_default.py` & `rateslib-1.2.0/tests/test_default.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import pytest
 from pandas import Series
 
 import context
-from rateslib import defaults, default_context
+from rateslib import defaults, default_context, __version__
 from rateslib.instruments import IRS
 from rateslib.curves import Curve
 from rateslib import dt
 
 
+def test_version():
+    assert __version__ == "1.2.0"
+
+
 @pytest.mark.parametrize("name", ["estr", "sonia", "sofr", "swestr", "nowa"])
 def test_fixings(name):
     result = defaults.fixings[name]
     assert isinstance(result, Series)
 
 
 def test_context_raises():
```

### Comparing `rateslib-1.1.1/tests/test_dual.py` & `rateslib-1.2.0/tests/test_dual.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 import pytest
 import math
 import numpy as np
 from packaging import version
+from statistics import NormalDist
 
 import context
+
 from rateslib.dual import (
     Dual,
     Dual2,
     dual_exp,
     dual_log,
     dual_solve,
+    dual_norm_cdf,
+    dual_inv_norm_cdf,
     set_order,
+    gradient,
+    DUAL_CORE_PY,
+)
+
+# Python Dual implementation
+from rateslib.dual.dual import (
     _plu_decomp,
     _pivot_matrix,
-    gradient,
 )
 
 
 @pytest.fixture()
 def x_1():
     return Dual(1, vars=["v0", "v1"], dual=[1, 2])
 
@@ -101,14 +110,15 @@
     result = x_1.__repr__()
     assert result == "<Dual: 1.000000, (v0, v1), [1.0, 2.0]>"
 
     result = y_2.__repr__()
     assert result == "<Dual2: 1.000000, (v0, v1), [1.0, 2.0], [[...]]>"
 
 
+@pytest.mark.skipif(not DUAL_CORE_PY, reason="Rust Dual does not format string in this way.")
 def test_dual_str(x_1, y_2):
     result = x_1.__str__()
     assert result == " val = 1.00000000\n  dv0 = 1.000000\n  dv1 = 2.000000\n"
 
     result = y_2.__str__()
     assert (
         result == " val = 1.00000000\n"
@@ -577,14 +587,67 @@
     ],
 )
 def test_exp(x):
     result = dual_exp(x)
     expected = math.exp(2)
     assert result == expected
 
+@pytest.mark.parametrize(
+    "x",
+    [
+        Dual(1.25, ["x"], []),
+        Dual2(1.25, ["x"], [], []),
+    ],
+)
+def test_norm_cdf(x):
+    result = dual_norm_cdf(x)
+    expected = NormalDist().cdf(1.250)
+    assert abs(result - expected) < 1e-10
+
+    approx_grad = (NormalDist().cdf(1.25001) - NormalDist().cdf(1.25)) * 100000
+    assert abs(gradient(result, ["x"])[0] - approx_grad) < 1e-5
+
+    if isinstance(x, Dual2):
+        approx_grad2 = (NormalDist().cdf(1.25) - NormalDist().cdf(1.24999)) * 100000
+        approx_grad2 = (approx_grad - approx_grad2) * 100000
+        assert abs(gradient(result, ["x"], order=2)[0] - approx_grad2) < 1e-5
+
+
+@pytest.mark.parametrize(
+    "x",
+    [
+        Dual(0.75, ["x"], []),
+        Dual2(0.75, ["x"], [], []),
+    ],
+)
+def test_inv_norm_cdf(x):
+    result = dual_inv_norm_cdf(x)
+    expected = NormalDist().inv_cdf(0.75)
+    assert abs(result - expected) < 1e-10
+
+    approx_grad = (NormalDist().inv_cdf(0.75001) - NormalDist().inv_cdf(0.75)) * 100000
+    assert abs(gradient(result, ["x"])[0] - approx_grad) < 1e-4
+
+    if isinstance(x, Dual2):
+        approx_grad2 = (NormalDist().inv_cdf(0.75) - NormalDist().inv_cdf(0.74999)) * 100000
+        approx_grad2 = (approx_grad - approx_grad2) * 100000
+        assert abs(gradient(result, ["x"], order=2)[0] - approx_grad2) < 1e-4
+
+
+def test_norm_cdf_value():
+    result = dual_norm_cdf(1.0)
+    expected = 0.8413
+    assert abs(result - expected) < 1e-4
+
+
+def test_inv_norm_cdf_value():
+    result = dual_inv_norm_cdf(0.50)
+    expected = 0.0
+    assert abs(result - expected) < 1e-4
+
 
 @pytest.mark.skip(reason="downcast vars is not used within the library, kept only for compat.")
 def test_downcast_vars():
     w = Dual(2, ["x", "y", "z"], [0, 1, 1])
     assert w.__downcast_vars__().vars == ("y", "z")
 
     x = Dual2(2, ["x", "y", "z"], [0, 1, 0], [0, 0, 0, 0, 0, 0, 0, 0, 1])
@@ -610,20 +673,20 @@
         base**exponent
 
 
 def test_keep_manifold_gradient():
     du2 = Dual2(
         10,
         ["x", "y", "z"],
-        dual=np.array([1, 2, 3]),
-        dual2=np.array([[2, 3, 4], [3, 4, 5], [4, 5, 6]]),
+        dual=[1, 2, 3],
+        dual2=[2, 3, 4, 3, 4, 5, 4, 5, 6],
     )
     result = gradient(du2, ["x", "z"], 1, keep_manifold=True)
     expected = np.array(
-        [Dual2(1, ["x", "z"], np.array([4, 8])), Dual2(3, ["x", "z"], np.array([8, 12]))]
+        [Dual2(1, ["x", "z"], [4, 8], []), Dual2(3, ["x", "z"], [8, 12], [])]
     )
     assertions = result == expected
     assert all(assertions)
 
 
 def test_dual_set_order(x_1, y_1):
     assert set_order(x_1, 1) == x_1
@@ -643,27 +706,27 @@
     )
     result, _ = _pivot_matrix(A, method=1)
     expected = np.array(
         [
             [1, 0, 0, 0, 0],
             [0, 1, 0, 0, 0],
             [0, 0, 0, 0, 1],
-            [0, 0, 0, 1, 0],
             [0, 0, 1, 0, 0],
+            [0, 0, 0, 1, 0],
         ]
     )
     assert np.all(result == expected)
     result, _ = _pivot_matrix(A, method=2)
     expected = np.array(
         [
             [1, 0, 0, 0, 0],
             [0, 1, 0, 0, 0],
             [0, 0, 0, 0, 1],
-            [0, 0, 1, 0, 0],
             [0, 0, 0, 1, 0],
+            [0, 0, 1, 0, 0],
         ]
     )
     assert np.all(result == expected)
 
 
 def test_sparse_plu():
     A = np.array(
@@ -706,38 +769,38 @@
     assertions = [abs(diff[i, 0]) < 1e-10 for i in range(A.shape[0])]
     assert all(assertions)
 
 
 def test_solve_lsqrs():
     A = np.array([[0, 1], [1, 1], [2, 1], [3, 1]])
     b = np.array([[-1, 0.2, 0.9, 2.1]]).T
-    result = dual_solve(A, b, allow_lsq=True)
+    result = dual_solve(A, b, allow_lsq=True, types=(float, float))
     assert abs(result[0, 0] - 1.0) < 1e-9
     assert abs(result[1, 0] + 0.95) < 1e-9
 
 
 def test_solve_dual():
     A = np.array([[1, 0], [0, 1]], dtype="object")
     b = np.array([Dual(2, ["x"], np.array([1])), Dual(5, ["x", "y"], np.array([1, 1]))])[
         :, np.newaxis
     ]
-    x = dual_solve(A, b)
+    x = dual_solve(A, b, types=(float, Dual))
     assertions = abs(b - x) < 1e-10
     assert all(assertions)
 
 
 def test_solve_dual2():
     A = np.array([
         [Dual2(1, [], [], []), Dual2(0, [], [], [])],
         [Dual2(0, [], [], []), Dual2(1, [], [], [])]
     ], dtype="object")
     b = np.array([Dual2(2, ["x"], [1], []), Dual2(5, ["x", "y"], [1, 1], [])])[
         :, np.newaxis
     ]
-    x = dual_solve(A, b)
+    x = dual_solve(A, b, types=(Dual2, Dual2))
     assertions = abs(b - x) < 1e-10
     assert all(assertions)
 
 
 def test_sparse_solve(A_sparse):
     b = np.array(
         [0, 0.90929743, 0.14112001, -0.7568025, -0.95892427, -0.2794155, 0.6569866, 0.98935825, 0]
@@ -746,14 +809,15 @@
     x = dual_solve(A_sparse, b)
     x_np = np.linalg.solve(A_sparse, b)
     diff = x - x_np
     assertions = [abs(diff[i, 0]) < 1e-10 for i in range(A_sparse.shape[0])]
     assert all(assertions)
 
 
+@pytest.mark.skipif(not DUAL_CORE_PY, reason="Rust Dual has not implemented Multi-Dim Solve")
 def test_multi_dim_solve():
     A = np.array([[Dual(0.5, [], []), Dual(2, ["y"], [])], [Dual(2.5, ["y"], []), Dual(4, [], [])]])
     b = np.array([[Dual(6.5, [], []), Dual(9, ["z"], [])], [Dual(14.5, ["y"], []), Dual(21, ["z"], [])]])
 
     x = dual_solve(A, b)
     result = np.matmul(A, x).flatten()
     expected = b.flatten()
@@ -886,12 +950,12 @@
         np.float16,
         np.float32,
         np.float64,
         np.longdouble,
     ],
 )
 def test_numpy_dtypes(z, dtype):
-    np.array([1], dtype=dtype) + z
-    z + np.array([1], dtype=dtype)
+    np.array([1, 2], dtype=dtype) + z
+    z + np.array([1, 2], dtype=dtype)
 
     z + dtype(2)
     dtype(2) + z
```

### Comparing `rateslib-1.1.1/tests/test_fx.py` & `rateslib-1.2.0/tests/test_fx.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,16 +332,16 @@
         "eurusd": Curve({dt(2022, 1, 1): 1.0, dt(2022, 1, 3): 0.997}),
         "noknok": Curve({dt(2022, 1, 1): 1.0, dt(2022, 1, 3): 0.996}),
         "nokeur": Curve({dt(2022, 1, 1): 1.0, dt(2022, 1, 3): 0.995}),
     }
     fxf = FXForwards(fx_rates, fx_curves)
     F0_usdeur = 0.9 * 0.997 / 0.999  # f_usdeur * v_eurusd / w_usdusd
     F0_eurnok = 8.888889 * 0.995 / 0.998  # f_eurnok * w_nokeur / v_eureur
-    assert abs(fxf.fx_rates_immediate.fx_array[0, 1].real - F0_usdeur) < 1e-15
-    assert abs(fxf.fx_rates_immediate.fx_array[1, 2].real - F0_eurnok) < 1e-15
+    assert abs(fxf.fx_rates_immediate.fx_array[0, 1].real - F0_usdeur) < 1e-14
+    assert abs(fxf.fx_rates_immediate.fx_array[1, 2].real - F0_eurnok) < 1e-14
 
 
 def test_fxforwards_bad_curves_raises(usdusd, eureur, usdeur):
     bad_curve = Curve({dt(2000, 1, 1): 1.00, dt(2023, 1, 1): 0.99})
     with pytest.raises(ValueError, match="`fx_curves` do not have the same initial"):
         FXForwards(
             FXRates({"usdeur": 0.9}, settlement=dt(2022, 1, 3)),
```

### Comparing `rateslib-1.1.1/tests/test_instruments.py` & `rateslib-1.2.0/tests/test_instruments.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,28 +15,36 @@
     IRS,
     STIRFuture,
     IIRS,
     SBS,
     FXSwap,
     FXExchange,
     Value,
+    VolValue,
     ZCS,
     ZCIS,
     _get_curve_from_solver,
     FRA,
     XCS,
     Portfolio,
     Spread,
     Fly,
+    FXCall,
+    FXPut,
+    FXRiskReversal,
+    FXStraddle,
+    FXStrangle,
+    FXBrokerFly,
     _get_curves_fx_and_base_maybe_from_solver,
 )
-from rateslib.dual import Dual, Dual2
+from rateslib.dual import Dual, Dual2, dual_exp, gradient
 from rateslib.calendars import dcf
-from rateslib.curves import Curve, IndexCurve, LineCurve
+from rateslib.curves import Curve, IndexCurve, LineCurve, MultiCsaCurve, CompositeCurve
 from rateslib.fx import FXRates, FXForwards
+from rateslib.fx_volatility import FXDeltaVolSmile
 from rateslib.solver import Solver
 
 
 @pytest.fixture()
 def curve():
     nodes = {
         dt(2022, 1, 1): 1.00,
@@ -94,15 +102,15 @@
 
 
 class TestCurvesandSolver:
 
     def test_get_curve_from_solver(self):
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
         inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
-        solver = Solver([curve], inst, [0.975])
+        solver = Solver([curve], [], inst, [0.975])
 
         result = _get_curve_from_solver("tagged", solver)
         assert result == curve
 
         result = _get_curve_from_solver(curve, solver)
         assert result == curve
 
@@ -131,15 +139,15 @@
     def test_get_curves_and_fx_from_solver(self, usdusd, usdeur, eureur, solver, fxf, fx, crv):
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
         inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
         fxfs = FXForwards(
             FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3)),
             {"usdusd": usdusd, "usdeur": usdeur, "eureur": eureur},
         )
-        solver = Solver([curve], inst, [0.975], fx=fxfs if fxf else NoInput(0)) if solver else NoInput(0)
+        solver = Solver([curve], [], inst, [0.975], fx=fxfs if fxf else NoInput(0)) if solver else NoInput(0)
         curve = curve if crv else NoInput(0)
 
         if solver is not NoInput(0) and fxf and fx is not NoInput(0):
             with pytest.warns(UserWarning):
                 #  Solver contains an `fx` attribute but an `fx` argument has been supplied
                 crv_result, fx_result, _ = _get_curves_fx_and_base_maybe_from_solver(
                     NoInput(0), solver, curve, fx, NoInput(0), "usd"
@@ -159,20 +167,39 @@
             if fxf:
                 assert fx_result == fxfs
             else:
                 assert fx_result is NoInput(0)
 
         assert crv_result == (curve, curve, curve, curve)
 
+    @pytest.mark.parametrize("obj", [
+        (Curve({dt(2000, 1, 1): 1.0})),
+        (LineCurve({dt(2000, 1, 1): 1.0})),
+        (IndexCurve({dt(2000, 1, 1): 1.0}, index_base=100.0)),
+        (CompositeCurve([Curve({dt(2000, 1, 1): 1.0})])),
+        (MultiCsaCurve([Curve({dt(2000, 1, 1): 1.0})])),
+        (FXDeltaVolSmile(
+            {0.1:1., 0.2:2., 0.5:3., 0.7:4., 0.9:5.},
+            dt(2023, 3, 16),
+            dt(2023, 6, 16),
+            "forward"
+        )),
+    ])
+    def test_get_curves_fx_and_base_maybe_from_solver_object_types(self, obj):
+        crv_result, _, _ = _get_curves_fx_and_base_maybe_from_solver(
+            obj, NoInput(0), NoInput(0), NoInput(0), NoInput(0), NoInput(0)
+        )
+        assert crv_result == (obj,) * 4
+
     def test_get_curves_and_fx_from_solver_raises(self):
         from rateslib.solver import Solver
 
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
         inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
-        solver = Solver([curve], inst, [0.975])
+        solver = Solver([curve], [], inst, [0.975])
 
         with pytest.raises(ValueError, match="`curves` must contain Curve, not str, if"):
             _get_curves_fx_and_base_maybe_from_solver(NoInput(0), NoInput(0), "tagged", NoInput(0), NoInput(0), "")
 
         with pytest.raises(ValueError, match="`curves` must contain str curve `id` s"):
             _get_curves_fx_and_base_maybe_from_solver(NoInput(0), solver, "bad_id", NoInput(0), NoInput(0), "")
 
@@ -181,29 +208,29 @@
 
     @pytest.mark.parametrize("num", [1, 2, 3, 4])
     def test_get_curves_from_solver_multiply(self, num):
         from rateslib.solver import Solver
 
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
         inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
-        solver = Solver([curve], inst, [0.975])
+        solver = Solver([curve], [], inst, [0.975])
         result, _, _ = _get_curves_fx_and_base_maybe_from_solver(
             NoInput(0), solver, ["tagged"] * num, NoInput(0), NoInput(0), ""
         )
         assert result == (curve, curve, curve, curve)
 
     def test_get_proxy_curve_from_solver(self, usdusd, usdeur, eureur):
         # TODO: check whether curves in fxf but not is solver should be allowed???
         curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="tagged")
         inst = [(Value(dt(2023, 1, 1)), ("tagged",), {})]
         fxf = FXForwards(
             FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3)),
             {"usdusd": usdusd, "usdeur": usdeur, "eureur": eureur},
         )
-        solver = Solver([curve], inst, [0.975], fx=fxf)
+        solver = Solver([curve], [], inst, [0.975], fx=fxf)
         curve = fxf.curve("eur", "usd")
         irs = IRS(dt(2022, 1, 1), "3m", "Q")
 
         # test the curve will return even though it is not included within the solver
         # because it is a proxy curve.
         irs.npv(curves=curve, solver=solver)
 
@@ -501,18 +528,17 @@
                 notional=-1e6,
                 # fx_fixing=0.999851,
                 # split_notional=1003052.812,
                 # points=2.523505,
             ),
             FXExchange(
                 settlement=dt(2022, 10, 1),
-                currency="eur",
-                leg2_currency="usd",
-                curves=["eureur", "eureur", "usdusd", "usdusd"],
-                notional=1e6 * 25 / 74.27,
+                pair="eurusd",
+                curves=[None, "eureur", None, "usdusd"],
+                notional=-1e6 * 25 / 74.27,
             ),
         ],
     )
     def test_null_priced_delta(self, inst):
         c1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="usdusd")
         c2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="eureur")
         c3 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.982}, id="eurusd")
@@ -549,15 +575,15 @@
     @pytest.mark.parametrize("inst, param", [
         (IRS(dt(2022, 7, 1), "3M", "A", curves="usdusd"), "fixed_rate"),
         (FRA(dt(2022, 7, 1), "3M", "Q", curves="usdusd"), "fixed_rate"),
         (SBS(dt(2022, 7, 1), "3M", "Q", curves=["usdusd", "usdusd", "eureur", "usdusd"]), "float_spread"),
         (ZCS(dt(2022, 1, 1), "1Y", "Q", curves=["usdusd"]), "fixed_rate"),
         (ZCIS(dt(2022, 1, 1), "1Y", "A", curves=["usdusd", "usdusd", "eu_cpi", "usdusd"]), "fixed_rate"),
         (IIRS(dt(2022, 1, 1), "1Y", "Q", curves=["eu_cpi", "usdusd", "usdusd", "usdusd"]), "fixed_rate"),
-        (FXExchange(dt(2022, 3, 1), currency="usd", leg2_currency="eur", curves=[NoInput(0), "usdusd", NoInput(0), "eurusd"]), "fx_rate")
+        (FXExchange(dt(2022, 3, 1), pair="usdeur", curves=[NoInput(0), "usdusd", NoInput(0), "eurusd"]), "fx_rate")
     ])
     def test_null_priced_delta_round_trip_one_pricing_param(self, inst, param):
         c1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="usdusd")
         c2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="eureur")
         c3 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.982}, id="eurusd")
         c4 = IndexCurve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.995}, id="eu_cpi", index_base=100.0)
         fxf = FXForwards(
@@ -861,14 +887,39 @@
             convention="act360",
             curves=[{"3m": "3m", "6m": "6m"}, "3m"],
             leg2_fixing_method="ibor",
         )
         cashflows = irs.cashflows(solver=solver)
         assert (cashflows.loc[("leg2", 0), "Rate"] - 3.93693) < 1e-4
 
+    def test_no_rfr_fixings_raises(self):
+        # GH 170
+        T_irs = IRS(
+            effective=dt(2020, 12, 15),
+            termination=dt(2037, 12, 15),
+            notional=-600e6,
+            frequency="A",
+            leg2_frequency="A",
+            fixed_rate=4.5,
+            curves="curve"
+        )
+        par_curve = Curve(
+            nodes={
+                dt(2022, 1, 1): 1.0,
+                dt(2023, 1, 1): 1.0,
+                dt(2024, 1, 1): 1.0,
+                dt(2025, 1, 1): 1.0,
+            },
+            id="curve",
+        )
+        with pytest.raises(ValueError, match="RFRs could not be calculated, have you missed"):
+            T_irs.cashflows(curves=par_curve)
+        with pytest.raises(ValueError, match="RFRs could not be calculated, have you missed"):
+            T_irs.npv(curves=par_curve)
+
 
 class TestIIRS:
     def test_index_base_none_populated(self, curve):
         i_curve = IndexCurve(
             {dt(2022, 1, 1): 1.0, dt(2022, 2, 1): 0.5, dt(2034, 1, 1): 0.4},
             index_lag=3,
             index_base=100.0,
@@ -1199,17 +1250,16 @@
             Value(effective=dt(2022, 7, 1), metric="bad").rate(curve)
 
 
 class TestFXExchange:
     def test_cashflows(self):
         fxe = FXExchange(
             settlement=dt(2022, 10, 1),
-            currency="eur",
-            leg2_currency="usd",
-            notional=1e6,
+            pair="eurusd",
+            notional=-1e6,
             fx_rate=2.05,
         )
         result = fxe.cashflows()
         expected = DataFrame(
             {
                 "Type": ["Cashflow", "Cashflow"],
                 "Period": ["Exchange", "Exchange"],
@@ -1231,64 +1281,73 @@
             ("usd", 1.20),
             ("eur", FXRates({"eurusd": 1.20})),
         ],
     )
     def test_npv_rate(self, curve, curve2, base, fx):
         fxe = FXExchange(
             settlement=dt(2022, 3, 1),
-            currency="eur",
-            leg2_currency="usd",
+            pair="eurusd",
             fx_rate=1.2080131682341035,
         )
         if not isinstance(fx, FXRates):
             with pytest.warns(UserWarning):
                 result = fxe.npv([NoInput(0), curve, NoInput(0), curve2], NoInput(0), fx, base, local=False)
         else:
             result = fxe.npv([NoInput(0), curve, NoInput(0), curve2], NoInput(0), fx, base, local=False)
         assert abs(result - 0.0) < 1e-8
 
     def test_rate(self, curve, curve2):
         fxe = FXExchange(
             settlement=dt(2022, 3, 1),
-            currency="eur",
-            leg2_currency="usd",
+            pair="eurusd",
             fx_rate=1.2080131682341035,
         )
         result = fxe.rate([NoInput(0), curve, NoInput(0), curve2], NoInput(0), 1.20)
         expected = 1.2080131682341035
         assert abs(result - expected) < 1e-7
 
     def test_npv_fx_numeric(self, curve):
         # This demonstrates the ambiguity and poor practice of
         # using numeric fx as pricing input, although it will return.
         fxe = FXExchange(
             settlement=dt(2022, 3, 1),
-            currency="eur",
-            leg2_currency="usd",
+            pair="eurusd",
             fx_rate=1.2080131682341035,
+            notional=-1e6,
         )
         # result_ = fxe.npv([curve] * 4, fx=2.0, local=True)
         with pytest.warns(UserWarning):
             result = fxe.npv([curve] * 4, fx=2.0)
             expected = -993433.103425 * 2.0 + 1200080.27069
             assert abs(result - expected) < 1e-5
 
         # with pytest.raises(ValueError, match="Cannot calculate `npv`"):
         #     fxe.npv([curve] * 4, fx=2.0, base="bad")
 
     def test_npv_no_fx_raises(self, curve):
         fxe = FXExchange(
             settlement=dt(2022, 3, 1),
-            currency="eur",
-            leg2_currency="usd",
+            pair="eurusd",
             fx_rate=1.2080131682341035,
         )
         with pytest.raises(ValueError, match="Must have some FX info"):
             fxe.npv(curve)
 
+    def test_notional_direction(self, curve, curve2):
+        fx1 = FXExchange(notional=1e6, pair="eurusd", settlement=dt(2022, 1, 1), fx_rate=1.20)
+        fx2 = FXExchange(notional=-1e6, pair="eurusd", settlement=dt(2022, 1, 1), fx_rate=1.30)
+        pf = Portfolio([fx1, fx2])
+        fx= FXRates({"eurusd": 1.30}, base="usd")
+        result = pf.npv(curves=[None, curve, None, curve2], fx=fx)
+        expected = 100000.0
+        assert abs(result - expected) < 1e-8
+        result = pf.npv(curves=[None, curve, None, curve2], fx=fx, base="eur")
+        expected = 100000.0 / 1.30
+        assert abs(result - expected) < 1e-8
+
 
 # test the commented out FXSwap variant
 # def test_fx_swap(curve, curve2):
 #     fxs = FXSwap(dt(2022, 1, 15), "3M", notional=1000, fx_fixing_points=(10.1, 105),
 #                  currency="eur", leg2_currency="sek")
 #     assert len(fxs.leg1.periods) == 2
 #     assert len(fxs.leg2.periods) == 2
@@ -2115,14 +2174,41 @@
             notional=1e6,
         )
         expected = fxf.swap("usdnok", [dt(2022, 2, 1), dt(2022, 10, 1)])
         result = fxs.rate([NoInput(0), curve, NoInput(0), curve2], NoInput(0), fxf)
         assert abs(result-expected) < 1e-10
         assert np.isclose(result.dual, expected.dual)
 
+    def test_fxswap_pair_arg(self, curve, curve2):
+        fxf = FXForwards(
+            FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            pair="usdnok",
+            payment_lag=0,
+            notional=1e6,
+        )
+        expected = fxf.swap("usdnok", [dt(2022, 2, 1), dt(2022, 10, 1)])
+        result = fxs.rate([NoInput(0), curve, NoInput(0), curve2], NoInput(0), fxf)
+        assert abs(result-expected) < 1e-10
+        assert np.isclose(result.dual, expected.dual)
+
+    def test_currency_arg_pair_overlap(self):
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            pair="usdnok",
+            currency="jpy",
+        )
+        assert fxs.leg1.currency == "usd"
+
+
     def test_fxswap_npv(self, curve, curve2):
         fxf = FXForwards(
             FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
             {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
         )
         fxs = FXSwap(
             dt(2022, 2, 1),
@@ -2267,14 +2353,64 @@
     #                         currency="usd", leg2_currency="nok",
     #                         payment_lag_exchange=0, notional=1e6,
     #                         leg2_fixed_rate=-1.0)
     #     npv_nok = fxs.npv([NoInput(0), fxf.curve("usd", "nok"), NoInput(0), curve2], NoInput(0), fxf)
     #     npv_usd = fxs.npv([NoInput(0), curve, NoInput(0), fxf.curve("nok", "usd")], NoInput(0), fxf)
     #     assert abs(npv_nok-npv_usd) < 1e-7  # npvs are equivalent becasue xcs basis =0
 
+    def test_transition_from_dual_to_dual2(self, curve, curve2):
+        # Test added for BUG, see PR: XXX
+        fxf = FXForwards(
+            FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxf._set_ad_order(1)
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag=0,
+            notional=1e6,
+        )
+        fxs.npv(
+            curves=[None, fxf.curve("usd", "usd"), None, fxf.curve("nok", "usd")],
+            fx=fxf
+        )
+        fxf._set_ad_order(2)
+        fxs.npv(
+            curves=[None, fxf.curve("usd", "usd"), None, fxf.curve("nok", "usd")],
+            fx=fxf
+        )
+
+    def test_transition_from_dual_to_dual2_rate(self, curve, curve2):
+        # Test added for BUG, see PR: XXX
+        fxf = FXForwards(
+            FXRates({"usdnok": 10}, settlement=dt(2022, 1, 3)),
+            {"usdusd": curve, "nokusd": curve2, "noknok": curve2},
+        )
+        fxf._set_ad_order(1)
+        fxs = FXSwap(
+            dt(2022, 2, 1),
+            "8M",
+            currency="usd",
+            leg2_currency="nok",
+            payment_lag=0,
+            notional=1e6,
+        )
+        fxs.rate(
+            curves=[None, fxf.curve("usd", "usd"), None, fxf.curve("nok", "usd")],
+            fx=fxf
+        )
+        fxf._set_ad_order(2)
+        fxs.rate(
+            curves=[None, fxf.curve("usd", "usd"), None, fxf.curve("nok", "usd")],
+            fx=fxf
+        )
+
 
 class TestSTIRFuture:
     def test_stir_rate(self, curve, curve2):
         stir = STIRFuture(
             effective=dt(2022, 3, 16),
             termination=dt(2022, 6, 15),
             spec="usd_stir",
@@ -2891,16 +3027,16 @@
     DataFrame([0.0],
               index=Index([dt(2022, 1, 15)], name="payment"),
               columns=MultiIndex.from_tuples([("EUR", "eur")],
                                              names=["local_ccy", "collateral_ccy"])
               )
     ),
     (
-    FXExchange(dt(2022, 1, 15), currency="eur", leg2_currency="usd", curves=["eureur", "eureur", "usdusd", "usdeur"]),
-    DataFrame([[-1000000.0, 1101072.93429]],
+    FXExchange(dt(2022, 1, 15), pair="eurusd", curves=["eureur", "eureur", "usdusd", "usdeur"]),
+    DataFrame([[1000000.0, -1101072.93429]],
               index=Index([dt(2022, 1, 15)], name="payment"),
               columns=MultiIndex.from_tuples([("EUR", "eur"), ("USD", "eur")],
                                              names=["local_ccy", "collateral_ccy"])
               )
     ),
     (
     XCS(dt(2022, 1, 5), "3M", "M", currency="eur", leg2_currency="usd", curves=["eureur", "eurusd", "usdusd", "usdusd"]),
@@ -2975,7 +3111,1159 @@
     )
     irs_mkt = IRS(
         dt(2023, 8, 1), "1Y", "Q", curves="usd", fixed_rate=2.0, notional=999556779.81,
     )
     result = irs_mkt.cashflows_table(solver=solver)
     assert abs(result.iloc[0, 0] - 69.49810) < 1e-5
     assert abs(result.iloc[3, 0] - 69.49810) < 1e-5
+
+
+@pytest.fixture()
+def fxfo():
+    # FXForwards for FX Options tests
+    eureur = Curve(
+        {dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.9851909811629752}, calendar="tgt", id="eureur"
+    )
+    usdusd = Curve(
+        {dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.976009366603271}, calendar="nyc", id="usdusd"
+    )
+    eurusd = Curve(
+        {dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.987092591908283}, id="eurusd"
+    )
+    fxr = FXRates({"eurusd": 1.0615}, settlement=dt(2023, 3, 20))
+    fxf = FXForwards(
+        fx_curves={"eureur": eureur, "eurusd": eurusd, "usdusd": usdusd},
+        fx_rates=fxr
+    )
+    # fxf.swap("eurusd", [dt(2023, 3, 20), dt(2023, 6, 20)]) = 60.10
+    return fxf
+
+
+class TestFXOptions:
+
+    # Bloomberg tests replicate https://quant.stackexchange.com/a/77802/29443
+    @pytest.mark.parametrize("pay, k, exp_pts, exp_prem, dlty, exp_dl", [
+        (dt(2023, 3, 20), 1.101, 69.378, 138756.54, "spot", 0.250124),
+        (dt(2023, 3, 20), 1.101, 69.378, 138756.54, "forward", 0.251754),
+        (dt(2023, 6, 20), 1.101, 70.226, 140451.53, "spot", 0.250124),  # BBG 0.250126
+        (dt(2023, 6, 20), 1.101, 70.226, 140451.53, "forward", 0.251754),  # BBG 0.251756
+        (dt(2023, 6, 20), 1.10101922, 70.180, 140360.17, "spot", 0.250000),
+    ])
+    @pytest.mark.parametrize("smile", [True, False])
+    def test_bbg_usd_pips(self, fxfo, pay, k, exp_pts, exp_prem, dlty, exp_dl, smile):
+        vol = FXDeltaVolSmile(
+            {
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            id="vol",
+            ad=1,
+        )
+        vol = vol if smile else 8.90
+        fxc = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            strike=k,
+            payment_lag=pay,
+            delivery_lag=2,
+            calendar="tgt",
+            modifier="mf",
+            premium_ccy="usd",
+            delta_type=dlty,
+        )
+        result = fxc.rate(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=vol,
+        )
+        assert abs(result - exp_pts) <1e-3
+
+        result = fxc.rate(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=vol,
+            metric="premium"
+        )
+        assert abs(result - exp_prem) <1e-2
+
+    @pytest.mark.parametrize("pay, k, exp_pts, exp_prem, dlty, exp_dl", [
+        (dt(2023, 3, 20), 1.101, 0.6536, 130717.44, "spot", 0.243588),
+        (dt(2023, 3, 20), 1.101, 0.6536, 130717.44, "forward", 0.245175),
+        (dt(2023, 6, 20), 1.101, 0.6578, 131569.29, "spot", 0.243548),
+        (dt(2023, 6, 20), 1.101, 0.6578, 131569.29, "forward", 0.245178),
+    ])
+    @pytest.mark.parametrize("smile", [False, True])
+    def test_premium_bbg_eur_pc(self, fxfo, pay, k, exp_pts, exp_prem, dlty, exp_dl, smile):
+        vol_ = 8.9 if not smile else FXDeltaVolSmile(
+            nodes={0.5: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type=dlty,
+        )
+        fxo = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=pay,
+            strike=k,
+            notional=20e6,
+            delta_type=dlty,
+            premium_ccy="eur",
+        )
+        result = fxo.rate(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=vol_,
+        )
+        expected = exp_pts
+        assert abs(result - expected) < 1e-3
+
+        result = 20e6 * result / 100
+        expected = exp_prem
+        assert abs(result - expected) < 1e-1
+
+    def test_fx_call_npv_unpriced(self, fxfo):
+        fxo = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=1.101,
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.npv(curves, fx=fxfo, vol=8.9)
+        expected = 0.0
+        assert abs(result - expected) < 1e-6
+
+    def test_fx_call_rate_specified_strike(self, fxfo):
+        fxo = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=1.101,
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=8.9)
+        expected = 70.225764
+        assert abs(result - expected) < 1e-6
+
+    @pytest.mark.parametrize("ccy, exp_rate, exp_strike", [
+        ("usd", 70.180131, 1.10101920113408469),
+        ("eur", 0.680949, 1.099976),
+    ])
+    @pytest.mark.parametrize("smile", [True, False])
+    def test_fx_call_rate_delta_strike(self, fxfo, ccy, exp_rate, exp_strike, smile):
+        vol = FXDeltaVolSmile(
+            {
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            id="vol",
+            ad=1,
+        )
+        vol = vol if smile else 8.90
+        fxo = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike="25d",
+            delta_type="spot",
+            premium_ccy=ccy,
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+        expected = exp_rate
+        assert abs(result - expected) < 1e-6
+        assert abs(fxo.periods[0].strike - exp_strike) < 1e-4
+
+    def test_fx_call_rate_expiry_tenor(self, fxfo):
+        fxo = FXCall(
+            pair="eurusd",
+            expiry="3m",
+            eval_date=dt(2023, 3, 16),
+            modifier="mf",
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=dt(2023, 6, 20),
+            calendar="tgt",
+            strike="25d",
+            delta_type="spot",
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=8.9)
+        expected = 70.180131
+        assert abs(result - expected) < 1e-6
+
+    def test_fx_call_plot_payoff(self, fxfo):
+        fxc = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            strike=1.101,
+            premium=0.0,
+        )
+        result = fxc.plot_payoff(
+            [1.03, 1.12],
+            fx=fxfo,
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        )
+        x, y = result[2][0]._x, result[2][0]._y
+        assert x[0] == 1.03
+        assert x[1000] == 1.12
+        assert y[0] == 0.0
+        assert y[1000] == (1.12 - 1.101) * 20e6
+
+    def test_fx_put_rate(self, fxfo):
+        fxo = FXPut(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike="-25d",
+            delta_type="spot",
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=10.15)
+        expected = 83.975596
+        assert abs(result - expected) < 1e-6
+
+    def test_str_tenor_raises(self):
+        with pytest.raises(ValueError, match="`expiry` as string tenor requires `eval_date`"):
+            FXCall(
+                pair="eurusd",
+                expiry="3m",
+            )
+
+    def test_premium_ccy_raises(self):
+        with pytest.raises(ValueError, match="`premium_ccy`: 'chf' must be one of option currency pair"):
+            FXCall(
+                pair="eurusd",
+                expiry="3m",
+                eval_date=dt(2023, 3, 16),
+                premium_ccy="chf",
+            )
+
+    @pytest.mark.parametrize("dlty", [("forward")])
+    def test_call_put_parity_50d(self, fxfo, dlty):
+        fxp = FXPut(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike="-50d",
+            premium_ccy="usd",
+            delta_type=dlty
+        )
+        fxc = FXCall(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike="50d",
+            premium_ccy="usd",
+            delta_type=dlty
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        assert abs(fxc.analytic_greeks(curves, fx=fxfo, vol=10.0)["delta"] - 0.5) < 1e-14
+        assert abs(fxc.periods[0].strike - 1.068856) < 1e-6
+        assert abs(fxp.analytic_greeks(curves, fx=fxfo, vol=10.0)["delta"] + 0.5) < 1e-14
+        assert abs(fxp.periods[0].strike - 1.068856) < 1e-6
+
+    def test_analytic_vega(self, fxfo):
+        fxo = FXCall(
+            pair="eurusd",
+            expiry="3m",
+            eval_date=dt(2023, 3, 16),
+            modifier="mf",
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=dt(2023, 3, 16),
+            calendar="tgt",
+            strike=1.101,
+            delta_type="spot",
+        )
+        result = fxo.analytic_greeks(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=8.9,
+        )["vega"]
+        # see test_periods/test_analytic_vega
+        assert abs(result * 20e6 / 100 - 33757.945) < 1e-2  # BBG validation gives 33775.78 $
+
+    def test_rate_vol_raises(self, fxfo):
+        args = {
+            "expiry": dt(2009, 6, 16),
+            "pair": "eurusd",
+            "curves": [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            "delta_type": "spot",
+        }
+        vol = FXDeltaVolSmile(
+            {0.75: 8.9},
+            eval_date=dt(2009, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            id="vol",
+            ad=1,
+        )
+        fxc = FXCall(strike=1.10, **args, notional=100e6, vol=vol)
+        with pytest.raises(ValueError, match="The `eval_date` on the FXDeltaVolSmile and the"):
+            fxc.rate(fx=fxfo)
+
+    @pytest.mark.parametrize("phi", [-1.0, 1.0])
+    @pytest.mark.parametrize("prem_ccy", ["usd", "eur"])
+    @pytest.mark.parametrize("dt_0", ["spot", "forward"])
+    @pytest.mark.parametrize("dt_1", ["spot", "forward", "spot_pa", "forward_pa"])
+    @pytest.mark.parametrize("smile", [True, False])
+    def test_atm_rates(self, fxfo, phi, prem_ccy, smile, dt_0, dt_1):
+        FXOp = FXCall if phi > 0 else FXPut
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type=dt_1,
+            id="vol",
+        )
+        vol = fxvs if smile else 9.50
+        fxo = FXOp(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type=dt_0,
+            vol=vol,
+            premium_ccy=prem_ccy,
+            strike="atm_delta",
+        )
+        result = fxo.analytic_greeks(fx=fxfo)
+
+        f_d = fxfo.rate("eurusd", dt(2023, 6, 20))
+        eta = 0.5 if prem_ccy == "usd" else -0.5
+        expected = f_d * dual_exp(result["__vol"]**2 * fxvs.t_expiry * eta)
+        assert abs(result["__strike"] - expected) < 1e-8
+
+    @pytest.mark.parametrize("phi", [1.0, -1.0])
+    def test_traded_option_rate_vol(self, fxfo, phi):
+        FXOp = FXCall if phi > 0 else FXPut
+        fxo = FXOp(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="spot",
+            premium_ccy="usd",
+            strike=1.05,
+            premium=100000.0,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+        )
+        result = fxo.rate(
+            curves=[None, fxfo.curve("eur", "usd", None, fxfo.curve("usd", "usd"))],
+            vol=fxvs,
+            fx=fxfo,
+            metric="vol",
+        )
+        expected = 8.899854
+        assert abs(result - expected) < 1e-6
+
+    def test_option_strike_premium_validation(self):
+        with pytest.raises(ValueError, match="`strike` for FXOption must be set"):
+            FXCall(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+            )
+
+        with pytest.raises(ValueError, match="FXOption with string delta as `strike` cannot be"):
+            FXCall(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+                strike="25d",
+                premium= 0.0
+            )
+
+    @pytest.mark.parametrize("notn, expected, phi",[
+        (1e6, [0.5, 500000], 1.0),
+        (2e6, [0.5, 1000000], 1.0),
+        (-2e6, [0.5, 1000000], 1.0),
+        (1e6, [-0.5, -500000], -1.0),
+        (2e6, [-0.5, -1000000], -1.0),
+        (-2e6, [-0.5, -1000000], -1.0),
+    ])
+    def test_greeks_delta_direction(self, fxfo, notn, expected, phi):
+        # test the delta and delta_eur are not impacted by a Buy or Sell. Delta is expressed relative to a Buy.
+        FXOp = FXCall if phi > 0 else FXPut
+        delta = f"{'-' if phi < 0 else ''}50d"
+        fxo = fxo = FXOp(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="forward",
+            premium_ccy="usd",
+            strike=delta,
+            notional=notn,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        result = fxo.analytic_greeks(curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")], vol=fxvs, fx=fxfo)
+        assert abs(result["delta"] - expected[0]) < 1e-6
+        assert abs(result["delta_eur"] - expected[1]) < 1e-6
+
+
+class TestRiskReversal:
+    @pytest.mark.parametrize("metric, expected", [
+        ("pips_or_%", -13.795465), ("vol", -1.25), ("premium", -27590.930533),
+    ])
+    def test_risk_reversal_rate_metrics(self, fxfo, metric, expected):
+        fxo = FXRiskReversal(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=["-25d", "25d"],
+            delta_type="spot",
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=[10.15, 8.9], metric=metric)
+        assert abs(result - expected) < 1e-6
+
+    @pytest.mark.parametrize("prem, prem_ccy, local, exp", [
+        ((NoInput(0), NoInput(0)), NoInput(0), False, 0.0),
+        ((NoInput(0), NoInput(0)), "eur", False, 0.0),
+        ((-167500.0, 140500.0), "usd", False, -219.590678),
+        ((-167500/1.06751, 140500/1.06751), "eur", False, -219.590678),
+        ((-167500/1.06751, 140500/1.06751), "eur", True, {"eur": 25121.646, "usd": -26879.673}),
+    ])
+    def test_risk_reversal_npv(self, fxfo, prem, prem_ccy, local, exp):
+        fxo = FXRiskReversal(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=[1.033, 1.101],
+            premium=prem,
+            premium_ccy=prem_ccy,
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.npv(curves, fx=fxfo, vol=[10.15, 8.9], local=local)
+        expected = exp
+        if not local:
+            assert abs(result - expected) < 1e-6
+        else:
+            for k in expected:
+                assert abs(result[k]-expected[k]) < 1e-3
+
+    def test_risk_reversal_plot(self, fxfo):
+        fxo = FXRiskReversal(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=[1.033, 1.101],
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.plot_payoff([1.03, 1.12], curves, fx=fxfo, vol=[10.15, 8.9])
+        x, y = result[2][0]._x, result[2][0]._y
+        assert x[0] == 1.03
+        assert x[1000] == 1.12
+        assert abs(y[0] + (1.033 - 1.03) * 20e6 ) < 1e-5
+        assert abs(y[1000] - (1.12-1.101) * 20e6) < 1e-5
+
+    def test_rr_strike_premium_validation(self):
+        with pytest.raises(ValueError, match="`strike` for FXRiskReversal must be set"):
+            FXRiskReversal(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+            )
+
+        with pytest.raises(ValueError, match="FXRiskReversal with string delta as `strike` cannot"):
+            FXRiskReversal(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+                strike=["25d", "35d"],
+                premium=[NoInput(0), 1.0],
+            )
+
+    @pytest.mark.parametrize("notn, expected_grks, expected_ccy",[
+        (1e6, [0.5, -1.329654, -0.035843], [500000, -14194.192533, -358.428628]),
+        (2e6, [0.5, -1.329654, -0.035843], [1000000, -28388.384, -716.8572]),
+        (-2e6, [0.5, -1.329654, -0.035843], [1000000, -28388.384, -716.8572]),
+    ])
+    def test_greeks_delta_direction(self, fxfo, notn, expected_grks, expected_ccy):
+        # test the delta and delta_eur are not impacted by a Buy or Sell. Delta is expressed relative to a Buy.
+        fxo = FXRiskReversal(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="forward",
+            premium_ccy="usd",
+            strike=["-30d", "20d"],
+            notional=notn,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        result = fxo.analytic_greeks(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            vol=fxvs,
+            fx=fxfo
+        )
+        assert abs(result["delta"] - expected_grks[0]) < 1e-6
+        assert abs(result["gamma"] - expected_grks[1]) < 1e-6
+        assert abs(result["vega"] - expected_grks[2]) < 1e-6
+
+        assert abs(result["delta_eur"] - expected_ccy[0]) < 1e-2
+        assert abs(result["gamma_eur_1%"] - expected_ccy[1]) < 1e-2
+        assert abs(result["vega_usd"] - expected_ccy[2]) < 1e-2
+
+
+class TestFXStraddle:
+
+    @pytest.mark.parametrize("dlty, strike, ccy, exp", [
+        # ("forward", ["50d", "-50d"], "usd", [1.068856203, 1.068856203]),
+        # ("spot", ["50d", "-50d"], "usd", [1.06841799, 1.069294591]),
+        ("spot", "atm_forward", "usd", [1.06750999, 1.06750999]),
+        ("spot", "atm_spot", "usd", [1.061500, 1.061500]),
+        ("forward", "atm_delta", "usd", [1.068856203, 1.068856203]),
+        ("spot", "atm_delta", "usd", [1.068856203, 1.068856203]),
+        ("spot", "atm_forward", "eur", [1.06750999, 1.06750999]),
+        ("spot", "atm_spot", "eur", [1.061500, 1.061500]),
+        ("forward", "atm_delta", "eur", [1.06616549, 1.06616549]),
+        ("spot", "atm_delta", "eur", [1.06616549, 1.06616549]),
+        # ("forward", ["50d", "-50d"], "eur", [1.0660752074, 1.06624508149]),  # pa strikes
+        # ("spot", ["50d", "-50d"], "eur", [1.0656079102, 1.066656812]),  # pa strikes
+    ])
+    @pytest.mark.parametrize("smile", [True, False])
+    def test_straddle_strikes(self, fxfo, dlty, strike, ccy, exp, smile):
+        fxvs = FXDeltaVolSmile(
+            nodes={0.5: 10.0},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        vol_ = fxvs if smile else 10.0
+        fxo = FXStraddle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=strike,
+            premium_ccy=ccy,
+            delta_type=dlty
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.npv(curves, fx=fxfo, vol=vol_)
+        call_k = fxo.periods[0].periods[0].strike
+        put_k = fxo.periods[1].periods[0].strike
+        assert abs(call_k - exp[0]) < 1e-7
+        assert abs(put_k - exp[1]) < 1e-7
+
+    @pytest.mark.parametrize("metric, expected", [
+        ("pips_or_%", 337.998151), ("vol", 7.9), ("premium", 675996.301147),
+    ])
+    def test_straddle_rate_metrics(self, fxfo, metric, expected):
+        fxo = FXStraddle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike="atm_delta",
+            delta_type="spot",
+        )
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=7.9, metric=metric)
+        assert abs(result - expected) < 1e-6
+
+    def test_strad_strike_premium_validation(self):
+        with pytest.raises(ValueError, match="`strike` for FXStraddle must be set"):
+            FXStraddle(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+            )
+
+        with pytest.raises(ValueError, match="FXStraddle with string delta as `strike` cannot"):
+            FXStraddle(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+                strike="25d",
+                premium=[NoInput(0), 1.0],
+            )
+
+    @pytest.mark.parametrize("notn, expected_grks, expected_ccy", [
+        (1e6, [0.0, 19.086488, 0.422238], [0, 203750.1688, 4222.379]),
+        (2e6, [0.0, 19.086488,  0.422238], [0, 407500.336, 8444.758]),
+        (-2e6, [0.0, 19.086488,  0.422238], [0, 407500.336, 8444.758]),
+    ])
+    def test_greeks_delta_direction(self, fxfo, notn, expected_grks, expected_ccy):
+        # test the delta and delta_eur are not impacted by a Buy or Sell. Delta is expressed relative to a Buy.
+        fxo = FXStraddle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="forward",
+            premium_ccy="usd",
+            strike="atm_delta",
+            notional=notn,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        result = fxo.analytic_greeks(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            vol=fxvs,
+            fx=fxfo
+        )
+        assert abs(result["delta"] - expected_grks[0]) < 1e-6
+        assert abs(result["gamma"] - expected_grks[1]) < 1e-6
+        assert abs(result["vega"] - expected_grks[2]) < 1e-6
+
+        assert abs(result["delta_eur"] - expected_ccy[0]) < 1e-2
+        assert abs(result["gamma_eur_1%"] - expected_ccy[1]) < 1e-2
+        assert abs(result["vega_usd"] - expected_ccy[2]) < 1e-2
+
+
+class TestFXStrangle:
+
+    @pytest.mark.parametrize("strike, ccy", [
+        ([1.02, 1.10], "usd"),
+        (["-20d", "20d"], "usd"),
+        ([1.02, 1.10], "eur"),
+        (["-20d", "20d"], "eur"),
+    ])
+    @pytest.mark.parametrize("smile", [True, False])
+    @pytest.mark.parametrize("delta_type", ["forward", "spot_pa"])
+    def test_strangle_rate(self, fxfo, delta_type, strike, ccy, smile):
+        # test pricing a straddle with vol 10.0 returns 10.0
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=strike,
+            premium_ccy=ccy,
+            delta_type="forward",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.9,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type=delta_type,
+        )
+        vol = fxvs if smile else 10.0
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        premium = fxo.rate(curves, fx=fxfo, vol=result, metric="pips_or_%")
+        metric = "pips" if ccy == "usd" else "percent"
+        premium_vol = fxo.periods[0].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol, metric=metric,
+        )
+        premium_vol += fxo.periods[1].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol, metric=metric,
+        )
+        assert abs(premium - premium_vol) < 5e-2
+
+    def test_strangle_rate_strike_str(self, fxfo):
+        # test pricing a strangle with delta as string that is not a delta percent should fail?
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=["atm_spot", "atm_forward"],
+            premium_ccy="eur",
+            delta_type="forward",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.9,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            ad=1
+        )
+        vol = fxvs
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        premium = fxo.rate(curves, fx=fxfo, vol=result, metric="pips_or_%")
+        metric = "percent"
+        premium_vol = fxo.periods[0].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol, metric=metric,
+        )
+        premium_vol += fxo.periods[1].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol, metric=metric,
+        )
+        assert abs(premium - premium_vol) < 5e-2
+
+    def test_strangle_rate_ad(self, fxfo):
+        # test pricing a strangle with delta as string that is not a delta percent should fail?
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=["atm_spot", "atm_forward"],
+            premium_ccy="eur",
+            delta_type="forward",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.9,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            ad=1,
+            id="vol"
+        )
+        vol = fxvs
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        #test fwd diff
+        m_ = {
+            0: [10.151, 7.9, 8.9],
+            1: [10.15, 7.901, 8.9],
+            2: [10.15, 7.9, 8.901],
+        }
+        for i in range(3):
+            fxvs2 = FXDeltaVolSmile(
+                nodes={
+                    0.25: m_[i][0],
+                    0.50: m_[i][1],
+                    0.75: m_[i][2],
+                },
+                eval_date=dt(2023, 3, 16),
+                expiry=dt(2023, 6, 16),
+                delta_type="spot",
+                ad=1,
+                id="vol"
+            )
+            result2 = fxo.rate(curves, fx=fxfo, vol=fxvs2)
+            fwd_diff = (result2 - result) * 1000.0
+            assert abs(fwd_diff - gradient(result, [f"vol{i}"])[0]) < 1e-4
+
+    def test_strangle_rate_ad2(self, fxfo):
+        # test pricing a strangle with delta as string that is not a delta percent should fail?
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=["atm_spot", "atm_forward"],
+            premium_ccy="eur",
+            delta_type="forward",
+        )
+        fxfo._set_ad_order(2)
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.9,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+            ad=2,
+            id="vol"
+        )
+        vol = fxvs
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        #test fwd diff
+        m_ = {
+            0: [10.151, 7.9, 8.9],
+            1: [10.15, 7.901, 8.9],
+            2: [10.15, 7.9, 8.901],
+        }
+        n_ = {
+            0: [10.149, 7.9, 8.9],
+            1: [10.15, 7.899, 8.9],
+            2: [10.15, 7.9, 8.899],
+        }
+        for i in range(3):
+            fxvs2 = FXDeltaVolSmile(
+                nodes={
+                    0.25: m_[i][0],
+                    0.50: m_[i][1],
+                    0.75: m_[i][2],
+                },
+                eval_date=dt(2023, 3, 16),
+                expiry=dt(2023, 6, 16),
+                delta_type="spot",
+                ad=2,
+                id="vol"
+            )
+            result_plus = fxo.rate(curves, fx=fxfo, vol=fxvs2)
+            fxvs3 = FXDeltaVolSmile(
+                nodes={
+                    0.25: n_[i][0],
+                    0.50: n_[i][1],
+                    0.75: n_[i][2],
+                },
+                eval_date=dt(2023, 3, 16),
+                expiry=dt(2023, 6, 16),
+                delta_type="spot",
+                ad=2,
+                id="vol"
+            )
+            result_min = fxo.rate(curves, fx=fxfo, vol=fxvs3)
+
+            fwd_diff = (result_plus + result_min - 2 * result) * 1000000.0
+            assert abs(fwd_diff - gradient(result, [f"vol{i}"], order=2)[0][0]) < 1e-4
+
+    def test_strangle_rate_2vols(self, fxfo):
+        # test pricing a straddle with vol [8.0, 10.0] returns a valid value close to 9.0
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=20e6,
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=["-25d", "25d"],
+            premium_ccy="usd",
+            delta_type="forward",
+        )
+        vol = [8.0, 10.0]
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        premium = fxo.rate(curves, fx=fxfo, vol=result, metric="pips_or_%")
+        premium_vol = fxo.periods[0].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol[0],
+        )
+        premium_vol += fxo.periods[1].periods[0].rate(
+            fxfo.curve("eur", "usd"), fxfo.curve("usd", "usd"), fx=fxfo, vol=vol[1],
+        )
+
+        assert abs(premium - premium_vol) < 5e-2
+
+    @pytest.mark.parametrize("notn, expected_grks, expected_ccy", [
+        (1e6, [-0.026421, 10.217464, 0.294607], [-26421.048, 109072.493, 2946.066]),
+        (2e6, [-0.026421, 10.217464, 0.294607], [-52842.096, 218144.986, 5892.132]),
+        (-2e6, [-0.026421, 10.217464, 0.294607],  [-52842.096, 218144.986, 5892.132]),
+    ])
+    @pytest.mark.parametrize("strikes", [("-20d", "20d"), (1.0238751229, 1.115919333)])
+    def test_greeks_delta_direction(self, fxfo, notn, expected_grks, expected_ccy, strikes):
+        # test the delta and delta_eur are not impacted by a Buy or Sell. Delta is expressed relative to a Buy.
+        fxo = FXStrangle(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="forward",
+            premium_ccy="usd",
+            strike=strikes,
+            notional=notn,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        result = fxo.analytic_greeks(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            vol=fxvs,
+            fx=fxfo
+        )
+        assert abs(result["delta"] - expected_grks[0]) < 1e-6
+        assert abs(result["gamma"] - expected_grks[1]) < 1e-6
+        assert abs(result["vega"] - expected_grks[2]) < 1e-6
+
+        assert abs(result["delta_eur"] - expected_ccy[0]) < 1e-1
+        assert abs(result["gamma_eur_1%"] - expected_ccy[1]) < 1e-1
+        assert abs(result["vega_usd"] - expected_ccy[2]) < 1e-1
+
+    def test_strang_strike_premium_validation(self):
+        with pytest.raises(ValueError, match="`strike` for FXStrangle must be set"):
+            FXStrangle(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+                strike=["25d", NoInput(0)],
+            )
+
+        with pytest.raises(ValueError, match="FXStrangle with string delta as `strike` cannot"):
+            FXStrangle(
+                pair="eurusd",
+                expiry=dt(2023, 6, 16),
+                strike=["25d", "35d"],
+                premium=[NoInput(0), 1.0],
+            )
+
+
+class TestFXBrokerFly:
+
+    @pytest.mark.parametrize("strike, ccy", [
+        ([1.024, 1.0683, 1.116], "usd"),
+        (["-20d", "atm_delta", "20d"], "usd"),
+        ([1.024, 1.0683, 1.116], "eur"),
+        (["-20d", "atm_delta", "20d"], "eur"),
+    ])
+    @pytest.mark.parametrize("smile", [True, False])
+    @pytest.mark.parametrize("delta_type", ["forward", "spot_pa"])
+    def test_fxbf_rate(self, fxfo, delta_type, strike, ccy, smile):
+        # test pricing a straddle with vol 10.0 returns 10.0
+        fxo = FXBrokerFly(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=[20e6, NoInput(0)],
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=strike,
+            premium_ccy=ccy,
+            delta_type="forward",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.8,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type=delta_type,
+        )
+        vol = fxvs if smile else 9.5
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+
+        approx_expected = 2.40 if smile else 0.0
+        assert abs(result-approx_expected) < 0.16
+
+    @pytest.mark.parametrize("strike, ccy", [
+        ([1.024, 1.0683, 1.116], "usd"),
+        (["-20d", "atm_delta", "20d"], "usd"),
+        ([1.0228, 1.0683, 1.1147], "eur"),
+        (["-20d", "atm_delta", "20d"], "eur"),
+    ])
+    @pytest.mark.parametrize("smile", [True])
+    def test_fxbf_rate_pips(self, fxfo, strike, ccy, smile):
+        fxo = FXBrokerFly(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=[20e6, NoInput(0)],
+            delivery_lag=2,
+            payment_lag=2,
+            calendar="tgt",
+            strike=strike,
+            premium_ccy=ccy,
+            delta_type="forward",
+            metric="pips_or_%",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.8,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="spot",
+        )
+        vol = fxvs if smile else 9.5
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+        expected = (-111.2, 0.1) if ccy == "usd" else (-1.041, 0.02)
+        assert abs(result - expected[0]) < expected[1]
+
+    @pytest.mark.parametrize("strike, ccy", [
+        ([1.024, 1.0683, 1.116], "usd"),
+        (["-20d", "atm_delta", "20d"], "usd"),
+        ([1.024, 1.06668, 1.116], "eur"),
+        (["-20d", "atm_delta", "20d"], "eur"),
+    ])
+    def test_fxbf_rate_premium(self, fxfo, strike, ccy):
+        fxo = FXBrokerFly(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=[20e6, NoInput(0)],
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            strike=strike,
+            premium_ccy=ccy,
+            delta_type="forward",
+            metric="premium",
+        )
+        fxvs = FXDeltaVolSmile(
+            nodes={
+                0.25: 10.15,
+                0.50: 7.8,
+                0.75: 8.9,
+            },
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        vol = fxvs
+        curves = [None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")]
+        result = fxo.rate(curves, fx=fxfo, vol=vol)
+        expected = (-221743, 100) if ccy == "usd" else (-210350, 800)
+        assert abs(result - expected[0]) < expected[1]
+
+    def test_bf_rate_vols_list(self, fxfo):
+        fxbf = FXBrokerFly(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            notional=[20e6, -13.5e6],
+            strike=("-20d", "atm_delta", "20d"),
+            payment_lag=2,
+            delivery_lag=2,
+            calendar="tgt",
+            premium_ccy="usd",
+            delta_type="spot",
+        )
+        result = fxbf.rate(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=[10.15, 1.0, 8.9],
+        )
+        expected = 8.539499
+        assert abs(result - expected) < 1e-6
+
+        result = fxbf.rate(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            fx=fxfo,
+            vol=[10.15, 7.8, 8.9],
+            metric="pips_or_%"
+        )
+        expected = -110.098920
+        assert abs(result - expected) < 1e-6
+
+    @pytest.mark.parametrize("notn, expected_grks, expected_ccy", [
+        ([1e6, NoInput(0)], [-0.026421, -3.099638, 0.000001], [-26421.063, -33088.735, 0.014]),
+        ([2e6, NoInput(0)], [-0.026421, -3.099638, 0.000001], [-52842.126, -66177.47, 0.028]),
+        ([-2e6, NoInput(0)], [-0.026421, -3.099638, 0.000001],  [-52842.126, -66177.47, 0.028]),
+        ([1e6, -600e3], [-0.026421, -1.234429, 0.041264], [-26421.063, -13177.651, 412.638])
+    ])
+    @pytest.mark.parametrize("strikes", [
+        ("-20d", "atm_delta", "20d"),
+        (1.023875122921023, 1.0683288279019205, 1.1159193339873164)
+    ])
+    def test_greeks_delta_direction(self, fxfo, notn, expected_grks, expected_ccy, strikes):
+        # test the delta and delta_eur are not impacted by a Buy or Sell. Delta is expressed relative to a Buy.
+        fxo = FXBrokerFly(
+            pair="eurusd",
+            expiry=dt(2023, 6, 16),
+            delivery_lag=dt(2023, 6, 20),
+            payment_lag=dt(2023, 6, 20),
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            delta_type="forward",
+            premium_ccy="usd",
+            strike=strikes,
+            notional=notn,
+        )
+        fxvs = FXDeltaVolSmile(
+            {0.25: 10.15, 0.5: 7.8, 0.75: 8.9},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+        )
+        result = fxo.analytic_greeks(
+            curves=[None, fxfo.curve("eur", "usd"), None, fxfo.curve("usd", "usd")],
+            vol=fxvs,
+            fx=fxfo
+        )
+        assert abs(result["delta"] - expected_grks[0]) < 1e-6
+        assert abs(result["gamma"] - expected_grks[1]) < 1e-4
+        assert abs(result["vega"] - expected_grks[2]) < 1e-5
+
+        assert abs(result["delta_eur"] - expected_ccy[0]) < 1e-1
+        assert abs(result["gamma_eur_1%"] - expected_ccy[1]) < 1.5
+        assert abs(result["vega_usd"] - expected_ccy[2]) < 1e-1
+
+
+class TestVolValue:
+
+    def test_solver_passthrough(self):
+        smile = FXDeltaVolSmile(
+            nodes={0.25: 10.0, 0.5: 10.0, 0.75: 10.0},
+            eval_date=dt(2023, 3, 16),
+            expiry=dt(2023, 6, 16),
+            delta_type="forward",
+            id="VolSmile",
+        )
+        instruments = [
+            VolValue(0.25, vol=smile),
+            VolValue(0.5, vol="VolSmile"),
+            VolValue(0.75, vol="VolSmile"),
+        ]
+        solver = Solver(curves=[smile], instruments=instruments, s=[8.9, 8.2, 9.1])
+        assert abs(smile[0.25] - 8.9) < 5e-7
+        assert abs(smile[0.5] - 8.2) < 5e-7
+        assert abs(smile[0.75] - 9.1) < 5e-7
+
+    def test_no_solver_vol_value(self):
+        vv = VolValue(0.25, vol="string_id")
+        with pytest.raises(ValueError, match="String `vol` ids require a `solver`"):
+            vv.rate()
```

### Comparing `rateslib-1.1.1/tests/test_instruments_bonds.py` & `rateslib-1.2.0/tests/test_instruments_bonds.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     FixedRateBond,
     Bill,
     FloatRateNote,
     BondFuture,
     IndexFixedRateBond,
 )
 from rateslib.dual import Dual, Dual2
-from rateslib.calendars import dcf
+from rateslib.calendars import dcf, get_calendar
 from rateslib.curves import Curve, IndexCurve, LineCurve
 from rateslib.fx import FXRates
 from rateslib.solver import Solver
 
 
 @pytest.fixture()
 def curve():
@@ -1501,32 +1501,42 @@
         assert abs(result - expected) < 1e-6
 
     @pytest.mark.parametrize(
         "metric, spd, exp",
         [
             ("clean_price", 0.0, 100),
             ("dirty_price", 0.0, 100),
-            ("clean_price", 50.0, 99.99602155150806),
-            ("dirty_price", 50.0, 100.03848730493272),
+            ("clean_price", 50.0, 99.99601798513253),
+            ("dirty_price", 50.0, 100.03848373855718),
         ],
     )
     def test_float_rate_bond_forward_prices(self, metric, spd, exp):
+        fixings = Series(
+            data=2.0,
+            index=date_range(start=dt(2007, 1, 1), end=dt(2010, 2, 28), freq=get_calendar("bus"))
+        )
         bond = FloatRateNote(
             effective=dt(2007, 1, 1),
             termination=dt(2017, 1, 1),
             frequency="S",
             convention="Act365f",
             ex_div=3,
             float_spread=spd,
             fixing_method="rfr_observation_shift",
+            calendar="bus",
+            fixings=fixings,
             method_param=5,
             spread_compound_method="none_simple",
             settle=2,
         )
-        curve = Curve({dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0}, convention="act365f")
+        curve = Curve(
+            {dt(2010, 3, 1): 1.0, dt(2017, 1, 1): 1.0},
+            convention="act365f",
+            calendar="bus"
+        )
         disc_curve = curve.shift(spd)
 
         result = bond.rate(
             curves=[curve, disc_curve], metric=metric, forward_settlement=dt(2010, 8, 1)
         )
         assert abs(result - exp) < 1e-8
```

### Comparing `rateslib-1.1.1/tests/test_legs.py` & `rateslib-1.2.0/tests/test_legs.py`

 * *Files identical despite different names*

### Comparing `rateslib-1.1.1/tests/test_periods.py` & `rateslib-1.2.0/tests/test_solver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1908 +1,1953 @@
 import pytest
-import re
 from datetime import datetime as dt
-from datetime import timedelta
-from pandas.testing import assert_frame_equal
-from pandas import DataFrame, Series, Index
+from pandas import DataFrame, MultiIndex
+from pandas.testing import assert_frame_equal, assert_series_equal
 import numpy as np
+from numpy.testing import assert_allclose
+from math import log, exp
 
 import context
+from rateslib import default_context
 from rateslib.default import NoInput
-from rateslib.periods import (
-    Cashflow,
-    FixedPeriod,
-    FloatPeriod,
-    IndexFixedPeriod,
-    IndexCashflow,
-    IndexMixin,
+from rateslib.curves import Curve, index_left, LineCurve, CompositeCurve
+from rateslib.solver import Solver, Gradients, newton_1dim, newton_ndim
+from rateslib.dual import Dual, Dual2, gradient
+from rateslib.instruments import (
+    IRS,
+    Value,
+    FloatRateNote,
+    Portfolio,
+    XCS,
+    FXStrangle,
+    FXStraddle,
+    FXRiskReversal,
+    FXBrokerFly,
+    FXSwap,
+    FXCall
 )
-from rateslib.fx import FXRates
-from rateslib.default import Defaults
-from rateslib.curves import Curve, LineCurve, IndexCurve, CompositeCurve
-from rateslib import defaults
+from rateslib.fx import FXRates, FXForwards
+from rateslib.fx_volatility import FXDeltaVolSmile, FXDeltaVolSurface
 
 
-@pytest.fixture()
-def curve():
-    nodes = {
-        dt(2022, 1, 1): 1.00,
-        dt(2022, 4, 1): 0.99,
-        dt(2022, 7, 1): 0.98,
-        dt(2022, 10, 1): 0.97,
-    }
-    return Curve(nodes=nodes, interpolation="log_linear")
+class TestGradients:
+    @classmethod
+    def setup_class(cls):
+        class Inst:
+            def __init__(self, rate):
+                self._rate = rate
+
+            def rate(self, *args, **kwargs):
+                return self._rate
+
+        class SolverProxy(Gradients):
+            variables = ["v1", "v2", "v3"]
+            r = [Dual(1.0, ["v1"], []), Dual(3.0, ["v1", "v2", "v3"], [2.0, 1.0, -2.0])]
+            _J = None
+            instruments = [
+                [Inst(Dual2(1.0, ["v1"], [1.0], [4.0])), tuple(), {}],
+                [
+                    Inst(
+                        Dual2(
+                            3.0,
+                            ["v1", "v2", "v3"],
+                            [2.0, 1.0, -2.0],
+                            [-2.0, 1.0, 1.0, 1.0, -3.0, 2.0, 1.0, 2.0, -4.0],
+                        )
+                    ),
+                    tuple(),
+                    {},
+                ],
+            ]
+            _J2 = None
+            _ad = 2
+            _grad_s_vT = np.array(
+                [
+                    [1.0, 2.0, 3.0],
+                    [2.0, 3.0, 4.0],
+                ]
+            )
 
+        setattr(cls, "solver", SolverProxy())
 
-@pytest.fixture()
-def fxr():
-    return FXRates({"usdnok": 10.0})
-
-
-@pytest.fixture()
-def rfr_curve():
-    v1 = 1 / (1 + 0.01 / 365)
-    v2 = v1 / (1 + 0.02 / 365)
-    v3 = v2 / (1 + 0.03 / 365)
-    v4 = v3 / (1 + 0.04 / 365)
-
-    nodes = {
-        dt(2022, 1, 1): 1.00,
-        dt(2022, 1, 2): v1,
-        dt(2022, 1, 3): v2,
-        dt(2022, 1, 4): v3,
-        dt(2022, 1, 5): v4,
-    }
-    return Curve(nodes=nodes, interpolation="log_linear", convention="act365f")
+    def test_J(self):
+        expected = np.array(
+            [
+                [1.0, 2.0],
+                [0.0, 1.0],
+                [0.0, -2.0],
+            ]
+        )
+        result = self.solver.J
+        assert_allclose(result, expected)
+
+    def test_grad_v_rT(self):
+        assert_allclose(self.solver.J, self.solver.grad_v_rT)
+
+    def test_J2(self):
+        expected = np.array(
+            [
+                [
+                    [8.0, 0.0, 0.0],
+                    [0.0, 0.0, 0.0],
+                    [0.0, 0.0, 0.0],
+                ],
+                [
+                    [-4.0, 2.0, 2.0],
+                    [2.0, -6.0, 4.0],
+                    [2.0, 4.0, -8.0],
+                ],
+            ]
+        )
+        expected = np.transpose(expected, (1, 2, 0))
+        result = self.solver.J2
+        assert_allclose(expected, result)
+
+    def test_grad_v_v_rT(self):
+        assert_allclose(self.solver.J2, self.solver.grad_v_v_rT)
+
+    def test_grad_s_vT(self):
+        expected = np.array(
+            [
+                [1.0, 2.0, 3.0],
+                [2.0, 3.0, 4.0],
+            ]
+        )
+        result = self.solver.grad_s_vT
+        assert_allclose(expected, result)
+
+
+@pytest.mark.parametrize("algo", ["gauss_newton", "levenberg_marquardt", "gradient_descent"])
+def test_basic_solver(algo):
+    curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        },
+        id="v",
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+    ]
+    s = np.array([1.0, 1.6, 2.0])
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+        algorithm=algo,
+    )
+    assert float(solver.g) < 1e-9
+    assert curve.nodes[dt(2022, 1, 1)] == Dual(1.0, ["v0"], [1])
+    expected = [1, 0.9899250357528555, 0.9680433953206192, 0.9407188354823821]
+    for i, key in enumerate(curve.nodes.keys()):
+        assert abs(float(curve.nodes[key]) - expected[i]) < 1e-6
+
+
+@pytest.mark.parametrize("algo", ["gauss_newton", "levenberg_marquardt", "gradient_descent"])
+def test_solver_reiterate(algo):
+    # test that curves are properly updated by a reiterate
+    curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        },
+        id="v",
+    )
+    instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "Q", curves="v"),
+        IRS(dt(2022, 1, 1), "2Y", "Q", curves="v"),
+        IRS(dt(2022, 1, 1), "3Y", "Q", curves="v"),
+    ]
+    s = np.array([1.0, 1.5, 2.0])
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+        algorithm=algo,
+    )
+    assert float(solver.g) < 1e-9
 
+    solver.s[1] = 1.6
+    solver.iterate()
 
-@pytest.fixture()
-def line_curve():
-    nodes = {
-        dt(2021, 12, 31): -99,
-        dt(2022, 1, 1): 1.00,
-        dt(2022, 1, 2): 2.00,
-        dt(2022, 1, 3): 3.00,
-        dt(2022, 1, 4): 4.00,
-        dt(2022, 1, 5): 5.00,
-    }
-    return LineCurve(nodes=nodes, interpolation="linear", convention="act365f")
+    # now check that a reiteration has resolved the curve
+    assert curve.nodes[dt(2022, 1, 1)] == Dual(1.0, ["v0"], [1])
+    expected = [1, 0.9899250357528555, 0.9680433953206192, 0.9407188354823821]
+    for i, key in enumerate(curve.nodes.keys()):
+        assert abs(float(curve.nodes[key]) - expected[i]) < 1e-6
+
+
+@pytest.mark.parametrize("algo", ["gauss_newton", "levenberg_marquardt", "gradient_descent"])
+def test_basic_solver_line_curve(algo):
+    curve = LineCurve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+        },
+        id="v",
+    )
+    instruments = [
+        (Value(dt(2022, 1, 1)), (curve,), {}),
+        (Value(dt(2023, 1, 1)), (curve,), {}),
+        (Value(dt(2024, 1, 1)), (curve,), {}),
+    ]
+    s = np.array([3.0, 3.6, 4.0])
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+        algorithm=algo,
+    )
+    assert float(solver.g) < 1e-9
+    for i, key in enumerate(curve.nodes.keys()):
+        assert abs(float(curve.nodes[key]) - s[i]) < 1e-5
+
+
+def test_basic_spline_solver():
+    spline_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.99,
+            dt(2024, 1, 1): 0.965,
+            dt(2025, 1, 1): 0.93,
+        },
+        interpolation="log_linear",
+        t=[
+            dt(2023, 1, 1),
+            dt(2023, 1, 1),
+            dt(2023, 1, 1),
+            dt(2023, 1, 1),
+            dt(2024, 1, 1),
+            dt(2025, 1, 3),
+            dt(2025, 1, 3),
+            dt(2025, 1, 3),
+            dt(2025, 1, 3),
+        ],
+        id="v",
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), (spline_curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), (spline_curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (spline_curve,), {}),
+    ]
+    s = np.array([1.0, 1.6, 2.0])
+    solver = Solver(
+        curves=[spline_curve],
+        instruments=instruments,
+        s=s,
+        algorithm="gauss_newton",
+    )
+    assert float(solver.g) < 1e-12
+    assert spline_curve.nodes[dt(2022, 1, 1)] == Dual(1.0, ["v0"], [1])
+    expected = [1, 0.98992503575307, 0.9680377261843034, 0.9407048036486593]
+    for i, key in enumerate(spline_curve.nodes.keys()):
+        assert abs(float(spline_curve.nodes[key]) - expected[i]) < 1e-11
+
+
+def test_large_spline_solver():
+    dates = [
+        dt(2000, 1, 3),
+        dt(2001, 1, 3),
+        dt(2002, 1, 3),
+        dt(2003, 1, 3),
+        dt(2004, 1, 3),
+        dt(2005, 1, 3),
+        dt(2006, 1, 3),
+        dt(2007, 1, 3),
+        dt(2008, 1, 3),
+        dt(2009, 1, 3),
+        dt(2010, 1, 3),
+        dt(2012, 1, 3),
+        dt(2015, 1, 3),
+        dt(2020, 1, 3),
+        dt(2025, 1, 3),
+        dt(2030, 1, 3),
+        dt(2035, 1, 3),
+        dt(2040, 1, 3),
+        dt(2050, 1, 3),
+    ]
+    curve = Curve(
+        nodes={_: 1.0 for _ in dates},
+        t=[dt(2000, 1, 3)] * 3 + dates[:-1] + [dt(2050, 1, 5)] * 4,
+        calendar="nyc",
+    )
+    solver = Solver(
+        curves=[curve],
+        instruments=[
+            IRS(dt(2000, 1, 3), _, spec="usd_irs", curves=curve) for _ in dates[1:]
+        ],
+        s=[1.0 + _ / 25 for _ in range(18)],
+    )
+    assert solver.result["status"] == "SUCCESS"
 
 
-class TestFXandBase:
-    def test_fx_and_base_raise(self):
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.96}, id="curve")
-        per = FixedPeriod(
-            dt(2022, 2, 1),
-            dt(2022, 3, 1),
-            dt(2022, 3, 1),
-            "A",
-            fixed_rate=2,
-            currency="usd",
+def test_solver_raises_len():
+    with pytest.raises(ValueError, match="`instrument_rates` must be same length"):
+        Solver(
+            instruments=[1],
+            s=[1, 2],
+        )
+
+    with pytest.raises(ValueError, match="`instrument_labels` must have length"):
+        Solver(
+            instruments=[1],
+            s=[1],
+            instrument_labels=[1, 2],
+        )
+
+    with pytest.raises(ValueError, match="`weights` must be same length"):
+        Solver(
+            instruments=[1, 2],
+            s=[1, 2],
+            instrument_labels=[1, 2],
+            weights=[1],
         )
-        with pytest.raises(ValueError, match="`base` "):
-            per.npv(curve, curve, base="eur")
 
-    def test_fx_and_base_warn1(self):
-        # base and numeric fx given.
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.96}, id="curve")
-        per = FixedPeriod(
-            dt(2022, 2, 1),
-            dt(2022, 3, 1),
-            dt(2022, 3, 1),
-            "A",
-            fixed_rate=2,
-            currency="usd",
-        )
-        with pytest.warns(UserWarning, match="`base` "):
-            per.npv(curve, curve, fx=1.1, base="eur")
 
-    def test_fx_and_base_warn2(self):
-        # base is none and numeric fx given.
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.96}, id="curve")
-        per = FixedPeriod(
-            dt(2022, 2, 1),
-            dt(2022, 3, 1),
-            dt(2022, 3, 1),
-            "A",
-            fixed_rate=2,
-            currency="usd",
+def test_basic_solver_weights():
+    # This test replicates test_basic_solver with the 3Y rate at two different rates.
+    # We vary the weights argument to selectively decide which one to use.
+    curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        },
+        id="v",
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+    ]
+    s = np.array([1.0, 1.6, 2.02, 1.98])  # average 3Y at approximately 2.0%
+    with default_context("algorithm", "gauss_newton"):
+        solver = Solver(
+            curves=[curve],
+            instruments=instruments,
+            s=s,
+            func_tol=0.00085,
+        )
+    assert float(solver.g) < 0.00085
+    assert curve.nodes[dt(2022, 1, 1)] == Dual(1.0, ["v0"], [1])
+    expected = [1, 0.9899250357528555, 0.9680433953206192, 0.9407188354823821]
+    for i, key in enumerate(curve.nodes.keys()):
+        assert abs(float(curve.nodes[key]) - expected[i]) < 1e-6
+
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+        weights=[1, 1, 1, 1e-6],
+        func_tol=1e-7,
+        algorithm="gauss_newton",
+    )
+    assert abs(float(instruments[2][0].rate(curve)) - 2.02) < 1e-4
+
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+        weights=[1, 1, 1e-6, 1],
+        func_tol=1e-7,
+        algorithm="gauss_newton",
+    )
+    assert abs(float(instruments[2][0].rate(curve)) - 1.98) < 1e-4
+
+
+def test_solver_independent_curve():
+    # Test that a solver can use an independent curve as a static object and solve
+    # without mutating that un-referenced object.
+    independent_curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.98,
+            dt(2024, 1, 1): 0.96,
+            dt(2025, 1, 1): 0.94,
+        }
+    )
+    expected = independent_curve.copy()
+    var_curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 0.99,
+            dt(2024, 1, 1): 0.98,
+            dt(2025, 1, 1): 0.97,
+        }
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), ([var_curve, independent_curve],), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), ([var_curve, independent_curve],), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), ([var_curve, independent_curve],), {}),
+    ]
+    s = np.array([2.00, 2.00, 2.00])
+    with default_context("curve_not_in_solver", "ignore"):
+        Solver(
+            curves=[var_curve],
+            instruments=instruments,
+            s=s,
+            func_tol=1e-13,
+            conv_tol=1e-13,
+        )
+    for i, instrument in enumerate(instruments):
+        assert abs(float(instrument[0].rate(*instrument[1], **instrument[2]) - s[i])) < 1e-7
+    assert independent_curve == expected
+
+
+class TestSolverCompositeCurve:
+    def test_solver_composite_curve(self):
+        # this test creates a solver with a composite curve
+        # for the purpose of adding a turn
+        c_base = Curve(
+            {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0, dt(2024, 1, 1): 1.0, dt(2025, 1, 1): 1.0},
+            id="sek_base",
         )
-        with pytest.warns(UserWarning, match="It is not best practice to provide"):
-            per.npv(curve, curve, fx=1.1)
+        c_turns = Curve(
+            {
+                dt(2022, 1, 1): 1.0,
+                dt(2022, 12, 30): 1.0,
+                dt(2023, 1, 1): 1.0,
+                dt(2025, 1, 1): 1.0,
+            },
+            id="sek_turns",
+        )
+        composite_curve = CompositeCurve([c_base, c_turns], id="sek")
 
+        instruments_turns = [
+            IRS(dt(2022, 1, 1), "1d", "A", curves="sek_turns"),
+            IRS(dt(2022, 12, 30), "1d", "A", curves="sek_turns"),
+            IRS(dt(2023, 1, 1), "1d", "A", curves="sek_turns"),
+        ]
+        s_turns = [0.0, -0.50, 0.0]
+        labels_turns = ["NA1", "Turn1", "NA2"]
+
+        instruments_base = [
+            IRS(dt(2022, 1, 1), "1Y", "A", curves="sek"),
+            IRS(dt(2022, 1, 1), "2Y", "A", curves="sek"),
+            IRS(dt(2022, 1, 1), "3Y", "A", curves="sek"),
+        ]
+        s_base = [2.0, 2.3, 2.4]
+        labels_base = ["1Y", "2Y", "3Y"]
+
+        solver = Solver(
+            curves=[c_base, c_turns, composite_curve],
+            instruments=instruments_turns + instruments_base,
+            s=s_turns + s_base,
+            instrument_labels=labels_turns + labels_base,
+            id="solv",
+        )
+
+        test_irs = IRS(dt(2022, 6, 1), "15M", "A", notional=1e6, curves="sek")
+
+        expected = 2.31735564
+        result = test_irs.rate(solver=solver)
+        assert (result - expected) < 1e-8
 
-class TestFloatPeriod:
-    def test_none_cashflow(self):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
+        delta = test_irs.delta(solver=solver)
+        expected = DataFrame(
+            data=[
+                -0.226074787,
+                0.2257131776,
+                0.0003616069,
+                -9.159037835,
+                131.75543312,
+                0.0033383280,
+            ],
+            columns=MultiIndex.from_tuples([("usd", "usd")], names=["local_ccy", "display_ccy"]),
+            index=MultiIndex.from_tuples(
+                [
+                    ("instruments", "solv", "NA1"),
+                    ("instruments", "solv", "Turn1"),
+                    ("instruments", "solv", "NA2"),
+                    ("instruments", "solv", "1Y"),
+                    ("instruments", "solv", "2Y"),
+                    ("instruments", "solv", "3Y"),
+                ],
+                names=["type", "solver", "label"],
+            ),
         )
-        assert float_period.cashflow(None) is None
+        assert_frame_equal(delta, expected)
 
-    @pytest.mark.parametrize(
-        "spread_method, float_spread, expected",
-        [
-            ("none_simple", 100.0, 24744.478172244584),
-            ("isda_compounding", 0.0, 24744.478172244584),
-            ("isda_compounding", 100.0, 25053.484941157145),
-            ("isda_flat_compounding", 100.0, 24867.852396116967),
-        ],
+
+def test_non_unique_curves():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    solver = Solver(
+        curves=[curve], instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})], s=[1]
     )
-    def test_float_period_analytic_delta(self, curve, spread_method, float_spread, expected):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            float_spread=float_spread,
-            spread_compound_method=spread_method,
+
+    with pytest.raises(ValueError, match="`curves` must each have their own unique"):
+        Solver(
+            curves=[curve2],
+            instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
+            s=[2],
+            pre_solvers=[solver],
+        )
+
+    with pytest.raises(ValueError, match="`curves` must each have their own unique"):
+        Solver(
+            curves=[curve, curve2],
+            instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
+            s=[2],
         )
-        result = float_period.analytic_delta(curve)
-        assert abs(result - expected) < 1e-7
 
-    @pytest.mark.parametrize(
-        "spread, crv, fx",
-        [
-            (4.00, True, 2.0),
-            (NoInput(0), False, 2.0),
-            (4.00, True, 10.0),
-            (NoInput(0), False, 10.0),
-        ],
+
+def test_max_iterations():
+    # This test replicates has an oscillatory solution between the different 3y rates.
+    curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        },
+        id="v",
     )
-    def test_float_period_cashflows(self, curve, fxr, spread, crv, fx):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            float_spread=spread,
-        )
-        curve = curve if crv else None
-        rate = None if curve is None else float(float_period.rate(curve))
-        cashflow = None if rate is None else rate * -1e9 * float_period.dcf / 100
-        expected = {
-            Defaults.headers["type"]: "FloatPeriod",
-            Defaults.headers["stub_type"]: "Regular",
-            Defaults.headers["a_acc_start"]: dt(2022, 1, 1),
-            Defaults.headers["a_acc_end"]: dt(2022, 4, 1),
-            Defaults.headers["payment"]: dt(2022, 4, 3),
-            Defaults.headers["notional"]: 1e9,
-            Defaults.headers["currency"]: "USD",
-            Defaults.headers["convention"]: "Act360",
-            Defaults.headers["dcf"]: float_period.dcf,
-            Defaults.headers["df"]: 0.9897791268897856 if crv else None,
-            Defaults.headers["rate"]: rate,
-            Defaults.headers["spread"]: 0 if spread is NoInput.blank else spread,
-            Defaults.headers["npv"]: -10096746.871171726 if crv else None,
-            Defaults.headers["cashflow"]: cashflow,
-            Defaults.headers["fx"]: fx,
-            Defaults.headers["npv_fx"]: -10096746.871171726 * fx if crv else None,
-            Defaults.headers["collateral"]: None,
-        }
-        if fx == 2.0:
-            with pytest.warns(UserWarning):
-                # It is not best practice to provide `fx` as numeric
-                result = float_period.cashflows(
-                    curve if crv else NoInput(0),
-                    fx=2.0,
-                    base=NoInput(0),
-                )
-        else:
-            result = float_period.cashflows(
-                curve if crv else NoInput(0),
-                fx=fxr,
-                base="nok",
-            )
-        assert result == expected
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+    ]
+    s = np.array([1.0, 1.6, 2.02, 1.98])  # average 3Y at approximately 2.0%
+    with default_context("algorithm", "gauss_newton"):
+        solver = Solver(
+            curves=[curve],
+            instruments=instruments,
+            s=s,
+            func_tol=1e-10,
+            max_iter=30,
+        )
+    assert len(solver.g_list) == 31
+
+
+def test_solver_pre_solver_dependency_generates_same_delta():
+    """
+    Build an ESTR curve with solver1.
+    Build an IBOR curve with solver2 dependent upon solver1.
+
+    Build an ESTR and IBOR curve simultaneously inside the same solver3.
+
+    Test the delta and the instrument calibration error
+    """
+    eur_disc_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0, dt(2024, 1, 1): 1.0}, id="eur"
+    )
+    eur_instruments = [
+        (IRS(dt(2022, 1, 1), "8M", "A"), (eur_disc_curve,), {}),
+        (IRS(dt(2022, 1, 1), "16M", "A"), (eur_disc_curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "A"), (eur_disc_curve,), {}),
+    ]
+    eur_disc_s = [2.01, 2.22, 2.55]
+    eur_disc_solver = Solver([eur_disc_curve], [], eur_instruments, eur_disc_s, id="estr")
 
-    def test_spread_compound_raises(self):
-        with pytest.raises(ValueError, match="`spread_compound_method`"):
-            FloatPeriod(
-                start=dt(2022, 1, 1),
-                end=dt(2022, 4, 1),
-                payment=dt(2022, 4, 3),
-                frequency="Q",
-                spread_compound_method="bad_vibes",
-            )
+    eur_ibor_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0, dt(2024, 1, 1): 1.0}, id="eur_ibor"
+    )
+    eur_ibor_instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "A"), ([eur_ibor_curve, eur_disc_curve],), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "A"), ([eur_ibor_curve, eur_disc_curve],), {}),
+    ]
+    eur_ibor_s = [2.25, 2.65]
+    eur_solver2 = Solver(
+        [eur_ibor_curve], [], eur_ibor_instruments, eur_ibor_s, pre_solvers=[eur_disc_solver], id="ibor"
+    )
 
-    def test_spread_compound_calc_raises(self):
-        period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            frequency="Q",
-            spread_compound_method="none_simple",
-            float_spread=1,
-        )
-        period.spread_compound_method = "bad_vibes"
-        with pytest.raises(ValueError, match="`spread_compound_method` must be in"):
-            period._isda_compounded_rate_with_spread(Series([1, 2]), Series([1, 1]))
-
-    def test_rfr_lockout_too_few_dates(self, curve):
-        period = FloatPeriod(
-            start=dt(2022, 1, 10),
-            end=dt(2022, 1, 15),
-            payment=dt(2022, 1, 15),
-            frequency="M",
-            fixing_method="rfr_lockout",
-            method_param=6,
-        )
-        with pytest.raises(ValueError, match="period has too few dates"):
-            period.rate(curve)
+    eur_disc_curve2 = Curve(
+        {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0, dt(2024, 1, 1): 1.0}, id="eur"
+    )
+    eur_ibor_curve2 = Curve(
+        {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0, dt(2024, 1, 1): 1.0}, id="eur_ibor"
+    )
+    eur_instruments2 = [
+        (IRS(dt(2022, 1, 1), "8M", "A"), (eur_disc_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "16M", "A"), (eur_disc_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "A"), (eur_disc_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "1Y", "A"), ([eur_ibor_curve2, eur_disc_curve2],), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "A"), ([eur_ibor_curve2, eur_disc_curve2],), {}),
+    ]
+    eur_disc_s2 = [2.01, 2.22, 2.55, 2.25, 2.65]
+    eur_solver_sim = Solver(
+        [eur_disc_curve2, eur_ibor_curve2],
+        [],
+        eur_instruments2,
+        eur_disc_s2,
+        id="eur_sol_sim",
+        instrument_labels=["estr0", "estr1", "estr2", "ibor0", "ibor1"],
+    )
 
-    def test_fixing_method_raises(self):
-        with pytest.raises(ValueError, match="`fixing_method`"):
-            FloatPeriod(
-                start=dt(2022, 1, 1),
-                end=dt(2022, 4, 1),
-                payment=dt(2022, 4, 3),
-                frequency="Q",
-                fixing_method="bad_vibes",
-            )
+    eur_swap = IRS(
+        dt(2022, 3, 1),
+        "16M",
+        "M",
+        fixed_rate=3.0,
+    )
 
-    def test_float_period_npv(self, curve):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-        )
-        result = float_period.npv(curve)
-        assert abs(result + 9997768.95848275) < 1e-7
+    delta_sim = eur_swap.delta([eur_ibor_curve2, eur_disc_curve2], eur_solver_sim)
+    delta_pre = eur_swap.delta([eur_ibor_curve, eur_disc_curve], eur_solver2)
+    delta_pre.index = delta_sim.index
+    assert_frame_equal(delta_sim, delta_pre)
+
+    error_sim = eur_solver_sim.error
+    error_pre = eur_solver2.error
+    assert_series_equal(error_pre, error_sim, check_index=False, rtol=1e-5, atol=1e-3)
 
-    def test_rfr_avg_method_raises(self, curve):
-        period = FloatPeriod(
-            dt(2022, 1, 1), dt(2022, 1, 4), dt(2022, 1, 4), "Q",
-            fixing_method="rfr_payment_delay_avg",
-            spread_compound_method="isda_compounding",
-        )
-        msg = "`spread_compound` method must be 'none_simple' in an RFR averaging " \
-              "period."
-        with pytest.raises(ValueError, match=msg):
-            period.rate(curve)
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_payment_delay_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1), dt(2022, 1, 4), dt(2022, 1, 4), "Q", fixing_method="rfr_payment_delay"
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.01 / 365) * (1 + 0.02 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_payment_delay_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_payment_delay",
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.10 / 365) * (1 + 0.08 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_payment_delay_avg_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1), dt(2022, 1, 4), dt(2022, 1, 4), "Q", fixing_method="rfr_payment_delay_avg"
-        )
-        result = period.rate(curve)
-        expected = (1.0 + 2.0 + 3.0) / 3
-        assert abs(result - expected) < 1e-11
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_payment_delay_avg_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_payment_delay_avg",
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = (10.0 + 8.0 + 3.0) / 3
-        assert abs(result - expected) < 1e-11
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_lockout_avg_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_lockout_avg",
-            method_param=2,
-        )
-        assert period._is_inefficient is True  # lockout requires all fixings.
-        result = period.rate(curve)
-        expected = 1.0
-        assert abs(result - expected) < 1e-11
-
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_lockout_avg",
-            method_param=1,
-        )
-        result = period.rate(rfr_curve)
-        expected = (2 + 3.0 + 3.0) / 3
-        assert abs(result - expected) < 1e-11
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_lockout_avg_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_lockout_avg",
-            method_param=2,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = 10.0
-        assert abs(result - expected) < 1e-12
-
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_lockout_avg",
-            method_param=1,
-            fixings=[10, 8],
-        )
-        result = period.rate(rfr_curve)
-        expected = (10.0 + 8.0 + 8.0 ) /3
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_lockout_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_lockout",
-            method_param=2,
-        )
-        assert period._is_inefficient is True  # lockout requires all fixings.
-        result = period.rate(curve)
-        expected = ((1 + 0.01 / 365) * (1 + 0.01 / 365) * (1 + 0.01 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_lockout",
-            method_param=1,
-        )
-        result = period.rate(rfr_curve)
-        expected = ((1 + 0.02 / 365) * (1 + 0.03 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_lockout_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 1),
-            dt(2022, 1, 4),
-            dt(2022, 1, 4),
-            "Q",
-            fixing_method="rfr_lockout",
-            method_param=2,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.10 / 365) * (1 + 0.10 / 365) * (1 + 0.10 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_lockout",
-            method_param=1,
-            fixings=[10, 8],
-        )
-        result = period.rate(rfr_curve)
-        expected = ((1 + 0.10 / 365) * (1 + 0.08 / 365) * (1 + 0.08 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_observation_shift_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift",
-            method_param=1,
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.01 / 365) * (1 + 0.02 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-        period = FloatPeriod(
-            dt(2022, 1, 3),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift",
-            method_param=2,
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.01 / 365) * (1 + 0.02 / 365) - 1) * 36500 / 2
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_observation_shift_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift",
-            method_param=1,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.10 / 365) * (1 + 0.08 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-        assert abs(result - expected) < 1e-12
-
-        period = FloatPeriod(
-            dt(2022, 1, 3),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift",
-            method_param=2,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = ((1 + 0.10 / 365) * (1 + 0.08 / 365) - 1) * 36500 / 2
-        assert abs(result - expected) < 1e-12
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_observation_shift_avg_method(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift_avg",
-            method_param=1,
-        )
-        result = period.rate(curve)
-        expected = (1.0 + 2 + 3) /3
-        assert abs(result - expected) < 1e-11
-
-        period = FloatPeriod(
-            dt(2022, 1, 3),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift_avg",
-            method_param=2,
-        )
-        result = period.rate(curve)
-        expected = (1.0 + 2.0) / 2
-        assert abs(result - expected) < 1e-11
-
-    @pytest.mark.parametrize("curve_type", ["curve", "line_curve"])
-    def test_rfr_observation_shift_avg_method_with_fixings(self, curve_type, rfr_curve, line_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            dt(2022, 1, 2),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift_avg",
-            method_param=1,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = (10.0 + 8.0 + 3.0) / 3
-        assert abs(result - expected) < 1e-11
-
-        period = FloatPeriod(
-            dt(2022, 1, 3),
-            dt(2022, 1, 5),
-            dt(2022, 1, 5),
-            "Q",
-            fixing_method="rfr_observation_shift_avg",
-            method_param=2,
-            fixings=[10, 8],
-        )
-        result = period.rate(curve)
-        expected = (10.0 + 8) / 2
-        assert abs(result - expected) < 1e-11
-
-    def test_dcf_obs_period_raises(self):
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, calendar="ldn")
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 12, 31),
-            payment=dt(2022, 12, 31),
-            frequency="A",
-            fixing_method="rfr_lookback",
-            method_param=5,
-        )
-        # this may only raise when lookback is used ?
-        with pytest.raises(ValueError, match="RFR Observation and Accrual DCF dates "):
-            float_period.rate(curve)
-
-    @pytest.mark.parametrize("curve_type", ["curve", "linecurve"])
-    @pytest.mark.parametrize(
-        "method, expected, expected_date",
-        [
-            ("rfr_payment_delay", [1000000, 1000082, 1000191, 1000561], dt(2022, 1, 6)),
-            ("rfr_observation_shift", [1499240, 1499281, 1499363, 1499486], dt(2022, 1, 4)),
-            ("rfr_lockout", [999931, 4999411, 0, 0], dt(2022, 1, 6)),
-            ("rfr_lookback", [999657, 999685, 2998726, 999821], dt(2022, 1, 4)),
-        ],
+
+def test_delta_gamma_calculation():
+    estr_curve = Curve(
+        {dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0}, id="estr_curve"
+    )
+    estr_instruments = [
+        (IRS(dt(2022, 1, 1), "10Y", "A"), (estr_curve,), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), (estr_curve,), {}),
+    ]
+    estr_solver = Solver(
+        [estr_curve], [], estr_instruments, [2.0, 1.5], id="estr", instrument_labels=["10Y", "20Y"]
     )
-    def test_rfr_fixings_array(self, curve_type, method, expected, expected_date):
-        # tests the fixings array and the compounding for different types of curve
-        # at different rates in the period.
-
-        v1 = 1 / (1 + 0.01 / 365)
-        v2 = v1 / (1 + 0.02 / 365)
-        v3 = v2 / (1 + 0.03 / 365)
-        v4 = v3 / (1 + 0.04 / 365)
-        v5 = v4 / (1 + 0.045 * 3 / 365)
-        v6 = v5 / (1 + 0.05 / 365)
-        v7 = v6 / (1 + 0.055 / 365)
-
-        nodes = {
-            dt(2022, 1, 3): 1.00,
-            dt(2022, 1, 4): v1,
-            dt(2022, 1, 5): v2,
-            dt(2022, 1, 6): v3,
-            dt(2022, 1, 7): v4,
-            dt(2022, 1, 10): v5,
-            dt(2022, 1, 11): v6,
-            dt(2022, 1, 12): v7,
-        }
-        curve = Curve(
-            nodes=nodes,
-            interpolation="log_linear",
-            convention="act365f",
-            calendar="bus",
-        )
 
-        line_curve = LineCurve(
-            nodes={
-                dt(2022, 1, 2): -99,
-                dt(2022, 1, 3): 1.0,
-                dt(2022, 1, 4): 2.0,
-                dt(2022, 1, 5): 3.0,
-                dt(2022, 1, 6): 4.0,
-                dt(2022, 1, 7): 4.5,
-                dt(2022, 1, 10): 5.0,
-                dt(2022, 1, 11): 5.5,
-            },
-            interpolation="linear",
-            convention="act365f",
-            calendar="bus",
-        )
-        rfr_curve = curve if curve_type == "curve" else line_curve
+    # Mechanism 1: dynamic
+    eur_swap = IRS(dt(2032, 1, 1), "10Y", "A", notional=100e6)
+    assert 74430 < float(eur_swap.delta(estr_curve, estr_solver).sum().iloc[0]) < 74432
+    assert -229 < float(eur_swap.gamma(estr_curve, estr_solver).sum().sum()) < -228
+
+    # Mechanism 1: dynamic names
+    assert 74430 < float(eur_swap.delta("estr_curve", estr_solver).sum().iloc[0]) < 74432
+    assert -229 < float(eur_swap.gamma("estr_curve", estr_solver).sum().sum()) < -228
+
+    # Mechanism 1: fails on None curve specification
+    with pytest.raises(TypeError, match="`curves` have not been supplied correctly"):
+        assert eur_swap.delta(NoInput(0), estr_solver)
+    with pytest.raises(TypeError, match="`curves` have not been supplied correctly"):
+        assert eur_swap.gamma(NoInput(0), estr_solver)
+
+    # Mechanism 2: static specific
+    eur_swap = IRS(dt(2032, 1, 1), "10Y", "A", notional=100e6, curves=estr_curve)
+    assert 74430 < float(eur_swap.delta(NoInput(0), estr_solver).sum().iloc[0]) < 74432
+    assert -229 < float(eur_swap.gamma(NoInput(0), estr_solver).sum().sum()) < -228
+
+    # Mechanism 2: static named
+    eur_swap = IRS(dt(2032, 1, 1), "10Y", "A", notional=100e6, curves="estr_curve")
+    assert 74430 < float(eur_swap.delta(NoInput(0), estr_solver).sum().iloc[0]) < 74432
+    assert -229 < float(eur_swap.gamma(NoInput(0), estr_solver).sum().sum()) < -228
+
+
+def test_solver_delta_fx_noinput():
+    estr_curve = Curve(
+        {dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0}, id="estr_curve"
+    )
+    estr_instruments = [
+        (IRS(dt(2022, 1, 1), "10Y", "A"), (estr_curve,), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), (estr_curve,), {}),
+    ]
+    estr_solver = Solver(
+        [estr_curve], [], estr_instruments, [2.0, 1.5], id="estr", instrument_labels=["10Y", "20Y"]
+    )
+    eur_swap = IRS(dt(2032, 1, 1), "10Y", "A", notional=100e6, fixed_rate=2)
+    npv = eur_swap.npv(curves=estr_curve, solver=estr_solver, local=True)
+    result = estr_solver.delta(npv)
+    assert type(result) is DataFrame
+
+
+def test_solver_pre_solver_dependency_generates_same_gamma():
+    estr_curve = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0})
+    estr_instruments = [
+        (IRS(dt(2022, 1, 1), "7Y", "A"), (estr_curve,), {}),
+        (IRS(dt(2022, 1, 1), "15Y", "A"), (estr_curve,), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), (estr_curve,), {}),
+    ]
+    estr_s = [2.0, 1.75, 1.5]
+    estr_labels = ["7ye", "15ye", "20ye"]
+    estr_solver = Solver(
+        [estr_curve],
+        [],
+        estr_instruments,
+        estr_s,
+        id="estr",
+        instrument_labels=estr_labels,
+        algorithm="gauss_newton"
+    )
 
-        period = FloatPeriod(
-            dt(2022, 1, 5),
-            dt(2022, 1, 11),
-            dt(2022, 1, 11),
-            "Q",
-            fixing_method=method,
-            convention="act365f",
-            notional=-1000000,
-        )
-        rate, table = period._rfr_fixings_array(
-            curve=rfr_curve, fixing_exposure=True, disc_curve=curve
-        )
+    ibor_curve = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0})
+    ibor_instruments = [
+        (IRS(dt(2022, 1, 1), "10Y", "A"), ([ibor_curve, estr_curve],), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), ([ibor_curve, estr_curve],), {}),
+    ]
+    ibor_s = [2.1, 1.65]
+    ibor_labels = ["10Yi", "20Yi"]
+    ibor_solver = Solver(
+        [ibor_curve],
+        [],
+        ibor_instruments,
+        ibor_s,
+        id="ibor",
+        instrument_labels=ibor_labels,
+        pre_solvers=[estr_solver],
+        algorithm="gauss_newton",
+    )
 
-        assert table["obs_dates"][1] == expected_date
-        for i, val in table["notional"].iloc[:-1].items():
-            assert abs(expected[i] - val) < 1
-
-    def test_rfr_fixings_array_raises(self, rfr_curve):
-        period = FloatPeriod(
-            dt(2022, 1, 5),
-            dt(2022, 1, 11),
-            dt(2022, 1, 11),
-            "Q",
-            fixing_method="rfr_payment_delay",
-            notional=-1000000,
-        )
-        period.fixing_method = "bad_vibes"
-        with pytest.raises(NotImplementedError, match="`fixing_method`"):
-            period._rfr_fixings_array(rfr_curve)
+    eur_swap = IRS(dt(2032, 1, 1), "10Y", "A", notional=100e6)
+    gamma_pre = eur_swap.gamma([ibor_curve, estr_curve], ibor_solver)
+    delta_pre = eur_swap.delta([ibor_curve, estr_curve], ibor_solver)
+
+    estr_curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0})
+    ibor_curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0})
+    sim_instruments = [
+        (IRS(dt(2022, 1, 1), "7Y", "A"), (estr_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "15Y", "A"), (estr_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), (estr_curve2,), {}),
+        (IRS(dt(2022, 1, 1), "10Y", "A"), ([ibor_curve2, estr_curve2],), {}),
+        (IRS(dt(2022, 1, 1), "20Y", "A"), ([ibor_curve2, estr_curve2],), {}),
+    ]
+    simultaneous_solver = Solver(
+        [estr_curve2, ibor_curve2],
+        [],
+        sim_instruments,
+        estr_s + ibor_s,
+        id="simul",
+        instrument_labels=estr_labels + ibor_labels,
+        algorithm="gauss_newton",
+    )
+    gamma_sim = eur_swap.gamma([ibor_curve2, estr_curve2], simultaneous_solver)
+    delta_sim = eur_swap.delta([ibor_curve2, estr_curve2], simultaneous_solver)
 
-    @pytest.mark.parametrize(
-        "method, param, expected",
-        [
-            ("rfr_payment_delay", 0, 1000000),
-            ("rfr_observation_shift", 1, 333319),
-            ("rfr_lookback", 1, 333319),
-        ],
+    # check arrays in construction of gamma
+    grad_s_vT_sim = simultaneous_solver.grad_s_vT_pre
+    grad_s_vT_pre = ibor_solver.grad_s_vT_pre
+    assert_allclose(grad_s_vT_pre, grad_s_vT_sim, atol=1e-14, rtol=1e-10)
+
+    simultaneous_solver._set_ad_order(2)
+    J2_sim = simultaneous_solver.J2_pre
+    ibor_solver._set_ad_order(2)
+    J2_pre = ibor_solver.J2_pre
+    assert_allclose(J2_pre, J2_sim, atol=1e-14, rtol=1e-10)
+
+    grad_s_s_vT_sim = simultaneous_solver.grad_s_s_vT_pre
+    grad_s_s_vT_pre = ibor_solver.grad_s_s_vT_pre
+    assert_allclose(grad_s_s_vT_pre, grad_s_s_vT_sim, atol=1e-14, rtol=1e-10)
+
+    gamma_pre.index = gamma_sim.index
+    gamma_pre.columns = gamma_sim.columns
+    delta_pre.index = delta_sim.index
+    assert_frame_equal(delta_sim, delta_pre)
+    assert_frame_equal(gamma_sim, gamma_pre)
+
+
+def test_nonmutable_presolver_defaults():
+    estr_curve = Curve({dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0})
+    estr_instruments = [
+        (IRS(dt(2022, 1, 1), "10Y", "A"), (estr_curve,), {}),
+    ]
+    estr_s = [2.0]
+    estr_labels = ["10ye"]
+    estr_solver = Solver(
+        [estr_curve],
+        [],
+        estr_instruments,
+        estr_s,
+        id="estr",
+        instrument_labels=estr_labels,
     )
-    def test_rfr_fixings_array_single_period(self, method, param, expected):
-        rfr_curve = Curve(
-            nodes={dt(2022, 1, 3): 1.0, dt(2022, 1, 15): 0.9995},
-            interpolation="log_linear",
-            convention="act365f",
-            calendar="bus",
-        )
-        period = FloatPeriod(
-            dt(2022, 1, 10),
-            dt(2022, 1, 11),
-            dt(2022, 1, 11),
-            "Q",
-            fixing_method=method,
-            method_param=param,
-            notional=-1000000,
-            convention="act365f",
-        )
-        result = period.fixings_table(rfr_curve)
-        assert abs(result["notional"].iloc[0] - expected) < 1
+    with pytest.raises(AttributeError, match="'tuple' object has no attribute"):
+        estr_solver.pre_solvers.extend([1, 2, 3])
 
-    @pytest.mark.parametrize(
-        "method, expected",
-        [
-            (
-                "none_simple",
-                ((1 + 0.01 / 365) * (1 + 0.02 / 365) * (1 + 0.03 / 365) - 1) * 36500 / 3
-                + 100 / 100,
-            ),
-            (
-                "isda_compounding",
-                ((1 + 0.02 / 365) * (1 + 0.03 / 365) * (1 + 0.04 / 365) - 1) * 36500 / 3,
-            ),
-            ("isda_flat_compounding", 3.000173518986841),
-        ],
+
+def test_solver_grad_s_vT_methods_equivalent():
+    curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+            dt(2026, 1, 1): 1.0,
+            dt(2027, 1, 1): 1.0,
+        }
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "1Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2022, 5, 1), "4Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "4Y", "A"), (curve,), {}),
+    ]
+    s = [1.2, 1.4, 1.6, 1.7, 1.9]
+    solver = Solver([curve], [], instruments, s, algorithm="gauss_newton")
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_analytical"
+    grad_s_vT_final_iter_anal = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_dual"
+    solver._grad_s_vT_final_iteration_algo = "gauss_newton_final"
+    solver._reset_properties_()
+    grad_s_vT_final_iter_dual = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_fixed_point_iteration"
+    solver._reset_properties_()
+    grad_s_vT_fixed_point_iter = solver.grad_s_vT
+
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_final_iter_anal, atol=1e-12)
+    assert_allclose(grad_s_vT_fixed_point_iter, grad_s_vT_final_iter_anal, atol=1e-12)
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_fixed_point_iter, atol=1e-12)
+
+
+def test_solver_grad_s_vT_methods_equivalent_overspecified_curve():
+    curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+            # dt(2026, 1, 1): 1.0,
+            dt(2027, 1, 1): 1.0,
+        }
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "1Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "2Y", "A"), (curve,), {}),
+        (IRS(dt(2022, 5, 1), "4Y", "A"), (curve,), {}),
+        (IRS(dt(2023, 1, 1), "4Y", "A"), (curve,), {}),
+    ]
+    s = [1.2, 1.4, 1.6, 1.7, 1.9]
+    solver = Solver([curve], [], instruments, s, algorithm="gauss_newton")
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_analytical"
+    grad_s_vT_final_iter_anal = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_final_iteration_dual"
+    solver._grad_s_vT_final_iteration_algo = "gauss_newton_final"
+    solver._reset_properties_()
+    grad_s_vT_final_iter_dual = solver.grad_s_vT
+
+    solver._grad_s_vT_method = "_grad_s_vT_fixed_point_iteration"
+    solver._reset_properties_()
+    grad_s_vT_fixed_point_iter = solver.grad_s_vT
+
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_final_iter_anal, atol=1e-6)
+    assert_allclose(grad_s_vT_fixed_point_iter, grad_s_vT_final_iter_anal, atol=1e-6)
+    assert_allclose(grad_s_vT_final_iter_dual, grad_s_vT_fixed_point_iter, atol=1e-6)
+
+
+def test_solver_second_order_vars_raise_on_first_order():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    solver = Solver(
+        curves=[curve], instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})], s=[1]
     )
-    def test_rfr_compounding_float_spreads(self, method, expected, rfr_curve):
-        period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 1, 4),
-            payment=dt(2022, 1, 4),
-            frequency="M",
-            float_spread=100,
-            spread_compound_method=method,
-            convention="act365f",
-        )
-        result = period.rate(rfr_curve)
-        assert abs(result - expected) < 1e-8
 
-    def test_ibor_rate_line_curve(self, line_curve):
-        period = FloatPeriod(
-            start=dt(2022, 1, 5),
-            end=dt(2022, 4, 5),
-            payment=dt(2022, 4, 5),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-        )
-        assert period._is_inefficient is False
-        assert period.rate(line_curve) == 3.0
+    with pytest.raises(ValueError, match="Cannot perform second derivative calc"):
+        solver.J2
 
-    def test_ibor_fixing_table(self, line_curve):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 4, 4),
-            payment=dt(2022, 4, 4),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-        )
-        result = float_period.fixings_table(line_curve)
-        expected = DataFrame(
-            {"obs_dates": [dt(2022, 1, 2)], "notional": [-1e6], "dcf": [None], "rates": [2.0]}
-        ).set_index("obs_dates")
-        assert_frame_equal(expected, result)
-
-    def test_ibor_fixing_table_fast(self, line_curve):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 4, 4),
-            payment=dt(2022, 4, 4),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-        )
-        result = float_period.fixings_table(line_curve, approximate=True)
-        expected = DataFrame(
-            {"obs_dates": [dt(2022, 1, 2)], "notional": [-1e6], "dcf": [None], "rates": [2.0]}
-        ).set_index("obs_dates")
-        assert_frame_equal(expected, result)
-
-    def test_ibor_fixings(self):
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2025, 1, 1): 0.90}, calendar="bus")
-        fixings = Series(
-            [1.00, 2.801, 1.00, 1.00],
-            index=[dt(2023, 3, 1), dt(2023, 3, 2), dt(2023, 3, 3), dt(2023, 3, 6)],
-        )
-        float_period = FloatPeriod(
-            start=dt(2023, 3, 6),
-            end=dt(2023, 6, 6),
-            payment=dt(2023, 6, 6),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-            fixings=fixings,
-        )
-        result = float_period.rate(curve)
-        assert result == 2.801
+    with pytest.raises(ValueError, match="Cannot perform second derivative calc"):
+        solver.grad_s_s_vT
 
-    def test_ibor_fixing_unavailable(self):
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2025, 1, 1): 0.90}, calendar="bus")
-        lcurve = LineCurve({dt(2022, 1, 1): 2.0, dt(2025, 1, 1): 4.0}, calendar="bus")
-        fixings = Series([2.801], index=[dt(2023, 3, 1)])
-        float_period = FloatPeriod(
-            start=dt(2023, 3, 20),
-            end=dt(2023, 6, 20),
-            payment=dt(2023, 6, 20),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-            fixings=fixings,
-        )
-        result = float_period.rate(curve)  # fixing occurs 18th Mar, not in `fixings`
-        assert abs(result - 3.476095729528156) < 1e-5
-        result = float_period.rate(lcurve)  # fixing occurs 18th Mar, not in `fixings`
-        assert abs(result - 2.801094890510949) < 1e-5
-
-    @pytest.mark.parametrize("float_spread", [0, 100])
-    def test_ibor_rate_df_curve(self, float_spread, curve):
-        period = FloatPeriod(
-            start=dt(2022, 4, 1),
-            end=dt(2022, 7, 1),
-            payment=dt(2022, 7, 1),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-            float_spread=float_spread,
-        )
-        expected = (0.99 / 0.98 - 1) * 36000 / 91 + float_spread / 100
-        assert period.rate(curve) == expected
 
-    @pytest.mark.parametrize("float_spread", [0, 100])
-    def test_ibor_rate_stub_df_curve(self, float_spread, curve):
-        period = FloatPeriod(
-            start=dt(2022, 4, 1),
-            end=dt(2022, 5, 1),
-            payment=dt(2022, 5, 1),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-            stub=True,
-            float_spread=float_spread,
-        )
-        expected = (0.99 / curve[dt(2022, 5, 1)] - 1) * 36000 / 30 + float_spread / 100
-        assert period.rate(curve) == expected
+def test_solver_second_order_vars_raise_on_first_order_pre_solvers():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    solver = Solver(
+        curves=[curve], instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})], s=[1]
+    )
+    curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="B")
+    solver2 = Solver(
+        curves=[curve2],
+        instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve2,), {})],
+        s=[1],
+        pre_solvers=[solver],
+    )
 
-    def test_single_fixing_override(self, curve):
-        period = FloatPeriod(
-            start=dt(2022, 4, 1),
-            end=dt(2022, 5, 1),
-            payment=dt(2022, 5, 1),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-            stub=True,
-            float_spread=100,
-            fixings=7.5,
-        )
-        expected = 7.5 + 1
-        assert period.rate(curve) == expected
+    with pytest.raises(ValueError, match="Cannot perform second derivative calc"):
+        solver2.J2_pre
 
-    @pytest.mark.parametrize("curve_type", ["curve", "linecurve"])
-    def test_period_historic_fixings(self, curve_type, line_curve, rfr_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        period = FloatPeriod(
-            start=dt(2021, 12, 30),
-            end=dt(2022, 1, 3),
-            payment=dt(2022, 1, 3),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            float_spread=100,
-            fixings=[1.5, 2.5],
-            convention="act365F",
-        )
-        expected = (
-            (1 + 0.015 / 365) * (1 + 0.025 / 365) * (1 + 0.01 / 365) * (1 + 0.02 / 365) - 1
-        ) * 36500 / 4 + 1
-        assert period.rate(curve) == expected
-
-    @pytest.mark.parametrize("curve_type", ["curve", "linecurve"])
-    def test_period_historic_fixings_series(self, curve_type, line_curve, rfr_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        fixings = Series(
-            [99, 99, 1.5, 2.5],
-            index=[dt(1995, 1, 1), dt(2021, 12, 29), dt(2021, 12, 30), dt(2021, 12, 31)],
-        )
-        period = FloatPeriod(
-            start=dt(2021, 12, 30),
-            end=dt(2022, 1, 3),
-            payment=dt(2022, 1, 3),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            float_spread=100,
-            fixings=fixings,
-            convention="act365F",
-        )
-        expected = (
-            (1 + 0.015 / 365) * (1 + 0.025 / 365) * (1 + 0.01 / 365) * (1 + 0.02 / 365) - 1
-        ) * 36500 / 4 + 1
-        result = period.rate(curve)
-        assert result == expected
-
-    @pytest.mark.parametrize("curve_type", ["curve", "linecurve"])
-    def test_period_historic_fixings_series_missing_warns(self, curve_type, line_curve, rfr_curve):
-        curve = rfr_curve if curve_type == "curve" else line_curve
-        fixings = Series([99, 99, 2.5], index=[dt(1995, 12, 1), dt(2021, 12, 30), dt(2022, 1, 1)])
-        period = FloatPeriod(
-            start=dt(2021, 12, 30),
-            end=dt(2022, 1, 3),
-            payment=dt(2022, 1, 3),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            float_spread=100,
-            fixings=fixings,
-            convention="act365F",
-        )
-        # expected = ((1 + 0.015 / 365) * (1 + 0.025 / 365) * (1 + 0.01 / 365) * (
-        #             1 + 0.02 / 365) - 1) * 36500 / 4 + 1
-        with pytest.warns(UserWarning):
-            period.rate(curve)
-        # assert result == expected
-
-    def test_fixing_with_float_spread_warning(self, curve):
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 4, 4),
-            payment=dt(2022, 4, 4),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            spread_compound_method="isda_compounding",
-            float_spread=100,
-            fixings=1.0,
-        )
-        with pytest.warns(UserWarning):
-            result = float_period.rate(curve)
-        assert result == 2.0
-
-    # @pytest.mark.skip(reason="str is an erroneous input to function: test redundant.")
-    # def test_float_period_rate_raises(self):
-    #     float_period = FloatPeriod(
-    #         start=dt(2022, 1, 4),
-    #         end=dt(2022, 4, 4),
-    #         payment=dt(2022, 4, 4),
-    #         frequency="Q",
-    #     )
-    #     with pytest.raises(TypeError, match="Curve must be of type"):
-    #         float_period.rate("bad_curve")
-
-    def test_float_period_fixings_list_raises_on_ibor(self, curve, line_curve):
-        with pytest.raises(ValueError, match="`fixings` cannot be supplied as list,"):
-            float_period = FloatPeriod(
-                start=dt(2022, 1, 4),
-                end=dt(2022, 4, 4),
-                payment=dt(2022, 4, 4),
-                frequency="Q",
-                fixing_method="ibor",
-                method_param=2,
-                fixings=[1.00],
-            )
+    with pytest.raises(ValueError, match="Cannot perform second derivative calc"):
+        solver.grad_s_s_vT_pre
 
-        float_period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 4, 4),
-            payment=dt(2022, 4, 4),
-            frequency="Q",
-            fixing_method="ibor",
-            method_param=2,
-        )
-        float_period.fixings = [1.0]
-        with pytest.raises(ValueError, match="`fixings` cannot be supplied as list,"):
-            float_period.rate(curve)
-        with pytest.raises(ValueError, match="`fixings` cannot be supplied as list,"):
-            float_period.rate(line_curve)
 
-    @pytest.mark.parametrize("meth, exp", [
-        ("rfr_payment_delay", DataFrame(
-            {
-                "obs_dates": [
-                    dt(2022, 12, 28),
-                    dt(2022, 12, 29),
-                    dt(2022, 12, 30),
-                    dt(2022, 12, 31),
-                    dt(2023, 1, 1),
-                ],
-                "notional": [
-                    0.0,
-                    0.0,
-                    0.0,
-                    -999821.37380,
-                    -999932.84380,
-                ],
-                "dcf": [0.0027777777777777778] * 5,
-                "rates": [1.19, 1.19, -8.81, 4.01364, 4.01364],
-            }
-        ).set_index("obs_dates")),
-        ("rfr_payment_delay_avg", DataFrame(
-            {
-                "obs_dates": [
-                    dt(2022, 12, 28),
-                    dt(2022, 12, 29),
-                    dt(2022, 12, 30),
-                    dt(2022, 12, 31),
-                    dt(2023, 1, 1),
-                ],
-                "notional": [
-                    0.0,
-                    0.0,
-                    0.0,
-                    -999888.52252,
-                    -1000000.00000,
-                ],
-                "dcf": [0.0027777777777777778] * 5,
-                "rates": [1.19, 1.19, -8.81, 4.01364, 4.01364],
-            }
-        ).set_index("obs_dates"))
-    ])
-    def test_rfr_fixings_table(self, curve, meth, exp):
-        float_period = FloatPeriod(
-            start=dt(2022, 12, 28),
-            end=dt(2023, 1, 2),
-            payment=dt(2023, 1, 2),
-            frequency="M",
-            fixings=[1.19, 1.19, -8.81],
-            fixing_method=meth,
+def test_bad_algo_raises():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    with pytest.raises(NotImplementedError, match="`algorithm`: bad_algo"):
+        Solver(
+            curves=[curve],
+            instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
+            s=[1],
+            algorithm="bad_algo",
         )
-        result = float_period.fixings_table(curve)
-        assert_frame_equal(result, exp, rtol=1e-4)
 
-        curve._set_ad_order(order=1)
-        # assert values are unchanged even if curve can calculate derivatives
-        result = float_period.fixings_table(curve)
-        assert_frame_equal(result, exp)
 
-    @pytest.mark.parametrize(
-        "method, param",
-        [
-            ("rfr_payment_delay", NoInput(0)),
-            ("rfr_lookback", 4),
-            ("rfr_lockout", 1),
-            ("rfr_observation_shift", 2),
-        ],
+def test_solver_float_rate_bond():
+    """
+    This test checks the rate method of FloatRateNote when using complex rate spread
+    calculations (which artificially introduces Dual2 and then removes it)
+    """
+    d_c = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2022, 7, 1): 0.94,
+            dt(2023, 1, 1): 0.92,
+            dt(2024, 1, 1): 0.9,
+        },
+        id="credit",
     )
-    @pytest.mark.parametrize(
-        "scm, spd",
-        [
-            ("none_simple", 1000.0),
-            ("isda_compounding", 1000.0),
-            ("isda_flat_compounding", 1000.0),
-        ],
-    )
-    @pytest.mark.parametrize(
-        "crv",
-        [
-            Curve(
-                {
-                    dt(2022, 1, 1): 1.00,
-                    dt(2022, 4, 1): 0.99,
-                    dt(2022, 7, 1): 0.98,
-                    dt(2022, 10, 1): 0.97,
-                    dt(2023, 6, 1): 0.96,
-                },
-                interpolation="log_linear",
-                calendar="bus",
+    f_c = d_c.copy()
+    f_c.id = "rfr"
+    instruments = [
+        (
+            FloatRateNote(
+                dt(2022, 1, 1), "6M", "Q", spread_compound_method="isda_compounding", settle=2
             ),
-        ],
+            ([f_c, d_c],),
+            {"metric": "spread"},
+        ),
+        (
+            FloatRateNote(
+                dt(2022, 1, 1), "1y", "Q", spread_compound_method="isda_compounding", settle=2
+            ),
+            ([f_c, d_c],),
+            {"metric": "spread"},
+        ),
+        (
+            FloatRateNote(
+                dt(2022, 1, 1), "18m", "Q", spread_compound_method="isda_compounding", settle=2
+            ),
+            ([f_c, d_c],),
+            {"metric": "spread"},
+        ),
+    ]
+    Solver([d_c], [], instruments, [25, 25, 25])
+    result = d_c.rate(dt(2022, 7, 1), "1D")
+    expected = f_c.rate(dt(2022, 7, 1), "1D") + 0.25
+    assert abs(result - expected) < 3e-4
+
+
+def test_solver_grad_s_s_vt_methods_equivalent():
+    curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+            dt(2026, 1, 1): 1.0,
+            dt(2027, 1, 1): 1.0,
+            dt(2028, 1, 1): 1.0,
+            dt(2029, 1, 1): 1.0,
+        },
+        id="curve",
     )
-    def test_rfr_fixings_table_fast(self, method, param, scm, spd, crv):
-        float_period = FloatPeriod(
-            start=dt(2022, 12, 28),
-            end=dt(2023, 1, 3),
-            payment=dt(2023, 1, 3),
-            frequency="M",
-            fixing_method=method,
-            method_param=param,
-            spread_compound_method=scm,
-            float_spread=spd,
-        )
-        expected = float_period.fixings_table(crv)
-        result = float_period.fixings_table(crv, approximate=True)
-        assert_frame_equal(result, expected, rtol=1e-2)
+    instruments = [
+        IRS(dt(2022, 1, 1), "1y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "2y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "3y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "4y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "5y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "6y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "7y", "A", curves="curve"),
+    ]
+    with default_context("algorithm", "gauss_newton"):
+        solver = Solver(
+            curves=[curve],
+            instruments=instruments,
+            s=[1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7],
+        )
+    grad_s_s_vt_fwddiff = solver._grad_s_s_vT_fwd_difference_method()
+    solver._set_ad_order(order=2)
+    grad_s_s_vt_final = solver._grad_s_s_vT_final_iteration_analytical()
+    solver._set_ad_order(order=1)
+    assert_allclose(grad_s_s_vt_final, grad_s_s_vt_fwddiff, atol=5e-7)
+
+
+def test_gamma_raises():
+    curve = Curve(
+        {
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2025, 1, 1): 1.0,
+        },
+        id="v",
+    )
+    instruments = [
+        (IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "2Y", "Q"), (curve,), {}),
+        (IRS(dt(2022, 1, 1), "3Y", "Q"), (curve,), {}),
+    ]
+    s = np.array([1.0, 1.6, 2.0])
+    solver = Solver(
+        curves=[curve],
+        instruments=instruments,
+        s=s,
+    )
+    with pytest.raises(ValueError, match="`Solver` must be in ad order 2"):
+        solver.gamma(100)
 
-    @pytest.mark.parametrize(
-        "method, param",
-        [
-            ("rfr_payment_delay_avg", None),
-            ("rfr_lookback_avg", 4),
-            ("rfr_lockout_avg", 1),
-            ("rfr_observation_shift_avg", 2),
-        ],
+
+def test_delta_irs_guide():
+    # this mirrors the delta user guide page
+    usd_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2022, 2, 1): 1.0,
+            dt(2022, 4, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+        },
+        id="sofr",
     )
-    @pytest.mark.parametrize(
-        "crv",
-        [
-            Curve(
-                {
-                    dt(2022, 1, 1): 1.00,
-                    dt(2022, 4, 1): 0.99,
-                    dt(2022, 7, 1): 0.98,
-                    dt(2022, 10, 1): 0.97,
-                    dt(2023, 6, 1): 0.96,
-                },
-                interpolation="log_linear",
-                calendar="bus",
-            ),
-        ],
+    instruments = [
+        IRS(dt(2022, 1, 1), "1m", "A", curves="sofr"),
+        IRS(dt(2022, 1, 1), "3m", "A", curves="sofr"),
+        IRS(dt(2022, 1, 1), "1y", "A", curves="sofr"),
+    ]
+    usd_solver = Solver(
+        curves=[usd_curve],
+        id="usd_sofr",
+        instruments=instruments,
+        s=[2.5, 3.25, 4.0],
+        instrument_labels=["1m", "3m", "1y"],
     )
-    def test_rfr_fixings_table_fast_avg(self, method, param, crv):
-        float_period = FloatPeriod(
-            start=dt(2022, 12, 28),
-            end=dt(2023, 1, 3),
-            payment=dt(2023, 1, 3),
-            frequency="M",
-            fixing_method=method,
-            method_param=param,
-            spread_compound_method="none_simple",
-            float_spread=100.0,
-        )
-        expected = float_period.fixings_table(crv)
-        result = float_period.fixings_table(crv, approximate=True)
-        assert_frame_equal(result, expected, rtol=1e-2)
-
-    def test_rfr_rate_fixings_series_monotonic_error(self):
-        nodes = {
-            dt(2022, 1, 1): 1.00,
-            dt(2022, 4, 1): 0.99,
-            dt(2022, 7, 1): 0.98,
-            dt(2022, 10, 1): 0.97,
-        }
-        curve = Curve(nodes=nodes, interpolation="log_linear")
-        fixings = Series(
-            [99, 2.25, 2.375, 2.5],
-            index=[dt(1995, 12, 1), dt(2021, 12, 30), dt(2022, 12, 31), dt(2022, 1, 1)],
-        )
-        period = FloatPeriod(
-            start=dt(2021, 12, 30),
-            end=dt(2022, 1, 3),
-            payment=dt(2022, 1, 3),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            float_spread=100,
-            fixings=fixings,
-            convention="act365F",
-        )
-        with pytest.raises(ValueError, match="`fixings` as a Series"):
-            period.rate(curve)
+    irs = IRS(
+        effective=dt(2022, 1, 1),
+        termination="6m",
+        frequency="A",
+        currency="usd",
+        fixed_rate=6.0,
+        curves="sofr",
+    )
+    result = irs.delta(solver=usd_solver, base="eur", local=True)  # local overrides base to USD
+    expected = DataFrame(
+        [[0], [16.77263], [32.60487]],
+        index=MultiIndex.from_product(
+            [["instruments"], ["usd_sofr"], ["1m", "3m", "1y"]], names=["type", "solver", "label"]
+        ),
+        columns=MultiIndex.from_tuples([("usd", "usd")], names=["local_ccy", "display_ccy"]),
+    )
+    assert_frame_equal(result, expected)
+
 
-    @pytest.mark.parametrize(
-        "scm, exp",
+def test_delta_irs_guide_fx_base():
+    # this mirrors the delta user guide page
+    usd_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2022, 2, 1): 1.0,
+            dt(2022, 4, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+        },
+        id="sofr",
+    )
+    instruments = [
+        IRS(dt(2022, 1, 1), "1m", "A", curves="sofr"),
+        IRS(dt(2022, 1, 1), "3m", "A", curves="sofr"),
+        IRS(dt(2022, 1, 1), "1y", "A", curves="sofr"),
+    ]
+    usd_solver = Solver(
+        curves=[usd_curve],
+        id="usd_sofr",
+        instruments=instruments,
+        s=[2.5, 3.25, 4.0],
+        instrument_labels=["1m", "3m", "1y"],
+    )
+    irs = IRS(
+        effective=dt(2022, 1, 1),
+        termination="6m",
+        frequency="A",
+        currency="usd",
+        fixed_rate=6.0,
+        curves="sofr",
+    )
+    fxr = FXRates({"eurusd": 1.1})
+    result = irs.delta(solver=usd_solver, base="eur", fx=fxr)
+    expected = DataFrame(
         [
-            ("none_simple", True),
-            ("isda_compounding", False),
+            [0, 0, 0],
+            [15.247847, 15.247847, 16.772632],
+            [29.640788, 29.640788, 32.60487],
+            [0.926514, 0.926514, 0.0],
         ],
+        index=MultiIndex.from_tuples(
+            [
+                ("instruments", "usd_sofr", "1m"),
+                ("instruments", "usd_sofr", "3m"),
+                ("instruments", "usd_sofr", "1y"),
+                ("fx", "fx", "eurusd"),
+            ],
+            names=["type", "solver", "label"],
+        ),
+        columns=MultiIndex.from_tuples(
+            [
+                ("all", "eur"),
+                ("usd", "eur"),
+                ("usd", "usd"),
+            ],
+            names=["local_ccy", "display_ccy"],
+        ),
     )
-    def test_float_spread_affects_fixing_exposure(self, scm, exp):
-        nodes = {
-            dt(2022, 1, 1): 1.00,
-            dt(2022, 4, 1): 0.99,
-            dt(2022, 7, 1): 0.98,
-            dt(2022, 10, 1): 0.97,
-        }
-        curve = Curve(nodes=nodes, interpolation="log_linear")
-        period = FloatPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 7, 1),
-            payment=dt(2022, 7, 1),
-            frequency="S",
-            fixing_method="rfr_payment_delay",
-            float_spread=0,
-            convention="act365F",
-            spread_compound_method=scm,
-        )
-        table = period.fixings_table(curve)
-        period.float_spread = 200
-        table2 = period.fixings_table(curve)
-        assert (table["notional"].iloc[0] == table2["notional"].iloc[0]) == exp
-
-    def test_custom_interp_rate_nan(self):
-        float_period = FloatPeriod(
-            start=dt(2022, 12, 28),
-            end=dt(2023, 1, 2),
-            payment=dt(2023, 1, 2),
-            frequency="M",
-            fixings=[1.19, 1.19],
-        )
+    assert_frame_equal(result, expected)
 
-        def interp(date, nodes):
-            if date < dt(2023, 1, 1):
-                return None
-            return 2.0
-
-        line_curve = LineCurve({dt(2023, 1, 1): 3.0, dt(2023, 2, 1): 2.0}, interpolation=interp)
-        curve = Curve({dt(2023, 1, 1): 1.0, dt(2023, 2, 1): 0.999})
-        with pytest.raises(ValueError, match="RFRs could not be calculated"):
-            float_period.fixings_table(line_curve, disc_curve=curve)
-
-    def test_method_param_raises(self):
-        with pytest.raises(ValueError, match='`method_param` must be >0 for "rfr_lock'):
-            FloatPeriod(
-                start=dt(2022, 1, 4),
-                end=dt(2022, 4, 4),
-                payment=dt(2022, 4, 4),
-                frequency="Q",
-                fixing_method="rfr_lockout",
-                method_param=0,
-                fixings=[1.00],
-            )
 
-        with pytest.raises(ValueError, match="`method_param` should not be used"):
-            FloatPeriod(
-                start=dt(2022, 1, 4),
-                end=dt(2022, 4, 4),
-                payment=dt(2022, 4, 4),
-                frequency="Q",
-                fixing_method="rfr_payment_delay",
-                method_param=2,
-                fixings=[1.00],
-            )
+# def test_irs_delta_curves_undefined():
+#     # the IRS is not constructed under best practice.
+#     # The delta solver does not know how to price the irs
+#     curve = Curve({dt(2022, 1, 1): 1.0, dt(2027, 1, 1): 0.99, dt(2032, 1, 1): 0.98},
+#                   id="sonia")
+#     instruments = [
+#         IRS(dt(2022, 1, 1), "5y", "A", curves="sonia"),
+#         IRS(dt(2027, 1, 1), "5y", "A", curves="sonia"),
+#     ]
+#     solver = Solver(
+#         curves=[curve],
+#         instruments=instruments,
+#         s=[2.0, 2.5],
+#     )
+#     irs = IRS(dt(2022, 1, 1), "10y", "S", fixed_rate=2.38)
+#     with pytest.raises(TypeError, match="`curves` have not been supplied"):
+#         irs.delta(solver=solver)
+
+
+def test_mechanisms_guide_gamma():
+    instruments = [
+        IRS(dt(2022, 1, 1), "4m", "Q", curves="sofr"),
+        IRS(dt(2022, 1, 1), "8m", "Q", curves="sofr"),
+    ]
+    s = [1.85, 2.10]
+    ll_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2022, 5, 1): 1.0, dt(2022, 9, 1): 1.0},
+        interpolation="log_linear",
+        id="sofr",
+    )
+    ll_solver = Solver(
+        curves=[ll_curve], instruments=instruments, s=s, instrument_labels=["4m", "8m"], id="sofr"
+    )
 
-    def test_analytic_delta_no_curve_raises(self):
-        float_period = FloatPeriod(
-            start=dt(2022, 12, 28),
-            end=dt(2023, 1, 2),
-            payment=dt(2023, 1, 2),
-            frequency="M",
-            fixings=[1.19, 1.19, -8.81],
-            spread_compound_method="isda_compounding",
-            float_spread=1.0,
-        )
-        with pytest.raises(TypeError, match="`curve` must be supplied"):
-            float_period.analytic_delta()
+    instruments = [
+        IRS(dt(2022, 1, 1), "3m", "Q", curves="estr"),
+        IRS(dt(2022, 1, 1), "9m", "Q", curves="estr"),
+    ]
+    s = [0.75, 1.65]
+    ll_curve = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 1): 1.0, dt(2022, 10, 1): 1.0},
+        interpolation="log_linear",
+        id="estr",
+    )
+    combined_solver = Solver(
+        curves=[ll_curve],
+        instruments=instruments,
+        s=s,
+        instrument_labels=["3m", "9m"],
+        pre_solvers=[ll_solver],
+        id="estr",
+    )
 
-    def test_more_series_fixings_than_calendar_from_curve_raises(self):
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, calendar="bus")
-        fixings = Series(
-            [1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0],
-            index=[
-                dt(2022, 1, 4),
-                dt(2022, 1, 5),
-                dt(2022, 1, 6),
-                dt(2022, 1, 7),
-                dt(2022, 1, 8),
-                dt(2022, 1, 9),
-                dt(2022, 1, 10),
+    irs = IRS(
+        effective=dt(2022, 1, 1),
+        termination="6m",
+        frequency="Q",
+        currency="usd",
+        notional=500e6,
+        fixed_rate=2.0,
+        curves="sofr",
+    )
+    irs2 = IRS(
+        effective=dt(2022, 1, 1),
+        termination="6m",
+        frequency="Q",
+        currency="eur",
+        notional=-300e6,
+        fixed_rate=1.0,
+        curves="estr",
+    )
+    pf = Portfolio([irs, irs2])
+    pf.npv(solver=combined_solver, local=True)
+    pf.delta(solver=combined_solver)
+    fxr = FXRates({"eurusd": 1.10})
+    fxr._set_ad_order(2)
+    result = pf.gamma(solver=combined_solver, fx=fxr, base="eur")
+    expected = DataFrame(
+        data=[
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.13769, 0.28088, 0.0],
+            [0.0, 0.0, 0.28088, 0.44493, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [-0.28930, -0.45081, 0.0, 0.0, -0.68937],
+            [-0.45081, -0.47449, 0.0, 0.0, -1.37372],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [-0.68937, -1.37372, 0.0, 0.0, 0.00064],
+            [-0.31823, -0.49590, 0.0, 0.0, 0.0],
+            [-0.49590, -0.52194, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0],
+            [-0.28930, -0.45081, 0.0, 0.0, -0.68937],
+            [-0.45081, -0.47449, 0.0, 0.0, -1.37372],
+            [0.0, 0.0, 0.13770, 0.28088, 0.0],
+            [0.0, 0.0, 0.28088, 0.44493, 0.0],
+            [-0.68937, -1.37372, 0.0, 0.0, 0.00064],
+        ],
+        index=MultiIndex.from_tuples(
+            [
+                ("eur", "eur", "instruments", "sofr", "4m"),
+                ("eur", "eur", "instruments", "sofr", "8m"),
+                ("eur", "eur", "instruments", "estr", "3m"),
+                ("eur", "eur", "instruments", "estr", "9m"),
+                ("eur", "eur", "fx", "fx", "eurusd"),
+                ("usd", "eur", "instruments", "sofr", "4m"),
+                ("usd", "eur", "instruments", "sofr", "8m"),
+                ("usd", "eur", "instruments", "estr", "3m"),
+                ("usd", "eur", "instruments", "estr", "9m"),
+                ("usd", "eur", "fx", "fx", "eurusd"),
+                ("usd", "usd", "instruments", "sofr", "4m"),
+                ("usd", "usd", "instruments", "sofr", "8m"),
+                ("usd", "usd", "instruments", "estr", "3m"),
+                ("usd", "usd", "instruments", "estr", "9m"),
+                ("usd", "usd", "fx", "fx", "eurusd"),
+                ("all", "eur", "instruments", "sofr", "4m"),
+                ("all", "eur", "instruments", "sofr", "8m"),
+                ("all", "eur", "instruments", "estr", "3m"),
+                ("all", "eur", "instruments", "estr", "9m"),
+                ("all", "eur", "fx", "fx", "eurusd"),
             ],
-        )
-        period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 1, 11),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            payment=dt(2022, 1, 9),
-            float_spread=10.0,
-            fixings=fixings,
-        )
-        with pytest.raises(ValueError, match="The supplied `fixings` contain more"):
-            period.rate(curve)
+            names=["local_ccy", "display_ccy", "type", "solver", "label"],
+        ),
+        columns=MultiIndex.from_tuples(
+            [
+                ("instruments", "sofr", "4m"),
+                ("instruments", "sofr", "8m"),
+                ("instruments", "estr", "3m"),
+                ("instruments", "estr", "9m"),
+                ("fx", "fx", "eurusd"),
+            ],
+            names=["type", "solver", "label"],
+        ),
+    )
+    assert_frame_equal(result, expected, atol=1e-2, rtol=1e-4)
 
-    def test_series_fixings_not_applicable_to_period(self):
-        # if a series is historic and of no relevance all fixings are forecast from crv
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, calendar="bus")
-        fixings = Series([1.0, 2.0, 3.0], index=[dt(2021, 1, 4), dt(2021, 1, 5), dt(2021, 1, 6)])
-        period = FloatPeriod(
-            start=dt(2022, 1, 4),
-            end=dt(2022, 1, 11),
-            frequency="Q",
-            fixing_method="rfr_payment_delay",
-            payment=dt(2022, 1, 9),
-            float_spread=10.0,
-            fixings=fixings,
-        )
-        result = period.rate(curve)
-        expected = 1.09136153  # series fixings are completely ignored
-        assert abs(result - expected) < 1e-5
 
-    @pytest.mark.parametrize(
-        "meth, param, exp",
+def test_solver_gamma_pnl_explain():
+    instruments = [
+        IRS(dt(2022, 1, 1), "10y", "A", currency="usd", curves="sofr"),
+        IRS(dt(2032, 1, 1), "10y", "A", currency="usd", curves="sofr"),
+        IRS(dt(2022, 1, 1), "10y", "A", currency="eur", curves="estr"),
+        IRS(dt(2032, 1, 1), "10y", "A", currency="eur", curves="estr"),
+        XCS(
+            dt(2022, 1, 1),
+            "10y",
+            "A",
+            currency="usd",
+            leg2_currency="usd",
+            curves=["estr", "eurusd", "sofr", "sofr"],
+        ),
+        XCS(
+            dt(2032, 1, 1),
+            "10y",
+            "A",
+            currency="usd",
+            leg2_currency="eur",
+            curves=["estr", "eurusd", "sofr", "sofr"],
+        ),
+    ]
+    # s_base = np.array([3.45, 2.85, 2.25, 0.9, -15, -10])
+    sofr = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0}, id="sofr")
+    estr = Curve(nodes={dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0}, id="estr")
+    eurusd = Curve(
+        nodes={dt(2022, 1, 1): 1.0, dt(2032, 1, 1): 1.0, dt(2042, 1, 1): 1.0}, id="eurusd"
+    )
+    fxr = FXRates({"eurusd": 1.05}, settlement=dt(2022, 1, 3))
+    fxf = FXForwards(fxr, {"eureur": estr, "eurusd": eurusd, "usdusd": sofr})
+    sofr_solver = Solver(
+        curves=[sofr],
+        instruments=instruments[:2],
+        s=[3.45, 2.85],
+        instrument_labels=["10y", "10y10y"],
+        id="sofr",
+        fx=fxf,
+    )
+    estr_solver = Solver(
+        curves=[estr],
+        instruments=instruments[2:4],
+        s=[2.25, 0.90],
+        instrument_labels=["10y", "10y10y"],
+        id="estr",
+        fx=fxf,
+    )
+    solver = Solver(
+        curves=[eurusd],
+        instruments=instruments[4:],
+        s=[-10, -15],
+        instrument_labels=["10y", "10y10y"],
+        id="xccy",
+        fx=fxf,
+        pre_solvers=[sofr_solver, estr_solver],
+    )
+
+    pf = Portfolio(
         [
-            ("rfr_payment_delay", NoInput(0), 3.1183733605),
-            ("rfr_observation_shift", 2, 3.085000395),
-            ("rfr_lookback", 2, 3.05163645),
-            ("rfr_lockout", 7, 3.00157855),
-        ],
+            IRS(
+                dt(2022, 1, 1),
+                "20Y",
+                "A",
+                currency="eur",
+                fixed_rate=2.0,
+                notional=1e8,
+                curves="estr",
+            ),
+        ]
     )
-    def test_norges_bank_nowa_calc_same(self, meth, param, exp):
-        # https://app.norges-bank.no/nowa/#/en/
-        curve = Curve({dt(2023, 8, 4): 1.0}, calendar="osl", convention="act365f")
-        period = FloatPeriod(
-            start=dt(2023, 4, 27),
-            end=dt(2023, 5, 12),
-            payment=dt(2023, 5, 16),
-            frequency="A",
-            fixing_method=meth,
-            method_param=param,
-            float_spread=0.0,
-            fixings=defaults.fixings["nowa"],
-        )
-        result = period.rate(curve)
-        assert abs(result - exp) < 1e-7
 
-    def test_interpolated_ibor_warns(self):
-        period = FloatPeriod(
-            start=dt(2023, 4, 27),
-            end=dt(2023, 6, 12),
-            payment=dt(2023, 6, 16),
-            frequency="A",
-            fixing_method="ibor",
-            method_param=1,
-            float_spread=0.0,
-            stub=True,
-        )
-        curve1 = LineCurve({dt(2022, 1, 1): 1.0, dt(2024, 2, 1): 1.0})
-        with pytest.warns(UserWarning):
-            period.rate({"1m": curve1})
-        with pytest.warns(UserWarning):
-            period.rate({"3m": curve1})
-
-    def test_interpolated_ibor_rate_line(self):
-        period = FloatPeriod(
-            start=dt(2023, 2, 1),
-            end=dt(2023, 4, 1),
-            payment=dt(2023, 4, 1),
-            frequency="A",
-            fixing_method="ibor",
-            method_param=1,
-            float_spread=0.0,
-            stub=True,
-        )
-        curve3 = LineCurve({dt(2022, 1, 1): 3.0, dt(2023, 2, 1): 3.0})
-        curve1 = LineCurve({dt(2022, 1, 1): 1.0, dt(2023, 2, 1): 1.0})
-        result = period.rate({"1M": curve1, "3m": curve3})
-        expected = 1.0 + (3.0 - 1.0) * (dt(2023, 4, 1) - dt(2023, 3, 1)) / (dt(2023, 5, 1) - dt(2023, 3, 1))
-        assert abs(result - expected) < 1e-8
-
-    def test_interpolated_ibor_rate_df(self):
-        period = FloatPeriod(
-            start=dt(2023, 2, 1),
-            end=dt(2023, 4, 1),
-            payment=dt(2023, 4, 1),
-            frequency="A",
-            fixing_method="ibor",
-            method_param=1,
-            float_spread=0.0,
-            stub=True,
-        )
-        curve3 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 2, 1): 0.97})
-        curve1 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 2, 1): 0.99})
-        result = period.rate({"1M": curve1, "3m": curve3})
-        a, b = 0.91399161, 2.778518365
-        expected = a + (b - a) * (dt(2023, 4, 1) - dt(2023, 3, 1)) / (dt(2023, 5, 1) - dt(2023, 3, 1))
-        assert abs(result - expected) < 1e-8
-
-    def test_rfr_period_curve_dict_raises(self, curve):
-        period = FloatPeriod(
-            start=dt(2023, 2, 1),
-            end=dt(2023, 4, 1),
-            payment=dt(2023, 4, 1),
-            frequency="A",
-            fixing_method="rfr_payment_delay",
-            float_spread=0.0,
-            stub=True,
-        )
-        with pytest.raises(ValueError, match="Must supply a valid curve for forecasting"):
-            period.rate({"rfr": curve})
+    npv_base = pf.npv(solver=solver, base="eur")
+    expected_npv = -6230451.035973
+    assert (npv_base - expected_npv) < 1e-5
+
+    delta_base = pf.delta(solver=solver, base="usd")
+    # this expectation is directly input from reviewed output.
+    expected_delta = DataFrame(
+        data=[
+            [3.51021, 0.0, 3.51021],
+            [-0.00005, 0.0, -0.00005],
+            [101841.37433, 97001.98184, 101841.37433],
+            [85750.45235, 81672.83139, 85750.45235],
+            [-3.55593, 0.0, -3.55593],
+            [0.00004, 0.0, 0.00004],
+            [-623.00136, 0.0, -623.00136],
+        ],
+        index=MultiIndex.from_tuples(
+            [
+                ("instruments", "sofr", "10y"),
+                ("instruments", "sofr", "10y10y"),
+                ("instruments", "estr", "10y"),
+                ("instruments", "estr", "10y10y"),
+                ("instruments", "xccy", "10y"),
+                ("instruments", "xccy", "10y10y"),
+                ("fx", "fx", "eurusd"),
+            ],
+            names=["type", "solver", "label"],
+        ),
+        columns=MultiIndex.from_tuples(
+            [("all", "usd"), ("eur", "eur"), ("eur", "usd")], names=["local_ccy", "display_ccy"]
+        ),
+    )
+    assert_frame_equal(delta_base, expected_delta, atol=1e-2, rtol=1e-4)
 
-    def test_ibor_stub_fixings_table(self):
-        period = FloatPeriod(
-            start=dt(2023, 2, 1),
-            end=dt(2023, 4, 1),
-            payment=dt(2023, 4, 1),
-            frequency="A",
-            fixing_method="ibor",
-            method_param=1,
-            float_spread=0.0,
-            stub=True,
-        )
-        curve3 = LineCurve({dt(2022, 1, 1): 3.0, dt(2023, 2, 1): 3.0})
-        curve1 = LineCurve({dt(2022, 1, 1): 1.0, dt(2023, 2, 1): 1.0})
-        result = period.fixings_table({"1M": curve1, "3m": curve3}, disc_curve=curve1)
-        expected = DataFrame(
-            data=[[-1e6, None, 2.01639]],
-            index=Index([dt(2023, 1, 31)], name="obs_dates"),
-            columns=["notional", "dcf", "rates"],
-        )
-        assert_frame_equal(result, expected)
+    gamma_base = pf.gamma(solver=solver, base="usd", local=True)  # local overrrides base to EUR
+    expected_gamma = DataFrame(
+        data=[
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, -102.972447, -81.00807888, 0.0, 0.0, 0.0],
+            [0.0, 0.0, -81.00807888, -87.84105303, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        ],
+        index=MultiIndex.from_tuples(
+            [
+                ("eur", "eur", "instruments", "sofr", "10y"),
+                ("eur", "eur", "instruments", "sofr", "10y10y"),
+                ("eur", "eur", "instruments", "estr", "10y"),
+                ("eur", "eur", "instruments", "estr", "10y10y"),
+                ("eur", "eur", "instruments", "xccy", "10y"),
+                ("eur", "eur", "instruments", "xccy", "10y10y"),
+                ("eur", "eur", "fx", "fx", "eurusd"),
+            ],
+            names=["local_ccy", "display_ccy", "type", "solver", "label"],
+        ),
+        columns=MultiIndex.from_tuples(
+            [
+                ("instruments", "sofr", "10y"),
+                ("instruments", "sofr", "10y10y"),
+                ("instruments", "estr", "10y"),
+                ("instruments", "estr", "10y10y"),
+                ("instruments", "xccy", "10y"),
+                ("instruments", "xccy", "10y10y"),
+                ("fx", "fx", "eurusd"),
+            ],
+            names=["type", "solver", "label"],
+        ),
+    )
+    assert_frame_equal(gamma_base, expected_gamma, atol=1e-2, rtol=1e-4)
 
-    def test_local_historical_pay_date_issue(self, curve):
-        period = FloatPeriod(dt(2021, 1, 1), dt(2021, 4, 1), dt(2021, 4, 1), "Q")
-        result = period.npv(curve, local=True)
-        assert result == {"usd": 0.0}
-
-
-class TestFixedPeriod:
-    def test_fixed_period_analytic_delta(self, curve, fxr):
-        fixed_period = FixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            currency="usd",
-        )
-        result = fixed_period.analytic_delta(curve)
-        assert abs(result - 24744.478172244584) < 1e-7
 
-        result = fixed_period.analytic_delta(curve, curve, fxr, "nok")
-        assert abs(result - 247444.78172244584) < 1e-7
+def test_gamma_with_fxrates_ad_order_1_raises():
+    # when calculating gamma, AD order 2 is needed, the fx rates object passed
+    # must also be converted. TODO
+    pass
 
-    def test_fixed_period_analytic_delta_fxr_base(self, curve, fxr):
-        fixed_period = FixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            currency="usd",
-        )
-        fxr = FXRates({"usdnok": 10.0}, base="NOK")
-        result = fixed_period.analytic_delta(curve, curve, fxr)
-        assert abs(result - 247444.78172244584) < 1e-7
 
-    @pytest.mark.parametrize(
-        "rate, crv, fx",
-        [
-            (4.00, True, 2.0),
-            (NoInput(0), False, 2.0),
-            (4.00, True, 10),
-            (NoInput(0), False, 10),
+def test_error_labels():
+    solver_with_error = Solver(
+        curves=[
+            Curve(
+                nodes={dt(2022, 1, 1): 1.0, dt(2022, 7, 1): 1.0, dt(2023, 1, 1): 1.0}, id="curve1"
+            )
+        ],
+        instruments=[
+            IRS(dt(2022, 1, 1), "1M", "A", curves="curve1"),
+            IRS(dt(2022, 1, 1), "2M", "A", curves="curve1"),
+            IRS(dt(2022, 1, 1), "3M", "A", curves="curve1"),
+            IRS(dt(2022, 1, 1), "4M", "A", curves="curve1"),
+            IRS(dt(2022, 1, 1), "8M", "A", curves="curve1"),
+            IRS(dt(2022, 1, 1), "12M", "A", curves="curve1"),
         ],
+        s=[2.0, 2.2, 2.3, 2.4, 2.45, 2.55],
+        id="rates",
     )
-    def test_fixed_period_cashflows(self, curve, fxr, rate, crv, fx):
-        # also test the inputs to fx as float and as FXRates (10 is for
-        fixed_period = FixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            fixed_rate=rate,
-        )
+    result = solver_with_error.error
+    assert abs(result.loc[("rates", "rates0")] - 22.798) < 1e-2
 
-        cashflow = None if rate is NoInput.blank else rate * -1e9 * fixed_period.dcf / 100
-        expected = {
-            Defaults.headers["type"]: "FixedPeriod",
-            Defaults.headers["stub_type"]: "Regular",
-            Defaults.headers["a_acc_start"]: dt(2022, 1, 1),
-            Defaults.headers["a_acc_end"]: dt(2022, 4, 1),
-            Defaults.headers["payment"]: dt(2022, 4, 3),
-            Defaults.headers["notional"]: 1e9,
-            Defaults.headers["currency"]: "USD",
-            Defaults.headers["convention"]: "Act360",
-            Defaults.headers["dcf"]: fixed_period.dcf,
-            Defaults.headers["df"]: 0.9897791268897856 if crv else None,
-            Defaults.headers["rate"]: rate,
-            Defaults.headers["spread"]: None,
-            Defaults.headers["npv"]: -9897791.268897856 if crv else None,
-            Defaults.headers["cashflow"]: cashflow,
-            Defaults.headers["fx"]: fx,
-            Defaults.headers["npv_fx"]: -9897791.268897855 * fx if crv else None,
-            Defaults.headers["collateral"]: None,
-        }
-        if fx == 2.0:
-            with pytest.warns(UserWarning):
-                # supplying `fx` as numeric
-                result = fixed_period.cashflows(curve if crv else NoInput(0), fx=2.0, base=NoInput(0))
-        else:
-            result = fixed_period.cashflows(curve if crv else NoInput(0), fx=fxr, base="nok")
-        assert result == expected
-
-    def test_fixed_period_npv(self, curve, fxr):
-        fixed_period = FixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
+
+def test_solver_non_unique_id_raises():
+    curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="A")
+    solver = Solver(
+        curves=[curve],
+        instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve,), {})],
+        s=[1],
+        id="bad",
+    )
+    curve2 = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.98}, id="B")
+    with pytest.raises(ValueError, match="Solver `id`s must be unique"):
+        Solver(
+            curves=[curve2],
+            instruments=[(IRS(dt(2022, 1, 1), "1Y", "Q"), (curve2,), {})],
+            s=[1],
+            id="bad",
+            pre_solvers=[solver],
         )
-        result = fixed_period.npv(curve)
-        assert abs(result + 9897791.268897833) < 1e-7
 
-        result = fixed_period.npv(curve, curve, fxr, "nok")
-        assert abs(result + 98977912.68897833) < 1e-6
 
-    def test_fixed_period_npv_raises(self, curve):
-        fixed_period = FixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-        )
-        with pytest.raises(
-            TypeError,
-            match=re.escape("`curves` have not been supplied correctly.")
-        ):
-            fixed_period.npv()
+def test_solving_indirect_parameters_from_proxy_composite():
+    eureur = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="eureur")
+    eurspd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.999}, id="eurspd")
+    eur3m = CompositeCurve([eureur, eurspd], id="eur3m")
+    usdusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="usdusd")
+    eurusd = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 1.0}, id="eurusd")
+    fxr = FXRates({"eurusd": 1.1}, settlement=dt(2022, 1, 3))
+    fxf = FXForwards(
+        fx_rates=fxr,
+        fx_curves={
+            "eureur": eureur,
+            "usdusd": usdusd,
+            "eurusd": eurusd,
+        },
+    )
+    usdeur = fxf.curve("usd", "eur", id="usdeur")
+    instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", currency="eur", curves=["eur3m", "eureur"]),
+        IRS(dt(2022, 1, 1), "1Y", "A", currency="usd", curves="usdusd"),
+        XCS(
+            dt(2022, 1, 1),
+            "1Y",
+            "A",
+            currency="eur",
+            leg2_currency="usd",
+            curves=["eureur", "eureur", "usdusd", "usdeur"],
+        ),
+    ]
+    Solver(
+        curves=[eureur, eur3m, usdusd, eurusd, usdeur],
+        instruments=instruments,
+        s=[2.0, 2.7, -15],
+        fx=fxf,
+    )
+
 
+def test_solver_dimensions_of_matmul():
+    swaps = [
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="chf", currency="chf"),
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="gbp", currency="gbp"),
+        IRS(dt(2023, 7, 21), "9m", "A", fixed_rate=2.0, curves="usd", currency="usd"),
+    ]
+    chf_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="chf", currency="chf"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="chf", currency="chf"),
+    ]
+    gbp_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="gbp", currency="gbp"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="gbp", currency="gbp"),
+    ]
+    usd_inst = [
+        IRS(dt(2023, 7, 21), "6m", "A", curves="usd", currency="usd"),
+        IRS(dt(2023, 7, 21), "1y", "A", curves="usd", currency="usd"),
+    ]
+    usd = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="usd",
+    )
+    gbp = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="gbp",
+    )
+    chf = Curve(
+        {dt(2023, 7, 21): 1.0, dt(2024, 1, 21): 1.0, dt(2024, 7, 21): 1.0},
+        id="chf",
+    )
+    fxr = FXRates({"gbpusd": 1.25, "chfgbp": 1.1})
+    solver1 = Solver(curves=[chf], instruments=chf_inst, s=[1.5, 1.8], id="CHF")
+    solver2 = Solver(
+        curves=[gbp], instruments=gbp_inst, s=[1.6, 1.7], id="GBP", pre_solvers=[solver1]
+    )
+    solver3 = Solver(
+        curves=[usd], instruments=usd_inst, s=[1.7, 1.9], id="USD", pre_solvers=[solver2]
+    )
+    pf = Portfolio(swaps)
+    pf.delta(solver=solver3, base="gbp", fx=fxr)
+    pf.gamma(solver=solver3, base="gbp", fx=fxr)
+
+
+def test_pre_solver_single_fx_object():
+    # this test considers building up FXForwards using chined solvers.
+    uu = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="uu")
+    ee = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="ee")
+    gg = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="gg")
+    eu = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="eu")
+    gu = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99}, id="gu")
+
+    fxf1 = FXForwards(
+        fx_rates=FXRates({"eurusd": 1.0}, settlement=dt(2022, 1, 1)),
+        fx_curves={
+            "usdusd": uu,
+            "eureur": ee,
+            "eurusd": eu,
+        },
+    )
 
-class TestCashflow:
-    def test_cashflow_analytic_delta(self, curve):
-        cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
-        assert cashflow.analytic_delta(curve) == 0
+    fxf2 = FXForwards(
+        fx_rates=FXRates({"eurusd": 1.0, "gbpusd": 1.5}, settlement=dt(2022, 1, 1)),
+        fx_curves={
+            "usdusd": uu,
+            "eureur": ee,
+            "gbpgbp": gg,
+            "eurusd": eu,
+            "gbpusd": gu,
+        },
+    )
 
-    @pytest.mark.parametrize(
-        "crv, fx",
-        [
-            (True, 2.0),
-            (False, 2.0),
-            (True, 10.0),
-            (False, 10.0),
+    s1 = Solver(
+        curves=[uu, ee, gg],
+        instruments=[
+            IRS(dt(2022, 1, 1), "1y", "A", curves="uu"),
+            IRS(dt(2022, 1, 1), "1y", "A", curves="ee"),
+            IRS(dt(2022, 1, 1), "1y", "A", curves="gg"),
         ],
+        s=[1.5, 1.5, 1.0],
+        id="local",
     )
-    def test_cashflow_cashflows(self, curve, fxr, crv, fx):
-        cashflow = Cashflow(notional=1e9, payment=dt(2022, 4, 3))
-        curve = curve if crv else NoInput(0)
-        expected = {
-            Defaults.headers["type"]: "Cashflow",
-            Defaults.headers["stub_type"]: None,
-            Defaults.headers["a_acc_start"]: None,
-            Defaults.headers["a_acc_end"]: None,
-            Defaults.headers["payment"]: dt(2022, 4, 3),
-            Defaults.headers["currency"]: "USD",
-            Defaults.headers["notional"]: 1e9,
-            Defaults.headers["convention"]: None,
-            Defaults.headers["dcf"]: None,
-            Defaults.headers["df"]: 0.9897791268897856 if crv else None,
-            Defaults.headers["rate"]: None,
-            Defaults.headers["spread"]: None,
-            Defaults.headers["npv"]: -989779126.8897856 if crv else None,
-            Defaults.headers["cashflow"]: -1e9,
-            Defaults.headers["fx"]: fx,
-            Defaults.headers["npv_fx"]: -989779126.8897856 * fx if crv else None,
-            Defaults.headers["collateral"]: None,
-        }
-        if fx == 2.0:
-            with pytest.warns(UserWarning):
-                # supplying `fx` as numeric
-                result = cashflow.cashflows(
-                    curve if crv else NoInput(0),
-                    fx=2.0,
-                    base=NoInput(0),
-                )
-        else:
-            result = cashflow.cashflows(
-                curve if crv else NoInput(0),
-                fx=fxr,
-                base="nok",
+    s2 = Solver(
+        curves=[eu],
+        instruments=[
+            XCS(
+                dt(2022, 1, 1),
+                "1Y",
+                "Q",
+                currency="eur",
+                leg2_currency="usd",
+                curves=["ee", "eu", "uu", "uu"],
             )
-        assert result == expected
+        ],
+        s=[10.0],
+        id="x1",
+        fx=fxf1,
+        pre_solvers=[s1],
+    )
+    Solver(
+        curves=[gu],
+        instruments=[
+            XCS(
+                dt(2022, 1, 1),
+                "1Y",
+                "Q",
+                currency="gbp",
+                leg2_currency="usd",
+                curves=["gg", "gu", "uu", "uu"],
+            )
+        ],
+        s=[20.0],
+        id="x2",
+        fx=fxf2,
+        pre_solvers=[s2],
+    )
+    result = gu[dt(2023, 1, 1)]
+    expected = 0.988
+    assert (result - expected) < 1e-4
 
-    def test_cashflow_npv_raises(self, curve):
-        with pytest.raises(
-            TypeError,
-            match="`curves` have not been supplied correctly."
-        ):
-            cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
-            cashflow.npv()
-        cashflow = Cashflow(notional=1e6, payment=dt(2022, 1, 1))
-        assert cashflow.analytic_delta(curve) == 0
-
-    def test_cashflow_npv_local(self, curve):
-        cashflow = Cashflow(notional=1e9, payment=dt(2022, 4, 3), currency="nok")
-        result = cashflow.npv(curve, local=True)
-        expected = {"nok": -989779126.8897856}
-        assert result == expected
-
-
-class TestIndexFixedPeriod:
-    @pytest.mark.parametrize(
-        "method, expected", [("daily", 201.00502512562812), ("monthly", 200.98317675333183)]
-    )
-    def test_period_rate(self, method, expected):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-            index_method=method,
-        )
-        index_curve = IndexCurve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-            index_base=200.0,
-        )
-        _, result, _ = index_period.index_ratio(index_curve)
-        assert abs(result - expected) < 1e-8
 
-    def test_period_cashflow(self):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-        )
-        index_curve = IndexCurve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-            index_base=200.0,
-        )
-        result = index_period.real_cashflow
-        expected = -1e7 * ((dt(2022, 4, 1) - dt(2022, 1, 1)) / timedelta(days=360)) * 4
-        assert abs(result - expected) < 1e-8
-
-        result = index_period.cashflow(index_curve)
-        expected = expected * index_curve.index_value(dt(2022, 4, 3)) / 100.0
-        assert abs(result - expected) < 1e-8
-
-    def test_period_analytic_delta(self, fxr, curve):
-        index_curve = IndexCurve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-            index_base=200.0,
-        )
-        fixed_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            currency="usd",
-            index_base=200.0,
-            index_fixings=300.0,
-        )
-        result = fixed_period.analytic_delta(index_curve, curve)
-        assert abs(result - 24744.478172244584 * 300.0 / 200.0) < 1e-7
+def test_solver_jacobians_in_text():
+    par_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2027, 1, 1): 1.0,
+            dt(2032, 1, 1): 1.0
+        },
+        id="curve",
+    )
+    par_instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "2Y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "5Y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "10Y", "A", curves="curve"),
+    ]
+    par_solver = Solver(
+        curves=[par_curve],
+        instruments=par_instruments,
+        s=[1.21, 1.635, 1.885, 1.93],
+        id="par_solver",
+        instrument_labels=["1Y", "2Y", "5Y", "10Y"],
+    )
+    fwd_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+            dt(2027, 1, 1): 1.0,
+            dt(2032, 1, 1): 1.0
+        },
+        id="curve"
+    )
+    fwd_instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+        IRS(dt(2023, 1, 1), "1Y", "A", curves="curve"),
+        IRS(dt(2024, 1, 1), "3Y", "A", curves="curve"),
+        IRS(dt(2027, 1, 1), "5Y", "A", curves="curve"),
+    ]
+    s_fwd = [float(_.rate(solver=par_solver)) for _ in fwd_instruments]
+    fwd_solver = Solver(
+        curves=[fwd_curve],
+        instruments=fwd_instruments,
+        s=s_fwd,
+        id="fwd_solver",
+        instrument_labels=["1Y", "1Y1Y", "2Y3Y", "5Y5Y"],
+    )
+    S_BA = par_solver.jacobian(fwd_solver).to_numpy()
+    S_AB = fwd_solver.jacobian(par_solver).to_numpy()
+    assert np.all(np.isclose(np.eye(4), np.matmul(S_AB, S_BA)))
 
-        result = fixed_period.analytic_delta(index_curve, curve, fxr, "nok")
-        assert abs(result - 247444.78172244584 * 300.0 / 200.0) < 1e-7
 
-    @pytest.mark.parametrize(
-        "fixings, method",
-        [
-            (300.0, "daily"),
-            (
-                Series([1.0, 300, 5], index=[dt(2022, 4, 2), dt(2022, 4, 3), dt(2022, 4, 4)]),
-                "daily",
-            ),
-            (Series([100.0, 500], index=[dt(2022, 4, 2), dt(2022, 4, 4)]), "daily"),
-            (Series([300.0, 500], index=[dt(2022, 4, 1), dt(2022, 4, 5)]), "monthly"),
-        ],
+def test_solver_jacobians_pre():
+    par_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+        },
+        id="curve",
+    )
+    par_instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+        IRS(dt(2022, 1, 1), "2Y", "A", curves="curve"),
+    ]
+    par_solver = Solver(
+        curves=[par_curve],
+        instruments=par_instruments,
+        s=[1.21, 1.635],
+        id="par_solver",
+        instrument_labels=["1Y", "2Y"],
+    )
+    par_curve2 = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+        },
+        id="curve2",
+    )
+    par_instruments2 = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve2"),
+        IRS(dt(2022, 1, 1), "2Y", "A", curves="curve2"),
+    ]
+    par_solver2 = Solver(
+        curves=[par_curve2],
+        instruments=par_instruments2,
+        s=[1.21, 1.635],
+        id="par_solver2",
+        instrument_labels=["1Y", "2Y"],
+        pre_solvers=[par_solver],
     )
-    def test_period_fixings_series(self, fixings, method, curve):
-        fixed_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            currency="usd",
-            index_base=200.0,
-            index_fixings=fixings,
-            index_method=method,
-        )
-        result = fixed_period.analytic_delta(None, curve)
-        assert abs(result - 24744.478172244584 * 300.0 / 200.0) < 1e-7
 
-    def test_period_raises(self):
-        with pytest.raises(ValueError, match="`index_method` must be "):
-            IndexFixedPeriod(
-                start=dt(2022, 1, 1),
-                end=dt(2022, 4, 1),
-                payment=dt(2022, 4, 3),
-                notional=1e9,
-                convention="Act360",
-                termination=dt(2022, 4, 1),
-                frequency="Q",
-                currency="usd",
-                index_base=200.0,
-                index_method="BAD",
-            )
+    fwd_curve = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+        },
+        id="curve"
+    )
+    fwd_instruments = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve"),
+        IRS(dt(2023, 1, 1), "1Y", "A", curves="curve"),
+    ]
+    s_fwd = [float(_.rate(solver=par_solver2)) for _ in fwd_instruments]
+    fwd_solver = Solver(
+        curves=[fwd_curve],
+        instruments=fwd_instruments,
+        s=s_fwd,
+        id="fwd_solver",
+        instrument_labels=["1Y", "1Y1Y"],
+    )
+    fwd_curve2 = Curve(
+        nodes={
+            dt(2022, 1, 1): 1.0,
+            dt(2023, 1, 1): 1.0,
+            dt(2024, 1, 1): 1.0,
+        },
+        id="curve2"
+    )
+    fwd_instruments2 = [
+        IRS(dt(2022, 1, 1), "1Y", "A", curves="curve2"),
+        IRS(dt(2023, 1, 1), "1Y", "A", curves="curve2"),
+    ]
+    s_fwd2 = [float(_.rate(solver=par_solver2)) for _ in fwd_instruments2]
+    fwd_solver2 = Solver(
+        curves=[fwd_curve2],
+        instruments=fwd_instruments2,
+        s=s_fwd2,
+        id="fwd_solver2",
+        instrument_labels=["1Y", "1Y1Y"],
+        pre_solvers=[fwd_solver],
+    )
 
-    def test_period_npv(self, curve):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-        )
-        index_curve = IndexCurve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-            index_base=200.0,
-        )
-        result = index_period.npv(index_curve, curve)
-        expected = -19895057.826930363
-        assert abs(result - expected) < 1e-8
-
-        result = index_period.npv(index_curve, curve, local=True)
-        assert abs(result["usd"] - expected) < 1e-8
-
-    def test_period_npv_raises(self):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-        )
-        with pytest.raises(
-                TypeError,
-                match=re.escape("`curves` have not been supplied correctly.")
-        ):
-            index_period.npv()
-
-    @pytest.mark.parametrize("curve_", [True, False])
-    def test_period_cashflows(self, curve, curve_):
-        curve = curve if curve_ else NoInput(0)
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 4, 1),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 1),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-            index_fixings=200.0,
-        )
-        result = index_period.cashflows(curve)
-        expected = {
-            "Type": "IndexFixedPeriod",
-            "Period": "Regular",
-            "Ccy": "USD",
-            "Acc Start": dt(2022, 1, 1),
-            "Acc End": dt(2022, 4, 1),
-            "Payment": dt(2022, 4, 3),
-            "Convention": "Act360",
-            "DCF": 0.25,
-            "DF": 0.9897791268897856 if curve_ else None,
-            "Notional": 1e9,
-            "Rate": 4.0,
-            "Spread": None,
-            "Cashflow": -20000000.0,
-            "Real Cashflow": -10e6,
-            "Index Base": 100.0,
-            "Index Val": 200.0,
-            "Index Ratio": 2.0,
-            "NPV": -19795582.53779571 if curve_ else None,
-            "FX Rate": 1.0,
-            "NPV Ccy": -19795582.53779571 if curve_ else None,
-            Defaults.headers["collateral"]: None,
-        }
-        assert result == expected
+    S_BA = par_solver2.jacobian(fwd_solver2)
+    S_AB = fwd_solver2.jacobian(par_solver2)
+    assert np.all(np.isclose(np.eye(4), np.matmul(S_AB.to_numpy(), S_BA.to_numpy())))
 
-    def test_cashflow_returns_none(self):
-        i_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 2, 1),
-            payment=dt(2022, 2, 1),
-            frequency="M",
-            index_base=100.0,
-        )
-        assert i_period.cashflow() is None
-        assert i_period.real_cashflow is None
 
-    def test_cashflow_no_index_rate(self):
-        i_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 2, 1),
-            payment=dt(2022, 2, 1),
-            frequency="M",
-            index_base=100.0,
-        )
-        result = i_period.cashflows()
-        assert result[Defaults.headers["index_ratio"]] is None
+def test_newton_solver_1dim_dual():
+    def root(x, s):
+        return x**2 - s, 2*x
 
-    def test_bad_curve(self):
-        i_period = IndexFixedPeriod(
-            start=dt(2022, 1, 1),
-            end=dt(2022, 2, 1),
-            payment=dt(2022, 2, 1),
-            frequency="M",
-            index_base=100.0,
-        )
-        curve = Curve({dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99})
-        with pytest.raises(TypeError, match="`index_value` must be forecast from"):
-            i_period.index_ratio(curve)
-
-    # TEST REDUNDANT: function was changed to fallback to forecast from curve
-    # def test_cannot_forecast_from_fixings(self):
-    #     i_fixings = Series([100], index=[dt(2021, 1, 1)])
-    #     i_period = IndexFixedPeriod(
-    #         start=dt(2022, 1, 1),
-    #         end=dt(2022, 2, 1),
-    #         payment=dt(2022, 2, 1),
-    #         frequency="M",
-    #         index_base=100.0,
-    #         index_fixings=i_fixings,
-    #     )
-    #     curve = IndexCurve(
-    #         {dt(2022, 1, 1): 1.0, dt(2023, 1, 1): 0.99},
-    #         index_lag=3,
-    #         index_base=100.0
-    #     )
-    #     with pytest.raises(ValueError, match="`index_fixings` cannot forecast the"):
-    #         i_period.index_ratio(curve)
-
-    def test_index_fixings_linear_interp(self):
-        i_fixings = Series([173.1, 174.2], index=[dt(2001, 7, 1), dt(2001, 8, 1)])
-        result = IndexMixin._index_value(
-            i_fixings=i_fixings, i_curve=None, i_date=dt(2001, 7, 20), i_lag=3, i_method="daily"
-        )
-        expected = 173.1 + 19 / 31 * (174.2 - 173.1)
-        assert abs(result - expected) < 1e-6
+    x0 = Dual(1.0, ["x"], [])
+    s = Dual(2.0, ["s"], [])
+    result = newton_1dim(root, x0, args=(s,))
 
-    def test_composite_curve(self):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-        )
-        index_curve = IndexCurve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-            index_base=200.0,
-        )
-        composite_curve = CompositeCurve([index_curve])
-        _, result, _ = index_period.index_ratio(composite_curve)
+    expected = 0.5 / 2.0**0.5
+    sensitivity = gradient(result["g"], ["s"])[0]
+    assert abs(expected - sensitivity) < 1e-9
 
-    def test_composite_curve_raises(self):
-        index_period = IndexFixedPeriod(
-            start=dt(2022, 1, 3),
-            end=dt(2022, 4, 3),
-            payment=dt(2022, 4, 3),
-            notional=1e9,
-            convention="Act360",
-            termination=dt(2022, 4, 3),
-            frequency="Q",
-            fixed_rate=4.00,
-            currency="usd",
-            index_base=100.0,
-        )
-        curve = Curve(
-            nodes={dt(2022, 1, 1): 1.0, dt(2022, 4, 3): 0.995},
-        )
-        composite_curve = CompositeCurve([curve])
-        with pytest.raises(TypeError, match="`index_value` must be forecast from"):
-            _, result, _ = index_period.index_ratio(composite_curve)
-
-
-class TestIndexCashflow:
-    def test_cashflow_analytic_delta(self, curve):
-        cashflow = IndexCashflow(notional=1e6, payment=dt(2022, 1, 1), index_base=100)
-        assert cashflow.analytic_delta(curve) == 0
-
-    def test_index_cashflow(self):
-        cf = IndexCashflow(notional=1e6, payment=dt(2022, 1, 1), index_base=100, index_fixings=200)
-        assert cf.real_cashflow == -1e6
-
-        assert cf.cashflow(None) == -2e6
-
-    def test_index_cashflow_npv(self, curve):
-        cf = IndexCashflow(notional=1e6, payment=dt(2022, 1, 1), index_base=100, index_fixings=200)
-        assert abs(cf.npv(curve) + 2e6) < 1e-6
-
-    def test_cashflow_no_index_rate(self):
-        i_period = IndexCashflow(
-            notional=200.0,
-            payment=dt(2022, 2, 1),
-            index_base=100.0,
-        )
-        result = i_period.cashflows()
-        assert result[Defaults.headers["index_ratio"]] is None
 
-    def test_index_only(self, curve):
-        cf = IndexCashflow(
-            notional=1e6,
-            payment=dt(2022, 1, 1),
-            index_base=100,
-            index_fixings=200,
-            index_only=True,
-        )
-        assert abs(cf.npv(curve) + 1e6) < 1e-6
+def test_newton_solver_1dim_dual2():
+    def root(x, s):
+        return x**2 - s, 2*x
+
+    x0 = Dual2(1.0, ["x"], [], [])
+    s = Dual2(2.0, ["s"], [], [])
+    result = newton_1dim(root, x0, args=(s,))
+
+    expected = 0.5 / 2.0**0.5
+    sensitivity = gradient(result["g"], ["s"])[0]
+    assert abs(expected - sensitivity) < 1e-9
+
+    expected = -0.25 * (1 / 2.0**1.5)
+    sensitivity = gradient(result["g"], ["s"], order=2)[0, 0]
+    assert abs(expected - sensitivity) < 1e-9
+
+
+def test_newton_solver_2dim_dual():
+    def root(g, s):
+        f0 = g[0] ** 2 + g[1] ** 2 + s
+        f1 = g[0] ** 2 - 2 * g[1]**2 - s
+
+        f00 = 2 * g[0]
+        f01 = 2 * g[1]
+        f10 = 2 * g[0]
+        f11 = -4 * g[1]
+
+        return [f0, f1], [[f00, f01], [f10, f11]]
+
+    g0 = [Dual(1.0, ["x"], []), Dual(2.0, ["y"], [])]
+    s = Dual(-2.0, ["s"], [])
+    result = newton_ndim(root, g0, args=(s,))
+
+    expected_x = (2/3)**0.5
+    assert abs(result["g"][0] - expected_x) < 1e-9
+
+    expected_y = (4/3)**0.5
+    assert abs(result["g"][1] - expected_y) < 1e-9
+
+    expected_y = -0.5 * (2/3)**0.5 * (2.0)**-0.5
+    expected_x = -0.5 * (1/3.0)**0.5 * (2.0)**-0.5
+
+    sensitivity_x = gradient(result["g"][0], ["s"])[0]
+    sensitivity_y = gradient(result["g"][1], ["s"])[0]
+    assert abs(expected_x - sensitivity_x) < 1e-9
+    assert abs(expected_y - sensitivity_y) < 1e-9
+
+
+def test_newton_solver_2dim_dual2():
+    def root(g, s):
+        f0 = g[0] ** 2 + g[1] ** 2 + s
+        f1 = g[0] ** 2 - 2 * g[1]**2 - s
+
+        f00 = 2 * g[0]
+        f01 = 2 * g[1]
+        f10 = 2 * g[0]
+        f11 = -4 * g[1]
+
+        return [f0, f1], [[f00, f01], [f10, f11]]
+
+    g0 = [Dual2(1.0, ["x"], [], []), Dual2(2.0, ["y"], [], [])]
+    s = Dual2(-2.0, ["s"], [], [])
+    result = newton_ndim(root, g0, args=(s,))
+
+    expected_x = (2 / 3) ** 0.5
+    assert abs(result["g"][0] - expected_x) < 1e-9
+    expected_y = (4 / 3) ** 0.5
+    assert abs(result["g"][1] - expected_y) < 1e-9
+
+    expected_y = -0.5 * (2 / 3) ** 0.5 * (2.0) ** -0.5
+    expected_x = -0.5 * (1 / 3.0) ** 0.5 * (2.0) ** -0.5
+    sensitivity_x = gradient(result["g"][0], ["s"])[0]
+    sensitivity_y = gradient(result["g"][1], ["s"])[0]
+    assert abs(expected_x - sensitivity_x) < 1e-9
+    assert abs(expected_y - sensitivity_y) < 1e-9
+
+    expected_y2 = -0.25 * (2/3)**0.5 * (2.0) ** -1.5
+    expected_x2 = -0.25 * (1/3) ** 0.5 * (2.0) ** -1.5
+    sensitivity_x2 = gradient(result["g"][0], ["s"], order=2)[0, 0]
+    sensitivity_y2 = gradient(result["g"][1], ["s"], order=2)[0, 0]
+    assert abs(expected_x2 - sensitivity_x2) < 1e-9
+    assert abs(expected_y2 - sensitivity_y2) < 1e-9
 
-    def test_index_cashflow_floats(self, curve):
-        icurve = IndexCurve(
-            nodes = {
-                dt(2022, 1, 1): 1.00,
-                dt(2022, 4, 1): 0.99,
-                dt(2022, 7, 1): 0.98,
-                dt(2022, 10, 1): 0.97,
-            },
-            index_base=100.0,
-        )
-        icurve._set_ad_order(1)
-        curve._set_ad_order(1)
-        cf = IndexCashflow(notional=1e6, payment=dt(2022, 7, 1), index_base=100)
-        result = cf.cashflows(icurve, curve)
-        assert isinstance(result["Cashflow"], float)
 
+def test_newton_1d_failed_state():
+    def root(g):
+        f0 = g**2 + 10.0
+        f1 = 2 * g
+        return f0, f1
 
-def test_base_period_dates_raise():
-    with pytest.raises(ValueError):
-        _ = FixedPeriod(dt(2023, 1, 1), dt(2022, 1, 1), dt(2024, 1, 1), "Q")
+    result = newton_1dim(root, 1.5, max_iter=5, raise_on_fail=False)
+    assert result["state"] == -1
+
+
+def test_newton_ndim_raises():
+    def root(g):
+        f0_0 = g[0]**2 + 10.0
+        f0_1 = g[0] + g[1]**2 - 2.0
+        return [f0_0, f0_1], [[2*g[0], 0.0], [1.0, 2*g[1]]]
+
+    with pytest.raises(ValueError, match="`max_iter`: 5 exceeded in 'newton_ndim'"):
+        newton_ndim(root, [0.5, 1.0], max_iter=5)
+
+
+def test_solver_with_vol_smile():
+    eureur = Curve({dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.9851909811629752}, calendar="tgt", id="eureur")
+    usdusd = Curve({dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.976009366603271}, calendar="nyc", id="usdusd")
+    # eurusd = Curve({dt(2023, 3, 16): 1.0, dt(2023, 9, 16): 0.987092591908283}, id="eurusd")
+    fxr = FXRates({"eurusd": 1.3088}, settlement=dt(2023, 3, 20))
+    fxf = FXForwards(
+        fx_curves={"eureur": eureur, "eurusd": eureur, "usdusd": usdusd},
+        fx_rates=fxr
+    )
+    fxf._set_ad_order(1)
+    solver = Solver(
+        curves=[eureur, usdusd],
+        instruments=[
+            IRS(dt(2023, 3, 20), "1m", curves=[eureur], spec="eur_irs"),
+            IRS(dt(2023, 3, 20), "1m", curves=[usdusd], spec="usd_irs"),
+        ],
+        s=[2.0113, 0.3525],
+        fx=fxf,
+    )
+    eurusd_1m_smile = FXDeltaVolSmile(
+        nodes={
+            0.25: 10.0,
+            0.50: 10.0,
+            0.75: 10.0,
+        },
+        eval_date=dt(2023, 3, 16),
+        expiry=dt(2023, 4, 18),
+        delta_type="spot",
+        id="smile",
+        )
+    args = {
+        "pair": "eurusd",
+        "expiry": dt(2023, 4, 18),
+        "curves": [None, "eureur", None, "usdusd"],
+        "delta_type": "spot",
+        "vol": "smile"
+    }
+    solver2 = Solver(
+        pre_solvers=[solver],
+        curves=[eurusd_1m_smile],
+        instruments=[
+            FXStraddle(strike="atm_delta", **args),
+            FXRiskReversal(strike=["-25d", "25d"], **args),
+            FXStrangle(strike=["-25d", "25d"], **args)
+        ],
+        s=[21.6215, -0.5, 22.359],
+        fx=fxf,
+    )
+
+def test_solver_with_surface():
+    eureur = Curve({dt(2024, 5, 7): 1.0, dt(2025, 5, 30): 1.0}, calendar="tgt", id="eureur")
+    eurusd = Curve({dt(2024, 5, 7): 1.0, dt(2025, 5, 30): 1.0}, id="eurusd")
+    usdusd = Curve({dt(2024, 5, 7): 1.0, dt(2025, 5, 30): 1.0}, calendar="nyc", id="usdusd")
+    # Create an FX Forward market with spot FX rate data
+    fxf = FXForwards(
+        fx_rates=FXRates({"eurusd": 1.0760}, settlement=dt(2024, 5, 9)),
+        fx_curves={"eureur": eureur, "usdusd": usdusd, "eurusd": eurusd},
+    )
+    solver = Solver(
+        curves=[eureur, eurusd, usdusd],
+        instruments=[
+            IRS(dt(2024, 5, 9), "3W", spec="eur_irs", curves="eureur"),
+            IRS(dt(2024, 5, 9), "3W", spec="usd_irs", curves="usdusd"),
+            FXSwap(dt(2024, 5, 9), "3W", currency="eur", leg2_currency="usd", curves=[None, "eurusd", None, "usdusd"]),
+        ],
+        s=[3.90, 5.32, 8.85],
+        instrument_labels=["3w EU", "3w US", "3w FXSw"],
+        fx=fxf,
+    )
+    surface = FXDeltaVolSurface(
+        eval_date=dt(2024, 5, 7),
+        expiries=[dt(2024, 5, 28), dt(2024, 6, 7)],
+        delta_indexes=[0.1, 0.25, 0.5, 0.75, 0.9],
+        delta_type="forward",
+        node_values=np.ones(shape=(2, 5)) * 5.0,
+        id="eurusd_vol",
+    )
+    data = DataFrame(
+        data=[
+            [5.493, -0.157, 0.071, -0.289, 0.238],
+            [5.525, -0.213, 0.075, -0.400, 0.250],
+        ],
+        columns=["ATM", "25dRR", "25dBF", "10dRR", "25dBF"],
+        index=[dt(2024, 5, 28), dt(2024, 6, 7)]
+    )
+    fx_args = dict(
+        pair="eurusd",
+        delta_type="spot",
+        calendar="tgt",
+        curves=[None, "eurusd", None, "usdusd"],
+        vol="eurusd_vol"
+    )
+    instruments, s, labels = [], [], []
+    for e, row in enumerate(data.itertuples()):
+        instruments.extend([
+            FXStraddle(strike="atm_delta", expiry=row[0], **fx_args),
+            FXRiskReversal(strike=["-25d", "25d"], expiry=row[0], **fx_args),
+            FXBrokerFly(strike=["-25d", "atm_delta", "25d"], expiry=row[0], **fx_args),
+            FXRiskReversal(strike=["-10d", "10d"], expiry=row[0], **fx_args),
+            FXBrokerFly(strike=["-10d", "atm_delta", "10d"], expiry=row[0], **fx_args),
+        ])
+        s.extend([row[1], row[2], row[3], row[4], row[5]])
+        labels.extend([f"atm{e}", f"25rr{e}", f"25bf{e}", f"10rr{e}", f"10bf{e}"])
+    surf_solver = Solver(
+        surfaces=[surface],
+        instruments=instruments,
+        s=s,
+        pre_solvers=[solver],
+        instrument_labels=labels,
+        fx=fxf,
+    )
+    fxc = FXCall(
+        expiry=dt(2024, 6, 7),
+        strike=1.08,
+        **fx_args
+    )
+    fxc.analytic_greeks(solver=surf_solver)
+    fxc.delta(solver=surf_solver)
+    fxc.gamma(solver=surf_solver)
```

### Comparing `rateslib-1.1.1/tests/test_scheduling.py` & `rateslib-1.2.0/tests/test_scheduling.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,18 +117,18 @@
         assert result[1]["back_stub"] == exp_stub
         assert result[1]["roll"] == exp_roll
 
 
 @pytest.mark.parametrize(
     "e, t, stub, exp_roll, exp_stub",
     [
-        (dt(2022, 2, 26), dt(2024, 2, 26), "SHORTFRONT", 26, None),
-        (dt(2022, 2, 26), dt(2024, 2, 26), "LONGFRONT", 26, None),
-        (dt(2022, 2, 26), dt(2024, 2, 26), "SHORTBACK", 26, None),
-        (dt(2022, 2, 26), dt(2024, 2, 26), "LONGBACK", 26, None),
+        (dt(2022, 2, 26), dt(2024, 2, 26), "SHORTFRONT", 26, NoInput(0)),
+        (dt(2022, 2, 26), dt(2024, 2, 26), "LONGFRONT", 26, NoInput(0)),
+        (dt(2022, 2, 26), dt(2024, 2, 26), "SHORTBACK", 26, NoInput(0)),
+        (dt(2022, 2, 26), dt(2024, 2, 26), "LONGBACK", 26, NoInput(0)),
     ],
 )
 def test_infer_stub_date_no_inference_on_regular(e, t, stub, exp_roll, exp_stub, cal_):
     result = _infer_stub_date(e, t, "Q", stub, NoInput(0), NoInput(0), "MF", False, NoInput(0), cal_)
     assert result[0]
     if "FRONT" in stub:
         assert result[1]["front_stub"] == exp_stub
@@ -148,15 +148,15 @@
         dt(2024, 2, 26),
         "MF",
         NoInput(0),
         NoInput(0),
         cal_,
     )
     assert result[0]
-    assert result[1]["front_stub"] is None
+    assert result[1]["front_stub"] is NoInput(0)
     assert result[1]["roll"] == 26
 
     result = _infer_stub_date(
         dt(2022, 2, 26),
         dt(2024, 4, 26),
         "Q",
         "FRONTSHORTBACK",
@@ -164,15 +164,15 @@
         NoInput(0),
         "MF",
         NoInput(0),
         NoInput(0),
         cal_,
     )
     assert result[0]
-    assert result[1]["back_stub"] is None
+    assert result[1]["back_stub"] is NoInput(0)
     assert result[1]["roll"] == 26
 
 
 @pytest.mark.parametrize(
     "e, t, stub",
     [
         (dt(2022, 2, 26), dt(2024, 4, 22), "SHORTFRONT"),
@@ -427,31 +427,31 @@
 @pytest.mark.parametrize(
     "effective, termination, uf, ub, roll, expected",
     [
         (
             dt(2023, 2, 4),
             dt(2023, 9, 4),
             dt(2023, 3, 4),
-            None,
+            NoInput(0),
             4,
             [dt(2023, 2, 4), dt(2023, 3, 4), dt(2023, 6, 4), dt(2023, 9, 4)],
         ),
         (
             dt(2023, 2, 4),
             dt(2023, 9, 4),
-            None,
+            NoInput(0),
             dt(2023, 8, 4),
             4,
             [dt(2023, 2, 4), dt(2023, 5, 4), dt(2023, 8, 4), dt(2023, 9, 4)],
         ),
         (
             dt(2023, 3, 4),
             dt(2023, 9, 4),
-            None,
-            None,
+            NoInput(0),
+            NoInput(0),
             4,
             [dt(2023, 3, 4), dt(2023, 6, 4), dt(2023, 9, 4)],
         ),
         (
             dt(2023, 2, 4),
             dt(2023, 10, 4),
             dt(2023, 3, 4),
```

