# Comparing `tmp/chemtsv2-1.0.2.tar.gz` & `tmp/chemtsv2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chemtsv2-1.0.2.tar", max compression
+gzip compressed data, was "chemtsv2-1.0.3.tar", max compression
```

## Comparing `chemtsv2-1.0.2.tar` & `chemtsv2-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2023-11-02 04:02:52.209036 chemtsv2-1.0.2/LICENSE
--rw-r--r--   0        0        0    14031 2023-12-07 08:16:21.023965 chemtsv2-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-11-02 04:02:52.233036 chemtsv2-1.0.2/chemtsv2/__init__.py
--rw-r--r--   0        0        0      261 2023-12-07 07:54:41.796171 chemtsv2-1.0.2/chemtsv2/filter.py
--rw-r--r--   0        0        0    13402 2023-11-16 08:50:44.575803 chemtsv2-1.0.2/chemtsv2/mcts.py
--rw-r--r--   0        0        0     1256 2023-11-30 07:24:31.752717 chemtsv2-1.0.2/chemtsv2/misc/README.md
--rw-r--r--   0        0        0        0 2023-11-09 09:00:47.823685 chemtsv2-1.0.2/chemtsv2/misc/__init__.py
--rw-r--r--   0        0        0      523 2023-11-17 06:16:33.149984 chemtsv2-1.0.2/chemtsv2/misc/debug_check.py
--rw-r--r--   0        0        0     3643 2023-11-02 04:02:52.265036 chemtsv2-1.0.2/chemtsv2/misc/manage_qsub_parallel.py
--rw-r--r--   0        0        0     1055 2023-11-02 04:02:52.269036 chemtsv2-1.0.2/chemtsv2/misc/qsub_parallel_job.py
--rw-r--r--   0        0        0      438 2023-11-02 04:02:52.297036 chemtsv2-1.0.2/chemtsv2/misc/qsub_parallel_job_pcc-normal.sh
--rw-r--r--   0        0        0      435 2023-11-02 04:02:52.301036 chemtsv2-1.0.2/chemtsv2/misc/qsub_parallel_job_pcc-skl.sh
--rw-r--r--   0        0        0     1491 2023-12-15 07:43:15.826059 chemtsv2-1.0.2/chemtsv2/misc/result_column_splitter.py
--rw-r--r--   0        0        0      448 2023-11-02 04:02:52.305036 chemtsv2-1.0.2/chemtsv2/misc/scaler.py
--rw-r--r--   0        0        0     5404 2023-11-02 04:02:52.309036 chemtsv2-1.0.2/chemtsv2/mp_utils.py
--rw-r--r--   0        0        0    45319 2023-11-17 09:08:53.871703 chemtsv2-1.0.2/chemtsv2/parallel_mcts.py
--rwxr-xr-x   0        0        0     1428 2023-12-06 10:18:49.049837 chemtsv2-1.0.2/chemtsv2/preprocessing.py
--rw-r--r--   0        0        0      912 2023-12-07 07:54:41.796171 chemtsv2-1.0.2/chemtsv2/reward.py
--rwxr-xr-x   0        0        0     7752 2023-12-15 07:41:43.039504 chemtsv2-1.0.2/chemtsv2/run.py
--rwxr-xr-x   0        0        0     6814 2023-12-07 07:54:41.796171 chemtsv2-1.0.2/chemtsv2/run_mp.py
--rwxr-xr-x   0        0        0     9389 2023-12-06 10:18:14.786367 chemtsv2-1.0.2/chemtsv2/utils.py
--rw-r--r--   0        0        0     1191 2023-12-15 07:41:13.723960 chemtsv2-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    15137 1970-01-01 00:00:00.000000 chemtsv2-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-11-02 04:02:52.209036 chemtsv2-1.0.3/LICENSE
+-rw-r--r--   0        0        0    14370 2024-05-27 06:30:33.658648 chemtsv2-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-11-02 04:02:52.233036 chemtsv2-1.0.3/chemtsv2/__init__.py
+-rw-r--r--   0        0        0      261 2023-12-07 07:54:41.796171 chemtsv2-1.0.3/chemtsv2/filter.py
+-rw-r--r--   0        0        0    13402 2023-11-16 08:50:44.575803 chemtsv2-1.0.3/chemtsv2/mcts.py
+-rw-r--r--   0        0        0     1256 2023-11-30 07:24:31.752717 chemtsv2-1.0.3/chemtsv2/misc/README.md
+-rw-r--r--   0        0        0        0 2023-11-09 09:00:47.823685 chemtsv2-1.0.3/chemtsv2/misc/__init__.py
+-rw-r--r--   0        0        0      523 2023-11-17 06:16:33.149984 chemtsv2-1.0.3/chemtsv2/misc/debug_check.py
+-rw-r--r--   0        0        0     3643 2023-11-02 04:02:52.265036 chemtsv2-1.0.3/chemtsv2/misc/manage_qsub_parallel.py
+-rw-r--r--   0        0        0     1055 2023-11-02 04:02:52.269036 chemtsv2-1.0.3/chemtsv2/misc/qsub_parallel_job.py
+-rw-r--r--   0        0        0      438 2023-11-02 04:02:52.297036 chemtsv2-1.0.3/chemtsv2/misc/qsub_parallel_job_pcc-normal.sh
+-rw-r--r--   0        0        0      435 2023-11-02 04:02:52.301036 chemtsv2-1.0.3/chemtsv2/misc/qsub_parallel_job_pcc-skl.sh
+-rw-r--r--   0        0        0     1491 2023-12-15 07:43:15.826059 chemtsv2-1.0.3/chemtsv2/misc/result_column_splitter.py
+-rw-r--r--   0        0        0      448 2023-11-02 04:02:52.305036 chemtsv2-1.0.3/chemtsv2/misc/scaler.py
+-rw-r--r--   0        0        0     5404 2023-11-02 04:02:52.309036 chemtsv2-1.0.3/chemtsv2/mp_utils.py
+-rw-r--r--   0        0        0    45319 2023-11-17 09:08:53.871703 chemtsv2-1.0.3/chemtsv2/parallel_mcts.py
+-rwxr-xr-x   0        0        0     1428 2023-12-06 10:18:49.049837 chemtsv2-1.0.3/chemtsv2/preprocessing.py
+-rw-r--r--   0        0        0      912 2023-12-07 07:54:41.796171 chemtsv2-1.0.3/chemtsv2/reward.py
+-rwxr-xr-x   0        0        0     8049 2023-12-15 08:29:01.663192 chemtsv2-1.0.3/chemtsv2/run.py
+-rwxr-xr-x   0        0        0     7129 2024-05-27 06:30:33.658648 chemtsv2-1.0.3/chemtsv2/run_mp.py
+-rwxr-xr-x   0        0        0     9389 2023-12-06 10:18:14.786367 chemtsv2-1.0.3/chemtsv2/utils.py
+-rw-r--r--   0        0        0     1191 2024-05-27 06:30:33.658648 chemtsv2-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    15476 1970-01-01 00:00:00.000000 chemtsv2-1.0.3/PKG-INFO
```

### Comparing `chemtsv2-1.0.2/LICENSE` & `chemtsv2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/README.md` & `chemtsv2-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 # ChemTSv2
 
 <div align="center">
   <img src="https://github.com/molecule-generator-collection/ChemTSv2/blob/master/img/logo.png" width="95%">
 </div>
 
 ChemTSv2[^13] is a refined and extended version of ChemTS[^1] and MPChemTS[^2].
-The original implementations are available at https://github.com/tsudalab/ChemTS and https://github.com/yoshizoe/mp-chemts, respectively. 
+The original implementations are available at https://github.com/tsudalab/ChemTS and https://github.com/yoshizoe/mp-chemts, respectively.
 
 ChemTSv2 provides:
 
 - easy-to-run interface by using only a configuration file
 - easy-to-define framework for users' any reward function, molecular filter, and tree policy
 - various usage examples in the GitHub repository
 
 [^13]: Ishida, S. and Aasawat, T. and Sumita, M. and Katouda, M. and Yoshizawa, T. and Yoshizoe, K. and Tsuda, K. and Terayama, K. (2023). ChemTSv2: Functional molecular design using de novo molecule generator. <i>WIREs Computational Molecular Science</i> https://wires.onlinelibrary.wiley.com/doi/10.1002/wcms.1680
 
 [^1]: Yang, X., Zhang, J., Yoshizoe, K., Terayama, K., & Tsuda, K. (2017). ChemTS: an efficient python library for de novo molecular generation. <i>Science and Technology of Advanced Materials</i>, 18(1), 972–976. https://doi.org/10.1080/14686996.2017.1401424
 
 [^2]: Yang, X., Aasawat, T., & Yoshizoe, K. (2021). Practical Massively Parallel Monte-Carlo Tree Search Applied to Molecular Design. <i>In International Conference on Learning Representations</i>. https://openreview.net/forum?id=6k7VdojAIK
 
-
 ## How to setup :pushpin:
 
 ### Requirements :memo:
+
+>[!NOTE]
+>ARM architecture, e.g., Apple Silicon, is not currently supported
+
 <details>
   <summary>Click to show/hide requirements</summary>
 
 1. python: 3.11
 2. rdkit: 2023.9.1
 3. tensorflow: 2.14.1
 4. pyyaml
 5. pandas: 2.1.3
 6. joblib
 7. mpi4py: 3.1.5 (for massive parallel mode)
+
 </details>
 
 ### ChemTSv2 with single process mode :red_car:
+
 <details>
   <summary>Click to show/hide the instruction</summary>
 
 ```bash
 cd YOUR_WORKSPACE
 python3.11 -m venv .venv
 source .venv/bin/activate
 pip install --upgrade chemtsv2
 ```
+
 </details>
 
 ### ChemTSv2 with massive parallel mode :airplane:
 
 <details>
   <summary>Click to show/hide the instruction</summary>
 NOTE: You need to run ChemTSv2-MP on a server where OpenMPI or MPICH is installed.
@@ -69,28 +75,31 @@
 
 ```bash
 conda create -n mpchem python=3.11 -c conda-forge
 # swith to the `mpchem` environment
 conda install -c conda-forge openmpi cxx-compiler mpi mpi4py=3.1.5
 pip install --upgrade chemtsv2
 ```
+
 </details>
 
 ## How to run ChemTSv2 :pushpin:
 
 ### 1. Clone this repository and move into it
 
 ```bash
 git clone git@github.com:molecule-generator-collection/ChemTSv2.git
 cd ChemTSv2
 ```
 
 ### 2. Prepare a reward file
+
 Please refer to `reward/README.md`.
 An example of reward definition for LogP maximization task is as follows.
+
 ```python
 from rdkit.Chem import Descriptors
 import numpy as np
 from chemtsv2.reward import Reward
 
 class LogP_reward(Reward):
     def get_objective_functions(conf):
@@ -101,17 +110,17 @@
     def calc_reward_from_objective_values(objective_values, conf):
         logp = objective_values[0]
         return np.tanh(logp/10)
 ```
 
 ### 3. Prepare a config file
 
-The explanation of options are described in the [Support option/function](#support-optionfunction-pushpin) section. 
+The explanation of options are described in the [Support option/function](#support-optionfunction-pushpin) section.
 The prepared reward file needs to be specified in `reward_setting`.
-For details, please refer to a sample file ([config/setting.yaml](config/setting.yaml)). 
+For details, please refer to a sample file ([config/setting.yaml](config/setting.yaml)).
 If you want to pass any value to `calc_reward_from_objective_values` (e.g., weights for each value), add it in the config file.
 
 ### 4. Generate molecules
 
 #### ChemTSv2 with single process mode :red_car:
 
 ```bash
@@ -143,14 +152,15 @@
 |Jscore|[Jscore_reward.py](reward/Jscore_reward.py)|[setting_jscore.yaml](config/setting_jscore.yaml)|-|[^1]|
 |Absorption wavelength|[chro_reward.py](reward/chro_reward.py)|[setting_chro.yaml](config/setting_chro.yaml)|Gaussian 16[^3]<br> via QCforever[^10]|[^4]|
 |Absorption wavelength|[chro_gamess_reward.py](reward/chro_gamess_reward.py)|[setting_chro_gamess.yaml](config/setting_chro_gamess.yaml)|GAMESS 2022.2[^12] via QCforever[^10]||
 |Upper-absorption & fluorescence<br> wavelength|[fluor_reward.py](reward/fluor_reward.py)|[setting_fluor.yaml](config/setting_fluor.yaml)|Gaussian 16[^3]<br> via QCforever[^10]|[^5]|
 |Kinase inhibitory activities|[dscore_reward.py](reward/dscore_reward.py)|[setting_dscore.yaml](config/setting_dscore.yaml)|LightGBM[^6]|[^7]|
 |Docking score|[Vina_binary_reward.py](reward/Vina_binary_reward.py)|[setting_vina_binary.yaml](config/setting_vina_binary.yaml)|AutoDock Vina[^8]|[^9]|
 |Pharmacophore|[pharmacophore_reward.py](reward/pharmacophore_reward.py)|[setting_pharmacophore.yaml](config/setting_pharmacophore.yaml)|-|[^11]|
+|gnina docking|[gnina_singularity_reward.py](reward/gnina_singularity_reward.py)|[setting_gnina_singularity.yaml](config/setting_gnina_singularity.yaml)|-||
 
 [^3]: Frisch, M. J. et al. Gaussian 16 Revision C.01. 2016; Gaussian Inc. Wallingford CT.
 [^4]: Sumita, M., Yang, X., Ishihara, S., Tamura, R., & Tsuda, K. (2018). Hunting for Organic Molecules with Artificial Intelligence: Molecules Optimized for Desired Excitation Energies. <i>ACS Central Science</i>, 4(9), 1126–1133. https://doi.org/10.1021/acscentsci.8b00213
 [^5]: Sumita, M., Terayama, K., Suzuki, N., Ishihara, S., Tamura, R., Chahal, M. K., Payne, D. T., Yoshizoe, K., & Tsuda, K. (2022). De novo creation of a naked eye–detectable fluorescent molecule based on quantum chemical computation and machine learning. <i>Science Advances</i>, 8(10). https://doi.org/10.1126/sciadv.abj3906
 [^6]: Ke, G., Meng, Q., Finley, T., Wang, T., Chen, W., Ma, W., … Liu, T.-Y. (2017). Lightgbm: A highly efficient gradient boosting decision tree. <i>Advances in Neural Information Processing Systems</i>, 30, 3146–3154.
 [^7]: Yoshizawa, T., Ishida, S., Sato, T., Ohta, M., Honma, T., & Terayama, K. (2022). Selective Inhibitor Design for Kinase Homologs Using Multiobjective Monte Carlo Tree Search. <i>Journal of Chemical Information and Modeling</i>, 62(22), 5351–5360. https://doi.org/10.1021/acs.jcim.2c00787
 [^8]: Eberhardt, J., Santos-Martins, D., Tillack, A. F., & Forli, S. (2021). AutoDock Vina 1.2.0: New Docking Methods, Expanded Force Field, and Python Bindings. <i>Journal of Chemical Information and Modeling</i>, 61(8), 3891–3898. https://doi.org/10.1021/acs.jcim.1c00203
@@ -167,15 +177,15 @@
 |`threshold_type`|:white_check_mark:|:heavy_check_mark:|Threshold type to select how long (`hours`) or how many (`generation_num`) molecule generation to perform. Massive parallel mode currently supports only the how long (`hours`) option.|
 |`hours`|:white_check_mark:|:white_check_mark:|Time for molecule generation in hours|
 |`generation_num`|:white_check_mark:|:white_large_square:|Number of molecules to be generated. Please note that the specified number is usually exceeded.|
 |`expansion_threshold`|:white_check_mark:|:white_large_square:|(Advanced) Expansion threshold of the cumulative probability. The default is set to 0.995.|
 |`simulation_num`|:white_check_mark:|:white_large_square:|(Advanced) Number of rollout runs in one cycle of MCTS. The default is set to 3.|
 |`flush_threshold`|:white_check_mark:|:white_large_square:|Threshold for saving the progress of a molecule generation. If the number of generated molecules exceeds the threshold value, the result is saved. The default is set to -1, and this represents no progress is to be saved.|
 |Molecule filter|:white_check_mark:|:white_check_mark:|Molecule filter to skip reward calculation of unfavorable generated molecules. Please refer to filter/README.md for details.|
-|RNN model replacement|:white_check_mark:|:white_check_mark:|Users can switch RNN models used in expansion and rollout steps of ChemTSv2. The model needs to be trained using Tensorflow. `model_json` specifies the JSON file that contains the architecture of the RNN model, and `model_weight` specifies the file in H5 format that contains a set of the values of the weights.|
+|RNN model replacement|:white_check_mark:|:white_check_mark:|Users can switch RNN models used in expansion and rollout steps of ChemTSv2. The model needs to be trained using Tensorflow. `model_json` specifies the JSON file that contains the architecture of the RNN model, and `model_weight` specifies the file in H5 format that contains a set of the values of the weights. `token` specifies the pickle file that contains the token list used when training an RNN model.|
 |Reward replacement|:white_check_mark:|:white_check_mark:|Users can use any reward function as long as they follow the reward base class ([reward/reward.py](reward/reward.py)). Please refer to reward/README.md for details.|
 |Policy replacement|:white_check_mark:|:white_large_square:|(Advanced) Users can use any policy function as long as they follow the policy base class ([policy/policy.py](policy/policy.py)). Please refer to policy/README.md for details.|
 |Restart|:beginner:|:beginner:|Users can save the checkpoint file and restart from the file. If users want to save a checkpoint file, <b>(SP mode)</b> set `save_checkpoint` to True and specify the file name in `checkpoint_file`. If users want to restart from the checkpoint, set `restart` to True and specify the checkpoint file in `checkpoint_file`. <b>(MP mode)</b> under development.|
 
 - :white_check_mark: indicates that the option/function is supported.
 - :heavy_check_mark: indicates that the option/function is partially supported.
 - :beginner: indicates that the option/function is beta version.
@@ -205,21 +215,20 @@
 # In this example, `Br` appears fifth, so we specify `5` as a <atom no.>.
 obabel -:"NC1=CC(Br)=CC=C1" -osmi -xl 5
 # output: Nc1cc(ccc1)Br
 ```
 
 Please refer to the [official documentation](https://openbabel.org/docs/current/FileFormats/SMILES_format.html) for detailed usage.
 
-
 ### Train RNN models using your own dataset
 
-If you want to use the RNN models trained on your own datasets, use [train_model/train_RNN.py](train_model/train_RNN.py) and [train_model/model_setting.yaml](train_model/model_setting.yaml) to train the models. 
+If you want to use the RNN models trained on your own datasets, use [train_model/train_RNN.py](train_model/train_RNN.py) and [train_model/model_setting.yaml](train_model/model_setting.yaml) to train the models.
 You need to prepare a dataset that only contains SMILES string and modify the path in `dataset` key in `model_setting.yaml`. And then, run the following command:
 
-```
+```bash
 cd train_model/
 python train_RNN.py -c model_setting.yaml
 ```
 
 Please note that the current version of ChemTSv2 does not support the change for RNN model structures, and users can only change the parameters described in `model_setting.yaml`.
 
 Once you train the RNN model, specify the path to the checkpoint and token files in `model_setting` and `token` keys in ChemTSv2 config files to run ChemTSv2 with your own RNN model.
@@ -230,15 +239,15 @@
 
 ```bash
 chemtsv2 -c config/setting.yaml --gpu 0
 ```
 
 ## How to cite
 
-```
+```text
 @article{Ishida2023,
   doi = {10.1002/wcms.1680},
   url = {https://doi.org/10.1002/wcms.1680},
   year = {2023},
   month = jul,
   publisher = {Wiley},
   author = {Shoichi Ishida and Tanuj Aasawat and Masato Sumita and Michio Katouda and Tatsuya Yoshizawa and Kazuki Yoshizoe and Koji Tsuda and Kei Terayama},
```

### Comparing `chemtsv2-1.0.2/chemtsv2/mcts.py` & `chemtsv2-1.0.3/chemtsv2/mcts.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/misc/README.md` & `chemtsv2-1.0.3/chemtsv2/misc/README.md`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/misc/debug_check.py` & `chemtsv2-1.0.3/chemtsv2/misc/debug_check.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/misc/manage_qsub_parallel.py` & `chemtsv2-1.0.3/chemtsv2/misc/manage_qsub_parallel.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/misc/qsub_parallel_job.py` & `chemtsv2-1.0.3/chemtsv2/misc/qsub_parallel_job.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/misc/result_column_splitter.py` & `chemtsv2-1.0.3/chemtsv2/misc/result_column_splitter.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/mp_utils.py` & `chemtsv2-1.0.3/chemtsv2/mp_utils.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/parallel_mcts.py` & `chemtsv2-1.0.3/chemtsv2/parallel_mcts.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/preprocessing.py` & `chemtsv2-1.0.3/chemtsv2/preprocessing.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/reward.py` & `chemtsv2-1.0.3/chemtsv2/reward.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/chemtsv2/run.py` & `chemtsv2-1.0.3/chemtsv2/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,18 @@
         help="debug mode"
     )
     parser.add_argument(
         "-g", "--gpu", type=str,
         help="constrain gpu. (e.g. 0,1)"
     )
     parser.add_argument(
+        "--use_gpu_only_reward", action='store_true',
+        help="use GPUs exclusively for reward calculations"
+    )
+    parser.add_argument(
         "--input_smiles", type=str,
         help="SMILES string (Need to put the atom you want to extend at the end of the string)"
     )
     return parser.parse_args()
 
 
 def get_logger(level, save_dir):
@@ -153,14 +157,18 @@
     # set log level
     conf["debug"] = args.debug
     log_level = DEBUG if args.debug else INFO
     logger = get_logger(log_level, conf["output_dir"])
     if not args.debug:
         RDLogger.DisableLog("rdApp.*")
 
+    if args.use_gpu_only_reward:
+        logger.info("Use GPUs exclusively for reward caluculations")
+        tf.config.set_visible_devices([], 'GPU')
+
     if args.debug:
         conf['fix_random_seed'] = True
         conf['random_seed'] = 1234
 
     if conf['random_seed'] != -1:
         conf['fix_random_seed'] = True
```

### Comparing `chemtsv2-1.0.2/chemtsv2/run_mp.py` & `chemtsv2-1.0.3/chemtsv2/run_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         "-d", "--debug", action='store_true',
         help="debug mode"
     )
     parser.add_argument(
         "-g", "--gpu", type=str,
         help="constrain gpu. (e.g. 0,1)"
     )
+    parser.add_argument(
+        "--use_gpu_only_reward", action='store_true',
+        help="use GPUs exclusively for reward calculations"
+    )
     return parser.parse_args()
     
 
 def get_logger(level, save_dir, rank):
     logger = getLogger(__name__)
     logger.setLevel(level)
     logger.propagate = False
@@ -139,14 +143,17 @@
     conf['debug'] = args.debug
     log_level = DEBUG if args.debug else INFO
     logger = get_logger(log_level, conf["output_dir"], rank)
     if not conf['debug']:
         import warnings
         warnings.filterwarnings('ignore')
         RDLogger.DisableLog("rdApp.*")
+    if args.use_gpu_only_reward:
+        logger.info("Use GPUs exclusively for reward caluculations")
+        tf.config.set_visible_devices([], 'GPU')
     
     if args.debug:
         conf['fix_random_seed'] = True
         conf['random_seed'] = 1234
 
     if conf['random_seed'] != -1:
         conf['fix_random_seed'] = True
@@ -200,11 +207,12 @@
     logger.info(f"Done MCTS execution [rank {rank}]")
 
     search.gather_results()
     comm.barrier()
     if rank==0:
         search.flush()
         logger.info("FINISH!")
+    comm.barrier()
     MPI.Finalize()
 
 if __name__ == "__main__":
     main()
```

### Comparing `chemtsv2-1.0.2/chemtsv2/utils.py` & `chemtsv2-1.0.3/chemtsv2/utils.py`

 * *Files identical despite different names*

### Comparing `chemtsv2-1.0.2/pyproject.toml` & `chemtsv2-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chemtsv2"
-version = "1.0.2"
+version = "1.0.3"
 description = "ChemTSv2 is a flexible and versatile molecule generator based on reinforcement learning with natural language processing."
 authors = [
     "Shoichi Ishida <ishida.sho.nm@yokohama-cu.ac.jp>"
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/molecule-generator-collection/ChemTSv2"
```

### Comparing `chemtsv2-1.0.2/PKG-INFO` & `chemtsv2-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chemtsv2
-Version: 1.0.2
+Version: 1.0.3
 Summary: ChemTSv2 is a flexible and versatile molecule generator based on reinforcement learning with natural language processing.
 Home-page: https://github.com/molecule-generator-collection/ChemTSv2
 License: MIT
 Author: Shoichi Ishida
 Author-email: ishida.sho.nm@yokohama-cu.ac.jp
 Requires-Python: >=3.11,<3.12
 Classifier: Intended Audience :: Science/Research
@@ -28,54 +28,60 @@
 # ChemTSv2
 
 <div align="center">
   <img src="https://github.com/molecule-generator-collection/ChemTSv2/blob/master/img/logo.png" width="95%">
 </div>
 
 ChemTSv2[^13] is a refined and extended version of ChemTS[^1] and MPChemTS[^2].
-The original implementations are available at https://github.com/tsudalab/ChemTS and https://github.com/yoshizoe/mp-chemts, respectively. 
+The original implementations are available at https://github.com/tsudalab/ChemTS and https://github.com/yoshizoe/mp-chemts, respectively.
 
 ChemTSv2 provides:
 
 - easy-to-run interface by using only a configuration file
 - easy-to-define framework for users' any reward function, molecular filter, and tree policy
 - various usage examples in the GitHub repository
 
 [^13]: Ishida, S. and Aasawat, T. and Sumita, M. and Katouda, M. and Yoshizawa, T. and Yoshizoe, K. and Tsuda, K. and Terayama, K. (2023). ChemTSv2: Functional molecular design using de novo molecule generator. <i>WIREs Computational Molecular Science</i> https://wires.onlinelibrary.wiley.com/doi/10.1002/wcms.1680
 
 [^1]: Yang, X., Zhang, J., Yoshizoe, K., Terayama, K., & Tsuda, K. (2017). ChemTS: an efficient python library for de novo molecular generation. <i>Science and Technology of Advanced Materials</i>, 18(1), 972–976. https://doi.org/10.1080/14686996.2017.1401424
 
 [^2]: Yang, X., Aasawat, T., & Yoshizoe, K. (2021). Practical Massively Parallel Monte-Carlo Tree Search Applied to Molecular Design. <i>In International Conference on Learning Representations</i>. https://openreview.net/forum?id=6k7VdojAIK
 
-
 ## How to setup :pushpin:
 
 ### Requirements :memo:
+
+>[!NOTE]
+>ARM architecture, e.g., Apple Silicon, is not currently supported
+
 <details>
   <summary>Click to show/hide requirements</summary>
 
 1. python: 3.11
 2. rdkit: 2023.9.1
 3. tensorflow: 2.14.1
 4. pyyaml
 5. pandas: 2.1.3
 6. joblib
 7. mpi4py: 3.1.5 (for massive parallel mode)
+
 </details>
 
 ### ChemTSv2 with single process mode :red_car:
+
 <details>
   <summary>Click to show/hide the instruction</summary>
 
 ```bash
 cd YOUR_WORKSPACE
 python3.11 -m venv .venv
 source .venv/bin/activate
 pip install --upgrade chemtsv2
 ```
+
 </details>
 
 ### ChemTSv2 with massive parallel mode :airplane:
 
 <details>
   <summary>Click to show/hide the instruction</summary>
 NOTE: You need to run ChemTSv2-MP on a server where OpenMPI or MPICH is installed.
@@ -96,28 +102,31 @@
 
 ```bash
 conda create -n mpchem python=3.11 -c conda-forge
 # swith to the `mpchem` environment
 conda install -c conda-forge openmpi cxx-compiler mpi mpi4py=3.1.5
 pip install --upgrade chemtsv2
 ```
+
 </details>
 
 ## How to run ChemTSv2 :pushpin:
 
 ### 1. Clone this repository and move into it
 
 ```bash
 git clone git@github.com:molecule-generator-collection/ChemTSv2.git
 cd ChemTSv2
 ```
 
 ### 2. Prepare a reward file
+
 Please refer to `reward/README.md`.
 An example of reward definition for LogP maximization task is as follows.
+
 ```python
 from rdkit.Chem import Descriptors
 import numpy as np
 from chemtsv2.reward import Reward
 
 class LogP_reward(Reward):
     def get_objective_functions(conf):
@@ -128,17 +137,17 @@
     def calc_reward_from_objective_values(objective_values, conf):
         logp = objective_values[0]
         return np.tanh(logp/10)
 ```
 
 ### 3. Prepare a config file
 
-The explanation of options are described in the [Support option/function](#support-optionfunction-pushpin) section. 
+The explanation of options are described in the [Support option/function](#support-optionfunction-pushpin) section.
 The prepared reward file needs to be specified in `reward_setting`.
-For details, please refer to a sample file ([config/setting.yaml](config/setting.yaml)). 
+For details, please refer to a sample file ([config/setting.yaml](config/setting.yaml)).
 If you want to pass any value to `calc_reward_from_objective_values` (e.g., weights for each value), add it in the config file.
 
 ### 4. Generate molecules
 
 #### ChemTSv2 with single process mode :red_car:
 
 ```bash
@@ -170,14 +179,15 @@
 |Jscore|[Jscore_reward.py](reward/Jscore_reward.py)|[setting_jscore.yaml](config/setting_jscore.yaml)|-|[^1]|
 |Absorption wavelength|[chro_reward.py](reward/chro_reward.py)|[setting_chro.yaml](config/setting_chro.yaml)|Gaussian 16[^3]<br> via QCforever[^10]|[^4]|
 |Absorption wavelength|[chro_gamess_reward.py](reward/chro_gamess_reward.py)|[setting_chro_gamess.yaml](config/setting_chro_gamess.yaml)|GAMESS 2022.2[^12] via QCforever[^10]||
 |Upper-absorption & fluorescence<br> wavelength|[fluor_reward.py](reward/fluor_reward.py)|[setting_fluor.yaml](config/setting_fluor.yaml)|Gaussian 16[^3]<br> via QCforever[^10]|[^5]|
 |Kinase inhibitory activities|[dscore_reward.py](reward/dscore_reward.py)|[setting_dscore.yaml](config/setting_dscore.yaml)|LightGBM[^6]|[^7]|
 |Docking score|[Vina_binary_reward.py](reward/Vina_binary_reward.py)|[setting_vina_binary.yaml](config/setting_vina_binary.yaml)|AutoDock Vina[^8]|[^9]|
 |Pharmacophore|[pharmacophore_reward.py](reward/pharmacophore_reward.py)|[setting_pharmacophore.yaml](config/setting_pharmacophore.yaml)|-|[^11]|
+|gnina docking|[gnina_singularity_reward.py](reward/gnina_singularity_reward.py)|[setting_gnina_singularity.yaml](config/setting_gnina_singularity.yaml)|-||
 
 [^3]: Frisch, M. J. et al. Gaussian 16 Revision C.01. 2016; Gaussian Inc. Wallingford CT.
 [^4]: Sumita, M., Yang, X., Ishihara, S., Tamura, R., & Tsuda, K. (2018). Hunting for Organic Molecules with Artificial Intelligence: Molecules Optimized for Desired Excitation Energies. <i>ACS Central Science</i>, 4(9), 1126–1133. https://doi.org/10.1021/acscentsci.8b00213
 [^5]: Sumita, M., Terayama, K., Suzuki, N., Ishihara, S., Tamura, R., Chahal, M. K., Payne, D. T., Yoshizoe, K., & Tsuda, K. (2022). De novo creation of a naked eye–detectable fluorescent molecule based on quantum chemical computation and machine learning. <i>Science Advances</i>, 8(10). https://doi.org/10.1126/sciadv.abj3906
 [^6]: Ke, G., Meng, Q., Finley, T., Wang, T., Chen, W., Ma, W., … Liu, T.-Y. (2017). Lightgbm: A highly efficient gradient boosting decision tree. <i>Advances in Neural Information Processing Systems</i>, 30, 3146–3154.
 [^7]: Yoshizawa, T., Ishida, S., Sato, T., Ohta, M., Honma, T., & Terayama, K. (2022). Selective Inhibitor Design for Kinase Homologs Using Multiobjective Monte Carlo Tree Search. <i>Journal of Chemical Information and Modeling</i>, 62(22), 5351–5360. https://doi.org/10.1021/acs.jcim.2c00787
 [^8]: Eberhardt, J., Santos-Martins, D., Tillack, A. F., & Forli, S. (2021). AutoDock Vina 1.2.0: New Docking Methods, Expanded Force Field, and Python Bindings. <i>Journal of Chemical Information and Modeling</i>, 61(8), 3891–3898. https://doi.org/10.1021/acs.jcim.1c00203
@@ -194,15 +204,15 @@
 |`threshold_type`|:white_check_mark:|:heavy_check_mark:|Threshold type to select how long (`hours`) or how many (`generation_num`) molecule generation to perform. Massive parallel mode currently supports only the how long (`hours`) option.|
 |`hours`|:white_check_mark:|:white_check_mark:|Time for molecule generation in hours|
 |`generation_num`|:white_check_mark:|:white_large_square:|Number of molecules to be generated. Please note that the specified number is usually exceeded.|
 |`expansion_threshold`|:white_check_mark:|:white_large_square:|(Advanced) Expansion threshold of the cumulative probability. The default is set to 0.995.|
 |`simulation_num`|:white_check_mark:|:white_large_square:|(Advanced) Number of rollout runs in one cycle of MCTS. The default is set to 3.|
 |`flush_threshold`|:white_check_mark:|:white_large_square:|Threshold for saving the progress of a molecule generation. If the number of generated molecules exceeds the threshold value, the result is saved. The default is set to -1, and this represents no progress is to be saved.|
 |Molecule filter|:white_check_mark:|:white_check_mark:|Molecule filter to skip reward calculation of unfavorable generated molecules. Please refer to filter/README.md for details.|
-|RNN model replacement|:white_check_mark:|:white_check_mark:|Users can switch RNN models used in expansion and rollout steps of ChemTSv2. The model needs to be trained using Tensorflow. `model_json` specifies the JSON file that contains the architecture of the RNN model, and `model_weight` specifies the file in H5 format that contains a set of the values of the weights.|
+|RNN model replacement|:white_check_mark:|:white_check_mark:|Users can switch RNN models used in expansion and rollout steps of ChemTSv2. The model needs to be trained using Tensorflow. `model_json` specifies the JSON file that contains the architecture of the RNN model, and `model_weight` specifies the file in H5 format that contains a set of the values of the weights. `token` specifies the pickle file that contains the token list used when training an RNN model.|
 |Reward replacement|:white_check_mark:|:white_check_mark:|Users can use any reward function as long as they follow the reward base class ([reward/reward.py](reward/reward.py)). Please refer to reward/README.md for details.|
 |Policy replacement|:white_check_mark:|:white_large_square:|(Advanced) Users can use any policy function as long as they follow the policy base class ([policy/policy.py](policy/policy.py)). Please refer to policy/README.md for details.|
 |Restart|:beginner:|:beginner:|Users can save the checkpoint file and restart from the file. If users want to save a checkpoint file, <b>(SP mode)</b> set `save_checkpoint` to True and specify the file name in `checkpoint_file`. If users want to restart from the checkpoint, set `restart` to True and specify the checkpoint file in `checkpoint_file`. <b>(MP mode)</b> under development.|
 
 - :white_check_mark: indicates that the option/function is supported.
 - :heavy_check_mark: indicates that the option/function is partially supported.
 - :beginner: indicates that the option/function is beta version.
@@ -232,21 +242,20 @@
 # In this example, `Br` appears fifth, so we specify `5` as a <atom no.>.
 obabel -:"NC1=CC(Br)=CC=C1" -osmi -xl 5
 # output: Nc1cc(ccc1)Br
 ```
 
 Please refer to the [official documentation](https://openbabel.org/docs/current/FileFormats/SMILES_format.html) for detailed usage.
 
-
 ### Train RNN models using your own dataset
 
-If you want to use the RNN models trained on your own datasets, use [train_model/train_RNN.py](train_model/train_RNN.py) and [train_model/model_setting.yaml](train_model/model_setting.yaml) to train the models. 
+If you want to use the RNN models trained on your own datasets, use [train_model/train_RNN.py](train_model/train_RNN.py) and [train_model/model_setting.yaml](train_model/model_setting.yaml) to train the models.
 You need to prepare a dataset that only contains SMILES string and modify the path in `dataset` key in `model_setting.yaml`. And then, run the following command:
 
-```
+```bash
 cd train_model/
 python train_RNN.py -c model_setting.yaml
 ```
 
 Please note that the current version of ChemTSv2 does not support the change for RNN model structures, and users can only change the parameters described in `model_setting.yaml`.
 
 Once you train the RNN model, specify the path to the checkpoint and token files in `model_setting` and `token` keys in ChemTSv2 config files to run ChemTSv2 with your own RNN model.
@@ -257,15 +266,15 @@
 
 ```bash
 chemtsv2 -c config/setting.yaml --gpu 0
 ```
 
 ## How to cite
 
-```
+```text
 @article{Ishida2023,
   doi = {10.1002/wcms.1680},
   url = {https://doi.org/10.1002/wcms.1680},
   year = {2023},
   month = jul,
   publisher = {Wiley},
   author = {Shoichi Ishida and Tanuj Aasawat and Masato Sumita and Michio Katouda and Tatsuya Yoshizawa and Kazuki Yoshizoe and Koji Tsuda and Kei Terayama},
```

