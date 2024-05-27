# Comparing `tmp/mlcvzoo_mmdetection-6.5.1.tar.gz` & `tmp/mlcvzoo_mmdetection-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmdetection-6.5.1.tar", max compression
+gzip compressed data, was "mlcvzoo_mmdetection-6.6.0.tar", max compression
```

## Comparing `mlcvzoo_mmdetection-6.5.1.tar` & `mlcvzoo_mmdetection-6.6.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    11412 2024-02-06 13:44:45.410090 mlcvzoo_mmdetection-6.5.1/LICENSE
--rw-r--r--   0        0        0     1434 2024-02-19 10:17:25.192082 mlcvzoo_mmdetection-6.5.1/README.md
--rw-r--r--   0        0        0      244 2024-02-19 10:17:25.192082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/__init__.py
--rw-r--r--   0        0        0     9290 2024-02-19 10:17:25.192082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/configuration.py
--rw-r--r--   0        0        0        0 2024-02-19 10:17:44.016734 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/__init__.py
--rw-r--r--   0        0        0     4214 2024-02-19 10:17:25.192082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/converter.py
--rw-r--r--   0        0        0     2104 2024-02-13 15:48:56.179579 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/inferencer.py
--rw-r--r--   0        0        0     9243 2024-02-06 13:44:45.410090 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
--rw-r--r--   0        0        0    22270 2024-02-19 10:17:25.192082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/model.py
--rw-r--r--   0        0        0    10890 2024-02-19 10:17:25.196082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/object_detection_model.py
--rw-r--r--   0        0        0      196 2024-02-06 13:44:45.410090 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/py.typed
--rw-r--r--   0        0        0    14343 2024-02-19 10:17:25.196082 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/segmentation_model.py
--rw-r--r--   0        0        0     4561 2024-02-06 13:44:45.414090 mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/utils.py
--rw-r--r--   0        0        0     5023 2024-02-19 10:17:25.200082 mlcvzoo_mmdetection-6.5.1/pyproject.toml
--rw-r--r--   0        0        0     3688 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2024-05-27 09:57:50.612666 mlcvzoo_mmdetection-6.6.0/LICENSE
+-rw-r--r--   0        0        0     1434 2024-05-27 09:57:50.612666 mlcvzoo_mmdetection-6.6.0/README.md
+-rw-r--r--   0        0        0      244 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/__init__.py
+-rw-r--r--   0        0        0    10169 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/configuration.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:27:01.135779 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/__init__.py
+-rw-r--r--   0        0        0     5513 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/converter.py
+-rw-r--r--   0        0        0     2137 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/inferencer.py
+-rw-r--r--   0        0        0      421 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/structs.py
+-rw-r--r--   0        0        0     9243 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
+-rw-r--r--   0        0        0    23206 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/model.py
+-rw-r--r--   0        0        0    11020 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/object_detection_model.py
+-rw-r--r--   0        0        0      196 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/py.typed
+-rw-r--r--   0        0        0    14473 2024-05-27 09:57:50.616666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/segmentation_model.py
+-rw-r--r--   0        0        0     4561 2024-05-27 09:57:50.620666 mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/utils.py
+-rw-r--r--   0        0        0     5158 2024-05-27 09:57:50.620666 mlcvzoo_mmdetection-6.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.6.0/PKG-INFO
```

### Comparing `mlcvzoo_mmdetection-6.5.1/LICENSE` & `mlcvzoo_mmdetection-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.5.1/README.md` & `mlcvzoo_mmdetection-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/configuration.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -237,14 +237,36 @@
 
     @property
     def checkpoint_paths(self) -> List[str]:
         return [self.checkpoint_path]
 
 
 @define
+class MMDetectionMMDeployTensorRTConfig(MMDetectionMMDeployConfig):
+    """Definition of attributes needed to deploy a model using MMDeploy with TensorRT."""
+
+    __related_strict__ = True
+
+    checkpoint_path: str = related.StringField()
+    config_path: Optional[str] = related.ChildField(
+        cls=str, default=None, required=False
+    )
+    config_dict: Optional[Dict[str, Any]] = related.ChildField(
+        cls=dict, default=None, required=False
+    )
+    cfg_options: Optional[Dict[str, Any]] = related.ChildField(
+        cls=dict, default=None, required=False
+    )
+
+    @property
+    def checkpoint_paths(self) -> List[str]:
+        return [self.checkpoint_path]
+
+
+@define
 class MMDetectionConfig(ModelConfiguration):
     """Definition of attributes for a MMDetectionModel."""
 
     __related_strict__ = True
 
     class_mapping: ClassMappingConfig = related.ChildField(cls=ClassMappingConfig)
 
@@ -264,10 +286,16 @@
 
     mmdeploy_onnxruntime_float16_config: Optional[
         MMDetectionMMDeployOnnxruntimeConfig
     ] = related.ChildField(
         cls=MMDetectionMMDeployOnnxruntimeConfig, default=None, required=False
     )
 
+    mmdeploy_tensorrt_config: Optional[
+        MMDetectionMMDeployTensorRTConfig
+    ] = related.ChildField(
+        cls=MMDetectionMMDeployTensorRTConfig, default=None, required=False
+    )
+
     mm_config: MMConfig = related.ChildField(
         cls=MMConfig, default=Factory(MMConfig), required=False
     )
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/converter.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/converter.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 # SPDX-License-Identifier: OLFL-1.3
 
 """Wrapper to convert MMDetection models using MMDeploy."""
 
 import copy
 import os
 import shutil
-from typing import cast
+from typing import List, cast
 
 from mmdeploy.apis import torch2onnx
 from mmdeploy.apis.utils import to_backend
 from mmdeploy.backend.sdk.export_info import export2SDK
 from mmdeploy.utils import get_backend, get_ir_config
 from mmengine.config import Config
 
 from mlcvzoo_mmdetection.configuration import (
     MMDetectionMMDeployConfig,
     MMDetectionMMDeployOnnxruntimeConfig,
 )
+from mlcvzoo_mmdetection.mlcvzoo_mmdeploy.structs import MMDeployBackendType
 from mlcvzoo_mmdetection.utils import init_mm_config
 
 
 class MMDeployConverter:  # pylint: disable=too-few-public-methods
     """Converter for MMDetection models using MMDeploy."""
 
     def __init__(
@@ -54,36 +55,74 @@
         try:
             backend_type = self.mmdeploy_cfg["backend_config"]["type"]
         except KeyError as exc:
             raise KeyError(
                 "Invalid MMDeploy configuration. Key 'backend_config.type' is not specified."
             ) from exc
 
-        if backend_type == "onnxruntime":
-            return self._deploy_onnx_runtime()
+        if backend_type == MMDeployBackendType.ONNXRUNTIME:
+            return self.__deploy_onnxruntime()
+
+        if backend_type == MMDeployBackendType.TENSORRT:
+            return self.__deploy_tensorrt()
 
         raise NotImplementedError(
             f"Invalid MMDeploy configuration. The backend type '{backend_type}' is not supported."
         )
 
-    def _deploy_onnx_runtime(self) -> None:
+    def __deploy_onnxruntime(self) -> None:
         """Run a deployment for backend type onnxruntime.
 
         Raises:
-            ValueError: If the value for 'device_string' in the MMDeploy configuration is set to
-                'cuda'.
+            ValueError: If the value for 'device_string' in the MMDeploy configuration is not
+                'cpu'.
+        """
+
+        # Narrow type
+        mmdeploy_config = cast(
+            MMDetectionMMDeployOnnxruntimeConfig, self.mmdeploy_config
+        )
+
+        if self.mmdeploy_config.device_string != "cpu":
+            raise ValueError("Backend onnxruntime is only supported on CPU.")
+
+        checkpoint_paths = self.__deploy_common()
+
+        # For the onnxruntime backend only one is file generated
+        # Move generated end2end.onnx to the correct location
+        shutil.move(src=checkpoint_paths[0], dst=mmdeploy_config.checkpoint_path)
+
+    def __deploy_tensorrt(self) -> None:
+        """Run a deployment for backend type tensorrt.
+
+        Raises:
+            ValueError: If the value for 'device_string' in the MMDeploy configuration does not
+                start with 'cuda'.
         """
 
         # Narrow type
         mmdeploy_config = cast(
             MMDetectionMMDeployOnnxruntimeConfig, self.mmdeploy_config
         )
 
-        if self.mmdeploy_config.device_string == "cuda":
-            raise ValueError("Backend onnxruntime is not supported on GPU.")
+        if not self.mmdeploy_config.device_string.startswith("cuda"):
+            raise ValueError("Backend tensorrt is only supported on GPU.")
+
+        checkpoint_paths = self.__deploy_common()
+
+        # For the tensorrt backend only one file is generated
+        # Move generated end2end.engine to the correct location
+        shutil.move(src=checkpoint_paths[0], dst=mmdeploy_config.checkpoint_path)
+
+    def __deploy_common(self) -> List[str]:
+        """Run common steps for a MMdeploy deployment.
+
+        Returns:
+            List[str]: A list of generated backend specific model filepaths.
+        """
 
         if self.mmdeploy_config.dump_info:
             export2SDK(
                 deploy_cfg=self.mmdeploy_cfg,
                 # Use a deep copy to prevent changes in the model config
                 model_cfg=copy.deepcopy(self.model_config),
                 work_dir=self.mmdeploy_config.work_dir,
@@ -101,22 +140,20 @@
             save_file=ir_save_file,
             deploy_cfg=self.mmdeploy_cfg,
             model_cfg=self.model_config,
             model_checkpoint=self.checkpoint_path,
             device=self.mmdeploy_config.device_string,
         )
 
-        # Convert to onnxruntime
+        # Convert to backend
         backend = get_backend(self.mmdeploy_cfg)
 
         # MMdeploy always returns a list of backend files
-        checkpoint_paths = to_backend(
+        checkpoint_paths: List[str] = to_backend(
             backend_name=backend,
             ir_files=[os.path.join(self.mmdeploy_config.work_dir, ir_save_file)],
             work_dir=self.mmdeploy_config.work_dir,
             deploy_cfg=self.mmdeploy_cfg,
             device=self.mmdeploy_config.device_string,
         )
 
-        # For the onnxruntime backend only one file generated
-        # Move generated end2end.onnx to the correct location
-        shutil.move(src=checkpoint_paths[0], dst=mmdeploy_config.checkpoint_path)
+        return checkpoint_paths
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/inferencer.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdeploy/inferencer.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 #
 # Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
 # SPDX-License-Identifier: OLFL-1.3
 
 """Wrapper to run converted MMDetection models."""
 
-from typing import List
+from typing import Any, List
 
 import torch
 from mmdeploy.apis.utils import build_task_processor
 from mmdeploy.utils import get_input_shape
 from mmdet.apis.det_inferencer import InputsType
-from mmdet.structures.det_data_sample import DetDataSample
 from mmengine.config import Config
 
 from mlcvzoo_mmdetection.configuration import MMDetectionMMDeployConfig
 from mlcvzoo_mmdetection.utils import init_mm_config
 
 
 class MMDeployInferencer:  # pylint: disable=too-few-public-methods
@@ -38,26 +37,28 @@
         self.mmdeploy_model = self.task_processor.build_backend_model(
             model_files=mmdeploy_config.checkpoint_paths,
             data_preprocessor_updater=self.task_processor.update_data_preprocessor,
         )
 
         self._input_shape = get_input_shape(deploy_cfg=mmdeploy_cfg)
 
-    def __call__(self, inputs: InputsType) -> List[DetDataSample]:
+    # The return type can be a list of different MMLab data types, on which we are not dependent in
+    # this repo.
+    def __call__(self, inputs: InputsType) -> List[Any]:
         """Run inference for given inputs.
 
         To be compatible with MMDetections DetInferencer, the __call__ method is used.
 
         Args:
             inputs (InputsType): The inputs to run an inference on.
 
         Returns:
-            List[DetDataSample]: List of predictions.
+            List[Any]: List of predictions.
         """
         model_inputs, _ = self.task_processor.create_input(
             imgs=inputs, input_shape=self._input_shape
         )
 
         with torch.no_grad():
-            result: List[DetDataSample] = self.mmdeploy_model.test_step(model_inputs)
+            result: List[Any] = self.mmdeploy_model.test_step(model_inputs)
 
         return result
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/model.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,24 @@
             and self.configuration.mmdeploy_onnxruntime_float16_config.config_path
         ) and string_replacement_map:
             self.configuration.mmdeploy_onnxruntime_float16_config.config_path = modify_config(
                 config_path=self.configuration.mmdeploy_onnxruntime_float16_config.config_path,
                 string_replacement_map=string_replacement_map,
             )
 
+        # config path to MMDeploy specific .py file for TensorRT is set
+        if (
+            self.configuration.mmdeploy_tensorrt_config
+            and self.configuration.mmdeploy_tensorrt_config.config_path
+        ) and string_replacement_map:
+            self.configuration.mmdeploy_tensorrt_config.config_path = modify_config(
+                config_path=self.configuration.mmdeploy_tensorrt_config.config_path,
+                string_replacement_map=string_replacement_map,
+            )
+
         self.cfg = init_mm_config(
             mm_config=self.configuration.mm_config,
         )
         self.__init_dataloader()
         self.__deploy(runtime=runtime, init_for_inference=init_for_inference)
 
         Model.__init__(
@@ -173,15 +183,15 @@
                 )
 
         if self.configuration.mm_config.cfg_options is None:
             self.configuration.mm_config.cfg_options = (
                 self.configuration.train_config.argparse_config.cfg_options
             )
 
-    def __get__mmdeploy_config(
+    def _get_mmdeploy_config(
         self, runtime: Optional[str] = None
     ) -> Optional[MMDetectionMMDeployConfig]:
         """Check for the existence and return MMDeploy configuration.
 
         If no runtime is given, the MMDeploy configuration is selected by the runtime attribute of
         the instance.
 
@@ -224,14 +234,22 @@
                 raise ValueError(
                     "The mmdeploy_onnxruntime_float16_config must be provided for runtime "
                     "'ONNXRUNTIME_FLOAT16'."
                 )
 
             return self.configuration.mmdeploy_onnxruntime_float16_config
 
+        if runtime == Runtime.TENSORRT:
+            if self.configuration.mmdeploy_tensorrt_config is None:
+                raise ValueError(
+                    "The mmdeploy_tensorrt_config must be provided for runtime 'TENSORRT'."
+                )
+
+            return self.configuration.mmdeploy_tensorrt_config
+
         raise ValueError(
             f"Getting MMDeploy config is not supported for runtime '{self.runtime}'."
         )
 
     def __init_dataloader(self) -> None:
         dataset_type = self._get_dataset_type()
         # Update the class-mapping configuration for a dataset of the dataloaders,
@@ -280,18 +298,22 @@
                 )
                 self.net = self.inferencer.model
 
                 if self.configuration.inference_config.checkpoint_path != "":
                     self.restore(
                         checkpoint_path=self.configuration.inference_config.checkpoint_path
                     )
-        elif self.runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
-            # Return value of __get__mmdeploy_config will not be None
+        elif self.runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
+            # Return value of _get_mmdeploy_config will not be None
             mmdeploy_config = cast(
-                MMDetectionMMDeployConfig, self.__get__mmdeploy_config()
+                MMDetectionMMDeployConfig, self._get_mmdeploy_config()
             )
 
             if MMDeployInferencer is None:
                 raise RuntimeError(
                     "Extra 'mmdeploy' must be installed to run a model which is deployed with "
                     "MMDeploy."
                 )
@@ -427,18 +449,22 @@
             return
 
         if not init_for_inference:
             raise ValueError(
                 f"Deploying for training is not supported for runtime '{runtime}'."
             )
 
-        if runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
-            # Return value of __get__mmdeploy_config will not be None
+        if runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
+            # Return value of _get_mmdeploy_config will not be None
             mmdeploy_config = cast(
-                MMDetectionMMDeployConfig, self.__get__mmdeploy_config(runtime=runtime)
+                MMDetectionMMDeployConfig, self._get_mmdeploy_config(runtime=runtime)
             )
         else:
             raise ValueError(f"Deployment is not supported for runtime '{runtime}'.")
 
         if not all(
             os.path.exists(checkpoint_path)
             for checkpoint_path in mmdeploy_config.checkpoint_paths
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/object_detection_model.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/object_detection_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,19 @@
 
             # For a single data_item we only have one prediction
             return data_item, self.__decode_mmdet_result(
                 prediction=cast(DetInferencer, self.inferencer)(
                     inputs=data_item, return_datasample=True, batch_size=1
                 )["predictions"][0]
             )
-        if self.runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
+        if self.runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
             if self.inferencer is None:
                 raise no_inferencer_error
 
             if MMDeployInferencer is None:
                 raise RuntimeError(
                     "Extra 'mmdeploy' must be installed to run a model which is deployed with "
                     "MMDeploy."
@@ -250,15 +254,19 @@
                 raise no_inferencer_error
 
             predictions: List[DetDataSample] = cast(DetInferencer, self.inferencer)(
                 inputs=data_items,
                 return_datasample=True,
                 batch_size=len(data_items),
             )["predictions"]
-        elif self.runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
+        elif self.runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
             if self.inferencer is None:
                 raise no_inferencer_error
 
             if MMDeployInferencer is None:
                 raise RuntimeError(
                     "Extra 'mmdeploy' must be installed to run a model which is deployed with "
                     "MMDeploy."
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/segmentation_model.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/segmentation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,19 @@
                 raise no_inferencer_error
 
             return data_item, self.__decode_mmdet_result(
                 prediction=cast(DetInferencer, self.inferencer)(
                     inputs=data_item, return_datasample=True, batch_size=1
                 )["predictions"][0]
             )
-        if self.runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
+        if self.runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
             if self.inferencer is None:
                 raise no_inferencer_error
 
             if MMDeployInferencer is None:
                 raise RuntimeError(
                     "Extra 'mmdeploy' must be installed to run a model which is deployed with "
                     "MMDeploy."
@@ -317,15 +321,19 @@
 
             # TODO: add batch-size as parameter
             predictions: List[DetDataSample] = cast(DetInferencer, self.inferencer)(
                 inputs=data_items,
                 return_datasample=True,
                 batch_size=len(data_items),
             )["predictions"]
-        elif self.runtime in (Runtime.ONNXRUNTIME, Runtime.ONNXRUNTIME_FLOAT16):
+        elif self.runtime in (
+            Runtime.ONNXRUNTIME,
+            Runtime.ONNXRUNTIME_FLOAT16,
+            Runtime.TENSORRT,
+        ):
             if self.inferencer is None:
                 raise no_inferencer_error
 
             if MMDeployInferencer is None:
                 raise RuntimeError(
                     "Extra 'mmdeploy' must be installed to run a model which is deployed with "
                     "MMDeploy."
```

### Comparing `mlcvzoo_mmdetection-6.5.1/mlcvzoo_mmdetection/utils.py` & `mlcvzoo_mmdetection-6.6.0/mlcvzoo_mmdetection/utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_mmdetection-6.5.1/pyproject.toml` & `mlcvzoo_mmdetection-6.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mlcvzoo-mmdetection"
 description = "MLCVZoo MMDetection Package"
-version = "6.5.1"
+version = "6.6.0"
 license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
@@ -50,14 +50,17 @@
 pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
 nptyping = { version = ">=2.0" }
 # torch 2.0.1 has missing cuda dependencies https://github.com/pytorch/pytorch/issues/100974
 torch = { version = ">=1.9,!=2.0.1" }
 torchvision = { version = ">=0.10" }
+# tensorrt>=8.6.0 has dependencies on cuda 12
+tensorrt = { version = "==8.5.3.1", optional=true }
+
 
 # TODO: Remove when issue is resolved, normally yapf is not a first-level depedency of mlcvzoo-mmdetection
 #       Issue: https://github.com/open-mmlab/mmdetection/issues/10962
 yapf = { version = "*,!=0.40.2" }
 
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
@@ -78,14 +81,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.extras]
 mmdeploy = ["mmdeploy"]
 mmsegmentation = ["mmsegmentation"]
 onnxruntime = ["mmdeploy", "onnxruntime"]
 onnxruntime-float16 = ["mmdeploy", "onnxruntime", "onnxconverter-common"]
+tensorrt = ["mmdeploy", "tensorrt"]
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.master]
 extension-pkg-whitelist = ["numpy", "cv2"]
 jobs = 0
```

### Comparing `mlcvzoo_mmdetection-6.5.1/PKG-INFO` & `mlcvzoo_mmdetection-6.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmdetection
-Version: 6.5.1
+Version: 6.6.0
 Summary: MLCVZoo MMDetection Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection
 License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,29 +16,31 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mmdeploy
 Provides-Extra: mmsegmentation
 Provides-Extra: onnxruntime
 Provides-Extra: onnxruntime-float16
+Provides-Extra: tensorrt
 Requires-Dist: attrs (>=20)
 Requires-Dist: mlcvzoo_base (>=5.7,<6.0)
 Requires-Dist: mmcv (>=2,<3)
-Requires-Dist: mmdeploy (>=1.3.0) ; extra == "mmdeploy" or extra == "onnxruntime" or extra == "onnxruntime-float16"
+Requires-Dist: mmdeploy (>=1.3.0) ; extra == "mmdeploy" or extra == "onnxruntime" or extra == "onnxruntime-float16" or extra == "tensorrt"
 Requires-Dist: mmdet (>=3,<4)
 Requires-Dist: mmengine (>=0.7,<0.8)
 Requires-Dist: mmsegmentation (>=1,<2) ; extra == "mmsegmentation"
 Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
 Requires-Dist: onnxconverter-common (>=1.14.0) ; extra == "onnxruntime-float16"
 Requires-Dist: onnxruntime (>=1.16.0) ; extra == "onnxruntime" or extra == "onnxruntime-float16"
 Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: opencv-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
 Requires-Dist: related-mltoolbox (>=1,<2)
+Requires-Dist: tensorrt (==8.5.3.1) ; extra == "tensorrt"
 Requires-Dist: torch (>=1.9,!=2.0.1)
 Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Requires-Dist: yapf (!=0.40.2)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo-models/mlcvzoo-mmdetection
 Description-Content-Type: text/markdown
```

