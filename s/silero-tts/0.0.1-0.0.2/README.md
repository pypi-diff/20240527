# Comparing `tmp/silero_tts-0.0.1.tar.gz` & `tmp/silero_tts-0.0.2.tar.gz`

## Comparing `silero_tts-0.0.1.tar` & `silero_tts-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     8340 2020-02-02 00:00:00.000000 silero_tts-0.0.1/README_RU.MD
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 silero_tts-0.0.1/requirements.txt
--rw-r--r--   0        0        0     5299 2020-02-02 00:00:00.000000 silero_tts-0.0.1/silero_tts/__main__.py
--rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 silero_tts-0.0.1/silero_tts/lang_data.py
--rw-r--r--   0        0        0    31173 2020-02-02 00:00:00.000000 silero_tts-0.0.1/silero_tts/latest_silero_models.yml
--rw-r--r--   0        0        0    11707 2020-02-02 00:00:00.000000 silero_tts-0.0.1/silero_tts/silero_tts.py
--rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 silero_tts-0.0.1/silero_tts/transliterate.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 silero_tts-0.0.1/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 silero_tts-0.0.1/LICENSE
--rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 silero_tts-0.0.1/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 silero_tts-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 silero_tts-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8323 2020-02-02 00:00:00.000000 silero_tts-0.0.2/README_RU.MD
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 silero_tts-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 silero_tts-0.0.2/test.py
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/__main__.py
+-rw-r--r--   0        0        0     5505 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/lang_data.py
+-rw-r--r--   0        0        0    12673 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/silero_tts.py
+-rw-r--r--   0        0        0    12996 2020-02-02 00:00:00.000000 silero_tts-0.0.2/silero_tts/transliterate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 silero_tts-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 silero_tts-0.0.2/tests/test_syntez.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 silero_tts-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 silero_tts-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 silero_tts-0.0.2/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 silero_tts-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 silero_tts-0.0.2/PKG-INFO
```

### Comparing `silero_tts-0.0.1/README_RU.MD` & `silero_tts-0.0.2/README_RU.MD`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Silero TTS Enhanced
 
 **README доступен на следующих языках:**
 
-[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README.md)
-[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.md)
+[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced)
+[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.MD)
 
 Silero TTS Enhanced - это библиотека Python, которая предоставляет удобный способ синтеза речи из текста с использованием различных моделей Silero TTS, языков и голосов. Она может использоваться как автономный скрипт или интегрироваться в ваши собственные проекты на Python.
 
 ## Особенности
 
 - Поддержка нескольких языков и моделей
 - Автоматическая загрузка последнего файла конфигурации модели
@@ -83,15 +83,15 @@
 
 Вы также можете интегрировать Silero TTS в свои собственные проекты на Python, импортируя класс `SileroTTS` и используя его методы.
 
 ```python
 from silero_tts.silero_tts import SileroTTS
 
 # Инициализация объекта TTS
-tts = SileroTTS(model_id='v3_en', language='en', speaker='en_3', sample_rate=48000, device='cpu')
+tts = SileroTTS(model_id='v4_ru', language='ru', speaker='aidar', sample_rate=48000, device='cpu')
 
 # Синтез речи из текста
 text = "Привет, мир!"
 tts.tts(text, 'output.wav')
 
 # Синтез речи из текстового файла
 # tts.from_file('input.txt', 'output.wav')
@@ -138,8 +138,8 @@
 ## Лицензия
 
 Этот проект лицензирован под [MIT License](LICENSE).
 
 ## Благодарности
 
 - [Silero Models](https://github.com/snakers4/silero-models) за предоставление моделей TTS
-- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) эта библиотека вдохновила меня на создание этого проекта.
+- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) эта библиотека вдохновила меня на создание этого проекта.
```

### Comparing `silero_tts-0.0.1/requirements.txt` & `silero_tts-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.1/silero_tts/__main__.py` & `silero_tts-0.0.2/silero_tts/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     parser.add_argument('--input-file', type=str, help='Input text file to synthesize')
     parser.add_argument('--input-dir', type=str, help='Input directory with text files to synthesize')
     parser.add_argument('--output-file', type=str, default='output.wav', help='Output audio file (default: output.wav)')
     parser.add_argument('--output-dir', type=str, default='output', help='Output directory for synthesized audio files (default: output)')
     args = parser.parse_args()
 
     try:
+         
+        models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
+
+        if not os.path.exists(models_file):
+            logger.warning(f"Models config file not found: {models_file}. Downloading...")
+            SileroTTS.download_models_config_static(models_file)
+        
         if args.list_models:
             models = SileroTTS.get_available_models()
             logger.info(f"Available models: {models}")
         else:
             if not args.language:
                 logger.error("Please specify the language using the --language flag.")
                 logger.info(f"Available languages: {', '.join(SileroTTS.get_available_languages())}")
```

### Comparing `silero_tts-0.0.1/silero_tts/lang_data.py` & `silero_tts-0.0.2/silero_tts/lang_data.py`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.1/silero_tts/silero_tts.py` & `silero_tts-0.0.2/silero_tts/silero_tts.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,17 +48,20 @@
             self.download_models_config(models_file)
 
         with open(models_file, 'r', encoding='utf-8') as f:
             models_config = yaml.safe_load(f)
         logger.success(f"Models config loaded from: {models_file}")
         return models_config
 
-    def download_models_config(self, models_file):
+    def download_models_config(self, models_file=None):
         url = "https://raw.githubusercontent.com/snakers4/silero-models/master/models.yml"
         response = requests.get(url)
+        
+        if models_file is None:
+            models_file = os.path.join(os.path.dirname(__file__), 'models.yml')
 
         if response.status_code == 200:
             with open(models_file, 'w', encoding='utf-8') as f:
                 f.write(response.text)
             logger.success(f"Models config file downloaded: {models_file}")
         else:
             logger.error(f"Failed to download models config file. Status code: {response.status_code}")
@@ -216,15 +219,15 @@
 
     @staticmethod
     def get_available_models():
         models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
 
         if not os.path.exists(models_file):
             logger.warning(f"Models config file not found: {models_file}. Downloading...")
-            SileroTTS.download_models_config(models_file)
+            SileroTTS.download_models_config_static(models_file)
 
         with open(models_file, 'r', encoding='utf-8') as f:
             models_config = yaml.safe_load(f)
 
         models_dict = {}
         for lang, models in models_config['tts_models'].items():
             models_dict[lang] = list(models.keys())
@@ -233,35 +236,52 @@
 
     @staticmethod
     def get_latest_model(language):
         models_file = os.path.join(os.path.dirname(__file__), 'latest_silero_models.yml')
 
         if not os.path.exists(models_file):
             logger.warning(f"Models config file not found: {models_file}. Downloading...")
-            SileroTTS.download_models_config(models_file)
+            SileroTTS.download_models_config_static(models_file)
 
         with open(models_file, 'r', encoding='utf-8') as f:
             models_config = yaml.safe_load(f)
 
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
-            SileroTTS.download_models_config(models_file)
-
+            SileroTTS.download_models_config_static(models_file)
+    
         with open(models_file, 'r', encoding='utf-8') as f:
             models_config = yaml.safe_load(f)
-
+    
         return list(models_config['tts_models'].keys())
+            
+    
+    @staticmethod
+    def download_models_config_static(models_file=None):
+        url = "https://raw.githubusercontent.com/snakers4/silero-models/master/models.yml"
+        response = requests.get(url)
+        
+        if models_file is None:
+            models_file = os.path.join(os.path.dirname(__file__), 'models.yml')
+
+        if response.status_code == 200:
+            with open(models_file, 'w', encoding='utf-8') as f:
+                f.write(response.text)
+            logger.success(f"Models config file downloaded: {models_file}")
+        else:
+            logger.error(f"Failed to download models config file. Status code: {response.status_code}")
+            raise Exception(f"Failed to download models config file. Status code: {response.status_code}")
 
 
 if __name__== '__main__':
     tts = SileroTTS(model_id='v4_ru',
                     language='ru',
                     speaker='aidar',
                     sample_rate=48000,
```

### Comparing `silero_tts-0.0.1/silero_tts/transliterate.py` & `silero_tts-0.0.2/silero_tts/transliterate.py`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.1/.gitignore` & `silero_tts-0.0.2/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -155,7 +155,9 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 output.wav
+silero_tts/latest_silero_models.yml
+/tests/tests_temp
```

### Comparing `silero_tts-0.0.1/LICENSE` & `silero_tts-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `silero_tts-0.0.1/README.md` & `silero_tts-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Silero TTS
 
 **README is available in the following languages:**
 
-[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README.md)
-[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.md)
+[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced)
+[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.MD)
 
 Silero TTS is a Python library that provides an easy way to synthesize speech from text using various Silero TTS models, languages, and speakers. It can be used as a standalone script or integrated into your own Python projects.
 
 ## Features
 
 - Support for multiple languages and models
 - Automatic downloading of the latest model configuration file
@@ -138,8 +138,8 @@
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
 
 ## Acknowledgements
 
 - [Silero Models](https://github.com/snakers4/silero-models) for providing the TTS models
-- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) this library inspired me to create this project.
+- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) this library inspired me to create this project.
```

### Comparing `silero_tts-0.0.1/pyproject.toml` & `silero_tts-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling","hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "silero-tts"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="daswer123", email="daswerq123@gmail.com" },
 ]
 description = "Script over the official Silero so that it can be conveniently and quickly used from the code or from the console"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `silero_tts-0.0.1/PKG-INFO` & `silero_tts-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: silero-tts
-Version: 0.0.1
+Version: 0.0.2
 Summary: Script over the official Silero so that it can be conveniently and quickly used from the code or from the console
 Project-URL: Homepage, https://github.com/daswer123/silero_cli
 Project-URL: Bug Tracker, https://github.com/daswer123/silero_cli/issues
 Author-email: daswer123 <daswerq123@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,16 +21,16 @@
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 # Silero TTS
 
 **README is available in the following languages:**
 
-[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README.md)
-[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.md)
+[![EN](https://img.shields.io/badge/EN-blue.svg)](https://github.com/daswer123/silero-tts-enhanced)
+[![RU](https://img.shields.io/badge/RU-red.svg)](https://github.com/daswer123/silero-tts-enhanced/blob/main/README_RU.MD)
 
 Silero TTS is a Python library that provides an easy way to synthesize speech from text using various Silero TTS models, languages, and speakers. It can be used as a standalone script or integrated into your own Python projects.
 
 ## Features
 
 - Support for multiple languages and models
 - Automatic downloading of the latest model configuration file
@@ -161,8 +161,8 @@
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
 
 ## Acknowledgements
 
 - [Silero Models](https://github.com/snakers4/silero-models) for providing the TTS models
-- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) this library inspired me to create this project.
+- [silero_tts_standalone](https://github.com/S-trace/silero_tts_standalone) this library inspired me to create this project.
```

