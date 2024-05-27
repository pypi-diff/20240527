# Comparing `tmp/surya_ocr-0.4.8.tar.gz` & `tmp/surya_ocr-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surya_ocr-0.4.8.tar", max compression
+gzip compressed data, was "surya_ocr-0.4.9.tar", max compression
```

## Comparing `surya_ocr-0.4.8.tar` & `surya_ocr-0.4.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    35085 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/LICENSE
--rw-r--r--   0        0        0    25008 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/README.md
--rw-r--r--   0        0        0     3084 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/detect_layout.py
--rw-r--r--   0        0        0     3314 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/detect_text.py
--rw-r--r--   0        0        0     6909 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/ocr_app.py
--rw-r--r--   0        0        0     4112 2024-05-23 23:12:59.433462 surya_ocr-0.4.8/ocr_text.py
--rw-r--r--   0        0        0     1344 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     3720 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/reading_order.py
--rw-r--r--   0        0        0      616 2024-05-23 23:12:59.437462 surya_ocr-0.4.8/run_ocr_app.py
--rw-r--r--   0        0        0      827 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/bbox.py
--rw-r--r--   0        0        0     4239 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/metrics.py
--rw-r--r--   0        0        0     4971 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/tesseract.py
--rw-r--r--   0        0        0      887 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/benchmark/util.py
--rw-r--r--   0        0        0     5467 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/detection.py
--rw-r--r--   0        0        0      603 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/langs.py
--rw-r--r--   0        0        0     2268 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/load.py
--rw-r--r--   0        0        0     3642 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/input/processing.py
--rw-r--r--   0        0        0     2138 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/languages.py
--rw-r--r--   0        0        0     8723 2024-05-23 23:12:59.577463 surya_ocr-0.4.8/surya/layout.py
--rw-r--r--   0        0        0    13801 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/detection/processor.py
--rw-r--r--   0        0        0     5938 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/detection/segformer.py
--rw-r--r--   0        0        0      159 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/config.py
--rw-r--r--   0        0        0    25734 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/decoder.py
--rw-r--r--   0        0        0     3670 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/encoder.py
--rw-r--r--   0        0        0     3902 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/encoderdecoder.py
--rw-r--r--   0        0        0     1567 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/model.py
--rw-r--r--   0        0        0     5738 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/ordering/processor.py
--rw-r--r--   0        0        0     1676 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/config.py
--rw-r--r--   0        0        0    32140 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/decoder.py
--rw-r--r--   0        0        0     2762 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/encoder.py
--rw-r--r--   0        0        0     2841 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/model.py
--rw-r--r--   0        0        0     8188 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/processor.py
--rw-r--r--   0        0        0     3588 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/model/recognition/tokenizer.py
--rw-r--r--   0        0        0     3953 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/ocr.py
--rw-r--r--   0        0        0     5838 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/ordering.py
--rw-r--r--   0        0        0     5806 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/affinity.py
--rw-r--r--   0        0        0      853 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/fonts.py
--rw-r--r--   0        0        0     7803 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/heatmap.py
--rw-r--r--   0        0        0     3313 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/math/latex.py
--rw-r--r--   0        0        0     3114 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/math/render.py
--rw-r--r--   0        0        0     4382 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/text.py
--rw-r--r--   0        0        0     1253 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/postprocessing/util.py
--rw-r--r--   0        0        0     4004 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/recognition.py
--rw-r--r--   0        0        0     4490 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/schema.py
--rw-r--r--   0        0        0     3776 2024-05-23 23:12:59.581463 surya_ocr-0.4.8/surya/settings.py
--rw-r--r--   0        0        0    26351 1970-01-01 00:00:00.000000 surya_ocr-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35085 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/LICENSE
+-rw-r--r--   0        0        0    25318 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/README.md
+-rw-r--r--   0        0        0     3084 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/detect_layout.py
+-rw-r--r--   0        0        0     3314 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/detect_text.py
+-rw-r--r--   0        0        0     6909 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/ocr_app.py
+-rw-r--r--   0        0        0     4126 2024-05-27 21:56:35.869538 surya_ocr-0.4.9/ocr_text.py
+-rw-r--r--   0        0        0     1344 2024-05-27 21:56:35.873538 surya_ocr-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3720 2024-05-27 21:56:35.873538 surya_ocr-0.4.9/reading_order.py
+-rw-r--r--   0        0        0      616 2024-05-27 21:56:35.873538 surya_ocr-0.4.9/run_ocr_app.py
+-rw-r--r--   0        0        0      827 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/benchmark/bbox.py
+-rw-r--r--   0        0        0     4239 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/benchmark/metrics.py
+-rw-r--r--   0        0        0     4971 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/benchmark/tesseract.py
+-rw-r--r--   0        0        0      887 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/benchmark/util.py
+-rw-r--r--   0        0        0     5467 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/detection.py
+-rw-r--r--   0        0        0      603 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/input/langs.py
+-rw-r--r--   0        0        0     2268 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/input/load.py
+-rw-r--r--   0        0        0     3514 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/input/processing.py
+-rw-r--r--   0        0        0     2138 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/languages.py
+-rw-r--r--   0        0        0     8723 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/layout.py
+-rw-r--r--   0        0        0    13801 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/model/detection/processor.py
+-rw-r--r--   0        0        0     5938 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/model/detection/segformer.py
+-rw-r--r--   0        0        0      159 2024-05-27 21:56:36.013539 surya_ocr-0.4.9/surya/model/ordering/config.py
+-rw-r--r--   0        0        0    25734 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/ordering/decoder.py
+-rw-r--r--   0        0        0     3670 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/ordering/encoder.py
+-rw-r--r--   0        0        0     3902 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/ordering/encoderdecoder.py
+-rw-r--r--   0        0        0     1567 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/ordering/model.py
+-rw-r--r--   0        0        0     5738 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/ordering/processor.py
+-rw-r--r--   0        0        0     1676 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/config.py
+-rw-r--r--   0        0        0    21213 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/decoder.py
+-rw-r--r--   0        0        0    20397 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/encoder.py
+-rw-r--r--   0        0        0     2864 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/model.py
+-rw-r--r--   0        0        0     8026 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/processor.py
+-rw-r--r--   0        0        0     3588 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/model/recognition/tokenizer.py
+-rw-r--r--   0        0        0     3953 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/ocr.py
+-rw-r--r--   0        0        0     5838 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/ordering.py
+-rw-r--r--   0        0        0     5806 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/affinity.py
+-rw-r--r--   0        0        0      853 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/fonts.py
+-rw-r--r--   0        0        0     7803 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/heatmap.py
+-rw-r--r--   0        0        0     3313 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/math/latex.py
+-rw-r--r--   0        0        0     3114 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/math/render.py
+-rw-r--r--   0        0        0     4382 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/text.py
+-rw-r--r--   0        0        0     1253 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/postprocessing/util.py
+-rw-r--r--   0        0        0    10012 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/recognition.py
+-rw-r--r--   0        0        0     4490 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/schema.py
+-rw-r--r--   0        0        0     3887 2024-05-27 21:56:36.017539 surya_ocr-0.4.9/surya/settings.py
+-rw-r--r--   0        0        0    26661 1970-01-01 00:00:00.000000 surya_ocr-0.4.9/PKG-INFO
```

### Comparing `surya_ocr-0.4.8/LICENSE` & `surya_ocr-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/README.md` & `surya_ocr-0.4.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,24 @@
 langs = ["en"] # Replace with your languages
 det_processor, det_model = segformer.load_processor(), segformer.load_model()
 rec_model, rec_processor = load_model(), load_processor()
 
 predictions = run_ocr([image], [langs], det_model, det_processor, rec_model, rec_processor)
 ```
 
+### Compilation
+
+The OCR model can be compiled to get an ~15% speedup in total inference time.  The first run will be slow while it compiles, though. First set `RECOGNITION_STATIC_CACHE=true`, then:
+
+```python
+import torch
+
+rec_model.decoder.model.decoder = torch.compile(rec_model.decoder.model.decoder)
+```
+
 ## Text line detection
 
 This command will write out a json file with the detected bboxes.
 
 ```shell
 surya_detect DATA_PATH --images
 ```
```

### Comparing `surya_ocr-0.4.8/detect_layout.py` & `surya_ocr-0.4.9/detect_layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/detect_text.py` & `surya_ocr-0.4.9/detect_text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/ocr_app.py` & `surya_ocr-0.4.9/ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/ocr_text.py` & `surya_ocr-0.4.9/ocr_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import argparse
 import json
 from collections import defaultdict
 
+import torch
+
 from surya.input.langs import replace_lang_with_code, get_unique_langs
 from surya.input.load import load_from_folder, load_from_file, load_lang_file
 from surya.model.detection.segformer import load_model as load_detection_model, load_processor as load_detection_processor
 from surya.model.recognition.model import load_model as load_recognition_model
 from surya.model.recognition.processor import load_processor as load_recognition_processor
 from surya.model.recognition.tokenizer import _tokenize
 from surya.ocr import run_ocr
```

### Comparing `surya_ocr-0.4.8/pyproject.toml` & `surya_ocr-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surya-ocr"
-version = "0.4.8"
+version = "0.4.9"
 description = "OCR, layout, reading order, and line detection in 90+ languages"
 authors = ["Vik Paruchuri <vik.paruchuri@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/VikParuchuri/surya"
 keywords = ["ocr", "pdf", "text detection", "text recognition"]
 packages = [
```

### Comparing `surya_ocr-0.4.8/reading_order.py` & `surya_ocr-0.4.9/reading_order.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/run_ocr_app.py` & `surya_ocr-0.4.9/run_ocr_app.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/benchmark/bbox.py` & `surya_ocr-0.4.9/surya/benchmark/bbox.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/benchmark/metrics.py` & `surya_ocr-0.4.9/surya/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/benchmark/tesseract.py` & `surya_ocr-0.4.9/surya/benchmark/tesseract.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/benchmark/util.py` & `surya_ocr-0.4.9/surya/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/detection.py` & `surya_ocr-0.4.9/surya/detection.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/input/langs.py` & `surya_ocr-0.4.9/surya/input/langs.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/input/load.py` & `surya_ocr-0.4.9/surya/input/load.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/input/processing.py` & `surya_ocr-0.4.9/surya/input/processing.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,18 +44,17 @@
         return splits, split_heights
     return [img.copy()], [img_height]
 
 
 def prepare_image_detection(img, processor):
     new_size = (processor.size["width"], processor.size["height"])
 
-    img.thumbnail(new_size, Image.Resampling.LANCZOS) # Shrink largest dimension to fit new size
-    img = img.resize(new_size, Image.Resampling.LANCZOS) # Stretch smaller dimension to fit new size
-
     img = np.asarray(img, dtype=np.uint8)
+    img = cv2.resize(img, new_size, interpolation=cv2.INTER_LANCZOS4)
+
     img = processor(img)["pixel_values"][0]
     img = torch.from_numpy(img)
     return img
 
 
 def open_pdf(pdf_filepath):
     return pypdfium2.PdfDocument(pdf_filepath)
```

### Comparing `surya_ocr-0.4.8/surya/languages.py` & `surya_ocr-0.4.9/surya/languages.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/layout.py` & `surya_ocr-0.4.9/surya/layout.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/detection/processor.py` & `surya_ocr-0.4.9/surya/model/detection/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/detection/segformer.py` & `surya_ocr-0.4.9/surya/model/detection/segformer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/ordering/decoder.py` & `surya_ocr-0.4.9/surya/model/ordering/decoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/ordering/encoder.py` & `surya_ocr-0.4.9/surya/model/ordering/encoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/ordering/encoderdecoder.py` & `surya_ocr-0.4.9/surya/model/ordering/encoderdecoder.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/ordering/model.py` & `surya_ocr-0.4.9/surya/model/ordering/model.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/ordering/processor.py` & `surya_ocr-0.4.9/surya/model/ordering/processor.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/recognition/config.py` & `surya_ocr-0.4.9/surya/model/recognition/config.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/model/recognition/model.py` & `surya_ocr-0.4.9/surya/model/recognition/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import warnings
+
+import torch
+
 warnings.filterwarnings("ignore", message="torch.utils._pytree._register_pytree_node is deprecated")
 
 import logging
 logging.getLogger("transformers.modeling_utils").setLevel(logging.ERROR)
 
-from typing import List, Optional
+from typing import List, Optional, Tuple
 from transformers import VisionEncoderDecoderModel, VisionEncoderDecoderConfig, AutoModel, AutoModelForCausalLM
 from surya.model.recognition.config import MBartMoEConfig, VariableDonutSwinConfig
 from surya.model.recognition.encoder import VariableDonutSwinModel
 from surya.model.recognition.decoder import MBartMoE
 from surya.settings import settings
 
 
@@ -54,7 +57,8 @@
             "decoder_input_ids": decoder_inputs["input_ids"],
             "encoder_outputs": encoder_outputs,
             "past_key_values": decoder_inputs["past_key_values"],
             "use_cache": use_cache,
             "decoder_langs": decoder_inputs["langs"],
         }
         return input_dict
+
```

### Comparing `surya_ocr-0.4.8/surya/model/recognition/processor.py` & `surya_ocr-0.4.9/surya/model/recognition/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from typing import Dict, Union, Optional, List, Tuple
+from typing import Dict, Union, Optional, List, Iterable
 
 import cv2
 from torch import TensorType
-from transformers import DonutImageProcessor, DonutProcessor, AutoImageProcessor, DonutSwinConfig
-from transformers.image_processing_utils import BaseImageProcessor, get_size_dict, BatchFeature
-from transformers.image_transforms import to_channel_dimension_format, pad, _rescale_for_pil_conversion, to_pil_image
-from transformers.image_utils import PILImageResampling, ImageInput, ChannelDimension, make_list_of_images, \
-    valid_images, to_numpy_array, is_scaled_image, infer_channel_dimension_format, get_image_size
+from transformers import DonutImageProcessor, DonutProcessor
+from transformers.image_processing_utils import BatchFeature
+from transformers.image_transforms import pad, normalize
+from transformers.image_utils import PILImageResampling, ImageInput, ChannelDimension, make_list_of_images, get_image_size
 import numpy as np
 from PIL import Image
 import PIL
 from surya.model.recognition.tokenizer import Byt5LangTokenizer
 from surya.settings import settings
 
 
@@ -26,15 +25,16 @@
     def __init__(self, *args, max_size=None, train=False, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.patch_size = kwargs.get("patch_size", (4, 4))
         self.max_size = max_size
         self.train = train
 
-    def numpy_resize(self, image: np.ndarray, size, interpolation=cv2.INTER_LANCZOS4):
+    @classmethod
+    def numpy_resize(cls, image: np.ndarray, size, interpolation=cv2.INTER_LANCZOS4):
         height, width = image.shape[:2]
         max_width, max_height = size["width"], size["height"]
 
         if (height == max_height and width <= max_width) or (width == max_width and height <= max_height):
             return image
 
         scale = min(max_width / width, max_height / height)
@@ -43,57 +43,53 @@
         new_height = int(height * scale)
 
         resized_image = cv2.resize(image, (new_width, new_height), interpolation=interpolation)
         resized_image = resized_image.transpose(2, 0, 1)
 
         return resized_image
 
-    def process_inner(self, images: List[np.ndarray], train=False):
+    def process_inner(self, images: List[np.ndarray]):
         assert images[0].shape[2] == 3 # RGB input images, channel dim last
 
         # Rotate if the bbox is wider than it is tall
-        images = [self.align_long_axis(image, size=self.max_size, input_data_format=ChannelDimension.LAST) for image in images]
+        images = [SuryaImageProcessor.align_long_axis(image, size=self.max_size, input_data_format=ChannelDimension.LAST) for image in images]
 
         # Verify that the image is wider than it is tall
         for img in images:
             assert img.shape[1] >= img.shape[0]
 
         # This also applies the right channel dim format, to channel x height x width
-        images = [self.numpy_resize(img, self.max_size, self.resample) for img in images]
+        images = [SuryaImageProcessor.numpy_resize(img, self.max_size, self.resample) for img in images]
         assert images[0].shape[0] == 3 # RGB input images, channel dim first
 
         # Convert to float32 for rescale/normalize
         images = [img.astype(np.float32) for img in images]
 
         # Pads with 255 (whitespace)
         # Pad to max size to improve performance
         max_size = self.max_size
         images = [
-            self.pad_image(
+            SuryaImageProcessor.pad_image(
                 image=image,
                 size=max_size,
-                random_padding=train, # Change amount of padding randomly during training
                 input_data_format=ChannelDimension.FIRST,
                 pad_value=settings.RECOGNITION_PAD_VALUE
             )
             for image in images
         ]
         # Rescale and normalize
+        for idx in range(len(images)):
+            images[idx] = images[idx] * self.rescale_factor
         images = [
-            self.rescale(img, scale=self.rescale_factor, input_data_format=ChannelDimension.FIRST)
-            for img in images
-        ]
-        images = [
-            self.normalize(img, mean=self.image_mean, std=self.image_std, input_data_format=ChannelDimension.FIRST)
+            SuryaImageProcessor.normalize(img, mean=self.image_mean, std=self.image_std, input_data_format=ChannelDimension.FIRST)
             for img in images
         ]
 
         return images
 
-
     def preprocess(
         self,
         images: ImageInput,
         do_resize: bool = None,
         size: Dict[str, int] = None,
         resample: PILImageResampling = None,
         do_thumbnail: bool = None,
@@ -110,50 +106,48 @@
         input_data_format: Optional[Union[str, ChannelDimension]] = None,
         **kwargs,
     ) -> PIL.Image.Image:
         images = make_list_of_images(images)
 
         # Convert to numpy for later processing steps
         images = [np.array(img) for img in images]
-        images = self.process_inner(images, train=self.train)
+        images = self.process_inner(images)
+
         data = {"pixel_values": images}
         return BatchFeature(data=data, tensor_type=return_tensors)
 
+    @classmethod
     def pad_image(
-        self,
+        cls,
         image: np.ndarray,
         size: Dict[str, int],
-        random_padding: bool = False,
         data_format: Optional[Union[str, ChannelDimension]] = None,
         input_data_format: Optional[Union[str, ChannelDimension]] = None,
         pad_value: float = 0.0,
     ) -> np.ndarray:
         output_height, output_width = size["height"], size["width"]
         input_height, input_width = get_image_size(image, channel_dim=input_data_format)
 
         delta_width = output_width - input_width
         delta_height = output_height - input_height
 
         assert delta_width >= 0 and delta_height >= 0
 
-        if random_padding:
-            pad_top = np.random.randint(low=0, high=delta_height + 1)
-            pad_left = np.random.randint(low=0, high=delta_width + 1)
-        else:
-            pad_top = delta_height // 2
-            pad_left = delta_width // 2
+        pad_top = delta_height // 2
+        pad_left = delta_width // 2
 
         pad_bottom = delta_height - pad_top
         pad_right = delta_width - pad_left
 
         padding = ((pad_top, pad_bottom), (pad_left, pad_right))
         return pad(image, padding, data_format=data_format, input_data_format=input_data_format, constant_values=pad_value)
 
+    @classmethod
     def align_long_axis(
-        self,
+        cls,
         image: np.ndarray,
         size: Dict[str, int],
         data_format: Optional[Union[str, ChannelDimension]] = None,
         input_data_format: Optional[Union[str, ChannelDimension]] = None,
     ) -> np.ndarray:
         input_height, input_width = image.shape[:2]
         output_height, output_width = size["height"], size["width"]
@@ -161,14 +155,28 @@
         if (output_width < output_height and input_width > input_height) or (
             output_width > output_height and input_width < input_height
         ):
             image = np.rot90(image, 3)
 
         return image
 
+    @classmethod
+    def normalize(
+        cls,
+        image: np.ndarray,
+        mean: Union[float, Iterable[float]],
+        std: Union[float, Iterable[float]],
+        data_format: Optional[Union[str, ChannelDimension]] = None,
+        input_data_format: Optional[Union[str, ChannelDimension]] = None,
+        **kwargs,
+    ) -> np.ndarray:
+        return normalize(
+            image, mean=mean, std=std, data_format=data_format, input_data_format=input_data_format, **kwargs
+        )
+
 
 class SuryaProcessor(DonutProcessor):
     def __init__(self, image_processor=None, tokenizer=None, train=False, **kwargs):
         image_processor = SuryaImageProcessor.from_pretrained(settings.RECOGNITION_MODEL_CHECKPOINT)
         tokenizer = Byt5LangTokenizer()
         if image_processor is None:
             raise ValueError("You need to specify an `image_processor`.")
@@ -176,18 +184,14 @@
             raise ValueError("You need to specify a `tokenizer`.")
 
         super().__init__(image_processor, tokenizer)
         self.current_processor = self.image_processor
         self._in_target_context_manager = False
 
     def __call__(self, *args, **kwargs):
-        # For backward compatibility
-        if self._in_target_context_manager:
-            return self.current_processor(*args, **kwargs)
-
         images = kwargs.pop("images", None)
         text = kwargs.pop("text", None)
         lang = kwargs.pop("lang", None)
 
         if len(args) > 0:
             images = args[0]
             args = args[1:]
```

### Comparing `surya_ocr-0.4.8/surya/model/recognition/tokenizer.py` & `surya_ocr-0.4.9/surya/model/recognition/tokenizer.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/ocr.py` & `surya_ocr-0.4.9/surya/ocr.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/ordering.py` & `surya_ocr-0.4.9/surya/ordering.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/affinity.py` & `surya_ocr-0.4.9/surya/postprocessing/affinity.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/fonts.py` & `surya_ocr-0.4.9/surya/postprocessing/fonts.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/heatmap.py` & `surya_ocr-0.4.9/surya/postprocessing/heatmap.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/math/latex.py` & `surya_ocr-0.4.9/surya/postprocessing/math/latex.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/math/render.py` & `surya_ocr-0.4.9/surya/postprocessing/math/render.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/text.py` & `surya_ocr-0.4.9/surya/postprocessing/text.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/postprocessing/util.py` & `surya_ocr-0.4.9/surya/postprocessing/util.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/schema.py` & `surya_ocr-0.4.9/surya/schema.py`

 * *Files identical despite different names*

### Comparing `surya_ocr-0.4.8/surya/settings.py` & `surya_ocr-0.4.9/surya/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
         "zh": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
         "ja": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
         "ko": os.path.join(FONT_DIR, "GoNotoCJKCore.ttf"),
     }
     RECOGNITION_FONT_DL_BASE: str = "https://github.com/satbyy/go-noto-universal/releases/download/v7.0"
     RECOGNITION_BENCH_DATASET_NAME: str = "vikp/rec_bench"
     RECOGNITION_PAD_VALUE: int = 255 # Should be 0 or 255
+    RECOGNITION_STATIC_CACHE: bool = False # Static cache for torch compile
+    RECOGNITION_MAX_LANGS: int = 4
 
     # Layout
     LAYOUT_MODEL_CHECKPOINT: str = "vikp/surya_layout2"
     LAYOUT_BENCH_DATASET_NAME: str = "vikp/publaynet_bench"
 
     # Ordering
     ORDER_MODEL_CHECKPOINT: str = "vikp/surya_order"
```

### Comparing `surya_ocr-0.4.8/PKG-INFO` & `surya_ocr-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surya-ocr
-Version: 0.4.8
+Version: 0.4.9
 Summary: OCR, layout, reading order, and line detection in 90+ languages
 Home-page: https://github.com/VikParuchuri/surya
 License: GPL-3.0-or-later
 Keywords: ocr,pdf,text detection,text recognition
 Author: Vik Paruchuri
 Author-email: vik.paruchuri@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
@@ -147,14 +147,24 @@
 langs = ["en"] # Replace with your languages
 det_processor, det_model = segformer.load_processor(), segformer.load_model()
 rec_model, rec_processor = load_model(), load_processor()
 
 predictions = run_ocr([image], [langs], det_model, det_processor, rec_model, rec_processor)
 ```
 
+### Compilation
+
+The OCR model can be compiled to get an ~15% speedup in total inference time.  The first run will be slow while it compiles, though. First set `RECOGNITION_STATIC_CACHE=true`, then:
+
+```python
+import torch
+
+rec_model.decoder.model.decoder = torch.compile(rec_model.decoder.model.decoder)
+```
+
 ## Text line detection
 
 This command will write out a json file with the detected bboxes.
 
 ```shell
 surya_detect DATA_PATH --images
 ```
```

