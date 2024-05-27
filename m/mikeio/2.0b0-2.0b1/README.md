# Comparing `tmp/mikeio-2.0b0.tar.gz` & `tmp/mikeio-2.0b1.tar.gz`

## Comparing `mikeio-2.0b0.tar` & `mikeio-2.0b1.tar`

### file list

```diff
@@ -1,233 +1,234 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mikeio-2.0b0/.gitattributes
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 mikeio-2.0b0/CITATION.cff
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 mikeio-2.0b0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 mikeio-2.0b0/CONTRIBUTING.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 mikeio-2.0b0/Dependencies.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mikeio-2.0b0/License.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mikeio-2.0b0/MANIFEST.in
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mikeio-2.0b0/Makefile
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mikeio-2.0b0/conftest.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 mikeio-2.0b0/mypy.ini
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mikeio-2.0b0/pytest.ini
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mikeio-2.0b0/requirements_min.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mikeio-2.0b0/setup.cfg
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mikeio-2.0b0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/docs_dead_links.yml
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/downstream_test.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/full_test.yml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/legacy_test.yml
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/notebooks_test.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/perf_test.yml
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mikeio-2.0b0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/.gitignore
--rw-r--r--   0        0        0    17564 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/MIKE-IO-Icon-Pos-RGB.png
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/MIKE-IO-Logo-Pos-RGB.svg
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_quarto.yml
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_sidebar.yml
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/design.qmd
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/index.qmd
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/_extension.yml
--rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/fontawesome.lua
--rw-r--r--   0        0        0   140200 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/css/all.css
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/css/latex-fontsize.css
--rw-r--r--   0        0        0   180104 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.ttf
--rw-r--r--   0        0        0    92140 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.woff2
--rw-r--r--   0        0        0    76072 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.ttf
--rw-r--r--   0        0        0    25124 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.woff2
--rw-r--r--   0        0        0   384736 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.ttf
--rw-r--r--   0        0        0   133940 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.woff2
--rw-r--r--   0        0        0   181852 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   105536 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    23940 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   388460 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   154228 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/interlinks/interlinks.lua
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0  1458641 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_inv/numpy_objects.json
--rw-r--r--   0        0        0  3527650 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_inv/pandas_objects.json
--rw-r--r--   0        0        0  2070099 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_inv/scipy_objects.json
--rw-r--r--   0        0        0  1808234 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/_inv/xarray_objects.json
--rw-r--r--   0        0        0   544223 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/BW_Ronne_Layout1998_rotated.dfs2
--rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/BW_Ronne_Layout1998_rotated_crop.dfs2
--rw-r--r--   0        0        0   127789 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/FakeLake.dfsu
--rw-r--r--   0        0        0    54573 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/FakeLake_NONUTM.dfsu
--rw-r--r--   0        0        0   241633 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/Grid1.dfs3
--rw-r--r--   0        0        0   166091 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/HD2D.dfsu
--rw-r--r--   0        0        0   256944 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/Karup_MIKE_SHE_head_output.dfs3
--rw-r--r--   0        0        0   279558 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/Karup_MIKE_SHE_output.dfs2
--rw-r--r--   0        0        0    90438 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/M3WFM_sponge_local_coordinates.dfs2
--rw-r--r--   0        0        0   232505 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/MIKE21SW_dir_sector_area_spectra.dfsu
--rw-r--r--   0        0        0   555625 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/NorthSea_HD_and_windspeed.dfsu
--rw-r--r--   0        0        0   180184 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/Slottskogen.asc.zip
--rw-r--r--   0        0        0   365148 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/State_Area.dfsu
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/State_wlbc_north_err.dfs1
--rw-r--r--   0        0        0   110332 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/altimetry_NorthSea_20171027.csv
--rw-r--r--   0        0        0    28491 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/area_freq_spectra.dfsu
--rw-r--r--   0        0        0   196493 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/area_spectra.dfsu
--rw-r--r--   0        0        0    72175 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/basin_2dv.dfsu
--rw-r--r--   0        0        0   181575 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/basin_3d.dfsu
--rw-r--r--   0        0        0    32045 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/co2-mm-mlo.csv
--rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/da_diagnostic.dfs0
--rw-r--r--   0        0        0    19605 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/dir_wave_analysis_spectra.dfs2
--rw-r--r--   0        0        0   694129 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/dissolved_oxygen.dfs3
--rw-r--r--   0        0        0    20829 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/eq.dfs2
--rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/eq_relative.dfs0
--rw-r--r--   0        0        0   268841 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/europe_wind_long_lat.dfs2
--rw-r--r--   0        0        0   120232 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/gebco_2020_n56.3_s55.2_w12.2_e13.1.nc
--rw-r--r--   0        0        0   228707 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/gebco_sound.dfs2
--rw-r--r--   0        0        0    84666 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/gebco_sound_crop_rotate.dfs2
--rw-r--r--   0        0        0    49641 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/gfs_wind.nc
--rw-r--r--   0        0        0   337299 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/global_long_lat_pacific_view_temperature_delta.dfs2
--rw-r--r--   0        0        0   649616 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/hd_vertical_slice.dfs2
--rw-r--r--   0        0        0   386188 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/kalundborg_coarse.mesh
--rw-r--r--   0        0        0   457167 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/kalundborg_transect.dfsu
--rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/line_dir_spectra.dfsu
--rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/line_freq_spectra.dfsu
--rw-r--r--   0        0        0    67078 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/line_spectra.dfsu
--rw-r--r--   0        0        0   186688 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/many_items.dfs0
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/neq_daily_time_unit.dfs0
--rw-r--r--   0        0        0   123639 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/north_sea_2.mesh
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/nx1.dfs1
--rw-r--r--   0        0        0    38048 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/odense_rough.mesh
--rw-r--r--   0        0        0    38048 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/odense_rough2.MESH
--rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/oresundHD_run1.dfsu
--rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/oresundHD_run2.dfsu
--rw-r--r--   0        0        0  1511214 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/oresund_sigma_z.dfsu
--rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/oresund_vertical_slice.dfsu
--rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/oresund_vertical_slice2.DFSU
--rw-r--r--   0        0        0    91216 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/physical_basin_wave_maker_signal.dfs1
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/positions.xyz
--rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pt_freq_spectra.dfsu
--rw-r--r--   0        0        0    50550 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pt_spectra.dfs2
--rw-r--r--   0        0        0    76049 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pt_spectra.dfsu
--rw-r--r--   0        0        0    51017 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/quad_tri.mesh
--rw-r--r--   0        0        0    22816 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/random.dfs0
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/random.dfs1
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/random.dfs2
--rw-r--r--   0        0        0    22826 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/random_timestepunit_hours.dfs0
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/random_two_item.dfs2
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/single_layer.dfs3
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/single_row.dfs2
--rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/single_time_dt_zero.dfs2
--rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/single_timestep.dfs3
--rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/sw_points.dfs0
--rw-r--r--   0        0        0    77771 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/template.sw
--rw-r--r--   0        0        0    57490 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/template_modified.sw
--rw-r--r--   0        0        0    97752 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/test_dfs3.dfs3
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/tide1.dfs1
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/tide12.dfs1
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/tide2.dfs1
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/tide2_offset.dfs1
--rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/tide4.dfs1
--rw-r--r--   0        0        0    76208 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/track_extraction_case02_indata.dfsu
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/track_extraction_case02_track.csv
--rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/txconc.dfs1
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/untitled_3_items.dfs0
--rw-r--r--   0        0        0    99633 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/utm_not_rotated_neurope_temp.dfs2
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/uv_vertical_daily.dfs2
--rw-r--r--   0        0        0    74421 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/vu_tide_hourly.dfs1
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/water.xyz
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/waterlevel_north.dfs1
--rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/waterlevel_viken.dfs0
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/waves.dfs0
--rw-r--r--   0        0        0    40056 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/waves.dfs2
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/waves2.DFS0
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/winches.xyz
--rw-r--r--   0        0        0    87261 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/wind_north_sea.dfsu
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/consistency/oresundHD.dfs0
--rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/consistency/oresundHD.dfs1
--rw-r--r--   0        0        0    19471 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/consistency/oresundHD.dfs2
--rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/consistency/oresundHD.dfsu
--rw-r--r--   0        0        0   131823 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/Karup_basic.she
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/Karup_mini.she
--rw-r--r--   0        0        0    73742 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/OresundHD2D_EnKF10.m21fm
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/Setup_WaveSpectraConverter.21t
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/concat.mzt
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/filenames.pfs
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/grid1.gsf
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/illegal.pfs
--rw-r--r--   0        0        0    95804 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/lake.m21fm
--rw-r--r--   0        0        0    33842 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/lake.sw
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/minimal.ecolab
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/multiple_root_elements.pfs
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/multiple_unique_root_elements.pfs
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/nonunique.pfs
--rw-r--r--   0        0        0   220540 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/oresund.mdf
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/readme.md
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/simple.pfs
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/data/pfs/t1_t0.mzt
--rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/Dfsu-2D-interpolation.qmd
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/Generic.qmd
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/Time-interpolation.qmd
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/index.qmd
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/dfs2/bathy.qmd
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/dfs2/gfs.qmd
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/examples/dfs2/index.qmd
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/data-structures.md
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dataarray.qmd
--rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dataset.qmd
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dfs0.qmd
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dfs1.qmd
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dfs2.qmd
--rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/dfsu.qmd
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/eum.qmd
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/generic.md
--rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/getting-started.qmd
--rw-r--r--   0        0        0    46550 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/mauna_loa_co2.dfs0
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/mesh.qmd
--rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 mikeio-2.0b0/docs/user-guide/pfs.qmd
--rw-r--r--   0        0        0     6695 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/__init__.py
--rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/_interpolation.py
--rw-r--r--   0        0        0     7022 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/_spectral.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/_time.py
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/_track.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/exceptions.py
--rw-r--r--   0        0        0    31728 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/generic.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/xyz.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dataset/__init__.py
--rw-r--r--   0        0        0    23362 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dataset/_data_plot.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dataset/_data_utils.py
--rw-r--r--   0        0        0    66431 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dataset/_dataarray.py
--rw-r--r--   0        0        0    64634 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dataset/_dataset.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/__init__.py
--rw-r--r--   0        0        0    17007 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/_dfs.py
--rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/_dfs0.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/_dfs1.py
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/_dfs2.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfs/_dfs3.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/__init__.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_common.py
--rw-r--r--   0        0        0    20512 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_dfsu.py
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_factory.py
--rw-r--r--   0        0        0    15047 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_layered.py
--rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_mesh.py
--rw-r--r--   0        0        0    15952 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/dfsu/_spectral.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/eum/__init__.py
--rw-r--r--   0        0        0    44301 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/eum/_eum.py
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/pfs/__init__.py
--rw-r--r--   0        0        0    13903 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/pfs/_pfsdocument.py
--rw-r--r--   0        0        0    14817 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/pfs/_pfssection.py
--rw-r--r--   0        0        0    41057 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_FM_geometry.py
--rw-r--r--   0        0        0    31810 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_FM_geometry_layered.py
--rw-r--r--   0        0        0     7203 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_FM_geometry_spectral.py
--rw-r--r--   0        0        0    21744 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_FM_utils.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/__init__.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_geometry.py
--rw-r--r--   0        0        0    43248 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_grid_geometry.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/_utils.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 mikeio-2.0b0/mikeio/spatial/crs.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mikeio-2.0b0/.gitignore
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 mikeio-2.0b0/README.md
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 mikeio-2.0b0/pyproject.toml
--rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 mikeio-2.0b0/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mikeio-2.0b1/.gitattributes
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 mikeio-2.0b1/CITATION.cff
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 mikeio-2.0b1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 mikeio-2.0b1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 mikeio-2.0b1/Dependencies.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 mikeio-2.0b1/License.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 mikeio-2.0b1/MANIFEST.in
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 mikeio-2.0b1/Makefile
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mikeio-2.0b1/conftest.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 mikeio-2.0b1/mypy.ini
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 mikeio-2.0b1/pytest.ini
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 mikeio-2.0b1/requirements_min.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 mikeio-2.0b1/setup.cfg
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 mikeio-2.0b1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/docs_dead_links.yml
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/downstream_test.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/full_test.yml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/legacy_test.yml
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/notebooks_test.yml
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/perf_test.yml
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 mikeio-2.0b1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/.gitignore
+-rw-r--r--   0        0        0    17564 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/MIKE-IO-Icon-Pos-RGB.png
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/MIKE-IO-Logo-Pos-RGB.svg
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_quarto.yml
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_sidebar.yml
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/design.qmd
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/index.qmd
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/_extension.yml
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/fontawesome.lua
+-rw-r--r--   0        0        0   140200 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/css/all.css
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/css/latex-fontsize.css
+-rw-r--r--   0        0        0   180104 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.ttf
+-rw-r--r--   0        0        0    92140 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.woff2
+-rw-r--r--   0        0        0    76072 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.ttf
+-rw-r--r--   0        0        0    25124 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.woff2
+-rw-r--r--   0        0        0   384736 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.ttf
+-rw-r--r--   0        0        0   133940 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.woff2
+-rw-r--r--   0        0        0   181852 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   105536 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    60520 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    23940 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   388460 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   154228 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10556 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/interlinks/interlinks.lua
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0  1458641 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_inv/numpy_objects.json
+-rw-r--r--   0        0        0  3527650 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_inv/pandas_objects.json
+-rw-r--r--   0        0        0  2070099 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_inv/scipy_objects.json
+-rw-r--r--   0        0        0  1808234 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/_inv/xarray_objects.json
+-rw-r--r--   0        0        0   544223 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/BW_Ronne_Layout1998_rotated.dfs2
+-rw-r--r--   0        0        0     5483 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/BW_Ronne_Layout1998_rotated_crop.dfs2
+-rw-r--r--   0        0        0   127789 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/FakeLake.dfsu
+-rw-r--r--   0        0        0    54573 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/FakeLake_NONUTM.dfsu
+-rw-r--r--   0        0        0   241633 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/Grid1.dfs3
+-rw-r--r--   0        0        0   166091 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/HD2D.dfsu
+-rw-r--r--   0        0        0   256944 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/Karup_MIKE_SHE_head_output.dfs3
+-rw-r--r--   0        0        0   279558 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/Karup_MIKE_SHE_output.dfs2
+-rw-r--r--   0        0        0    90438 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/M3WFM_sponge_local_coordinates.dfs2
+-rw-r--r--   0        0        0   232505 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/MIKE21SW_dir_sector_area_spectra.dfsu
+-rw-r--r--   0        0        0   555625 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/NorthSea_HD_and_windspeed.dfsu
+-rw-r--r--   0        0        0   180184 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/Slottskogen.asc.zip
+-rw-r--r--   0        0        0   365148 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/State_Area.dfsu
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/State_wlbc_north_err.dfs1
+-rw-r--r--   0        0        0   110332 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/altimetry_NorthSea_20171027.csv
+-rw-r--r--   0        0        0    28491 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/area_freq_spectra.dfsu
+-rw-r--r--   0        0        0   196493 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/area_spectra.dfsu
+-rw-r--r--   0        0        0    72175 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/basin_2dv.dfsu
+-rw-r--r--   0        0        0   181575 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/basin_3d.dfsu
+-rw-r--r--   0        0        0    32045 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/co2-mm-mlo.csv
+-rw-r--r--   0        0        0    40767 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/da_diagnostic.dfs0
+-rw-r--r--   0        0        0    19605 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/dir_wave_analysis_spectra.dfs2
+-rw-r--r--   0        0        0   694129 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/dissolved_oxygen.dfs3
+-rw-r--r--   0        0        0    20829 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/eq.dfs2
+-rw-r--r--   0        0        0    26143 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/eq_relative.dfs0
+-rw-r--r--   0        0        0   268841 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/europe_wind_long_lat.dfs2
+-rw-r--r--   0        0        0   120232 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/gebco_2020_n56.3_s55.2_w12.2_e13.1.nc
+-rw-r--r--   0        0        0   228707 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/gebco_sound.dfs2
+-rw-r--r--   0        0        0    84666 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/gebco_sound_crop_rotate.dfs2
+-rw-r--r--   0        0        0    49641 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/gfs_wind.nc
+-rw-r--r--   0        0        0   337299 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/global_long_lat_pacific_view_temperature_delta.dfs2
+-rw-r--r--   0        0        0   649616 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/hd_vertical_slice.dfs2
+-rw-r--r--   0        0        0   386188 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/kalundborg_coarse.mesh
+-rw-r--r--   0        0        0   457167 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/kalundborg_transect.dfsu
+-rw-r--r--   0        0        0     5402 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/line_dir_spectra.dfsu
+-rw-r--r--   0        0        0    11081 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/line_freq_spectra.dfsu
+-rw-r--r--   0        0        0    67078 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/line_spectra.dfsu
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/local_coordinates.dfs3
+-rw-r--r--   0        0        0   186688 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/many_items.dfs0
+-rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/neq_daily_time_unit.dfs0
+-rw-r--r--   0        0        0   123639 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/north_sea_2.mesh
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/nx1.dfs1
+-rw-r--r--   0        0        0    38048 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/odense_rough.mesh
+-rw-r--r--   0        0        0    38048 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/odense_rough2.MESH
+-rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/oresundHD_run1.dfsu
+-rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/oresundHD_run2.dfsu
+-rw-r--r--   0        0        0  1511214 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/oresund_sigma_z.dfsu
+-rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/oresund_vertical_slice.dfsu
+-rw-r--r--   0        0        0    47378 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/oresund_vertical_slice2.DFSU
+-rw-r--r--   0        0        0    91216 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/physical_basin_wave_maker_signal.dfs1
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/positions.xyz
+-rw-r--r--   0        0        0    10436 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pt_freq_spectra.dfsu
+-rw-r--r--   0        0        0    50550 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pt_spectra.dfs2
+-rw-r--r--   0        0        0    76049 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pt_spectra.dfsu
+-rw-r--r--   0        0        0    51017 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/quad_tri.mesh
+-rw-r--r--   0        0        0    22816 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/random.dfs0
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/random.dfs1
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/random.dfs2
+-rw-r--r--   0        0        0    22826 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/random_timestepunit_hours.dfs0
+-rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/random_two_item.dfs2
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/single_layer.dfs3
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/single_row.dfs2
+-rwxr-xr-x   0        0        0      691 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/single_time_dt_zero.dfs2
+-rw-r--r--   0        0        0     7765 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/single_timestep.dfs3
+-rw-r--r--   0        0        0    15736 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/sw_points.dfs0
+-rw-r--r--   0        0        0    77771 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/template.sw
+-rw-r--r--   0        0        0    57490 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/template_modified.sw
+-rw-r--r--   0        0        0    97752 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/test_dfs3.dfs3
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/tide1.dfs1
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/tide12.dfs1
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/tide2.dfs1
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/tide2_offset.dfs1
+-rw-r--r--   0        0        0     5409 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/tide4.dfs1
+-rw-r--r--   0        0        0    76208 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/track_extraction_case02_indata.dfsu
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/track_extraction_case02_track.csv
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/txconc.dfs1
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/untitled_3_items.dfs0
+-rw-r--r--   0        0        0    99633 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/utm_not_rotated_neurope_temp.dfs2
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/uv_vertical_daily.dfs2
+-rw-r--r--   0        0        0    74421 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/vu_tide_hourly.dfs1
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/water.xyz
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/waterlevel_north.dfs1
+-rw-r--r--   0        0        0     8146 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/waterlevel_viken.dfs0
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/waves.dfs0
+-rw-r--r--   0        0        0    40056 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/waves.dfs2
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/waves2.DFS0
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/winches.xyz
+-rw-r--r--   0        0        0    87261 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/wind_north_sea.dfsu
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/consistency/oresundHD.dfs0
+-rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/consistency/oresundHD.dfs1
+-rw-r--r--   0        0        0    19471 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/consistency/oresundHD.dfs2
+-rw-r--r--   0        0        0   435606 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/consistency/oresundHD.dfsu
+-rw-r--r--   0        0        0   131823 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/Karup_basic.she
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/Karup_mini.she
+-rw-r--r--   0        0        0    73742 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/OresundHD2D_EnKF10.m21fm
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/Setup_WaveSpectraConverter.21t
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/concat.mzt
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/filenames.pfs
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/grid1.gsf
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/illegal.pfs
+-rw-r--r--   0        0        0    95804 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/lake.m21fm
+-rw-r--r--   0        0        0    33842 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/lake.sw
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/minimal.ecolab
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/multiple_root_elements.pfs
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/multiple_unique_root_elements.pfs
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/nonunique.pfs
+-rw-r--r--   0        0        0   220540 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/oresund.mdf
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/readme.md
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/simple.pfs
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/data/pfs/t1_t0.mzt
+-rw-r--r--   0        0        0     4264 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/Dfsu-2D-interpolation.qmd
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/Generic.qmd
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/Time-interpolation.qmd
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/index.qmd
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/dfs2/bathy.qmd
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/dfs2/gfs.qmd
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/examples/dfs2/index.qmd
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/data-structures.md
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dataarray.qmd
+-rw-r--r--   0        0        0     4717 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dataset.qmd
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dfs0.qmd
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dfs1.qmd
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dfs2.qmd
+-rw-r--r--   0        0        0     5053 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/dfsu.qmd
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/eum.qmd
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/generic.qmd
+-rw-r--r--   0        0        0     2814 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/getting-started.qmd
+-rw-r--r--   0        0        0    46550 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/mauna_loa_co2.dfs0
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/mesh.qmd
+-rw-r--r--   0        0        0     5839 2020-02-02 00:00:00.000000 mikeio-2.0b1/docs/user-guide/pfs.qmd
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/__init__.py
+-rw-r--r--   0        0        0     5067 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/_interpolation.py
+-rw-r--r--   0        0        0     7022 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/_spectral.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/_time.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/_track.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/exceptions.py
+-rw-r--r--   0        0        0    31728 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/generic.py
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/xyz.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dataset/__init__.py
+-rw-r--r--   0        0        0    26740 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dataset/_data_plot.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dataset/_data_utils.py
+-rw-r--r--   0        0        0    66967 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dataset/_dataarray.py
+-rw-r--r--   0        0        0    64780 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dataset/_dataset.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/__init__.py
+-rw-r--r--   0        0        0    17109 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/_dfs.py
+-rw-r--r--   0        0        0    13183 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/_dfs0.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/_dfs1.py
+-rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/_dfs2.py
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfs/_dfs3.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/__init__.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_common.py
+-rw-r--r--   0        0        0    20901 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_dfsu.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_factory.py
+-rw-r--r--   0        0        0    15419 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_layered.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_mesh.py
+-rw-r--r--   0        0        0    16916 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/dfsu/_spectral.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/eum/__init__.py
+-rw-r--r--   0        0        0    44457 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/eum/_eum.py
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/pfs/__init__.py
+-rw-r--r--   0        0        0    14521 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/pfs/_pfsdocument.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/pfs/_pfssection.py
+-rw-r--r--   0        0        0    39275 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_FM_geometry.py
+-rw-r--r--   0        0        0    32454 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_FM_geometry_layered.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_FM_geometry_spectral.py
+-rw-r--r--   0        0        0    23662 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_FM_utils.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/__init__.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_geometry.py
+-rw-r--r--   0        0        0    43438 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_grid_geometry.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/_utils.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 mikeio-2.0b1/mikeio/spatial/crs.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 mikeio-2.0b1/.gitignore
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 mikeio-2.0b1/README.md
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 mikeio-2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 mikeio-2.0b1/PKG-INFO
```

### Comparing `mikeio-2.0b0/CODE_OF_CONDUCT.md` & `mikeio-2.0b1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/CONTRIBUTING.md` & `mikeio-2.0b1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/License.txt` & `mikeio-2.0b1/License.txt`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/Makefile` & `mikeio-2.0b1/Makefile`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mypy.ini` & `mikeio-2.0b1/mypy.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [mypy]
 python_version = 3.10
 warn_return_any = false
 allow_redefinition = True
 warn_unreachable = True
-
+disallow_untyped_defs = True
 
 [mypy-mikeio.spatial]
 warn_return_any = True
 
 [mypy-mikeio.dataset.*]
 disallow_incomplete_defs = True
```

### Comparing `mikeio-2.0b0/.devcontainer/devcontainer.json` & `mikeio-2.0b1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/ISSUE_TEMPLATE/feature_request.md` & `mikeio-2.0b1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/build_docs.yml` & `mikeio-2.0b1/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/docs.yml` & `mikeio-2.0b1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/docs_dead_links.yml` & `mikeio-2.0b1/.github/workflows/docs_dead_links.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/downstream_test.yml` & `mikeio-2.0b1/.github/workflows/downstream_test.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/full_test.yml` & `mikeio-2.0b1/.github/workflows/full_test.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/legacy_test.yml` & `mikeio-2.0b1/.github/workflows/legacy_test.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/notebooks_test.yml` & `mikeio-2.0b1/.github/workflows/notebooks_test.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/perf_test.yml` & `mikeio-2.0b1/.github/workflows/perf_test.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/.github/workflows/python-publish.yml` & `mikeio-2.0b1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/MIKE-IO-Icon-Pos-RGB.png` & `mikeio-2.0b1/docs/MIKE-IO-Icon-Pos-RGB.png`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/MIKE-IO-Logo-Pos-RGB.svg` & `mikeio-2.0b1/docs/MIKE-IO-Logo-Pos-RGB.svg`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_quarto.yml` & `mikeio-2.0b1/docs/_quarto.yml`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         - user-guide/dataset.qmd
         - user-guide/dfs0.qmd
         - user-guide/dfs1.qmd
         - user-guide/dfs2.qmd
         - user-guide/dfsu.qmd
         - user-guide/mesh.qmd
         - user-guide/eum.qmd
-        - user-guide/generic.md
+        - user-guide/generic.qmd
         - user-guide/pfs.qmd
       - section: Examples
         href: examples/index.qmd
         contents:
           - section: Dfs2
             href: examples/dfs2/index.qmd
             contents:
@@ -72,15 +72,15 @@
       numpy: 
         url: https://numpy.org/doc/stable/
       xarray: 
         url: https://xarray.pydata.org/en/stable/
       pandas: 
         url: https://pandas.pydata.org/docs/
       scipy: 
-        url: https://docs.scipy.org/doc/scipy/reference/
+        url: https://docs.scipy.org/doc/scipy/
 
 quartodoc:
   style: pkgdown
   title: API Reference
   dir: api
   package: mikeio
   options:
```

### Comparing `mikeio-2.0b0/docs/_sidebar.yml` & `mikeio-2.0b1/docs/_sidebar.yml`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/design.qmd` & `mikeio-2.0b1/docs/design.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/index.qmd` & `mikeio-2.0b1/docs/index.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/fontawesome.lua` & `mikeio-2.0b1/docs/_extensions/fontawesome/fontawesome.lua`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/css/all.css` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/css/all.css`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Brands-Regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/FontAwesome6Free-Solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.ttf` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.woff2` & `mikeio-2.0b1/docs/_extensions/fontawesome/assets/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/interlinks/interlinks.lua` & `mikeio-2.0b1/docs/_extensions/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_extensions/machow/interlinks/interlinks.lua` & `mikeio-2.0b1/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_inv/numpy_objects.json` & `mikeio-2.0b1/docs/_inv/numpy_objects.json`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_inv/pandas_objects.json` & `mikeio-2.0b1/docs/_inv/pandas_objects.json`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_inv/scipy_objects.json` & `mikeio-2.0b1/docs/_inv/scipy_objects.json`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/_inv/xarray_objects.json` & `mikeio-2.0b1/docs/_inv/xarray_objects.json`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/BW_Ronne_Layout1998_rotated.dfs2` & `mikeio-2.0b1/docs/data/BW_Ronne_Layout1998_rotated.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/BW_Ronne_Layout1998_rotated_crop.dfs2` & `mikeio-2.0b1/docs/data/BW_Ronne_Layout1998_rotated_crop.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/FakeLake.dfsu` & `mikeio-2.0b1/docs/data/FakeLake.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/FakeLake_NONUTM.dfsu` & `mikeio-2.0b1/docs/data/FakeLake_NONUTM.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/Grid1.dfs3` & `mikeio-2.0b1/docs/data/Grid1.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/HD2D.dfsu` & `mikeio-2.0b1/docs/data/HD2D.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/Karup_MIKE_SHE_head_output.dfs3` & `mikeio-2.0b1/docs/data/Karup_MIKE_SHE_head_output.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/Karup_MIKE_SHE_output.dfs2` & `mikeio-2.0b1/docs/data/Karup_MIKE_SHE_output.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/M3WFM_sponge_local_coordinates.dfs2` & `mikeio-2.0b1/docs/data/M3WFM_sponge_local_coordinates.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/MIKE21SW_dir_sector_area_spectra.dfsu` & `mikeio-2.0b1/docs/data/MIKE21SW_dir_sector_area_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/NorthSea_HD_and_windspeed.dfsu` & `mikeio-2.0b1/docs/data/NorthSea_HD_and_windspeed.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/Slottskogen.asc.zip` & `mikeio-2.0b1/docs/data/Slottskogen.asc.zip`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/State_Area.dfsu` & `mikeio-2.0b1/docs/data/State_Area.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/State_wlbc_north_err.dfs1` & `mikeio-2.0b1/docs/data/State_wlbc_north_err.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/altimetry_NorthSea_20171027.csv` & `mikeio-2.0b1/docs/data/altimetry_NorthSea_20171027.csv`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/area_freq_spectra.dfsu` & `mikeio-2.0b1/docs/data/area_freq_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/area_spectra.dfsu` & `mikeio-2.0b1/docs/data/area_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/basin_2dv.dfsu` & `mikeio-2.0b1/docs/data/basin_2dv.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/basin_3d.dfsu` & `mikeio-2.0b1/docs/data/basin_3d.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/co2-mm-mlo.csv` & `mikeio-2.0b1/docs/data/co2-mm-mlo.csv`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/da_diagnostic.dfs0` & `mikeio-2.0b1/docs/data/da_diagnostic.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/dir_wave_analysis_spectra.dfs2` & `mikeio-2.0b1/docs/data/dir_wave_analysis_spectra.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/dissolved_oxygen.dfs3` & `mikeio-2.0b1/docs/data/dissolved_oxygen.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/eq.dfs2` & `mikeio-2.0b1/docs/data/eq.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/eq_relative.dfs0` & `mikeio-2.0b1/docs/data/eq_relative.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/europe_wind_long_lat.dfs2` & `mikeio-2.0b1/docs/data/europe_wind_long_lat.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/gebco_2020_n56.3_s55.2_w12.2_e13.1.nc` & `mikeio-2.0b1/docs/data/gebco_2020_n56.3_s55.2_w12.2_e13.1.nc`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/gebco_sound.dfs2` & `mikeio-2.0b1/docs/data/gebco_sound.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/gebco_sound_crop_rotate.dfs2` & `mikeio-2.0b1/docs/data/gebco_sound_crop_rotate.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/gfs_wind.nc` & `mikeio-2.0b1/docs/data/gfs_wind.nc`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/global_long_lat_pacific_view_temperature_delta.dfs2` & `mikeio-2.0b1/docs/data/global_long_lat_pacific_view_temperature_delta.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/hd_vertical_slice.dfs2` & `mikeio-2.0b1/docs/data/hd_vertical_slice.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/kalundborg_coarse.mesh` & `mikeio-2.0b1/docs/data/kalundborg_coarse.mesh`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/kalundborg_transect.dfsu` & `mikeio-2.0b1/docs/data/kalundborg_transect.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/line_dir_spectra.dfsu` & `mikeio-2.0b1/docs/data/line_dir_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/line_freq_spectra.dfsu` & `mikeio-2.0b1/docs/data/line_freq_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/line_spectra.dfsu` & `mikeio-2.0b1/docs/data/line_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/many_items.dfs0` & `mikeio-2.0b1/docs/data/many_items.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/neq_daily_time_unit.dfs0` & `mikeio-2.0b1/docs/data/neq_daily_time_unit.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/north_sea_2.mesh` & `mikeio-2.0b1/docs/data/north_sea_2.mesh`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/nx1.dfs1` & `mikeio-2.0b1/docs/data/nx1.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/odense_rough.mesh` & `mikeio-2.0b1/docs/data/odense_rough.mesh`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/odense_rough2.MESH` & `mikeio-2.0b1/docs/data/odense_rough2.MESH`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/oresundHD_run1.dfsu` & `mikeio-2.0b1/docs/data/oresundHD_run1.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/oresundHD_run2.dfsu` & `mikeio-2.0b1/docs/data/oresundHD_run2.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/oresund_sigma_z.dfsu` & `mikeio-2.0b1/docs/data/oresund_sigma_z.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/oresund_vertical_slice.dfsu` & `mikeio-2.0b1/docs/data/oresund_vertical_slice.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/oresund_vertical_slice2.DFSU` & `mikeio-2.0b1/docs/data/oresund_vertical_slice2.DFSU`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/physical_basin_wave_maker_signal.dfs1` & `mikeio-2.0b1/docs/data/physical_basin_wave_maker_signal.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pt_freq_spectra.dfsu` & `mikeio-2.0b1/docs/data/pt_freq_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pt_spectra.dfs2` & `mikeio-2.0b1/docs/data/pt_spectra.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pt_spectra.dfsu` & `mikeio-2.0b1/docs/data/pt_spectra.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/quad_tri.mesh` & `mikeio-2.0b1/docs/data/quad_tri.mesh`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/random.dfs0` & `mikeio-2.0b1/docs/data/random.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/random.dfs1` & `mikeio-2.0b1/docs/data/random.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/random.dfs2` & `mikeio-2.0b1/docs/data/random.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/random_timestepunit_hours.dfs0` & `mikeio-2.0b1/docs/data/random_timestepunit_hours.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/random_two_item.dfs2` & `mikeio-2.0b1/docs/data/random_two_item.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/single_layer.dfs3` & `mikeio-2.0b1/docs/data/single_layer.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/single_row.dfs2` & `mikeio-2.0b1/docs/data/single_row.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/single_time_dt_zero.dfs2` & `mikeio-2.0b1/docs/data/single_time_dt_zero.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/single_timestep.dfs3` & `mikeio-2.0b1/docs/data/single_timestep.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/sw_points.dfs0` & `mikeio-2.0b1/docs/data/sw_points.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/template.sw` & `mikeio-2.0b1/docs/data/template.sw`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/template_modified.sw` & `mikeio-2.0b1/docs/data/template_modified.sw`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/test_dfs3.dfs3` & `mikeio-2.0b1/docs/data/test_dfs3.dfs3`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/tide1.dfs1` & `mikeio-2.0b1/docs/data/tide1.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/tide12.dfs1` & `mikeio-2.0b1/docs/data/tide12.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/tide2.dfs1` & `mikeio-2.0b1/docs/data/tide2.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/tide2_offset.dfs1` & `mikeio-2.0b1/docs/data/tide2_offset.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/tide4.dfs1` & `mikeio-2.0b1/docs/data/tide4.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/track_extraction_case02_indata.dfsu` & `mikeio-2.0b1/docs/data/track_extraction_case02_indata.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/track_extraction_case02_track.csv` & `mikeio-2.0b1/docs/data/track_extraction_case02_track.csv`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/txconc.dfs1` & `mikeio-2.0b1/docs/data/txconc.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/untitled_3_items.dfs0` & `mikeio-2.0b1/docs/data/untitled_3_items.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/utm_not_rotated_neurope_temp.dfs2` & `mikeio-2.0b1/docs/data/utm_not_rotated_neurope_temp.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/uv_vertical_daily.dfs2` & `mikeio-2.0b1/docs/data/uv_vertical_daily.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/vu_tide_hourly.dfs1` & `mikeio-2.0b1/docs/data/vu_tide_hourly.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/water.xyz` & `mikeio-2.0b1/docs/data/water.xyz`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/waterlevel_north.dfs1` & `mikeio-2.0b1/docs/data/waterlevel_north.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/waterlevel_viken.dfs0` & `mikeio-2.0b1/docs/data/waterlevel_viken.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/waves.dfs0` & `mikeio-2.0b1/docs/data/waves.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/waves.dfs2` & `mikeio-2.0b1/docs/data/waves.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/waves2.DFS0` & `mikeio-2.0b1/docs/data/waves2.DFS0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/wind_north_sea.dfsu` & `mikeio-2.0b1/docs/data/wind_north_sea.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/consistency/oresundHD.dfs0` & `mikeio-2.0b1/docs/data/consistency/oresundHD.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/consistency/oresundHD.dfs1` & `mikeio-2.0b1/docs/data/consistency/oresundHD.dfs1`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/consistency/oresundHD.dfs2` & `mikeio-2.0b1/docs/data/consistency/oresundHD.dfs2`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/consistency/oresundHD.dfsu` & `mikeio-2.0b1/docs/data/consistency/oresundHD.dfsu`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/Karup_basic.she` & `mikeio-2.0b1/docs/data/pfs/Karup_basic.she`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/Karup_mini.she` & `mikeio-2.0b1/docs/data/pfs/Karup_mini.she`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/OresundHD2D_EnKF10.m21fm` & `mikeio-2.0b1/docs/data/pfs/OresundHD2D_EnKF10.m21fm`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/Setup_WaveSpectraConverter.21t` & `mikeio-2.0b1/docs/data/pfs/Setup_WaveSpectraConverter.21t`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/concat.mzt` & `mikeio-2.0b1/docs/data/pfs/concat.mzt`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/grid1.gsf` & `mikeio-2.0b1/docs/data/pfs/grid1.gsf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/lake.m21fm` & `mikeio-2.0b1/docs/data/pfs/lake.m21fm`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/lake.sw` & `mikeio-2.0b1/docs/data/pfs/lake.sw`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/minimal.ecolab` & `mikeio-2.0b1/docs/data/pfs/minimal.ecolab`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/multiple_root_elements.pfs` & `mikeio-2.0b1/docs/data/pfs/multiple_root_elements.pfs`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/multiple_unique_root_elements.pfs` & `mikeio-2.0b1/docs/data/pfs/multiple_unique_root_elements.pfs`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/oresund.mdf` & `mikeio-2.0b1/docs/data/pfs/oresund.mdf`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/data/pfs/t1_t0.mzt` & `mikeio-2.0b1/docs/data/pfs/t1_t0.mzt`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/Dfsu-2D-interpolation.qmd` & `mikeio-2.0b1/docs/examples/Dfsu-2D-interpolation.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/Generic.qmd` & `mikeio-2.0b1/docs/examples/Generic.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/Time-interpolation.qmd` & `mikeio-2.0b1/docs/examples/Time-interpolation.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/index.qmd` & `mikeio-2.0b1/docs/examples/index.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/dfs2/bathy.qmd` & `mikeio-2.0b1/docs/examples/dfs2/bathy.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/examples/dfs2/gfs.qmd` & `mikeio-2.0b1/docs/examples/dfs2/gfs.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/user-guide/data-structures.md` & `mikeio-2.0b1/docs/user-guide/data-structures.md`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/user-guide/dataarray.qmd` & `mikeio-2.0b1/docs/user-guide/dataarray.qmd`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+aliases:
+  - ../dataarray.html
+---
+
 # DataArray
 
 The [DataArray](`mikeio.DataArray`) is the common MIKE IO data structure 
 for *item* data from dfs files. 
 The [](`mikeio.read`) methods returns a Dataset as a container of DataArrays (Dfs items)
 
 Each DataArray have the following properties:
@@ -88,24 +93,22 @@
 
 
 
 ## Properties
 
 The DataArray has several properties:
 
-* n_items - Number of items
-* n_timesteps - Number of timesteps
-* n_elements - Number of elements
-* start_time - First time instance (as datetime)
-* end_time - Last time instance (as datetime)
-* is_equidistant - Is the time series equidistant in time
-* timestep - Time step in seconds (if is_equidistant)
-* shape - Shape of each item
+* time - Time index
+* geometry - geometry of the data (e.g. `spatial.GeometryFM2D`)
+* shape - Shape of the data
 * deletevalue - File delete value (NaN value)
 
+```{python}
+da.geometry
+```
 
 
 ## Methods
 
 DataArray has several useful methods for working with data, 
 including different ways of *selecting* data:
```

### Comparing `mikeio-2.0b0/docs/user-guide/dfs0.qmd` & `mikeio-2.0b1/docs/user-guide/dfs0.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+aliases:
+  - ../dfs0.html
+---
+
 # Dfs0
 
 A dfs0 file is also called a time series file.
 
 Working with data from dfs0 files are conveniently done in one of two ways:
 
 * [](`mikeio.Dataset`) - keeps EUM information (convenient if you save data to new dfs0 file)
```

### Comparing `mikeio-2.0b0/docs/user-guide/dfs1.qmd` & `mikeio-2.0b1/docs/user-guide/dfs1.qmd`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+aliases:
+  - ../dfs1.html
+---
+
 # Dfs1
 
 A dfs1 file contains node-based line series data. Dfs1 files do not contain enough metadata to determine their geographical position, but have a relative distance from the origo. 
 
 
 ```{python}
 import mikeio
```

### Comparing `mikeio-2.0b0/docs/user-guide/dfs2.qmd` & `mikeio-2.0b1/docs/user-guide/dfs2.qmd`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+---
+aliases:
+  - ../dfs2.html
+---
+
 # Dfs2
 
 A dfs2 file is also called a grid series file. Values in a dfs2 file are ‘element based’, i.e. values are defined in the centre of each grid cell. 
 
 
 ```{python}
 import mikeio
```

### Comparing `mikeio-2.0b0/docs/user-guide/dfsu.qmd` & `mikeio-2.0b1/docs/user-guide/dfsu.qmd`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 ::: callout-note
 In MIKE Zero, node ids, element ids and layer ids are 1-based.  In MIKE IO, all ids are **0-based** following standard Python indexing. That means, as an example, that when finding the element closest to a point its id will be 1 lower in MIKE IO compared to examining the file in MIKE Zero.
 :::
 
 ## MIKE IO Flexible Mesh Geometry 
 
-MIKE IO has a Flexible Mesh Geometry class, [`GeometryFM`](`mikeio.spatial.GeometryFM2D`), containing the list of node coordinates and the element table which defines the mesh, as well as a number of derived properties (e.g. element coordinates) and methods making it convenient to work with the mesh. 
+MIKE IO has Flexible Mesh Geometry classes, e.g. [`GeometryFM2D`](`mikeio.spatial.GeometryFM2D`), containing the list of node coordinates and the element table which defines the mesh, as well as a number of derived properties (e.g. element coordinates) and methods making it convenient to work with the mesh. 
 
 | Property  |      Description     |
 |----------|--------------|
 | `n_nodes` | Number of nodes | 
 | `node_coordinates` | Coordinates (x,y,z) of all nodes | 
 | `codes` | Codes of all nodes (0:water, 1:land, >=2:open boundary) | 
 | `boundary_polylines` | Lists of closed polylines defining domain outline |
```

### Comparing `mikeio-2.0b0/docs/user-guide/eum.qmd` & `mikeio-2.0b1/docs/user-guide/eum.qmd`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+aliases:
+  - ../eum.html
+---
+
 # EUM
 
 The dfs items in MIKE IO are represented by the `ItemInfo` class. 
 An ItemInfo consists of:
 
 * name - a user-defined string 
 * type - an [`EUMType`](`mikeio.EUMType`)
```

### Comparing `mikeio-2.0b0/docs/user-guide/generic.md` & `mikeio-2.0b1/docs/user-guide/generic.qmd`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+---
+aliases:
+  - ../generic.html
+---
+
 # Generic
 
 The generic module contains functionality that works for all types of dfs (dfs0, dfs1, dfs2, dfs3, dfsu) files: 
 
 * [`concat()`](`mikeio.generic.concat`) - Concatenates files along the time axis
 * [`extract()`](`mikeio.generic.extract`) - Extract timesteps and/or items to a new dfs file
 * [`diff()`](`mikeio.generic.diff`) - Calculate difference between two dfs files with identical geometry
```

### Comparing `mikeio-2.0b0/docs/user-guide/getting-started.qmd` & `mikeio-2.0b1/docs/user-guide/getting-started.qmd`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ds
 ```
 
 Read more on the [Dfs2 page](dfs2.qmd).
 
 
 ## {{< fa toolbox >}} Generic dfs
-MIKE IO has [`generic`](generic.md) functionality that works for all dfs files: 
+MIKE IO has [`generic`](generic.qmd) functionality that works for all dfs files: 
 
 * [`concat()`](`mikeio.generic.concat`) - Concatenates files along the time axis
 * [`extract()`](`mikeio.generic.extract`) - Extract timesteps and/or items to a new dfs file
 * [`diff()`](`mikeio.generic.diff`) - Calculate difference between two dfs files with identical geometry
 * [`sum()`](`mikeio.generic.sum`) - Calculate the sum of two dfs files
 * [`scale()`](`mikeio.generic.scale`) - Apply scaling to any dfs file
 * [`avg_time()`](`mikeio.generic.avg_time`) - Create a temporally averaged dfs file
```

### Comparing `mikeio-2.0b0/docs/user-guide/mauna_loa_co2.dfs0` & `mikeio-2.0b1/docs/user-guide/mauna_loa_co2.dfs0`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/user-guide/mesh.qmd` & `mikeio-2.0b1/docs/user-guide/mesh.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/docs/user-guide/pfs.qmd` & `mikeio-2.0b1/docs/user-guide/pfs.qmd`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/__init__.py` & `mikeio-2.0b1/mikeio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #   X.YrcN  # Release Candidate
 #   X.Y     # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
 
-__version__ = "2.0.b0"  # TODO use git hash instead for dev version?
+__version__ = "2.0.b1"  # TODO use git hash instead for dev version?
 # __version__ = "1.5.0"
 __dfs_version__: int = 200
 
 
 if "64" not in architecture()[0]:
     raise Exception("This library has not been tested for a 32 bit system.")
 
@@ -48,15 +48,15 @@
 
 def read(
     filename: str | Path,
     *,
     items: str | int | Sequence[str | int] | None = None,
     time: int | str | slice | None = None,
     keepdims: bool = False,
-    **kwargs,
+    **kwargs: Any,
 ) -> Dataset:
     """Read all or a subset of the data from a dfs file
 
     All dfs files can be subsetted with the *items* and *time* arguments. But
     the following file types also have the shown additional arguments:
 
     * Dfs2: area
```

### Comparing `mikeio-2.0b0/mikeio/_interpolation.py` & `mikeio-2.0b1/mikeio/_interpolation.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/_spectral.py` & `mikeio-2.0b1/mikeio/_spectral.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/_time.py` & `mikeio-2.0b1/mikeio/_time.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/_track.py` & `mikeio-2.0b1/mikeio/_track.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 from pathlib import Path
 from collections.abc import Sequence
-from typing import Callable, Tuple
+from typing import Any, Callable, Tuple
 
 import numpy as np
 import pandas as pd
 
 from .dataset import Dataset
 from .dfs import Dfs0
 from .eum import ItemInfo
@@ -21,15 +21,15 @@
     geometry: GeometryFM2D,
     track: str | Dataset | pd.DataFrame,
     items: Sequence[ItemInfo],
     item_numbers: Sequence[int],
     time_steps: Sequence[int],
     n_elements: int,
     method: str,
-    dtype,
+    dtype: Any,  # TODO DTypeLike?
     data_read_func: Callable[[int, int], Tuple[np.ndarray, float]],
 ) -> Dataset:
 
     if not isinstance(geometry, GeometryFM2D):
         raise NotImplementedError("Only implemented for 2d flexible mesh geometries")
 
     n_items = len(item_numbers)
@@ -115,15 +115,15 @@
     step = time_steps[dfsu_step]
     for i, item in enumerate(item_numbers):
         d, t2 = data_read_func(item, step)
         t2 = t2 - 1e-10  # TODO what is this operation doing?
         d[d == deletevalue] = np.nan
         d2[i, :] = d
 
-    def is_EOF(step):
+    def is_EOF(step: int) -> bool:
         return step >= len(time_steps)
 
     # loop over track points
     for i_interp, t in enumerate(range(i_start, i_end + 1)):
         t_rel[t]  # time of point relative to dfsu start
 
         read_next = t_rel[t] > t2
```

### Comparing `mikeio-2.0b0/mikeio/exceptions.py` & `mikeio-2.0b1/mikeio/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 from __future__ import annotations
 from typing import Any
 
 
 class DataDimensionMismatch(ValueError):
-    def __init__(self):
+    def __init__(self) -> None:
         self.message = (
             "Data matrices in the x dimension do not all match in the data list."
             "Data is a list of matrices [t, x]."
         )
         super().__init__(self.message)
 
 
 class ItemsError(ValueError):
-    def __init__(self, n_items_file):
+    def __init__(self, n_items_file: int) -> None:
         self.n_items_file = n_items_file
         super().__init__(
             f"'items' must be (a list of) integers between 0 and {n_items_file-1} or str."
         )
 
 
 class InvalidGeometry(ValueError):
-    def __init__(self, message="Invalid operation for this type of geometry"):
+    def __init__(
+        self, message: str = "Invalid operation for this type of geometry"
+    ) -> None:
         super().__init__(message)
 
 
 class InvalidDataValueType(ValueError):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__(
             "Invalid data type. Choose 'Instantaneous', 'Accumulated', 'StepAccumulated', "
             "'MeanStepBackward', or 'MeanStepForward'"
         )
 
 
 class OutsideModelDomainError(ValueError):
```

### Comparing `mikeio-2.0b0/mikeio/generic.py` & `mikeio-2.0b1/mikeio/generic.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/xyz.py` & `mikeio-2.0b1/mikeio/xyz.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,19 +9,19 @@
     df = pd.read_csv(filename, sep="\t", header=None)
     if df.shape[1] == 1:
         df = pd.read_csv(filename, sep=" ", header=None)
 
     ncol = df.shape[1]
     NAMES = ["x", "y", "z", "name"]
 
-    df.columns = NAMES[:ncol]  # type: ignore
+    df.columns = NAMES[:ncol]
 
     return df
 
 
-def dataframe_to_xyz(self, filename: str | Path) -> None:
+def dataframe_to_xyz(self: pd.DataFrame, filename: str | Path) -> None:
     # TODO validation
     self.to_csv(filename, sep="\t", header=False, index=False)
 
 
 # Monkey patch method on DataFrame for convenience
-pd.DataFrame.to_xyz = dataframe_to_xyz  # type: ignore
+pd.DataFrame.to_xyz = dataframe_to_xyz
```

### Comparing `mikeio-2.0b0/mikeio/dataset/_data_plot.py` & `mikeio-2.0b1/mikeio/dataset/_data_plot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 from typing import Any, Tuple, TYPE_CHECKING
 
+from matplotlib.figure import Figure
 import numpy as np
+import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 
 from ..spatial._FM_utils import _plot_map, _plot_vertical_profile
 
 from .._spectral import plot_2dspectrum
 
 if TYPE_CHECKING:
@@ -44,30 +46,32 @@
         if self.da.ndim == 1:
             if self.da._has_time_axis:
                 return self._timeseries(self.da.values, fig, ax, **kwargs)
             else:
                 return self._line_not_timeseries(self.da.values, ax, **kwargs)
 
         if self.da.ndim == 2:
-            return ax.imshow(self.da.values, **kwargs)
+            return ax.imshow(self.da.values, **kwargs)  # type: ignore
 
         # if everything else fails, plot histogram
         return self._hist(ax, **kwargs)
 
     @staticmethod
-    def _get_ax(ax=None, figsize=None):
-        import matplotlib.pyplot as plt  # type: ignore
+    def _get_ax(
+        ax: Axes | None = None, figsize: Tuple[float, float] | None = None
+    ) -> Axes:
 
         if ax is None:
             _, ax = plt.subplots(figsize=figsize)
         return ax
 
     @staticmethod
-    def _get_fig_ax(ax=None, figsize=None):
-        import matplotlib.pyplot as plt  # type: ignore
+    def _get_fig_ax(
+        ax: Axes | None = None, figsize: Tuple[float, float] | None = None
+    ) -> Tuple[Figure, Axes]:
 
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
         return fig, ax
 
@@ -110,44 +114,51 @@
         return self._hist(ax, **kwargs)
 
     def _hist(self, ax: Axes, **kwargs: Any) -> Any:
         result = ax.hist(self.da.values.ravel(), **kwargs)
         ax.set_xlabel(self._label_txt())
         return result
 
-    def line(self, ax=None, figsize=None, **kwargs):
+    def line(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as lines (timeseries if time is present)"""
         fig, ax = self._get_fig_ax(ax, figsize)
         if self.da._has_time_axis:
             return self._timeseries(self.da.values, fig, ax, **kwargs)
         else:
             return self._line_not_timeseries(self.da.values, ax, **kwargs)
 
-    def _timeseries(self, values, fig, ax, **kwargs):
+    def _timeseries(
+        self, values: np.ndarray, fig: Figure, ax: Axes, **kwargs: Any
+    ) -> Axes:
         if "title" in kwargs:
             title = kwargs.pop("title")
             ax.set_title(title)
         ax.plot(self.da.time, values, **kwargs)
         ax.set_xlabel("time")
         fig.autofmt_xdate()
         ax.set_ylabel(self._label_txt())
         return ax
 
-    def _line_not_timeseries(self, values, ax, **kwargs):
+    def _line_not_timeseries(self, values: np.ndarray, ax: Axes, **kwargs: Any) -> Axes:
         title = kwargs.pop("title") if "title" in kwargs else f"{self.da.time[0]}"
         ax.set_title(title)
         ax.plot(values, **kwargs)
         ax.set_xlabel(self.da.dims[0])
         ax.set_ylabel(self._label_txt())
         return ax
 
-    def _label_txt(self):
+    def _label_txt(self) -> str:
         return f"{self.da.name} [{self.da.unit.short_name}]"
 
-    def _get_first_step_values(self):
+    def _get_first_step_values(self) -> np.ndarray:
         if self.da.n_timesteps > 1:
             return self.da.values[0]
         else:
             return np.squeeze(self.da.values)
 
 
 class _DataArrayPlotterGrid1D(_DataArrayPlotter):
@@ -160,66 +171,92 @@
     >>> da.plot.line()
     >>> da.plot.timeseries()
     >>> da.plot.imshow()
     >>> da.plot.pcolormesh()
     >>> da.plot.hist()
     """
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         _, ax = self._get_fig_ax(ax, figsize)
         if self.da.n_timesteps == 1:
             return self.line(ax, **kwargs)
         else:
             return self.pcolormesh(ax, **kwargs)
 
-    def line(self, ax=None, figsize=None, **kwargs):
+    def line(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot as spatial lines"""
         _, ax = self._get_fig_ax(ax, figsize)
         return self._lines(ax, **kwargs)
 
-    def timeseries(self, ax=None, figsize=None, **kwargs):
+    def timeseries(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot as timeseries"""
         if self.da.n_timesteps == 1:
             raise ValueError("Not possible with single timestep DataArray")
         fig, ax = self._get_fig_ax(ax, figsize)
         return super()._timeseries(self.da.values, fig, ax, **kwargs)
 
-    def imshow(self, ax=None, figsize=None, **kwargs):
+    def imshow(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot as 2d"""
         if not self.da._has_time_axis:
             raise ValueError(
                 "Not possible without time axis. DataArray only has 1 dimension."
             )
         fig, ax = self._get_fig_ax(ax, figsize)
         pos = ax.imshow(self.da.values, **kwargs)
         fig.colorbar(pos, ax=ax, label=self._label_txt())
         return ax
 
-    def pcolormesh(self, ax=None, figsize=None, title=None, **kwargs):
+    def pcolormesh(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        title: str | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot multiple lines as 2d color plot"""
         if not self.da._has_time_axis:
             raise ValueError(
                 "Not possible without time axis. DataArray only has 1 dimension."
             )
+        fig, ax = self._get_fig_ax(ax, figsize)
         if title is not None:
             ax.set_title(title)
-        fig, ax = self._get_fig_ax(ax, figsize)
         pos = ax.pcolormesh(
             self.da.geometry.x,
             self.da.time,
             self.da.values,
             shading="nearest",
             **kwargs,
         )
         _ = fig.colorbar(pos, label=self._label_txt())
         ax.set_xlabel(self.da.geometry._axis_name)
         ax.set_ylabel("time")
         return ax
 
-    def _lines(self, ax=None, title=None, **kwargs):
+    def _lines(self, ax: Axes, title: str | None = None, **kwargs: Any) -> Axes:
         """x-lines - one per timestep"""
         if title is not None:
             ax.set_title(title)
         elif self.da.n_timesteps == 1:
             ax.set_title(f"{self.da.time[0]}")
         ax.plot(self.da.geometry.x, self.da.values.T, **kwargs)
         ax.set_xlabel(self.da.geometry._axis_name)
@@ -237,18 +274,29 @@
     ```{python}
     import mikeio
     da = mikeio.read("../data/gebco_sound.dfs2")["Elevation"]
     da.plot()
     ```
     """
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         return self.pcolormesh(ax, figsize, **kwargs)
 
-    def contour(self, ax=None, figsize=None, title=None, **kwargs):
+    def contour(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        title: str | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as contour lines
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/gebco_sound.dfs2")["Elevation"]
         da.plot.contour()
@@ -263,15 +311,22 @@
         # fig.colorbar(pos, label=self._label_txt())
         ax.clabel(pos, fmt="%1.2f", inline=1, fontsize=9)
         self._set_aspect_and_labels(ax, self.da.geometry, y)
         if title is not None:
             ax.set_title(title)
         return ax
 
-    def contourf(self, ax=None, figsize=None, label=None, title=None, **kwargs):
+    def contourf(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        title: str | None = None,
+        label: str | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as filled contours
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/gebco_sound.dfs2")["Elevation"]
         da.plot.contourf()
@@ -287,15 +342,22 @@
         pos = ax.contourf(x, y, values, **kwargs)
         fig.colorbar(pos, label=label, pad=0.01)
         self._set_aspect_and_labels(ax, self.da.geometry, y)
         if title is not None:
             ax.set_title(title)
         return ax
 
-    def pcolormesh(self, ax=None, figsize=None, label=None, title=None, **kwargs):
+    def pcolormesh(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        title: str | None = None,
+        label: str | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as coloured patches
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/gebco_sound.dfs2")["Elevation"]
         da.plot.pcolormesh()
@@ -311,26 +373,26 @@
         pos = ax.pcolormesh(xn, yn, values, **kwargs)
         fig.colorbar(pos, label=label, pad=0.01)
         self._set_aspect_and_labels(ax, self.da.geometry, yn)
         if title is not None:
             ax.set_title(title)
         return ax
 
-    def _get_x_y(self):
+    def _get_x_y(self) -> Tuple[np.ndarray, np.ndarray]:
         x = self.da.geometry.x
         y = self.da.geometry.y
         return x, y
 
-    def _get_xn_yn(self):
+    def _get_xn_yn(self) -> Tuple[np.ndarray, np.ndarray]:
         xn = self.da.geometry._centers_to_nodes(self.da.geometry.x)
         yn = self.da.geometry._centers_to_nodes(self.da.geometry.y)
         return xn, yn
 
     @staticmethod
-    def _set_aspect_and_labels(ax, geometry, y):
+    def _set_aspect_and_labels(ax: Axes, geometry: Any, y: np.ndarray) -> None:
         if geometry.is_spectral:
             ax.set_xlabel("Frequency [Hz]")
             ax.set_ylabel("Directions [degree]")
         elif geometry._is_rotated:
             ax.set_xlabel("[m]")
             ax.set_ylabel("[m]")
         elif geometry.projection == "NON-UTM":
@@ -360,86 +422,116 @@
     ```{python}
     import mikeio
     da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
     da.plot()
     ```
     """
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as coloured patches"""
         ax = self._get_ax(ax, figsize)
         return self._plot_FM_map(ax, **kwargs)
 
-    def patch(self, ax=None, figsize=None, **kwargs):
+    def patch(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as coloured patches
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
         da.plot.patch()
         ```
         """
         ax = self._get_ax(ax, figsize)
         kwargs["plot_type"] = "patch"
         return self._plot_FM_map(ax, **kwargs)
 
-    def contour(self, ax=None, figsize=None, **kwargs):
+    def contour(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as contour lines
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
         da.plot.contour()
         ```
         """
         ax = self._get_ax(ax, figsize)
         kwargs["plot_type"] = "contour"
         return self._plot_FM_map(ax, **kwargs)
 
-    def contourf(self, ax=None, figsize=None, **kwargs):
+    def contourf(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as filled contours
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
         da.plot.contourf()
         ```
         """
         ax = self._get_ax(ax, figsize)
         kwargs["plot_type"] = "contourf"
         return self._plot_FM_map(ax, **kwargs)
 
-    def mesh(self, ax=None, figsize=None, **kwargs):
+    def mesh(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot mesh only
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
         da.plot.mesh()
         ```
         """
         return self.da.geometry.plot.mesh(figsize=figsize, ax=ax, **kwargs)
 
-    def outline(self, ax=None, figsize=None, **kwargs):
+    def outline(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot domain outline (using the boundary_polylines property)
 
         Examples
         --------
         ```{python}
         da = mikeio.read("../data/HD2D.dfsu")["Surface elevation"]
         da.plot.outline()
         ```
         """
         return self.da.geometry.plot.outline(figsize=figsize, ax=ax, **kwargs)
 
-    def _plot_FM_map(self, ax, **kwargs):
+    def _plot_FM_map(self, ax: Axes, **kwargs: Any) -> Axes:
         values = self._get_first_step_values()
 
         title = f"{self.da.time[0]}"
         if self.da.geometry.is_layered:
             # select surface as default plotting for 3d files
             values = values[self.da.geometry.top_elements]
             geometry = self.da.geometry.geometry2d
@@ -476,24 +568,41 @@
     >>> da = dsp["Temperature"]
     >>> dsp.plot()
     >>> dsp.plot(extrapolate=False, marker='o')
     >>> dsp.plot.pcolormesh()
     >>> dsp.plot.hist()
     """
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         ax = self._get_ax(ax, figsize)
         return self.line(ax, **kwargs)
 
-    def line(self, ax=None, figsize=None, extrapolate=True, **kwargs):
+    def line(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        extrapolate: bool = True,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as vertical lines"""
         ax = self._get_ax(ax, figsize)
         return self._line(ax, extrapolate=extrapolate, **kwargs)
 
-    def _line(self, ax=None, show_legend=None, extrapolate=True, **kwargs):
+    def _line(
+        self,
+        ax: Axes,
+        show_legend: bool | None = None,
+        extrapolate: bool = True,
+        **kwargs: Any,
+    ) -> Axes:
         import matplotlib.pyplot as plt
 
         if "title" in kwargs:
             title = kwargs.pop("title")
             ax.set_title(title)
 
         if show_legend is None:
@@ -513,15 +622,21 @@
         ax.set_ylabel("z")
 
         if show_legend:
             plt.legend()
 
         return ax
 
-    def pcolormesh(self, ax=None, figsize=None, title=None, **kwargs):
+    def pcolormesh(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        title: str | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data as coloured patches"""
         fig, ax = self._get_fig_ax(ax, figsize)
         ze = self.da.geometry.calc_ze()
         pos = ax.pcolormesh(
             self.da.time,
             ze,
             self.da.values.T,
@@ -546,95 +661,120 @@
     --------
     >>> da = mikeio.read("oresund_vertical_slice.dfsu")["Temperature"]
     >>> da.plot()
     >>> da.plot.mesh()
     >>> da.plot.hist()
     """
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         ax = self._get_ax(ax, figsize)
         return self._plot_transect(ax=ax, **kwargs)
 
-    def _plot_transect(self, **kwargs):
+    def _plot_transect(self, **kwargs: Any) -> Axes:
         if "label" not in kwargs:
             kwargs["label"] = self._label_txt()
         if "title" not in kwargs:
             kwargs["title"] = self.da.time[0]
-
-        values, zn = self._get_first_step_values()
+        assert self.da._zn is not None
+        if self.da.n_timesteps > 1:
+            values = self.da.values[0]
+            zn = self.da._zn[0]
+        else:
+            values = np.squeeze(self.da.values)
+            zn = np.squeeze(self.da._zn)  # type: ignore
         g = self.da.geometry
         return _plot_vertical_profile(
             node_coordinates=g.node_coordinates,
             element_table=g.element_table,
             values=values,
             zn=zn,
             is_geo=g.is_geo,
             **kwargs,
         )
 
-    def _get_first_step_values(self):
-        if self.da.n_timesteps > 1:
-            return self.da.values[0], self.da._zn[0]
-        else:
-            return np.squeeze(self.da.values), np.squeeze(self.da._zn)
-
 
 class _DataArrayPlotterPointSpectrum(_DataArrayPlotter):
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         # ax = self._get_ax(ax, figsize)
         if self.da.n_frequencies > 0 and self.da.n_directions > 0:
             return self._plot_2dspectrum(figsize=figsize, **kwargs)
         elif self.da.n_frequencies == 0:
             return self._plot_dirspectrum(ax=ax, figsize=figsize, **kwargs)
         elif self.da.n_directions == 0:
             return self._plot_freqspectrum(ax=ax, figsize=figsize, **kwargs)
         else:
             raise ValueError("Spectrum could not be plotted")
 
-    def patch(self, **kwargs):
+    def patch(self, **kwargs: Any) -> Axes:
         kwargs["plot_type"] = "patch"
         return self._plot_2dspectrum(**kwargs)
 
-    def contour(self, **kwargs):
+    def contour(self, **kwargs: Any) -> Axes:
         kwargs["plot_type"] = "contour"
         return self._plot_2dspectrum(**kwargs)
 
-    def contourf(self, **kwargs):
+    def contourf(self, **kwargs: Any) -> Axes:
         kwargs["plot_type"] = "contourf"
         return self._plot_2dspectrum(**kwargs)
 
-    def _plot_freqspectrum(self, ax=None, figsize=None, **kwargs):
-        ax = self._plot_1dspectrum(self.da.frequencies, ax, figsize, **kwargs)
+    def _plot_freqspectrum(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
+        ax = self._plot_1dspectrum(self.da.frequencies, ax, figsize, **kwargs)  # type: ignore
         ax.set_xlabel("frequency [Hz]")
         ax.set_ylabel("directionally integrated energy [m*m*s]")
         return ax
 
-    def _plot_dirspectrum(self, ax=None, figsize=None, **kwargs):
-        ax = self._plot_1dspectrum(self.da.directions, ax, figsize, **kwargs)
+    def _plot_dirspectrum(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
+        ax = self._plot_1dspectrum(self.da.directions, ax, figsize, **kwargs)  # type: ignore
         ax.set_xlabel("directions [degrees]")
         ax.set_ylabel("directional spectral energy [m*m*s]")
-        ax.set_xticks(self.da.directions[::2])
+        ax.set_xticks(self.da.directions[::2])  # type: ignore
         return ax
 
-    def _plot_1dspectrum(self, x_values, ax=None, figsize=None, **kwargs):
+    def _plot_1dspectrum(
+        self,
+        x_values: np.ndarray,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         ax = self._get_ax(ax, figsize)
         y_values = self._get_first_step_values()
 
         if "linestyle" not in kwargs:
             kwargs["linestyle"] = "-"
         if "marker" not in kwargs:
             kwargs["marker"] = "."
 
         title = kwargs.pop("title") if "title" in kwargs else self._get_title()
         ax.set_title(title)
 
         ax.plot(x_values, y_values, **kwargs)
         return ax
 
-    def _plot_2dspectrum(self, **kwargs):
+    def _plot_2dspectrum(self, **kwargs: Any) -> Axes:
         values = self._get_first_step_values()
 
         if "figsize" not in kwargs or kwargs["figsize"] is None:
             kwargs["figsize"] = (7, 7)
         if "label" not in kwargs:
             kwargs["label"] = self._label_txt()
         if "title" not in kwargs:
@@ -676,35 +816,46 @@
         super().__init__(Hm0)
 
 
 class _DatasetPlotter:
     def __init__(self, ds: Dataset) -> None:
         self.ds = ds
 
-    def __call__(self, figsize=None, **kwargs):
+    def __call__(
+        self, figsize: Tuple[float, float] | None = None, **kwargs: Any
+    ) -> Axes:
         """Plot multiple DataArrays as time series (only possible dfs0-type data)"""
         if self.ds.dims == ("time",):
             df = self.ds.to_dataframe()
             return df.plot(figsize=figsize, **kwargs)
         else:
             raise ValueError(
                 "Could not plot Dataset. Try plotting one of its DataArrays instead..."
             )
 
     @staticmethod
-    def _get_fig_ax(ax=None, figsize=None):
+    def _get_fig_ax(
+        ax: Axes | None = None, figsize: Tuple[float, float] | None = None
+    ) -> Tuple[Figure, Axes]:
         import matplotlib.pyplot as plt
 
         if ax is None:
             fig, ax = plt.subplots(figsize=figsize)
         else:
             fig = plt.gcf()
         return fig, ax
 
-    def scatter(self, x, y, ax=None, figsize=None, **kwargs):
+    def scatter(
+        self,
+        x: str | int,
+        y: str | int,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         """Plot data from two DataArrays against each other in a scatter plot
 
         Parameters
         ----------
         x : str or int
             Identifier for first DataArray
         y : str or int
@@ -736,9 +887,9 @@
         ax.scatter(xval, yval, **kwargs)
 
         ax.set_xlabel(self._label_txt(self.ds[x]))
         ax.set_ylabel(self._label_txt(self.ds[y]))
         return ax
 
     @staticmethod
-    def _label_txt(da):
+    def _label_txt(da: DataArray) -> str:
         return f"{da.name} [{da.unit.name}]"
```

### Comparing `mikeio-2.0b0/mikeio/dataset/_data_utils.py` & `mikeio-2.0b1/mikeio/dataset/_data_utils.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dataset/_dataarray.py` & `mikeio-2.0b1/mikeio/dataset/_dataarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,20 @@
                 element_table=g.element_table,
                 element_ids=g.element_ids,
             )
         else:
             geometry = GeometryUndefined()
 
         return DataArray(
-            data=Hm0, time=self.da.time, item=item, dims=dims, geometry=geometry
+            data=Hm0,
+            time=self.da.time,
+            item=item,
+            dims=dims,
+            geometry=geometry,
+            dt=self.da._dt,
         )
 
 
 class DataArray:
     """DataArray with data and metadata for a single item in a dfs file
 
     The DataArray has these main properties:
@@ -158,18 +163,20 @@
         data: np.ndarray,
         *,
         time: pd.DatetimeIndex | str | None = None,
         item: ItemInfo | None = None,
         geometry: GeometryType | None = None,
         zn: np.ndarray | None = None,
         dims: Sequence[str] | None = None,
+        dt: float = 1.0,
     ) -> None:
         # TODO: add optional validation validate=True
         self._values = self._parse_data(data)
         self.time: pd.DatetimeIndex = self._parse_time(time)
+        self._dt = dt
 
         geometry = GeometryUndefined() if geometry is None else geometry
         self.dims = self._parse_dims(dims, geometry)
 
         self._check_time_data_length(self.time)
 
         self.item = self._parse_item(item)
@@ -417,19 +424,19 @@
     def is_equidistant(self) -> bool:
         """Is DataArray equidistant in time?"""
         if len(self.time) < 3:
             return True
         return len(self.time.to_series().diff().dropna().unique()) == 1
 
     @property
-    def timestep(self) -> float | None:
+    def timestep(self) -> float:
         """Time step in seconds if equidistant (and at
-        least two time instances); otherwise None
+        least two time instances); otherwise original time step is returned.
         """
-        dt = None
+        dt = self._dt
         if len(self.time) > 1 and self.is_equidistant:
             first: pd.Timestamp = self.time[0]
             second: pd.Timestamp = self.time[1]
             dt = (second - first).total_seconds()
         return dt
 
     @property
@@ -535,14 +542,15 @@
         return DataArray(
             data=data,
             time=self.time,
             item=self.item,
             geometry=self.geometry,
             zn=self._zn,
             dims=tuple(dims),
+            dt=self._dt,
         )
 
     # ============= Select/interp ===========
     def __getitem__(self, key: Any) -> "DataArray":
         da = self
         dims = self.dims
         key = self._getitem_parse_key(key)
@@ -714,14 +722,15 @@
         return DataArray(
             data=dat,
             time=time,
             item=deepcopy(self.item),
             geometry=geometry,
             zn=zn,
             dims=dims,
+            dt=self._dt,
         )
 
     def sel(
         self,
         *,
         time: str | pd.DatetimeIndex | "DataArray" | None = None,
         **kwargs: Any,
@@ -965,15 +974,19 @@
                 # this is not supported yet (see above)
                 # else:
                 #    geometry = GeometryPoint3D(
                 #        x=x, y=y, z=z, projection=self.geometry.projection
                 #    )
 
             da = DataArray(
-                data=dai, time=self.time, geometry=geometry, item=deepcopy(self.item)
+                data=dai,
+                time=self.time,
+                geometry=geometry,
+                item=deepcopy(self.item),
+                dt=self._dt,
             )
         else:
             da = self.copy()
 
         # interp in time
         if time is not None:
             da = da.interp_time(time)
@@ -1093,14 +1106,15 @@
 
         return DataArray(
             data=data,
             time=t_out_index,
             item=deepcopy(self.item),
             geometry=self.geometry,
             zn=zn,
+            dt=self._dt,
         )
 
     def interp_na(self, axis: str = "time", **kwargs: Any) -> "DataArray":
         """Fill in NaNs by interpolating according to different methods.
 
         Wrapper of [](`xarray.DataArray.interpolate_na`)
 
@@ -1193,15 +1207,19 @@
             )
         else:
             raise NotImplementedError(
                 "Interpolation to other geometry not yet supported"
             )
         assert isinstance(ari, np.ndarray)
         dai = DataArray(
-            data=ari, time=self.time, geometry=geom, item=deepcopy(self.item)
+            data=ari,
+            time=self.time,
+            geometry=geom,
+            item=deepcopy(self.item),
+            dt=self._dt,
         )
 
         if hasattr(other, "time"):
             dai = dai.interp_time(other.time)
 
         assert isinstance(dai, DataArray)
 
@@ -1502,14 +1520,15 @@
         return DataArray(
             data=data,
             time=time,
             item=item,
             geometry=geometry,
             dims=dims,
             zn=zn,
+            dt=self._dt,
         )
 
     @overload
     def quantile(self, q: float, **kwargs: Any) -> "DataArray": ...
 
     @overload
     def quantile(self, q: Sequence[float], **kwargs: Any) -> "Dataset": ...
@@ -1595,15 +1614,21 @@
             qdat = func(self.values, q=q, axis=axis, **kwargs)
             geometry = self.geometry if axis == 0 else GeometryUndefined()
             zn = self._zn if axis == 0 else None
 
             dims = tuple([d for i, d in enumerate(self.dims) if i != axis])
             item = deepcopy(self.item)
             return DataArray(
-                data=qdat, time=time, item=item, geometry=geometry, dims=dims, zn=zn
+                data=qdat,
+                time=time,
+                item=item,
+                geometry=geometry,
+                dims=dims,
+                zn=zn,
+                dt=self._dt,
             )
         else:
             res = []
             for quantile in q:
                 qd = self._quantile(q=quantile, axis=axis, func=func)
                 newname = f"Quantile {quantile}, {self.name}"
                 qd.name = newname
@@ -1743,19 +1768,20 @@
     def _boolmask_to_new_DataArray(self, bmask) -> "DataArray":  # type: ignore
         return DataArray(
             data=bmask,
             time=self.time,
             item=ItemInfo("Boolean"),
             geometry=self.geometry,
             zn=self._zn,
+            dt=self._dt,
         )
 
     # ============= output methods: to_xxx() ===========
 
-    def _to_dataset(self):
+    def _to_dataset(self) -> "Dataset":
         """Create a single-item dataset"""
         from mikeio import Dataset
 
         return Dataset(
             {self.name: self}
         )  # Single-item Dataset (All info is contained in the DataArray, no need for additional info)
```

### Comparing `mikeio-2.0b0/mikeio/dataset/_dataset.py` & `mikeio-2.0b1/mikeio/dataset/_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,18 +90,19 @@
         ),
         time: pd.DatetimeIndex | None = None,
         items: Sequence[ItemInfo] | None = None,
         geometry: Any = None,
         zn: NDArray[np.floating] | None = None,
         dims: Tuple[str, ...] | None = None,
         validate: bool = True,
+        dt: float = 1.0,
     ):
         if not self._is_DataArrays(data):
             data = self._create_dataarrays(
-                data=data, time=time, items=items, geometry=geometry, zn=zn, dims=dims  # type: ignore
+                data=data, time=time, items=items, geometry=geometry, zn=zn, dims=dims, dt=dt  # type: ignore
             )
         self._data_vars: MutableMapping[str, DataArray] = self._init_from_DataArrays(data, validate=validate)  # type: ignore
         self.plot = _DatasetPlotter(self)
 
     @staticmethod
     def _is_DataArrays(data: Any) -> bool:
         """Check if input is Sequence/Mapping of DataArrays"""
@@ -119,29 +120,30 @@
                     # raise TypeError("Please provide List/Mapping of DataArrays")
             return True
         return False
 
     @staticmethod
     def _create_dataarrays(
         data: Sequence[NDArray[np.floating]] | NDArray[np.floating],
-        time: pd.DatetimeIndex | None = None,
-        items: Sequence[ItemInfo] | None = None,
-        geometry: Any = None,
-        zn: NDArray[np.floating] | None = None,
-        dims: Tuple[str, ...] | None = None,
+        time: pd.DatetimeIndex,
+        items: Sequence[ItemInfo],
+        geometry: Any,
+        zn: NDArray[np.floating],
+        dims: Tuple[str, ...],
+        dt: float,
     ) -> Mapping[str, DataArray]:
         if not isinstance(data, Iterable):
             data = [data]
         items = Dataset._parse_items(items, len(data))
 
         # TODO: skip validation for all items after the first?
         data_vars = {}
         for dd, it in zip(data, items):
             data_vars[it.name] = DataArray(
-                data=dd, time=time, item=it, geometry=geometry, zn=zn, dims=dims
+                data=dd, time=time, item=it, geometry=geometry, zn=zn, dims=dims, dt=dt
             )
         return data_vars
 
     def _init_from_DataArrays(
         self, data: Sequence[DataArray] | Mapping[str, DataArray], validate: bool = True
     ) -> MutableMapping[str, DataArray]:
         """Initialize Dataset object with Iterable of DataArrays"""
@@ -300,14 +302,19 @@
             self._id_of_DataArrays_equal(da, new_da)
 
     # ============ end of init =============
 
     # ============= Basic properties/methods ===========
 
     @property
+    def _dt(self) -> float:
+        """Original time step in seconds"""
+        return self[0]._dt
+
+    @property
     def time(self) -> pd.DatetimeIndex:
         """Time axis"""
         return list(self)[0].time
 
     @time.setter
     def time(self, new_time: pd.DatetimeIndex) -> None:
         for da in self:
@@ -322,19 +329,19 @@
     @property
     def end_time(self) -> datetime:
         """Last time instance (as datetime)"""
         # TODO: use pd.Timestamp instead
         return self.time[-1].to_pydatetime()  # type: ignore
 
     @property
-    def timestep(self) -> float | None:
+    def timestep(self) -> float:
         """Time step in seconds if equidistant (and at
-        least two time instances); otherwise None
+        least two time instances); otherwise original time step is returned.
         """
-        dt = None
+        dt = self._dt
         if len(self.time) > 1 and self.is_equidistant:
             dt = (self.time[1] - self.time[0]).total_seconds()
         return dt
 
     @property
     def is_equidistant(self) -> bool:
         """Is Dataset equidistant in time?"""
@@ -689,28 +696,28 @@
             if not self._is_key_time(s.start):
                 return False
         if s.stop is not None:
             if not self._is_key_time(s.stop):
                 return False
         return True
 
-    def _is_key_time(self, key):  # type: ignore
+    def _is_key_time(self, key: Any) -> bool:
         if isinstance(key, slice):
             return False
         if isinstance(key, (int, float)):
             return False
         if isinstance(key, str) and key in self.names:
             return False
         if isinstance(key, str) and len(key) > 0 and key[0].isnumeric():
             # TODO: try to parse with pandas
             return True
         if isinstance(key, (datetime, np.datetime64, pd.Timestamp)):
             return True
 
-        return False
+        return False  # type: ignore
 
     def _multi_indexing_attempted(self, key: Any) -> bool:
         # find out if user is attempting ds[2, :, 1] or similar (not allowed)
         # this is not bullet-proof, but a good estimate
         if not isinstance(key, tuple):
             return False
         for k in key:
```

### Comparing `mikeio-2.0b0/mikeio/dfs/_dfs.py` & `mikeio-2.0b1/mikeio/dfs/_dfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,15 +412,22 @@
             t_seconds[i] = itemdata.Time
 
         time = pd.to_datetime(t_seconds, unit="s", origin=self.start_time)
 
         items = _get_item_info(self._dfs.ItemInfo, item_numbers)
 
         self._dfs.Close()
-        return Dataset(data_list, time, items, geometry=self.geometry, validate=False)
+        return Dataset(
+            data_list,
+            time,
+            items,
+            geometry=self.geometry,
+            validate=False,
+            dt=self._timestep,
+        )
 
     def _open(self) -> None:
         raise NotImplementedError("Should be implemented by subclass")
 
     def _get_item_info(self, item_numbers: Sequence[int]) -> List[ItemInfo]:
         """Read DFS ItemInfo
```

### Comparing `mikeio-2.0b0/mikeio/dfs/_dfs0.py` & `mikeio-2.0b1/mikeio/dfs/_dfs0.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfs/_dfs1.py` & `mikeio-2.0b1/mikeio/dfs/_dfs1.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfs/_dfs2.py` & `mikeio-2.0b1/mikeio/dfs/_dfs2.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfs/_dfs3.py` & `mikeio-2.0b1/mikeio/dfs/_dfs3.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,15 @@
             items=items,
             geometry=geometry,
             dims=dims,
             validate=False,
         )
 
     @staticmethod
-    def _get_bottom_values(data):
+    def _get_bottom_values(data: np.ndarray) -> np.ndarray:
 
         assert len(data.shape) == 3
         b = np.empty_like(data[0])
         b[:] = np.nan
         data = np.flipud(data)
         for layer in range(data.shape[0]):  # going from surface to bottom
             y = data[layer, ...]
@@ -281,24 +281,24 @@
         return b
 
     @property
     def geometry(self) -> Grid3D:
         return self._geometry
 
     @property
-    def dx(self):
+    def dx(self) -> float:
         """Step size in x direction"""
         return self._dx
 
     @property
-    def dy(self):
+    def dy(self) -> float:
         """Step size in y direction"""
         return self._dy
 
     @property
-    def dz(self):
+    def dz(self) -> float:
         """Step size in y direction"""
         return self._dz
 
     @property
-    def shape(self):
+    def shape(self) -> Tuple[int, int, int, int]:
         return (self._n_timesteps, self._nz, self._ny, self._nx)
```

### Comparing `mikeio-2.0b0/mikeio/dfsu/_common.py` & `mikeio-2.0b1/mikeio/dfsu/_common.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfsu/_dfsu.py` & `mikeio-2.0b1/mikeio/dfsu/_dfsu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Collection, Sequence, Tuple
+
+from typing import Any, Literal, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 from mikecore.DfsFactory import DfsFactory
 from mikecore.DfsuBuilder import DfsuBuilder
 from mikecore.DfsuFile import DfsuFile, DfsuFileType
 from mikecore.eum import eumQuantity, eumUnit
@@ -38,21 +39,18 @@
     filename: str
         dfsu filename
     data: Dataset
         Dataset to be written
     """
     filename = str(filename)
 
-    if len(data.time) == 1:
-        dt = 1  # TODO is there any sensible default?
-    else:
-        if not data.is_equidistant:
-            raise ValueError("Non-equidistant time axis is not supported.")
+    if not data.is_equidistant:
+        raise ValueError("Non-equidistant time axis is not supported.")
 
-        dt = (data.time[1] - data.time[0]).total_seconds()  # type: ignore
+    dt = data.timestep
     n_time_steps = len(data.time)
 
     geometry = data.geometry
     dfsu_filetype = DfsuFileType.Dfsu2D
 
     if geometry.is_layered:
         dfsu_filetype = geometry._type.value
@@ -268,15 +266,15 @@
         self._type = info.type
         self._deletevalue = info.deletevalue
         self._time = info.time
         self._timestep = info.timestep
         self._items = info.items
         self._geometry = self._read_geometry(self._filename)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         out = [f"<mikeio.{self.__class__.__name__}>"]
 
         out.append(f"number of elements: {self.geometry.n_elements}")
         out.append(f"number of nodes: {self.geometry.n_nodes}")
         out.append(f"projection: {self.geometry.projection_string}")
         if self.n_items < 10:
             out.append("items:")
@@ -289,15 +287,15 @@
         else:
             out.append(
                 f"time: {str(self.time[0])} - {str(self.time[-1])} ({self.n_timesteps} records)"
             )
         return str.join("\n", out)
 
     @property
-    def geometry(self):
+    def geometry(self) -> Any:
         return self._geometry
 
     @property
     def deletevalue(self) -> float:
         """File delete value"""
         return self._deletevalue
 
@@ -357,15 +355,15 @@
         return geometry
 
     def read(
         self,
         *,
         items: str | int | Sequence[str | int] | None = None,
         time: int | str | slice | None = None,
-        elements: Collection[int] | None = None,
+        elements: Sequence[int] | np.ndarray | None = None,
         area: Tuple[float, float, float, float] | None = None,
         x: float | None = None,
         y: float | None = None,
         keepdims: bool = False,
         dtype: Any = np.float32,
         error_bad_data: bool = True,
         fill_bad_data_value: float = np.nan,
@@ -481,18 +479,29 @@
 
         if elements is not None and len(elements) == 1:
             # squeeze point data
             dims = tuple([d for d in dims if d != "element"])
             data_list = [np.squeeze(d, axis=-1) for d in data_list]
 
         return Dataset(
-            data_list, time, items, geometry=geometry, dims=dims, validate=False
+            data_list,
+            time,
+            items,
+            geometry=geometry,
+            dims=dims,
+            validate=False,
+            dt=self.timestep,
         )
 
-    def _parse_geometry_sel(self, area, x, y):
+    def _parse_geometry_sel(
+        self,
+        area: Tuple[float, float, float, float] | None,
+        x: float | None,
+        y: float | None,
+    ) -> np.ndarray | None:
         """Parse geometry selection
 
         Parameters
         ----------
         area : list[float], optional
             Read only data inside (horizontal) area given as a
             bounding box (tuple with left, lower, right, upper)
@@ -525,15 +534,22 @@
         if (x is not None) or (y is not None) or (area is not None):
             # selection was attempted
             if (elements is None) or len(elements) == 0:
                 raise ValueError("No elements in selection!")
 
         return elements
 
-    def get_overset_grid(self, dx=None, dy=None, nx=None, ny=None, buffer=0.0):
+    def get_overset_grid(
+        self,
+        dx: float | None = None,
+        dy: float | None = None,
+        nx: int | None = None,
+        ny: int | None = None,
+        buffer: float = 0.0,
+    ) -> Grid2D:
         """get a 2d grid that covers the domain by specifying spacing or shape
 
         Parameters
         ----------
         dx : float, optional
             grid resolution in x-direction (or in x- and y-direction)
         dy : float, optional
@@ -569,15 +585,21 @@
         self, item: int, step: int
     ) -> Tuple[np.ndarray, pd.Timestamp]:
         dfs = DfsuFile.Open(self._filename)
         itemdata = dfs.ReadItemTimeStep(item + 1, step)
 
         return itemdata.Data, itemdata.Time
 
-    def extract_track(self, track, items=None, method="nearest", dtype=np.float32):
+    def extract_track(
+        self,
+        track: pd.DataFrame,
+        items: int | str | Sequence[int | str] | None = None,
+        method: Literal["nearest", "inverse_distance"] = "nearest",
+        dtype: Any = np.float32,
+    ) -> Dataset:
         """
         Extract track data from a dfsu file
 
         Parameters
         ---------
         track: pandas.DataFrame
             with DatetimeIndex and (x, y) of track points as first two columns
```

### Comparing `mikeio-2.0b0/mikeio/dfsu/_factory.py` & `mikeio-2.0b1/mikeio/dfsu/_factory.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfsu/_layered.py` & `mikeio-2.0b1/mikeio/dfsu/_layered.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 from pathlib import Path
-from typing import Any, Collection, Sequence, Tuple, TYPE_CHECKING
+from typing import Any, Sequence, Tuple, TYPE_CHECKING
 
+from matplotlib.axes import Axes
 import numpy as np
 from mikecore.DfsuFile import DfsuFile, DfsuFileType
 import pandas as pd
 from scipy.spatial import cKDTree
 from tqdm import trange
 
 from ..dataset import DataArray, Dataset
@@ -13,15 +14,20 @@
     _get_item_info,
     _read_item_time_step,
     _valid_item_numbers,
     _valid_timesteps,
 )
 from ..eum import EUMType, ItemInfo
 from .._interpolation import get_idw_interpolant, interp2d
-from ..spatial import GeometryFM3D, GeometryFMVerticalProfile, GeometryPoint3D
+from ..spatial import (
+    GeometryFM3D,
+    GeometryFMVerticalProfile,
+    GeometryPoint3D,
+    GeometryFM2D,
+)
 from ..spatial._FM_utils import _plot_vertical_profile
 from ._dfsu import (
     _get_dfsu_info,
     get_nodes_from_source,
     get_elements_from_source,
     _validate_elements_and_geometry_sel,
 )
@@ -40,15 +46,15 @@
         self._deletevalue = info.deletevalue
         self._time = info.time
         self._timestep = info.timestep
         self._geometry = self._read_geometry(self._filename)
         # 3d files have a zn item
         self._items = self._read_items(self._filename)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         out = [f"<mikeio.{self.__class__.__name__}>"]
 
         out.append(f"number of elements: {self.geometry.n_elements}")
         out.append(f"number of nodes: {self.geometry.n_nodes}")
         out.append(f"projection: {self.geometry.projection_string}")
         out.append(f"number of sigma layers: {self.geometry.n_sigma_layers}")
         if (
@@ -59,15 +65,15 @@
                 f"max number of z layers: {self.geometry.n_layers - self.geometry.n_sigma_layers}"
             )
         if self.n_items < 10:
             out.append("items:")
             for i, item in enumerate(self.items):
                 out.append(f"  {i}:  {item}")
         else:
-            out.append(f"number of items: {self.geometry.n_items}")
+            out.append(f"number of items: {self.n_items}")
         if self.n_timesteps == 1:
             out.append(f"time: time-invariant file (1 step) at {self.time[0]}")
         else:
             out.append(
                 f"time: {str(self.time[0])} - {str(self.time[-1])} ({self.n_timesteps} records)"
             )
         return str.join("\n", out)
@@ -174,15 +180,15 @@
         return self.n_layers - self.n_sigma_layers
 
     def read(
         self,
         *,
         items: str | int | Sequence[str | int] | None = None,
         time: int | str | slice | None = None,
-        elements: Collection[int] | None = None,
+        elements: Sequence[int] | None = None,
         area: Tuple[float, float, float, float] | None = None,
         x: float | None = None,
         y: float | None = None,
         z: float | None = None,
         layers: int | Layer | Sequence[int] | None = None,
         keepdims: bool = False,
         dtype: Any = np.float32,
@@ -242,15 +248,15 @@
                 or (y is not None)
                 or (area is not None)
                 or (layers is not None)
             ):
                 elements = self.geometry.find_index(  # type: ignore
                     x=x, y=y, z=z, area=area, layers=layers
                 )
-                if len(elements) == 0:
+                if len(elements) == 0:  # type: ignore
                     raise ValueError("No elements in selection!")
 
         geometry = (
             self.geometry
             if elements is None
             else self.geometry.elements_to_geometry(elements)
         )
@@ -340,25 +346,38 @@
                 data_list[1:],  # skip zn item
                 time,
                 items,
                 geometry=geometry,
                 zn=data_list[0],
                 dims=dims,
                 validate=False,
+                dt=self.timestep,
             )
         else:
             return Dataset(
-                data_list, time, items, geometry=geometry, dims=dims, validate=False
+                data_list,
+                time,
+                items,
+                geometry=geometry,
+                dims=dims,
+                validate=False,
+                dt=self.timestep,
             )
 
 
 class Dfsu2DV(DfsuLayered):
     def plot_vertical_profile(
-        self, values, time_step=None, cmin=None, cmax=None, label="", **kwargs
-    ):
+        self,
+        values: np.ndarray | DataArray,
+        time_step: int | None = None,
+        cmin: float | None = None,
+        cmax: float | None = None,
+        label: str = "",
+        **kwargs: Any,
+    ) -> Axes:
         """
         Plot unstructured vertical profile
 
         Parameters
         ----------
         values: np.array
             value for each element to plot
@@ -400,15 +419,15 @@
             label=label,
             **kwargs,
         )
 
 
 class Dfsu3D(DfsuLayered):
     @property
-    def geometry2d(self):
+    def geometry2d(self) -> GeometryFM2D:
         """The 2d geometry for a 3d object"""
         return self.geometry.geometry2d
 
     def extract_surface_elevation_from_3d(self, n_nearest: int = 4) -> DataArray:
         """
         Extract surface elevation from a 3d dfsu file (based on zn)
         to a new 2d dfsu file with a surface elevation item.
```

### Comparing `mikeio-2.0b0/mikeio/dfsu/_mesh.py` & `mikeio-2.0b1/mikeio/dfsu/_mesh.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/dfsu/_spectral.py` & `mikeio-2.0b1/mikeio/dfsu/_spectral.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Sized, Tuple, Any
+from typing import Sequence, Sized, Tuple, Any
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 from mikecore.DfsuFile import DfsuFile, DfsuFileType
 from tqdm import trange
 
@@ -33,15 +33,15 @@
         self._type = info.type
         self._deletevalue = info.deletevalue
         self._time = info.time
         self._timestep = info.timestep
         self._items = info.items
         self._geometry = self._read_geometry(self._filename)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         out = [f"<mikeio.{self.__class__.__name__}>"]
 
         if self._type is not DfsuFileType.DfsuSpectral0D:
             if self._type is not DfsuFileType.DfsuSpectral1D:
                 out.append(f"number of elements: {self.geometry.n_elements}")
             out.append(f"number of nodes: {self.geometry.n_nodes}")
         if self.geometry.is_spectral:
@@ -52,15 +52,15 @@
         if self.geometry.projection_string:
             out.append(f"projection: {self.geometry.projection_string}")
         if self.n_items < 10:
             out.append("items:")
             for i, item in enumerate(self.items):
                 out.append(f"  {i}:  {item}")
         else:
-            out.append(f"number of items: {self.geometry.n_items}")
+            out.append(f"number of items: {self.n_items}")
         if self.n_timesteps == 1:
             out.append(f"time: time-invariant file (1 step) at {self.time[0]}")
         else:
             out.append(
                 f"time: {str(self.time[0])} - {str(self.time[-1])} ({self.n_timesteps} records)"
             )
         return str.join("\n", out)
@@ -158,30 +158,30 @@
                     frequencies=frequencies,
                     directions=directions,
                 )
         dfs.Close()
         return geometry
 
     @property
-    def n_frequencies(self):
+    def n_frequencies(self) -> int | None:
         """Number of frequencies"""
         return 0 if self.frequencies is None else len(self.frequencies)
 
     @property
-    def frequencies(self):
+    def frequencies(self) -> np.ndarray | None:
         """Frequency axis"""
         return self.geometry._frequencies
 
     @property
-    def n_directions(self):
+    def n_directions(self) -> int | None:
         """Number of directions"""
         return 0 if self.directions is None else len(self.directions)
 
     @property
-    def directions(self):
+    def directions(self) -> np.ndarray | None:
         """Directional axis"""
         return self.geometry._directions
 
     def _get_spectral_data_shape(
         self, n_steps: int, elements: Sized | None, dfsu_type: DfsuFileType
     ) -> Tuple[Tuple[int, ...], Tuple[int, ...], Tuple[str, ...]]:
         dims = [] if n_steps == 1 else ["time"]
@@ -218,23 +218,23 @@
             dims.append("frequency")
 
         return read_shape, shape, tuple(dims)
 
     def read(
         self,
         *,
-        items=None,
-        time=None,
-        elements=None,
-        nodes=None,
-        area=None,
-        x=None,
-        y=None,
-        keepdims=False,
-        dtype=np.float32,
+        items: str | int | Sequence[str | int] | None = None,
+        time: int | str | slice | None = None,
+        elements: Sequence[int] | np.ndarray | None = None,
+        nodes: Sequence[int] | np.ndarray | None = None,
+        area: Tuple[float, float, float, float] | None = None,
+        x: float | None = None,
+        y: float | None = None,
+        keepdims: bool = False,
+        dtype: Any = np.float32,
     ) -> Dataset:
         """
         Read data from a spectral dfsu file
 
         Parameters
         ---------
         items: list[int] or list[str], optional
@@ -348,15 +348,20 @@
         dfs.Close()
 
         time = pd.to_datetime(t_seconds, unit="s", origin=self.start_time)
         return Dataset(
             data_list, time, items, geometry=geometry, dims=dims, validate=False
         )
 
-    def _parse_geometry_sel(self, area, x, y):
+    def _parse_geometry_sel(
+        self,
+        area: Tuple[float, float, float, float] | None,
+        x: float | None,
+        y: float | None,
+    ) -> np.ndarray | None:
         """Parse geometry selection
 
         Parameters
         ----------
         area : list[float], optional
             Read only data inside (horizontal) area given as a
             bounding box (tuple with left, lower, right, upper)
@@ -377,27 +382,37 @@
         ------
         ValueError
             If no elements are found in selection
         """
         elements = None
 
         if area is not None:
+            assert isinstance(
+                self.geometry, (GeometryFMLineSpectrum, GeometryFMAreaSpectrum)
+            )
             elements = self.geometry._elements_in_area(area)
 
         if (x is not None) or (y is not None):
+            assert isinstance(
+                self.geometry, (GeometryFMLineSpectrum, GeometryFMAreaSpectrum)
+            )
             elements = self.geometry.find_index(x=x, y=y)
 
         if (x is not None) or (y is not None) or (area is not None):
             # selection was attempted
             if (elements is None) or len(elements) == 0:
                 raise ValueError("No elements in selection!")
 
         return elements
 
-    def _parse_elements_nodes(self, elements, nodes):
+    def _parse_elements_nodes(
+        self,
+        elements: Sequence[int] | np.ndarray | None,
+        nodes: Sequence[int] | np.ndarray | None,
+    ) -> Tuple[Any, Any]:
         if self._type == DfsuFileType.DfsuSpectral0D:
             if elements is not None or nodes is not None:
                 raise ValueError(
                     "Reading specific elements/nodes is not supported for DfsuSpectral0D"
                 )
             geometry = self.geometry
             return geometry, None
@@ -406,31 +421,33 @@
             if elements is not None:
                 raise ValueError(
                     "Reading specific elements is not supported for DfsuSpectral1D"
                 )
             if nodes is None:
                 geometry = self.geometry
             else:
-                geometry = self.geometry._nodes_to_geometry(nodes)
-                nodes = [nodes] if np.isscalar(nodes) else nodes
+                geometry = self.geometry._nodes_to_geometry(nodes)  # type: ignore
+                nodes = [nodes] if np.isscalar(nodes) else nodes  # type: ignore
             return geometry, nodes
 
         elif self._type == DfsuFileType.DfsuSpectral2D:
             if nodes is not None:
                 raise ValueError(
                     "Reading specific nodes is only supported for DfsuSpectral1D"
                 )
             if elements is None:
                 geometry = self.geometry
             else:
                 elements = (
-                    [elements] if np.isscalar(elements) else list(elements)
+                    [elements] if np.isscalar(elements) else list(elements)  # type: ignore
                 )  # TODO check this
-                geometry = self.geometry.elements_to_geometry(elements)
-            return geometry, elements
+                geometry = self.geometry.elements_to_geometry(elements)  # type: ignore
+            return geometry, elements  # type: ignore
+
+        raise NotImplementedError(f"Not valid for type:{self._type}")
 
     def calc_Hm0_from_spectrum(
         self, spectrum: np.ndarray | DataArray, tail: bool = True
     ) -> np.ndarray:
         """Calculate significant wave height (Hm0) from spectrum
 
         Parameters
```

### Comparing `mikeio-2.0b0/mikeio/eum/_eum.py` & `mikeio-2.0b1/mikeio/eum/_eum.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 2800
 >>>
 
 """
 
 from __future__ import annotations
 from enum import IntEnum
-from typing import Dict, List, Sequence, Literal
+from typing import Any, Sequence, Literal
 
 import pandas as pd
 from mikecore.DfsFile import DataValueType, DfsDynamicItemInfo
-from mikecore.eum import eumUnit, eumWrapper
+from mikecore.eum import eumUnit, eumItem, eumWrapper
 
 from ..exceptions import InvalidDataValueType
 
 
-def _type_list(search=None):
+def _type_list(search: str | None = None) -> dict[eumItem, str]:
     """Get a dictionary of the EUM items
 
     Notes
     -----
     An alternative to `type_list` is to use `mikeio.eum.Item`
 
     Parameters
@@ -65,15 +65,15 @@
                 if search in value.lower() or search == value.lower()
             ]
         )
 
     return items
 
 
-def _unit_list(eum_type: int) -> Dict[str, eumUnit]:
+def _unit_list(eum_type: int) -> dict[str, eumUnit]:
     """Get a dictionary of valid units
 
     Parameters
     ----------
     type_enum: int
         EUM variable type, e.g. 100006 or EUMType.Temperature
 
@@ -94,15 +94,15 @@
 class TimeAxisType(IntEnum):
 
     EquidistantRelative = 1
     NonEquidistantRelative = 2
     EquidistantCalendar = 3
     NonEquidistantCalendar = 4
 
-    def __repr__(self):
+    def __repr__(self) -> str:
 
         return self.name
 
 
 class TimeStepUnit(IntEnum):
 
     SECOND = 1400
@@ -713,38 +713,38 @@
     NearBedLoad_per_Length = 110307
     Substance_per_UnitArea = 110308
     AccNearBedLoad_per_Length = 110309
     ThermalConductivity = 110310
     DirectionalVariance = 110311
     SpecificDissipationRate = 110312
 
-    def __init__(self, code):
+    def __init__(self, code: int) -> None:
         self.code = code
 
     @property
-    def display_name(self):
+    def display_name(self) -> str:
         """Display friendly name"""
         name = self.name
         name = name.replace("_", " ")
         return name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
 
         return self.display_name
 
     @property
-    def units(self):
+    def units(self) -> list[EUMUnit]:
         """List valid units for this EUM type"""
-        temp = _unit_list(self.code).items()
-        return [EUMUnit(value) for _, value in temp]
+        temp = _unit_list(self.code).values()
+        return [EUMUnit(value) for value in temp]
 
     @staticmethod
-    def search(pattern) -> List["EUMType"]:
-        temp = _type_list(pattern).items()
-        return [EUMType(key) for key, _ in temp]
+    def search(pattern: str) -> list[EUMType]:
+        temp = _type_list(pattern).keys()
+        return [EUMType(key) for key in temp]
 
 
 class EUMUnit(IntEnum):
     """EUM unit
 
     Examples
     --------
@@ -1355,26 +1355,26 @@
     mS_per_cm = 99261
     mu_S_per_cm = 99262
     kg_per__meter_sec_ = 99263
     cPoise = 99264
     lbf_sec_per_feet_pow_2 = 99265
     pound_per__sec_feet_ = 99266
 
-    def __init__(self, code):
+    def __init__(self, code: int) -> None:
         self.code = code
 
     @property
-    def display_name(self):
+    def display_name(self) -> str:
         """Display friendly name"""
         name = self.name
         name = name.replace("_", " ")
         return name
 
     @property
-    def short_name(self):
+    def short_name(self) -> str:
 
         unit_short_names = {
             "kilometer": "km",
             "centimeter": "cm",
             "millimeter": "mm",
             "meter": "m",
             "liter": "l",
@@ -1391,15 +1391,15 @@
         }
 
         name = self.name
         for key, value in unit_short_names.items():
             name = name.replace(key, value)
         return name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
 
         return self.display_name
 
 
 class ItemInfo:
     """ItemInfo
 
@@ -1478,27 +1478,27 @@
 
         self.data_value_type = to_datatype(data_value_type)
 
         if not isinstance(name, str):
             raise ValueError("Invalid name, name should be a string")
         self.name: str = name
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         if not isinstance(other, ItemInfo):
             return NotImplemented
 
         # an alternative approach to this long expression is to use dataclasses (Python>=3.7)
         return (
             self.name == other.name
             and self.type == other.type
             and self.unit == other.unit
             and self.data_value_type == other.data_value_type
         )
 
-    def __repr__(self):
+    def __repr__(self) -> str:
 
         if self.data_value_type == DataValueType.Instantaneous:
             return f"{self.name} <{self.type.display_name}> ({self.unit.display_name})"
         else:
             return f"{self.name} <{self.type.display_name}> ({self.unit.display_name}) - {self.data_value_type}"
 
     @staticmethod
@@ -1514,15 +1514,15 @@
         return ItemInfo(name, itemtype, unit, data_value_type)
 
 
 class ItemInfoList(list):
     def __init__(self, items: Sequence[ItemInfo]):
         super().__init__(items)
 
-    def to_dataframe(self):
+    def to_dataframe(self) -> pd.DataFrame:
         data = [
             {"name": item.name, "type": item.type.name, "unit": item.unit.name}
             for item in self
         ]
         return pd.DataFrame(data)
```

### Comparing `mikeio-2.0b0/mikeio/pfs/__init__.py` & `mikeio-2.0b1/mikeio/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/pfs/_pfsdocument.py` & `mikeio-2.0b1/mikeio/pfs/_pfsdocument.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from __future__ import annotations
 import re
 import warnings
 from collections import Counter
 from collections.abc import Mapping, Sequence
 from datetime import datetime
 from pathlib import Path
-from typing import Callable, Dict, List, TextIO, Tuple
+from typing import Any, Callable, Dict, List, TextIO, Tuple
 
 import yaml
 
 from ._pfssection import PfsNonUniqueList, PfsSection
 
 
-def parse_yaml_preserving_duplicates(src, unique_keywords=False):
+def parse_yaml_preserving_duplicates(
+    src: Any, unique_keywords: bool = False
+) -> dict[str, Any]:
     class PreserveDuplicatesLoader(yaml.loader.Loader):
         pass
 
-    def map_constructor_duplicates(loader, node, deep=False):
+    def map_constructor_duplicates(loader: Any, node: Any, deep: bool = False) -> Any:
         keys = [loader.construct_object(node, deep=deep) for node, _ in node.value]
         vals = [loader.construct_object(node, deep=deep) for _, node in node.value]
         key_count = Counter(keys)
         data = {}
         for key, val in zip(keys, vals):
             if key_count[key] > 1:
                 if key not in data:
                     data[key] = PfsNonUniqueList()
                 data[key].append(val)
             else:
                 data[key] = val
         return data
 
-    def map_constructor_duplicate_sections(loader, node, deep=False):
+    def map_constructor_duplicate_sections(
+        loader: Any, node: Any, deep: bool = False
+    ) -> Any:
         keys = [loader.construct_object(node, deep=deep) for node, _ in node.value]
         vals = [loader.construct_object(node, deep=deep) for _, node in node.value]
         key_count = Counter(keys)
         data = {}
         for key, val in zip(keys, vals):
             if key_count[key] > 1:
                 if isinstance(val, dict):
@@ -79,24 +83,24 @@
         If True: warnings will be issued if non-unique keywords
         are present and the first occurence will be used
         by default False
     """
 
     def __init__(
         self,
-        data: TextIO | PfsSection | Dict | str | Path,
+        data: TextIO | PfsSection | Mapping[str | PfsSection, Any] | str | Path,
         *,
-        encoding="cp1252",
-        names=None,
-        unique_keywords=False,
-    ):
+        encoding: str = "cp1252",
+        names: Sequence[str] | None = None,
+        unique_keywords: bool = False,
+    ) -> None:
         if isinstance(data, (str, Path)) or hasattr(data, "read"):
             if names is not None:
                 raise ValueError("names cannot be given as argument if input is a file")
-            names, sections = self._read_pfs_file(data, encoding, unique_keywords)
+            names, sections = self._read_pfs_file(data, encoding, unique_keywords)  # type: ignore
         else:
             names, sections = self._parse_non_file_input(data, names)
 
         d = self._to_nonunique_key_dict(names, sections)
         super().__init__(d)
 
         self._ALIAS_LIST = ["_ALIAS_LIST"]  # ignore these in key list
@@ -108,35 +112,35 @@
         """Create a PfsDocument from a string"""
         from io import StringIO
 
         f = StringIO(text)
         return PfsDocument(f)
 
     @staticmethod
-    def _to_nonunique_key_dict(keys, vals):
+    def _to_nonunique_key_dict(keys: Any, vals: Any) -> dict[Any, Any]:
         key_count = Counter(keys)
         data = {}
         for key, val in zip(keys, vals):
             if key_count[key] > 1:
                 if key not in data:
                     data[key] = PfsNonUniqueList()
                 data[key].append(val)
             else:
                 data[key] = val
         return data
 
-    def keys(self):
+    def keys(self) -> List[str]:  # type: ignore
         """Return a list of the PfsDocument's keys (target names)"""
         return [k for k, _ in self.items()]
 
-    def values(self):
+    def values(self) -> List[PfsSection | PfsNonUniqueList]:  # type: ignore
         """Return a list of the PfsDocument's values (targets)."""
         return [v for _, v in self.items()]
 
-    def items(self):
+    def items(self) -> List[Tuple[str, PfsSection | PfsNonUniqueList]]:  # type: ignore
         """Return a new view of the PfsDocument's items ((key, value) pairs)"""
         return [(k, v) for k, v in self.__dict__.items() if k not in self._ALIAS_LIST]
 
     def to_dict(self) -> dict:
         """Convert to (nested) dict (as a copy)"""
         d = super().to_dict()
         _ = d.pop("_ALIAS_LIST")
@@ -181,33 +185,43 @@
     def copy(self) -> PfsDocument:
         """Return a deep copy of the PfsDocument"""
 
         text = repr(self)
 
         return PfsDocument.from_text(text)
 
-    def _read_pfs_file(self, filename, encoding, unique_keywords=False):
+    def _read_pfs_file(
+        self,
+        filename: str | Path | TextIO,
+        encoding: str | None,
+        unique_keywords: bool = False,
+    ) -> Tuple[List[str], List[PfsSection]]:
         try:
             yml = self._pfs2yaml(filename, encoding)
             target_list = parse_yaml_preserving_duplicates(yml, unique_keywords)
         except (
             AttributeError
         ):  # This is the error raised if parsing fails, try again with the normal loader
             target_list = yaml.load(yml, Loader=yaml.CFullLoader)
         except FileNotFoundError as e:
             raise FileNotFoundError(str(e))
         except Exception as e:
             raise ValueError(f"{filename} could not be parsed. " + str(e))
-        sections = [PfsSection(list(d.values())[0]) for d in target_list]
-        names = [list(d.keys())[0] for d in target_list]
+        sections = [PfsSection(list(d.values())[0]) for d in target_list]  # type: ignore
+        names = [list(d.keys())[0] for d in target_list]  # type: ignore
         return names, sections
 
     @staticmethod
     def _parse_non_file_input(
-        input: Dict | PfsSection | Sequence[PfsSection] | Sequence[Dict],
+        input: (
+            Mapping[str | PfsSection, Any]
+            | PfsSection
+            | Sequence[PfsSection]
+            | Sequence[Dict]
+        ),
         names: Sequence[str] | None = None,
     ) -> Tuple[Sequence[str], List[PfsSection]]:
         """dict/PfsSection or lists of these can be parsed"""
         if names is None:
             assert isinstance(input, Mapping), "input must be a mapping"
             names, sections = PfsDocument._unravel_items(input.items)
             for sec in sections:
@@ -237,15 +251,15 @@
         if len(names) != len(sections):
             raise ValueError(
                 f"Length of names ({len(names)}) does not match length of target sections ({len(sections)})"
             )
         return names, sections
 
     @property
-    def _is_FM_engine(self):
+    def _is_FM_engine(self) -> bool:
         return "FemEngine" in self.names[0]
 
     def _add_all_FM_aliases(self) -> None:
         """create MIKE FM module aliases"""
         self._add_FM_alias("HD", "HYDRODYNAMIC_MODULE")
         self._add_FM_alias("SW", "SPECTRAL_WAVE_MODULE")
         self._add_FM_alias("TR", "TRANSPORT_MODULE")
```

### Comparing `mikeio-2.0b0/mikeio/pfs/_pfssection.py` & `mikeio-2.0b1/mikeio/pfs/_pfssection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 from __future__ import annotations
+from collections.abc import KeysView, ValuesView
 from datetime import datetime
 from types import SimpleNamespace
-from typing import Any, Callable, Dict, List, Mapping, MutableMapping, Sequence
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    ItemsView,
+    List,
+    Mapping,
+    MutableMapping,
+    Sequence,
+)
 
 import pandas as pd
 
 
 def _merge_dict(a: Dict[str, Any], b: Mapping[str, Any]) -> Dict[str, Any]:
     """merges dict b into dict a; handling non-unique keys"""
     for key in b:
@@ -20,15 +30,15 @@
     return a
 
 
 class PfsNonUniqueList(list):
     pass
 
 
-class PfsSection(SimpleNamespace, MutableMapping):
+class PfsSection(SimpleNamespace, MutableMapping[str, Any]):
     @staticmethod
     def from_dataframe(df: pd.DataFrame, prefix: str) -> "PfsSection":
         """Create a PfsSection from a DataFrame
 
         Parameters
         ----------
         df: dataframe
@@ -49,44 +59,44 @@
         mikeio.PfsSection.from_dataframe(df,"STATION_")
         ```
         """
         d = {f"{prefix}{idx}": row.to_dict() for idx, row in df.iterrows()}
 
         return PfsSection(d)
 
-    def __init__(self, dictionary, **kwargs):
+    def __init__(self, dictionary: Mapping[str, Any], **kwargs: Any) -> None:
         super().__init__(**kwargs)
         for key, value in dictionary.items():
             self.__set_key_value(key, value, copy=True)
 
     def __repr__(self) -> str:
         return "\n".join(self._to_txt_lines())
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self.__dict__)
 
-    def __iter__(self):
+    def __iter__(self) -> Any:
         iter(self)
 
-    def __contains__(self, key):
+    def __contains__(self, key: Any) -> bool:
         return key in self.keys()
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return getattr(self, key)
 
-    def __setitem__(self, key, value):
+    def __setitem__(self, key: str, value: Any) -> None:
         self.__set_key_value(key, value)
 
-    def __delitem__(self, key):
+    def __delitem__(self, key: str) -> None:
         if key in self.keys():
             self.__delattr__(key)
         else:
             raise IndexError("Key not found")
 
-    def __set_key_value(self, key, value, copy=False):
+    def __set_key_value(self, key: str, value: Any, copy: bool = False) -> None:
         if value is None:
             value = {}
 
         if isinstance(value, dict):
             d = value.copy() if copy else value
             self.__setattr__(key, PfsSection(d))
         elif isinstance(value, PfsNonUniqueList):
@@ -98,21 +108,21 @@
                     sections.append(PfsSection(d))
                 else:
                     sections.append(self._parse_value(v))
             self.__setattr__(key, sections)
         else:
             self.__setattr__(key, self._parse_value(value))
 
-    def _parse_value(self, v):
+    def _parse_value(self, v: Any) -> Any:
         if isinstance(v, str) and self._str_is_scientific_float(v):
             return float(v)
         return v
 
     @staticmethod
-    def _str_is_scientific_float(s):
+    def _str_is_scientific_float(s: str) -> bool:
         """True: -1.0e2, 1E-4, -0.1E+0.5; False: E12, E-4"""
         if len(s) < 3:
             return False
         if (
             s.count(".") <= 2
             and s.lower().count("e") == 1
             and s.lower()[0] != "e"
@@ -128,44 +138,44 @@
                 float(s)
                 return True
             except ValueError:
                 return False
         else:
             return False
 
-    def pop(self, key, *args):
+    def pop(self, key: Any, default: Any = None) -> Any:
         """If key is in the dictionary, remove it and return its
         value, else return default. If default is not given and
         key is not in the dictionary, a KeyError is raised."""
-        return self.__dict__.pop(key, *args)
+        return self.__dict__.pop(key, default)
 
-    def get(self, key, *args):
+    def get(self, key: Any, default: Any = None) -> Any:
         """Return the value for key if key is in the PfsSection,
         else default. If default is not given, it defaults to None,
         so that this method never raises a KeyError."""
-        return self.__dict__.get(key, *args)
+        return self.__dict__.get(key, default)
 
-    def clear(self):
+    def clear(self) -> None:
         """Remove all items from the PfsSection."""
         return self.__dict__.clear()
 
-    def keys(self):
+    def keys(self) -> KeysView[str]:
         """Return a new view of the PfsSection's keys"""
         return self.__dict__.keys()
 
-    def values(self):
+    def values(self) -> ValuesView[Any]:
         """Return a new view of the PfsSection's values."""
         return self.__dict__.values()
 
-    def items(self):
+    def items(self) -> ItemsView[str, Any]:
         """Return a new view of the PfsSection's items ((key, value) pairs)"""
         return self.__dict__.items()
 
     # TODO: better name
-    def update_recursive(self, key, value):
+    def update_recursive(self, key: Any, value: Any) -> None:
         """Update recursively all matches of key with value"""
         for k, v in self.items():
             if isinstance(v, PfsSection):
                 self[k].update_recursive(key, value)
             elif k == key:
                 self[k] = value
 
@@ -223,17 +233,24 @@
         return (
             self.__class__._merge_PfsSections(results)
             if len(results) > 0
             else PfsSection({})
         )
 
     def _find_patterns_generator(
-        self, keypat=None, parampat=None, secpat=None, keylist=[], case=False
-    ):
+        self,
+        keypat: str | None = None,
+        parampat: Any = None,
+        secpat: str | None = None,
+        keylist: List[str] | None = None,
+        case: bool = False,
+    ) -> Any:
         """Look for patterns in either keys, params or sections"""
+
+        keylist = [] if keylist is None else keylist
         for k, v in self.items():
             kk = str(k) if case else str(k).lower()
 
             if isinstance(v, PfsSection):
                 if secpat and secpat in kk:
                     yield from self._yield_deep_dict(keylist + [k], v)
                 else:
@@ -243,23 +260,23 @@
             else:
                 if keypat and keypat in kk:
                     yield from self._yield_deep_dict(keylist + [k], v)
                 if self._param_match(parampat, v, case):
                     yield from self._yield_deep_dict(keylist + [k], v)
 
     @staticmethod
-    def _yield_deep_dict(keys, val):
+    def _yield_deep_dict(keys: Sequence[str], val: Any) -> Any:
         """yield a deep nested dict with keys with a single deep value val"""
         for j in range(len(keys) - 1, -1, -1):
             d = {keys[j]: val}
             val = d
         yield d
 
     @staticmethod
-    def _param_match(parampat: Any, v: Any, case: bool) -> bool:
+    def _param_match(parampat: Any, v: Any, case: bool) -> Any:
         if parampat is None:
             return False
         if type(v) != type(parampat):
             return False
         if isinstance(v, str):
             vv = str(v) if case else str(v).lower()
             return parampat in vv
@@ -280,15 +297,15 @@
 
     def _to_txt_lines(self) -> List[str]:
         lines: List[str] = []
         self._write_with_func(lines.append, newline="")
         return lines
 
     def _write_with_func(
-        self, func: Callable, level: int = 0, newline: str = "\n"
+        self, func: Callable[[str], Any], level: int = 0, newline: str = "\n"
     ) -> None:
         """Write pfs nested objects
 
         Parameters
         ----------
         func : Callable
             A function that performs the writing e.g. to a file
@@ -328,15 +345,17 @@
                 for subv in v:
                     subv = self._prepare_value_for_write(subv)
                     func(f"{lvl_prefix * level}{k} = {subv}{newline}")
             else:
                 v = self._prepare_value_for_write(v)
                 func(f"{lvl_prefix * level}{k} = {v}{newline}")
 
-    def _prepare_value_for_write(self, v):
+    def _prepare_value_for_write(
+        self, v: str | bool | datetime | list[str | bool | datetime]
+    ) -> str:
         """catch peculiarities of string formatted pfs data
 
         Parameters
         ----------
         v : str
             value from one pfs line
 
@@ -368,15 +387,15 @@
             out = []
             for subv in v:
                 out.append(str(self._prepare_value_for_write(subv)))
             v = ", ".join(out)
 
         return v
 
-    def to_dict(self) -> dict:
+    def to_dict(self) -> dict[str, Any]:
         """Convert to (nested) dict (as a copy)"""
         d = self.__dict__.copy()
         for key, value in d.items():
             if isinstance(value, PfsSection):
                 d[key] = value.to_dict()
         return d
 
@@ -426,14 +445,14 @@
         res = []
         for j in range(n_sections):
             k = f"{prefix}{j+1}"
             res.append(self[k].to_dict())
         return pd.DataFrame(res, index=range(1, n_sections + 1))
 
     @classmethod
-    def _merge_PfsSections(cls, sections: Sequence[Dict]) -> "PfsSection":
+    def _merge_PfsSections(cls, sections: Sequence[dict[str, Any]]) -> "PfsSection":
         """Merge a list of PfsSections/dict"""
         assert len(sections) > 0
         a = sections[0]
         for b in sections[1:]:
             a = _merge_dict(a, b)
         return cls(a)
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_FM_geometry.py` & `mikeio-2.0b1/mikeio/spatial/_FM_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 from collections import namedtuple
 from functools import cached_property
 from pathlib import Path
 from typing import (
-    Collection,
     List,
     Any,
     Literal,
     Sequence,
     Sized,
     Tuple,
     TYPE_CHECKING,
@@ -378,15 +377,15 @@
     @codes.setter
     def codes(self, v: np.ndarray) -> None:
         if len(v) != self.n_nodes:
             raise ValueError(f"codes must have length of nodes ({self.n_nodes})")
         self._codes = np.array(v, dtype=np.int32)
 
     @property
-    def boundary_codes(self):
+    def boundary_codes(self) -> list[int]:
         """Unique list of boundary codes"""
         valid = list(set(self.codes))
         return [code for code in valid if code > 0]
 
 
 class GeometryFM2D(_GeometryFM):
     def __init__(
@@ -940,24 +939,24 @@
         )
 
         # boundary faces are those appearing only once
         bnd_face_id = face_counts == 1
         return all_faces[uf_id[bnd_face_id]]
 
     def isel(
-        self, idx: Collection[int], keepdims: bool = False, **kwargs: Any
+        self, idx: Sequence[int], keepdims: bool = False, **kwargs: Any
     ) -> "GeometryFM2D" | GeometryPoint2D:
         """export a selection of elements to a new geometry
 
         Typically not called directly, but by Dataset/DataArray's
         isel() or sel() methods.
 
         Parameters
         ----------
-        idx : collection(int)
+        idx : list(int)
             collection of element indicies
         keepdims : bool, optional
             Should the original Geometry type be kept (keepdims=True)
             or should it be reduced e.g. to a GeometryPoint2D if possible
             (keepdims=False), by default False
 
         Returns
@@ -966,18 +965,15 @@
             geometry subset
 
         See Also
         --------
         find_index : find element indicies for points or an area
         """
 
-        if self._type == DfsuFileType.DfsuSpectral1D:
-            return self._nodes_to_geometry(nodes=idx)
-        else:
-            return self.elements_to_geometry(elements=idx, keepdims=keepdims)
+        return self.elements_to_geometry(elements=idx, keepdims=keepdims)
 
     def find_index(
         self,
         x: float | np.ndarray | None = None,
         y: float | np.ndarray | None = None,
         coords: np.ndarray | None = None,
         area: (
@@ -1068,81 +1064,32 @@
             polygon = np.array(area)
             xy = self.element_coordinates[:, :2]
             mask = self._inside_polygon(polygon, xy)
             return np.where(mask)[0]
         else:
             raise ValueError("'area' must be bbox [x0,y0,x1,y1] or polygon")
 
-    def _nodes_to_geometry(
-        self, nodes: Collection[int]
-    ) -> "GeometryFM2D" | GeometryPoint2D:
-        """export a selection of nodes to new flexible file geometry
-
-        Note: takes only the elements for which all nodes are selected
-
-        Parameters
-        ----------
-        nodes : list(int)
-            list of node ids
-
-        Returns
-        -------
-        UnstructuredGeometry
-            which can be used for further extraction or saved to file
-        """
-        nodes = np.atleast_1d(nodes)  # type: ignore
-        if len(nodes) == 1:
-            xy = self.node_coordinates[nodes[0], :2]
-            return GeometryPoint2D(xy[0], xy[1])
-
-        elements = []
-        for j, el_nodes in enumerate(self.element_table):
-            if np.all(np.isin(el_nodes, nodes)):
-                elements.append(j)
-
-        assert len(elements) > 0, "no elements found"
-        elements = np.sort(elements)  # make sure elements are sorted!
-
-        node_ids, elem_tbl = self._get_nodes_and_table_for_elements(elements)
-        node_coords = self.node_coordinates[node_ids]
-        codes = self.codes[node_ids]
-
-        return GeometryFM2D(
-            node_coordinates=node_coords,
-            codes=codes,
-            node_ids=node_ids,
-            dfsu_type=self._type,
-            projection=self.projection_string,
-            element_table=elem_tbl,
-            element_ids=self.element_ids[elements],
-            reindex=True,
-        )
-
     def elements_to_geometry(
-        self, elements: int | Collection[int], keepdims: bool = False
+        self, elements: int | Sequence[int], keepdims: bool = False
     ) -> "GeometryFM2D" | GeometryPoint2D:
         if isinstance(elements, (int, np.integer)):
             sel_elements: List[int] = [elements]
         else:
             sel_elements = list(elements)
         if len(sel_elements) == 1 and not keepdims:
             x, y, _ = self.element_coordinates[sel_elements.pop(), :]
 
             return GeometryPoint2D(x=x, y=y, projection=self.projection)
 
-        sorted_elements = np.sort(
-            sel_elements
-        )  # make sure elements are sorted! # TODO is this necessary? If so, should be done in the initialiser
-
         # extract information for selected elements
 
-        node_ids, elem_tbl = self._get_nodes_and_table_for_elements(sorted_elements)
+        node_ids, elem_tbl = self._get_nodes_and_table_for_elements(sel_elements)
         node_coords = self.node_coordinates[node_ids]
         codes = self.codes[node_ids]
-        elem_ids = self.element_ids[sorted_elements]
+        elem_ids = self.element_ids[sel_elements]
 
         return GeometryFM2D(
             node_coordinates=node_coords,
             codes=codes,
             node_ids=node_ids,
             projection=self.projection_string,
             element_table=elem_tbl,
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_FM_geometry_layered.py` & `mikeio-2.0b1/mikeio/spatial/_FM_geometry_layered.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 from functools import cached_property
-from typing import Any, Collection, Iterable, Literal, Sequence, List, Tuple
+from pathlib import Path
 
+from typing import Any, Iterable, Literal, Sequence, List, Tuple
+
+from matplotlib.axes import Axes
 import numpy as np
 from mikecore.DfsuFile import DfsuFileType
 
 
 from ._FM_geometry import GeometryFM2D, _GeometryFM, _GeometryFMPlotter
 from ._geometry import GeometryPoint3D
 
-from ._FM_utils import _plot_vertical_profile
+from ._FM_utils import _plot_vertical_profile, BoundaryPolylines
 
 from ._utils import _relative_cumulative_distance
 
 Layer = Literal["all", "bottom", "top"]
 
 
 class _GeometryFMLayered(_GeometryFM):
@@ -65,78 +68,74 @@
         )
 
     @cached_property
     def geometry2d(self) -> GeometryFM2D:
         return self.to_2d_geometry()
 
     def isel(
-        self, idx: Collection[int], keepdims: bool = False, **kwargs: Any
+        self, idx: Sequence[int], keepdims: bool = False, **kwargs: Any
     ) -> GeometryFM3D | GeometryPoint3D | GeometryFM2D | GeometryFMVerticalColumn:
 
         return self.elements_to_geometry(elements=idx, keepdims=keepdims)
 
     def elements_to_geometry(
         self,
-        elements: int | Collection[int],
+        elements: int | Sequence[int] | np.ndarray,
         node_layers: Layer = "all",
         keepdims: bool = False,
     ) -> GeometryFM3D | GeometryPoint3D | GeometryFM2D | GeometryFMVerticalColumn:
         sel_elements: List[int]
 
         if isinstance(elements, (int, np.integer)):
             sel_elements = [elements]
         else:
             sel_elements = list(elements)
         if len(sel_elements) == 1 and not keepdims:
             x, y, z = self.element_coordinates[sel_elements.pop(), :]
 
             return GeometryPoint3D(x=x, y=y, z=z, projection=self.projection)
 
-        sorted_elements = np.sort(
-            sel_elements
-        )  # make sure elements are sorted! # TODO is this necessary?
-
         # create new geometry
         new_type = self._type
 
-        layers_used = self.layer_ids[sorted_elements]
+        layers_used = self.layer_ids[sel_elements]
         unique_layer_ids = np.unique(layers_used)
         n_layers = len(unique_layer_ids)
 
         if n_layers > 1:
             bottom: Layer = "bottom"
             elem_bot = self.get_layer_elements(layers=bottom)
-            if np.all(np.in1d(sorted_elements, elem_bot)):
+            if np.all(np.in1d(sel_elements, elem_bot)):
                 n_layers = 1
 
         if (
             self._type == DfsuFileType.Dfsu3DSigma
             or self._type == DfsuFileType.Dfsu3DSigmaZ
         ) and n_layers == 1:
             new_type = DfsuFileType.Dfsu2D
 
         if n_layers == 1 and node_layers == "all":
             node_layers = "bottom"
 
         # extract information for selected elements
         if n_layers == 1:
-            elem2d = self.elem2d_ids[sorted_elements]
+            elem2d = self.elem2d_ids[sel_elements]
             geom2d = self.geometry2d
             node_ids, elem_tbl = geom2d._get_nodes_and_table_for_elements(elem2d)
             assert len(elem_tbl[0]) <= 4, "Not a 2D element"
             node_coords = geom2d.node_coordinates[node_ids]
             codes = geom2d.codes[node_ids]
             elem_ids = self._element_ids[elem2d]
         else:
             node_ids, elem_tbl = self._get_nodes_and_table_for_elements(
-                sorted_elements, node_layers=node_layers
+                sel_elements, node_layers=node_layers
             )
             node_coords = self.node_coordinates[node_ids]
             codes = self.codes[node_ids]
-            elem_ids = self._element_ids[sorted_elements]
+            elem_ids = self._element_ids[sel_elements]
 
         if new_type == DfsuFileType.Dfsu2D:
             return GeometryFM2D(
                 node_coordinates=node_coords,
                 codes=codes,
                 node_ids=node_ids,
                 projection=self.projection_string,
@@ -179,15 +178,15 @@
     @cached_property
     def element_coordinates(self) -> np.ndarray:
         """Center coordinates of each element"""
         return self._calc_element_coordinates(maxnodes=8)
 
     def _get_nodes_and_table_for_elements(
         self,
-        elements: Collection[int] | np.ndarray,
+        elements: Sequence[int] | np.ndarray,
         node_layers: Layer = "all",
     ) -> Tuple[Any, Any]:
         """list of nodes and element table for a list of elements
 
         Parameters
         ----------
         elements : np.array(int)
@@ -265,36 +264,36 @@
                     znj_3d = self.node_coordinates[elem_nodes3d[jn], 2]
                     zn[elem_nodes[jn]] = min(zn[elem_nodes[jn]], znj_3d)
             geom.node_coordinates[:, 2] = zn
 
         return geom
 
     @cached_property
-    def n_elements(self):
+    def n_elements(self) -> int:
         """Number of 3d elements"""
         return len(self.element_table)
 
     @property
-    def n_nodes(self):
+    def n_nodes(self) -> int:
         return len(self.node_coordinates)
 
     @property
-    def is_2d(self):
+    def is_2d(self) -> bool:
         return False
 
     @property
     def ndim(self) -> int:
         return 3
 
     @property
     def is_layered(self) -> bool:
         return True
 
     @cached_property
-    def layer_ids(self):
+    def layer_ids(self) -> np.ndarray:
         """The layer number (0=bottom, 1, 2, ...) for each 3d element"""
         if self._layer_ids is None:
             res = self._get_2d_to_3d_association()
             self._e2_e3_table = res[0]
             self._2d_ids = res[1]
             self._layer_ids = res[2]
         return self._layer_ids
@@ -311,30 +310,32 @@
 
     @property
     def n_z_layers(self) -> int:
         """Maximum number of z-layers"""
         return self.n_layers - self.n_sigma_layers
 
     @cached_property
-    def top_elements(self):
+    def top_elements(self) -> np.ndarray:
         """List of 3d element ids of surface layer"""
         # note: if subset of elements is selected then this cannot be done!
 
         # fast path if no z-layers
         if self.n_z_layers == 0:
             return np.arange(
                 start=self.n_sigma_layers - 1,
                 stop=self.n_elements,
                 step=self.n_sigma_layers,
             )
         else:
             # slow path
             return self._find_top_layer_elements(self.element_table)
 
-    def _elements_in_area(self, area):
+    def _elements_in_area(
+        self, area: Sequence[Tuple[float, float]] | Sequence[float]
+    ) -> np.ndarray:
         """Find element ids of elements inside area"""
         idx2d = self.geometry2d._elements_in_area(area)
         if len(idx2d) > 0:
             return np.hstack(self.e2_e3_table[idx2d])
         else:
             return np.array([], dtype=int)
 
@@ -408,15 +409,15 @@
         return n_layers_column
 
     @cached_property
     def bottom_elements(self) -> np.ndarray:
         """List of 3d element ids of bottom layer"""
         return self.top_elements - self.n_layers_per_column + 1
 
-    def get_layer_elements(self, layers: int | Layer | Iterable[int]) -> np.ndarray:
+    def get_layer_elements(self, layers: int | Layer | Sequence[int]) -> np.ndarray:
         """3d element ids for one (or more) specific layer(s)
 
         Parameters
         ----------
         layers : int or list(int)
             layer between 0 (bottom) and n_layers-1 (top)
             (can also be negative counting from -1 at the top layer)
@@ -505,38 +506,41 @@
                 layerid.append(ll)
 
         e2_to_e3 = np.array(e2_to_e3, dtype=object)
         index2d = np.array(index2d)
         layerid = np.array(layerid)
         return e2_to_e3, index2d, layerid
 
-    def _z_idx_in_column(self, e3_col, z):
+    def _z_idx_in_column(self, e3_col: np.ndarray, z: np.ndarray) -> np.ndarray:
         dz = self._dz[e3_col]
         z_col = self.element_coordinates[e3_col, 2]
         z_face = np.append(z_col - dz / 2, z_col[-1] + dz[-1] / 2)
         if z < z_face[0] or z > z_face[-1]:
             xy = tuple(self.element_coordinates[e3_col[0], :2])
             raise ValueError(
                 f"z value '{z}' is outside water column [{z_face[0]},{z_face[-1]}] in point x,y={xy}"
             )
         idx = np.searchsorted(z_face, z) - 1
         return idx
 
-    def _find_elem3d_from_elem2d(self, elem2d, z):
+    def _find_elem3d_from_elem2d(
+        self, elem2d: int | np.ndarray, z: np.ndarray | float
+    ) -> np.ndarray:
         """Find 3d element ids from 2d element ids and z-values"""
 
         # TODO: coordinate with _find_3d_from_2d_points()
 
         elem2d = [elem2d] if np.isscalar(elem2d) else elem2d
         elem2d = np.asarray(elem2d)
         z_vec = np.full(elem2d.shape, fill_value=z) if np.isscalar(z) else z
+
         elem3d = np.full_like(elem2d, fill_value=-1)
         for j, e2 in enumerate(elem2d):
             idx_3d = np.hstack(self.e2_e3_table[e2])
-            elem3d[j] = idx_3d[self._z_idx_in_column(idx_3d, z_vec[j])]
+            elem3d[j] = idx_3d[self._z_idx_in_column(idx_3d, z_vec[j])]  # type: ignore
 
             # z_col = self.element_coordinates[idx_3d, 2]
             # elem3d[j] = (np.abs(z_col - z_vec[j])).argmin()  # nearest
         return elem3d
 
     # def _find_3d_from_2d_points(self, elem2d, z=None, layer=None):
 
@@ -585,19 +589,19 @@
     #         idx = idx[0]
     #     else:
     #         idx = np.reshape(idx, orig_shape)
 
     #     return idx
 
     @cached_property
-    def _dz(self):
+    def _dz(self) -> np.ndarray:
         """Height of each 3d element (using static zn information)"""
         return self._calc_dz()
 
-    def _calc_dz(self):
+    def _calc_dz(self) -> np.ndarray:
         """Height of 3d elements using static or dynamic zn information"""
         element_table = self.element_table
         n_elements = len(element_table)
 
         zn = self.node_coordinates[:, 2]
         zn_is_2d = len(zn.shape) == 2
         shape = (zn.shape[0], n_elements) if zn_is_2d else (n_elements,)
@@ -642,21 +646,21 @@
             n_sigma=n_sigma,
             validate=validate,
             reindex=reindex,
         )
         self.plot = _GeometryFMPlotter(self)
 
     @property
-    def boundary_polylines(self):
+    def boundary_polylines(self) -> BoundaryPolylines:
         return self.geometry2d.boundary_polylines
 
-    def contains(self, points) -> np.ndarray:
+    def contains(self, points: np.ndarray) -> np.ndarray:
         return self.geometry2d.contains(points)
 
-    def to_mesh(self, outfilename):
+    def to_mesh(self, outfilename: str | Path) -> None:
         return self.geometry2d.to_mesh(outfilename)
 
     def find_index(
         self,
         x: float | None = None,
         y: float | None = None,
         z: float | None = None,
@@ -730,15 +734,15 @@
             n_sigma=n_sigma,
             validate=validate,
             reindex=reindex,
         )
         self.plot = _GeometryFMVerticalProfilePlotter(self)
 
     @cached_property
-    def relative_element_distance(self):
+    def relative_element_distance(self) -> np.ndarray:
         ec = self.element_coordinates
         nc0 = self.node_coordinates[0, :2]
         return _relative_cumulative_distance(ec, nc0, is_geo=self.is_geo)
 
     def get_nearest_relative_distance(self, coords: Tuple[float, float]) -> float:
         """For a point near a transect, find the nearest relative distance
         for showing position on transect plot.
@@ -755,15 +759,22 @@
         """
         xe = self.element_coordinates[:, 0]
         ye = self.element_coordinates[:, 1]
         dd2 = np.square(xe - coords[0]) + np.square(ye - coords[1])
         idx = np.argmin(dd2)
         return self.relative_element_distance[idx]
 
-    def find_index(self, x=None, y=None, z=None, coords=None, layers=None):
+    def find_index(
+        self,
+        x: float | None = None,
+        y: float | None = None,
+        z: float | None = None,
+        coords: np.ndarray | None = None,
+        layers: int | Sequence[int] | Layer | None = None,
+    ) -> np.ndarray:
 
         if layers is not None:
             idx = self.get_layer_elements(layers)
         else:
             idx = self._element_ids
 
         # select in space
@@ -771,30 +782,30 @@
             (coords is not None)
             or (x is not None)
             or (y is not None)
             or (z is not None)
         ):
             if coords is not None:
                 coords = np.atleast_2d(coords)
-                xy = coords[:, :2]
-                z = coords[:, 2] if coords.shape[1] == 3 else None
+                xy = coords[:, :2]  # type: ignore
+                z = coords[:, 2] if coords.shape[1] == 3 else None  # type: ignore
             else:
-                xy = np.vstack((x, y)).T
+                xy = np.vstack((x, y)).T  # type: ignore
 
             idx_2d = self._find_nearest_element_2d(coords=xy)
 
             if z is None:
                 idx_3d = np.hstack(self.e2_e3_table[idx_2d])
             else:
                 idx_3d = self._find_elem3d_from_elem2d(idx_2d, z)
             idx = np.intersect1d(idx, idx_3d)
 
         return idx
 
-    def _find_nearest_element_2d(self, coords):
+    def _find_nearest_element_2d(self, coords: np.ndarray) -> np.ndarray:
         ec2d = self.element_coordinates[self.top_elements, :2]
         xe, ye = ec2d[:, 0], ec2d[:, 1]
         coords = np.atleast_2d(coords)
         idx = np.zeros(len(coords), dtype=int)
         for j, pt in enumerate(coords):
             x, y = pt[0:2]
             idx[j] = np.argmin((xe - x) ** 2 + (ye - y) ** 2)
@@ -878,25 +889,30 @@
         return zf
 
 
 class _GeometryFMVerticalProfilePlotter:
     def __init__(self, geometry: "GeometryFMVerticalProfile") -> None:
         self.g = geometry
 
-    def __call__(self, ax=None, figsize=None, **kwargs):
+    def __call__(
+        self,
+        ax: Axes | None = None,
+        figsize: Tuple[float, float] | None = None,
+        **kwargs: Any,
+    ) -> Axes:
         import matplotlib.pyplot as plt
 
         if ax is None:
             _, ax = plt.subplots(figsize=figsize)
         x = self.g.node_coordinates[:, 0]
         y = self.g.node_coordinates[:, 1]
         ax.plot(x, y, **kwargs)
         return ax
 
-    def mesh(self, title="Mesh", edge_color="0.5", **kwargs):
+    def mesh(self, title: str = "Mesh", edge_color: str = "0.5", **kwargs: Any) -> Axes:
 
         v = np.full_like(self.g.element_coordinates[:, 0], np.nan)
         return _plot_vertical_profile(
             node_coordinates=self.g.node_coordinates,
             element_table=self.g.element_table,
             values=v,
             is_geo=self.g.is_geo,
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_FM_geometry_spectral.py` & `mikeio-2.0b1/mikeio/spatial/_FM_geometry_spectral.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Collection, Any, Tuple
+from typing import Any, Sequence, Tuple
 
 
 import numpy as np
 from mikecore.DfsuFile import DfsuFileType
 
 
 from ._geometry import _Geometry
@@ -123,20 +123,20 @@
         """Directional axis"""
         return self._directions
 
 
 # TODO reconsider inheritance to avoid overriding method signature
 class GeometryFMAreaSpectrum(_GeometryFMSpectrum):
     def isel(  # type: ignore
-        self, idx: Collection[int], **kwargs: Any
+        self, idx: Sequence[int], **kwargs: Any
     ) -> "GeometryFMPointSpectrum" | "GeometryFMAreaSpectrum":
         return self.elements_to_geometry(elements=idx)
 
     def elements_to_geometry(  # type: ignore
-        self, elements: Collection[int], keepdims: bool = False
+        self, elements: Sequence[int], keepdims: bool = False
     ) -> "GeometryFMPointSpectrum" | "GeometryFMAreaSpectrum":
         """export a selection of elements to new flexible file geometry
         Parameters
         ----------
         elements : list(int)
             list of element ids
         keepdims: bool
@@ -152,15 +152,14 @@
             return GeometryFMPointSpectrum(
                 frequencies=self._frequencies,
                 directions=self._directions,
                 x=coords[0],
                 y=coords[1],
             )
 
-        elements = np.sort(elements)  # make sure elements are sorted!
         node_ids, elem_tbl = self._get_nodes_and_table_for_elements(elements)
         node_coords = self.node_coordinates[node_ids]
         codes = self.codes[node_ids]
 
         geom = GeometryFMAreaSpectrum(
             node_coordinates=node_coords,
             codes=codes,
@@ -174,27 +173,31 @@
         )
         geom._type = self._type
         return geom
 
 
 # TODO this inherits indirectly from GeometryFM2D, which is not ideal
 class GeometryFMLineSpectrum(_GeometryFMSpectrum):
-    def isel(self, idx=None, axis="node"):
+    def isel(  # type: ignore
+        self, idx: Sequence[int], axis: str = "node"
+    ) -> GeometryFMPointSpectrum | GeometryFMLineSpectrum:
         return self._nodes_to_geometry(nodes=idx)
 
-    def _nodes_to_geometry(self, nodes):
+    def _nodes_to_geometry(  # type: ignore
+        self, nodes: Sequence[int]
+    ) -> GeometryFMPointSpectrum | GeometryFMLineSpectrum:
         """export a selection of nodes to new flexible file geometry
         Note: takes only the elements for which all nodes are selected
         Parameters
         ----------
         nodes : list(int)
             list of node ids
         Returns
         -------
-        UnstructuredGeometry
+        GeometryFMPointSpectrum | GeometryFMLineSpectrum
             which can be used for further extraction or saved to file
         """
         nodes = np.atleast_1d(nodes)
         if len(nodes) == 1:
             coords = self.node_coordinates[nodes[0], :2]
             return GeometryFMPointSpectrum(
                 frequencies=self._frequencies,
@@ -205,26 +208,25 @@
 
         elements = []
         for j, el_nodes in enumerate(self.element_table):
             if np.all(np.isin(el_nodes, nodes)):
                 elements.append(j)
 
         assert len(elements) > 0, "no elements found"
-        elements = np.sort(elements)  # make sure elements are sorted!
 
         node_ids, elem_tbl = self._get_nodes_and_table_for_elements(elements)
         node_coords = self.node_coordinates[node_ids]
         codes = self.codes[node_ids]
 
         geom = GeometryFMLineSpectrum(
             node_coordinates=node_coords,
             codes=codes,
             node_ids=node_ids,
             projection=self.projection_string,
+            dfsu_type=self._type,
             element_table=elem_tbl,
             element_ids=self.element_ids[elements],
             frequencies=self._frequencies,
             directions=self._directions,
             reindex=True,
         )
-        geom._type = self._type  # TODO
         return geom
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_FM_utils.py` & `mikeio-2.0b1/mikeio/spatial/_FM_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+from __future__ import annotations
+from typing import Any, Literal, Sequence, Tuple
+from matplotlib.axes import Axes
+from matplotlib.cm import ScalarMappable
+from matplotlib.collections import PatchCollection
+from matplotlib.colors import Colormap, Normalize
+from matplotlib.figure import Figure
+from matplotlib.tri import Triangulation
 import numpy as np
 from collections import namedtuple
 
 from ._utils import _relative_cumulative_distance
 
 
 MESH_COL = "0.95"
@@ -10,34 +18,36 @@
 BoundaryPolylines = namedtuple(
     "BoundaryPolylines",
     ["n_exteriors", "exteriors", "n_interiors", "interiors"],
 )
 
 
 def _plot_map(
-    node_coordinates,
-    element_table,
-    element_coordinates,
+    node_coordinates: np.ndarray,
+    element_table: np.ndarray,
+    element_coordinates: np.ndarray,
     boundary_polylines: BoundaryPolylines,
-    projection="",
-    z=None,
-    plot_type="patch",
-    title=None,
-    label=None,
-    cmap=None,
-    vmin=None,
-    vmax=None,
-    levels=None,
-    n_refinements=0,
-    show_mesh=False,
-    show_outline=True,
-    figsize=None,
-    ax=None,
-    add_colorbar=True,
-):
+    projection: str = "",
+    z: np.ndarray | None = None,
+    plot_type: Literal[
+        "patch", "mesh_only", "shaded", "contour", "contourf", "outline_only"
+    ] = "patch",
+    title: str | None = None,
+    label: str | None = None,
+    cmap: Colormap | None = None,
+    vmin: float | None = None,
+    vmax: float | None = None,
+    levels: int | Sequence[float] | None = None,
+    n_refinements: int = 0,
+    show_mesh: bool = False,
+    show_outline: bool = True,
+    figsize: Tuple[float, float] | None = None,
+    ax: Axes | None = None,
+    add_colorbar: bool = True,
+) -> Axes:
     """
     Plot unstructured data and/or mesh, mesh outline
 
     Parameters
     ----------
     node_coordinates,
     element_table,
@@ -146,15 +156,15 @@
 
     vmin, vmax, cmap, cmap_norm, cmap_ScMappable, levels = __set_colormap_levels(
         cmap, vmin, vmax, levels, z
     )
     cbar_extend = __cbar_extend(z, vmin, vmax)
 
     if plot_type == "patch":
-        fig_obj = __plot_patch(
+        fig_obj: Any = __plot_patch(
             ax, nc, element_table, show_mesh, cmap, cmap_norm, z, vmin, vmax
         )
 
     else:
         # do node-based triangular plot
         mesh_linewidth = 0.0
         if show_mesh and __is_tri_only(element_table):
@@ -209,20 +219,27 @@
         __add_outline(ax, boundary_polylines)
 
     if add_colorbar:
         __add_colorbar(ax, cmap_ScMappable, fig_obj, label, levels, cbar_extend)
 
     __set_plot_limits(ax, nc)
 
-    ax.set_title(title)
+    if title:
+        ax.set_title(title)
 
     return ax
 
 
-def __set_colormap_levels(cmap, vmin, vmax, levels, z):
+def __set_colormap_levels(
+    cmap: Colormap | str,
+    vmin: float | None,
+    vmax: float | None,
+    levels: int | Sequence[float] | np.ndarray | None,
+    z: np.ndarray,
+) -> Tuple[float, float, Colormap, Normalize, ScalarMappable, np.ndarray]:
     """Set colormap, levels, vmin, vmax, and cmap_norm
 
     Parameters
     ----------
     cmap : str or matplotlib.colors.Colormap
         colormap name or colormap object
     vmin : float
@@ -262,47 +279,47 @@
         vmax = vmin + 0.2
 
     cmap_norm = None
     cmap_ScMappable = None
     if levels is not None:
         if np.isscalar(levels):
             n_levels = levels
-            levels = np.linspace(vmin, vmax, n_levels)
+            levels = np.linspace(vmin, vmax, n_levels)  # type: ignore
         else:
-            n_levels = len(levels)
-            vmin = min(levels)
-            vmax = max(levels)
+            n_levels = len(levels)  # type: ignore
+            vmin = min(levels)  # type: ignore
+            vmax = max(levels)  # type: ignore
 
         levels = np.array(levels)
 
         if isinstance(cmap, str):
             cmap = matplotlib.colormaps[cmap]
         cmap_norm = mplc.BoundaryNorm(levels, cmap.N)
         cmap_ScMappable = cm.ScalarMappable(cmap=cmap, norm=cmap_norm)
 
     if levels is None:
         levels = np.linspace(vmin, vmax, 10)
 
-    return vmin, vmax, cmap, cmap_norm, cmap_ScMappable, levels
+    return vmin, vmax, cmap, cmap_norm, cmap_ScMappable, levels  # type: ignore
 
 
-def __set_plot_limits(ax, nc) -> None:
+def __set_plot_limits(ax: Axes, nc: np.ndarray) -> None:
     """Set default plot limits
 
     Override with matplotlib ax.set_xlim, ax.set_ylim
     """
     xmin, xmax = nc[:, 0].min(), nc[:, 0].max()
     ymin, ymax = nc[:, 1].min(), nc[:, 1].max()
 
     xybuf = 6e-3 * (xmax - xmin)
     ax.set_xlim(xmin - xybuf, xmax + xybuf)
     ax.set_ylim(ymin - xybuf, ymax + xybuf)
 
 
-def __plot_mesh_only(ax, nc, element_table):
+def __plot_mesh_only(ax: Axes, nc: np.ndarray, element_table: np.ndarray) -> None:
     """plot mesh only (no data)
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     nc : array of float
@@ -320,15 +337,15 @@
     patches = _to_polygons(nc, element_table)
     fig_obj = PatchCollection(
         patches, edgecolor=MESH_COL_DARK, facecolor="none", linewidths=0.3
     )
     ax.add_collection(fig_obj)
 
 
-def __plot_outline_only(ax, boundary_polylines: BoundaryPolylines):
+def __plot_outline_only(ax: Axes, boundary_polylines: BoundaryPolylines) -> Axes:
     """plot outline only (no data)
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     boundary_polylines : BoundaryPolylines
@@ -339,15 +356,25 @@
     matplotlib.axes.Axes
         axes object
     """
     __add_outline(ax, boundary_polylines)
     return ax
 
 
-def __plot_patch(ax, nc, element_table, show_mesh, cmap, cmap_norm, z, vmin, vmax):
+def __plot_patch(
+    ax: Axes,
+    nc: np.ndarray,
+    element_table: np.ndarray,
+    show_mesh: bool,
+    cmap: Colormap,
+    cmap_norm: Normalize,
+    z: np.ndarray,
+    vmin: float,
+    vmax: float,
+) -> PatchCollection:
     """plot patch with data from z
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     nc : array of float
@@ -369,16 +396,14 @@
 
     Returns
     -------
     matplotlib.axes.Axes
         axes object
     """
 
-    from matplotlib.collections import PatchCollection
-
     patches = _to_polygons(nc, element_table)
 
     if show_mesh:
         edgecolor = MESH_COL
         linewidth = 0.4
     else:
         edgecolor = "face"
@@ -395,15 +420,21 @@
     fig_obj.set_array(z)
     fig_obj.set_clim(vmin, vmax)
     ax.add_collection(fig_obj)
 
     return fig_obj
 
 
-def __get_tris(nc, element_table, ec, z, n_refinements):
+def __get_tris(
+    nc: np.ndarray,
+    element_table: np.ndarray,
+    ec: np.ndarray,
+    z: np.ndarray,
+    n_refinements: int,
+) -> Tuple[Triangulation, np.ndarray]:
     """get triangulation object and node-centered data
 
     Parameters
     ----------
     nc : array of float
         node coordinates
     element_table : array of int
@@ -431,15 +462,22 @@
         # TODO: refinements doesn't seem to work for 3d files?
         refiner = tri.UniformTriRefiner(triang)
         triang, zn = refiner.refine_field(zn, subdiv=n_refinements)
 
     return triang, zn
 
 
-def __add_colorbar(ax, cmap_ScMappable, fig_obj, label, levels, cbar_extend) -> None:
+def __add_colorbar(
+    ax: Axes,
+    cmap_ScMappable: ScalarMappable,
+    fig_obj: Figure,
+    label: str,
+    levels: np.ndarray,
+    cbar_extend: str,
+) -> None:
     """add colorbar to axes
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     cmap_ScMappable : matplotlib.cm.ScalarMappable
@@ -461,24 +499,24 @@
     from mpl_toolkits.axes_grid1 import make_axes_locatable  # type: ignore
     import matplotlib.pyplot as plt
 
     cax = make_axes_locatable(ax).append_axes("right", size="5%", pad=0.05)
     cmap_sm = cmap_ScMappable if cmap_ScMappable else fig_obj
 
     plt.colorbar(
-        cmap_sm,
+        cmap_sm,  # type: ignore
         label=label,
         cax=cax,
         ticks=levels,
         boundaries=levels,
         extend=cbar_extend,
     )
 
 
-def __set_aspect_ratio(ax, nc, projection):
+def __set_aspect_ratio(ax: Axes, nc: np.ndarray, projection: str) -> None:
     """set aspect ratio
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     nc : array of float
@@ -494,15 +532,17 @@
     if is_geo:
         mean_lat = np.mean(nc[:, 1])
         ax.set_aspect(1.0 / np.cos(np.pi * mean_lat / 180))
     else:
         ax.set_aspect("equal")
 
 
-def __add_non_tri_mesh(ax, nc, element_table, plot_type) -> None:
+def __add_non_tri_mesh(
+    ax: Axes, nc: np.ndarray, element_table: np.ndarray, plot_type: str
+) -> None:
     """add non-triangular mesh to axes
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     nc : array of float
@@ -529,15 +569,15 @@
         edgecolor=mesh_col,
         facecolor="none",
         linewidths=mesh_linewidth,
     )
     ax.add_collection(p)
 
 
-def __add_outline(ax, boundary_polylines: BoundaryPolylines) -> None:
+def __add_outline(ax: Axes, boundary_polylines: BoundaryPolylines) -> None:
     """add outline to axes
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         axes object
     boundary_polylines: BoundaryPolylines
@@ -549,31 +589,31 @@
     """
 
     lines = boundary_polylines.exteriors + boundary_polylines.interiors
     for line in lines:
         ax.plot(*line.xy.T, color="0.4", linewidth=1.2)
 
 
-def _set_xy_label_by_projection(ax, projection):
+def _set_xy_label_by_projection(ax: Axes, projection: str) -> None:
     if (not projection) or projection == "NON-UTM":
         ax.set_xlabel("x [m]")
         ax.set_ylabel("y [m]")
     elif projection == "LONG/LAT":
         ax.set_xlabel("Longitude [degrees]")
         ax.set_ylabel("Latitude [degrees]")
     else:
         ax.set_xlabel("Easting [m]")
         ax.set_ylabel("Northing [m]")
 
 
-def __is_tri_only(element_table):
+def __is_tri_only(element_table: np.ndarray) -> bool:
     return max([len(el) for el in element_table]) == 3
 
 
-def _to_polygons(node_coordinates, element_table):
+def _to_polygons(node_coordinates: np.ndarray, element_table: np.ndarray) -> list[Any]:
     """generate matplotlib polygons from element table for plotting
 
     Returns
     -------
     list(matplotlib.patches.Polygon)
         list of polygons for plotting
     """
@@ -590,16 +630,20 @@
 
         polygon = Polygon(pcoords, closed=True)
         polygons.append(polygon)
     return polygons
 
 
 def _get_node_centered_data(
-    node_coordinates, element_table, element_coordinates, data, extrapolate=True
-):
+    node_coordinates: np.ndarray,
+    element_table: np.ndarray,
+    element_coordinates: np.ndarray,
+    data: np.ndarray,
+    extrapolate: bool = True,
+) -> np.ndarray:
     """convert cell-centered data to node-centered by pseudo-laplacian method
 
     Parameters
     ----------
     node_coordinates,
     element_table,
     element_coordinates
@@ -650,21 +694,24 @@
             ]
             node_centered_data[n] = np.sum(InvDis * data[item]) / np.sum(InvDis)
 
     return node_centered_data
 
 
 def __create_tri_only_element_table(
-    node_coordinates, element_table, element_coordinates, data
-):
+    node_coordinates: np.ndarray,
+    element_table: np.ndarray,
+    element_coordinates: np.ndarray,
+    data: np.ndarray,
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """Convert quad/tri mesh to pure tri-mesh"""
 
     if __is_tri_only(element_table):
         # already tri-only? just convert to 2d array
-        return np.stack(element_table), element_coordinates, data
+        return np.stack(element_table), element_coordinates, data  # type: ignore
 
     ec = element_coordinates.copy()
 
     elem_table = [list(element_table[i]) for i in range(len(element_table))]
     tmp_elmnt_nodes = elem_table.copy()
     for el, item in enumerate(tmp_elmnt_nodes):
         if len(item) == 4:
@@ -682,15 +729,17 @@
 
             # use same data in two new tri elements
             data = np.append(data, data[el])
 
     return np.asarray(elem_table), ec, data
 
 
-def __cbar_extend(calc_data, vmin, vmax) -> str:
+def __cbar_extend(
+    calc_data: np.ndarray | None, vmin: float | None, vmax: float | None
+) -> str:
     if calc_data is None:
         return "neither"
     extend_min = calc_data.min() < vmin if vmin is not None else False
     extend_max = calc_data.max() > vmax if vmax is not None else False
     if extend_min and extend_max:
         extend = "both"
     elif extend_min:
@@ -699,25 +748,25 @@
         extend = "max"
     else:
         extend = "neither"
     return extend
 
 
 def _plot_vertical_profile(
-    node_coordinates,
-    element_table,
-    values,
-    zn=None,
-    is_geo=False,
-    cmin=None,
-    cmax=None,
-    label="",
-    add_colorbar=True,
-    **kwargs,
-):
+    node_coordinates: np.ndarray,
+    element_table: np.ndarray,
+    values: np.ndarray,
+    zn: np.ndarray | None = None,
+    is_geo: bool = False,
+    cmin: float | None = None,
+    cmax: float | None = None,
+    label: str = "",
+    add_colorbar: bool = True,
+    **kwargs: Any,
+) -> Axes:
     """
     Plot unstructured vertical profile
 
     Parameters
     ----------
     node_coordinates: np.array
     element_table: np.array[np.array]
@@ -802,13 +851,13 @@
 
     if "title" in kwargs:
         ax.set_title(kwargs["title"])
 
     return ax
 
 
-def _Get_2DVertical_elements(element_table):
+def _Get_2DVertical_elements(element_table: np.ndarray) -> np.ndarray:
     # if (type == DfsuFileType.DfsuVerticalProfileSigmaZ) or (
     #     type == DfsuFileType.DfsuVerticalProfileSigma
     # ):
     elements = [list(element_table[i]) for i in range(len(list(element_table)))]
     return np.asarray(elements)
```

### Comparing `mikeio-2.0b0/mikeio/spatial/__init__.py` & `mikeio-2.0b1/mikeio/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/mikeio/spatial/_geometry.py` & `mikeio-2.0b1/mikeio/spatial/_geometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 
 from collections import namedtuple
-from typing import Tuple
+from typing import Any, Tuple
 
 from mikecore.Projections import MapProjection
 
 BoundingBox = namedtuple("BoundingBox", ["left", "bottom", "right", "top"])
 
 
 class _Geometry(ABC):
@@ -18,15 +18,15 @@
 
     @property
     def projection_string(self) -> str:
         """The projection string"""
         return self._projstr
 
     @property
-    def projection(self):
+    def projection(self) -> str:
         """The projection"""
         return self._projstr
 
     @property
     def is_geo(self) -> bool:
         """Are coordinates geographical (LONG/LAT)?"""
         return self._projstr == "LONG/LAT"
@@ -44,15 +44,15 @@
     @property
     @abstractmethod
     def default_dims(self) -> Tuple[str, ...]:
         pass
 
 
 class GeometryUndefined(_Geometry):
-    def __repr__(self):
+    def __repr__(self) -> str:
         return "GeometryUndefined()"
 
     @property
     def ndim(self) -> int:
         raise NotImplementedError()
 
     @property
@@ -82,40 +82,40 @@
         return f"POINT ({self.x} {self.y})"
 
     @property
     def ndim(self) -> int:
         """Geometry dimension"""
         return 0
 
-    def to_shapely(self):
+    def to_shapely(self) -> Any:
         from shapely.geometry import Point
 
         return Point(self.x, self.y)
 
 
 class GeometryPoint3D(_Geometry):
     def __init__(self, x: float, y: float, z: float, projection: str = "LONG/LAT"):
         super().__init__(projection)
 
         self.x = x
         self.y = y
         self.z = z
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"GeometryPoint3D(x={self.x}, y={self.y}, z={self.z})"
 
     @property
     def default_dims(self) -> Tuple[str, ...]:
         return ()
 
     @property
     def wkt(self) -> str:
         return f"POINT Z ({self.x} {self.y} {self.z})"
 
     @property
     def ndim(self) -> int:
         return 0
 
-    def to_shapely(self):
+    def to_shapely(self) -> Any:
         from shapely.geometry import Point
 
         return Point(self.x, self.y, self.z)
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_grid_geometry.py` & `mikeio-2.0b1/mikeio/spatial/_grid_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,19 +490,14 @@
                 raise ValueError("x0,y0 cannot be provided together with bbox")
             self._create_in_bbox(bbox, dx=dx, dy=dy, nx=nx, ny=ny)
         else:
             self._x0, self._dx, self._nx = _parse_grid_axis("x", x, x0, dx, nx)
             dy = self._dx if dy is None else dy
             self._y0, self._dy, self._ny = _parse_grid_axis("y", y, y0, dy, ny)
 
-        if self.is_local_coordinates and not (is_spectral or is_vertical):
-            self._x0 = self._x0 + self._dx / 2
-            self._y0 = self._y0 + self._dy / 2
-            self._shift_origin_on_write = False
-
         self.is_spectral = is_spectral
         self.is_vertical = is_vertical
 
         self.plot = _Grid2DPlotter(self)
 
     @property
     def default_dims(self) -> Tuple[str, ...]:
@@ -645,16 +640,21 @@
 
     @property
     def x(self) -> np.ndarray:
         """array of x coordinates (element center)"""
         if self.is_spectral and self.dx > 1:
             return self._logarithmic_f(self.nx, self._x0, self.dx)
 
-        x1 = self._x0 + self.dx * (self.nx - 1)
-        x_local = np.linspace(self._x0, x1, self.nx)
+        if self.is_local_coordinates and not (self.is_spectral or self.is_vertical):
+            x0 = self._x0 + self._dx / 2
+        else:
+            x0 = self._x0
+
+        x1 = x0 + self.dx * (self.nx - 1)
+        x_local = np.linspace(x0, x1, self.nx)
         if self._is_rotated or self.is_spectral:
             return x_local
         else:
             return x_local + self._origin[0]
 
     @staticmethod
     def _logarithmic_f(
@@ -680,16 +680,21 @@
         logdf = np.log(f0 * freq_factor) - logf0
         logf = logf0 + logdf * np.arange(n)
         return np.exp(logf)
 
     @property
     def y(self) -> np.ndarray:
         """array of y coordinates (element center)"""
-        y1 = self._y0 + self.dy * (self.ny - 1)
-        y_local = np.linspace(self._y0, y1, self.ny)
+        if self.is_local_coordinates and not (self.is_spectral or self.is_vertical):
+            y0 = self._y0 + self._dy / 2
+        else:
+            y0 = self._y0
+
+        y1 = y0 + self.dy * (self.ny - 1)
+        y_local = np.linspace(y0, y1, self.ny)
         return y_local if self._is_rotated else y_local + self._origin[1]
 
     @property
     def nx(self) -> int:
         """number of x grid points"""
         return self._nx
 
@@ -1126,18 +1131,14 @@
         self._y0, self._dy, self._ny = _parse_grid_axis("y", y, y0, dy, ny)
         self._z0, self._dz, self._nz = _parse_grid_axis("z", z, z0, dz, nz)
 
         self._projstr = projection  # TODO handle other types than string
         self._origin = origin
         self._orientation = orientation
 
-        if self.is_local_coordinates:
-            self._x0 = self._x0 + self._dx / 2
-            self._y0 = self._y0 + self._dy / 2
-
     @property
     def default_dims(self) -> Tuple[str, ...]:
         return ("z", "y", "x")
 
     @property
     def ndim(self) -> int:
         return 3
@@ -1145,16 +1146,18 @@
     @property
     def _is_rotated(self) -> Any:
         return np.abs(self._orientation) > 1e-5
 
     @property
     def x(self) -> np.ndarray:
         """array of x-axis coordinates (element center)"""
-        x1 = self._x0 + self.dx * (self.nx - 1)
-        x_local = np.linspace(self._x0, x1, self.nx)
+        x0 = self._x0 + self._dx / 2 if self.is_local_coordinates else self._x0
+
+        x1 = x0 + self.dx * (self.nx - 1)
+        x_local = np.linspace(x0, x1, self.nx)
         return x_local if self._is_rotated else x_local + self.origin[0]
 
     @property
     def dx(self) -> float:
         """x-axis grid spacing"""
         return self._dx
 
@@ -1162,16 +1165,17 @@
     def nx(self) -> int:
         """number of x grid points"""
         return self._nx
 
     @property
     def y(self) -> np.ndarray:
         """array of y-axis coordinates (element center)"""
-        y1 = self._y0 + self.dy * (self.ny - 1)
-        y_local = np.linspace(self._y0, y1, self.ny)
+        y0 = self._y0 + self._dy / 2 if self.is_local_coordinates else self._y0
+        y1 = y0 + self.dy * (self.ny - 1)
+        y_local = np.linspace(y0, y1, self.ny)
         return y_local if self._is_rotated else y_local + self.origin[1]
 
     @property
     def dy(self) -> float:
         """y-axis grid spacing"""
         return self._dy
 
@@ -1365,15 +1369,19 @@
         d = np.diff(g.z[layers])
         if len(d) > 0:
             if np.any(d < 1) or not np.allclose(d, d[0]):
                 warnings.warn("Extracting non-equidistant layers! Cannot use Grid3D.")
                 return GeometryUndefined()
 
         geometry = Grid3D(
-            x=g.x,
-            y=g.y,
+            x0=g._x0,
+            y0=g._y0,
+            nx=g._nx,
+            dx=g._dx,
+            ny=g._ny,
+            dy=g._dy,
             z=g.z[layers],
             origin=g._origin,
             projection=g.projection,
             orientation=g.orientation,
         )
         return geometry
```

### Comparing `mikeio-2.0b0/mikeio/spatial/_utils.py` & `mikeio-2.0b1/mikeio/spatial/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
+from __future__ import annotations
+
+from typing import Tuple
+
 import numpy as np
 
 from ._geometry import BoundingBox
 
 
 def xy_to_bbox(xy: np.ndarray, buffer: float = 0.0) -> BoundingBox:
     """return bounding box for list of coordinates"""
     left = xy[:, 0].min() - buffer
     bottom = xy[:, 1].min() - buffer
     right = xy[:, 0].max() + buffer
     top = xy[:, 1].max() + buffer
     return BoundingBox(left, bottom, right, top)
 
 
-def dist_in_meters(coords, pt, is_geo=False):
+def dist_in_meters(
+    coords: np.ndarray, pt: Tuple[float, float], is_geo: bool = False
+) -> np.ndarray:
     """get distance between array of coordinates and point
 
     Parameters
     ----------
     coords : n-by-2 array
         x, y coordinates
     pt : [float, float]
@@ -34,32 +40,35 @@
     ye = coords[:, 1]
     xp = pt[0]
     yp = pt[1]
     if is_geo:
         d = _get_dist_geo(xe, ye, xp, yp)
     else:
         d = np.sqrt(np.square(xe - xp) + np.square(ye - yp))
-    return d
+    return d  # type: ignore
 
 
-def _get_dist_geo(lon, lat, lon1, lat1):
+def _get_dist_geo(lon: float, lat: float, lon1: float, lat1: float) -> float:
     # assuming input in degrees!
     R = 6371e3  # Earth radius in metres
     dlon = np.deg2rad(lon1 - lon)
     dlon[dlon > np.pi] = dlon[dlon > np.pi] - 2 * np.pi
     dlon[dlon < -np.pi] = dlon[dlon < -np.pi] + 2 * np.pi
     dlat = np.deg2rad(lat1 - lat)
     x = dlon * np.cos(np.deg2rad((lat + lat1) / 2))
     y = dlat
     d = R * np.sqrt(np.square(x) + np.square(y))
-    return d
+    return d  # type: ignore
 
 
-def _relative_cumulative_distance(coords, reference=None, is_geo=False):
+def _relative_cumulative_distance(
+    coords: np.ndarray, reference: np.ndarray | None = None, is_geo: bool = False
+) -> np.ndarray:
     """Calculate the cumulative relative distance along a path"""
     coords = np.atleast_2d(coords)
     d = np.zeros_like(coords[:, 0])
     if reference is not None:
-        d[0] = dist_in_meters(coords[0, 0:2], reference[0:2], is_geo)[0]
+        pt = (reference[0], reference[1])
+        d[0] = dist_in_meters(coords[0, 0:2], pt=pt, is_geo=is_geo)[0]
     for j in range(1, len(d)):
         d[j] = d[j - 1] + dist_in_meters(coords[j, 0:2], coords[j - 1, 0:2], is_geo)[0]
-    return d
+    return d  # type: ignore
```

### Comparing `mikeio-2.0b0/mikeio/spatial/crs.py` & `mikeio-2.0b1/mikeio/spatial/crs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import warnings
+from typing import TYPE_CHECKING
 
 from mikecore.Projections import Cartography, MapProjection
 
+if TYPE_CHECKING:
+    from pyproj import crs
 # import pyproj
 
 
 class CRSConversionWarning(Warning):
     """Used when an ad hoc conversion is performed."""
 
     pass
@@ -68,15 +71,15 @@
     def is_geographical(self) -> bool:
         return MapProjection.IsGeographical(self.projection_string)
 
     @property
     def is_projected(self) -> bool:
         return not self.is_geographical
 
-    def to_pyproj(self):
+    def to_pyproj(self) -> "crs.CRS":
         """
         Convert projection to pyptoj.CRS object.
 
         Returns
         -------
         pyproj.CRS
 
@@ -89,15 +92,15 @@
                 category=CRSConversionWarning,
             )
             return pyproj.CRS.from_epsg(4326)
         else:
             return pyproj.CRS.from_string(self.projection_string)
 
     @classmethod
-    def from_pyproj(cls, pyproj_crs):
+    def from_pyproj(cls, pyproj_crs: "crs.CRS") -> "CRS":
         """
         Create CRS object from pyproj.CRS object.
 
         Parameters
         ----------
         pyproj_crs : pyproj.CRS
             pyproj.CRS object.
@@ -107,21 +110,21 @@
         CRS
             CRS instance.
 
         """
 
         return cls(projection_string=pyproj_crs.to_wkt(version="WKT1_ESRI"))
 
-    def to_epsg(self, min_confidence: float = 70.0) -> int:
+    def to_epsg(self, min_confidence: int = 70) -> int:
         """
         Convert projection to pyptoj.CRS object.
 
         Parameters
         ----------
-        min_confidence : float, optional
+        min_confidence : integer, optional
             A value between 0-100 where 100 is the most confident. Default is 70.
             See 'pyproj.CRS.to_epsg' for more details.
 
         Returns
         -------
         int
             EPSG code.
@@ -145,15 +148,15 @@
         else:
             raise RuntimeError(
                 f"pyproj.to_epsg returned '{type(epsg_code).__name__}', "
                 f"expected None or int"
             )
 
     @classmethod
-    def from_epsg(cls, epsg: int):
+    def from_epsg(cls, epsg: int) -> "CRS":
         """
         Create CRS object from EPSG code.
 
         Parameters
         ----------
         epsg : int
             EPSG code.
```

### Comparing `mikeio-2.0b0/README.md` & `mikeio-2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `mikeio-2.0b0/pyproject.toml` & `mikeio-2.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 exclude = ["notebooks", "tests", "images"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name="mikeio"
-version="2.0.b0"
+version="2.0.b1"
 dependencies = [
     "mikecore>=0.2.1",
     "numpy>=1.22.0",
     "pandas>=1.3",
     "matplotlib>=3.6.0",
     "scipy>=1.0",
     "PyYAML",
```

### Comparing `mikeio-2.0b0/PKG-INFO` & `mikeio-2.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mikeio
-Version: 2.0b0
+Version: 2.0b1
 Summary: A package that uses the DHI dfs libraries to create, write and read dfs and mesh files.
 Project-URL: Homepage, https://github.com/DHI/mikeio
 Project-URL: Bug Tracker, https://github.com/DHI/mikeio/issues
 Author-email: Henrik Andersson <jan@dhigroup.com>, Jesper Sandvig Mariegaard <jem@dhigroup.com>
 License-Expression: BSD-3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

