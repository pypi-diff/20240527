# Comparing `tmp/project_ppchem_tools_kit-1.0.0.tar.gz` & `tmp/project_ppchem_tools_kit-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_ppchem_tools_kit-1.0.0.tar", max compression
+gzip compressed data, was "project_ppchem_tools_kit-1.1.0.tar", max compression
```

## Comparing `project_ppchem_tools_kit-1.0.0.tar` & `project_ppchem_tools_kit-1.1.0.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-1.0.0/LICENSE
--rw-r--r--   0        0        0     9620 2024-05-20 14:19:51.999970 project_ppchem_tools_kit-1.0.0/README.md
--rw-r--r--   0        0        0     1119 2024-05-20 15:24:49.364904 project_ppchem_tools_kit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/__init__.py
--rw-r--r--   0        0        0      537 2024-05-20 14:52:11.199976 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/add_data_point.py
--rw-r--r--   0        0        0      439 2024-05-20 14:52:11.201062 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/bind_enter.py
--rw-r--r--   0        0        0      672 2024-05-20 12:02:51.196051 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/browse_excel_file.py
--rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/clear_input.py
--rw-r--r--   0        0        0      528 2024-05-20 14:52:11.201388 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/copy_text.py
--rw-r--r--   0        0        0      979 2024-05-20 12:23:16.912190 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/create_radio_button.py
--rw-r--r--   0        0        0     3300 2024-05-20 14:52:11.202010 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_graph.py
--rw-r--r--   0        0        0     2646 2024-05-20 14:52:11.202368 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py
--rw-r--r--   0        0        0     1229 2024-05-20 14:52:11.203373 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_molecule.py
--rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_result.py
--rw-r--r--   0        0        0     8474 2024-05-20 14:52:11.203706 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/error_calculation_interface.py
--rw-r--r--   0        0        0    11926 2024-05-20 14:52:11.204368 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/graph_function.py
--rw-r--r--   0        0        0     2251 2024-05-20 14:52:11.205130 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/linear_regression.py
--rw-r--r--   0        0        0     1555 2024-05-20 14:52:11.206095 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/make_graph.py
--rw-r--r--   0        0        0      710 2024-05-20 14:52:11.206377 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/name_to_smiles.py
--rw-r--r--   0        0        0      568 2024-05-20 14:52:11.207080 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/on_closing.py
--rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/on_radio_select.py
--rw-r--r--   0        0        0     1893 2024-05-20 14:52:11.207375 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/open_graph_settings_window.py
--rw-r--r--   0        0        0     2291 2024-05-20 14:52:11.207905 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/process_input.py
--rw-r--r--   0        0        0      462 2024-05-20 14:52:11.208858 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/relative_to_assets.py
--rw-r--r--   0        0        0      364 2024-05-20 14:52:11.209157 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/select_all.py
--rw-r--r--   0        0        0      564 2024-05-20 14:52:11.209435 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_axes_color.py
--rw-r--r--   0        0        0      701 2024-05-20 14:52:11.209690 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_background_color.py
--rw-r--r--   0        0        0      840 2024-05-20 14:52:11.210035 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
--rw-r--r--   0        0        0      401 2024-05-20 14:52:11.210482 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_grid_color.py
--rw-r--r--   0        0        0      493 2024-05-20 14:52:11.211071 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_label_color.py
--rw-r--r--   0        0        0      590 2024-05-20 14:52:11.211500 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_line_color.py
--rw-r--r--   0        0        0      706 2024-05-20 14:52:11.211802 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_scale.py
--rw-r--r--   0        0        0      515 2024-05-20 14:52:11.212405 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
--rw-r--r--   0        0        0      308 2024-05-20 14:52:11.212717 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/toggle_grid.py
--rw-r--r--   0        0        0      654 2024-05-20 14:52:11.213814 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/update_clock.py
--rw-r--r--   0        0        0      987 2024-05-20 14:52:11.214223 project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/welcome_message.py
--rw-r--r--   0        0        0    10969 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-1.1.0/LICENSE
+-rw-r--r--   0        0        0    10402 2024-05-27 08:07:35.473361 project_ppchem_tools_kit-1.1.0/README.md
+-rw-r--r--   0        0        0     1064 2024-05-27 09:20:57.405517 project_ppchem_tools_kit-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/__init__.py
+-rw-r--r--   0        0        0      537 2024-05-20 14:52:11.199976 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/add_data_point.py
+-rw-r--r--   0        0        0      672 2024-05-20 12:02:51.196051 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/browse_excel_file.py
+-rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/clear_input.py
+-rw-r--r--   0        0        0      528 2024-05-20 14:52:11.201388 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/copy_text.py
+-rw-r--r--   0        0        0      979 2024-05-20 12:23:16.912190 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/create_radio_button.py
+-rw-r--r--   0        0        0     3300 2024-05-20 14:52:11.202010 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_graph.py
+-rw-r--r--   0        0        0     2646 2024-05-20 14:52:11.202368 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py
+-rw-r--r--   0        0        0     1229 2024-05-20 14:52:11.203373 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_molecule.py
+-rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_result.py
+-rw-r--r--   0        0        0     8474 2024-05-20 14:52:11.203706 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/error_calculation_interface.py
+-rw-r--r--   0        0        0    11926 2024-05-20 14:52:11.204368 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/graph_function.py
+-rw-r--r--   0        0        0     2251 2024-05-20 14:52:11.205130 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/linear_regression.py
+-rw-r--r--   0        0        0     1555 2024-05-20 14:52:11.206095 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/make_graph.py
+-rw-r--r--   0        0        0      710 2024-05-20 14:52:11.206377 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/name_to_smiles.py
+-rw-r--r--   0        0        0      568 2024-05-20 14:52:11.207080 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/on_closing.py
+-rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/on_radio_select.py
+-rw-r--r--   0        0        0     1893 2024-05-20 14:52:11.207375 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/open_graph_settings_window.py
+-rw-r--r--   0        0        0     2291 2024-05-20 14:52:11.207905 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/process_input.py
+-rw-r--r--   0        0        0      462 2024-05-20 14:52:11.208858 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/relative_to_assets.py
+-rw-r--r--   0        0        0      364 2024-05-20 14:52:11.209157 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/select_all.py
+-rw-r--r--   0        0        0      564 2024-05-20 14:52:11.209435 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_axes_color.py
+-rw-r--r--   0        0        0      701 2024-05-20 14:52:11.209690 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_background_color.py
+-rw-r--r--   0        0        0      840 2024-05-20 14:52:11.210035 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
+-rw-r--r--   0        0        0      401 2024-05-20 14:52:11.210482 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_grid_color.py
+-rw-r--r--   0        0        0      493 2024-05-20 14:52:11.211071 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_label_color.py
+-rw-r--r--   0        0        0      590 2024-05-20 14:52:11.211500 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_line_color.py
+-rw-r--r--   0        0        0      706 2024-05-20 14:52:11.211802 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_scale.py
+-rw-r--r--   0        0        0      515 2024-05-20 14:52:11.212405 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
+-rw-r--r--   0        0        0      308 2024-05-20 14:52:11.212717 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/toggle_grid.py
+-rw-r--r--   0        0        0      719 2024-05-24 08:14:06.304018 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/update_clock.py
+-rw-r--r--   0        0        0      987 2024-05-20 14:52:11.214223 project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/welcome_message.py
+-rw-r--r--   0        0        0    11751 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-1.1.0/PKG-INFO
```

### Comparing `project_ppchem_tools_kit-1.0.0/LICENSE` & `project_ppchem_tools_kit-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/README.md` & `project_ppchem_tools_kit-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 
 <p align="center">
-   <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
-   
-
-
- </p>
-
-
-
-
- <h1 align="center">🧰 Tools Kit</h1>
+  <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
+</p>
+                                                              
+<div align="center">
+  <h1 style="font-size: 3em;">🛠️ Tools Kit 🛠 </h1>
+</div>
 
- <p align="center">
-  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/actions"><img src="https://img.shields.io/badge/build-passing-brightgreen.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Build Status"></a>
-<a href="https://github.com/sgrunber/Project-ppchem-tools-kit"><img src="https://img.shields.io/badge/coverage-95%25-brightgreen.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Coverage"></a>
-<a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="License"></a>
 
+<p align="center">
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/actions">
+    <img src="https://img.shields.io/badge/build-passing-brightgreen.svg?style=for-the-badge&logo=github&logoColor=white" alt="Build Status">
+  </a>
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit">
+    <img src="https://img.shields.io/badge/coverage-95%25-brightgreen.svg?style=for-the-badge&logo=github&logoColor=white" alt="Coverage">
+  </a>
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE">
+    <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=github&logoColor=white" alt="License">
+  </a>
 </p>
 
+
 ## 📖 Description
 The **Tools Kit** package allows chemistry students to find basic information on molecules and provides easy access to some graphs and calculations required in experimental laboratories.
 
 **🌙 Note**: For an aesthetically pleasing experience, it is recommended to use the dark mode interface if you are on a Mac or any other platform that supports it.
 
 
 ## 📚 Table of Contents
@@ -39,25 +42,46 @@
 To start, fork the repository to your own GitHub account.  
 To do so, navigate to the repository page and click the *"Fork"* button. The repository will then be copied to your account, and you will be able to access it.
 
 ### 2. 📥 Clone the Repository
 
  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/tree/main"><img src="https://img.shields.io/badge/GitHub--181717.svg?logo=github&logoColor=white&style=for-the-badge&logoWidth=40&logoColor=white" alt="GitHub"></a>
 
-Next, clone the repository using the following command (replace *username* with your GitHub username):
+Next, clone the repository using the following command:
+
+#### a) Using HTTPS (default):
 
 ```bash
 git clone https://github.com/sgrunber/Project-ppchem-tools-kit.git
 ```
+#### b) Using SSH (recommended for users who have set up SSH):
+
+To clone with SSH, use the following command:
+
+```bash
+git clone git@github.com:sgrunber/Project-ppchem-tools-kit.git
+```
+
 
 ### 3. ⬇️ Install with pip
 
-  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v0.1.3-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
 
-You can also install Tools Kit using pip:
+After cloning, navigate into the cloned directory and install the package locally using pip:
+
+```bash
+cd path/to/Project-ppchem-tools-kit
+pip install .
+```
+This will install the package and its dependencies from the cloned repository, automatically fetching the latest version:
+
+
+
+  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v1.0.0-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
+
+Alternatively, you can install Tools Kit using pip, which will fetch and install the latest updated version from PyPI:
 
 ```bash
 pip install Project_ppchem-tools-kit
 ```
 
 ## 🚀 Usage
 <a id="usage"></a>
@@ -104,30 +128,31 @@
 2. ⚖️ Molecular Weight
    - Input: SMILES of the molecule
    - Output: Corresponding molar mass in g/mol
 
 3. 📈 Linear Regression
    - Input: Excel document (imported by pressing the Browse button)
    - Output: Linear regression graph with the R<sup>2</sup> value
+        - Options: The graph allows customization of various parameters such as changing scales, axis labels, title, displaying maximum values, enabling gridlines, adjusting line types and colors, modifying grid and label axes, and background color.
 
 4. 📊 Graph Maker
    - Input: Excel document with x and y values arranged in two columns
    - Output: Graph plotting all values
       - Options: The graph allows customization of various parameters such as changing scales, axis labels, title, displaying maximum values, enabling gridlines, adjusting line types and colors, modifying grid and label axes, and background color.
 
 
-5. 📉 Error Propagation
+5. 🧮 Error Propagation
    - Input: Variables, their values, and their uncertainties.
    - Output: Mean value, its uncertainty, and the result can be copied as LaTeX code for easy inclusion in documents.
 
-6. 🧪 Show Molecule
+6. 🔬 Show Molecule
    - Input: SMILES
    - Output: Molecular structure
 
-The graphs in sections 3 and 4 can also include input for the title and X, Y axis labels.
+
 
 ## 🤝 Contributing
 <a id="contributing"></a>
 
 Contributions are welcome! To contribute to **Tools Kit**, please follow these steps:
 
 1. **Fork** the project to your GitHub account.
```

#### html2text {}

```diff
@@ -1,59 +1,68 @@
                                 [logo_project]
-                         ************ ?ð??§?° TToooollss KKiitt ************
+                     ************ ?ð??? ?ï?¸? TToooollss KKiitt ?ð???  ************
                        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]_[_L_i_c_e_n_s_e_]
 ## ð Description The **Tools Kit** package allows chemistry students to find
 basic information on molecules and provides easy access to some graphs and
 calculations required in experimental laboratories. **ð Note**: For an
 aesthetically pleasing experience, it is recommended to use the dark mode
 interface if you are on a Mac or any other platform that supports it. ## ð
 Table of Contents - [Installation](#ï¸-installation) - [Usage](#ï¸-usage) -
 [Features](#ï¸-features) - [Contributing](#ï¸-contributing) - [Cite Us](#ï¸-
 cite-us) - [License](#ï¸-license) - [Screenshots](#ï¸-screenshots) ## ð ï¸
 Installation ### 1. ð´ Fork the Repository To start, fork the repository to
 your own GitHub account. To do so, navigate to the repository page and click
 the *"Fork"* button. The repository will then be copied to your account, and
 you will be able to access it. ### 2. ð¥ Clone the Repository _[_G_i_t_H_u_b_]Next,
-clone the repository using the following command (replace *username* with your
-GitHub username): ```bash git clone https://github.com/sgrunber/Project-ppchem-
-tools-kit.git ``` ### 3. â¬ï¸ Install with pip _[_P_y_P_I_]You can also install
-Tools Kit using pip: ```bash pip install Project_ppchem-tools-kit ``` ## ð
-Usage To use Tools Kit and access its features, follow these steps after
-cloning the repository: ### Using Jupyter Notebook: _[_J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k_]1. Launch
-Jupyter Notebook by navigating to the cloned repository directory in your
-terminal and running the command: ```bash jupyter notebook ``` 2. In the
-Jupyter Notebook interface, navigate to the `notebooks` directory. 3. Open the
-notebook named `project_report.ipynb`. 4. Follow the instructions inside the
-notebook to interact with the Tools Kit interface and utilize its features for
-molecule analysis, graph plotting, error calculation, and more. This notebook
-provides an interactive environment for convenient usage of Tools Kit directly
-within Visual Studio Code. ### Usage with Visual Studio Code: _[_V_S_C_o_d_e_]1. Open
-Visual Studio Code and navigate to the cloned directory. 2. Install the Jupyter
+clone the repository using the following command: #### a) Using HTTPS
+(default): ```bash git clone https://github.com/sgrunber/Project-ppchem-tools-
+kit.git ``` #### b) Using SSH (recommended for users who have set up SSH): To
+clone with SSH, use the following command: ```bash git clone git@github.com:
+sgrunber/Project-ppchem-tools-kit.git ``` ### 3. â¬ï¸ Install with pip After
+cloning, navigate into the cloned directory and install the package locally
+using pip: ```bash cd path/to/Project-ppchem-tools-kit pip install . ``` This
+will install the package and its dependencies from the cloned repository,
+automatically fetching the latest version: _[_P_y_P_I_]Alternatively, you can install
+Tools Kit using pip, which will fetch and install the latest updated version
+from PyPI: ```bash pip install Project_ppchem-tools-kit ``` ## ð Usage To
+use Tools Kit and access its features, follow these steps after cloning the
+repository: ### Using Jupyter Notebook: _[_J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k_]1. Launch Jupyter
+Notebook by navigating to the cloned repository directory in your terminal and
+running the command: ```bash jupyter notebook ``` 2. In the Jupyter Notebook
+interface, navigate to the `notebooks` directory. 3. Open the notebook named
+`project_report.ipynb`. 4. Follow the instructions inside the notebook to
+interact with the Tools Kit interface and utilize its features for molecule
+analysis, graph plotting, error calculation, and more. This notebook provides
+an interactive environment for convenient usage of Tools Kit directly within
+Visual Studio Code. ### Usage with Visual Studio Code: _[_V_S_C_o_d_e_]1. Open Visual
+Studio Code and navigate to the cloned directory. 2. Install the Jupyter
 extension if not already installed. You can do this by searching for "Jupyter"
 in the Extensions view (Ctrl+Shift+X) and installing the "Python" extension
 pack. 3. Open the `notebooks` directory in Visual Studio Code. 4. Open the
 notebook named `project_report.ipynb`. 5. Follow the instructions inside the
 notebook to interact with the Tools Kit interface and utilize its features for
 molecule analysis, graph plotting, error calculation, and more. This notebook
 provides an interactive environment for convenient usage of Tools Kit with
 Jupyter Notebook. ## ð§ª Features 1. ð§¬ Molecule Name - Input: Raw formula
 of the molecule - Output: SMILES of the molecule 2. âï¸ Molecular Weight -
 Input: SMILES of the molecule - Output: Corresponding molar mass in g/mol 3.
 ð Linear Regression - Input: Excel document (imported by pressing the Browse
-button) - Output: Linear regression graph with the R2 value 4. ð Graph Maker
-- Input: Excel document with x and y values arranged in two columns - Output:
-Graph plotting all values - Options: The graph allows customization of various
-parameters such as changing scales, axis labels, title, displaying maximum
-values, enabling gridlines, adjusting line types and colors, modifying grid and
-label axes, and background color. 5. ð Error Propagation - Input: Variables,
-their values, and their uncertainties. - Output: Mean value, its uncertainty,
-and the result can be copied as LaTeX code for easy inclusion in documents. 6.
-ð§ª Show Molecule - Input: SMILES - Output: Molecular structure The graphs in
-sections 3 and 4 can also include input for the title and X, Y axis labels. ##
-ð¤ Contributing Contributions are welcome! To contribute to **Tools Kit**,
+button) - Output: Linear regression graph with the R2 value - Options: The
+graph allows customization of various parameters such as changing scales, axis
+labels, title, displaying maximum values, enabling gridlines, adjusting line
+types and colors, modifying grid and label axes, and background color. 4. ð
+Graph Maker - Input: Excel document with x and y values arranged in two columns
+- Output: Graph plotting all values - Options: The graph allows customization
+of various parameters such as changing scales, axis labels, title, displaying
+maximum values, enabling gridlines, adjusting line types and colors, modifying
+grid and label axes, and background color. 5. ð§® Error Propagation - Input:
+Variables, their values, and their uncertainties. - Output: Mean value, its
+uncertainty, and the result can be copied as LaTeX code for easy inclusion in
+documents. 6. ð¬ Show Molecule - Input: SMILES - Output: Molecular structure
+## ð¤ Contributing Contributions are welcome! To contribute to **Tools Kit**,
 please follow these steps: 1. **Fork** the project to your GitHub account. 2.
 Create a new branch for your feature or bug fix: ```bash git checkout -
 b feature/your-feature-name ``` 3. **Create a new branch for your feature or
 bug fix:** ```bash git checkout -b feature/your-feature-name ``` 4. **Make your
 changes and ensure they adhere to the project's coding conventions and style
 guidelines.** 5. **Commit your changes with descriptive messages explaining the
 purpose of your changes:** ```bash git commit -am 'Add some feature' ``` 6.
```

### Comparing `project_ppchem_tools_kit-1.0.0/pyproject.toml` & `project_ppchem_tools_kit-1.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Project-ppchem-tools-kit"
-version = "1.0.0"
+version = "1.1.0"
 description = "Basic Chemistry Toolkit"
 authors = ["Méloé Enzinger <meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
     "Chemistry",
     "Tools kit",
@@ -25,21 +25,19 @@
 numpy5 = "^0.1"
 numpy = "^1.26.4"
 pillow = "10.2.0"
 pubchempy = "1.0.4"
 rdkit = "2023.9.6"
 requests = "2.31.0"
 matplotlib = "3.7.2"
-pandas = "2.0.3"
+pandas = "1.5.0"
 reportlab = "4.2.0"
 pyperclip = "1.8.2"
 openpyxl = "3.1.2"
 
-[tool.poetry.group.dev.dependencies]
-pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/sgrunber/Project-ppchem-tools-kit"
```

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/add_data_point.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/add_data_point.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/browse_excel_file.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/browse_excel_file.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/copy_text.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/copy_text.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/create_radio_button.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/create_radio_button.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_graph.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_graph.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_max_point_and_coords.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_molecule.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_molecule.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/display_result.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/display_result.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/error_calculation_interface.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/error_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/graph_function.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/graph_function.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/linear_regression.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/linear_regression.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/make_graph.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/make_graph.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/name_to_smiles.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/name_to_smiles.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/on_closing.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/on_closing.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/open_graph_settings_window.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/open_graph_settings_window.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/process_input.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/process_input.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_axes_color.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_axes_color.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_background_color.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_background_color.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_custom_labels_and_title.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_line_color.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_line_color.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/set_scale.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/set_scale.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/smiles_to_molar_mass.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/update_clock.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/update_clock.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 window = None
 import tkinter as tk
 from datetime import datetime
 
 
 
-def update_clock():
+def update_clock(window, clock_label, date_label):
     """Updates the clock label with the current time and date every second."""
     current_time = datetime.now().strftime('%H:%M:%S')
     current_date = datetime.now().strftime('%Y-%m-%d')
     clock_label.config(text=current_time)
     date_label.config(text=current_date)
-    window.after(1000, update_clock)
+    window.after(1000, update_clock, window, clock_label, date_label)
+
 
 date_label = tk.Label(window, text="", font=("Times New Roman", 20), bg="#1B262C", fg="#FFFFFF")
 date_label.place(x=890, y=10)
 
 clock_label = tk.Label(window, text="", font=("Times New Roman", 20), bg="#1B262C", fg="#FFFFFF")
 clock_label.place(x=890, y=40)
```

### Comparing `project_ppchem_tools_kit-1.0.0/src/project_ppchem_tools_kit/welcome_message.py` & `project_ppchem_tools_kit-1.1.0/src/project_ppchem_tools_kit/welcome_message.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-1.0.0/PKG-INFO` & `project_ppchem_tools_kit-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Project-ppchem-tools-kit
-Version: 1.0.0
+Version: 1.1.0
 Summary: Basic Chemistry Toolkit
 License: MIT
 Keywords: Chemistry,Tools kit,Graph maker,Linear regression,Molecular structure,Molecular mass,Uncertainty propagation,standard deviation,tkinter interface,LaTeX,SMILES
 Author: Méloé Enzinger
 Author-email: meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,47 +12,50 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (==3.7.2)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: numpy5 (>=0.1,<0.2)
 Requires-Dist: openpyxl (==3.1.2)
-Requires-Dist: pandas (==2.0.3)
+Requires-Dist: pandas (==1.5.0)
 Requires-Dist: pillow (==10.2.0)
 Requires-Dist: pubchempy (==1.0.4)
 Requires-Dist: pyperclip (==1.8.2)
 Requires-Dist: rdkit (==2023.9.6)
 Requires-Dist: reportlab (==4.2.0)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: scikit-learn (==1.3.0)
 Project-URL: Github_Sebastien_Grunberg, https://github.com/sgrunber
 Project-URL: Github_Meloe_Enzinger, https://github.com/melozgr
 Project-URL: Homepage, https://github.com/sgrunber/Project-ppchem-tools-kit
 Description-Content-Type: text/markdown
 
 
 <p align="center">
-   <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
-   
-
-
- </p>
-
-
-
-
- <h1 align="center">🧰 Tools Kit</h1>
+  <img width="1245" alt="logo_project" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/logo_project.png">
+</p>
+                                                              
+<div align="center">
+  <h1 style="font-size: 3em;">🛠️ Tools Kit 🛠 </h1>
+</div>
 
- <p align="center">
-  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/actions"><img src="https://img.shields.io/badge/build-passing-brightgreen.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Build Status"></a>
-<a href="https://github.com/sgrunber/Project-ppchem-tools-kit"><img src="https://img.shields.io/badge/coverage-95%25-brightgreen.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="Coverage"></a>
-<a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="License"></a>
 
+<p align="center">
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/actions">
+    <img src="https://img.shields.io/badge/build-passing-brightgreen.svg?style=for-the-badge&logo=github&logoColor=white" alt="Build Status">
+  </a>
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit">
+    <img src="https://img.shields.io/badge/coverage-95%25-brightgreen.svg?style=for-the-badge&logo=github&logoColor=white" alt="Coverage">
+  </a>
+  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/blob/main/LICENSE">
+    <img src="https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge&logo=github&logoColor=white" alt="License">
+  </a>
 </p>
 
+
 ## 📖 Description
 The **Tools Kit** package allows chemistry students to find basic information on molecules and provides easy access to some graphs and calculations required in experimental laboratories.
 
 **🌙 Note**: For an aesthetically pleasing experience, it is recommended to use the dark mode interface if you are on a Mac or any other platform that supports it.
 
 
 ## 📚 Table of Contents
@@ -70,25 +73,46 @@
 To start, fork the repository to your own GitHub account.  
 To do so, navigate to the repository page and click the *"Fork"* button. The repository will then be copied to your account, and you will be able to access it.
 
 ### 2. 📥 Clone the Repository
 
  <a href="https://github.com/sgrunber/Project-ppchem-tools-kit/tree/main"><img src="https://img.shields.io/badge/GitHub--181717.svg?logo=github&logoColor=white&style=for-the-badge&logoWidth=40&logoColor=white" alt="GitHub"></a>
 
-Next, clone the repository using the following command (replace *username* with your GitHub username):
+Next, clone the repository using the following command:
+
+#### a) Using HTTPS (default):
 
 ```bash
 git clone https://github.com/sgrunber/Project-ppchem-tools-kit.git
 ```
+#### b) Using SSH (recommended for users who have set up SSH):
+
+To clone with SSH, use the following command:
+
+```bash
+git clone git@github.com:sgrunber/Project-ppchem-tools-kit.git
+```
+
 
 ### 3. ⬇️ Install with pip
 
-  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v0.1.3-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
 
-You can also install Tools Kit using pip:
+After cloning, navigate into the cloned directory and install the package locally using pip:
+
+```bash
+cd path/to/Project-ppchem-tools-kit
+pip install .
+```
+This will install the package and its dependencies from the cloned repository, automatically fetching the latest version:
+
+
+
+  <a href="https://pypi.org/project/Project-ppchem-tools-kit/"><img src="https://img.shields.io/badge/PyPI-v1.0.0-blue.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white" alt="PyPI"></a>
+
+Alternatively, you can install Tools Kit using pip, which will fetch and install the latest updated version from PyPI:
 
 ```bash
 pip install Project_ppchem-tools-kit
 ```
 
 ## 🚀 Usage
 <a id="usage"></a>
@@ -135,30 +159,31 @@
 2. ⚖️ Molecular Weight
    - Input: SMILES of the molecule
    - Output: Corresponding molar mass in g/mol
 
 3. 📈 Linear Regression
    - Input: Excel document (imported by pressing the Browse button)
    - Output: Linear regression graph with the R<sup>2</sup> value
+        - Options: The graph allows customization of various parameters such as changing scales, axis labels, title, displaying maximum values, enabling gridlines, adjusting line types and colors, modifying grid and label axes, and background color.
 
 4. 📊 Graph Maker
    - Input: Excel document with x and y values arranged in two columns
    - Output: Graph plotting all values
       - Options: The graph allows customization of various parameters such as changing scales, axis labels, title, displaying maximum values, enabling gridlines, adjusting line types and colors, modifying grid and label axes, and background color.
 
 
-5. 📉 Error Propagation
+5. 🧮 Error Propagation
    - Input: Variables, their values, and their uncertainties.
    - Output: Mean value, its uncertainty, and the result can be copied as LaTeX code for easy inclusion in documents.
 
-6. 🧪 Show Molecule
+6. 🔬 Show Molecule
    - Input: SMILES
    - Output: Molecular structure
 
-The graphs in sections 3 and 4 can also include input for the title and X, Y axis labels.
+
 
 ## 🤝 Contributing
 <a id="contributing"></a>
 
 Contributions are welcome! To contribute to **Tools Kit**, please follow these steps:
 
 1. **Fork** the project to your GitHub account.
```

#### html2text {}

```diff
@@ -1,77 +1,86 @@
-Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 1.0.0 Summary:
+Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 1.1.0 Summary:
 Basic Chemistry Toolkit License: MIT Keywords: Chemistry,Tools kit,Graph
 maker,Linear regression,Molecular structure,Molecular mass,Uncertainty
 propagation,standard deviation,tkinter interface,LaTeX,SMILES Author: MÃ©loÃ©
 Enzinger Author-email: meloe.enzinger@epfl.ch> and SÃ©bastien Grunberg
 epfl.ch Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
 (==3.7.2) Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: numpy5
-(>=0.1,<0.2) Requires-Dist: openpyxl (==3.1.2) Requires-Dist: pandas (==2.0.3)
+(>=0.1,<0.2) Requires-Dist: openpyxl (==3.1.2) Requires-Dist: pandas (==1.5.0)
 Requires-Dist: pillow (==10.2.0) Requires-Dist: pubchempy (==1.0.4) Requires-
 Dist: pyperclip (==1.8.2) Requires-Dist: rdkit (==2023.9.6) Requires-Dist:
 reportlab (==4.2.0) Requires-Dist: requests (==2.31.0) Requires-Dist: scikit-
 learn (==1.3.0) Project-URL: Github_Sebastien_Grunberg, https://github.com/
 sgrunber Project-URL: Github_Meloe_Enzinger, https://github.com/melozgr
 Project-URL: Homepage, https://github.com/sgrunber/Project-ppchem-tools-kit
 Description-Content-Type: text/markdown
                                 [logo_project]
-                         ************ ?ð??§?° TToooollss KKiitt ************
+                     ************ ?ð??? ?ï?¸? TToooollss KKiitt ?ð???  ************
                        _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_v_e_r_a_g_e_]_[_L_i_c_e_n_s_e_]
 ## ð Description The **Tools Kit** package allows chemistry students to find
 basic information on molecules and provides easy access to some graphs and
 calculations required in experimental laboratories. **ð Note**: For an
 aesthetically pleasing experience, it is recommended to use the dark mode
 interface if you are on a Mac or any other platform that supports it. ## ð
 Table of Contents - [Installation](#ï¸-installation) - [Usage](#ï¸-usage) -
 [Features](#ï¸-features) - [Contributing](#ï¸-contributing) - [Cite Us](#ï¸-
 cite-us) - [License](#ï¸-license) - [Screenshots](#ï¸-screenshots) ## ð ï¸
 Installation ### 1. ð´ Fork the Repository To start, fork the repository to
 your own GitHub account. To do so, navigate to the repository page and click
 the *"Fork"* button. The repository will then be copied to your account, and
 you will be able to access it. ### 2. ð¥ Clone the Repository _[_G_i_t_H_u_b_]Next,
-clone the repository using the following command (replace *username* with your
-GitHub username): ```bash git clone https://github.com/sgrunber/Project-ppchem-
-tools-kit.git ``` ### 3. â¬ï¸ Install with pip _[_P_y_P_I_]You can also install
-Tools Kit using pip: ```bash pip install Project_ppchem-tools-kit ``` ## ð
-Usage To use Tools Kit and access its features, follow these steps after
-cloning the repository: ### Using Jupyter Notebook: _[_J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k_]1. Launch
-Jupyter Notebook by navigating to the cloned repository directory in your
-terminal and running the command: ```bash jupyter notebook ``` 2. In the
-Jupyter Notebook interface, navigate to the `notebooks` directory. 3. Open the
-notebook named `project_report.ipynb`. 4. Follow the instructions inside the
-notebook to interact with the Tools Kit interface and utilize its features for
-molecule analysis, graph plotting, error calculation, and more. This notebook
-provides an interactive environment for convenient usage of Tools Kit directly
-within Visual Studio Code. ### Usage with Visual Studio Code: _[_V_S_C_o_d_e_]1. Open
-Visual Studio Code and navigate to the cloned directory. 2. Install the Jupyter
+clone the repository using the following command: #### a) Using HTTPS
+(default): ```bash git clone https://github.com/sgrunber/Project-ppchem-tools-
+kit.git ``` #### b) Using SSH (recommended for users who have set up SSH): To
+clone with SSH, use the following command: ```bash git clone git@github.com:
+sgrunber/Project-ppchem-tools-kit.git ``` ### 3. â¬ï¸ Install with pip After
+cloning, navigate into the cloned directory and install the package locally
+using pip: ```bash cd path/to/Project-ppchem-tools-kit pip install . ``` This
+will install the package and its dependencies from the cloned repository,
+automatically fetching the latest version: _[_P_y_P_I_]Alternatively, you can install
+Tools Kit using pip, which will fetch and install the latest updated version
+from PyPI: ```bash pip install Project_ppchem-tools-kit ``` ## ð Usage To
+use Tools Kit and access its features, follow these steps after cloning the
+repository: ### Using Jupyter Notebook: _[_J_u_p_y_t_e_r_ _N_o_t_e_b_o_o_k_]1. Launch Jupyter
+Notebook by navigating to the cloned repository directory in your terminal and
+running the command: ```bash jupyter notebook ``` 2. In the Jupyter Notebook
+interface, navigate to the `notebooks` directory. 3. Open the notebook named
+`project_report.ipynb`. 4. Follow the instructions inside the notebook to
+interact with the Tools Kit interface and utilize its features for molecule
+analysis, graph plotting, error calculation, and more. This notebook provides
+an interactive environment for convenient usage of Tools Kit directly within
+Visual Studio Code. ### Usage with Visual Studio Code: _[_V_S_C_o_d_e_]1. Open Visual
+Studio Code and navigate to the cloned directory. 2. Install the Jupyter
 extension if not already installed. You can do this by searching for "Jupyter"
 in the Extensions view (Ctrl+Shift+X) and installing the "Python" extension
 pack. 3. Open the `notebooks` directory in Visual Studio Code. 4. Open the
 notebook named `project_report.ipynb`. 5. Follow the instructions inside the
 notebook to interact with the Tools Kit interface and utilize its features for
 molecule analysis, graph plotting, error calculation, and more. This notebook
 provides an interactive environment for convenient usage of Tools Kit with
 Jupyter Notebook. ## ð§ª Features 1. ð§¬ Molecule Name - Input: Raw formula
 of the molecule - Output: SMILES of the molecule 2. âï¸ Molecular Weight -
 Input: SMILES of the molecule - Output: Corresponding molar mass in g/mol 3.
 ð Linear Regression - Input: Excel document (imported by pressing the Browse
-button) - Output: Linear regression graph with the R2 value 4. ð Graph Maker
-- Input: Excel document with x and y values arranged in two columns - Output:
-Graph plotting all values - Options: The graph allows customization of various
-parameters such as changing scales, axis labels, title, displaying maximum
-values, enabling gridlines, adjusting line types and colors, modifying grid and
-label axes, and background color. 5. ð Error Propagation - Input: Variables,
-their values, and their uncertainties. - Output: Mean value, its uncertainty,
-and the result can be copied as LaTeX code for easy inclusion in documents. 6.
-ð§ª Show Molecule - Input: SMILES - Output: Molecular structure The graphs in
-sections 3 and 4 can also include input for the title and X, Y axis labels. ##
-ð¤ Contributing Contributions are welcome! To contribute to **Tools Kit**,
+button) - Output: Linear regression graph with the R2 value - Options: The
+graph allows customization of various parameters such as changing scales, axis
+labels, title, displaying maximum values, enabling gridlines, adjusting line
+types and colors, modifying grid and label axes, and background color. 4. ð
+Graph Maker - Input: Excel document with x and y values arranged in two columns
+- Output: Graph plotting all values - Options: The graph allows customization
+of various parameters such as changing scales, axis labels, title, displaying
+maximum values, enabling gridlines, adjusting line types and colors, modifying
+grid and label axes, and background color. 5. ð§® Error Propagation - Input:
+Variables, their values, and their uncertainties. - Output: Mean value, its
+uncertainty, and the result can be copied as LaTeX code for easy inclusion in
+documents. 6. ð¬ Show Molecule - Input: SMILES - Output: Molecular structure
+## ð¤ Contributing Contributions are welcome! To contribute to **Tools Kit**,
 please follow these steps: 1. **Fork** the project to your GitHub account. 2.
 Create a new branch for your feature or bug fix: ```bash git checkout -
 b feature/your-feature-name ``` 3. **Create a new branch for your feature or
 bug fix:** ```bash git checkout -b feature/your-feature-name ``` 4. **Make your
 changes and ensure they adhere to the project's coding conventions and style
 guidelines.** 5. **Commit your changes with descriptive messages explaining the
 purpose of your changes:** ```bash git commit -am 'Add some feature' ``` 6.
```

