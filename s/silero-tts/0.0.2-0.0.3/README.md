# Comparing `tmp/silero_tts-0.0.2.tar.gz` & `tmp/silero_tts-0.0.3.tar.gz`

## Comparing `silero_tts-0.0.2.tar` & `silero_tts-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     8323 2020-02-02 00:00:00.000000 silero_tts-0.0.2/README_RU.MD
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 silero_tts-0.0.2/requirements.txt
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 silero_tts-0.0.2/test.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/__main__.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/lang_data.py
--rw-r--r--   0        0        0    12673 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/silero_tts.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/transliterate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_tts-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 silero_tts-0.0.2/tests/test_syntez.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 silero_tts-0.0.2/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 silero_tts-0.0.2/LICENSE
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 silero_tts-0.0.2/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 silero_tts-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 silero_tts-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8323 2020-02-02 00:00:00.000000 silero_tts-0.0.3/README_RU.MD
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 silero_tts-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     6607 2020-02-02 00:00:00.000000 silero_tts-0.0.3/silero_tts/__main__.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 silero_tts-0.0.3/silero_tts/lang_data.py
+-rw-r--r--   0        0        0    13752 2020-02-02 00:00:00.000000 silero_tts-0.0.3/silero_tts/silero_tts.py
+-rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 silero_tts-0.0.3/silero_tts/transliterate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_tts-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 silero_tts-0.0.3/tests/test_syntez.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 silero_tts-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 silero_tts-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 silero_tts-0.0.3/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 silero_tts-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 silero_tts-0.0.3/PKG-INFO
```

### Comparing `silero_tts-0.0.2/README_RU.MD` & `silero_tts-0.0.3/README_RU.MD`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/requirements.txt` & `silero_tts-0.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/silero_tts/__main__.py` & `silero_tts-0.0.3/silero_tts/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,31 +7,30 @@
 def main():
     parser = argparse.ArgumentParser(description='Silero TTS CLI')
     parser.add_argument('--list-models', action='store_true', help='List available models')
     parser.add_argument('--list-speakers', action='store_true', help='List available speakers for a model')
     parser.add_argument('--language', type=str, help='Language code')
     parser.add_argument('--model', type=str, help='Model ID (default: latest version for the language)')
     parser.add_argument('--speaker', type=str, help='Speaker name (default: first available speaker for the model)')
-    parser.add_argument('--sample-rate', type=int, default=48000, help='Sample rate (default: 48000)')
+    parser.add_argument('--sample-rate', type=int, help='Sample rate (default: highest available for the model)')
     parser.add_argument('--device', type=str, default='cpu', help='Device to use (default: cpu)')
     parser.add_argument('--text', type=str, help='Text to synthesize')
     parser.add_argument('--input-file', type=str, help='Input text file to synthesize')
     parser.add_argument('--input-dir', type=str, help='Input directory with text files to synthesize')
     parser.add_argument('--output-file', type=str, default='output.wav', help='Output audio file (default: output.wav)')
     parser.add_argument('--output-dir', type=str, default='output', help='Output directory for synthesized audio files (default: output)')
     args = parser.parse_args()
 
     try:
-         
         models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
 
         if not os.path.exists(models_file):
             logger.warning(f"Models config file not found: {models_file}. Downloading...")
             SileroTTS.download_models_config_static(models_file)
-        
+
         if args.list_models:
             models = SileroTTS.get_available_models()
             logger.info(f"Available models: {models}")
         else:
             if not args.language:
                 logger.error("Please specify the language using the --language flag.")
                 logger.info(f"Available languages: {', '.join(SileroTTS.get_available_languages())}")
@@ -39,26 +38,38 @@
             elif args.language not in SileroTTS.get_available_languages():
                 logger.error(f"Language '{args.language}' is not supported.")
                 logger.info(f"Available languages: {', '.join(SileroTTS.get_available_languages())}")
                 return
 
             if not args.model:
                 args.model = SileroTTS.get_latest_model(args.language)
-                logger.warning(f"Using the latest model for {args.language}: {args.model}")
+                logger.warning(f"Model not specified. Using the latest model for {args.language}: {args.model}")
                 logger.info(f"You can specify a different model using the --model flag.")
                 logger.info(f"Example: --model v4_ru")
                 logger.info(f"Available models for {args.language}: {', '.join(SileroTTS.get_available_models()[args.language])}")
 
+            if not args.sample_rate:
+                available_sample_rates = SileroTTS.get_available_sample_rates_static(args.language, args.model)
+                args.sample_rate = max(available_sample_rates)
+                logger.warning(f"Sample rate not specified. Using the highest available sample rate: {args.sample_rate}")
+            else:
+                available_sample_rates = SileroTTS.get_available_sample_rates_static(args.language, args.model)
+                if args.sample_rate not in available_sample_rates:
+                    logger.warning(f"The specified sample rate {args.sample_rate} is not supported by the model {args.model}.")
+                    logger.info(f"Available sample rates for this model: {', '.join(map(str, available_sample_rates))}")
+                    args.sample_rate = max(available_sample_rates)
+                    logger.info(f"Using the highest available sample rate: {args.sample_rate}")
+
             logger.info(f"Initializing TTS with model: {args.model}, language: {args.language}, speaker: {args.speaker}")
             tts = SileroTTS(model_id=args.model, language=args.language, speaker=args.speaker,
                             sample_rate=args.sample_rate, device=args.device)
             logger.success(f"TTS initialized successfully.")
 
             if not args.speaker:
-                logger.warning(f"Using the default speaker: {tts.speaker}")
+                logger.warning(f"Speaker not specified. Using the default speaker: {tts.speaker}")
                 logger.info(f"You can specify a different speaker using the --speaker flag.")
                 logger.info(f"Example: --speaker aidar")
                 logger.info(f"Available speakers for model {args.model}: {', '.join(tts.get_available_speakers())}")
 
             if args.list_speakers:
                 speakers = tts.get_available_speakers()
                 logger.info(f"Available speakers for model {args.model}: {speakers}")
@@ -87,9 +98,9 @@
                         output_path = os.path.join(args.output_dir, f"{os.path.splitext(txt_file)[0]}.wav")
                         tts.from_file(input_path, output_path)
 
                     logger.success(f"Batch synthesis completed. Output files saved in: {args.output_dir}")
     except Exception as e:
         logger.exception(f"An error occurred: {str(e)}")
 
-if __name__ == '__main__':
+if __name__== '__main__':
     main()
```

### Comparing `silero_tts-0.0.2/silero_tts/lang_data.py` & `silero_tts-0.0.3/silero_tts/lang_data.py`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/silero_tts/silero_tts.py` & `silero_tts-0.0.3/silero_tts/silero_tts.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,23 @@
             logger.success(f"Models config file downloaded: {models_file}")
         else:
             logger.error(f"Failed to download models config file. Status code: {response.status_code}")
             raise Exception(f"Failed to download models config file. Status code: {response.status_code}")
 
     def get_available_speakers(self):
         return self.tts_model.speakers
+    
+    def get_available_sample_rates(self):
+        model_config = self.models_config['tts_models'][self.language][self.model_id]['latest']
+        sample_rates = model_config.get('sample_rate', [])
+
+        if not isinstance(sample_rates, list):
+            sample_rates = [sample_rates]
+
+        return sample_rates
 
     def validate_model(self):
         model_config = self.models_config['tts_models'][self.language][self.model_id]['latest']
 
         if self.sample_rate not in model_config['sample_rate']:
             logger.error(f"Sample rate {self.sample_rate} is not supported for model '{self.model_id}'. Supported sample rates: {model_config['sample_rate']}")
             raise ValueError(f"Sample rate {self.sample_rate} is not supported for model '{self.model_id}'. Supported sample rates: {model_config['sample_rate']}")
@@ -248,22 +257,22 @@
         models = models_config['tts_models'][language]
         latest_model = sorted(models.keys(), reverse=True)[0]
         return latest_model
 
     @staticmethod
     def get_available_languages():
         models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
-    
+
         if not os.path.exists(models_file):
             logger.warning(f"Models config file not found: {models_file}. Downloading...")
             SileroTTS.download_models_config_static(models_file)
-    
+
         with open(models_file, 'r', encoding='utf-8') as f:
             models_config = yaml.safe_load(f)
-    
+
         return list(models_config['tts_models'].keys())
             
     
     @staticmethod
     def download_models_config_static(models_file=None):
         url = "https://raw.githubusercontent.com/snakers4/silero-models/master/models.yml"
         response = requests.get(url)
@@ -276,14 +285,34 @@
                 f.write(response.text)
             logger.success(f"Models config file downloaded: {models_file}")
         else:
             logger.error(f"Failed to download models config file. Status code: {response.status_code}")
             raise Exception(f"Failed to download models config file. Status code: {response.status_code}")
 
 
+    @staticmethod
+    def get_available_sample_rates_static(language, model_id):
+        models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
+
+        if not os.path.exists(models_file):
+            logger.warning(f"Models config file not found: {models_file}. Downloading...")
+            SileroTTS.download_models_config_static(models_file)
+
+        with open(models_file, 'r', encoding='utf-8') as f:
+            models_config = yaml.safe_load(f)
+
+        model_config = models_config['tts_models'][language][model_id]['latest']
+        sample_rates = model_config.get('sample_rate', [])
+
+        if not isinstance(sample_rates, list):
+            sample_rates = [sample_rates]
+
+        return sample_rates
+
+
 if __name__== '__main__':
     tts = SileroTTS(model_id='v4_ru',
                     language='ru',
                     speaker='aidar',
                     sample_rate=48000,
                     device='cpu')
```

### Comparing `silero_tts-0.0.2/silero_tts/transliterate.py` & `silero_tts-0.0.3/silero_tts/transliterate.py`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/tests/test_syntez.py` & `silero_tts-0.0.3/tests/test_syntez.py`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/.gitignore` & `silero_tts-0.0.3/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -157,7 +157,8 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 output.wav
 silero_tts/latest_silero_models.yml
 /tests/tests_temp
+test.py
```

### Comparing `silero_tts-0.0.2/LICENSE` & `silero_tts-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/README.md` & `silero_tts-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.2/pyproject.toml` & `silero_tts-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-tts"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="daswer123", email="daswerq123@gmail.com" },
 ]
 description = "Script over the official Silero so that it can be conveniently and quickly used from the code or from the console"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `silero_tts-0.0.2/PKG-INFO` & `silero_tts-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: silero-tts
-Version: 0.0.2
+Version: 0.0.3
 Summary: Script over the official Silero so that it can be conveniently and quickly used from the code or from the console
 Project-URL: Homepage, https://github.com/daswer123/silero_cli
 Project-URL: Bug Tracker, https://github.com/daswer123/silero_cli/issues
 Author-email: daswer123 <daswerq123@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

