# Comparing `tmp/adetailer-24.5.0.tar.gz` & `tmp/adetailer-24.5.1.tar.gz`

## Comparing `adetailer-24.5.0.tar` & `adetailer-24.5.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 adetailer-24.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    16006 2020-02-02 00:00:00.000000 adetailer-24.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 adetailer-24.5.0/Taskfile.yml
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 adetailer-24.5.0/install.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 adetailer-24.5.0/preload.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 adetailer-24.5.0/.github/workflows/lgtm.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 adetailer-24.5.0/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 adetailer-24.5.0/.github/workflows/stale.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adetailer-24.5.0/.vscode/extensions.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 adetailer-24.5.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/__init__.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/conditional.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/helper.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/p_method.py
--rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/traceback.py
--rw-r--r--   0        0        0    23520 2020-02-02 00:00:00.000000 adetailer-24.5.0/aaaaaa/ui.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/__version__.py
--rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/args.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/common.py
--rw-r--r--   0        0        0     6731 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/mask.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/mediapipe.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 adetailer-24.5.0/adetailer/ultralytics.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 adetailer-24.5.0/controlnet_ext/__init__.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adetailer-24.5.0/controlnet_ext/common.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 adetailer-24.5.0/controlnet_ext/controlnet_ext.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 adetailer-24.5.0/controlnet_ext/controlnet_ext_forge.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 adetailer-24.5.0/controlnet_ext/restore.py
--rw-r--r--   0        0        0    34230 2020-02-02 00:00:00.000000 adetailer-24.5.0/scripts/!adetailer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/__init__.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/conftest.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/test_args.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/test_common.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/test_mask.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/test_mediapipe.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 adetailer-24.5.0/tests/test_ultralytics.py
--rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 adetailer-24.5.0/.gitignore
--rw-r--r--   0        0        0    34270 2020-02-02 00:00:00.000000 adetailer-24.5.0/LICENSE.md
--rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 adetailer-24.5.0/README.md
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 adetailer-24.5.0/pyproject.toml
--rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 adetailer-24.5.0/PKG-INFO
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 adetailer-24.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    16172 2020-02-02 00:00:00.000000 adetailer-24.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 adetailer-24.5.1/Taskfile.yml
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 adetailer-24.5.1/install.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 adetailer-24.5.1/preload.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 adetailer-24.5.1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 adetailer-24.5.1/.github/ISSUE_TEMPLATE/feature_request.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 adetailer-24.5.1/.github/workflows/lgtm.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 adetailer-24.5.1/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 adetailer-24.5.1/.github/workflows/stale.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 adetailer-24.5.1/.vscode/extensions.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 adetailer-24.5.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/__init__.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/conditional.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/helper.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/p_method.py
+-rw-r--r--   0        0        0     4273 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/traceback.py
+-rw-r--r--   0        0        0    23520 2020-02-02 00:00:00.000000 adetailer-24.5.1/aaaaaa/ui.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/__version__.py
+-rw-r--r--   0        0        0     9341 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/args.py
+-rw-r--r--   0        0        0     4346 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/common.py
+-rw-r--r--   0        0        0     6799 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/mask.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/mediapipe.py
+-rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 adetailer-24.5.1/adetailer/ultralytics.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 adetailer-24.5.1/controlnet_ext/__init__.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 adetailer-24.5.1/controlnet_ext/common.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 adetailer-24.5.1/controlnet_ext/controlnet_ext.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 adetailer-24.5.1/controlnet_ext/controlnet_ext_forge.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 adetailer-24.5.1/controlnet_ext/restore.py
+-rw-r--r--   0        0        0    34230 2020-02-02 00:00:00.000000 adetailer-24.5.1/scripts/!adetailer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/__init__.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/conftest.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/test_args.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/test_common.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/test_mask.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/test_mediapipe.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 adetailer-24.5.1/tests/test_ultralytics.py
+-rw-r--r--   0        0        0     3897 2020-02-02 00:00:00.000000 adetailer-24.5.1/.gitignore
+-rw-r--r--   0        0        0    34270 2020-02-02 00:00:00.000000 adetailer-24.5.1/LICENSE.md
+-rw-r--r--   0        0        0     8479 2020-02-02 00:00:00.000000 adetailer-24.5.1/README.md
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 adetailer-24.5.1/pyproject.toml
+-rw-r--r--   0        0        0     9179 2020-02-02 00:00:00.000000 adetailer-24.5.1/PKG-INFO
```

### Comparing `adetailer-24.5.0/.pre-commit-config.yaml` & `adetailer-24.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/CHANGELOG.md` & `adetailer-24.5.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 2024-05-20
+
+- v24.5.1
+- uv를 사용하지 않게 함
+- 모든 허깅페이스 모델을 동시에 다운로드 시도함
+- 기본 탭 수를 2에서 4로 변경
+
 ## 2024-05-19
 
 - v24.5.0
 - 개별 탭 활성화/비활성화 체크박스 추가
 - ad_extra_model_dir 옵션에 |로 구분된 여러 디렉토리를 추가할 수 있게 함 (PR #596)
 - `hypertile` 빌트인 확장이 지원되도록 함
 - 항상 cond 캐시를 비움
```

### Comparing `adetailer-24.5.0/Taskfile.yml` & `adetailer-24.5.1/Taskfile.yml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/install.py` & `adetailer-24.5.1/install.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import importlib.util
-import os
 import subprocess
 import sys
 from importlib.metadata import version  # python >= 3.8
 
 from packaging.version import parse
 
 import_name = {"py-cpuinfo": "cpuinfo", "protobuf": "google.protobuf"}
@@ -35,50 +34,42 @@
         pkg_version = version(package)
         return parse(min_version) <= parse(pkg_version) <= parse(max_version)
     except Exception:
         return False
 
 
 def run_pip(*args):
-    subprocess.run([sys.executable, "-m", "pip", "install", *args], check=False)
-
-
-def run_uv_pip(*args):
-    subprocess.run([sys.executable, "-m", "uv", "pip", "install", *args], check=False)
+    subprocess.run([sys.executable, "-m", "pip", "install", *args], check=True)
 
 
 def install():
     deps = [
         # requirements
         ("ultralytics", "8.2.0", None),
         ("mediapipe", "0.10.13", None),
         ("rich", "13.0.0", None),
         # mediapipe
         ("protobuf", "4.25.3", "4.9999"),
     ]
 
-    if not is_installed("uv", "0.1.44", None):
-        run_pip("uv>=0.1.44")
-
-    os.environ["UV_PYTHON"] = sys.executable
-
     pkgs = []
     for pkg, low, high in deps:
         if not is_installed(pkg, low, high):
             if low and high:
                 cmd = f"{pkg}>={low},<={high}"
             elif low:
                 cmd = f"{pkg}>={low}"
             elif high:
                 cmd = f"{pkg}<={high}"
             else:
                 cmd = pkg
             pkgs.append(cmd)
 
-    run_uv_pip(*pkgs)
+    if pkgs:
+        run_pip(*pkgs)
 
 
 try:
     import launch
 
     skip_install = launch.args.skip_install
 except Exception:
```

### Comparing `adetailer-24.5.0/.github/ISSUE_TEMPLATE/bug_report.yaml` & `adetailer-24.5.1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/.github/ISSUE_TEMPLATE/feature_request.yaml` & `adetailer-24.5.1/.github/ISSUE_TEMPLATE/feature_request.yaml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/.github/workflows/pypi.yml` & `adetailer-24.5.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/aaaaaa/helper.py` & `adetailer-24.5.1/aaaaaa/helper.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/aaaaaa/p_method.py` & `adetailer-24.5.1/aaaaaa/p_method.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/aaaaaa/traceback.py` & `adetailer-24.5.1/aaaaaa/traceback.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/aaaaaa/ui.py` & `adetailer-24.5.1/aaaaaa/ui.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/adetailer/args.py` & `adetailer-24.5.1/adetailer/args.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/adetailer/common.py` & `adetailer-24.5.1/adetailer/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,40 @@
 from __future__ import annotations
 
 import os
 from collections import OrderedDict
+from concurrent.futures import ThreadPoolExecutor
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, Optional
+from typing import Any, Generic, Optional, TypeVar
 
 from huggingface_hub import hf_hub_download
 from PIL import Image, ImageDraw
 from rich import print
 from torchvision.transforms.functional import to_pil_image
 
 REPO_ID = "Bingsu/adetailer"
-_download_failed = False
+
+T = TypeVar("T", int, float)
 
 
 @dataclass
-class PredictOutput:
-    bboxes: list[list[int | float]] = field(default_factory=list)
+class PredictOutput(Generic[T]):
+    bboxes: list[list[T]] = field(default_factory=list)
     masks: list[Image.Image] = field(default_factory=list)
     preview: Optional[Image.Image] = None
 
 
-def hf_download(file: str, repo_id: str = REPO_ID) -> str | None:
-    global _download_failed
-
-    if _download_failed:
-        return "INVALID"
-
+def hf_download(file: str, repo_id: str = REPO_ID) -> str:
     try:
         path = hf_hub_download(repo_id, file)
     except Exception:
         msg = f"[-] ADetailer: Failed to load model {file!r} from huggingface"
         print(msg)
         path = "INVALID"
-        _download_failed = True
     return path
 
 
 def safe_mkdir(path: str | os.PathLike[str]) -> None:
     path = Path(path)
     if not path.exists() and path.parent.exists() and os.access(path.parent, os.W_OK):
         path.mkdir()
@@ -46,38 +42,49 @@
 
 def scan_model_dir(path: Path) -> list[Path]:
     if not path.is_dir():
         return []
     return [p for p in path.rglob("*") if p.is_file() and p.suffix == ".pt"]
 
 
+def download_models(*names: str) -> dict[str, str]:
+    models = OrderedDict()
+    with ThreadPoolExecutor() as executor:
+        for name in names:
+            if "-world" in name:
+                models[name] = executor.submit(
+                    hf_download, name, repo_id="Bingsu/yolo-world-mirror"
+                )
+            else:
+                models[name] = executor.submit(hf_download, name)
+    return {name: future.result() for name, future in models.items()}
+
+
 def get_models(
     *dirs: str | os.PathLike[str], huggingface: bool = True
 ) -> OrderedDict[str, str]:
     model_paths = []
 
     for dir_ in dirs:
         if not dir_:
             continue
         model_paths.extend(scan_model_dir(Path(dir_)))
 
     models = OrderedDict()
     if huggingface:
-        models.update(
-            {
-                "face_yolov8n.pt": hf_download("face_yolov8n.pt"),
-                "face_yolov8s.pt": hf_download("face_yolov8s.pt"),
-                "hand_yolov8n.pt": hf_download("hand_yolov8n.pt"),
-                "person_yolov8n-seg.pt": hf_download("person_yolov8n-seg.pt"),
-                "person_yolov8s-seg.pt": hf_download("person_yolov8s-seg.pt"),
-                "yolov8x-worldv2.pt": hf_download(
-                    "yolov8x-worldv2.pt", repo_id="Bingsu/yolo-world-mirror"
-                ),
-            }
-        )
+        to_download = [
+            "face_yolov8n.pt",
+            "face_yolov8s.pt",
+            "hand_yolov8n.pt",
+            "person_yolov8n-seg.pt",
+            "person_yolov8s-seg.pt",
+            "yolov8x-worldv2.pt",
+        ]
+        models.update(download_models(*to_download))
+
     models.update(
         {
             "mediapipe_face_full": "mediapipe_face_full",
             "mediapipe_face_short": "mediapipe_face_short",
             "mediapipe_face_mesh": "mediapipe_face_mesh",
             "mediapipe_face_mesh_eyes_only": "mediapipe_face_mesh_eyes_only",
         }
```

### Comparing `adetailer-24.5.0/adetailer/mask.py` & `adetailer-24.5.1/adetailer/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from enum import IntEnum
 from functools import partial, reduce
 from math import dist
-from typing import Any
+from typing import Any, TypeVar
 
 import cv2
 import numpy as np
 from PIL import Image, ImageChops
 
 from adetailer.args import MASK_MERGE_INVERT
 from adetailer.common import PredictOutput, ensure_pil_image
@@ -22,14 +22,17 @@
 
 class MergeInvert(IntEnum):
     NONE = 0
     MERGE = 1
     MERGE_INVERT = 2
 
 
+T = TypeVar("T", int, float)
+
+
 def _dilate(arr: np.ndarray, value: int) -> np.ndarray:
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (value, value))
     return cv2.dilate(arr, kernel, iterations=1)
 
 
 def _erode(arr: np.ndarray, value: int) -> np.ndarray:
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (value, value))
@@ -92,15 +95,15 @@
 
 def has_intersection(im1: Any, im2: Any) -> bool:
     arr1 = np.array(ensure_pil_image(im1, "L"))
     arr2 = np.array(ensure_pil_image(im2, "L"))
     return not is_all_black(cv2.bitwise_and(arr1, arr2))
 
 
-def bbox_area(bbox: list[float]) -> float:
+def bbox_area(bbox: list[T]) -> T:
     return (bbox[2] - bbox[0]) * (bbox[3] - bbox[1])
 
 
 def mask_preprocess(
     masks: list[Image.Image],
     kernel: int = 0,
     x_offset: int = 0,
@@ -137,56 +140,56 @@
         masks = [dilate_erode(m, kernel) for m in masks]
         masks = [m for m in masks if not is_all_black(m)]
 
     return mask_merge_invert(masks, mode=merge_invert)
 
 
 # Bbox sorting
-def _key_left_to_right(bbox: list[float]) -> float:
+def _key_left_to_right(bbox: list[T]) -> T:
     """
     Left to right
 
     Parameters
     ----------
-    bbox: list[float]
+    bbox: list[int] | list[float]
         list of [x1, y1, x2, y2]
     """
     return bbox[0]
 
 
-def _key_center_to_edge(bbox: list[float], *, center: tuple[float, float]) -> float:
+def _key_center_to_edge(bbox: list[T], *, center: tuple[float, float]) -> float:
     """
     Center to edge
 
     Parameters
     ----------
-    bbox: list[float]
+    bbox: list[int] | list[float]
         list of [x1, y1, x2, y2]
     image: Image.Image
         the image
     """
     bbox_center = ((bbox[0] + bbox[2]) / 2, (bbox[1] + bbox[3]) / 2)
     return dist(center, bbox_center)
 
 
-def _key_area(bbox: list[float]) -> float:
+def _key_area(bbox: list[T]) -> T:
     """
     Large to small
 
     Parameters
     ----------
-    bbox: list[float]
+    bbox: list[int] | list[float]
         list of [x1, y1, x2, y2]
     """
     return -bbox_area(bbox)
 
 
 def sort_bboxes(
-    pred: PredictOutput, order: int | SortBy = SortBy.NONE
-) -> PredictOutput:
+    pred: PredictOutput[T], order: int | SortBy = SortBy.NONE
+) -> PredictOutput[T]:
     if order == SortBy.NONE or len(pred.bboxes) <= 1:
         return pred
 
     if order == SortBy.LEFT_TO_RIGHT:
         key = _key_left_to_right
     elif order == SortBy.CENTER_TO_EDGE:
         width, height = pred.preview.size
@@ -201,33 +204,35 @@
     idx = sorted(range(items), key=lambda i: key(pred.bboxes[i]))
     pred.bboxes = [pred.bboxes[i] for i in idx]
     pred.masks = [pred.masks[i] for i in idx]
     return pred
 
 
 # Filter by ratio
-def is_in_ratio(bbox: list[float], low: float, high: float, orig_area: int) -> bool:
+def is_in_ratio(bbox: list[T], low: float, high: float, orig_area: int) -> bool:
     area = bbox_area(bbox)
     return low <= area / orig_area <= high
 
 
-def filter_by_ratio(pred: PredictOutput, low: float, high: float) -> PredictOutput:
+def filter_by_ratio(
+    pred: PredictOutput[T], low: float, high: float
+) -> PredictOutput[T]:
     if not pred.bboxes:
         return pred
 
     w, h = pred.preview.size
     orig_area = w * h
     items = len(pred.bboxes)
     idx = [i for i in range(items) if is_in_ratio(pred.bboxes[i], low, high, orig_area)]
     pred.bboxes = [pred.bboxes[i] for i in idx]
     pred.masks = [pred.masks[i] for i in idx]
     return pred
 
 
-def filter_k_largest(pred: PredictOutput, k: int = 0) -> PredictOutput:
+def filter_k_largest(pred: PredictOutput[T], k: int = 0) -> PredictOutput[T]:
     if not pred.bboxes or k == 0:
         return pred
     areas = [bbox_area(bbox) for bbox in pred.bboxes]
     idx = np.argsort(areas)[-k:]
     idx = idx[::-1]
     pred.bboxes = [pred.bboxes[i] for i in idx]
     pred.masks = [pred.masks[i] for i in idx]
```

### Comparing `adetailer-24.5.0/adetailer/mediapipe.py` & `adetailer-24.5.1/adetailer/mediapipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return func(image, confidence)
     msg = f"[-] ADetailer: Invalid mediapipe model type: {model_type}, Available: {list(mapping.keys())!r}"
     raise RuntimeError(msg)
 
 
 def mediapipe_face_detection(
     model_type: int, image: Image.Image, confidence: float = 0.3
-) -> PredictOutput:
+) -> PredictOutput[float]:
     import mediapipe as mp
 
     img_width, img_height = image.size
 
     mp_face_detection = mp.solutions.face_detection
     draw_util = mp.solutions.drawing_utils
 
@@ -64,15 +64,17 @@
 
     masks = create_mask_from_bbox(bboxes, image.size)
     preview = Image.fromarray(preview_array)
 
     return PredictOutput(bboxes=bboxes, masks=masks, preview=preview)
 
 
-def mediapipe_face_mesh(image: Image.Image, confidence: float = 0.3) -> PredictOutput:
+def mediapipe_face_mesh(
+    image: Image.Image, confidence: float = 0.3
+) -> PredictOutput[int]:
     import mediapipe as mp
 
     mp_face_mesh = mp.solutions.face_mesh
     draw_util = mp.solutions.drawing_utils
     drawing_styles = mp.solutions.drawing_styles
 
     w, h = image.size
@@ -94,30 +96,32 @@
                 image=preview,
                 landmark_list=landmarks,
                 connections=mp_face_mesh.FACEMESH_TESSELATION,
                 landmark_drawing_spec=None,
                 connection_drawing_spec=drawing_styles.get_default_face_mesh_tesselation_style(),
             )
 
-            points = np.intp([(land.x * w, land.y * h) for land in landmarks.landmark])
+            points = np.array(
+                [[land.x * w, land.y * h] for land in landmarks.landmark], dtype=int
+            )
             outline = cv2.convexHull(points).reshape(-1).tolist()
 
             mask = Image.new("L", image.size, "black")
             draw = ImageDraw.Draw(mask)
             draw.polygon(outline, fill="white")
             masks.append(mask)
 
         bboxes = create_bbox_from_mask(masks, image.size)
         preview = Image.fromarray(preview)
         return PredictOutput(bboxes=bboxes, masks=masks, preview=preview)
 
 
 def mediapipe_face_mesh_eyes_only(
     image: Image.Image, confidence: float = 0.3
-) -> PredictOutput:
+) -> PredictOutput[int]:
     import mediapipe as mp
 
     mp_face_mesh = mp.solutions.face_mesh
 
     left_idx = np.array(list(mp_face_mesh.FACEMESH_LEFT_EYE)).flatten()
     right_idx = np.array(list(mp_face_mesh.FACEMESH_RIGHT_EYE)).flatten()
 
@@ -132,15 +136,17 @@
         if pred.multi_face_landmarks is None:
             return PredictOutput()
 
         preview = image.copy()
         masks = []
 
         for landmarks in pred.multi_face_landmarks:
-            points = np.intp([(land.x * w, land.y * h) for land in landmarks.landmark])
+            points = np.array(
+                [[land.x * w, land.y * h] for land in landmarks.landmark], dtype=int
+            )
             left_eyes = points[left_idx]
             right_eyes = points[right_idx]
             left_outline = cv2.convexHull(left_eyes).reshape(-1).tolist()
             right_outline = cv2.convexHull(right_eyes).reshape(-1).tolist()
 
             mask = Image.new("L", image.size, "black")
             draw = ImageDraw.Draw(mask)
```

### Comparing `adetailer-24.5.0/adetailer/ultralytics.py` & `adetailer-24.5.1/adetailer/ultralytics.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 def ultralytics_predict(
     model_path: str | Path,
     image: Image.Image,
     confidence: float = 0.3,
     device: str = "",
     classes: str = "",
-) -> PredictOutput:
+) -> PredictOutput[float]:
     from ultralytics import YOLO
 
     model = YOLO(model_path)
     apply_classes(model, model_path, classes)
     pred = model(image, conf=confidence, device=device)
 
     bboxes = pred[0].boxes.xyxy.cpu().numpy()
```

### Comparing `adetailer-24.5.0/controlnet_ext/__init__.py` & `adetailer-24.5.1/controlnet_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/controlnet_ext/controlnet_ext.py` & `adetailer-24.5.1/controlnet_ext/controlnet_ext.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/controlnet_ext/controlnet_ext_forge.py` & `adetailer-24.5.1/controlnet_ext/controlnet_ext_forge.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/controlnet_ext/restore.py` & `adetailer-24.5.1/controlnet_ext/restore.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/scripts/!adetailer.py` & `adetailer-24.5.1/scripts/!adetailer.py`

 * *Files 0% similar despite different names*

```diff
@@ -849,18 +849,18 @@
 
 
 def on_ui_settings():
     section = ("ADetailer", AFTER_DETAILER)
     shared.opts.add_option(
         "ad_max_models",
         shared.OptionInfo(
-            default=2,
+            default=4,
             label="Max models",
             component=gr.Slider,
-            component_args={"minimum": 1, "maximum": 10, "step": 1},
+            component_args={"minimum": 1, "maximum": 15, "step": 1},
             section=section,
         ),
     )
 
     shared.opts.add_option(
         "ad_extra_models_dir",
         shared.OptionInfo(
```

### Comparing `adetailer-24.5.0/tests/test_args.py` & `adetailer-24.5.1/tests/test_args.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/tests/test_common.py` & `adetailer-24.5.1/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/tests/test_mask.py` & `adetailer-24.5.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/tests/test_ultralytics.py` & `adetailer-24.5.1/tests/test_ultralytics.py`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/.gitignore` & `adetailer-24.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/LICENSE.md` & `adetailer-24.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/README.md` & `adetailer-24.5.1/README.md`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/pyproject.toml` & `adetailer-24.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adetailer-24.5.0/PKG-INFO` & `adetailer-24.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: adetailer
-Version: 24.5.0
+Version: 24.5.1
 Summary: An object detection and auto-mask extension for stable diffusion webui.
 Project-URL: repository, https://github.com/Bing-su/adetailer
 Author-email: dowon <ks2515@naver.com>
 License: AGPL-3.0
 License-File: LICENSE.md
 Keywords: adetailer,stable-diffusion,stable-diffusion-webui,ultralytics
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

