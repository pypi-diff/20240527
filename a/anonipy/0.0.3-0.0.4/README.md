# Comparing `tmp/anonipy-0.0.3.tar.gz` & `tmp/anonipy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonipy-0.0.3.tar", last modified: Wed May 22 14:00:03 2024, max compression
+gzip compressed data, was "anonipy-0.0.4.tar", last modified: Mon May 27 20:23:33 2024, max compression
```

## Comparing `anonipy-0.0.3.tar` & `anonipy-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.216376 anonipy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 13:59:59.000000 anonipy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-22 14:00:03.216376 anonipy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-22 13:59:59.000000 anonipy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.208376 anonipy-0.0.3/anonipy/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.208376 anonipy-0.0.3/anonipy/anonymize/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/anonipy/anonymize/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/extractors/entity_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/extractors/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/anonipy/anonymize/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/date_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/llm_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/mask_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/generators/number_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/anonipy/anonymize/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/strategies/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/strategies/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/strategies/pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/anonymize/strategies/redaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/anonipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/utils/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-22 13:59:59.000000 anonipy-0.0.3/anonipy/utils/language_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/anonipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7505 2024-05-22 14:00:03.000000 anonipy-0.0.3/anonipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 14:00:03.000000 anonipy-0.0.3/anonipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:00:03.000000 anonipy-0.0.3/anonipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 14:00:03.000000 anonipy-0.0.3/anonipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 14:00:03.000000 anonipy-0.0.3/anonipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-22 13:59:59.000000 anonipy-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 13:59:59.000000 anonipy-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 14:00:03.216376 anonipy-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:00:03.212376 anonipy-0.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_language_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:59:59.000000 anonipy-0.0.3/test/test_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-27 20:23:29.000000 anonipy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-27 20:23:33.356148 anonipy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-27 20:23:29.000000 anonipy-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.348147 anonipy-0.0.4/anonipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/entity_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/date_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/llm_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/mask_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/number_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/redaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/language_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/anonipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-27 20:23:29.000000 anonipy-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 20:23:29.000000 anonipy-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 20:23:33.356148 anonipy-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_language_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_strategies.py
```

### Comparing `anonipy-0.0.3/LICENSE` & `anonipy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/PKG-INFO` & `anonipy-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -26,22 +26,23 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Source, https://github.com/eriknovak/anonipy
 Project-URL: Docs, https://github.com/eriknovak/anonipy
+Keywords: python,machine learning,natural language processing,anonymization
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy
 Requires-Dist: gliner
 Requires-Dist: gliner-spacy
 Requires-Dist: transformers
```

### Comparing `anonipy-0.0.3/README.md` & `anonipy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/extractors/entity_extractor.py` & `anonipy-0.0.4/anonipy/anonymize/extractors/entity_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,10 +76,10 @@
 
         # TODO: make this part more generic
         anoni_entities = []
         spacy_entities = []
         for e in doc.ents:
             label = list(filter(lambda x: x["label"] == e.label_, self.labels))[0]
             if re.match(label["regex"], e.text):
-                anoni_entities.append(convert_spacy_to_entity(e, label))
+                anoni_entities.append(convert_spacy_to_entity(e, **label))
                 spacy_entities.append(e)
         return anoni_entities, spacy_entities
```

### Comparing `anonipy-0.0.3/anonipy/anonymize/generators/date_generator.py` & `anonipy-0.0.4/anonipy/anonymize/generators/date_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/generators/llm_label_generator.py` & `anonipy-0.0.4/anonipy/anonymize/generators/llm_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/generators/mask_label_generator.py` & `anonipy-0.0.4/anonipy/anonymize/generators/mask_label_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,24 +30,26 @@
         self.context_window = context_window
         if use_gpu and not torch.cuda.is_available():
             warnings.warn(
                 "The use_gpu=True flag requires GPU/CUDA, but it is not available. Setting use_gpu=False."
             )
             use_gpu = False
 
+        # prepare the fill-mask pipeline and store the mask token
         model, tokenizer = self._prepare_model_and_tokenizer(model_name, use_gpu)
+        self.mask_token = tokenizer.mask_token
         self.pipeline = pipeline(
-            "fill-mask", model=model, tokenizer=tokenizer, top_k=10
+            "fill-mask", model=model, tokenizer=tokenizer, top_k=40
         )
 
     def generate(self, entity: Entity, text: str, *args, **kwargs):
         masks = self._create_masks(entity)
         input_texts = self._prepare_generate_inputs(masks, text)
         suggestions = self.pipeline(input_texts)
-        return self._create_substitute(masks, suggestions)
+        return self._create_substitute(entity, masks, suggestions)
 
     # =================================
     # Private methods
     # =================================
 
     def _prepare_model_and_tokenizer(self, model_name: str, use_gpu: bool):
         # prepare the model
@@ -63,15 +65,15 @@
         masks = []
         chunks = re.split(r"\s+", entity.text)
         for idx in range(len(chunks)):
             masks.append(
                 {
                     "true_text": chunks[idx],
                     "mask_text": " ".join(
-                        chunks[0:idx] + ["<mask>"] + chunks[idx + 1 :]
+                        chunks[0:idx] + [self.mask_token] + chunks[idx + 1 :]
                     ),
                     "start_index": entity.start_index,
                     "end_index": entity.end_index,
                 }
             )
         return masks
 
@@ -86,22 +88,23 @@
                 text[: m["start_index"]] + m["mask_text"] + text[m["end_index"] :],
                 m["start_index"],
                 m["end_index"],
             )
             for m in masks
         ]
 
-    def _create_substitute(self, masks, suggestions):
+    def _create_substitute(self, entity: Entity, masks, suggestions):
         substitute_chunks = []
         for mask, suggestion in zip(masks, suggestions):
             suggestion = suggestion if type(suggestion) == list else [suggestion]
             viable_suggestions = list(
                 filter(
-                    lambda x: x["token_str"] not in STOPWORDS
-                    and x["token_str"] != mask["true_text"],
+                    lambda x: x["token_str"] != mask["true_text"]
+                    and re.match(entity.regex, x["token_str"])
+                    and x["token_str"] not in STOPWORDS,
                     suggestion,
                 )
             )
             substitute_chunks.append([s["token_str"] for s in viable_suggestions[:3]])
         combinations = list(itertools.product(*substitute_chunks))
         combinations = list(map(lambda x: " ".join(set(x)), combinations))
         return random.choice(combinations) if len(combinations) > 0 else "None"
```

### Comparing `anonipy-0.0.3/anonipy/anonymize/generators/number_generator.py` & `anonipy-0.0.4/anonipy/anonymize/generators/number_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/regex.py` & `anonipy-0.0.4/anonipy/anonymize/regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 The regex definitions for various use cases
 """
 
 from collections import defaultdict
 
+from ..constants import ENTITY_TYPES
+
+
 # =====================================
 # Regex definitions
 # =====================================
 
 REGEX_STRING = ".*"
 REGEX_INTEGER = "\d+"
 REGEX_FLOAT = "[\d\.,]+"
@@ -29,20 +32,20 @@
 
 
 class RegexMap:
 
     def __init__(self):
         self.regex_mapping = defaultdict(lambda: ".*")
         # Define the regex mappings
-        self.regex_mapping["string"] = REGEX_STRING
-        self.regex_mapping["integer"] = REGEX_INTEGER
-        self.regex_mapping["float"] = REGEX_FLOAT
-        self.regex_mapping["date"] = REGEX_DATE
-        self.regex_mapping["email"] = REGEX_EMAIL_ADDRESS
-        self.regex_mapping["phone_number"] = REGEX_PHONE_NUMBER
-        self.regex_mapping["website_url"] = REGEX_WEBSITE_URL
+        self.regex_mapping[ENTITY_TYPES.STRING] = REGEX_STRING
+        self.regex_mapping[ENTITY_TYPES.INTEGER] = REGEX_INTEGER
+        self.regex_mapping[ENTITY_TYPES.FLOAT] = REGEX_FLOAT
+        self.regex_mapping[ENTITY_TYPES.DATE] = REGEX_DATE
+        self.regex_mapping[ENTITY_TYPES.EMAIL] = REGEX_EMAIL_ADDRESS
+        self.regex_mapping[ENTITY_TYPES.PHONE_NUMBER] = REGEX_PHONE_NUMBER
+        self.regex_mapping[ENTITY_TYPES.WEBSITE_URL] = REGEX_WEBSITE_URL
 
     def __call__(self, type: str) -> str:
         return self.regex_mapping[type]
 
 
 regex_map = RegexMap()
```

### Comparing `anonipy-0.0.3/anonipy/anonymize/strategies/masking.py` & `anonipy-0.0.4/anonipy/anonymize/strategies/masking.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/strategies/pseudonymization.py` & `anonipy-0.0.4/anonipy/anonymize/strategies/pseudonymization.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/anonymize/strategies/redaction.py` & `anonipy-0.0.4/anonipy/anonymize/strategies/redaction.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/utils/file_system.py` & `anonipy-0.0.4/anonipy/utils/file_system.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy/utils/language_detector.py` & `anonipy-0.0.4/anonipy/utils/language_detector.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.3/anonipy.egg-info/PKG-INFO` & `anonipy-0.0.4/anonipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -26,22 +26,23 @@
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Source, https://github.com/eriknovak/anonipy
 Project-URL: Docs, https://github.com/eriknovak/anonipy
+Keywords: python,machine learning,natural language processing,anonymization
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: spacy
 Requires-Dist: gliner
 Requires-Dist: gliner-spacy
 Requires-Dist: transformers
```

### Comparing `anonipy-0.0.3/anonipy.egg-info/SOURCES.txt` & `anonipy-0.0.4/anonipy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,13 +27,14 @@
 anonipy/anonymize/strategies/interface.py
 anonipy/anonymize/strategies/masking.py
 anonipy/anonymize/strategies/pseudonymization.py
 anonipy/anonymize/strategies/redaction.py
 anonipy/utils/__init__.py
 anonipy/utils/file_system.py
 anonipy/utils/language_detector.py
+test/test_entity.py
 test/test_extractors.py
 test/test_file_system.py
 test/test_generators.py
 test/test_language_detector.py
 test/test_regex.py
 test/test_strategies.py
```

### Comparing `anonipy-0.0.3/pyproject.toml` & `anonipy-0.0.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
-version = "0.0.3"
+version = "0.0.4"
 name = "anonipy"
 description = "The data anonymization package"
 authors=[{ name = "Erik Novak", email = "erik.novak@ijs.si" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 dynamic = ["dependencies"]
+keywords = ["python", "machine learning", "natural language processing", "anonymization"]
 classifiers = [
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
+    "Topic :: Scientific/Engineering :: Artificial Intelligence"
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Source = "https://github.com/eriknovak/anonipy"
 Docs = "https://github.com/eriknovak/anonipy"
```

