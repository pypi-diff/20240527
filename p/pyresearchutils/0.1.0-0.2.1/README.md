# Comparing `tmp/pyresearchutils-0.1.0.tar.gz` & `tmp/pyresearchutils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresearchutils-0.1.0.tar", last modified: Wed Jun  1 12:50:23 2022, max compression
+gzip compressed data, was "pyresearchutils-0.2.1.tar", last modified: Mon May 27 06:36:52 2024, max compression
```

## Comparing `pyresearchutils-0.1.0.tar` & `pyresearchutils-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/pyresearchutils/
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3197 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/config_reader.py
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1157 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/initlized_log.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/log_folder.py
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     2388 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/metric_averaging.py
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/pyresearchutils/signal_processing/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/signal_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/signal_processing/metric.py
--rw-r--r--   0 runner    (1001) docker     (121)      482 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/signal_processing/spectrum.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/timing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/pyresearchutils/torch/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/torch/numpy_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      304 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/torch/tensor_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/pyresearchutils/torch/working_device.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:50:23.911051 pyresearchutils-0.1.0/pyresearchutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-06-01 12:50:23.000000 pyresearchutils-0.1.0/pyresearchutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-06-01 12:50:23.000000 pyresearchutils-0.1.0/pyresearchutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:50:23.000000 pyresearchutils-0.1.0/pyresearchutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-01 12:50:23.000000 pyresearchutils-0.1.0/pyresearchutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-01 12:50:23.000000 pyresearchutils-0.1.0/pyresearchutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-01 12:50:23.915051 pyresearchutils-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-06-01 12:49:40.000000 pyresearchutils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:36:52.406684 pyresearchutils-0.2.1/pyresearchutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/config_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/initlized_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/log_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5905 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/metric_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/metric_lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/pyresearchutils/signal_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/signal_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/signal_processing/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/signal_processing/spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/timing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/pyresearchutils/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/torch/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/torch/numpy_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/torch/tensor_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/torch/working_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/pyresearchutils/wandb_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/pyresearchutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-27 06:36:52.000000 pyresearchutils-0.2.1/pyresearchutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-27 06:36:52.000000 pyresearchutils-0.2.1/pyresearchutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:36:52.000000 pyresearchutils-0.2.1/pyresearchutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 06:36:52.000000 pyresearchutils-0.2.1/pyresearchutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-27 06:36:52.000000 pyresearchutils-0.2.1/pyresearchutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-27 06:36:52.410684 pyresearchutils-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-27 06:36:36.000000 pyresearchutils-0.2.1/setup.py
```

### Comparing `pyresearchutils-0.1.0/LICENSE` & `pyresearchutils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyresearchutils-0.1.0/pyresearchutils/config_reader.py` & `pyresearchutils-0.2.1/pyresearchutils/config_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 import json
 
 import copy
 
 from pyresearchutils import constants
 
 
+def _handle_boolean(input_dict):
+    for name, c in input_dict.items():
+        if isinstance(c, str):
+            if c.lower() == "true":
+                input_dict[name] = True
+            if c.lower() == "false":
+                input_dict[name] = False
+
+
 class ConfigReader(object):
     def __init__(self):
         self.arg_dict = dict()
         self.enum_dict = dict()
         self.parameters = None
 
     def add_parameter(self, name, **kwargs):
         if name == constants.CONFIG:
             raise Exception(f"Cant user the argument named:{constants.CONFIG}")
         if kwargs.get('enum'):
             self.enum_dict[name] = kwargs.get('enum')
             kwargs.pop('enum')
         self.arg_dict.update({name: kwargs})
 
+    def notebook_parameters(self, **kwargs):
+        self.get_user_arguments()
+        return self.parameters
+
     def _handle_enums(self, input_dict):
         for name, c in self.enum_dict.items():
             input_dict[name] = c[input_dict[name]]
         return input_dict
 
-    def _handle_boolean(self, input_dict):
-        # output_dict = copy.copy(input_dict)
-        for name, c in input_dict.items():
-            if isinstance(c, str):
-                if c.lower() == "true":
-                    input_dict[name] = True
-                if c.lower() == "false":
-                    input_dict[name] = False
-        # return output_dict
-
     def _handle_enums2str(self, input_dict):
         for name, c in self.enum_dict.items():
             input_dict[name] = input_dict[name].name
         return input_dict
 
     def get_user_arguments(self):
         if self.parameters is None:
@@ -51,15 +54,15 @@
             parameters, _ = argparser.parse_known_args()
             parameters_dict = vars(parameters)
             for pname, pvalue in self.arg_dict.items():
                 if parameters.__getattribute__(pname) == pvalue["default"] and lcfg.get(
                         pname) is not None:  # Same as defulat
                     parameters_dict[pname] = lcfg.get(pname)
             parameters_dict = self._handle_enums(parameters_dict)
-            self._handle_boolean(parameters_dict)
+            _handle_boolean(parameters_dict)
             self.parameters = Namespace(**parameters_dict)
         return self.parameters
 
     def save_config(self, folder):
         args = self.get_user_arguments()
         args = copy.deepcopy(args)
         args_dict = vars(args)
@@ -74,13 +77,26 @@
         config_file = config_args.__getattribute__(constants.CONFIG)
         if config_args.__getattribute__(constants.CONFIG) is None:
             return {}
         with open(config_file, 'r') as outfile:
             cfg = json.load(outfile)
         return cfg
 
+    def decode_run_parameters(self, in_dict):
+        new_dict = {}
+        for k, v in self.arg_dict.items():
+            if isinstance(v, dict):
+                v = v["default"]
+            if in_dict.get(k) is None:
+                new_dict.update({k: v})
+            else:
+                new_dict.update({k: in_dict.get(k)})
+            if self.enum_dict.get(k) is not None:
+                new_dict[k] = new_dict[k].split(".")[-1]
+        return Namespace(**self._handle_enums(new_dict))
+
 
 def initialized_config_reader(default_base_log_folder=None):
     cr = ConfigReader()
     cr.add_parameter(constants.BASELOGFOLDER, default=default_base_log_folder, type=str)
     cr.add_parameter(constants.SEED, default=0, type=int)
     return cr
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils/initlized_log.py` & `pyresearchutils-0.2.1/pyresearchutils/initlized_log.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,47 @@
 import os
-import wandb
+
 from pyresearchutils import logger
 from pyresearchutils.seed import set_seed
 from pyresearchutils.log_folder import generate_log_folder
 from pyresearchutils.config_reader import ConfigReader
 from pyresearchutils import constants
 
+if constants.FOUND_WANDB:
+    import wandb
+else:
+    wandb = None
+
 
 def initialized_log(project_name: str, config_reader: ConfigReader = None,
                     enable_wandb: bool = False):
-    args = config_reader.get_user_arguments()
+    """
+
+    Args:
+        project_name:
+        config_reader:
+        enable_wandb:
 
-    os.makedirs(args.base_log_folder, exist_ok=True)
-    run_log_dir = generate_log_folder(args.base_log_folder)
+    Returns:
 
-    logger.set_log_folder(run_log_dir)
-    set_seed(args.seed)
+    """
+    run_log_dir = None
+    args = None
     if config_reader is not None:
+        args = config_reader.get_user_arguments()
+
+        os.makedirs(args.base_log_folder, exist_ok=True)
+        run_log_dir = generate_log_folder(args.base_log_folder)
+
+        logger.set_log_folder(run_log_dir)
+        set_seed(args.seed)
         config_reader.save_config(run_log_dir)
-    logger.info(f"Log Folder Set to {run_log_dir}")
-    if enable_wandb:
-        wandb.init(project=project_name, dir=args.base_log_folder)  # Set WandB Folder to log folder
-        wandb.config.update(config_reader.get_user_arguments())  # adds all of the arguments as config variables®
+        logger.info(f"Log Folder Set to {run_log_dir}")
+    if constants.FOUND_WANDB and enable_wandb:
+        wandb.init(project=project_name,
+                   dir=args.base_log_folder if config_reader is not None else None)  # Set WandB Folder to log folder
+        if config_reader is not None:
+            wandb.config.update(config_reader.get_user_arguments())  # adds all of the arguments as config variables®
     if constants.FOUND_PYTORCH:
         from pyresearchutils.torch.working_device import get_working_device
         constants.DEVICE = get_working_device()
     return args, run_log_dir
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils/logger.py` & `pyresearchutils-0.2.1/pyresearchutils/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         'info': logging.INFO,
         'warning': logging.WARNING,
         'error': logging.ERROR,
         'critical': logging.CRITICAL
     }
     LOG_PATH = None
     LOG_FILE = None
+    LOG_WARNING = None
     CONSOLE = None
 
     @staticmethod
     def __check_path_create_dir(log_path: str):
         """
         Create a path if not exist. Otherwise, do nothing.
         Args:
@@ -86,74 +87,90 @@
     def get_logger():
         """
         Returns: An instance of the logger.
         """
         return logging.getLogger(LOGGER_NAME)
 
     @staticmethod
+    def set_logger():
+        logger = Logger.get_logger()
+        FORMAT = "[%(asctime)s][$BOLD%(name)-20s$RESET][%(levelname)-18s]  %(message)s ($BOLD%(filename)s$RESET:%(lineno)d)"
+        COLOR_FORMAT = formatter_message(FORMAT, True)
+        formatter = ColoredFormatter(COLOR_FORMAT)
+
+        ch = logging.StreamHandler()
+        ch.setLevel(logging.INFO)
+        ch.setFormatter(formatter)
+        logger.addHandler(ch)
+        Logger.CONSOLE = ch
+
+    @staticmethod
     def set_log_file(log_folder: str = None):
         """
         Setting the logger log file path. The method gets the folder for the log file.
         In that folder, it creates a log file according to the timestamp.
         Args:
             log_folder: Folder path to hold the log file.
 
         """
 
         logger = Logger.get_logger()
-
-        ts = datetime.now(tz=None).strftime("%d%m%Y_%H%M%S")
-
-        FORMAT = "[%(asctime)s][$BOLD%(name)-20s$RESET][%(levelname)-18s]  %(message)s ($BOLD%(filename)s$RESET:%(lineno)d)"
-        COLOR_FORMAT = formatter_message(FORMAT, True)
-        formatter = ColoredFormatter(COLOR_FORMAT)
-
         text_formatter = logging.Formatter(
             '[%(asctime)s][%(name)-20s][%(levelname)-18s]  %(message)s (%(filename)s:%(lineno)d)')
+        ts = datetime.now(tz=None).strftime("%d%m%Y_%H%M%S")
 
         Logger.LOG_PATH = os.path.join(log_folder)
         log_name = os.path.join(Logger.LOG_PATH, f'research_logs_{ts}.log')
 
         Logger.__check_path_create_dir(Logger.LOG_PATH)
 
         fh = logging.FileHandler(log_name)
         fh.setLevel(logging.NOTSET)
         fh.setFormatter(text_formatter)
         logger.addHandler(fh)
 
-        ch = logging.StreamHandler()
-        ch.setLevel(logging.INFO)
-        ch.setFormatter(formatter)
-        logger.addHandler(ch)
         Logger.LOG_FILE = log_name
-        Logger.CONSOLE = ch
 
 
 def set_log_folder(folder: str, level: int = logging.INFO):
     """
     Set a directory path for saving a log file.
 
     Args:
         folder: Folder path to save the log file.
         level: Level of verbosity to set to the logger.
 
     """
+    Logger.set_logger()
     Logger.set_log_file(folder)
     Logger.set_logger_level(level)
 
 
 def get_log_file():
     return Logger.LOG_FILE
 
 
+def get_log_warning_status():
+    return Logger.LOG_WARNING
+
+
+def disable_folder_warning():
+    """
+    Set a directory path for saving a log file.
+
+
+    """
+    Logger.set_logger()
+    Logger.LOG_WARNING = False
+
+
 def check_logger_path():
-    if get_log_file() is None:
-        logger_path = os.getcwd()
-        set_log_folder(logger_path)
-        warning(f"Logger is set automatically to {logger_path}")
+    if get_log_warning_status() is None:
+        disable_folder_warning()
+        warning(f"Logger folder is not set")
 
 
 ########################################
 # Delegating methods to wrapped logger
 ########################################
 def critical(msg: str):
     """
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils/metric_averaging.py` & `pyresearchutils-0.2.1/pyresearchutils/metric_averaging.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,39 @@
 import numpy as np
 
 
 class IsBest(object):
     def __init__(self):
         self.min_value = np.inf
         self.max_value = -np.inf
+        self.is_last_best = False
 
     def update_value(self, value: float):
+        """
+        Update the last best, min value and max value using the current value.
+        Args:
+            value: A floating point value.
+
+        Returns: None
+
+        """
+        self.is_last_best = self.is_best(value) # Update last best
         self.min_value = np.minimum(value, self.min_value)
         self.max_value = np.maximum(value, self.max_value)
 
     def is_best(self, value) -> bool:
-        # TODO: add maximal best
-        return value <= self.max_value
+        """
+        This function check a given value is best.
+        Args:
+            value: A floating point value.
+
+        Returns: a boolean stating it this is the best results so far.
+
+        """
+        return value <= self.min_value
 
 
 class SingleMetricAveraging(object):
     def __init__(self):
         self.n: int = 0
         self.accumulator: float = 0
 
@@ -74,9 +91,8 @@
             if self.best_dict.get(k) is None:
                 self.best_dict[k] = IsBest()
             self.best_dict[k].update_value(v)
 
     def is_best(self, name) -> bool:
         if len(self.best_dict) == 0:
             return True
-        v = self.result[name]
-        return self.best_dict[name].is_best(v)
+        return self.best_dict[name].is_last_best
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils/torch/numpy_dataset.py` & `pyresearchutils-0.2.1/pyresearchutils/torch/numpy_dataset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import numpy as np
 from torch.utils.data.dataset import Dataset
 
 
 class NumpyDataset(Dataset):
-    def __init__(self, data, label, transform):
+    def __init__(self, data, label, transform, metadata=None, extend=None):
         self.data = data
         self.label = label
+        self.metadata = metadata
         self.transform = transform
         self.n = len(data)
+        self.extend = extend
 
     def set_transform(self, transform):
         self.transform = transform
 
     def __getitem__(self, index):
+        index = index % self.n
         d = self.data[index]
         if self.transform is not None:
             d = self.transform(d)
         l = self.label[index]
-        return d, l
+        if self.metadata is None:
+            return d, l
+        else:
+            return d, l, self.metadata[index]
 
     def __len__(self):
-        return self.n
+        return self.n if self.extend is None else self.extend
 
     def get_min_max_vector(self):
         x = np.stack(self.data)
         return np.min(x, axis=0).astype("float32"), (np.max(x, axis=0) - np.min(x, axis=0)).astype("float32")
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils/torch/working_device.py` & `pyresearchutils-0.2.1/pyresearchutils/torch/working_device.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 import torch
 from pyresearchutils.logger import info
 from pyresearchutils import constants
 
 
 def get_working_device():
     if constants.DEVICE is None:
@@ -9,9 +11,9 @@
         info("Current Working Device is set to:" + str(working_device))
         constants.DEVICE = working_device
         return working_device
     else:
         return constants.DEVICE
 
 
-def update_device(x: torch.Tensor) -> torch.Tensor:
-    return x.to(get_working_device())
+def update_device(*args) -> List:
+    return [a.to(get_working_device()) for a in args]
```

### Comparing `pyresearchutils-0.1.0/pyresearchutils.egg-info/SOURCES.txt` & `pyresearchutils-0.2.1/pyresearchutils.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 pyresearchutils/__init__.py
 pyresearchutils/config_reader.py
 pyresearchutils/constants.py
 pyresearchutils/initlized_log.py
 pyresearchutils/log_folder.py
 pyresearchutils/logger.py
 pyresearchutils/metric_averaging.py
+pyresearchutils/metric_collector.py
+pyresearchutils/metric_lister.py
 pyresearchutils/seed.py
 pyresearchutils/timing.py
+pyresearchutils/wandb_helpers.py
 pyresearchutils.egg-info/PKG-INFO
 pyresearchutils.egg-info/SOURCES.txt
 pyresearchutils.egg-info/dependency_links.txt
 pyresearchutils.egg-info/requires.txt
 pyresearchutils.egg-info/top_level.txt
 pyresearchutils/signal_processing/__init__.py
 pyresearchutils/signal_processing/metric.py
 pyresearchutils/signal_processing/spectrum.py
 pyresearchutils/torch/__init__.py
+pyresearchutils/torch/ema.py
 pyresearchutils/torch/numpy_dataset.py
 pyresearchutils/torch/tensor_helpers.py
 pyresearchutils/torch/working_device.py
```

### Comparing `pyresearchutils-0.1.0/setup.py` & `pyresearchutils-0.2.1/setup.py`

 * *Files identical despite different names*

