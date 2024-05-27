# Comparing `tmp/whisper-ctranslate2-0.4.3.tar.gz` & `tmp/whisper_ctranslate2-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.4.3.tar", last modified: Mon May  6 20:34:45 2024, max compression
+gzip compressed data, was "whisper_ctranslate2-0.4.4.tar", last modified: Mon May 27 14:26:56 2024, max compression
```

## Comparing `whisper-ctranslate2-0.4.3.tar` & `whisper_ctranslate2-0.4.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.4.3/LICENSE
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.3/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-05-04 18:06:24.000000 whisper-ctranslate2-0.4.3/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.064273 whisper-ctranslate2-0.4.3/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.065273 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    14799 2024-04-10 13:52:29.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/commandline.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3567 2024-04-07 16:26:12.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/diarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live_old.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6776 2024-05-06 20:17:31.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-04-07 16:42:56.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     8977 2024-02-23 21:46:59.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10210 2024-04-07 17:57:01.000000 whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.066273 whisper-ctranslate2-0.4.3/tests/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper-ctranslate2-0.4.3/tests/testdiarization.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper-ctranslate2-0.4.3/tests/testlive.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper-ctranslate2-0.4.3/tests/testwriters.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-06 20:34:45.067273 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/
--rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-05-06 20:34:45.000000 whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-27 14:26:56.403162 whisper_ctranslate2-0.4.4/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper_ctranslate2-0.4.4/LICENSE
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-27 14:26:56.403162 whisper_ctranslate2-0.4.4/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6047 2024-01-04 19:51:41.000000 whisper_ctranslate2-0.4.4/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2024-05-27 14:26:56.403162 whisper_ctranslate2-0.4.4/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1690 2024-05-04 18:06:24.000000 whisper_ctranslate2-0.4.4/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-27 14:26:56.401162 whisper_ctranslate2-0.4.4/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-27 14:26:56.402162 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    14799 2024-04-10 13:52:29.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/commandline.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3567 2024-04-07 16:26:12.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/diarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2892 2023-11-27 18:25:52.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5344 2024-01-15 16:02:59.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5343 2024-01-15 14:41:09.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/live_old.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6776 2024-05-06 20:17:31.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2024-05-06 20:36:08.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     9257 2024-05-27 14:22:56.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10210 2024-04-07 17:57:01.000000 whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-27 14:26:56.402162 whisper_ctranslate2-0.4.4/tests/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1977 2024-01-04 19:51:41.000000 whisper_ctranslate2-0.4.4/tests/testdiarization.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      638 2024-01-06 20:57:51.000000 whisper_ctranslate2-0.4.4/tests/testlive.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    11496 2024-02-21 19:27:42.000000 whisper_ctranslate2-0.4.4/tests/testwriters.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2024-05-27 14:26:56.403162 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/
+-rw-r--r--   0 jordi     (1000) jordi     (1000)     7148 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      698 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2024-05-27 14:26:56.000000 whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.4.3/LICENSE` & `whisper_ctranslate2-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/PKG-INFO` & `whisper_ctranslate2-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.3
+Version: 0.4.4
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.4.3/README.md` & `whisper_ctranslate2-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/setup.py` & `whisper_ctranslate2-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/commandline.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/commandline.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/diarization.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/diarization.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/languages.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/live.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/live_old.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/live_old.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/transcribe.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 8% similar despite different names*

```diff
@@ -220,38 +220,45 @@
     diarization_output = {}
     if diarization:
         diarization_output = get_diarization(audio, diarize_model, verbose)
 
     # We need to do first the diarization of all files because CTranslate2 and torch
     # use incompatible CUDA versions and once CTranslate2 is used torch will not work
     for audio_path in audio:
-        if verbose and len(audio) > 1:
-            print(f"\nFile: '{audio_path} ({task})'")
+        try:
+            if verbose and len(audio) > 1:
+                print(f"\nFile: '{audio_path} ({task})'")
+
+            start_time = datetime.datetime.now()
+            result = transcribe.inference(
+                audio_path,
+                task,
+                language,
+                verbose,
+                False,
+                options,
+            )
 
-        start_time = datetime.datetime.now()
-        result = transcribe.inference(
-            audio_path,
-            task,
-            language,
-            verbose,
-            False,
-            options,
-        )
-
-        if diarization:
-            if verbose:
-                print(
-                    f"Time used for transcription: {datetime.datetime.now() - start_time}"
+            if diarization:
+                if verbose:
+                    print(
+                        f"Time used for transcription: {datetime.datetime.now() - start_time}"
+                    )
+                result = diarize_model.assign_speakers_to_segments(
+                    diarization_output[audio_path], result, speaker_name
                 )
-            result = diarize_model.assign_speakers_to_segments(
-                diarization_output[audio_path], result, speaker_name
-            )
 
-        writer = get_writer(output_format, output_dir)
-        writer(result, audio_path, writer_args)
+            writer = get_writer(output_format, output_dir)
+            writer(result, audio_path, writer_args)
+
+        except Exception as e:
+            sys.stderr.write(
+                f"Error: unable to process file: {audio_path} with exception '{e}'\n"
+            )
+            continue
 
     if verbose:
         print(f"Transcription results written to '{output_dir}' directory")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `whisper-ctranslate2-0.4.3/src/whisper_ctranslate2/writers.py` & `whisper_ctranslate2-0.4.4/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/tests/testdiarization.py` & `whisper_ctranslate2-0.4.4/tests/testdiarization.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/tests/testlive.py` & `whisper_ctranslate2-0.4.4/tests/testlive.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/tests/testwriters.py` & `whisper_ctranslate2-0.4.4/tests/testwriters.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.4.3
+Version: 0.4.4
 Summary: Whisper command line client that uses CTranslate2 and faster-whisper
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.4.3/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper_ctranslate2-0.4.4/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

