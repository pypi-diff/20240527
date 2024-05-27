# Comparing `tmp/wafl_llm-0.0.83-py3-none-any.whl.zip` & `tmp/wafl_llm-0.0.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,22 @@
-Zip file size: 9098 bytes, number of entries: 15
+Zip file size: 13984 bytes, number of entries: 20
 -rw-r--r--  2.0 unx        0 b- defN 23-Dec-26 12:22 wafl_llm/__init_.py
 -rw-r--r--  2.0 unx       36 b- defN 23-Dec-26 12:30 wafl_llm/__main__.py
--rw-r--r--  2.0 unx     2289 b- defN 24-May-11 08:37 wafl_llm/command_line.py
--rw-r--r--  2.0 unx      222 b- defN 24-May-11 09:09 wafl_llm/config.json
+-rw-r--r--  2.0 unx     2306 b- defN 24-May-25 09:21 wafl_llm/command_line.py
+-rw-r--r--  2.0 unx      222 b- defN 24-May-25 11:59 wafl_llm/config.json
 -rw-r--r--  2.0 unx       70 b- defN 23-Apr-05 20:00 wafl_llm/config.properties
--rw-r--r--  2.0 unx     2564 b- defN 24-May-11 10:50 wafl_llm/llm_handler.py
+-rw-r--r--  2.0 unx     3417 b- defN 24-May-25 11:58 wafl_llm/default_handler.py
+-rw-r--r--  2.0 unx     3443 b- defN 24-May-27 09:51 wafl_llm/llama3_handler.py
+-rw-r--r--  2.0 unx      562 b- defN 24-May-24 11:00 wafl_llm/llm_handler.py
+-rw-r--r--  2.0 unx      967 b- defN 24-May-25 11:58 wafl_llm/llm_handler_factory.py
+-rw-r--r--  2.0 unx     2848 b- defN 24-May-25 09:01 wafl_llm/mistral_handler.py
+-rw-r--r--  2.0 unx     3922 b- defN 24-May-27 09:52 wafl_llm/phi3_4k_handler.py
 -rw-r--r--  2.0 unx     1650 b- defN 23-Dec-27 12:11 wafl_llm/sentence_embedder_handler.py
 -rw-r--r--  2.0 unx     2415 b- defN 23-Dec-27 12:11 wafl_llm/speaker_handler.py
--rw-r--r--  2.0 unx       69 b- defN 24-May-11 11:16 wafl_llm/variables.py
--rw-r--r--  2.0 unx     4622 b- defN 24-May-11 09:31 wafl_llm/whisper_handler.py
--rw-r--r--  2.0 unx     2648 b- defN 24-May-11 11:22 wafl_llm-0.0.83.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-11 11:22 wafl_llm-0.0.83.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 24-May-11 11:22 wafl_llm-0.0.83.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-11 11:22 wafl_llm-0.0.83.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1206 b- defN 24-May-11 11:22 wafl_llm-0.0.83.dist-info/RECORD
-15 files, 17948 bytes uncompressed, 7092 bytes compressed:  60.5%
+-rw-r--r--  2.0 unx       69 b- defN 24-May-27 14:00 wafl_llm/variables.py
+-rw-r--r--  2.0 unx     4672 b- defN 24-May-24 11:02 wafl_llm/whisper_handler.py
+-rw-r--r--  2.0 unx     2445 b- defN 24-May-27 14:07 wafl_llm-0.0.90.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 14:07 wafl_llm-0.0.90.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 24-May-27 14:07 wafl_llm-0.0.90.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-27 14:07 wafl_llm-0.0.90.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1627 b- defN 24-May-27 14:07 wafl_llm-0.0.90.dist-info/RECORD
+20 files, 30828 bytes uncompressed, 11322 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -9,38 +9,53 @@
 
 Filename: wafl_llm/config.json
 Comment: 
 
 Filename: wafl_llm/config.properties
 Comment: 
 
+Filename: wafl_llm/default_handler.py
+Comment: 
+
+Filename: wafl_llm/llama3_handler.py
+Comment: 
+
 Filename: wafl_llm/llm_handler.py
 Comment: 
 
+Filename: wafl_llm/llm_handler_factory.py
+Comment: 
+
+Filename: wafl_llm/mistral_handler.py
+Comment: 
+
+Filename: wafl_llm/phi3_4k_handler.py
+Comment: 
+
 Filename: wafl_llm/sentence_embedder_handler.py
 Comment: 
 
 Filename: wafl_llm/speaker_handler.py
 Comment: 
 
 Filename: wafl_llm/variables.py
 Comment: 
 
 Filename: wafl_llm/whisper_handler.py
 Comment: 
 
-Filename: wafl_llm-0.0.83.dist-info/METADATA
+Filename: wafl_llm-0.0.90.dist-info/METADATA
 Comment: 
 
-Filename: wafl_llm-0.0.83.dist-info/WHEEL
+Filename: wafl_llm-0.0.90.dist-info/WHEEL
 Comment: 
 
-Filename: wafl_llm-0.0.83.dist-info/entry_points.txt
+Filename: wafl_llm-0.0.90.dist-info/entry_points.txt
 Comment: 
 
-Filename: wafl_llm-0.0.83.dist-info/top_level.txt
+Filename: wafl_llm-0.0.90.dist-info/top_level.txt
 Comment: 
 
-Filename: wafl_llm-0.0.83.dist-info/RECORD
+Filename: wafl_llm-0.0.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wafl_llm/command_line.py

```diff
@@ -34,15 +34,15 @@
 
     log_dir = f"{_running_path}/logs/"
     if os.path.exists(log_dir):
         print("Removing the prior logs/ directory.")
         shutil.rmtree(log_dir)
 
     config_path = f"{_path}/config.json"
-    if os.path.exists("config.json"):
+    if os.path.exists("config.json"):   #### load right config.json
         print("Found existing config.json in local directory.")
         config_path = f"{_running_path}/config.json"
 
     for service in services:
         if os.path.exists(f"models/{service}.mar"):
             continue
 
@@ -50,17 +50,15 @@
         os.system(
             f"torch-model-archiver --model-name '{service}' --version 0.0.1 "
             f"--handler {_path}/{service}_handler.py "
             f"--extra-files {config_path} "
             f"--export-path models/"
         )
 
-    os.system(
-        f"cp {_path}/config.properties ./config.properties"
-    )
+    os.system(f"cp {_path}/config.properties ./config.properties")
 
     os.system(
         "torchserve --start --model-store models "
         "--models "
         "bot=llm.mar "
         "speaker=speaker.mar "
         "whisper=whisper.mar "
@@ -92,8 +90,8 @@
 
     except RuntimeError as e:
         print(e)
         print("WAFL_LLM ended due to the exception above.")
 
 
 if __name__ == "__main__":
-    main()
+    main()
```

## wafl_llm/config.json

### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'llm_model'": "'fractalego/wafl-phi3-mini-4k'"}*

```diff
@@ -1,6 +1,6 @@
 {
-    "llm_model": "fractalego/wafl-mistral_v0.1",
+    "llm_model": "fractalego/wafl-phi3-mini-4k",
     "sentence_embedder_models": "TaylorAI/gte-tiny",
     "speaker_model": "facebook/fastspeech2-en-ljspeech",
     "whisper_model": "fractalego/personal-whisper-distilled-model"
 }
```

## wafl_llm/llm_handler.py

```diff
@@ -1,68 +1,16 @@
-import json
 import logging
 import os
-import torch
 
-from vllm import LLM, SamplingParams
-from ts.torch_handler.base_handler import BaseHandler
-from wafl_llm.variables import get_variables
+from wafl_llm.llm_handler_factory import LLMHandlerFactory
 
 _path = os.path.dirname(__file__)
 _logger = logging.getLogger(__file__)
 
-
-class ChatbotHandler(BaseHandler):
-    def __init__(self):
-        super().__init__()
-        self.initialized = False
-        _logger.info("The handler is created!")
-        self._config = json.load(open(os.path.join(_path, "config.json"), "r"))
-
-    def initialize(self, ctx):
-        self.manifest = ctx.manifest
-        model_name = self._config["llm_model"]
-        _logger.info(f"Loading the model {model_name}.")
-        self._llm = LLM(model=model_name, dtype="bfloat16")
-        _logger.info("Transformer model loaded successfully.")
-        self.initialized = True
-
-    def preprocess(self, data):
-        prompt = data[0].get("body").get("data")
-        temperature = data[0].get("body").get("temperature")
-        num_tokens = data[0].get("body").get("num_tokens")
-        last_strings = data[0].get("body").get("last_strings")
-        num_replicas = data[0].get("body").get("num_replicas")
-        return {
-            "prompt": prompt,
-            "temperature": temperature,
-            "num_tokens": num_tokens,
-            "last_strings": last_strings,
-            "num_replicas": num_replicas,
-        }
-
-    def inference(self, data):
-        with torch.no_grad():
-            prompt = data["prompt"]
-            temperature = data["temperature"]
-            num_tokens = data["num_tokens"]
-            last_strings = data["last_strings"]
-            num_replicas = data["num_replicas"]
-            prompts = [prompt] * num_replicas
-            sampling_params = SamplingParams(temperature=temperature, top_p=0.95, stop=last_strings, max_tokens=num_tokens)
-            outputs = self._llm.generate(
-                prompts, sampling_params
-            )
-            return "<||>".join(output.outputs[0].text for output in outputs)
-
-    def postprocess(self, inference_output):
-        return [json.dumps({"prediction": inference_output, "status": "success", "version": get_variables()["version"]})]
-
-
-_service = ChatbotHandler()
+_service = LLMHandlerFactory().get_llm_handler()
 
 
 def handle(data, context):
     try:
         if not _service.initialized:
             _service.initialize(context)
```

## wafl_llm/variables.py

```diff
@@ -1,4 +1,4 @@
 def get_variables():
     return {
-        "version": "0.0.83",
+        "version": "0.0.90",
     }
```

## wafl_llm/whisper_handler.py

```diff
@@ -27,15 +27,19 @@
         self.processor = WhisperProcessor.from_pretrained(model_name)
         self._starting_tokens = self.processor.tokenizer.convert_tokens_to_ids(
             ["<|startoftranscript|>", "<|notimestamps|>"]
         )
         self._ending_tokens = self.processor.tokenizer.convert_tokens_to_ids(
             ["<|endoftext|>"]
         )
-        self.model = BetterTransformer.transform(self.model, keep_original_model=True).cuda().half()
+        self.model = (
+            BetterTransformer.transform(self.model, keep_original_model=True)
+            .cuda()
+            .half()
+        )
         self.model = torch.compile(self.model)
         _logger.info("Whisper model loaded successfully.")
         self.initialized = True
 
     def preprocess(self, data):
         waveform = data[0].get("body").get("waveform")
         num_beams = data[0].get("body").get("num_beams")
```

## Comparing `wafl_llm-0.0.83.dist-info/METADATA` & `wafl_llm-0.0.90.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: wafl-llm
-Version: 0.0.83
+Version: 0.0.90
 Summary: A hybrid chatbot - LLM side.
 Home-page: http://github.com/fractalego/wafl_llm
 Author: Alberto Cetoli
 Author-email: alberto@fractalego.io
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 Requires-Dist: vllm (==0.4.2)
 Requires-Dist: torch (==2.3.0)
 Requires-Dist: flash-attn (==2.5.8)
-Requires-Dist: transformers (==4.40.0)
+Requires-Dist: transformers (==4.41.0)
 Requires-Dist: sentencepiece (==0.1.98)
 Requires-Dist: accelerate (==0.28.0)
 Requires-Dist: bitsandbytes (==0.41.3)
 Requires-Dist: optimum (==1.8.6)
 Requires-Dist: onnx (==1.13.0)
 Requires-Dist: datasets (==2.8.0)
 Requires-Dist: mpi4py (==3.1.4)
@@ -67,20 +67,14 @@
 }
 ```
 
 The models are downloaded from the HugggingFace repository. Any other compatible model should work.
 
 
 #### Docker
-A docker image can be used to run it as in the following:
-
-```bash
-$ docker run -p8080:8080 --env NVIDIA_DISABLE_REQUIRE=1 --gpus all fractalego/wafl-llm:latest
-```
-
-or one can clone this repository and run the following
+Run the following
 
 ```bash
 docker/build.sh
 docker run -p8080:8080 --env NVIDIA_DISABLE_REQUIRE=1 --gpus all wafl-llm
 ```
```

## Comparing `wafl_llm-0.0.83.dist-info/RECORD` & `wafl_llm-0.0.90.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 wafl_llm/__init_.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 wafl_llm/__main__.py,sha256=-GqoftNECZBtC8F82KWJrdSD05BcKBrrL0ElHEEUHyk,36
-wafl_llm/command_line.py,sha256=sYIipi9aJihHLbxs5xFlWDHVYAi4VUJ20aMcJOh48UQ,2289
-wafl_llm/config.json,sha256=uLx47gUedv9Qy2B40M4_hrwS2h5u3PtKAzUlgC1mQ34,222
+wafl_llm/command_line.py,sha256=MqTKHlNd098DmwBi-xBRRAn_4DUvUXvvdR1xaK72_M0,2306
+wafl_llm/config.json,sha256=jbRjDSTHbhFbFqhUB_8CnBlOnm5qECZMAJD2rjU8z2Y,222
 wafl_llm/config.properties,sha256=KPwiBH_SgU1owEfcNFfKiHfvy6o31WneCFxe1l4t8uM,70
-wafl_llm/llm_handler.py,sha256=F3Uhb5njxfrG9lcoQQB0jjdIloHXLNvo38CrwUptoCs,2564
+wafl_llm/default_handler.py,sha256=XK9-sOqcJzR97I5-8_gcgiwGnNTFiOV99AHQ1RC1Hss,3417
+wafl_llm/llama3_handler.py,sha256=TbA5zXEg3tl95mg72UzEccCAnJ16iiIObzaOnH62ys8,3443
+wafl_llm/llm_handler.py,sha256=CCHL2UYund43QocKEtXCNJWzgc9hgQgxQxK0FVC4py8,562
+wafl_llm/llm_handler_factory.py,sha256=QKGFh2wVnyT19Cu-iQmEogzeZnNLW4yPjTjJidujh3k,967
+wafl_llm/mistral_handler.py,sha256=kk5AMeJW1hpop1btCYPs0qiYsEI2_0-dxR7Un_HTr6I,2848
+wafl_llm/phi3_4k_handler.py,sha256=fCA60gSmbF45dFCnURxfPetKoc_4UBhitiDLk61bUFw,3922
 wafl_llm/sentence_embedder_handler.py,sha256=UBCDhulQV4sOu3dB5m7Q3tbNshBoxXXu6eryM-tBI5k,1650
 wafl_llm/speaker_handler.py,sha256=GPSe2vNN6zkqONdayMwH7Hrtw-GeDfzUFPwhTzyk8jo,2415
-wafl_llm/variables.py,sha256=zRIDWq2mgG02ZYOg8bLUK6Dtlg9LAOwJBWXjAYhFhbk,69
-wafl_llm/whisper_handler.py,sha256=XXEvgW4I0IBtsQ74eiR9g8ygdqVoH6eBucymSH7DzvY,4622
-wafl_llm-0.0.83.dist-info/METADATA,sha256=_hLfPBrI3FBJ5xH3HN2uZqrI3A-ZN0Rk8fdIAnqnIGE,2648
-wafl_llm-0.0.83.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-wafl_llm-0.0.83.dist-info/entry_points.txt,sha256=2aX6hSVH8cANvHV9aDNHY2s3ECFVNnndVE2H6Nl3mQo,56
-wafl_llm-0.0.83.dist-info/top_level.txt,sha256=SgJ63Mt3tPHkpirFUEJaxICtIav4HvK4i_vDc1q7E-M,9
-wafl_llm-0.0.83.dist-info/RECORD,,
+wafl_llm/variables.py,sha256=YXpplpwX0DeWmkfoaQMgppiKThpu3X2jwrjMRcX3V04,69
+wafl_llm/whisper_handler.py,sha256=UvYC3z2ldfJe8035ne80b7on-CfhX6k-v2yOOkEtZps,4672
+wafl_llm-0.0.90.dist-info/METADATA,sha256=V2Be_pQUVZPpgaz8WFcI03mxGtF0BX80F_H7aq2OoxY,2445
+wafl_llm-0.0.90.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+wafl_llm-0.0.90.dist-info/entry_points.txt,sha256=2aX6hSVH8cANvHV9aDNHY2s3ECFVNnndVE2H6Nl3mQo,56
+wafl_llm-0.0.90.dist-info/top_level.txt,sha256=SgJ63Mt3tPHkpirFUEJaxICtIav4HvK4i_vDc1q7E-M,9
+wafl_llm-0.0.90.dist-info/RECORD,,
```

