# Comparing `tmp/massivechem-4.1.tar.gz` & `tmp/massivechem-4.3.tar.gz`

## Comparing `massivechem-4.1.tar` & `massivechem-4.3.tar`

### file list

```diff
@@ -1,87 +1,52 @@
--rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-4.1/IMG_2856.jpg
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 massivechem-4.1/MASSIVEChem.yml
--rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-4.1/Spectrum_output.png
--rw-r--r--   0        0        0    79006 2020-02-02 00:00:00.000000 massivechem-4.1/bokeh_with_plotly.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/molecule_image.png
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-4.1/project_final.yml
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/modules.xml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/vcs.xml
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/workspace.xml
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/input/input.html
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/input/input.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 massivechem-4.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0    35964 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/COPIED_VERSION.py
--rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/base64_encoded_images.pkl
--rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/big_func.html
--rw-r--r--   0        0        0    19780 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/big_func.py
--rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/conversion.py
--rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/copy_file.py
--rw-r--r--   0        0        0     6815 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/encoded_image.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functional_group_display.py
--rw-r--r--   0        0        0     4629 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functional_group_finder.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    38793 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/gpt4otest.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/last.py
--rw-r--r--   0        0        0    13760 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/mol_web_show_copy.html
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0    14962 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test_image.html
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/test_image.py
--rw-r--r--   0        0        0  3897887 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/mol_3d.html
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/mol_web_show_copy.py
--rw-r--r--   0        0        0    15657 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/smiles_to_3D_plot.html
--rw-r--r--   0        0        0    30227 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    24297 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/spectrum_copy.html
--rw-r--r--   0        0        0    26678 2020-02-02 00:00:00.000000 massivechem-4.1/THOMAS_IS_BEST/igor_chem/spectrum_copy.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/random_tests.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 massivechem-4.1/Thomas/tests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/checklist.txt
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/project_report.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/notebooks/test.ipynb
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/SMILEs_interpreter.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/all_in_one.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/atom_present_list.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/calculate_unsaturation.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/delta_function_plotter.py
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/double_plot.py
--rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/functional_group_display.py
--rw-r--r--   0        0        0     6769 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/functional_group_finder.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/ionisation_method.py
--rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/main_function.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/mol_web_show.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/molecule_list_generator.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/peak_merger.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/peak_sorter.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/smiles_to_3D_plot.py
--rw-r--r--   0        0        0    64806 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/spectrum.html
--rw-r--r--   0        0        0    27288 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/spectrum.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 massivechem-4.1/scripts/sulphur_nitrogen_adder.py
--rw-r--r--   0        0        0    65603 2020-02-02 00:00:00.000000 massivechem-4.1/src/MASSiveChem/MASSiveChem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.1/src/MASSiveChem/__init__.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/SMILEs_interpreter_tests.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/all_in_one_tests.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/atom_present_list_tests.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/delta_function_plotter_tests.py
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/double_plot_tests.py
--rw-r--r--   0        0        0     6149 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/functional_group_display_tests.py
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/functional_group_finder_tests.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/ionisation_method_tests.py
--rw-r--r--   0        0        0    12336 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/main_function_tests.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/mol_web_show_tests.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/molecule_list_generator_tests.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/peak_merger_tests.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/smiles_to_3D_plot_tests.py
--rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/spectrum_tests.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/sulphur_nitrogen_adder_tests.py
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 massivechem-4.1/tests/tests/unsaturation_tests.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 massivechem-4.1/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 massivechem-4.1/LICENSE.txt
--rw-r--r--   0        0        0     6627 2020-02-02 00:00:00.000000 massivechem-4.1/README.md
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 massivechem-4.1/pyproject.toml
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 massivechem-4.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.3/Focused_spectrum.png
+-rw-r--r--   0        0        0   219083 2020-02-02 00:00:00.000000 massivechem-4.3/Logo.jpg
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 massivechem-4.3/MASSIVEChem.yml
+-rw-r--r--   0        0        0    26315 2020-02-02 00:00:00.000000 massivechem-4.3/Schematic_mass_spectrum.png
+-rw-r--r--   0        0        0   196052 2020-02-02 00:00:00.000000 massivechem-4.3/Spectrum_output.png
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 massivechem-4.3/project_final.yml
+-rw-r--r--   0        0        0   103430 2020-02-02 00:00:00.000000 massivechem-4.3/notebooks/backup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.3/notebooks/checklist.txt
+-rw-r--r--   0        0        0   130996 2020-02-02 00:00:00.000000 massivechem-4.3/notebooks/project_report.ipynb
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/SMILEs_interpreter.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/all_in_one.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/calculate_unsaturation.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/delta_function_plotter.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/double_plot.py
+-rw-r--r--   0        0        0     4413 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/functional_group_display.py
+-rw-r--r--   0        0        0     8956 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/functional_group_finder.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/ionisation_method.py
+-rw-r--r--   0        0        0    12521 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/main_function.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/mol_web_show.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/molecule_list_generator.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/peak_merger.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/peak_sorter.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    29627 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/spectrum.py
+-rw-r--r--   0        0        0    30019 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/spectrum_3D.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 massivechem-4.3/scripts/sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0   103430 2020-02-02 00:00:00.000000 massivechem-4.3/src/MASSiveChem/MASSiveChem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.3/src/MASSiveChem/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 massivechem-4.3/test/__init__.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_SMILEs_interpreter.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_calculate_unsaturation.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_delta_function_plotter.py
+-rw-r--r--   0        0        0     4552 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_double_plot.py
+-rw-r--r--   0        0        0     7670 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_functional_group_display.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_functional_group_finder.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_ionisation_method.py
+-rw-r--r--   0        0        0    16540 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_main_function.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_mol_web_show.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_molecule_list_generator.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_peak_merger.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_peak_sorter.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_smiles_to_3D_plot.py
+-rw-r--r--   0        0        0    27750 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_spectrum.py
+-rw-r--r--   0        0        0    31039 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_spectrum_3D.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_sulphur_nitrogen_adder.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 massivechem-4.3/test/test_sulphur_nitrogen_finder.py
+-rw-r--r--   0        0        0     5179 2020-02-02 00:00:00.000000 massivechem-4.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 massivechem-4.3/LICENSE.txt
+-rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 massivechem-4.3/README.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 massivechem-4.3/pyproject.toml
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 massivechem-4.3/PKG-INFO
```

### Comparing `massivechem-4.1/IMG_2856.jpg` & `massivechem-4.3/Logo.jpg`

 * *Files identical despite different names*

### Comparing `massivechem-4.1/MASSIVEChem.yml` & `massivechem-4.3/MASSIVEChem.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,48 @@
-name: project_final
+name: MASSIVEChem
 channels:
   - defaults
 dependencies:
   - bzip2=1.0.8=h2bbff1b_6
   - ca-certificates=2024.3.11=haa95532_0
   - libffi=3.4.4=hd77b12b_1
-  - openssl=3.0.13=h2bbff1b_1
+  - openssl=3.0.13=h2bbff1b_2
   - pip=24.0=py310haa95532_0
   - python=3.10.12=he1021f5_0
   - setuptools=69.5.1=py310haa95532_0
   - sqlite=3.45.3=h2bbff1b_0
   - tk=8.6.14=h0416ee5_0
-  - vc=14.2=h21ff451_1
-  - vs2015_runtime=14.27.29016=h5e58377_2
+  - vc=14.2=h2eaa2aa_1
+  - vs2015_runtime=14.29.30133=h43f2093_3
   - wheel=0.43.0=py310haa95532_0
   - xz=5.4.6=h8cc25b3_1
   - zlib=1.2.13=h8cc25b3_1
   - pip:
       - bleach==6.1.0
       - bokeh==3.4.1
       - certifi==2024.2.2
       - charset-normalizer==3.3.2
       - colorama==0.4.6
       - contourpy==1.2.1
-      - cycler==0.12.1
-      - filelock==3.14.0
-      - fonttools==4.51.0
       - idna==3.7
       - jinja2==3.1.4
-      - kiwisolver==1.4.5
       - linkify-it-py==2.0.3
       - markdown==3.6
       - markdown-it-py==3.0.0
       - markupsafe==2.1.5
-      - matplotlib==3.8.4
       - mdit-py-plugins==0.4.1
       - mdurl==0.1.2
       - networkx==3.3
       - numpy==1.26.4
       - packaging==24.0
       - pandas==2.2.2
-      - panel==1.4.2
+      - panel==1.4.3
       - param==2.1.0
       - pillow==10.3.0
       - plotly==5.22.0
-      - pyparsing==3.1.2
-      - pyproject-api==1.6.1
       - python-dateutil==2.9.0.post0
       - pytz==2024.1
       - pyviz-comms==3.0.2
       - pyyaml==6.0.1
       - rdkit==2023.9.6
       - requests==2.32.2
       - six==1.16.0
@@ -59,8 +52,8 @@
       - typing-extensions==4.11.0
       - tzdata==2024.1
       - uc-micro-py==1.0.3
       - urllib3==2.2.1
       - webencodings==0.5.1
       - xyz2graph==2.0.0
       - xyzservices==2024.4.0
-prefix: C:\Users\maintenant Pret\anaconda3\envs\project_final
+
```

### Comparing `massivechem-4.1/Spectrum_output.png` & `massivechem-4.3/Spectrum_output.png`

 * *Files identical despite different names*

### Comparing `massivechem-4.1/project_final.yml` & `massivechem-4.3/project_final.yml`

 * *Files identical despite different names*

### Comparing `massivechem-4.1/THOMAS_IS_BEST/test.py` & `massivechem-4.3/scripts/functional_group_finder.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,22 @@
     
     Input: molecule under SMILEs representation
     
     Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError("Enter a non-empty string as argument")
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
+    if not mol_in:
+        raise ValueError('Incorrect SMILEs input')
+
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
         'Alcohol': 'C[Oh1+0]',
         'Aldehyde': 'C[Ch1]=O',
         'Ketone': 'CC(=O)C',
         'Carboxylic Acid': 'CC(=O)[Oh1]',
@@ -66,76 +71,107 @@
     for name, smarts in functional_groups_smarts.items():
         if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
                 functional_groups_contained.append(name)
 
     # exceptions for conflicts during the iteration of functional groups
     for functional_group in functional_groups_contained:
-        if functional_group == 'Carboxylic Acid':
+        if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
-        elif 'Amine' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amine')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
-
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
+    
+    
     return functional_groups_contained
 
-print(functional_group_finder('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'))
```

### Comparing `massivechem-4.1/THOMAS_IS_BEST/igor_chem/mol_web_show_copy.py` & `massivechem-4.3/scripts/mol_web_show.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,37 +5,34 @@
 import base64
 
 from bokeh.plotting import show
 from bokeh.io import show
 from bokeh.models import Div
 
 
-def mol_web_show(mol_smi, show_Hs=False, show_3D = False):
+def mol_web_show(mol_smi):
 
     #---------------------------------------------------------------------------------------------#
     '''
-    mol_web_show(mol_smi, show_Hs=False, show_3D = False)
+    mol_web_show(mol_smi)
     
-    Input: SMILEs of a molecule. Also specify if want the function to show the hydrogens explicitely or the 3D
+    Input: SMILEs of a molecule
     
     Output: image of the molecule as a bokeh plot
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError('Incorrect SMILEs input')
+    
     # Generate the image from the molecule
     mol = Chem.MolFromSmiles(mol_smi)
 
-    # Show the molecule in 3D if specified
-    if show_3D:
-        mol = Chem.AddHs(mol)
-        AllChem.EmbedMolecule(mol)
-    
-    # Adds the hydrogens to the molecule if specified
-    if show_Hs:
-        mol = Chem.AddHs(mol)
+    if mol is None:
+        raise ValueError('Incorrect SMILEs input')
 
     #Draws the image
     image = Draw.MolToImage(mol)
 
     #stocks the image in a base64 format
     buffered = BytesIO()
     image.save(buffered, format="PNG")
@@ -43,10 +40,7 @@
     image_url = f"data:image/png;base64,{image_base64}"
 
     # Create a Div element to display the image
     img_div = Div(text=f'<img src="{image_url}" style="width:350px;height:350px;">')
    
     return img_div
     
-input_mol = input('MOL:  ')
-
-show(mol_web_show(input_mol,False,True))
```

### Comparing `massivechem-4.1/THOMAS_IS_BEST/igor_chem/smiles_to_3D_plot.py` & `massivechem-4.3/test/test_spectrum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,124 +1,112 @@
 from rdkit import Chem
-from rdkit.Chem import AllChem
-import tempfile
-from xyz2graph import MolGraph, to_plotly_figure
-import panel as pn
-
-def smiles_to_3D_plot(smiles):
-
-     #---------------------------------------------------------------------------------------------#
-    '''
-    smiles_to_3D_plot(smiles)
-    
-    Input: molecule is a SMILEs format
-
-    Output: panel graph of the molecule in 3D and interactive
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    # Generate 3D coordinates from SMILES string
-    mol = Chem.MolFromSmiles(smiles)
-    mol = Chem.AddHs(mol)  # Add hydrogens for better geometry optimization
-    AllChem.EmbedMolecule(mol, randomSeed=42)  # Embed the molecule in 3D space
-    AllChem.MMFFOptimizeMolecule(mol)  # Optimize the geometry using MMFF94 force field
-
-    # Create a temporary file to store the 
-    with tempfile.NamedTemporaryFile(delete=False) as tmp:
-        tmp.write(f"{mol.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
-        for atom in mol.GetAtoms():
-            pos = mol.GetConformer().GetAtomPosition(atom.GetIdx())
-            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
-        tmp_path = tmp.name
-
-    # Create the MolGraph object
-    mg = MolGraph()
-    
-    # Read the data from the temporary file
-    mg.read_xyz(tmp_path)
-
-    # Create the Plotly figure object
-    fig = to_plotly_figure(mg)
-
-    plotly_pane = pn.pane.Plotly(fig)
-    
-    return plotly_pane
-
-# Example usage
-input_mol = input('MOL:  ')
-
-
-
-"""bokeh_pane = pn.pane.Bokeh(bokeh)
-
-layout = pn.Row(bokeh_pane,plotly_pane)
-
-layout.show()"""
-
-
-from rdkit import Chem
 from rdkit.Chem import Draw, AllChem
 
 from bokeh.plotting import figure, show, row
 from bokeh.models.tickers import FixedTicker
 from bokeh.layouts import row, column
 from bokeh.io import show
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
 
 import base64
 from io import BytesIO
 
-
-def spectrum(mol_smi, imprecision_True_False, apparatus_resolution,search_directory='.'):
-
-    C, N, HX, halogens_hydrogen = 0, 0, 0, ['F', 'Cl', 'Br', 'I', 'At', 'H']
-
-    mol = Chem.AddHs(Chem.MolFromSmiles(mol_smi))
-
-    for atom in mol.GetAtoms():
-        if atom.GetSymbol() == 'C':
-            C += 1
-        elif atom.GetSymbol() == 'N':
-            N += 1
-        elif atom.GetSymbol() in halogens_hydrogen:
-            HX += 1
-
-    unsaturation = C + 1 + (N - HX) / 2
-
-    nbr_atoms = mol.GetNumAtoms()
-
-    mol, list_atoms,list_atoms = Chem.MolFromSmiles(mol_smi),[],[]
-    for atom in mol.GetAtoms():
-        list_atoms.append(atom.GetSymbol())
-    for atom in mol.GetAtoms():
-        element = (f'{atom.GetSymbol()} : {list_atoms.count(atom.GetSymbol())}')   
-        if element not in list_atoms:
-            list_atoms.append(element)
+def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
-    mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057, 59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 91.90504, 90.90565, 89.9047, 95.90827]
-    abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003, 0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031, 0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097, 0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 0.027999999999999997]
-    isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Та', 'Та', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
+    mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
+            136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
+            12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
+            113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
+            52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
+            159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
+            56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
+            75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 
+            177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 
+            114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 
+            81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 
+            94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 
+            141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057,
+            59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 
+            185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 
+            104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 
+            84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 
+            35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 
+            81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 
+            143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 
+            87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 
+            121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 
+            202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 
+            171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 
+            91.90504, 90.90565, 89.9047, 95.90827]
+    
+
+    abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 
+                0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 
+                0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 
+                0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 
+                0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 
+                0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 
+                0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 
+                0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 
+                0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 
+                1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 
+                0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 
+                0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 
+                0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 
+                0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003,
+                0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 
+                0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 
+                0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 
+                0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 
+                0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 
+                0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 
+                0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031,
+                0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097,
+                0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 
+                0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 
+                1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 
+                0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 
+                0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 
+                0.027999999999999997]
+    
+
+    isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 
+                'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 
+                'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 
+                'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 
+                'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 
+                'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 
+                'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 
+                'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 
+                'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
+                'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
+                'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
+                'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
+                'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
+                'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
+    if not mol_smi:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
 
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     if mol_without_Hs is None:
-        print('')
-        print("Invalid SMILEs input.")
-        print('Please try again with a different SMILEs.')
-        exit()
-
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    
     mol = Chem.AddHs(mol_without_Hs)
 
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
-
+    
+    if not list_atoms:
+        return None
+    
     #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
 
     if 'H' in list_atoms:
 
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
 
@@ -262,20 +250,20 @@
     x_in = x_out
     y_in = y_out
     maximum = max(y_in)
 
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)  
-        print('N')
+        
     
     if has_S:
         x_in.append(x_in[1]-0.004)  
         y_in.append(0.008*count_S*maximum)
-        print('S')
+        
 
     x_out, y_out = [],[]
 
     while len(x_in)>0:
         min_x = min(x_in)
         index_min = x_in.index(min_x)
         x_out.append(min_x)
@@ -377,55 +365,22 @@
 
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
-        'Alcohol': 'C[Oh1+0]',
-        'Aldehyde': 'C[Ch1]=O',
-        'Ketone': 'CC(=O)C',
-        'Carboxylic Acid': 'CC(=O)[Oh1]',
-        'Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*',
-        'Amide': 'C(=O)N',
-        'Amine': '[C][N]',
-        'Nitrile': 'C#N',
-        'Chloride': 'Cl',
-        'Bromide': 'Br',
-        'Fluoride': 'F',
-        'Iodide': 'I',
-        'Alkene': 'C=C',
-        'Alkyne': 'C#C',
-        'Imine': 'C=N*',
-        'Amino acid': '[Nh2][Ch1*]C(=O)O',
-        'Proline': '[Nh1][Ch1*]C(=O)O',
-        'Thiol': '[Sh1]',
-        'Sulfide': '*[Sh0]*',
-        'Acyl Chloride': 'CC(=O)Cl',
-        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
-        'Nitro': 'C[N+](=O)[O-]',
-        'Enamine': 'C=C[Nh0]',
-        'Enamine2': 'C=C[Nh1]',
-        'Enamine3': 'C=C[Nh2]',
-        'Imide': 'C(=O)NC(=O)*',
-        'Azide': 'CNNN',
-        'Enol': 'C=C([Oh1])C',
-        'Hemiacetal': 'CC(O)(O)C',
-        'Carbonate': '[Oh0]C(=O)[Oh0]',
-        'Carbonate2': '[Oh1]C(=O)[Oh1]',
-        'Disulfide': 'CSSC',
-        'Sulfoxide': 'CS(=O)C',
-        'Sulfone': '*[So2](=O)(=O)*',
-        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
-        'Thioester': 'C(=O)S*',
-        'Phosphine': '*[Po0](*)*',
-        'Phosphate': '*OP(=O)(O)O',
-        'Benzene': 'c1ccccc1',
-        'Peroxide':'C[Oh0][Oh0]C'
+        'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': '*C(=O)[Oh1]','Ester': 'CC(=O)[Oh0]',
+        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
+        'Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O','Proline': '[Nh1][Ch1*]C(=O)O',
+        'Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*','Nitro': 'C[N+](=O)[O-]',
+        'Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*','Azide': 'CNNN','Enol': 'C=C([Oh1])C',
+        'Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]','Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C',
+        'Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*','Phosphine': '*[Po0](*)*','Phosphate': '*OP(=O)(O)O',
+        'Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
     }
 
     # check that the substructure from functional_groups_smarts are contained in mol_smi
 
     for name, smarts in functional_groups_smarts.items():
         if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
@@ -567,70 +522,48 @@
     ]
     num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
-    last = row(img_div, func_group_table)
+    last = column(img_div, func_group_table)
     final = row(double_graph, last)
+    return final
 
-    return last, double_graph
-
-
-
-
-"""bokeh_pane = pn.pane.Bokeh(spectrum(input_mol, True, 0.01))
-
-layout = pn.Column(bokeh_pane,smiles_to_3D_plot(input_mol))"""
-
-
-
-def smiles_to_3D_plot2(mol_smi,last,double_graph):
-
-     #---------------------------------------------------------------------------------------------#
-    '''
-    smiles_to_3D_plot(smiles)
-    
-    Input: molecule is a SMILEs format
-
-    Output: panel graph of the molecule in 3D and interactive
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    # Generate 3D coordinates from SMILES string
-    mol2 = Chem.MolFromSmiles(mol_smi)
-    mol2 = Chem.AddHs(mol2)  # Add hydrogens for better geometry optimization
-    AllChem.EmbedMolecule(mol2, randomSeed=42)  # Embed the molecule in 3D space
-    AllChem.MMFFOptimizeMolecule(mol2)  # Optimize the geometry using MMFF94 force field
 
-    # Create a temporary file to store the 
-    with tempfile.NamedTemporaryFile(delete=False) as tmp:
-        tmp.write(f"{mol2.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
-        for atom in mol2.GetAtoms():
-            pos = mol2.GetConformer().GetAtomPosition(atom.GetIdx())
-            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
-        tmp_path = tmp.name
+import unittest
 
-    # Create the MolGraph object
-    mg = MolGraph()
+class TestSpectrum3D(unittest.TestCase):
     
-    # Read the data from the temporary file
-    mg.read_xyz(tmp_path)
-
-    # Create the Plotly figure object
-    fig = to_plotly_figure(mg)
+    def setUp(self):
+        self.apparatus_resolution = 0.01
 
-    plotly_pane = pn.pane.Plotly(fig)
+    def test_butane_False(self):
+        mol_smi = "CCCC"
+        imprecision_True_False = False
+        result = spectrum(mol_smi, imprecision_True_False, self.apparatus_resolution)
+        self.assertIsNotNone(result)
+    
+    def test_butane_True(self):
+        mol_smi = "CCCC"
+        imprecision_True_False = True
+        result = spectrum(mol_smi, imprecision_True_False, self.apparatus_resolution)
+        self.assertIsNotNone(result)
 
-    p1_pane = pn.pane.Bokeh(last)
-    p2_pane = pn.pane.Bokeh(double_graph)
-
-    layout12 = pn.Column( plotly_pane, p1_pane)
-    final = pn.Row(p2_pane, layout12)
+    def test_empty_input(self):
+        
+        with self.assertRaises(ValueError):
+            imprecision_True_False= False
+            spectrum("",imprecision_True_False, self.apparatus_resolution)
 
-    return final
+    def test_invalid_input(self):
+        
+        with self.assertRaises(ValueError):
+            imprecision_True_False = False
+            spectrum("invalid_smiles",imprecision_True_False, self.apparatus_resolution)  
+        
 
-p1, p2 = spectrum(input_mol, True, 0.01)
+if __name__ == '__main__':
+    unittest.main()
 
 
-smiles_to_3D_plot2(input_mol, p1, p2).show()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `massivechem-4.1/THOMAS_IS_BEST/igor_chem/spectrum_copy.py` & `massivechem-4.3/scripts/spectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,139 @@
 from rdkit import Chem
-from rdkit.Chem import Draw, AllChem
+from rdkit.Chem import Draw
 
 from bokeh.plotting import figure, show, row
 from bokeh.models.tickers import FixedTicker
 from bokeh.layouts import row, column
 from bokeh.io import show
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
 
 import base64
 from io import BytesIO
 
 
+def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
 
+    #tests for wether the input is valid
+    if mol_smi is None:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a boolean value')
+    if apparatus_resolution < 0:
+        raise ValueError('Enter a positive value')
+    if type(apparatus_resolution) != float:
+        raise ValueError('Enter an integer value')
 
 
+    #lists of the data to facilitise the pip-installability of the package
 
+    mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
+            136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
+            12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
+            113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
+            52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
+            159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
+            56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
+            75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 
+            177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 
+            114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 
+            81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 
+            94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 
+            141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057,
+            59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 
+            185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 
+            104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 
+            84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 
+            35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 
+            81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 
+            143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 
+            87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 
+            121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 
+            202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 
+            171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 
+            91.90504, 90.90565, 89.9047, 95.90827]
+    
 
+    abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 
+                0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 
+                0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 
+                0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 
+                0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 
+                0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 
+                0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 
+                0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 
+                0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 
+                1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 
+                0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 
+                0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 
+                0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 
+                0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003,
+                0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 
+                0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 
+                0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 
+                0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 
+                0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 
+                0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 
+                0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031,
+                0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097,
+                0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 
+                0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 
+                1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 
+                0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 
+                0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 
+                0.027999999999999997]
+    
 
-
-def spectrum(mol_smi, imprecision_True_False, apparatus_resolution,search_directory='.'):
-
-    C, N, HX, halogens_hydrogen = 0, 0, 0, ['F', 'Cl', 'Br', 'I', 'At', 'H']
-
-    mol = Chem.AddHs(Chem.MolFromSmiles(mol_smi))
-
-    for atom in mol.GetAtoms():
-        if atom.GetSymbol() == 'C':
-            C += 1
-        elif atom.GetSymbol() == 'N':
-            N += 1
-        elif atom.GetSymbol() in halogens_hydrogen:
-            HX += 1
-
-    unsaturation = C + 1 + (N - HX) / 2
-
-    nbr_atoms = mol.GetNumAtoms()
-
-    mol, list_atoms,list_atoms = Chem.MolFromSmiles(mol_smi),[],[]
-    for atom in mol.GetAtoms():
-        list_atoms.append(atom.GetSymbol())
-    for atom in mol.GetAtoms():
-        element = (f'{atom.GetSymbol()} : {list_atoms.count(atom.GetSymbol())}')   
-        if element not in list_atoms:
-            list_atoms.append(element)
-
-    #lists of the data to facilitise the pip-installability of the package
-
-    mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057, 59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 91.90504, 90.90565, 89.9047, 95.90827]
-    abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003, 0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031, 0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097, 0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 0.027999999999999997]
-    isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Та', 'Та', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
+    isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 
+                'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 
+                'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 
+                'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 
+                'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 
+                'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 
+                'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 
+                'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 
+                'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
+                'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
+                'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
+                'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
+                'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
+                'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
+    
 
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
-    if mol_without_Hs is None:
-        print('')
-        print("Invalid SMILEs input.")
-        print('Please try again with a different SMILEs.')
-        exit()
 
+    
     mol = Chem.AddHs(mol_without_Hs)
 
+    '''molecule list generator'''
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
+    print(list_atoms)
 
     #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
 
+    '''Ionisation method'''
     if 'H' in list_atoms:
 
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
-
+    print(list_atoms)
     render_imprecise_list = imprecision_True_False 
     #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
 
-    #check for sulphur and nitrogen
-
+    
     has_N = False
     count_N = 0
     has_S = False
     count_S = 0
+
+    '''sulphur_nitrogen_finder function'''
     if 'N' in list_atoms and list_atoms.count('N')%2 == 1:
         has_N = True
         count_N = list_atoms.count('N')
         
     if 'S' in list_atoms and list_atoms.count('S')%2 == 1:
         has_S = True
         count_S = list_atoms.count('S')
@@ -92,14 +141,15 @@
 
 
     list_output = []
     mass_copy = mass.copy()
     abundance_copy = abundance.copy()
     isotopes_copy = isotopes.copy()
 
+    '''main function'''
     for i in range (isotopes.count(list_atoms[0])):
         
         index = isotopes.index(list_atoms[0])
         list_output.append([mass_copy[index],abundance_copy[index]])
         mass_copy.pop(index)
         abundance_copy.pop(index)
         isotopes_copy.pop(index)
@@ -128,18 +178,18 @@
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
-                #removes any molecule who's probability is below 0.0001
+                #removes any molecule who's probability is below 0.00001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
@@ -176,26 +226,28 @@
 
 
     
     x_in, y_in = x_axis_final, y_axis_final
     
     x_out, y_out = [],[]
 
+    '''list_sorter function'''
     while len(x_in)>0:
         min_x = min(x_in)
         index_min = x_in.index(min_x)
         x_out.append(min_x)
         y_out.append(y_in[index_min])
         x_in.pop(index_min)
         y_in.pop(index_min)
 
 
 
     x_in, y_in = x_out, y_out 
-#resolution
+    
+    '''peak_merger function'''
     x_out, y_out = [],[]
     while len(x_in)>1:
         
         if x_in[0]>x_in[1]-apparatus_resolution:
             y_in[1] = y_in[0] + y_in[1]
             x_in[1] = (x_in[0] + x_in[1])/2
             x_in.pop(0)
@@ -204,28 +256,28 @@
             x_out.append(x_in[0])
             y_out.append(y_in[0])
             x_in.pop(0)
             y_in.pop(0)
     x_out.append(x_in[0])
     y_out.append(y_in[0])
 
-
     x_in = x_out
     y_in = y_out
     maximum = max(y_in)
 
+    '''sulphur_nitrogen_plotter function'''
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)  
-        print('N')
+        
     
     if has_S:
         x_in.append(x_in[1]-0.004)  
         y_in.append(0.008*count_S*maximum)
-        print('S')
+        
 
     x_out, y_out = [],[]
 
     while len(x_in)>0:
         min_x = min(x_in)
         index_min = x_in.index(min_x)
         x_out.append(min_x)
@@ -233,14 +285,15 @@
         x_in.pop(index_min)
         y_in.pop(index_min)
 
     x_in, y_in = x_out, y_out 
 
     min_x , max_x = min(x_in), max(x_in)
 
+    '''delta_function_plotter function'''
     x_axis, y_axis = [min_x-0.2],[0]
     for i in range (len(x_in)):
         x_axis.append(x_in[i]-10**(-100))
         x_axis.append(x_in[i])
         x_axis.append(x_in[i]+10**(-100))
         y_axis.append(0)
         y_axis.append(y_in[i])
@@ -249,28 +302,30 @@
     x_axis.append(max_x+0.2)
     y_axis.append(0)
 
 
     x_in = x_axis
     y_in = y_axis
 
+    '''double_plot function'''
     ticked_peaks = []
     for i in range(len(x_in)):
         if imprecision_True_False:    
             if y_in[i] > 0.001:
                 ticked_peaks.append(x_in[i])
         else:
             ticked_peaks.append(x_in[i])
 
     #creates the principal graph, mass spectrum of the molecule (interactive)
 
     princ_graph = figure(width=700, title=f'Mass spectrum of molecule')
     princ_graph = figure(x_axis_label = '[m/z]')
     princ_graph = figure(y_axis_label = 'Abundance')
     princ_graph.xaxis.axis_label = "[m/z]"
+    princ_graph.yaxis.axis_label = "Abundance"
     princ_graph.title = 'Mass spectrum of molecule'
     princ_graph.height = 500
     princ_graph.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
     princ_graph.add_tools(WheelPanTool(dimension="height"))
     princ_graph.add_tools(WheelZoomTool(dimensions="height"))
     princ_graph.line(x_in, y_in, line_width=1)
     princ_graph.xaxis.major_label_orientation = "horizontal"
@@ -326,56 +381,24 @@
     img_div = Div(text=f'<img src="{image_url}" style="width:350px;height:350px;">')
 
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
+    '''functional_group_finder function'''
     functional_groups_smarts = {
-        'Alcohol': 'C[Oh1+0]',
-        'Aldehyde': 'C[Ch1]=O',
-        'Ketone': 'CC(=O)C',
-        'Carboxylic Acid': 'CC(=O)[Oh1]',
-        'Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*',
-        'Amide': 'C(=O)N',
-        'Amine': '[C][N]',
-        'Nitrile': 'C#N',
-        'Chloride': 'Cl',
-        'Bromide': 'Br',
-        'Fluoride': 'F',
-        'Iodide': 'I',
-        'Alkene': 'C=C',
-        'Alkyne': 'C#C',
-        'Imine': 'C=N*',
-        'Amino acid': '[Nh2][Ch1*]C(=O)O',
-        'Proline': '[Nh1][Ch1*]C(=O)O',
-        'Thiol': '[Sh1]',
-        'Sulfide': '*[Sh0]*',
-        'Acyl Chloride': 'CC(=O)Cl',
-        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
-        'Nitro': 'C[N+](=O)[O-]',
-        'Enamine': 'C=C[Nh0]',
-        'Enamine2': 'C=C[Nh1]',
-        'Enamine3': 'C=C[Nh2]',
-        'Imide': 'C(=O)NC(=O)*',
-        'Azide': 'CNNN',
-        'Enol': 'C=C([Oh1])C',
-        'Hemiacetal': 'CC(O)(O)C',
-        'Carbonate': '[Oh0]C(=O)[Oh0]',
-        'Carbonate2': '[Oh1]C(=O)[Oh1]',
-        'Disulfide': 'CSSC',
-        'Sulfoxide': 'CS(=O)C',
-        'Sulfone': '*[So2](=O)(=O)*',
-        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
-        'Thioester': 'C(=O)S*',
-        'Phosphine': '*[Po0](*)*',
-        'Phosphate': '*OP(=O)(O)O',
-        'Benzene': 'c1ccccc1',
-        'Peroxide':'C[Oh0][Oh0]C'
+        'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': 'CC(=O)[Oh1]','Ester': 'CC(=O)[Oh0]',
+        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
+        'Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O','Proline': '[Nh1][Ch1*]C(=O)O',
+        'Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*','Nitro': 'C[N+](=O)[O-]',
+        'Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*','Azide': 'CNNN','Enol': 'C=C([Oh1])C',
+        'Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]','Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C',
+        'Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*','Phosphine': '*[Po0](*)*',
+        'Phosphate': '*OP(=O)(O)O','Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
     }
 
     # check that the substructure from functional_groups_smarts are contained in mol_smi
 
     for name, smarts in functional_groups_smarts.items():
         if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
@@ -385,75 +408,103 @@
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
                 if 'Ether' in functional_groups_contained:
                     functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
-    if 'Carboxilic Acid' and 'Ester' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
     #initiate empty variables
     present_group_smarts = []    
     present_group_images_base64 = []
     
     #appends the smarts of the contained functional groups
     for i,j in functional_groups_smarts.items():
@@ -480,49 +531,57 @@
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
                 image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
                 #appends the image to an empty dictionnary
                 present_group_images_base64.append(image_base64)
+            elif x == '[N]':
+                mol2 = Chem.MolFromSmiles('CN')
+
+                #creates the image
+                image = Draw.MolToImage(mol2)
+
+                # Convert the image to base64 format
+                buffered = BytesIO()
+                image.save(buffered, format="PNG")
+                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+                #appends the image to an empty dictionnary
+                present_group_images_base64.append(image_base64)
             else:
                 #creates the image
                 image = Draw.MolToImage(mol)
 
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
                 image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
                 #appends the image to an empty dictionnary
                 present_group_images_base64.append(image_base64)
 
     #creates a dictionnary that links the name of the functional group to its image
-    data = dict(
-        groups=functional_groups_contained,
-        images=present_group_images_base64
-    )
+    data = dict(groups=functional_groups_contained,images=present_group_images_base64)
     source = ColumnDataSource(data)
 
     #template for the bokeh table that read the base64 format 
     template = """
     <div>
         <img src="data:image/png;base64, <%= value %>" style="width:50px;height:50px;">
     </div>
     """
 
     # initiallizing the bokeh figure using the previous template for each functional group
-    columns = [
-        TableColumn(field="groups", title="Functional Groups"),
-        TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))
-    ]
+    columns = [TableColumn(field="groups", title="Functional Groups"),
+    TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))]
     num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
     last = column(img_div, func_group_table)
     final = row(double_graph, last)
     return final
 
-show(spectrum('NCCCCS', True, 0.01))
+show(spectrum('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C', True, 0.01))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `massivechem-4.1/scripts/all_in_one.py` & `massivechem-4.3/scripts/all_in_one.py`

 * *Files 27% similar despite different names*

```diff
@@ -17,14 +17,23 @@
                     - p4 : buttons with info on the molecule
     
     Output: bokeh page with all 4 graphs well arranged
 
     '''
     #---------------------------------------------------------------------------------------------#
     
+    if not p1:
+        raise ValueError("Enter a non-empty plot")
+    if not p2:
+        raise ValueError("Enter a non-empty plot")
+    if not p3:
+        raise ValueError("Enter a non-empty plot")
+    if not p4:
+        raise ValueError("Enter a non-empty plot")
+    
     #creates a layout in row with p3 and p4
     layout1 = row(p3, p4)
 
     #creates a layout in column with p2 and layout1
     layout2 = column(p2, layout1)
 
     #creates the final layout in row with layout1 and p1
```

### Comparing `massivechem-4.1/scripts/calculate_unsaturation.py` & `massivechem-4.3/scripts/calculate_unsaturation.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,24 @@
     calculate_unsaturation(mol_smile)
 
     Input: molecule under SMILEs representation
 
     Output: unsaturation of the input molecule (integer value)
     '''
     #---------------------------------------------------------------------------------------------# 
-
+    if mol_smile == None:
+        raise ValueError('Enter a non-empty input')
+    
     C, N, HX, halogens_hydrogen = 0, 0, 0, ['F', 'Cl', 'Br', 'I', 'At', 'H']
 
     mol = Chem.AddHs(Chem.MolFromSmiles(mol_smile))
-
+    
+    if mol == None:
+        raise ValueError('Invalid SMILEs representation')
+    
     for atom in mol.GetAtoms():
         if atom.GetSymbol() == 'C':
             C += 1
         elif atom.GetSymbol() == 'N':
             N += 1
         elif atom.GetSymbol() in halogens_hydrogen:
             HX += 1
```

### Comparing `massivechem-4.1/scripts/double_plot.py` & `massivechem-4.3/scripts/double_plot.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     Output: 2 Bokeh graphs:
             - One that shows the mass spectrum of the molecule to which the user can interact
             -Another that is the same graph but shows where the user is zooming on the first graph
     '''
     #---------------------------------------------------------------------------------------------#
 
     # tells where to put the graduation on the graph
-
+    if not x_in:
+        raise ValueError("Enter a non-empty list as first argument")
+    if not y_in:
+        raise ValueError("Enter a non-empty list as second argument")
+    if len(x_in) != len(y_in):
+        raise ValueError("The two lists must have the same length")
+    
     ticked_peaks = []
     for i in range(len(x_in)):
         if y_in[i] > 0.0001:
             ticked_peaks.append(x_in[i])
 
     #creates the principal graph, mass spectrum of the molecule (interactive)
```

### Comparing `massivechem-4.1/scripts/functional_group_display.py` & `massivechem-4.3/scripts/functional_group_display.py`

 * *Files identical despite different names*

### Comparing `massivechem-4.1/scripts/ionisation_method.py` & `massivechem-4.3/scripts/ionisation_method.py`

 * *Files identical despite different names*

### Comparing `massivechem-4.1/scripts/main_function.py` & `massivechem-4.3/scripts/main_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
     
     Output: two lists:
     1. list of the masses (of individual molecules) of each possible combination of isotopes
     2. list of the probabilities of apparation of each of the molecules 
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
+
+    if not list_atoms:
+        raise ValueError('Enter a valid input for the first argument')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a valid input for the second argument')
+    
     render_imprecise_list = imprecision_True_False 
     #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
     
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057, 59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 91.90504, 90.90565, 89.9047, 95.90827]
     abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003, 0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031, 0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097, 0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 0.027999999999999997]
     isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Та', 'Та', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
 
@@ -28,16 +34,14 @@
         has_N = True
         count_N = list_atoms.count('N')
     elif 'S' in list_atoms and list_atoms.count('S')%2 == 1:
         has_S = True
         count_S = list_atoms.count('S')
 
 
-    print(list_atoms)
-
     list_output = []
     mass_copy = mass.copy()
     abundance_copy = abundance.copy()
     isotopes_copy = isotopes.copy()
 
     for i in range (isotopes.count(list_atoms[0])):
         
@@ -71,30 +75,30 @@
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
-                #removes any molecule who's probability is below 0.0001
+                #removes any molecule who's probability is below 0.00001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
                 isotopes_copy.pop(index)
                 
         list_output = list_output_new
         list_atoms.pop(0)
-    print(list_output)
+
 
 
     #Conversion of list_output (which is a list of lists) to a combination of two lists (x_axis & y_axis)
 
     x_axis, y_axis = [],[]
     x_axis_final, y_axis_final = [],[]
     for j in range (len(list_output)):
```

### Comparing `massivechem-4.1/scripts/molecule_list_generator.py` & `massivechem-4.3/scripts/molecule_list_generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,12 +4,13 @@
     molecule_list_generator(mol)
     
     Input: molecule under MOL representation
     
     Output: list containing the atomic symbol of each atom in the input molecule
     '''
     #---------------------------------------------------------------------------------------------#
-
+    if not mol:
+        raise ValueError('Enter a non-empty input')
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
     return list_atoms
```

### Comparing `massivechem-4.1/scripts/peak_merger.py` & `massivechem-4.3/scripts/peak_merger.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
     2. ordered list of the probabilities of apparation of each of the molecules
     
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not x_in:
+        raise ValueError('Empty list entry')
+    if not y_in:
+        raise ValueError('Empty list entry')
+    if len(x_in) != len(y_in):
+        raise ValueError('Lists should be of the same size')
+
     x_out, y_out = [],[]
     while len(x_in)>1:
         if x_in[0]>x_in[1]-apparatus_resolution:
             y_in[1] = y_in[0] + y_in[1]
             x_in[1] = (x_in[0] + x_in[1])/2
             x_in.pop(0)
             y_in.pop(0)
```

### Comparing `massivechem-4.1/scripts/peak_sorter.py` & `massivechem-4.3/scripts/peak_sorter.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,21 @@
     Output: two lists:
     1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
     2. ordered list of the probabilities of apparation of each of the molecules
     
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
+    
+    if not x_in:
+        raise ValueError('Empty list entry')
+    if not y_in:
+        raise ValueError('Empty list entry')
+    if len(x_in) != len(y_in):
+        raise ValueError('Lists should be of the same size')
 
     x_out, y_out = [],[]
     while len(x_in)>0:
         min_x = min(x_in)
         index_min = x_in.index(min_x)
         x_out.append(min_x)
         y_out.append(y_in[index_min])
```

### Comparing `massivechem-4.1/scripts/smiles_to_3D_plot.py` & `massivechem-4.3/scripts/smiles_to_3D_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from rdkit import Chem
 from rdkit.Chem import AllChem
 import tempfile
 from xyz2graph import MolGraph, to_plotly_figure
 import panel as pn
 
-def smiles_to_3D_plot(mol_smi,last,double_graph):
+def smiles_to_3D_plot(mol_smi):
 
      #---------------------------------------------------------------------------------------------#
     '''
     smiles_to_3D_plot(smiles)
     
     Input: molecule is a SMILEs format
 
     Output: panel graph of the molecule in 3D and interactive
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError("Enter a non-empty string as argument")
+
     # Generate 3D coordinates from SMILES string
     mol2 = Chem.MolFromSmiles(mol_smi)
     mol2 = Chem.AddHs(mol2)  # Add hydrogens for better geometry optimization
     AllChem.EmbedMolecule(mol2, randomSeed=42)  # Embed the molecule in 3D space
     AllChem.MMFFOptimizeMolecule(mol2)  # Optimize the geometry using MMFF94 force field
 
     # Create a temporary file to store the 
@@ -35,23 +38,15 @@
     
     # Read the data from the temporary file
     mg.read_xyz(tmp_path)
 
     # Create the Plotly figure object
     fig = to_plotly_figure(mg)
 
-    plotly_pane = pn.pane.Plotly(fig)
-
-    p1_pane = pn.pane.Bokeh(last)
-    p2_pane = pn.pane.Bokeh(double_graph)
-
-    layout12 = pn.Column( plotly_pane, p1_pane)
-    final = pn.Row(p2_pane, layout12)
-
-    return final
+    return fig
 
 # Example usage
 input_mol = input('MOL:  ')
 smiles_to_3D_plot(input_mol).show()
```

### Comparing `massivechem-4.1/scripts/spectrum.py` & `massivechem-4.3/test/test_spectrum_3D.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,26 @@
 from bokeh.io import show
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
 
 import base64
 from io import BytesIO
 
+import panel as pn
+import xyz2graph
+import tempfile
+from xyz2graph import MolGraph, to_plotly_figure
 
-def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
+
+def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
+    mol_smi_3D = mol_smi
+
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
             12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
             113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
             52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
             159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
             56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
@@ -84,26 +91,31 @@
                 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
                 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
                 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
                 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
                 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
                 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
     
+    if not mol_smi:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
 
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     
     mol = Chem.AddHs(mol_without_Hs)
 
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
-
+    
+    if not list_atoms:
+        return None
+    
     #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
 
     if 'H' in list_atoms:
 
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
 
@@ -163,18 +175,18 @@
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
-                #removes any molecule who's probability is below 0.0001
+                #removes any molecule who's probability is below 0.00001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
@@ -363,15 +375,15 @@
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
         'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': '*C(=O)[Oh1]','Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
+        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
         'Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O','Proline': '[Nh1][Ch1*]C(=O)O',
         'Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*','Nitro': 'C[N+](=O)[O-]',
         'Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*','Azide': 'CNNN','Enol': 'C=C([Oh1])C',
         'Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]','Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C',
         'Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*','Phosphine': '*[Po0](*)*','Phosphate': '*OP(=O)(O)O',
         'Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
     }
@@ -387,78 +399,103 @@
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
                 if 'Ether' in functional_groups_contained:
                     functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Amide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amine')
-    if 'Carboxilic Acid' and 'Ester' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
     #initiate empty variables
     present_group_smarts = []    
     present_group_images_base64 = []
     
     #appends the smarts of the contained functional groups
     for i,j in functional_groups_smarts.items():
@@ -485,27 +522,14 @@
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
                 image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
                 #appends the image to an empty dictionnary
                 present_group_images_base64.append(image_base64)
-            elif x == '[N]':
-                mol2 = Chem.MolFromSmiles('CN')
-
-                #creates the image
-                image = Draw.MolToImage(mol2)
-
-                # Convert the image to base64 format
-                buffered = BytesIO()
-                image.save(buffered, format="PNG")
-                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
-
-                #appends the image to an empty dictionnary
-                present_group_images_base64.append(image_base64)
             else:
                 #creates the image
                 image = Draw.MolToImage(mol)
 
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
@@ -535,12 +559,85 @@
     ]
     num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
-    last = column(img_div, func_group_table)
-    final = row(double_graph, last)
-    return final
+    last = row(img_div, func_group_table)
+
+    # Generate 3D coordinates from SMILES string
+    mol_3D = Chem.MolFromSmiles(mol_smi_3D)
+    mol_3D = Chem.AddHs(mol_3D)  # Add hydrogens for better geometry optimization
+    AllChem.EmbedMolecule(mol_3D, randomSeed=42)  # Embed the molecule in 3D space
+    AllChem.MMFFOptimizeMolecule(mol_3D)  # Optimize the geometry using MMFF94 force field
+
+    # Create a temporary file to store the 
+    with tempfile.NamedTemporaryFile(delete=False) as tmp:
+        tmp.write(f"{mol_3D.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
+        for atom in mol_3D.GetAtoms():
+            pos = mol_3D.GetConformer().GetAtomPosition(atom.GetIdx())
+            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
+        tmp_path = tmp.name
+
+    # Create the MolGraph object
+    mg = MolGraph()
+    
+    # Read the data from the temporary file
+    mg.read_xyz(tmp_path)
+
+    # Create the Plotly figure object
+    fig = to_plotly_figure(mg)
+
+
+    # Converts all the graphs to pane to combine Bokeh and Plotly
+    fig_pane = pn.pane.Plotly(fig)
+
+    last_pane = pn.pane.Bokeh(last)
+
+    left_pane = pn.pane.Bokeh(double_graph)
+
+    # Creates the final plot
+    right_pane = pn.Column(fig_pane, last_pane)
+
+    total_plot_pane = pn.Row(left_pane, right_pane)
+
+    return total_plot_pane
+
+
+
+import unittest
+
+class TestSpectrum3D(unittest.TestCase):
+    
+    def setUp(self):
+        self.apparatus_resolution = 0.01
+
+    def test_butane_False(self):
+        mol_smi = "CCCC"
+        imprecision_True_False = False
+        result = spectrum_3D(mol_smi, imprecision_True_False, self.apparatus_resolution)
+        self.assertIsNotNone(result)
+    
+    def test_butane_True(self):
+        mol_smi = "CCCC"
+        imprecision_True_False = True
+        result = spectrum_3D(mol_smi, imprecision_True_False, self.apparatus_resolution)
+        self.assertIsNotNone(result)
+
+    def test_empty_input(self):
+        
+        with self.assertRaises(ValueError):
+            imprecision_True_False= False
+            spectrum_3D("",imprecision_True_False, self.apparatus_resolution)
+
+    def test_invalid_input(self):
+        
+        with self.assertRaises(ValueError):
+            imprecision_True_False = False
+            spectrum_3D("invalid_smiles",imprecision_True_False, self.apparatus_resolution)  
+        
+
+if __name__ == '__main__':
+    unittest.main()
+
 
-show(spectrum('CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C', True, 0.01))
```

### Comparing `massivechem-4.1/scripts/sulphur_nitrogen_adder.py` & `massivechem-4.3/scripts/sulphur_nitrogen_adder.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,14 +15,35 @@
     1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
     2. ordered list of the probabilities of apparation of each of the molecules
     
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not x_in:
+        raise ValueError("Enter a non-empty list")
+    if not y_in:
+        raise ValueError("Enter a non-empty list")
+    if len(x_in) != len(y_in):
+        raise ValueError("The two lists must have the same length")
+    if has_N not in [True, False]:
+        raise ValueError("The third argument must be a boolean")
+    if has_S not in [True, False]:
+        raise ValueError("The fourth argument must be a boolean")
+    if count_N < 0:
+        raise ValueError("The fifth argument must be a positive integer")
+    if count_S < 0:
+        raise ValueError("The sixth argument must be a positive integer")
+    if type(count_N) != int:
+        raise ValueError("The fifth argument must be an integer")
+    if type(count_S) != int:
+        raise ValueError("The sixth argument must be an integer")
+    if x_in != sorted(x_in):
+        raise ValueError("The first list must be ordered")
+
     maximum = max(y_in)
 
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)  
     
     if has_S:
```

### Comparing `massivechem-4.1/src/MASSiveChem/MASSiveChem.py` & `massivechem-4.3/notebooks/backup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,76 @@
 from rdkit import Chem
 from rdkit.Chem import Draw, AllChem
 
-import pandas as pd
-
 import base64
 
 import os
 
 from bokeh.plotting import figure, row
-from bokeh.models.tickers import FixedTicker
-from bokeh.layouts import row, column
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
+from bokeh.models.tickers import FixedTicker
 from bokeh.models.widgets import DataTable, TableColumn
+from bokeh.layouts import row, column
 
 from io import BytesIO
 
+import tempfile
+
+from xyz2graph import MolGraph, to_plotly_figure
+
+import panel as pn
+
+#main functions:
+#1
 def calculate_unsaturation(mol_smile) -> int:
     #---------------------------------------------------------------------------------------------#
     '''
     calculate_unsaturation(mol_smile)
 
     Input: molecule under SMILEs representation
 
     Output: unsaturation of the input molecule (integer value)
     '''
     #---------------------------------------------------------------------------------------------# 
-
+    if mol_smile == None:
+        raise ValueError('Enter a non-empty input')
+    
     C, N, HX, halogens_hydrogen = 0, 0, 0, ['F', 'Cl', 'Br', 'I', 'At', 'H']
 
     mol = Chem.AddHs(Chem.MolFromSmiles(mol_smile))
-
+    
+    if mol == None:
+        raise ValueError('Invalid SMILEs representation')
+    
     for atom in mol.GetAtoms():
         if atom.GetSymbol() == 'C':
             C += 1
         elif atom.GetSymbol() == 'N':
             N += 1
         elif atom.GetSymbol() in halogens_hydrogen:
             HX += 1
 
     unsaturation = C + 1 + (N - HX) / 2
 
     return unsaturation
 
-def SMILEs_interpreter(mol_smi):
-    #---------------------------------------------------------------------------------------------#
-    '''
-    SMILEs_interpreter(mol_smi)
-
-    Input: molecule under SMILEs representation
-    
-    Output: molecule under MOL representation
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    #Checks that the SMILEs input is correct/allowed
-
-    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+#2
+def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
 
+    #tests for wether the input is valid
     if mol_without_Hs is None:
-        print('')
-        print("Invalid SMILEs input.")
-        print('Please try again with a different SMILEs.')
-        exit()
-
-    mol = Chem.AddHs(mol_without_Hs)
-
-    return mol
-
-def molecule_list_generator(mol) -> list[str]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    molecule_list_generator(mol)
-    
-    Input: molecule under MOL representation
-    
-    Output: list containing the atomic symbol of each atom in the input molecule
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    list_atoms = []
-    for atom in mol.GetAtoms():
-        list_atoms.append(atom.GetSymbol())
-    return list_atoms
-
-def ionisation_method (list_atoms) -> list[str]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    ionisation_method (list_atoms)
-    
-    Input: list of atomic symbols of atoms in a given molecule
-    
-    Output: corrected list of atoms (i.e. list of atoms that enter spectrometry apparatus)
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    '''In the case of ionisation by proton, we need to add a H+ ion, which is done in the following'''
-    if 'H' in list_atoms:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a boolean value')
+    if apparatus_resolution < 0:
+        raise ValueError('Enter a positive value')
+    if type(apparatus_resolution) != float:
+        raise ValueError('Enter an integer value')
 
-        #Check that there is in fact a proton to remove
-        list_atoms.remove('H')
-    return list_atoms
 
-def main_function(list_atoms, imprecision_True_False) -> list[float]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    main_function(list_atoms)
-    
-    Input: list of atoms that enter the apparatus
-    
-    Output: two lists:
-    1. list of the masses (of individual molecules) of each possible combination of isotopes
-    2. list of the probabilities of apparation of each of the molecules 
-    (the mass in list 1 at index i is associated to the probability at index i in list 2)
-    '''
-    #---------------------------------------------------------------------------------------------#
-    render_imprecise_list = imprecision_True_False 
-    #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
-    
     #lists of the data to facilitise the pip-installability of the package
 
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
             12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
             113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
             52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
@@ -187,35 +137,60 @@
                 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
                 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
                 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
                 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
                 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
                 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
     
-    #check for sulphur and nitrogen
 
+    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+
+
+    
+    mol = Chem.AddHs(mol_without_Hs)
+
+    '''molecule list generator'''
+    list_atoms = []
+    for atom in mol.GetAtoms():
+        list_atoms.append(atom.GetSymbol())
+
+    #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
+
+    '''Ionisation method'''
+    if 'H' in list_atoms:
+
+        #Check that there is in fact a proton to remove
+        list_atoms.remove('H')
+
+    render_imprecise_list = imprecision_True_False 
+    #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
+
+    
     has_N = False
     count_N = 0
     has_S = False
     count_S = 0
+
+    '''sulphur_nitrogen_finder function'''
     if 'N' in list_atoms and list_atoms.count('N')%2 == 1:
         has_N = True
         count_N = list_atoms.count('N')
-    elif 'S' in list_atoms and list_atoms.count('S')%2 == 1:
+        
+    if 'S' in list_atoms and list_atoms.count('S')%2 == 1:
         has_S = True
         count_S = list_atoms.count('S')
 
 
-    print(list_atoms)
 
     list_output = []
     mass_copy = mass.copy()
     abundance_copy = abundance.copy()
     isotopes_copy = isotopes.copy()
 
+    '''main function'''
     for i in range (isotopes.count(list_atoms[0])):
         
         index = isotopes.index(list_atoms[0])
         list_output.append([mass_copy[index],abundance_copy[index]])
         mass_copy.pop(index)
         abundance_copy.pop(index)
         isotopes_copy.pop(index)
@@ -247,34 +222,35 @@
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
                 #removes any molecule who's probability is below 0.0001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
                 isotopes_copy.pop(index)
                 
         list_output = list_output_new
         list_atoms.pop(0)
-    print(list_output)
+    
 
 
     #Conversion of list_output (which is a list of lists) to a combination of two lists (x_axis & y_axis)
 
     x_axis, y_axis = [],[]
     x_axis_final, y_axis_final = [],[]
     for j in range (len(list_output)):
+        '''x_axis.append(list_output[j][0])'''
         x_axis.append(round(list_output[j][0],3)) # Adds rounded value (should help with Python-limitations that render a diff of magnitude 10^(-7) to combinatorics
         
         y_axis.append(list_output[j][1]) #Adds the true value
         
 
     #Compression of lists x_axis & y_axis into x_axis_final & y_axis_final so that peaks corresponding to same mass will be represented together 
     
@@ -286,597 +262,380 @@
                 x_axis_final.append(x_axis[j])
                 y_axis_final.append(y_axis[j])
             else:
                 index = x_axis_final.index(x_axis[j])
                 y_axis_final[index] =y_axis_final[index] + y_axis[j]
 
 
-    #if there is any, add peaks corresponding to Sulphur/Nitrogen presence
-    maximum = max(y_axis_final)
-    maximum_2 = 0
-    for i in range (len(y_axis_final)):
-        if y_axis_final[i]>maximum_2 and y_axis_final[i]< maximum:
-            maximum_2 = y_axis_final[i]
-    index = y_axis_final.index(maximum_2)
-
-    if has_N:
-        x_axis_final.append(x_axis_final[index] - 0.006)  
-        y_axis_final.append(0.0035*count_N*maximum)  
     
-    if has_S:
-        x_axis_final.append(x_axis_final[index]-0.004)  
-        y_axis_final.append(0.008*count_S*maximum)  
+    x_in, y_in = x_axis_final, y_axis_final
+    
+    x_out, y_out = [],[]
+
+    '''list_sorter function'''
+    while len(x_in)>0:
+        min_x = min(x_in)
+        index_min = x_in.index(min_x)
+        x_out.append(min_x)
+        y_out.append(y_in[index_min])
+        x_in.pop(index_min)
+        y_in.pop(index_min)
 
-    return x_axis_final, y_axis_final
 
-def peak_merger(x_in, y_in, apparatus_resolution) -> list[float]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    delta_function_plotter(x_in, y_in)
-    
-    Input: two lists + float:
-    1. ordered list of the masses (of individual molecules) of each possible combination of isotopes
-    2. ordered list of the probabilities of apparation of each of the molecules
-    3. apparatus precision (float representation of number which is the limit between two peaks above which they appear merged together)
-    
-    Output: two lists:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
-    
-    (the mass in list 1 at index i is associated to the probability at index i in list 2)
-    '''
-    #---------------------------------------------------------------------------------------------#
 
+    x_in, y_in = x_out, y_out 
+    
+    '''peak_merger function'''
     x_out, y_out = [],[]
     while len(x_in)>1:
+        
         if x_in[0]>x_in[1]-apparatus_resolution:
             y_in[1] = y_in[0] + y_in[1]
             x_in[1] = (x_in[0] + x_in[1])/2
             x_in.pop(0)
             y_in.pop(0)
         else:
             x_out.append(x_in[0])
             y_out.append(y_in[0])
             x_in.pop(0)
             y_in.pop(0)
     x_out.append(x_in[0])
     y_out.append(y_in[0])
 
-    return x_out, y_out
-
-def sulphur_nitrogen_adder(x_in, y_in, has_N, has_S, count_N, count_S) -> list[float]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    sulphur_nitrogen_adder(x_in, y_in, has_N, has_S, count_N, count_S)
-    
-    Input: two lists + 4 booleans:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
-    3. boolean that tells if the molecule contains Nitrogen
-    4. boolean that tells if the molecule contains Sulphur
-    5. number of Nitrogen atoms in the molecule
-    6. number of Sulphur atoms in the molecule
-    
-    Output: two lists:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
-    
-    (the mass in list 1 at index i is associated to the probability at index i in list 2)
-    '''
-    #---------------------------------------------------------------------------------------------#
-
+    x_in = x_out
+    y_in = y_out
     maximum = max(y_in)
 
+    '''sulphur_nitrogen_plotter function'''
     if has_N:
         x_in.append(x_in[1] - 0.006)  
         y_in.append(0.0035*count_N*maximum)  
+        
     
     if has_S:
         x_in.append(x_in[1]-0.004)  
         y_in.append(0.008*count_S*maximum)
-
-
-    return x_in, y_in
-
-def peak_sorter(x_in, y_in) -> list[float]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    peak_sorter(x_in, y_in)
-    
-    Input: two lists:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
-    
-    Output: two lists:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
-    
-    (the mass in list 1 at index i is associated to the probability at index i in list 2)
-    '''
-    #---------------------------------------------------------------------------------------------#
+        
 
     x_out, y_out = [],[]
+
     while len(x_in)>0:
         min_x = min(x_in)
         index_min = x_in.index(min_x)
         x_out.append(min_x)
         y_out.append(y_in[index_min])
         x_in.pop(index_min)
         y_in.pop(index_min)
 
-    return x_out, y_out
-
-def delta_function_plotter(x_in, y_in) -> list[float]:
-    #---------------------------------------------------------------------------------------------#
-    '''
-    delta_function_plotter(x_in, y_in)
-    
-    Input: two lists:
-    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered)
-    2. list of the probabilities of apparation of each of the molecules (ordered)
-    
-    Output: two lists:
-    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered) with values of 0 (y_axis) added on eiter side of the "peak"
-    2. list of the probabilities of apparation of each of the molecules (ordered)
-    
-    (the mass in list 1 at index i is associated to the probability at index i in list 2)
-    '''
-    #---------------------------------------------------------------------------------------------#
+    x_in, y_in = x_out, y_out 
 
     min_x , max_x = min(x_in), max(x_in)
 
-    x_axis, y_axis = [min_x-0.5],[0]
+    '''delta_function_plotter function'''
+    x_axis, y_axis = [min_x-0.2],[0]
     for i in range (len(x_in)):
         x_axis.append(x_in[i]-10**(-100))
         x_axis.append(x_in[i])
         x_axis.append(x_in[i]+10**(-100))
         y_axis.append(0)
         y_axis.append(y_in[i])
         y_axis.append(0)
 
-    x_axis.append(max_x+1)
+    x_axis.append(max_x+0.2)
     y_axis.append(0)
 
-    return x_axis, y_axis
-
-def double_plot(x_in,y_in):
-
-    #---------------------------------------------------------------------------------------------#
-    '''
-    double_plot(x_in,y_in)
-    
-    Input: list of masses (x_in) and intensities (y_in)
-    
-    Output: 2 Bokeh graphs:
-            - One that shows the mass spectrum of the molecule to which the user can interact
-            -Another that is the same graph but shows where the user is zooming on the first graph
-    '''
-    #---------------------------------------------------------------------------------------------#
 
-    # tells where to put the graduation on the graph
+    x_in = x_axis
+    y_in = y_axis
 
+    '''double_plot function'''
     ticked_peaks = []
     for i in range(len(x_in)):
-        if y_in[i] > 0.0001:
+        if imprecision_True_False:    
+            if y_in[i] > 0.001:
+                ticked_peaks.append(x_in[i])
+        else:
             ticked_peaks.append(x_in[i])
 
     #creates the principal graph, mass spectrum of the molecule (interactive)
 
-    p1 = figure(width=700, title=f'Mass spectrum of molecule')
-    p1 = figure(x_axis_label = '[m/z]')
-    p1 = figure(y_axis_label = 'Abundance')
-    p1.xaxis.axis_label = "[m/z]"
-    p1.height = 500
-    p1.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
-    p1.add_tools(WheelPanTool(dimension="height"))
-    p1.add_tools(WheelZoomTool(dimensions="height"))
-    p1.line(x_in, y_in, line_width=1)
-    p1.xaxis.major_label_orientation = "horizontal"
+    princ_graph = figure(width=700, title=f'Mass spectrum of molecule')
+    princ_graph = figure(x_axis_label = '[m/z]')
+    princ_graph = figure(y_axis_label = 'Abundance')
+    princ_graph.xaxis.axis_label = "[m/z]"
+    princ_graph.yaxis.axis_label = "Abundance"
+    princ_graph.title = 'Mass spectrum of molecule'
+    princ_graph.height = 500
+    princ_graph.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
+    princ_graph.add_tools(WheelPanTool(dimension="height"))
+    princ_graph.add_tools(WheelZoomTool(dimensions="height"))
+    princ_graph.line(x_in, y_in, line_width=1)
+    princ_graph.xaxis.major_label_orientation = "horizontal"
 
      #creates the secondary graph, mass spectrum of the molecule (non-interactive)
 
-    p2 = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [Th]', y_axis_label='Intensity')
-    p2 = figure(width=300, title=f'Mass spectrum of molecule')
-    p2 = figure(toolbar_location=None)
-    p2.height = 300
-    p2.line(x_in, y_in, legend_label="Mass spectrum", line_width=1)
+    sec_graph = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [Th]', y_axis_label='Intensity')
+    sec_graph = figure(width=250, title=f'Mass spectrum of molecule')
+    sec_graph = figure(toolbar_location=None)
+    sec_graph.height = 250
+    sec_graph.line(x_in, y_in, legend_label="Mass spectrum", line_width=1)
 
     #creates a tool in order that the second graph shows where the zoom is on the first one
 
     box = BoxAnnotation(left=0, right=0, bottom=0, top=0,
     fill_alpha=0.1, line_color='red', fill_color='cornflowerblue')
 
     jscode = """
         box[%r] = cb_obj.start
         box[%r] = cb_obj.end
     """
 
     xcb = CustomJS(args=dict(box=box), code=jscode % ('left', 'right'))
     ycb = CustomJS(args=dict(box=box), code=jscode % ('bottom', 'top'))
 
-    p1.x_range.js_on_change('start', xcb)
-    p1.x_range.js_on_change('end', xcb)
-    p1.y_range.js_on_change('start', ycb)
-    p1.y_range.js_on_change('end', ycb)
+    princ_graph.x_range.js_on_change('start', xcb)
+    princ_graph.x_range.js_on_change('end', xcb)
+    princ_graph.y_range.js_on_change('start', ycb)
+    princ_graph.y_range.js_on_change('end', ycb)
 
     # adds the functionnality to the second figure
 
-    p2.add_layout(box)
+    sec_graph.add_layout(box)
 
     # creates a layout that displays the 2 graphs
 
-    layout = column(p1, p2)
-    print('here')
-    return layout
+    double_graph = column(princ_graph, sec_graph)
 
-def functional_group_finder(mol_smi):
 
-    #---------------------------------------------------------------------------------------------#
-    '''
-    functional_group_finder(mol_smi)
-    
-    Input: molecule under SMILEs representation
-    
-    Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
-    '''
-    #---------------------------------------------------------------------------------------------#
+    # Generate the image from the molecule
+    mol = Chem.MolFromSmiles(mol_smi)
+
+    #Draws the image
+    image = Draw.MolToImage(mol)
+
+    #stocks the image in a base64 format
+    buffered = BytesIO()
+    image.save(buffered, format="PNG")
+    image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+    image_url = f"data:image/png;base64,{image_base64}"
+
+    # Create a Div element to display the image
+    img_div = Div(text=f'<img src="{image_url}" style="width:350px;height:350px;">')
 
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
+    '''functional_group_finder function'''
     functional_groups_smarts = {
-        'Alcohol': 'C[Oh1+0]',
-        'Aldehyde': 'C[Ch1]=O',
-        'Ketone': 'CC(=O)C',
-        'Carboxylic Acid': 'CC(=O)[Oh1]',
-        'Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*',
-        'Amide': 'C(=O)N',
-        'Amine': '[C][N]',
-        'Nitrile': 'C#N',
-        'Chloride': 'Cl',
-        'Bromide': 'Br',
-        'Fluoride': 'F',
-        'Iodide': 'I',
-        'Alkene': 'C=C',
-        'Alkyne': 'C#C',
-        'Imine': 'C=N*',
-        'Amino acid': '[Nh2][Ch1*]C(=O)O',
-        'Proline': '[Nh1][Ch1*]C(=O)O',
-        'Thiol': '[Sh1]',
-        'Sulfide': '*[Sh0]*',
-        'Acyl Chloride': 'CC(=O)Cl',
-        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
-        'Nitro': 'C[N+](=O)[O-]',
-        'Enamine': 'C=C[Nh0]',
-        'Enamine2': 'C=C[Nh1]',
-        'Enamine3': 'C=C[Nh2]',
-        'Imide': 'C(=O)NC(=O)*',
-        'Azide': 'CNNN',
-        'Enol': 'C=C([Oh1])C',
-        'Hemiacetal': 'CC(O)(O)C',
-        'Carbonate': '[Oh0]C(=O)[Oh0]',
-        'Carbonate2': '[Oh1]C(=O)[Oh1]',
-        'Disulfide': 'CSSC',
-        'Sulfoxide': 'CS(=O)C',
-        'Sulfone': '*[So2](=O)(=O)*',
-        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
-        'Thioester': 'C(=O)S*',
-        'Phosphine': '*[Po0](*)*',
-        'Phosphate': '*OP(=O)(O)O',
-        'Benzene': 'c1ccccc1',
-        'Peroxide':'C[Oh0][Oh0]C'
+        'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': 'CC(=O)[Oh1]','Ester': 'CC(=O)[Oh0]',
+        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
+        'Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O','Proline': '[Nh1][Ch1*]C(=O)O',
+        'Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*','Nitro': 'C[N+](=O)[O-]',
+        'Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*','Azide': 'CNNN','Enol': 'C=C([Oh1])C',
+        'Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]','Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C',
+        'Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*','Phosphine': '*[Po0](*)*',
+        'Phosphate': '*OP(=O)(O)O','Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
     }
 
     # check that the substructure from functional_groups_smarts are contained in mol_smi
 
     for name, smarts in functional_groups_smarts.items():
         if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
                 functional_groups_contained.append(name)
 
     # exceptions for conflicts during the iteration of functional groups
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
-    
-    
-    return functional_groups_contained
-
-def functional_group_display(contained_functional_groups):
-
-    #---------------------------------------------------------------------------------------------#
-    '''
-    functional_group_display(contained_functional_groups)
-    
-    Input: list of all contained functional groups in the molecule
-
-    Output: bokeh table with the contained functional groups and their image
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    #dictionnary with functional groups and associated SMARTs
-    functional_groups_smarts = {
-        'Alcohol': 'C[Oh1+0]',
-        'Aldehyde': 'C[Ch1]=O',
-        'Ketone': 'CC(=O)C',
-        'Carboxylic Acid': 'CC(=O)[Oh1]',
-        'Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*',
-        'Amide': 'C(=O)N',
-        'Amine': '[C][N]',
-        'Nitrile': 'C#N',
-        'Chloride': 'Cl',
-        'Bromide': 'Br',
-        'Fluoride': 'F',
-        'Iodide': 'I',
-        'Alkene': 'C=C',
-        'Alkyne': 'C#C',
-        'Imine': 'C=N*',
-        'Amino acid': '[Nh2][Ch1*]C(=O)O',
-        'Proline': '[Nh1][Ch1*]C(=O)O',
-        'Thiol': '[Sh1]',
-        'Sulfide': '*[Sh0]*',
-        'Acyl Chloride': 'CC(=O)Cl',
-        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
-        'Nitro': 'C[N+](=O)[O-]',
-        'Enamine': 'C=C[Nh0]',
-        'Enamine2': 'C=C[Nh1]',
-        'Enamine3': 'C=C[Nh2]',
-        'Imide': 'C(=O)NC(=O)*',
-        'Azide': 'CNNN',
-        'Enol': 'C=C([Oh1])C',
-        'Hemiacetal': 'CC(O)(O)C',
-        'Carbonate': '[Oh0]C(=O)[Oh0]',
-        'Carbonate2': '[Oh1]C(=O)[Oh1]',
-        'Disulfide': 'CSSC',
-        'Sulfoxide': 'CS(=O)C',
-        'Sulfone': '*[So2](=O)(=O)*',
-        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
-        'Thioester': 'C(=O)S*',
-        'Phosphine': '*[Po0](*)*',
-        'Phosphate': '*OP(=O)(O)O',
-        'Benzene': 'c1ccccc1',
-        'Peroxide':'C[Oh0][Oh0]C'
-    }
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
     #initiate empty variables
     present_group_smarts = []    
     present_group_images_base64 = []
     
     #appends the smarts of the contained functional groups
     for i,j in functional_groups_smarts.items():
-        for x in contained_functional_groups:
+        for x in functional_groups_contained:
             if x == i:
                 present_group_smarts.append(j)
 
     #converts the smarts to images in base64 format
     for x in present_group_smarts:
 
         #converts SMARTs to SMILEs for the images to be nicer
         mol_x = Chem.MolFromSmarts(x)
         mol_smi = Chem.MolToSmiles(mol_x)
         mol = Chem.MolFromSmiles(mol_smi)
 
         if mol:
 
-            #creates the image
-            image = Draw.MolToImage(mol)
+            if x == 'CC(=O)[Oh0]':
+                mol2 = Chem.MolFromSmiles('CC(=O)OC')
 
-            # Convert the image to base64 format
-            buffered = BytesIO()
-            image.save(buffered, format="PNG")
-            image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+                #creates the image
+                image = Draw.MolToImage(mol2)
 
-            #appends the image to an empty dictionnary
-            present_group_images_base64.append(image_base64)
+                # Convert the image to base64 format
+                buffered = BytesIO()
+                image.save(buffered, format="PNG")
+                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+                #appends the image to an empty dictionnary
+                present_group_images_base64.append(image_base64)
+            elif x == '[N]':
+                mol2 = Chem.MolFromSmiles('CN')
+
+                #creates the image
+                image = Draw.MolToImage(mol2)
+
+                # Convert the image to base64 format
+                buffered = BytesIO()
+                image.save(buffered, format="PNG")
+                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+                #appends the image to an empty dictionnary
+                present_group_images_base64.append(image_base64)
+            else:
+                #creates the image
+                image = Draw.MolToImage(mol)
+
+                # Convert the image to base64 format
+                buffered = BytesIO()
+                image.save(buffered, format="PNG")
+                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+                #appends the image to an empty dictionnary
+                present_group_images_base64.append(image_base64)
 
     #creates a dictionnary that links the name of the functional group to its image
-    data = dict(
-        groups=contained_functional_groups,
-        images=present_group_images_base64
-    )
+    data = dict(groups=functional_groups_contained,images=present_group_images_base64)
     source = ColumnDataSource(data)
 
     #template for the bokeh table that read the base64 format 
     template = """
     <div>
         <img src="data:image/png;base64, <%= value %>" style="width:50px;height:50px;">
     </div>
     """
 
     # initiallizing the bokeh figure using the previous template for each functional group
-    columns = [
-        TableColumn(field="groups", title="Functional Groups"),
-        TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))
-    ]
-    num_groups = len(contained_functional_groups)
+    columns = [TableColumn(field="groups", title="Functional Groups"),
+    TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))]
+    num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
-    data_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
-
-    return data_table
-
-def mol_web_show(mol_smi, show_Hs=False, show_3D = False):
-
-     #---------------------------------------------------------------------------------------------#
-    '''
-    mol_web_show(mol_smi, show_Hs=False, show_3D = False)
-    
-    Input: SMILEs of a molecule. Also specify if want the function to show the hydrogens explicitely or the 3D
-    
-    Output: image of the molecule as a bokeh plot
-    '''
-    #---------------------------------------------------------------------------------------------#
-
-    # name of the file name to create
-    filename = 'molecule_image.png'
-
-    #finds the current directory
-    current_directory = os.getcwd()
-
-    #creates a file path to the current directory
-    filepath = os.path.join(current_directory, filename)
-
-    #checks if the file already exists
-    if not os.path.exists(filepath):
-
-        #if no, creates the path
-        with open(filepath, 'a'):
-            pass
-    else:
-
-        #else pass
-        pass
-
-    # Generate the image from the molecule
-    mol = Chem.MolFromSmiles(mol_smi)
-
-    # Adds the hydrogens to the molecule if specified
-    if show_Hs:
-        mol = Chem.AddHs(mol)
-
-    # Show the molecule in 3D if specified
-    if show_3D:
-        mol = AllChem.EmbedMolecule(mol)
-
-    image = Draw.MolToImage(mol)
-
-    # Save the image to a file
-    image.save(filepath)
-
-    # Creating a Bokeh figure to display the molecule
-    p = figure(width=350, height=350,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
-    p.image_url(url=[filepath], x=0, y=1, w=1, h=1)
-
-    # Hide grid lines and axes
-    p.xgrid.grid_line_color = None
-    p.ygrid.grid_line_color = None
-    p.xaxis.visible = False
-    p.yaxis.visible = False
-
-    return p
-
-def all_in_one(p1, p2, p3, p4):
-
-    #---------------------------------------------------------------------------------------------#
-    '''
-    all_in_one(p1,p2,p3, p4)
-    
-    Input: 3 bokeh plots
-            Usually used in this package:
-                    - p1 : bokeh double plot of mass spectrometry
-                    - p2 : image of the molecule
-                    - p3 : table of functional groups
-                    - p4 : buttons with info on the molecule
-    
-    Output: bokeh page with all 4 graphs well arranged
-
-    '''
-    #---------------------------------------------------------------------------------------------#
-    
-    #creates a layout in row with p3 and p4
-    layout1 = row(p3, p4)
-
-    #creates a layout in column with p2 and layout1
-    layout2 = column(p2, layout1)
-
-    #creates the final layout in row with layout1 and p1
-    layout = row(p1, layout2)
-
-    return layout
+    func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
-def atom_present_list(mol_smi):
-    #---------------------------------------------------------------------------------------------#
-    '''
-    atom_present_list(mol_smi)
-    
-    Input: molecule under MOL representation
-    
-    Output: list of atoms present in the molecule with their respective count
-    '''
-    #---------------------------------------------------------------------------------------------#
-    mol, list_atoms,list_atoms = Chem.MolFromSmiles(mol_smi),[],[]
-    for atom in mol.GetAtoms():
-        list_atoms.append(atom.GetSymbol())
-    for atom in mol.GetAtoms():
-        element = (f'{atom.GetSymbol()} : {list_atoms.count(atom.GetSymbol())}')   
-        if element not in list_atoms:
-            list_atoms.append(element)
-    return list_atoms
+    last = column(img_div, func_group_table)
+    final = row(double_graph, last)
+    return final
 
-def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
+#3
+def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
+    mol_smi_3D = mol_smi
+
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
             12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
             113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
             52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
             159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
             56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
@@ -952,15 +711,18 @@
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     
     mol = Chem.AddHs(mol_without_Hs)
 
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
-
+    
+    if not list_atoms:
+        return None
+    
     #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
 
     if 'H' in list_atoms:
 
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
 
@@ -1020,18 +782,18 @@
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
-                #removes any molecule who's probability is below 0.0001
+                #removes any molecule who's probability is below 0.00001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
@@ -1220,15 +982,15 @@
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
         'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': '*C(=O)[Oh1]','Ester': 'CC(=O)[Oh0]',
-        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
+        'Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl','Bromide': 'Br','Fluoride': 'F',
         'Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O','Proline': '[Nh1][Ch1*]C(=O)O',
         'Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*','Nitro': 'C[N+](=O)[O-]',
         'Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*','Azide': 'CNNN','Enol': 'C=C([Oh1])C',
         'Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]','Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C',
         'Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*','Phosphine': '*[Po0](*)*','Phosphate': '*OP(=O)(O)O',
         'Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
     }
@@ -1244,78 +1006,103 @@
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
                 if 'Ether' in functional_groups_contained:
                     functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Amide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amine')
-    if 'Carboxilic Acid' and 'Ester' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
     #initiate empty variables
     present_group_smarts = []    
     present_group_images_base64 = []
     
     #appends the smarts of the contained functional groups
     for i,j in functional_groups_smarts.items():
@@ -1342,27 +1129,14 @@
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
                 image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
                 #appends the image to an empty dictionnary
                 present_group_images_base64.append(image_base64)
-            elif x == '[N]':
-                mol2 = Chem.MolFromSmiles('CN')
-
-                #creates the image
-                image = Draw.MolToImage(mol2)
-
-                # Convert the image to base64 format
-                buffered = BytesIO()
-                image.save(buffered, format="PNG")
-                image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
-
-                #appends the image to an empty dictionnary
-                present_group_images_base64.append(image_base64)
             else:
                 #creates the image
                 image = Draw.MolToImage(mol)
 
                 # Convert the image to base64 format
                 buffered = BytesIO()
                 image.save(buffered, format="PNG")
@@ -1392,12 +1166,990 @@
     ]
     num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
-    last = column(img_div, func_group_table)
-    final = row(double_graph, last)
+    last = row(img_div, func_group_table)
+
+    # Generate 3D coordinates from SMILES string
+    mol_3D = Chem.MolFromSmiles(mol_smi_3D)
+    mol_3D = Chem.AddHs(mol_3D)  # Add hydrogens for better geometry optimization
+    AllChem.EmbedMolecule(mol_3D, randomSeed=42)  # Embed the molecule in 3D space
+    AllChem.MMFFOptimizeMolecule(mol_3D)  # Optimize the geometry using MMFF94 force field
+
+    # Create a temporary file to store the 
+    with tempfile.NamedTemporaryFile(delete=False) as tmp:
+        tmp.write(f"{mol_3D.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
+        for atom in mol_3D.GetAtoms():
+            pos = mol_3D.GetConformer().GetAtomPosition(atom.GetIdx())
+            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
+        tmp_path = tmp.name
+
+    # Create the MolGraph object
+    mg = MolGraph()
+    
+    # Read the data from the temporary file
+    mg.read_xyz(tmp_path)
+
+    # Create the Plotly figure object
+    fig = to_plotly_figure(mg)
+
+
+    # Converts all the graphs to pane to combine Bokeh and Plotly
+    fig_pane = pn.pane.Plotly(fig)
+
+    last_pane = pn.pane.Bokeh(last)
+
+    left_pane = pn.pane.Bokeh(double_graph)
+
+    # Creates the final plot
+    right_pane = pn.Column(fig_pane, last_pane)
+
+    total_plot_pane = pn.Row(left_pane, right_pane)
+
+    return total_plot_pane
+
+
+#functions that compose the main functions:
+
+def SMILEs_interpreter(mol_smi):
+    #---------------------------------------------------------------------------------------------#
+    '''
+    SMILEs_interpreter(mol_smi)
+
+    Input: molecule under SMILEs representation
+    
+    Output: molecule under MOL representation
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    #Checks that the SMILEs input is correct/allowed
+
+    mol_without_Hs = Chem.MolFromSmiles(mol_smi)
+
+    if mol_without_Hs is None:
+        raise ValueError('Invalid SMILEs representation')
+
+    mol = Chem.AddHs(mol_without_Hs)
+
+    return mol
+
+def molecule_list_generator(mol) -> list[str]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    molecule_list_generator(mol)
+    
+    Input: molecule under MOL representation
+    
+    Output: list containing the atomic symbol of each atom in the input molecule
+    '''
+    #---------------------------------------------------------------------------------------------#
+    if not mol:
+        raise ValueError('Enter a non-empty input')
+    list_atoms = []
+    for atom in mol.GetAtoms():
+        list_atoms.append(atom.GetSymbol())
+    return list_atoms
+
+def ionisation_method (list_atoms) -> list[str]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    ionisation_method (list_atoms)
+    
+    Input: list of atomic symbols of atoms in a given molecule
+    
+    Output: corrected list of atoms (i.e. list of atoms that enter spectrometry apparatus)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    '''In the case of ionisation by proton, we need to add a H+ ion, which is done in the following'''
+    if 'H' in list_atoms:
+
+        #Check that there is in fact a proton to remove
+        list_atoms.remove('H')
+    return list_atoms
+
+def sulphur_nitrogen_finder(list_atoms):
+    #---------------------------------------------------------------------------------------------#
+    '''
+    sulpher_nitrogen_finder(list_atoms)
+
+    Input: list of atoms in the molecule
+
+    Output: 2 booleans and 2 integers:
+    1. boolean that tells if the molecule contains an odd number of Nitrogen atoms
+    2. boolean that tells if the molecule contains an odd number of Sulphur atoms
+    3. number of Nitrogen atoms in the molecule (in case where there is an odd number)
+    4. number of Sulphur atoms in the molecule (in case where there is an odd number)
+    '''
+    #---------------------------------------------------------------------------------------------#
+    if not list_atoms:
+        raise ValueError("Enter a non-empty list")
+    if type(list_atoms) != list:
+        raise ValueError("Enter a list as argument")
+    
+
+    count_N = 0
+    has_N = False
+    if 'N' in list_atoms and list_atoms.count('N')%2 == 1:
+        has_N = True
+        count_N = list_atoms.count('N')
+    count_S = 0
+    has_S = False
+    if 'S' in list_atoms and list_atoms.count('S')%2 == 1:
+        has_S = True
+        count_S = list_atoms.count('S')
+    return has_N, has_S, count_N, count_S
+
+def main_function(list_atoms, imprecision_True_False) -> list[float]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    main_function(list_atoms)
+    
+    Input: list of atoms that enter the apparatus
+    
+    Output: two lists:
+    1. list of the masses (of individual molecules) of each possible combination of isotopes
+    2. list of the probabilities of apparation of each of the molecules 
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    if not list_atoms:
+        raise ValueError('Enter a valid input for the first argument')
+    if imprecision_True_False not in [True, False]:
+        raise ValueError('Enter a valid input for the second argument')
+    
+    render_imprecise_list = imprecision_True_False 
+    #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
+    
+    mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
+            136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
+            12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
+            113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
+            52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
+            159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
+            56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
+            75.9214, 73.92118, 72.92346, 71.92208, 69.92425, 2.014, 1.007825, 4.0026, 3.01603, 173.94005, 179.94655, 178.94582, 
+            177.9437, 176.94322, 203.97346, 201.97061, 200.97028, 199.9683, 198.96825, 197.96674, 195.9658, 164.93031, 126.90447, 
+            114.90388, 112.90406, 190.96059, 192.96292, 40.961826, 39.964, 38.963707, 77.9204, 85.910614, 83.91151, 82.91414, 
+            81.91348, 79.91638, 138.90634, 137.9071, 7.016003, 6.015121, 174.94077, 25.982594, 24.985838, 23.985043, 54.938046, 
+            94.90584, 93.90508, 91.90681, 99.90748, 97.9054, 96.90602, 95.90468, 15.000108, 14.003074, 22.989767, 92.90638, 142.9098, 
+            141.90771, 149.92088, 147.91689, 145.91312, 144.91257, 143.91008, 21.991383, 20.993843, 19.992435, 61.928345, 60.931057,
+            59.930786, 57.935345, 63.927967, 237.0482, 17.99916, 16.99913, 15.994915, 189.95844, 188.95813, 187.95586, 186.95573, 
+            185.95383, 183.95248, 191.96147, 30.973763, 206.97588, 205.97444, 203.97302, 207.97662, 109.90517, 107.90389, 105.90348, 
+            104.90508, 103.90403, 101.90563, 140.90765, 189.95992, 197.96786, 195.96492, 194.96477, 193.96266, 191.96101, 86.90919, 
+            84.9118, 186.95575, 184.95296, 102.9055, 103.905426, 101.90435, 100.90558, 99.90422, 98.90594, 97.90529, 95.9076, 
+            35.96708, 33.967865, 32.971455, 31.97207, 122.90421, 120.903824, 44.95591, 77.917305, 76.919914, 75.91921, 73.92248, 
+            81.916695, 79.91652, 29.97377, 28.976496, 27.976927, 153.92221, 151.91972, 149.91727, 148.91718, 147.91483, 146.9149, 
+            143.912, 123.90527, 121.90344, 119.9022, 118.90331, 117.90161, 116.902954, 115.90175, 114.90335, 113.90279, 111.90482, 
+            87.90562, 86.90888, 85.90926, 83.91343, 180.948, 179.94746, 158.92534, 125.90331, 124.904434, 123.902824, 122.904274, 
+            121.90305, 119.904045, 129.90623, 127.904465, 232.03806, 46.951763, 45.95263, 49.944794, 48.947872, 47.94795, 204.9744, 
+            202.97232, 168.93422, 50.943962, 49.947163, 185.95436, 183.95093, 182.95023, 181.9482, 179.9467, 173.93886, 172.9382, 
+            171.93637, 170.93633, 169.93475, 167.9339, 175.94257, 69.92532, 67.92484, 66.92713, 65.92603, 63.929146, 93.90647, 
+            91.90504, 90.90565, 89.9047, 95.90827]
+    
+
+    abundance = [0.48161000000000004, 0.51839, 1.0, 0.996, 0.00063, 0.00337, 1.0, 1.0, 0.8009999999999999, 0.19899999999999998, 
+                0.7170000000000001, 0.11230000000000001, 0.0785, 0.06593, 0.0242, 0.00101, 0.00106, 1.0, 1.0, 0.5069, 
+                0.49310000000000004, 0.011000000000000001, 0.9890000000000001, 4e-05, 0.02086, 0.00135, 0.00647, 0.96941, 0.00187, 
+                0.128, 0.1249, 0.0089, 0.07490000000000001, 0.2873, 0.1222, 0.2413, 0.11130000000000001, 0.8843000000000001, 0.0025, 
+                0.0019, 0.24230000000000002, 0.7576999999999999, 1.0, 0.02365, 0.095, 0.8379000000000001, 0.043449999999999996, 1.0, 
+                0.6917, 0.001, 0.0006, 0.282, 0.249, 0.255, 0.18899999999999997, 0.023399999999999997, 0.149, 0.268, 
+                0.22949999999999998, 0.336, 0.0161, 0.0014000000000000002, 0.522, 0.478, 1.0, 0.0028000000000000004, 0.021, 
+                0.059000000000000004, 0.39892000000000005, 0.60108, 0.2484, 0.1565, 0.2047, 0.14800000000000002, 0.0218, 0.002, 
+                0.2186, 0.07440000000000001, 0.3594, 0.07719999999999999, 0.2766, 0.21239999999999998, 0.00015, 0.99985, 1.0, 
+                1.37e-08, 0.0016200000000000001, 0.35100000000000003, 0.13629, 0.27297, 0.18606, 0.0687, 0.2986, 0.1318, 0.231, 
+                0.16870000000000002, 0.09970000000000001, 0.0015, 1.0, 1.0, 0.9570000000000001, 0.043, 0.373, 0.627, 0.067302, 
+                0.000117, 0.932581, 0.0034999999999999996, 0.17300000000000001, 0.57, 0.115, 0.11599999999999999, 0.0225, 0.999088, 
+                0.000902, 0.925, 0.075, 0.9741, 0.1101, 0.1, 0.7898999999999999, 1.0, 0.1592, 0.0925, 0.1484, 0.09630000000000001, 
+                0.2413, 0.0955, 0.1668, 0.0037, 0.9963, 1.0, 1.0, 0.12179999999999999, 0.2713, 0.0564, 0.0576, 0.17190000000000003,
+                0.083, 0.23800000000000002, 0.0925, 0.0027, 0.9048, 0.03634, 0.011399999999999999, 0.26222999999999996, 0.68077, 
+                0.009260000000000001, 1.0, 0.002, 0.0004, 0.9976, 0.264, 0.161, 0.133, 0.016, 0.0158, 0.0002, 0.41, 1.0, 0.221, 
+                0.24100000000000002, 0.013999999999999999, 0.524, 0.11720000000000001, 0.2646, 0.2733, 0.22329999999999997, 
+                0.1114, 0.0102, 1.0, 0.0001, 0.07200000000000001, 0.253, 0.33799999999999997, 0.32899999999999996, 0.0079, 0.2783, 
+                0.7217, 0.626, 0.374, 1.0, 0.18600000000000003, 0.316, 0.171, 0.126, 0.127, 0.018600000000000002, 0.0554, 0.0002, 
+                0.0421, 0.0075, 0.9501999999999999, 0.4264, 0.5736, 1.0, 0.2377, 0.07629999999999999, 0.09359999999999999, 0.0089, 
+                0.0874, 0.4961, 0.031, 0.0467, 0.9223, 0.22699999999999998, 0.267, 0.07400000000000001, 0.138, 0.113, 0.15, 0.031,
+                0.0579, 0.0463, 0.3259, 0.0858, 0.2422, 0.0768, 0.14529999999999998, 0.0036, 0.006500000000000001, 0.0097,
+                0.8258, 0.07, 0.0986, 0.005600000000000001, 0.9999800000000001, 0.00012, 1.0, 0.1893, 0.0712, 0.0479, 0.00905, 
+                0.0259, 0.00095, 0.3387, 0.317, 1.0, 0.073, 0.08, 0.054000000000000006, 0.055, 0.738, 0.7047599999999999, 0.29524, 
+                1.0, 0.9975, 0.0025, 0.28600000000000003, 0.307, 0.14279999999999998, 0.263, 0.0012, 0.318, 0.1612, 
+                0.21899999999999997, 0.14300000000000002, 0.0305, 0.0013, 0.127, 0.006, 0.188, 0.040999999999999995, 
+                0.27899999999999997, 0.486, 0.17379999999999998, 0.17149999999999999, 0.11220000000000001, 0.5145000000000001, 
+                0.027999999999999997]
+    
+
+    isotopes = ['Ag', 'Ag', 'Al', 'Ar', 'Ar', 'Ar', 'As', 'Au', 'B', 'B', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Ba', 'Be', 'Bi', 'Br', 
+                'Br', 'C', 'C', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Ca', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Cd', 'Ce', 'Ce', 'Ce', 'Ce', 
+                'Cl', 'Cl', 'Co', 'Cr', 'Cr', 'Cr', 'Cr', 'Cs', 'Cu', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Dy', 'Er', 'Er', 'Er', 
+                'Er', 'Er', 'Er', 'Eu', 'Eu', 'Fe ', 'Fe', 'Fe', 'Fe', 'Ga', 'Ga', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Gd', 'Ge', 
+                'Ge', 'Ge', 'Ge', 'Ge', 'H', 'H', 'He', 'He', 'Hf', 'Hf', 'Hf', 'Hf', 'Hf', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 'Hg', 
+                'Ho', 'I', 'In', 'In', 'Ir', 'Ir', 'K', 'K', 'K', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'Kr', 'La', 'La', 'Li', 'Li', 'Lu', 
+                'Mg', 'Mg', 'Mg', 'Mn', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'Mo', 'N', 'N', 'Na', 'Nb', 'Nd', 'Nd', 'Nd', 'Nd', 'Nd', 
+                'Nd', 'Nd', 'Ne', 'Ne', 'Ne', 'Ni', 'Ni', 'Ni', 'Ni', 'Ni', 'Np ', 'O', 'O', 'O', 'Os', 'Os', 'Os', 'Os', 'Os', 'Os', 
+                'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
+                'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
+                'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
+                'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
+                'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
+                'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
+    
+    #check for sulphur and nitrogen
+
+    has_N = False
+    count_N = 0
+    has_S = False
+    count_S = 0
+    if 'N' in list_atoms and list_atoms.count('N')%2 == 1:
+        has_N = True
+        count_N = list_atoms.count('N')
+    elif 'S' in list_atoms and list_atoms.count('S')%2 == 1:
+        has_S = True
+        count_S = list_atoms.count('S')
+
+
+    list_output = []
+    mass_copy = mass.copy()
+    abundance_copy = abundance.copy()
+    isotopes_copy = isotopes.copy()
+
+    for i in range (isotopes.count(list_atoms[0])):
+        
+        index = isotopes.index(list_atoms[0])
+        list_output.append([mass_copy[index],abundance_copy[index]])
+        mass_copy.pop(index)
+        abundance_copy.pop(index)
+        isotopes_copy.pop(index)
+
+    list_atoms = list_atoms[1:]
+
+    while len(list_atoms)>0:
+
+
+        #This runs over all atoms in molecule
+
+        list_output_new = []
+
+        for i in range (len(list_output)):
+
+
+            #This makes us run over all lists in list obtained before
+
+            mass_copy = mass.copy()
+            abundance_copy = abundance.copy()
+            isotopes_copy = isotopes.copy() 
+
+            for _ in range (isotopes.count(list_atoms[0])):
+
+
+                #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
+
+                index = isotopes.index(list_atoms[0])
+                new_mass = list_output[i][0] + mass_copy[index]
+                new_proba = list_output[i][1] * abundance_copy[index]
+
+
+                #removes any molecule who's probability is below 0.00001
+
+                if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
+                    if new_proba>0.00001:
+                        list_output_new.append([new_mass,new_proba])
+
+                else:
+                    list_output_new.append([new_mass,new_proba])
+
+                mass_copy.pop(index)
+                abundance_copy.pop(index)
+                isotopes_copy.pop(index)
+                
+        list_output = list_output_new
+        list_atoms.pop(0)
+
+
+
+    #Conversion of list_output (which is a list of lists) to a combination of two lists (x_axis & y_axis)
+
+    x_axis, y_axis = [],[]
+    x_axis_final, y_axis_final = [],[]
+    for j in range (len(list_output)):
+        x_axis.append(round(list_output[j][0],3)) # Adds rounded value (should help with Python-limitations that render a diff of magnitude 10^(-7) to combinatorics
+        
+        y_axis.append(list_output[j][1]) #Adds the true value
+        
+
+    #Compression of lists x_axis & y_axis into x_axis_final & y_axis_final so that peaks corresponding to same mass will be represented together 
+    
+    for j in range (len(x_axis)):
+            if x_axis.count(x_axis[j]) == 1:
+                x_axis_final.append(x_axis[j])
+                y_axis_final.append(y_axis[j])
+            elif x_axis_final.count(x_axis[j]) == 0:
+                x_axis_final.append(x_axis[j])
+                y_axis_final.append(y_axis[j])
+            else:
+                index = x_axis_final.index(x_axis[j])
+                y_axis_final[index] =y_axis_final[index] + y_axis[j]
+
+
+    #if there is any, add peaks corresponding to Sulphur/Nitrogen presence
+    maximum = max(y_axis_final)
+    maximum_2 = 0
+    for i in range (len(y_axis_final)):
+        if y_axis_final[i]>maximum_2 and y_axis_final[i]< maximum:
+            maximum_2 = y_axis_final[i]
+    index = y_axis_final.index(maximum_2)
+
+    if has_N:
+        x_axis_final.append(x_axis_final[index] - 0.006)  
+        y_axis_final.append(0.0035*count_N*maximum)  
+    
+    if has_S:
+        x_axis_final.append(x_axis_final[index]-0.004)  
+        y_axis_final.append(0.008*count_S*maximum)  
+
+    return x_axis_final, y_axis_final
+
+def peak_merger(x_in, y_in, apparatus_resolution) -> list[float]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    delta_function_plotter(x_in, y_in)
+    
+    Input: two lists + float:
+    1. ordered list of the masses (of individual molecules) of each possible combination of isotopes
+    2. ordered list of the probabilities of apparation of each of the molecules
+    3. apparatus precision (float representation of number which is the limit between two peaks above which they appear merged together)
+    
+    Output: two lists:
+    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
+    2. ordered list of the probabilities of apparation of each of the molecules
+    
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    if not x_in:
+        raise ValueError('Empty list entry')
+    if not y_in:
+        raise ValueError('Empty list entry')
+    if len(x_in) != len(y_in):
+        raise ValueError('Lists should be of the same size')
+
+    x_out, y_out = [],[]
+    while len(x_in)>1:
+        if x_in[0]>x_in[1]-apparatus_resolution:
+            y_in[1] = y_in[0] + y_in[1]
+            x_in[1] = (x_in[0] + x_in[1])/2
+            x_in.pop(0)
+            y_in.pop(0)
+        else:
+            x_out.append(x_in[0])
+            y_out.append(y_in[0])
+            x_in.pop(0)
+            y_in.pop(0)
+    x_out.append(x_in[0])
+    y_out.append(y_in[0])
+
+    return x_out, y_out
+
+def sulphur_nitrogen_adder(x_in, y_in, has_N, has_S, count_N, count_S) -> list[float]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    sulphur_nitrogen_adder(x_in, y_in, has_N, has_S, count_N, count_S)
+    
+    Input: two lists + 4 booleans:
+    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
+    2. ordered list of the probabilities of apparation of each of the molecules
+    3. boolean that tells if the molecule contains Nitrogen
+    4. boolean that tells if the molecule contains Sulphur
+    5. number of Nitrogen atoms in the molecule
+    6. number of Sulphur atoms in the molecule
+    
+    Output: two lists:
+    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
+    2. ordered list of the probabilities of apparation of each of the molecules
+    
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    if not x_in:
+        raise ValueError("Enter a non-empty list")
+    if not y_in:
+        raise ValueError("Enter a non-empty list")
+    if len(x_in) != len(y_in):
+        raise ValueError("The two lists must have the same length")
+    if has_N not in [True, False]:
+        raise ValueError("The third argument must be a boolean")
+    if has_S not in [True, False]:
+        raise ValueError("The fourth argument must be a boolean")
+    if count_N < 0:
+        raise ValueError("The fifth argument must be a positive integer")
+    if count_S < 0:
+        raise ValueError("The sixth argument must be a positive integer")
+    if type(count_N) != int:
+        raise ValueError("The fifth argument must be an integer")
+    if type(count_S) != int:
+        raise ValueError("The sixth argument must be an integer")
+    if x_in != sorted(x_in):
+        raise ValueError("The first list must be ordered")
+
+    maximum = max(y_in)
+
+    if has_N:
+        x_in.append(x_in[1] - 0.006)  
+        y_in.append(0.0035*count_N*maximum)  
+    
+    if has_S:
+        x_in.append(x_in[1]-0.004)  
+        y_in.append(0.008*count_S*maximum)
+
+
+    return x_in, y_in
+
+def peak_sorter(x_in, y_in) -> list[float]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    peak_sorter(x_in, y_in)
+    
+    Input: two lists:
+    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
+    2. ordered list of the probabilities of apparation of each of the molecules
+    
+    Output: two lists:
+    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
+    2. ordered list of the probabilities of apparation of each of the molecules
+    
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    '''
+    #---------------------------------------------------------------------------------------------#
+    
+    if not x_in:
+        raise ValueError('Empty list entry')
+    if not y_in:
+        raise ValueError('Empty list entry')
+    if len(x_in) != len(y_in):
+        raise ValueError('Lists should be of the same size')
+
+    x_out, y_out = [],[]
+    while len(x_in)>0:
+        min_x = min(x_in)
+        index_min = x_in.index(min_x)
+        x_out.append(min_x)
+        y_out.append(y_in[index_min])
+        x_in.pop(index_min)
+        y_in.pop(index_min)
+
+    return x_out, y_out
+
+def delta_function_plotter(x_in, y_in) -> list[float]:
+    #---------------------------------------------------------------------------------------------#
+    '''
+    delta_function_plotter(x_in, y_in)
+    
+    Input: two lists:
+    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered)
+    2. list of the probabilities of apparation of each of the molecules (ordered)
+    
+    Output: two lists:
+    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered) with values of 0 (y_axis) added on eiter side of the "peak"
+    2. list of the probabilities of apparation of each of the molecules (ordered)
+    
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+
+    if not x_in:
+        raise ValueError('Enter a valid input')
+    if not y_in:
+        raise ValueError('Enter a valid input')
+    if len(x_in) != len(y_in):
+        raise ValueError('Both entry should be of the same length')
+    
+    min_x , max_x = min(x_in), max(x_in)
+    
+
+    x_axis, y_axis = [min_x-0.5],[0]
+    for i in range (len(x_in)):
+        x_axis.append(x_in[i]-10**(-100))
+        x_axis.append(x_in[i])
+        x_axis.append(x_in[i]+10**(-100))
+        y_axis.append(0)
+        y_axis.append(y_in[i])
+        y_axis.append(0)
+
+    x_axis.append(max_x+1)
+    y_axis.append(0)
+
+    return x_axis, y_axis
+
+def double_plot(x_in,y_in):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    double_plot(x_in,y_in)
+    
+    Input: list of masses (x_in) and intensities (y_in)
+    
+    Output: 2 Bokeh graphs:
+            - One that shows the mass spectrum of the molecule to which the user can interact
+            -Another that is the same graph but shows where the user is zooming on the first graph
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    # tells where to put the graduation on the graph
+    if not x_in:
+        raise ValueError("Enter a non-empty list as first argument")
+    if not y_in:
+        raise ValueError("Enter a non-empty list as second argument")
+    if len(x_in) != len(y_in):
+        raise ValueError("The two lists must have the same length")
+    
+    ticked_peaks = []
+    for i in range(len(x_in)):
+        if y_in[i] > 0.0001:
+            ticked_peaks.append(x_in[i])
+
+    #creates the principal graph, mass spectrum of the molecule (interactive)
+
+    p1 = figure(width=700, title=f'Mass spectrum of molecule')
+    p1 = figure(x_axis_label = '[m/z]')
+    p1 = figure(y_axis_label = 'Abundance')
+    p1.xaxis.axis_label = "[m/z]"
+    p1.height = 500
+    p1.xaxis.ticker = FixedTicker(ticks=ticked_peaks)
+    p1.add_tools(WheelPanTool(dimension="height"))
+    p1.add_tools(WheelZoomTool(dimensions="height"))
+    p1.line(x_in, y_in, line_width=1)
+    p1.xaxis.major_label_orientation = "horizontal"
+
+     #creates the secondary graph, mass spectrum of the molecule (non-interactive)
+
+    p2 = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [Th]', y_axis_label='Intensity')
+    p2 = figure(width=300, title=f'Mass spectrum of molecule')
+    p2 = figure(toolbar_location=None)
+    p2.height = 300
+    p2.line(x_in, y_in, legend_label="Mass spectrum", line_width=1)
+
+    #creates a tool in order that the second graph shows where the zoom is on the first one
+
+    box = BoxAnnotation(left=0, right=0, bottom=0, top=0,
+    fill_alpha=0.1, line_color='red', fill_color='cornflowerblue')
+
+    jscode = """
+        box[%r] = cb_obj.start
+        box[%r] = cb_obj.end
+    """
+
+    xcb = CustomJS(args=dict(box=box), code=jscode % ('left', 'right'))
+    ycb = CustomJS(args=dict(box=box), code=jscode % ('bottom', 'top'))
+
+    p1.x_range.js_on_change('start', xcb)
+    p1.x_range.js_on_change('end', xcb)
+    p1.y_range.js_on_change('start', ycb)
+    p1.y_range.js_on_change('end', ycb)
+
+    # adds the functionnality to the second figure
+
+    p2.add_layout(box)
+
+    # creates a layout that displays the 2 graphs
+
+    layout = column(p1, p2)
+    print('here')
+    return layout
+
+def functional_group_finder(mol_smi):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    functional_group_finder(mol_smi)
+    
+    Input: molecule under SMILEs representation
+    
+    Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    if not mol_smi:
+        raise ValueError("Enter a non-empty string as argument")
+    # initiate variables
+    functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
+
+    # dictionnary of all the considered functional groups to check (some might be missing)
+
+    functional_groups_smarts = {'Alcohol': 'C[Oh1+0]','Aldehyde': 'C[Ch1]=O','Ketone': 'CC(=O)C','Carboxylic Acid': 'CC(=O)[Oh1]',
+        'Ester': 'CC(=O)[Oh0]','Ether': '*[Oh0]*','Amide': 'C(=O)N','Amine': '[C][N]','Nitrile': 'C#N','Chloride': 'Cl',
+        'Bromide': 'Br','Fluoride': 'F','Iodide': 'I','Alkene': 'C=C','Alkyne': 'C#C','Imine': 'C=N*','Amino acid': '[Nh2][Ch1*]C(=O)O',
+        'Proline': '[Nh1][Ch1*]C(=O)O','Thiol': '[Sh1]','Sulfide': '*[Sh0]*','Acyl Chloride': 'CC(=O)Cl','Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
+        'Nitro': 'C[N+](=O)[O-]','Enamine': 'C=C[Nh0]','Enamine2': 'C=C[Nh1]','Enamine3': 'C=C[Nh2]','Imide': 'C(=O)NC(=O)*',
+        'Azide': 'CNNN','Enol': 'C=C([Oh1])C','Hemiacetal': 'CC(O)(O)C','Carbonate': '[Oh0]C(=O)[Oh0]','Carbonate2': '[Oh1]C(=O)[Oh1]',
+        'Disulfide': 'CSSC','Sulfoxide': 'CS(=O)C','Sulfone': '*[So2](=O)(=O)*','Sulfonic acid': '*S(=O)(=O)[Oh1]','Thioester': 'C(=O)S*',
+        'Phosphine': '*[Po0](*)*','Phosphate': '*OP(=O)(O)O','Benzene': 'c1ccccc1','Peroxide':'C[Oh0][Oh0]C'
+    }
+
+    # check that the substructure from functional_groups_smarts are contained in mol_smi
+
+    for name, smarts in functional_groups_smarts.items():
+        if mol_in.HasSubstructMatch(Chem.MolFromSmarts(smarts)):
+            for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
+                functional_groups_contained.append(name)
+
+    # exceptions for conflicts during the iteration of functional groups
+    for functional_group in functional_groups_contained:
+        if 'Ester' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif functional_group == 'Carboxylic Acid':
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+        elif 'Phosphate' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Thioester' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+        elif 'Sulfonic acid' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+        elif 'Sulfoxide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+        elif 'Acyl Chloride' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+        elif 'Anhydride' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
+        elif 'Enamine2' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
+        elif 'Enamine3' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                functional_groups_contained.append('Enamine')
+        elif 'Imide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+        elif 'Enol' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+        elif 'Hemiacetal' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+        elif 'Carbonate2' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
+        elif 'Disulfide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+        elif 'Peroxide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+    
+    
+    return functional_groups_contained
+
+def functional_group_display(contained_functional_groups):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    functional_group_display(contained_functional_groups)
+    
+    Input: list of all contained functional groups in the molecule
+
+    Output: bokeh table with the contained functional groups and their image
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    #dictionnary with functional groups and associated SMARTs
+    functional_groups_smarts = {
+        'Alcohol': 'C[Oh1+0]',
+        'Aldehyde': 'C[Ch1]=O',
+        'Ketone': 'CC(=O)C',
+        'Carboxylic Acid': 'CC(=O)[Oh1]',
+        'Ester': 'CC(=O)[Oh0]',
+        'Ether': '*[Oh0]*',
+        'Amide': 'C(=O)N',
+        'Amine': '[C][N]',
+        'Nitrile': 'C#N',
+        'Chloride': 'Cl',
+        'Bromide': 'Br',
+        'Fluoride': 'F',
+        'Iodide': 'I',
+        'Alkene': 'C=C',
+        'Alkyne': 'C#C',
+        'Imine': 'C=N*',
+        'Amino acid': '[Nh2][Ch1*]C(=O)O',
+        'Proline': '[Nh1][Ch1*]C(=O)O',
+        'Thiol': '[Sh1]',
+        'Sulfide': '*[Sh0]*',
+        'Acyl Chloride': 'CC(=O)Cl',
+        'Anhydride': '*[Ch0](=O)O[Ch0](=O)*',
+        'Nitro': 'C[N+](=O)[O-]',
+        'Enamine': 'C=C[Nh0]',
+        'Enamine2': 'C=C[Nh1]',
+        'Enamine3': 'C=C[Nh2]',
+        'Imide': 'C(=O)NC(=O)*',
+        'Azide': 'CNNN',
+        'Enol': 'C=C([Oh1])C',
+        'Hemiacetal': 'CC(O)(O)C',
+        'Carbonate': '[Oh0]C(=O)[Oh0]',
+        'Carbonate2': '[Oh1]C(=O)[Oh1]',
+        'Disulfide': 'CSSC',
+        'Sulfoxide': 'CS(=O)C',
+        'Sulfone': '*[So2](=O)(=O)*',
+        'Sulfonic acid': '*S(=O)(=O)[Oh1]',
+        'Thioester': 'C(=O)S*',
+        'Phosphine': '*[Po0](*)*',
+        'Phosphate': '*OP(=O)(O)O',
+        'Benzene': 'c1ccccc1',
+        'Peroxide':'C[Oh0][Oh0]C'
+    }
+
+    #initiate empty variables
+    present_group_smarts = []    
+    present_group_images_base64 = []
+    
+    #appends the smarts of the contained functional groups
+    for i,j in functional_groups_smarts.items():
+        for x in contained_functional_groups:
+            if x == i:
+                present_group_smarts.append(j)
+
+    #converts the smarts to images in base64 format
+    for x in present_group_smarts:
+
+        #converts SMARTs to SMILEs for the images to be nicer
+        mol_x = Chem.MolFromSmarts(x)
+        mol_smi = Chem.MolToSmiles(mol_x)
+        mol = Chem.MolFromSmiles(mol_smi)
+
+        if mol:
+
+            #creates the image
+            image = Draw.MolToImage(mol)
+
+            # Convert the image to base64 format
+            buffered = BytesIO()
+            image.save(buffered, format="PNG")
+            image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+            #appends the image to an empty dictionnary
+            present_group_images_base64.append(image_base64)
+
+    #creates a dictionnary that links the name of the functional group to its image
+    data = dict(
+        groups=contained_functional_groups,
+        images=present_group_images_base64
+    )
+    source = ColumnDataSource(data)
+
+    #template for the bokeh table that read the base64 format 
+    template = """
+    <div>
+        <img src="data:image/png;base64, <%= value %>" style="width:50px;height:50px;">
+    </div>
+    """
+
+    # initiallizing the bokeh figure using the previous template for each functional group
+    columns = [
+        TableColumn(field="groups", title="Functional Groups"),
+        TableColumn(field="images", title="Images", width=200, formatter=HTMLTemplateFormatter(template=template))
+    ]
+    num_groups = len(contained_functional_groups)
+
+    table_height = min(200 + num_groups * 60, 800)
+
+    data_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
+
+    return data_table
+
+def mol_web_show(mol_smi, show_Hs=False, show_3D = False):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    mol_web_show(mol_smi, show_Hs=False, show_3D = False)
+    
+    Input: SMILEs of a molecule. Also specify if want the function to show the hydrogens explicitely or the 3D
+    
+    Output: image of the molecule as a bokeh plot
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    # name of the file name to create
+    filename = 'molecule_image.png'
+
+    #finds the current directory
+    current_directory = os.getcwd()
+
+    #creates a file path to the current directory
+    filepath = os.path.join(current_directory, filename)
+
+    #checks if the file already exists
+    if not os.path.exists(filepath):
+
+        #if no, creates the path
+        with open(filepath, 'a'):
+            pass
+    else:
+
+        #else pass
+        pass
+
+    # Generate the image from the molecule
+    mol = Chem.MolFromSmiles(mol_smi)
+
+    # Adds the hydrogens to the molecule if specified
+    if show_Hs:
+        mol = Chem.AddHs(mol)
+
+    # Show the molecule in 3D if specified
+    if show_3D:
+        mol = AllChem.EmbedMolecule(mol)
+
+    image = Draw.MolToImage(mol)
+
+    # Save the image to a file
+    image.save(filepath)
+
+    # Creating a Bokeh figure to display the molecule
+    p = figure(width=350, height=350,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
+    p.image_url(url=[filepath], x=0, y=1, w=1, h=1)
+
+    # Hide grid lines and axes
+    p.xgrid.grid_line_color = None
+    p.ygrid.grid_line_color = None
+    p.xaxis.visible = False
+    p.yaxis.visible = False
+
+    return p
+ 
+def all_in_one(p1, p2, p3, p4):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    all_in_one(p1,p2,p3, p4)
+    
+    Input: 3 bokeh plots
+            Usually used in this package:
+                    - p1 : bokeh double plot of mass spectrometry
+                    - p2 : image of the molecule
+                    - p3 : table of functional groups
+                    - p4 : buttons with info on the molecule
+    
+    Output: bokeh page with all 4 graphs well arranged
+
+    '''
+    #---------------------------------------------------------------------------------------------#
+    
+    if not p1:
+        raise ValueError("Enter a non-empty plot")
+    if not p2:
+        raise ValueError("Enter a non-empty plot")
+    if not p3:
+        raise ValueError("Enter a non-empty plot")
+    if not p4:
+        raise ValueError("Enter a non-empty plot")
+    
+    #creates a layout in row with p3 and p4
+    layout1 = row(p3, p4)
+
+    #creates a layout in column with p2 and layout1
+    layout2 = column(p2, layout1)
+
+    #creates the final layout in row with layout1 and p1
+    layout = row(p1, layout2)
+
+    return layout
+
+def smiles_to_3D_plot(mol_smi):
+
+     #---------------------------------------------------------------------------------------------#
+    '''
+    smiles_to_3D_plot(smiles)
+    
+    Input: molecule is a SMILEs format
+
+    Output: panel graph of the molecule in 3D and interactive
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    # Generate 3D coordinates from SMILES string
+    mol2 = Chem.MolFromSmiles(mol_smi)
+    mol2 = Chem.AddHs(mol2)  # Add hydrogens for better geometry optimization
+    AllChem.EmbedMolecule(mol2, randomSeed=42)  # Embed the molecule in 3D space
+    AllChem.MMFFOptimizeMolecule(mol2)  # Optimize the geometry using MMFF94 force field
+
+    # Create a temporary file to store the 
+    with tempfile.NamedTemporaryFile(delete=False) as tmp:
+        tmp.write(f"{mol2.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
+        for atom in mol2.GetAtoms():
+            pos = mol2.GetConformer().GetAtomPosition(atom.GetIdx())
+            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
+        tmp_path = tmp.name
+
+    # Create the MolGraph object
+    mg = MolGraph()
+    
+    # Read the data from the temporary file
+    mg.read_xyz(tmp_path)
+
+    # Create the Plotly figure object
+    fig = to_plotly_figure(mg)
+
+    return fig
+
+
+
+
 
-    return final
```

### Comparing `massivechem-4.1/tests/tests/double_plot_tests.py` & `massivechem-4.3/test/test_double_plot.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     Output: 2 Bokeh graphs:
             - One that shows the mass spectrum of the molecule to which the user can interact
             -Another that is the same graph but shows where the user is zooming on the first graph
     '''
     #---------------------------------------------------------------------------------------------#
 
     # tells where to put the graduation on the graph
-
+    if not x_in:
+        raise ValueError("Enter a non-empty list as first argument")
+    if not y_in:
+        raise ValueError("Enter a non-empty list as second argument")
+    if len(x_in) != len(y_in):
+        raise ValueError("The two lists must have the same length")
+    
     ticked_peaks = []
     for i in range(len(x_in)):
         if y_in[i] > 0.0001:
             ticked_peaks.append(x_in[i])
 
     #creates the principal graph, mass spectrum of the molecule (interactive)
 
@@ -71,47 +77,68 @@
 
     # creates a layout that displays the 2 graphs
 
     layout = column(p1, p2)
     print('here')
     return layout
 
-
 import unittest
 
 class TestDoublePlot(unittest.TestCase):
     def test_double_plot(self):
-        # Test the function with sample data
+
         x_in = [100, 200, 300, 400, 500]
         y_in = [0.1, 0.2, 0.3, 0.4, 0.5]
+
         layout = double_plot(x_in, y_in)
+
         self.assertIsNotNone(layout)
         self.assertEqual(len(layout.children), 2)  # Check if there are two plots in the layout
 
     def test_double_plot_empty_data(self):
-        # Test the function with empty data
+
         x_in = []
         y_in = []
-        layout = double_plot(x_in, y_in)
-        self.assertIsNotNone(layout)
-        self.assertEqual(len(layout.children), 2)  # Check if there are two plots in the layout
+
+        with self.assertRaises(ValueError):
+            double_plot(x_in, y_in)
+    
+    def test_double_plot_1_empty_data(self):
+
+        x_in = [1]
+        y_in = []
+
+        with self.assertRaises(ValueError):
+            double_plot(x_in, y_in)
+    
+    def test_double_plot_1_empty_data_2(self):
+
+        x_in = []
+        y_in = [1]
+
+        with self.assertRaises(ValueError):
+            double_plot(x_in, y_in)
 
     def test_double_plot_single_point(self):
-        # Test the function with a single point
+        
         x_in = [100]
         y_in = [0.1]
+
         layout = double_plot(x_in, y_in)
+
         self.assertIsNotNone(layout)
         self.assertEqual(len(layout.children), 2)  # Check if there are two plots in the layout
 
     def test_double_plot_identical_data(self):
-        # Test the function with identical x and y data
+        
         x_in = [100, 200, 300, 400, 500]
         y_in = [0.1, 0.1, 0.1, 0.1, 0.1]
+
         layout = double_plot(x_in, y_in)
+
         self.assertIsNotNone(layout)
         self.assertEqual(len(layout.children), 2)  # Check if there are two plots in the layout
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-4.1/tests/tests/functional_group_finder_tests.py` & `massivechem-4.3/test/test_functional_group_finder.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,17 +8,23 @@
     
     Input: molecule under SMILEs representation
     
     Output: list containing every functionl group contained (if a functional group is contained twice in the molecule, it will appear twice in this list)
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError("Enter a non-empty string as argument")
     # initiate variables
     functional_groups_contained, mol_in = [], Chem.MolFromSmiles(mol_smi)
 
+
+    if not mol_in:
+        raise ValueError('Incorrect SMILEs input')
+    
     # dictionnary of all the considered functional groups to check (some might be missing)
 
     functional_groups_smarts = {
         'Alcohol': 'C[Oh1+0]',
         'Aldehyde': 'C[Ch1]=O',
         'Ketone': 'CC(=O)C',
         'Carboxylic Acid': 'CC(=O)[Oh1]',
@@ -68,108 +74,156 @@
             for _ in range(len(mol_in.GetSubstructMatches(Chem.MolFromSmarts(smarts)))):
                 functional_groups_contained.append(name)
 
     # exceptions for conflicts during the iteration of functional groups
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+
     
     
     return functional_groups_contained
 
 import unittest
 
 class TestFunctionalGroupFinder(unittest.TestCase):
     def test_functional_group_finder_empty(self):
-        # Test the function with an empty SMILES string
-        mol_smi = ""
-        functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, [])
+
+        smiles = ""
+
+        with self.assertRaises(ValueError):
+            functional_group_finder(smiles)
+
+    def test_functional_group_finder_incorrect_smiles(self):
+
+        smiles = "CCXrtCC"
+
+        with self.assertRaises(ValueError):
+            functional_group_finder(smiles)
 
     def test_functional_group_finder_no_functional_groups(self):
-        # Test the function with a molecule without any functional groups
+        
         mol_smi = "CC"
+
         functional_groups = functional_group_finder(mol_smi)
+
         self.assertEqual(functional_groups, [])
 
     def test_functional_group_finder_single_functional_group(self):
-        # Test the function with a molecule containing a single functional group
+        
         mol_smi = "CCO"
+
         functional_groups = functional_group_finder(mol_smi)
+
         self.assertEqual(functional_groups, ['Alcohol'])
 
     def test_functional_group_finder_multiple_functional_groups(self):
-        # Test the function with a molecule containing multiple functional groups
+        
         mol_smi = "CCOCC(=O)OC"
+
         functional_groups = functional_group_finder(mol_smi)
+
         self.assertEqual(functional_groups, ['Ester', 'Ether'])
 
     def test_functional_group_finder_duplicate_functional_groups(self):
-        # Test the function with a molecule containing duplicate functional groups
-        mol_smi = "CCOCC(=O)OCCC(=O)OC(=O)C"
+        
+        mol_smi = "NCCCOCC1CC(C=O)CC(CCC=NC)C1"
+
         functional_groups = functional_group_finder(mol_smi)
-        self.assertEqual(functional_groups, ['Ester', 'Ether', 'Anhydride'])
+
+        self.assertEqual(functional_groups, ['Aldehyde', 'Ether', 'Amine', 'Amine', 'Imine'])
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-4.1/tests/tests/mol_web_show_tests.py` & `massivechem-4.3/test/test_mol_web_show.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,76 +5,117 @@
 import base64
 
 from bokeh.plotting import show
 from bokeh.io import show
 from bokeh.models import Div
 
 
-def mol_web_show(mol_smi, show_Hs=False, show_3D = False):
+def mol_web_show(mol_smi):
 
     #---------------------------------------------------------------------------------------------#
     '''
-    mol_web_show(mol_smi, show_Hs=False, show_3D = False)
+    mol_web_show(mol_smi)
     
-    Input: SMILEs of a molecule. Also specify if want the function to show the hydrogens explicitely or the 3D
+    Input: SMILEs of a molecule
     
     Output: image of the molecule as a bokeh plot
     '''
     #---------------------------------------------------------------------------------------------#
 
+    if not mol_smi:
+        raise ValueError('Incorrect SMILEs input')
+    
     # Generate the image from the molecule
     mol = Chem.MolFromSmiles(mol_smi)
 
-    # Show the molecule in 3D if specified
-    if show_3D:
-        mol = Chem.AddHs(mol)
-        AllChem.EmbedMolecule(mol)
-    
-    # Adds the hydrogens to the molecule if specified
-    if show_Hs:
-        mol = Chem.AddHs(mol)
+    if mol is None:
+        raise ValueError('Incorrect SMILEs input')
 
     #Draws the image
     image = Draw.MolToImage(mol)
 
     #stocks the image in a base64 format
     buffered = BytesIO()
     image.save(buffered, format="PNG")
     image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
     image_url = f"data:image/png;base64,{image_base64}"
 
     # Create a Div element to display the image
     img_div = Div(text=f'<img src="{image_url}" style="width:350px;height:350px;">')
    
     return img_div
-
+  
 import unittest
-
+from rdkit import Chem
+from rdkit.Chem import AllChem, Draw
+from io import BytesIO
+import base64
+from bokeh.models import Div
 
 class TestMolWebShow(unittest.TestCase):
 
-    def test_mol_web_show_no_Hs_no_3D(self):
-        # Test with no explicit hydrogens and no 3D
-        mol_smi = "CCO"  # Example SMILES string
-        result = mol_web_show(mol_smi, show_Hs=False, show_3D=False)
-        self.assertIsInstance(result, Div)  # Check if the output is a Div element
-
-    def test_mol_web_show_with_Hs_no_3D(self):
-        # Test with explicit hydrogens but no 3D
-        mol_smi = "CCO"  # Example SMILES string
-        result = mol_web_show(mol_smi, show_Hs=True, show_3D=False)
-        self.assertIsInstance(result, Div)  # Check if the output is a Div element
-
-    def test_mol_web_show_no_Hs_with_3D(self):
-        # Test with no explicit hydrogens but with 3D
-        mol_smi = "CCO"  # Example SMILES string
-        result = mol_web_show(mol_smi, show_Hs=False, show_3D=True)
-        self.assertIsInstance(result, Div)  # Check if the output is a Div element
-
-    def test_mol_web_show_with_Hs_with_3D(self):
-        # Test with explicit hydrogens and with 3D
-        mol_smi = "CCO"  # Example SMILES string
-        result = mol_web_show(mol_smi, show_Hs=True, show_3D=True)
-        self.assertIsInstance(result, Div)  # Check if the output is a Div element
+    def test_default_parameters(self):
+
+        mol_smi = "CCO"
+         
+        result = mol_web_show(mol_smi)
+
+        self.assertIsInstance(result, Div)
+
+    def test_small_smiles(self):
+        mol_smi = "CCO"  
+
+        result = mol_web_show(mol_smi)
+
+        self.assertIsInstance(result, Div)
+
+        mol = Chem.MolFromSmiles(mol_smi)
+        
+        image = Draw.MolToImage(mol)
+        buffered = BytesIO()
+        image.save(buffered, format="PNG")
+        image_base64_with_hs = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+        self.assertIn(image_base64_with_hs[:100], result.text)  
+
+    def test_invalid_smiles(self):
+
+        mol_smi = "InvalidSMILES"
+
+        with self.assertRaises(ValueError):
+            mol_web_show(mol_smi)
+
+    def test_empty_smiles(self):
+
+        mol_smi = ""
+
+        with self.assertRaises(ValueError):
+            mol_web_show(mol_smi)
+
+    def test_complex_smiles(self):
+
+        mol_smi = "C1=CC=C(C=C1)C2=CC=CC=C2" 
+
+        result = mol_web_show(mol_smi)
+
+        self.assertIsInstance(result, Div)
+    
+    def test_benzene(self):
+
+        mol_smi = "C1=CC=CC=C1" 
+
+        result = mol_web_show(mol_smi)
+
+        self.assertIsInstance(result, Div)
+
+        mol = Chem.MolFromSmiles(mol_smi)
+
+        image = Draw.MolToImage(mol)
+        buffered = BytesIO()
+        image.save(buffered, format="PNG")
+        image_base64_with_hs = base64.b64encode(buffered.getvalue()).decode("utf-8")
+
+        self.assertIn(image_base64_with_hs[:100], result.text) 
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `massivechem-4.1/tests/tests/peak_merger_tests.py` & `massivechem-4.3/scripts/delta_function_plotter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-def peak_merger(x_in, y_in, apparatus_resolution) -> list[float]:
+def delta_function_plotter(x_in, y_in) -> list[float]:
     #---------------------------------------------------------------------------------------------#
     '''
     delta_function_plotter(x_in, y_in)
     
-    Input: two lists + float:
-    1. ordered list of the masses (of individual molecules) of each possible combination of isotopes
-    2. ordered list of the probabilities of apparation of each of the molecules
-    3. apparatus precision (float representation of number which is the limit between two peaks above which they appear merged together)
+    Input: two lists:
+    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered)
+    2. list of the probabilities of apparation of each of the molecules (ordered)
     
     Output: two lists:
-    1. ordered list of the masses with values on y merged together if peaks within precision of apparatus
-    2. ordered list of the probabilities of apparation of each of the molecules
+    1. list of the masses (of individual molecules) of each possible combination of isotopes (ordered) with values of 0 (y_axis) added on eiter side of the "peak"
+    2. list of the probabilities of apparation of each of the molecules (ordered)
     
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
 
-    x_out, y_out = [],[]
-    while len(x_in)>1:
-        if x_in[0]>x_in[1]-apparatus_resolution:
-            y_in[1] = y_in[0] + y_in[1]
-            x_in[1] = (x_in[0] + x_in[1])/2
-            x_in.pop(0)
-            y_in.pop(0)
-        else:
-            x_out.append(x_in[0])
-            y_out.append(y_in[0])
-            x_in.pop(0)
-            y_in.pop(0)
-    x_out.append(x_in[0])
-    y_out.append(y_in[0])
 
-    return x_out, y_out
+    if not x_in:
+        raise ValueError('Enter a valid input')
+    if not y_in:
+        raise ValueError('Enter a valid input')
+    if len(x_in) != len(y_in):
+        raise ValueError('Both entry should be of the same length')
+    
+    min_x , max_x = min(x_in), max(x_in)
+    
+
+    x_axis, y_axis = [min_x-0.5],[0]
+    for i in range (len(x_in)):
+        x_axis.append(x_in[i]-10**(-100))
+        x_axis.append(x_in[i])
+        x_axis.append(x_in[i]+10**(-100))
+        y_axis.append(0)
+        y_axis.append(y_in[i])
+        y_axis.append(0)
+
+    x_axis.append(max_x+1)
+    y_axis.append(0)
+
+    return x_axis, y_axis
```

### Comparing `massivechem-4.1/tests/tests/spectrum_tests.py` & `massivechem-4.3/scripts/spectrum_3D.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,19 +7,29 @@
 from bokeh.io import show
 from bokeh.models import ColumnDataSource, HTMLTemplateFormatter, WheelPanTool, WheelZoomTool, BoxAnnotation, CustomJS, Div
 from bokeh.models.widgets import DataTable, TableColumn
 
 import base64
 from io import BytesIO
 
+import panel as pn
+import xyz2graph
+import tempfile
+from xyz2graph import MolGraph, to_plotly_figure
 
-def spectrum(mol_smi, imprecision_True_False, apparatus_resolution):
+
+
+
+
+def spectrum_3D(mol_smi, imprecision_True_False, apparatus_resolution):
 
     #lists of the data to facilitise the pip-installability of the package
 
+    mol_smi_3D = mol_smi
+
     mass = [108.904755, 106.90509, 26.981539, 39.962383, 37.96273, 35.967545, 74.92159, 196.96654, 11.009305, 10.012937, 137.90523, 
             136.9058, 135.90456, 134.90567, 133.90448, 131.90504, 129.90628, 9.012182, 208.98038, 78.918335, 80.91629, 13.003355, 
             12.0, 45.95369, 43.95548, 42.958767, 41.95862, 39.96259, 47.952534, 110.90418, 109.90301, 107.90418, 115.904755, 
             113.90336, 112.9044, 111.902756, 141.90924, 139.90543, 137.90599, 135.90714, 36.965904, 34.968853, 58.933197, 53.93888, 
             52.94065, 51.94051, 49.946045, 132.90543, 62.939598, 157.92441, 155.92528, 163.92917, 162.92873, 161.92679, 160.92693, 
             159.92519, 169.93546, 167.93237, 166.93205, 165.93028, 163.9292, 161.92877, 152.92122, 150.91985, 18.998404, 57.933277, 
             56.935394, 53.939613, 70.9247, 68.92558, 157.9241, 156.92395, 155.92212, 154.92262, 153.92087, 151.91978, 159.92705, 
@@ -84,26 +94,31 @@
                 'Os', 'P', 'Pb', 'Pb', 'Pb', 'Pb', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pd', 'Pr', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 'Pt', 
                 'Rb ', 'Rb', 'Re', 'Re', 'Rh', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'Ru', 'S', 'S', 'S', 'S', 'Sb', 'Sb', 'Sc', 'Se', 
                 'Se', 'Se', 'Se', 'Se', 'Se', 'Si', 'Si', 'Si', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sm', 'Sn', 'Sn', 'Sn', 'Sn', 
                 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sn', 'Sr', 'Sr', 'Sr', 'Sr', 'Ta', 'Ta', 'Tb', 'Te', 'Te', 'Te', 'Te', 'Te', 'Te', 
                 'Te', 'Te', 'Th', 'Ti', 'Ti', 'Ti', 'Ti', 'Ti', 'TI', 'TI', 'Tm', 'V', 'V', 'W', 'W', 'W', 'W', 'W', 'Yb', 'Yb', 'Yb', 
                 'Yb', 'Yb', 'Yb', 'Yb', 'Zn', 'Zn', 'Zn', 'Zn', 'Zn', 'Zr', 'Zr', 'Zr', 'Zr', 'Zr ']
     
+    if not mol_smi:
+        raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
 
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     if mol_without_Hs is None:
         raise ValueError('\nInvalid SMILEs enterred.\nPlease enter a different SMILEs.')
     
     mol = Chem.AddHs(mol_without_Hs)
 
     list_atoms = []
     for atom in mol.GetAtoms():
         list_atoms.append(atom.GetSymbol())
-
+    
+    if not list_atoms:
+        return None
+    
     #In the case of ionisation by proton, we need to add a H+ ion, which is done in the following
 
     if 'H' in list_atoms:
 
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
 
@@ -163,18 +178,18 @@
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
 
 
-                #removes any molecule who's probability is below 0.0001
+                #removes any molecule who's probability is below 0.00001
 
                 if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
-                    if new_proba>0.0001:
+                    if new_proba>0.00001:
                         list_output_new.append([new_mass,new_proba])
 
                 else:
                     list_output_new.append([new_mass,new_proba])
 
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
@@ -387,75 +402,103 @@
     for functional_group in functional_groups_contained:
         if 'Ester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
                 if 'Ether' in functional_groups_contained:
                     functional_groups_contained.remove('Ether')
         elif functional_group == 'Carboxylic Acid':
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-        elif 'Ester' == functional_group:
-            for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Phosphate' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
         elif 'Thioester' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfonic acid' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Sulfoxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Acyl Chloride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Chloride')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Anhydride' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.remove('Ester')
-                functional_groups_contained.append('Ether')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ester' in functional_groups_contained:
+                    functional_groups_contained.remove('Ester')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.append('Ether')
         elif 'Enamine2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine2')
-                functional_groups_contained.append('Enamine')
+                if 'Enamine2' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine2')
+                if 'Enamine' in functional_groups_contained:
+                    functional_groups_contained.append('Enamine')
         elif 'Enamine3' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Enamine3')
-                functional_groups_contained.remove('Amine')
+                if 'Enamine3' in functional_groups_contained:
+                    functional_groups_contained.remove('Enamine3')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
                 functional_groups_contained.append('Enamine')
         elif 'Imide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Amide')
-                functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
+                if 'Amide' in functional_groups_contained:
+                    functional_groups_contained.remove('Amide')
         elif 'Enol' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alkene')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alkene' in functional_groups_contained:
+                    functional_groups_contained.remove('Alkene')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Hemiacetal' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
         elif 'Carbonate2' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Alcohol')
-                functional_groups_contained.remove('Carbonate2')
-                functional_groups_contained.append('Carbonate')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Alcohol' in functional_groups_contained:
+                    functional_groups_contained.remove('Alcohol')
+                if 'Carbonate2' in functional_groups_contained:
+                    functional_groups_contained.remove('Carbonate2')
+                if 'Carbonate' in functional_groups_contained:
+                    functional_groups_contained.append('Carbonate')
         elif 'Disulfide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Sulfide')
-                functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
+                if 'Sulfide' in functional_groups_contained:
+                    functional_groups_contained.remove('Sulfide')
         elif 'Peroxide' == functional_group:
             for _ in range (functional_groups_contained.count(functional_group)):
-                functional_groups_contained.remove('Ether')
-                functional_groups_contained.remove('Ether')
-    if 'Carboxilic Acid' and 'Ester' in functional_groups_contained:
-        functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+                if 'Ether' in functional_groups_contained:
+                    functional_groups_contained.remove('Ether')
+        elif 'Amide' == functional_group:
+            for _ in range (functional_groups_contained.count(functional_group)):
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
+                if 'Amine' in functional_groups_contained:
+                    functional_groups_contained.remove('Amine')
 
     #initiate empty variables
     present_group_smarts = []    
     present_group_images_base64 = []
     
     #appends the smarts of the contained functional groups
     for i,j in functional_groups_smarts.items():
@@ -519,49 +562,51 @@
     ]
     num_groups = len(functional_groups_contained)
 
     table_height = min(200 + num_groups * 60, 800)
 
     func_group_table = DataTable(source=source, columns=columns, width=250, height=table_height, row_height=60)
 
-    last = column(img_div, func_group_table)
-    final = row(double_graph, last)
-    return final
+    last = row(img_div, func_group_table)
 
-#show(spectrum('CCCXCCC', True, 0.01))
+    # Generate 3D coordinates from SMILES string
+    mol_3D = Chem.MolFromSmiles(mol_smi_3D)
+    mol_3D = Chem.AddHs(mol_3D)  # Add hydrogens for better geometry optimization
+    AllChem.EmbedMolecule(mol_3D, randomSeed=42)  # Embed the molecule in 3D space
+    AllChem.MMFFOptimizeMolecule(mol_3D)  # Optimize the geometry using MMFF94 force field
 
+    # Create a temporary file to store the 
+    with tempfile.NamedTemporaryFile(delete=False) as tmp:
+        tmp.write(f"{mol_3D.GetNumAtoms()}\n\n".encode('utf-8'))  # Write number of atoms
+        for atom in mol_3D.GetAtoms():
+            pos = mol_3D.GetConformer().GetAtomPosition(atom.GetIdx())
+            tmp.write(f"{atom.GetSymbol()} {pos.x} {pos.y} {pos.z}\n".encode('utf-8'))
+        tmp_path = tmp.name
 
-import unittest
-from rdkit import Chem
-from bokeh.plotting import figure, Figure
+    # Create the MolGraph object
+    mg = MolGraph()
+    
+    # Read the data from the temporary file
+    mg.read_xyz(tmp_path)
 
+    # Create the Plotly figure object
+    fig = to_plotly_figure(mg)
+
+
+    # Converts all the graphs to pane to combine Bokeh and Plotly
+    fig_pane = pn.pane.Plotly(fig)
+
+    last_pane = pn.pane.Bokeh(last)
+
+    left_pane = pn.pane.Bokeh(double_graph)
+
+    # Creates the final plot
+    right_pane = pn.Column(fig_pane, last_pane)
+
+    total_plot_pane = pn.Row(left_pane, right_pane)
+
+    return total_plot_pane
+
+input_mol = input('Mol SMI: ')
+spectrum_3D(input_mol, True, 0.01).show()
 
-class TestSpectrumFunction(unittest.TestCase):
-    
-    def test_empty_smiles(self):
-        smiles = ""
-        result = spectrum(smiles, True, 0.1)
-        self.assertIsNone(result)
-    
-    def test_apparatus_resolution(self):
-        smiles = "CCO"
-        for res in [0.1, 0.5, 1.0]:
-            result = spectrum(smiles, True, res)
-            self.assertIsInstance(result, Figure)
-    
-    def test_imprecision_false(self):
-        smiles = "CCO"
-        result = spectrum(smiles, False, 0.1)
-        self.assertIsInstance(result, Figure)
-    
-    def test_imprecision_true(self):
-        smiles = "CCO"
-        result = spectrum(smiles, True, 0.1)
-        self.assertIsInstance(result, Figure)
-    
-    def test_valid_smiles(self):
-        smiles = "CCO"
-        result = spectrum(smiles, True, 0.1)
-        self.assertIsInstance(result, Figure)
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `massivechem-4.1/.gitignore` & `massivechem-4.3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Created by https://www.toptal.com/developers/gitignore/api/windows,macos,python,jupyternotebooks
-# Edit at https://www.toptal.com/developers/gitignore?templates=windows,macos,python,jupyternotebooks
+# Created by https://www.toptal.com/developers/gitignore/api/macos,linux,windows,jupyternotebooks,python
+# Edit at https://www.toptal.com/developers/gitignore?templates=macos,linux,windows,jupyternotebooks,python
 
 ### JupyterNotebooks ###
 # gitignore template for Jupyter Notebooks
 # website: http://jupyter.org/
 
 .ipynb_checkpoints
 */.ipynb_checkpoints/*
@@ -11,14 +11,29 @@
 # IPython
 profile_default/
 ipython_config.py
 
 # Remove previous ipynb_checkpoints
 #   git rm -r .ipynb_checkpoints/
 
+### Linux ###
+*~
+
+# temporary files which can be created if a process still has a handle open of a deleted file
+.fuse_hidden*
+
+# KDE directory preferences
+.directory
+
+# Linux trash folder which might appear on any partition or disk
+.Trash-*
+
+# .nfs files are created when an open file is removed but is still being accessed
+.nfs*
+
 ### macOS ###
 # General
 .DS_Store
 .AppleDouble
 .LSOverride
 
 # Icon must end with two \r
@@ -239,8 +254,8 @@
 *.msix
 *.msm
 *.msp
 
 # Windows shortcuts
 *.lnk
 
-# End of https://www.toptal.com/developers/gitignore/api/windows,macos,python,jupyternotebooks
+# End of https://www.toptal.com/developers/gitignore/api/macos,linux,windows,jupyternotebooks,python
```

### Comparing `massivechem-4.1/LICENSE.txt` & `massivechem-4.3/LICENSE.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2024 The Python Packaging Authority
+Copyright (c) 2024 MASSIVEChem
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `massivechem-4.1/README.md` & `massivechem-4.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-![logo](IMG_2856.jpg)
+![logo](Logo.jpg)
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
 # -         MASSIVEChem       - 
 
 [![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
 [![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
-[![GitHub3](https://img.shields.io/badge/License-3-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
 [![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
 
 
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
 #### Project within _practical programming in chemistry_ course -- EPFL CH-200
 
 ## Package description
@@ -26,15 +26,26 @@
 
 Developpers:
 - Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
 - Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
 - Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
 
 ### What is mass spectrometry ?
-   - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating pre-charged ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their composition.
+
+Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves three main steps:
+
+Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
+
+Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific m/z values. The unit of these m/z values is 1 Th or 1 $\frac{Da}{e}$.
+
+On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
+
+Mass spectrometry is widely used in various fields, including:
+
+Chemistry: For molecular identification and structural elucidation. Biochemistry: For studying proteins, peptides, and other biomolecules. Pharmaceuticals: For drug development and metabolite analysis. Environmental Science: For detecting pollutants and analysing environmental samples. Clinical Diagnostics: For identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
 
 Now, let us go through the steps required to use this package!
 
 ## Installation
 [![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
 
 MASSIVEChem can be installed using pip as
@@ -68,44 +79,40 @@
 
 
 
 
 
 
 ## Requirments
-The package runs on python 3.10 but supports python 3.8 through 3.10
-The package requires several other packages to function correctly.
+The package runs on python 3.10 but supports python 3.8 through 3.10.
+It requires several other packages to function correctly.
 
 ```bash
-matplotlib
 bokeh
 rdkit
-pandas
-panel 
-xyz2graph
+panel
 ```
 
+(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
 
 If all goes well during installation, the preceding packages should all install automatically.
 But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
 
 ```bash
 pip show "name of the package"
 ```
 
 If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
-pip install matplotlib
 pip install bokeh
 pip install rdkit
-pip install pandas
 pip install panel
 ```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function XXX. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
 
 ```bash
 python -m pip install git+https://github.com/zotko/xyz2graph.git
 ```
 
 
 ## Usage
@@ -113,26 +120,41 @@
 The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
 
 An example on how to make the function work is shown below for benzylpenicilin:
 
 The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
 
 ```bash
-import MASSIVEChem as ms
-from ms.MASSIVEChem import spectrum
+import MASSIVEChem.MASSIVEChem as MC
 from bokeh.plotting import show
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
 apparatus_resolution = 0.01
 
-show(spectrum(mol_smi, True, apparatus_resolution))
+show(MC.spectrum(mol_smi, True, apparatus_resolution))
+
+
+#The first input in ms.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01
+#the second computes an approximate spectrum if True and the precise spectrum if False
+
 ```
+
 The output of this command will be:
 
 ![Spectrum](Spectrum_output.png)
+
+Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
+
+<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
+
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
 '''link to jupter notebook'''
 
+## Fun !
+🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
+
+(_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `massivechem-4.1/pyproject.toml` & `massivechem-4.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 00000000: 5b62 7569 6c64 2d73 7973 7465 6d5d 0d0a  [build-system]..
 00000010: 7265 7175 6972 6573 203d 205b 2268 6174  requires = ["hat
 00000020: 6368 6c69 6e67 225d 0d0a 6275 696c 642d  chling"]..build-
 00000030: 6261 636b 656e 6420 3d20 2268 6174 6368  backend = "hatch
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 4d41 5353 4956 4543 6865 6d22 0d0a   "MASSIVEChem"..
-00000070: 7665 7273 696f 6e20 3d20 2234 2e31 220d  version = "4.1".
+00000070: 7665 7273 696f 6e20 3d20 2234 2e33 220d  version = "4.3".
 00000080: 0a64 6573 6372 6970 7469 6f6e 203d 2022  .description = "
 00000090: 4d41 5353 4956 4543 6865 6d20 6973 2061  MASSIVEChem is a
 000000a0: 2070 6970 2d69 6e73 7461 6c6c 6162 6c65   pip-installable
 000000b0: 2070 6163 6b61 6765 2066 6f72 2061 6e61   package for ana
 000000c0: 6c79 7469 6361 6c20 6368 656d 6973 7472  lytical chemistr
 000000d0: 792e 2049 7420 7369 6d75 6c61 7465 7320  y. It simulates 
 000000e0: 6d6f 6c65 6375 6c65 206d 6173 7320 7370  molecule mass sp
@@ -53,39 +53,37 @@
 00000340: 6572 6940 6570 666c 2e63 6822 207d 2c0d  eri@epfl.ch" },.
 00000350: 0a20 207b 206e 616d 6520 3d20 2241 7274  .  { name = "Art
 00000360: 6875 7220 4875 6d65 7279 222c 2065 6d61  hur Humery", ema
 00000370: 696c 203d 2022 6172 7468 7572 2e68 756d  il = "arthur.hum
 00000380: 6572 7940 6570 666c 2e63 6822 207d 0d0a  ery@epfl.ch" }..
 00000390: 5d0d 0a64 6570 656e 6465 6e63 6965 7320  ]..dependencies 
 000003a0: 3d20 5b0d 0a20 2022 7264 6b69 7422 2c0d  = [..  "rdkit",.
-000003b0: 0a20 2022 7061 6e64 6173 222c 0d0a 2020  .  "pandas",..  
-000003c0: 226d 6174 706c 6f74 6c69 6222 2c0d 0a20  "matplotlib",.. 
-000003d0: 2022 626f 6b65 6822 2c0d 0a20 2022 7061   "bokeh",..  "pa
-000003e0: 6e65 6c22 2c0d 0a5d 0d0a 636c 6173 7369  nel",..]..classi
-000003f0: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
-00000400: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
-00000410: 7573 203a 3a20 3420 2d20 4265 7461 222c  us :: 4 - Beta",
-00000420: 0d0a 2020 2020 2250 726f 6772 616d 6d69  ..    "Programmi
-00000430: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000440: 7974 686f 6e20 3a3a 2033 222c 0d0a 2020  ython :: 3",..  
-00000450: 2020 224c 6963 656e 7365 203a 3a20 4f53    "License :: OS
-00000460: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-00000470: 5420 4c69 6365 6e73 6522 2c0d 0a20 2020  T License",..   
-00000480: 2022 4f70 6572 6174 696e 6720 5379 7374   "Operating Syst
-00000490: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
-000004a0: 6465 6e74 220d 0a5d 0d0a 0d0a 5b70 726f  dent"..]....[pro
-000004b0: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
-000004c0: 7061 6765 203d 2022 6874 7470 733a 2f2f  page = "https://
-000004d0: 6769 7468 7562 2e63 6f6d 2f54 686f 6d61  github.com/Thoma
-000004e0: 7343 7373 6f6e 2f4d 4153 5349 5645 4368  sCsson/MASSIVECh
-000004f0: 656d 2e67 6974 220d 0a47 6974 4875 625f  em.git"..GitHub_
-00000500: 5468 6f6d 6173 5f43 6872 6973 7469 616e  Thomas_Christian
-00000510: 7373 6f6e 203d 2022 6874 7470 733a 2f2f  sson = "https://
-00000520: 6769 7468 7562 2e63 6f6d 2f54 686f 6d61  github.com/Thoma
-00000530: 7343 7373 6f6e 220d 0a47 6974 4875 625f  sCsson"..GitHub_
-00000540: 4967 6f72 5f47 6f6e 7465 7269 203d 2022  Igor_Gonteri = "
-00000550: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000560: 6f6d 2f69 676f 7267 6f6e 7465 7269 220d  om/igorgonteri".
-00000570: 0a47 6974 4875 625f 4172 7468 7572 5f48  .GitHub_Arthur_H
-00000580: 756d 6572 7920 3d20 2268 7474 7073 3a2f  umery = "https:/
-00000590: 2f67 6974 6875 622e 636f 6d2f 4172 7468  /github.com/Arth
-000005a0: 7572 686d 7922 0d0a                      urhmy"..
+000003b0: 0a20 2022 626f 6b65 6822 2c0d 0a20 2022  .  "bokeh",..  "
+000003c0: 7061 6e65 6c22 2c0d 0a5d 0d0a 636c 6173  panel",..]..clas
+000003d0: 7369 6669 6572 7320 3d20 5b0d 0a20 2020  sifiers = [..   
+000003e0: 2022 4465 7665 6c6f 706d 656e 7420 5374   "Development St
+000003f0: 6174 7573 203a 3a20 3420 2d20 4265 7461  atus :: 4 - Beta
+00000400: 222c 0d0a 2020 2020 2250 726f 6772 616d  ",..    "Program
+00000410: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000420: 2050 7974 686f 6e20 3a3a 2033 222c 0d0a   Python :: 3",..
+00000430: 2020 2020 224c 6963 656e 7365 203a 3a20      "License :: 
+00000440: 4f53 4920 4170 7072 6f76 6564 203a 3a20  OSI Approved :: 
+00000450: 4d49 5420 4c69 6365 6e73 6522 2c0d 0a20  MIT License",.. 
+00000460: 2020 2022 4f70 6572 6174 696e 6720 5379     "Operating Sy
+00000470: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000480: 656e 6465 6e74 220d 0a5d 0d0a 0d0a 5b70  endent"..]....[p
+00000490: 726f 6a65 6374 2e75 726c 735d 0d0a 486f  roject.urls]..Ho
+000004a0: 6d65 7061 6765 203d 2022 6874 7470 733a  mepage = "https:
+000004b0: 2f2f 6769 7468 7562 2e63 6f6d 2f54 686f  //github.com/Tho
+000004c0: 6d61 7343 7373 6f6e 2f4d 4153 5349 5645  masCsson/MASSIVE
+000004d0: 4368 656d 2e67 6974 220d 0a47 6974 4875  Chem.git"..GitHu
+000004e0: 625f 5468 6f6d 6173 5f43 6872 6973 7469  b_Thomas_Christi
+000004f0: 616e 7373 6f6e 203d 2022 6874 7470 733a  ansson = "https:
+00000500: 2f2f 6769 7468 7562 2e63 6f6d 2f54 686f  //github.com/Tho
+00000510: 6d61 7343 7373 6f6e 220d 0a47 6974 4875  masCsson"..GitHu
+00000520: 625f 4967 6f72 5f47 6f6e 7465 7269 203d  b_Igor_Gonteri =
+00000530: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
+00000540: 2e63 6f6d 2f69 676f 7267 6f6e 7465 7269  .com/igorgonteri
+00000550: 220d 0a47 6974 4875 625f 4172 7468 7572  "..GitHub_Arthur
+00000560: 5f48 756d 6572 7920 3d20 2268 7474 7073  _Humery = "https
+00000570: 3a2f 2f67 6974 6875 622e 636f 6d2f 4172  ://github.com/Ar
+00000580: 7468 7572 686d 7922 0d0a                 thurhmy"..
```

### Comparing `massivechem-4.1/PKG-INFO` & `massivechem-4.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: MASSIVEChem
-Version: 4.1
+Version: 4.3
 Summary: MASSIVEChem is a pip-installable package for analytical chemistry. It simulates molecule mass spectra and graphically displays them. It includes tools like a functional group finder and unsaturation calculator to aid chemical analysis.
 Project-URL: Homepage, https://github.com/ThomasCsson/MASSIVEChem.git
 Project-URL: GitHub_Thomas_Christiansson, https://github.com/ThomasCsson
 Project-URL: GitHub_Igor_Gonteri, https://github.com/igorgonteri
 Project-URL: GitHub_Arthur_Humery, https://github.com/Arthurhmy
 Author-email: Thomas Viking Christiansson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
@@ -12,33 +12,31 @@
 Keywords: Mass spectroscopy,chemical-engineering,chemical-property-prediction,cheminformatics,chemistry,chemistry-lab,functional group,spectrometry,spectroscopy,unsaturation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: bokeh
-Requires-Dist: matplotlib
-Requires-Dist: pandas
 Requires-Dist: panel
 Requires-Dist: rdkit
 Description-Content-Type: text/markdown
 
-![logo](IMG_2856.jpg)
+![logo](Logo.jpg)
 [![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ThomasCsson/MASSIVEChem)
 [![Thomas3](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org/)
 ![Thomas4](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
 [![Thomas6](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 
 
 # -         MASSIVEChem       - 
 
 [![GitHub2](https://img.shields.io/badge/Maintained%3F-yes-turquoise.svg)](https://pypi.org/user/Arthur.hmy/)
 [![python](https://img.shields.io/badge/Python-3.10-3776AB.svg?style=flat&logo=python&logoColor=orange)](https://www.python.org)
 [![GitHub3](https://img.shields.io/badge/Contributors-3-green.svg)](https://github.com/ThomasCsson/MASSIVEChem/graphs/contributors)
-[![GitHub3](https://img.shields.io/badge/License-3-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
+[![GitHub3](https://img.shields.io/badge/License-MIT-purple.svg)](https://github.com/ThomasCsson/MASSIVEChem/blob/main/LICENSE.txt)
 [![GitHub3](https://img.shields.io/badge/EPFL-CH200-red.svg)](https://edu.epfl.ch/studyplan/en/bachelor/chemistry-and-chemical-engineering/coursebook/practical-programming-in-chemistry-CH-200)
 
 
  - Python package for applied analytical chemistry focused primarily on mass speectrometry 
 #### Project within _practical programming in chemistry_ course -- EPFL CH-200
 
 ## Package description
@@ -50,15 +48,26 @@
 
 Developpers:
 - Thomas Viking Christiansson, student in chemical engineering at EPFL    [![jhc github](https://img.shields.io/badge/GitHub-ThomasCsson-181717.svg?style=flat&logo=github)](https://github.com/ThomasCsson)
 - Igor Gonteri, student in chemistry at EPFL                             [![jhc github](https://img.shields.io/badge/GitHub-igorgonteri-181717.svg?style=flat&logo=github)](https://github.com/igorgonteri)
 - Arthur Humery, student in chemical engineering at EPFL                [![jhc github](https://img.shields.io/badge/GitHub-Arthurhmy-181717.svg?style=flat&logo=github)](https://github.com/Arthurhmy)
 
 ### What is mass spectrometry ?
-   - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating pre-charged ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their composition.
+
+Mass spectrometry (MS) is an analytical technique used to measure the mass-to-charge ratio of ions. It helps identify the structure of the chemical compound present in a sample by generating a spectrum of the masses of its ions. The process involves three main steps:
+
+Ionisation: The sample is ionised, which means its molecules are converted into charged particles (ions). This can be done using various methods, such as electron impact (EI), electrospray ionisation (ESI), or matrix-assisted laser desorption/ionisation (MALDI). In this case, the ionisation is set to the most commonly used method; deprotonation.
+
+Mass Analysis: The ions are separated based on their mass-to-charge ratio (m/z). This is usually done using a mass analyser, such as a quadrupole, time-of-flight (TOF), or an ion trap. Each type of mass analyser works differently but ultimately serves to distinguish ions by their specific m/z values. The unit of these m/z values is 1 Th or 1 $\frac{Da}{e}$.
+
+On the y axis of the output spectrum, the relative abundance of the different ions is plotted. This abundance is given by the different natural abundances of the different isotopes of the atoms in the molecule. For example, the relative abundance of $^{13}C$ is 1.1% and that of $^{12}C$ is 98.9%.
+
+Mass spectrometry is widely used in various fields, including:
+
+Chemistry: For molecular identification and structural elucidation. Biochemistry: For studying proteins, peptides, and other biomolecules. Pharmaceuticals: For drug development and metabolite analysis. Environmental Science: For detecting pollutants and analysing environmental samples. Clinical Diagnostics: For identifying biomarkers and analysing complex biological samples. The technique's sensitivity, accuracy, and ability to analyse complex mixtures make it an essential tool in both research and applied sciences.
 
 Now, let us go through the steps required to use this package!
 
 ## Installation
 [![Thomas2](https://img.shields.io/badge/pypi-3775A9?style=for-the-badge&logo=pypi&logoColor=white)](https://pypi.org/project/MASSIVEChem/)
 
 MASSIVEChem can be installed using pip as
@@ -92,44 +101,40 @@
 
 
 
 
 
 
 ## Requirments
-The package runs on python 3.10 but supports python 3.8 through 3.10
-The package requires several other packages to function correctly.
+The package runs on python 3.10 but supports python 3.8 through 3.10.
+It requires several other packages to function correctly.
 
 ```bash
-matplotlib
 bokeh
 rdkit
-pandas
-panel 
-xyz2graph
+panel
 ```
 
+(Note: panel is not directly used, but is required for added functionality involving the 3 dimmensinal visualisation of the input molecule)
 
 If all goes well during installation, the preceding packages should all install automatically.
 But this can be checked by veryfying that they have all been installed in the desired environment. To do this, simply write the following command in the terminal:
 
 ```bash
 pip show "name of the package"
 ```
 
 If not, install them using the following commands. (Bear in mind that the package will not run without its dependencies. 
 
 ```bash
-pip install matplotlib
 pip install bokeh
 pip install rdkit
-pip install pandas
 pip install panel
 ```
-Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function XXX. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
+Additionally, the package 'xyz2graph' is required to run the 3D imaging functionallity in the function 'spectrum'. This package is not pip-installable, so to intall it yourslef, the following command needs to be run.
 
 ```bash
 python -m pip install git+https://github.com/zotko/xyz2graph.git
 ```
 
 
 ## Usage
@@ -137,26 +142,41 @@
 The principal function of this package takes the SMILEs of a molecule as an input and displays the mass spectrometry of the molecule as well as the molecule itself and  the functional groups it contains.
 
 An example on how to make the function work is shown below for benzylpenicilin:
 
 The ionization method is set to monodeprotonation and the resolution of the apparatus is 0.01 Th
 
 ```bash
-import MASSIVEChem as ms
-from ms.MASSIVEChem import spectrum
+import MASSIVEChem.MASSIVEChem as MC
 from bokeh.plotting import show
 
 mol_smi = 'CC1(C(N2C(S1)C(C2=O)NC(=O)CC3=CC=CC=C3)C(=O)O)C'
 apparatus_resolution = 0.01
 
-show(spectrum(mol_smi, True, apparatus_resolution))
+show(MC.spectrum(mol_smi, True, apparatus_resolution))
+
+
+#The first input in ms.spectrum is the molecule under SMILEs representation,
+#and the third is the resolution of the apparatus (typically, this value is of 0.01
+#the second computes an approximate spectrum if True and the precise spectrum if False
+
 ```
+
 The output of this command will be:
 
 ![Spectrum](Spectrum_output.png)
+
+Note that here there appear to be two overlapping peaks at ~ 334 [th]. This is due to the presence of an odd number of sulphur atoms. This causes there to be a peak 0.004 [th] infront of the second peak. This can be verified by zooming in on the sectrum:
+
+<img width="600" alt="Focused_spectrum" src="https://github.com/ThomasCsson/MASSIVEChem/assets/160872481/440ac2ea-c2fe-40ff-b1ed-1a447024bcb0">
+
 ## Getting started
 [![jupyter](https://img.shields.io/badge/Jupyter-Lab-F37626.svg?style=flat&logo=Jupyter)](https://jupyterlab.readthedocs.io/en/stable)
 
 To begin to use the package the following jupyter notebook will give you information about all the package's functions:
 
 '''link to jupter notebook'''
 
+## Fun !
+🐰 If you've made it this far through our project, you might want to try to find the hidden easter egg in this ReadMe :)🐰
+
+(_hint: you might want to try clicking on various badges throughout the ReadMe_)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

