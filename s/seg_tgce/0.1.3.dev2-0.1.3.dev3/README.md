# Comparing `tmp/seg_tgce-0.1.3.dev2.tar.gz` & `tmp/seg_tgce-0.1.3.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seg_tgce-0.1.3.dev2.tar", max compression
+gzip compressed data, was "seg_tgce-0.1.3.dev3.tar", max compression
```

## Comparing `seg_tgce-0.1.3.dev2.tar` & `seg_tgce-0.1.3.dev3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      322 2024-05-14 04:12:07.157195 seg_tgce-0.1.3.dev2/README.md
--rw-r--r--   0        0        0     1589 2024-05-21 12:58:28.996565 seg_tgce-0.1.3.dev2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/data/__init__.py
--rw-r--r--   0        0        0     1238 2024-05-20 13:03:41.594701 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/__init__.py
--rw-r--r--   0        0        0      391 2024-05-21 11:02:17.869649 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/__main__.py
--rw-r--r--   0        0        0     5233 2024-05-21 11:02:17.869649 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/generator.py
--rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/map.py
--rw-r--r--   0        0        0     1001 2024-05-20 12:31:40.420402 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/retrieve.py
--rw-r--r--   0        0        0      166 2024-05-20 11:50:15.678622 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/stage.py
--rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/visualizer.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/__init__.py
--rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/disturbance/model.py
--rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
--rw-r--r--   0        0        0      876 2024-05-14 03:55:28.061819 seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/oxford_pet.py
--rw-r--r--   0        0        0     2228 2024-05-14 03:55:28.058486 seg_tgce-0.1.3.dev2/seg_tgce/data/utils.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/experiments/__init__.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/experiments/apr_14_2024/__init__.py
--rw-r--r--   0        0        0      856 2024-05-21 11:39:33.344315 seg_tgce-0.1.3.dev2/seg_tgce/experiments/apr_14_2024/experiment.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/loss/__init__.py
--rw-r--r--   0        0        0     3490 2024-05-21 12:52:46.131164 seg_tgce-0.1.3.dev2/seg_tgce/loss/tgce.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/metrics/__init__.py
--rw-r--r--   0        0        0     1530 2024-05-21 12:52:02.884656 seg_tgce-0.1.3.dev2/seg_tgce/metrics/dice_coefficient.py
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/models/__init__.py
--rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.1.3.dev2/seg_tgce/models/ma_model.py
--rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.1.3.dev2/seg_tgce/models/unet.py
--rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.1.3.dev2/seg_tgce/py.typed
--rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/run/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/__init__.py
--rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/model_result.py
--rw-r--r--   0        0        0     2473 2024-05-21 12:52:02.877989 seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/plotting.py
--rw-r--r--   0        0        0     7072 2024-05-21 12:42:11.676806 seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/runner.py
--rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev2/seg_tgce/run/runner.py
--rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 seg_tgce-0.1.3.dev2/PKG-INFO
+-rw-r--r--   0        0        0      322 2024-05-14 04:12:07.157195 seg_tgce-0.1.3.dev3/README.md
+-rw-r--r--   0        0        0     1589 2024-05-27 03:52:55.898534 seg_tgce-0.1.3.dev3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/data/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-27 02:17:53.917965 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/__init__.py
+-rw-r--r--   0        0        0      297 2024-05-27 03:42:20.787420 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/__main__.py
+-rw-r--r--   0        0        0     1001 2024-05-20 12:31:40.420402 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/__retrieve.py
+-rw-r--r--   0        0        0     6824 2024-05-27 03:52:04.165387 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/generator.py
+-rw-r--r--   0        0        0      475 2024-04-30 04:42:11.177868 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/map.py
+-rw-r--r--   0        0        0      166 2024-05-20 11:50:15.678622 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/stage.py
+-rw-r--r--   0        0        0     2231 2024-05-06 04:51:09.581252 seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/visualizer.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/__init__.py
+-rw-r--r--   0        0        0     2465 2024-05-06 05:34:13.661853 seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/disturbance/model.py
+-rw-r--r--   0        0        0     2711 2024-05-14 03:29:38.912294 seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/oxford_iiit_pet.py
+-rw-r--r--   0        0        0      876 2024-05-14 03:55:28.061819 seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/oxford_pet.py
+-rw-r--r--   0        0        0     2228 2024-05-14 03:55:28.058486 seg_tgce-0.1.3.dev3/seg_tgce/data/utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/experiments/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/experiments/apr_14_2024/__init__.py
+-rw-r--r--   0        0        0      856 2024-05-21 11:39:33.344315 seg_tgce-0.1.3.dev3/seg_tgce/experiments/apr_14_2024/experiment.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/loss/__init__.py
+-rw-r--r--   0        0        0     3490 2024-05-21 12:52:46.131164 seg_tgce-0.1.3.dev3/seg_tgce/loss/tgce.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/metrics/__init__.py
+-rw-r--r--   0        0        0     1530 2024-05-21 12:52:02.884656 seg_tgce-0.1.3.dev3/seg_tgce/metrics/dice_coefficient.py
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/models/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-06 05:22:57.754965 seg_tgce-0.1.3.dev3/seg_tgce/models/ma_model.py
+-rw-r--r--   0        0        0     4618 2024-05-06 05:10:53.688560 seg_tgce-0.1.3.dev3/seg_tgce/models/unet.py
+-rw-r--r--   0        0        0        0 2024-04-30 04:42:11.177868 seg_tgce-0.1.3.dev3/seg_tgce/py.typed
+-rw-r--r--   0        0        0        0 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/run/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 04:39:26.044844 seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/__init__.py
+-rw-r--r--   0        0        0      414 2024-05-06 05:13:40.777698 seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/model_result.py
+-rw-r--r--   0        0        0     2473 2024-05-21 12:52:02.877989 seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/plotting.py
+-rw-r--r--   0        0        0     7072 2024-05-21 12:42:11.676806 seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/runner.py
+-rw-r--r--   0        0        0      800 2024-04-16 19:11:40.745930 seg_tgce-0.1.3.dev3/seg_tgce/run/runner.py
+-rw-r--r--   0        0        0     1144 1970-01-01 00:00:00.000000 seg_tgce-0.1.3.dev3/PKG-INFO
```

### Comparing `seg_tgce-0.1.3.dev2/pyproject.toml` & `seg_tgce-0.1.3.dev3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 description = "Framework for handling image segmentation in the context of multiple annotators"
 name = "seg_tgce"
-version = "0.1.3.dev2"
+version = "0.1.3.dev3"
 readme = "README.md"
 authors = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
 maintainers = [{ name = "Brandon Lotero", email = "blotero@gmail.com" }]
 license = { file = "../LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/blotero/seg_tgce"
 Documentation = "https://seg-tgce.readthedocs.io/en/latest/"
 Repository = "https://github.com/blotero/seg_tgce"
 Issues = "https://github.com/blotero/seg_tgce/issues"
 
 [tool.poetry]
 name = "seg_tgce"
-version = "0.1.3.dev2"
+version = "0.1.3.dev3"
 authors = ["Brandon Lotero <blotero@gmail.com>"]
 description = "A package for the SEG TGCE project"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/__init__.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 from typing import Tuple
 
 from .generator import ImageDataGenerator
 from .stage import Stage
 
-_DEFAULT_N_CLASSES = 6
-
 
 def get_all_data(
-    n_classes: int = _DEFAULT_N_CLASSES,
     image_size: Tuple[int, int] = (256, 256),
     batch_size: int = 32,
-    shuffle: bool = True,
+    shuffle: bool = False,
 ) -> Tuple[ImageDataGenerator, ...]:
     """
     Retrieve all data generators for the crowd segmentation task.
     returns a tuple of ImageDataGenerator instances for the train, val, and test stages.
     """
     return tuple(
         ImageDataGenerator(
             batch_size=batch_size,
-            n_classes=n_classes,
             image_size=image_size,
             shuffle=shuffle,
             stage=stage,
         )
         for stage in (Stage.TRAIN, Stage.VAL, Stage.TEST)
     )
 
 
 def get_stage_data(
     stage: Stage,
-    n_classes: int = _DEFAULT_N_CLASSES,
     image_size: Tuple[int, int] = (256, 256),
     batch_size: int = 32,
-    shuffle: bool = True,
+    shuffle: bool = False,
 ) -> ImageDataGenerator:
     """
     Retrieve a data generator for a specific stage of the crowd segmentation task.
     """
     return ImageDataGenerator(
         batch_size=batch_size,
-        n_classes=n_classes,
         image_size=image_size,
         shuffle=shuffle,
         stage=stage,
     )
```

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/generator.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,109 +3,154 @@
 from typing import List, Optional, Tuple, TypedDict
 
 import numpy as np
 from keras.preprocessing.image import img_to_array, load_img
 from keras.utils import Sequence
 from matplotlib import pyplot as plt
 from tensorflow import transpose
+from tensorflow import Tensor
+from tensorflow import argmax as tf_argmax
 
-from .retrieve import fetch_data, get_masks_dir, get_patches_dir
+from .__retrieve import fetch_data, get_masks_dir, get_patches_dir
 from .stage import Stage
 
 LOGGER = logging.getLogger(__name__)
 logging.basicConfig(level=logging.WARNING)
 
+CLASSES_DEFINITION = {
+    0: "Ignore",
+    1: "Other",
+    2: "Tumor",
+    3: "Stroma",
+    4: "Benign Inflammation",
+    5: "Necrosis",
+}
+
+
+class ScorerNotFoundError(Exception):
+    pass
+
+
+class InvalidClassLabelError(Exception):
+    pass
+
 
 class CustomPath(TypedDict):
     """Custom path for image and mask directories."""
 
     image_dir: str
     mask_dir: str
 
 
-class ImageDataGenerator(Sequence):  # pylint: disable=too-many-instance-attributes
+def get_image_filenames(image_dir: str) -> List[str]:
+    return sorted(
+        [filename for filename in os.listdir(image_dir) if filename.endswith(".png")]
+    )
+
+
+class ImageDataGenerator(Sequence):
     """
     Data generator for crowd segmentation data.
-    Delivered data is in the form of images and masks.
+    Delivered data is in the form of images, masks and scorers labels.
     Shapes are as follows:
     - images: (batch_size, image_size[0], image_size[1], 3)
-    - masks: (batch_size, image_size[0], image_size[1]), n_classes, n_scorers"""
+    - masks: (batch_size, image_size[0], image_size[1], n_classes, n_scorers)"""
 
     def __init__(  # pylint: disable=too-many-arguments
         self,
-        n_classes: int,
         image_size: Tuple[int, int] = (256, 256),
         batch_size: int = 32,
-        shuffle: bool = True,
+        shuffle: bool = False,
         stage: Stage = Stage.TRAIN,
         paths: Optional[CustomPath] = None,
-    ):
+    ) -> None:
         if paths is not None:
             image_dir = paths["image_dir"]
             mask_dir = paths["mask_dir"]
         else:
             fetch_data()
             image_dir = get_patches_dir(stage)
             mask_dir = get_masks_dir(stage)
         self.image_dir = image_dir
         self.mask_dir = mask_dir
         self.image_size = image_size
         self.batch_size = batch_size
         self.shuffle = shuffle
-        self.image_filenames = sorted(
-            [
-                filename
-                for filename in os.listdir(image_dir)
-                if filename.endswith(".png")
-            ]
-        )
-        self.n_scorers = len(os.listdir(mask_dir))
+        self.image_filenames = get_image_filenames(image_dir)
         self.scorers_tags = sorted(os.listdir(mask_dir))
-        LOGGER.info("Scorer tags: %s", self.scorers_tags)
-        self.n_classes = n_classes
         self.on_epoch_end()
 
-    def __len__(self):
+    @property
+    def classes_definition(self) -> dict[int, str]:
+        """Returns classes definition."""
+        return CLASSES_DEFINITION
+
+    @property
+    def n_classes(self) -> int:
+        """Returns number of classes."""
+        return len(self.classes_definition)
+
+    @property
+    def n_scorers(self) -> int:
+        """Returns number of scorers."""
+        return len(self.scorers_tags)
+
+    def __len__(self) -> int:
         return int(np.ceil(len(self.image_filenames) / self.batch_size))
 
-    def __getitem__(self, index):
+    def __getitem__(self, index: int) -> Tuple[Tensor, Tensor]:
         batch_filenames = self.image_filenames[
             index * self.batch_size : (index + 1) * self.batch_size
         ]
-        images, masks = self.__data_generation(batch_filenames)
-        return images, masks
+        return self.__data_generation(batch_filenames)
 
     def on_epoch_end(self) -> None:
         if self.shuffle:
             np.random.shuffle(self.image_filenames)
 
     def visualize_sample(
         self,
-        scorers: List[str],
-        batch_index: int = 1,
-        sample_index: int = 1,
+        scorers: Optional[List[str]] = None,
+        batch_index: int = 0,
+        sample_indexes: Optional[List[int]] = None,
     ) -> plt.Figure:
+        """
+        Visualizes a sample from the dataset."""
+        if scorers is None:
+            scorers = self.scorers_tags
         images, masks = self[batch_index]
+        if sample_indexes is None:
+            sample_indexes = [0, 1, 2, 3]
 
-        fig, axes = plt.subplots(len(scorers), self.n_classes + 1)
-        for scorer_num, scorer in enumerate(scorers):
-            for class_num in range(self.n_classes):
-                axes[scorer_num][0].imshow(images[sample_index].astype(int))
-                axes[scorer_num][class_num + 1].imshow(
-                    masks[sample_index, :, :, class_num, scorer_num]
+        fig, axes = plt.subplots(len(sample_indexes), len(scorers) + 1)
+        for ax in axes.flatten():
+            ax.axis("off")
+
+        for i, sample_index in enumerate(sample_indexes):
+            axes[i, 0].imshow(images[sample_index].astype(int))
+            axes[i, 0].set_title(
+                self.image_filenames[batch_index * self.batch_size + sample_index]
+            )
+            for j, scorer in enumerate(scorers):
+                if scorer not in self.scorers_tags:
+                    raise ScorerNotFoundError(
+                        f"Scorer {scorer} not found in the dataset scorers "
+                        f"({self.scorers_tags})."
+                    )
+                scorer_index = self.scorers_tags.index(scorer)
+                axes[i, j + 1].imshow(
+                    tf_argmax(masks[sample_index, :, :, :, scorer_index], axis=2),
+                    cmap="viridis",
                 )
-                axes[scorer_num][0].axis("off")
-                axes[scorer_num][class_num + 1].axis("off")
-                axes[scorer_num][0].set_title(f"Image (ann {scorer})")
-                axes[scorer_num][class_num + 1].set_title(f"Class {class_num}")
+                axes[i, j + 1].set_title(f"Label for {scorer}")
 
         plt.show()
         return fig
 
-    def __data_generation(self, batch_filenames):
+    def __data_generation(self, batch_filenames: List[str]) -> Tuple[Tensor, Tensor]:
         images = np.empty((self.batch_size, *self.image_size, 3))
         masks = np.empty(
             (
                 self.batch_size,
                 self.n_scorers,
                 self.n_classes,
                 *self.image_size,
@@ -120,29 +165,36 @@
                 if os.path.exists(mask_path):
                     mask_raw = load_img(
                         mask_path,
                         color_mode="grayscale",
                         target_size=self.image_size,
                     )
                     mask = img_to_array(mask_raw)
-                    for class_num in range(self.n_classes):
+                    if not np.all(
+                        np.isin(np.unique(mask), list(self.classes_definition))
+                    ):
+                        raise InvalidClassLabelError(
+                            f"Mask {mask_path} contains invalid values. "
+                            f"Expected values: {list(self.classes_definition)}."
+                            f"Values found: {np.unique(mask)}"
+                        )
+                    for class_num in self.classes_definition:
                         masks[batch][scorer][class_num] = np.where(
                             mask == class_num, 1, 0
                         ).reshape(*self.image_size)
-                    plt.show()
                 else:
                     LOGGER.info(
-                        (
-                            "Mask not found for scorer %s and image %s "
-                            "Filling up with zeros."
-                        ),
+                        "Mask not found for scorer %s and image %s",
                         scorer_dir,
                         filename,
                     )
-                    masks[batch, scorer] = np.zeros((self.n_classes, *self.image_size))
+                    masks[batch, scorer, 0] = np.ones(self.image_size)
+                    masks[batch, scorer, 1:] = np.zeros(
+                        (self.n_classes - 1, *self.image_size)
+                    )
 
             image = load_img(img_path, target_size=self.image_size)
             image = img_to_array(image)
 
             images[batch] = image
 
         return images, transpose(masks, perm=[0, 3, 4, 2, 1])
```

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/retrieve.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/__retrieve.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/crowd_seg/visualizer.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/crowd_seg/visualizer.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/disturbance/model.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/disturbance/model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/oxford_iiit_pet.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/oxford_iiit_pet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/oxford_pet/oxford_pet.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/oxford_pet/oxford_pet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/data/utils.py` & `seg_tgce-0.1.3.dev3/seg_tgce/data/utils.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/experiments/apr_14_2024/experiment.py` & `seg_tgce-0.1.3.dev3/seg_tgce/experiments/apr_14_2024/experiment.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/loss/tgce.py` & `seg_tgce-0.1.3.dev3/seg_tgce/loss/tgce.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/metrics/dice_coefficient.py` & `seg_tgce-0.1.3.dev3/seg_tgce/metrics/dice_coefficient.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/models/ma_model.py` & `seg_tgce-0.1.3.dev3/seg_tgce/models/ma_model.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/models/unet.py` & `seg_tgce-0.1.3.dev3/seg_tgce/models/unet.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/plotting.py` & `seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/plotting.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/run/oxford_ma_runner/runner.py` & `seg_tgce-0.1.3.dev3/seg_tgce/run/oxford_ma_runner/runner.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/seg_tgce/run/runner.py` & `seg_tgce-0.1.3.dev3/seg_tgce/run/runner.py`

 * *Files identical despite different names*

### Comparing `seg_tgce-0.1.3.dev2/PKG-INFO` & `seg_tgce-0.1.3.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seg_tgce
-Version: 0.1.3.dev2
+Version: 0.1.3.dev3
 Summary: A package for the SEG TGCE project
 Home-page: https://github.com/blotero/seg_tgce
 Author: Brandon Lotero
 Author-email: blotero@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

