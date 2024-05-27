# Comparing `tmp/datafog-3.2.1b3.tar.gz` & `tmp/datafog-3.2.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-3.2.1b3.tar", last modified: Sat May 18 21:13:33 2024, max compression
+gzip compressed data, was "datafog-3.2.1b4.tar", last modified: Mon May 27 19:25:19 2024, max compression
```

## Comparing `datafog-3.2.1b3.tar` & `datafog-3.2.1b4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.200146 datafog-3.2.1b3/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b3/LICENSE
--rw-r--r--   0 sidmohan   (501) staff       (20)     7962 2024-05-18 21:13:33.199989 datafog-3.2.1b3/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b3/README.md
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.192736 datafog-3.2.1b3/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b3/datafog/__about__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b3/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b3/datafog/config.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     3396 2024-05-18 21:01:49.000000 datafog-3.2.1b3/datafog/main.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.193708 datafog-3.2.1b3/datafog/processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b3/datafog/processing/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.194667 datafog-3.2.1b3/datafog/processing/image_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/image_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/image_processing/donut_processor.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/image_processing/image_downloader.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/image_processing/pytesseract_processor.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.195213 datafog-3.2.1b3/datafog/processing/spark_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b3/datafog/processing/spark_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b3/datafog/processing/spark_processing/pyspark_udfs.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.195702 datafog-3.2.1b3/datafog/processing/text_processing/
--rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/text_processing/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/processing/text_processing/spacy_pii_annotator.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.197971 datafog-3.2.1b3/datafog/services/
--rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b3/datafog/services/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b3/datafog/services/image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b3/datafog/services/spark_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b3/datafog/services/text_service.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.198543 datafog-3.2.1b3/datafog/telemetry/
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b3/datafog/telemetry/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     4434 2024-05-18 20:38:55.000000 datafog-3.2.1b3/datafog/telemetry/open_telemetry.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.193561 datafog-3.2.1b3/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     7962 2024-05-18 21:13:33.000000 datafog-3.2.1b3/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-18 21:13:33.000000 datafog-3.2.1b3/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-18 21:13:33.000000 datafog-3.2.1b3/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-18 21:13:33.000000 datafog-3.2.1b3/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-18 21:13:33.000000 datafog-3.2.1b3/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 21:13:33.200208 datafog-3.2.1b3/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-18 21:01:36.000000 datafog-3.2.1b3/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-18 21:13:33.199511 datafog-3.2.1b3/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b3/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b3/tests/test_image_service.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b3/tests/test_main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.214212 datafog-3.2.1b4/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1091 2024-05-18 18:25:55.000000 datafog-3.2.1b4/LICENSE
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:25:19.213889 datafog-3.2.1b4/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6738 2024-05-18 21:12:05.000000 datafog-3.2.1b4/README.md
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.209778 datafog-3.2.1b4/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2024-05-18 21:02:49.000000 datafog-3.2.1b4/datafog/__about__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      907 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      190 2024-05-18 19:53:32.000000 datafog-3.2.1b4/datafog/config.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3450 2024-05-27 19:24:27.000000 datafog-3.2.1b4/datafog/main.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.210920 datafog-3.2.1b4/datafog/processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      400 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/processing/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.211528 datafog-3.2.1b4/datafog/processing/image_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      146 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2872 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/donut_processor.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      787 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/image_downloader.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      297 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/image_processing/pytesseract_processor.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.211809 datafog-3.2.1b4/datafog/processing/spark_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      225 2024-05-18 19:53:34.000000 datafog-3.2.1b4/datafog/processing/spark_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2204 2024-05-18 21:08:15.000000 datafog-3.2.1b4/datafog/processing/spark_processing/pyspark_udfs.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212106 datafog-3.2.1b4/datafog/processing/text_processing/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       51 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/text_processing/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1300 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/processing/text_processing/spacy_pii_annotator.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212661 datafog-3.2.1b4/datafog/services/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      118 2024-05-18 18:25:55.000000 datafog-3.2.1b4/datafog/services/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1802 2024-05-18 21:08:15.000000 datafog-3.2.1b4/datafog/services/image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1030 2024-05-18 19:53:34.000000 datafog-3.2.1b4/datafog/services/spark_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      633 2024-05-18 21:08:14.000000 datafog-3.2.1b4/datafog/services/text_service.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.212952 datafog-3.2.1b4/datafog/telemetry/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-18 20:37:26.000000 datafog-3.2.1b4/datafog/telemetry/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2549 2024-05-27 19:21:35.000000 datafog-3.2.1b4/datafog/telemetry/open_telemetry.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.213576 datafog-3.2.1b4/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8252 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      972 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)      145 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2024-05-27 19:25:19.000000 datafog-3.2.1b4/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2024-05-27 19:25:19.214269 datafog-3.2.1b4/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1945 2024-05-27 19:05:19.000000 datafog-3.2.1b4/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2024-05-27 19:25:19.213376 datafog-3.2.1b4/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2024-05-18 18:25:55.000000 datafog-3.2.1b4/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2447 2024-05-18 18:25:55.000000 datafog-3.2.1b4/tests/test_image_service.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2785 2024-05-18 19:55:12.000000 datafog-3.2.1b4/tests/test_main.py
```

### Comparing `datafog-3.2.1b3/LICENSE` & `datafog-3.2.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/PKG-INFO` & `datafog-3.2.1b4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b3
+Version: 3.2.1b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: Requests==2.31.0
+Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast==0.0.0
+Requires-Dist: pydantic==1.10.15
+Requires-Dist: Pillow
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf
+Requires-Dist: pytesseract
+Requires-Dist: aiohttp
+Requires-Dist: pytest-asyncio
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -198,9 +208,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
+pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
+Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: pydantic==1.10.15 Requires-Dist:
+Pillow Requires-Dist: sentencepiece Requires-Dist: protobuf Requires-Dist:
+pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.1b3/README.md` & `datafog-3.2.1b4/README.md`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/__init__.py` & `datafog-3.2.1b4/datafog/__init__.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/main.py` & `datafog-3.2.1b4/datafog/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,17 @@
         spark_service=None,
         operations: List[OperationType] = [OperationType.ANNOTATE_PII],
     ):
         self.image_service = image_service
         self.text_service = text_service
         self.spark_service: SparkService = spark_service
         self.operations: List[OperationType] = operations
-        self.telemetry = Telemetry()
-        self.telemetry.set_tracer()
+        self._telemetry = Telemetry()
+        self._telemetry.set_tracer()
+        self._telemetry.datafog_creation("datafog")
 
     async def run_ocr_pipeline(self, image_urls: List[str]):
         """Run the OCR pipeline asynchronously."""
         extracted_text = await self.image_service.ocr_extract(image_urls)
         if OperationType.ANNOTATE_PII in self.operations:
             annotated_text = await self.text_service.batch_annotate_texts(
                 extracted_text
```

### Comparing `datafog-3.2.1b3/datafog/processing/image_processing/donut_processor.py` & `datafog-3.2.1b4/datafog/processing/image_processing/donut_processor.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/processing/image_processing/image_downloader.py` & `datafog-3.2.1b4/datafog/processing/image_processing/image_downloader.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/processing/spark_processing/pyspark_udfs.py` & `datafog-3.2.1b4/datafog/processing/spark_processing/pyspark_udfs.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/processing/text_processing/spacy_pii_annotator.py` & `datafog-3.2.1b4/datafog/processing/text_processing/spacy_pii_annotator.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/services/image_service.py` & `datafog-3.2.1b4/datafog/services/image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/services/spark_service.py` & `datafog-3.2.1b4/datafog/services/spark_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog/services/text_service.py` & `datafog-3.2.1b4/datafog/services/text_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/datafog.egg-info/PKG-INFO` & `datafog-3.2.1b4/datafog.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 3.2.1b3
+Version: 3.2.1b4
 Summary: Scan, redact, and manage PII in your documents before they get uploaded to a Retrieval Augmented Generation (RAG) system.
 Home-page: https://datafog.ai
 Author: Sid Mohan
 Author-email: sid@datafog.ai
 Maintainer: DataFog
 Maintainer-email: hi@datafog.ai
 License: MIT
 Project-URL: Homepage, https://datafog.ai
 Project-URL: Documentation, https://docs.datafog.ai
 Project-URL: Discord, https://discord.gg/bzDth394R4
 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python
 Keywords: pii,redaction,nlp,rag,retrieval augmented generation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: tox
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: Requests==2.31.0
+Requires-Dist: spacy==3.4.4
+Requires-Dist: en_spacy_pii_fast==0.0.0
+Requires-Dist: pydantic==1.10.15
+Requires-Dist: Pillow
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf
+Requires-Dist: pytesseract
+Requires-Dist: aiohttp
+Requires-Dist: pytest-asyncio
 
 <p align="center">
   <a href="https://www.datafog.ai"><img src="public/colorlogo.png" alt="DataFog logo"></a>
 </p>
 
 <p align="center">
     <b>Open-source DevSecOps for Generative AI Systems</b>. <br />
@@ -198,9 +208,7 @@
 
 ```
 
 ## License
 
 This software is published under the [MIT
 license](https://en.wikipedia.org/wiki/MIT_License).
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 2.1 Name: datafog Version: 3.2.1b3 Summary: Scan, redact, and
+Metadata-Version: 2.1 Name: datafog Version: 3.2.1b4 Summary: Scan, redact, and
 manage PII in your documents before they get uploaded to a Retrieval Augmented
 Generation (RAG) system. Home-page: https://datafog.ai Author: Sid Mohan
 Author-email: sid@datafog.ai Maintainer: DataFog Maintainer-email:
 hi@datafog.ai License: MIT Project-URL: Homepage, https://datafog.ai Project-
 URL: Documentation, https://docs.datafog.ai Project-URL: Discord, https://
 discord.gg/bzDth394R4 Project-URL: Twitter, https://twitter.com/datafoginc
 Project-URL: GitHub, https://github.com/datafog/datafog-python Keywords:
-pii,redaction,nlp,rag,retrieval augmented generation Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Framework :: tox
-Classifier: Framework :: Pytest Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research Classifier: Intended Audience
-:: Information Technology Classifier: Intended Audience :: System
-Administrators Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE
+pii,redaction,nlp,rag,retrieval augmented generation Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Framework :: tox Classifier: Framework :: Pytest
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Science/Research Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators Requires-Python: >=3.10
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+pandas Requires-Dist: Requests==2.31.0 Requires-Dist: spacy==3.4.4 Requires-
+Dist: en_spacy_pii_fast==0.0.0 Requires-Dist: pydantic==1.10.15 Requires-Dist:
+Pillow Requires-Dist: sentencepiece Requires-Dist: protobuf Requires-Dist:
+pytesseract Requires-Dist: aiohttp Requires-Dist: pytest-asyncio
                                 _[_D_a_t_a_F_o_g_ _l_o_g_o_]
                OOppeenn--ssoouurrccee DDeevvSSeeccOOppss ffoorr GGeenneerraattiivvee AAII SSyysstteemmss.
   _[_P_y_P_i_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _p_y_v_e_r_s_i_o_n_s_]_[_G_i_t_H_u_b_ _s_t_a_r_s_]_[_P_y_P_i_ _d_o_w_n_l_o_a_d_s_]_[_D_i_s_c_o_r_d_]_[_C_o_d_e
                      _s_t_y_l_e_:_ _b_l_a_c_k_]_[_c_o_d_e_c_o_v_]_[_G_i_t_H_u_b_ _I_s_s_u_e_s_]
 ## Overview ### What is DataFog? DataFog is an open-source DevSecOps platform
 that lets you scan and redact Personally Identifiable Information (PII) out of
 your Generative AI applications. ### Core Problem ![image](https://github.com/
```

### Comparing `datafog-3.2.1b3/datafog.egg-info/SOURCES.txt` & `datafog-3.2.1b4/datafog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/setup.py` & `datafog-3.2.1b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read README for the long description
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 def __version__():
-    return "3.2.1b3"
+    return "3.2.1b4"
 
 
 project_urls = {
     "Homepage": "https://datafog.ai",
     "Documentation": "https://docs.datafog.ai",
     "Discord": "https://discord.gg/bzDth394R4",
     "Twitter": "https://twitter.com/datafoginc",
```

### Comparing `datafog-3.2.1b3/tests/test_image_service.py` & `datafog-3.2.1b4/tests/test_image_service.py`

 * *Files identical despite different names*

### Comparing `datafog-3.2.1b3/tests/test_main.py` & `datafog-3.2.1b4/tests/test_main.py`

 * *Files identical despite different names*

