# Comparing `tmp/voicebox-tts-0.0.7.tar.gz` & `tmp/voicebox_tts-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-tts-0.0.7.tar", last modified: Thu Dec 28 19:00:59 2023, max compression
+gzip compressed data, was "voicebox_tts-0.0.8.tar", last modified: Mon May 27 08:12:19 2024, max compression
```

## Comparing `voicebox-tts-0.0.7.tar` & `voicebox_tts-0.0.8.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.414409 voicebox-tts-0.0.7/
--rw-rw-r--   0 austin    (1000) austin    (1000)     1069 2023-10-09 03:54:09.000000 voicebox-tts-0.0.7/LICENSE
--rw-r--r--   0 austin    (1000) austin    (1000)    10267 2023-12-28 19:00:59.414409 voicebox-tts-0.0.7/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)     6652 2023-12-28 18:42:23.000000 voicebox-tts-0.0.7/README.md
--rw-rw-r--   0 austin    (1000) austin    (1000)     2112 2023-12-28 18:57:19.000000 voicebox-tts-0.0.7/pyproject.toml
--rw-rw-r--   0 austin    (1000) austin    (1000)       38 2023-12-28 19:00:59.414409 voicebox-tts-0.0.7/setup.cfg
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.406408 voicebox-tts-0.0.7/src/
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.406408 voicebox-tts-0.0.7/src/voicebox/
--rw-rw-r--   0 austin    (1000) austin    (1000)      132 2023-12-28 18:53:19.000000 voicebox-tts-0.0.7/src/voicebox/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4485 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/__main__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2198 2023-12-22 05:30:01.000000 voicebox-tts-0.0.7/src/voicebox/audio.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.406408 voicebox-tts-0.0.7/src/voicebox/effects/
--rw-rw-r--   0 austin    (1000) austin    (1000)      608 2023-12-19 03:44:53.000000 voicebox-tts-0.0.7/src/voicebox/effects/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2299 2023-12-19 04:54:52.000000 voicebox-tts-0.0.7/src/voicebox/effects/chain.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      278 2023-12-19 04:21:09.000000 voicebox-tts-0.0.7/src/voicebox/effects/dc_offset.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1141 2023-12-19 05:32:27.000000 voicebox-tts-0.0.7/src/voicebox/effects/delay.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      519 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/effects/effect.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4185 2023-12-19 04:34:14.000000 voicebox-tts-0.0.7/src/voicebox/effects/eq.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2685 2023-12-22 05:27:07.000000 voicebox-tts-0.0.7/src/voicebox/effects/flanger.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1388 2023-12-19 04:45:50.000000 voicebox-tts-0.0.7/src/voicebox/effects/glitch.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1256 2023-12-19 04:51:38.000000 voicebox-tts-0.0.7/src/voicebox/effects/modulation.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      765 2023-12-19 04:53:06.000000 voicebox-tts-0.0.7/src/voicebox/effects/normalize.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1375 2023-12-19 04:54:52.000000 voicebox-tts-0.0.7/src/voicebox/effects/pedalboard.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      694 2023-12-19 03:11:41.000000 voicebox-tts-0.0.7/src/voicebox/effects/tail.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      188 2023-12-19 04:56:09.000000 voicebox-tts-0.0.7/src/voicebox/effects/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     6717 2023-12-22 05:27:07.000000 voicebox-tts-0.0.7/src/voicebox/effects/vocoder.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.406408 voicebox-tts-0.0.7/src/voicebox/examples/
--rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-10-17 01:14:20.000000 voicebox-tts-0.0.7/src/voicebox/examples/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1647 2023-12-28 18:47:35.000000 voicebox-tts-0.0.7/src/voicebox/examples/battle_droid.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1293 2023-12-28 18:49:50.000000 voicebox-tts-0.0.7/src/voicebox/examples/demo.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2208 2023-12-28 18:47:35.000000 voicebox-tts-0.0.7/src/voicebox/examples/glados.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1384 2023-12-28 18:47:35.000000 voicebox-tts-0.0.7/src/voicebox/examples/halo_spark.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.410408 voicebox-tts-0.0.7/src/voicebox/sinks/
--rw-rw-r--   0 austin    (1000) austin    (1000)      315 2023-12-22 05:11:06.000000 voicebox-tts-0.0.7/src/voicebox/sinks/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-20 01:46:44.000000 voicebox-tts-0.0.7/src/voicebox/sinks/distributor.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/sinks/sink.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1525 2023-12-20 02:01:04.000000 voicebox-tts-0.0.7/src/voicebox/sinks/sounddevice.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2614 2023-12-20 02:01:31.000000 voicebox-tts-0.0.7/src/voicebox/sinks/wavefile.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1066 2023-12-22 07:29:42.000000 voicebox-tts-0.0.7/src/voicebox/ssml.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.410408 voicebox-tts-0.0.7/src/voicebox/tts/
--rw-rw-r--   0 austin    (1000) austin    (1000)      675 2023-12-22 05:11:06.000000 voicebox-tts-0.0.7/src/voicebox/tts/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2463 2023-12-25 04:09:47.000000 voicebox-tts-0.0.7/src/voicebox/tts/amazonpolly.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     5698 2023-12-20 02:21:26.000000 voicebox-tts-0.0.7/src/voicebox/tts/cache.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1821 2023-12-22 05:45:11.000000 voicebox-tts-0.0.7/src/voicebox/tts/elevenlabs.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3024 2023-12-22 05:46:10.000000 voicebox-tts-0.0.7/src/voicebox/tts/espeakng.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1691 2023-12-22 05:48:06.000000 voicebox-tts-0.0.7/src/voicebox/tts/googlecloudtts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1183 2023-12-25 05:18:45.000000 voicebox-tts-0.0.7/src/voicebox/tts/gtts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1767 2023-12-22 05:59:17.000000 voicebox-tts-0.0.7/src/voicebox/tts/picotts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3513 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/tts/tts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2591 2023-12-22 05:09:28.000000 voicebox-tts-0.0.7/src/voicebox/tts/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      194 2023-11-18 03:18:52.000000 voicebox-tts-0.0.7/src/voicebox/types.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1383 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)       22 2023-12-28 18:53:19.000000 voicebox-tts-0.0.7/src/voicebox/version.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.410408 voicebox-tts-0.0.7/src/voicebox/voiceboxes/
--rw-rw-r--   0 austin    (1000) austin    (1000)      123 2023-12-28 18:37:25.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1684 2023-12-28 18:39:11.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/base.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     8219 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/parallel.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1587 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/queue.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1823 2023-12-28 18:39:11.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/simple.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3673 2023-12-28 18:32:50.000000 voicebox-tts-0.0.7/src/voicebox/voiceboxes/splitter.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.410408 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/
--rw-r--r--   0 austin    (1000) austin    (1000)    10267 2023-12-28 19:00:59.000000 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)     1693 2023-12-28 19:00:59.000000 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        1 2023-12-28 19:00:59.000000 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)      466 2023-12-28 19:00:59.000000 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/requires.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        9 2023-12-28 19:00:59.000000 voicebox-tts-0.0.7/src/voicebox_tts.egg-info/top_level.txt
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2023-12-28 19:00:59.410408 voicebox-tts-0.0.7/tests/
--rw-rw-r--   0 austin    (1000) austin    (1000)     2931 2023-12-22 05:27:48.000000 voicebox-tts-0.0.7/tests/test_audio.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      646 2023-11-12 19:59:26.000000 voicebox-tts-0.0.7/tests/test_ssml.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.233105 voicebox_tts-0.0.8/
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1069 2023-10-09 03:54:09.000000 voicebox_tts-0.0.8/LICENSE
+-rw-r--r--   0 austin    (1000) austin    (1000)    10058 2024-05-27 08:12:19.233105 voicebox_tts-0.0.8/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)     6443 2024-05-27 08:02:39.000000 voicebox_tts-0.0.8/README.md
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2112 2023-12-28 18:57:19.000000 voicebox_tts-0.0.8/pyproject.toml
+-rw-rw-r--   0 austin    (1000) austin    (1000)       38 2024-05-27 08:12:19.234105 voicebox_tts-0.0.8/setup.cfg
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.226105 voicebox_tts-0.0.8/src/
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.227105 voicebox_tts-0.0.8/src/voicebox/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      132 2023-12-28 18:53:19.000000 voicebox_tts-0.0.8/src/voicebox/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     4485 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/__main__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2198 2023-12-22 05:30:01.000000 voicebox_tts-0.0.8/src/voicebox/audio.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.228105 voicebox_tts-0.0.8/src/voicebox/effects/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      608 2023-12-19 03:44:53.000000 voicebox_tts-0.0.8/src/voicebox/effects/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2299 2023-12-19 04:54:52.000000 voicebox_tts-0.0.8/src/voicebox/effects/chain.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      278 2023-12-19 04:21:09.000000 voicebox_tts-0.0.8/src/voicebox/effects/dc_offset.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1141 2023-12-19 05:32:27.000000 voicebox_tts-0.0.8/src/voicebox/effects/delay.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      519 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/effects/effect.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     4185 2023-12-19 04:34:14.000000 voicebox_tts-0.0.8/src/voicebox/effects/eq.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2685 2023-12-22 05:27:07.000000 voicebox_tts-0.0.8/src/voicebox/effects/flanger.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1388 2023-12-19 04:45:50.000000 voicebox_tts-0.0.8/src/voicebox/effects/glitch.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1256 2023-12-19 04:51:38.000000 voicebox_tts-0.0.8/src/voicebox/effects/modulation.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      765 2023-12-19 04:53:06.000000 voicebox_tts-0.0.8/src/voicebox/effects/normalize.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1375 2023-12-19 04:54:52.000000 voicebox_tts-0.0.8/src/voicebox/effects/pedalboard.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      694 2023-12-19 03:11:41.000000 voicebox_tts-0.0.8/src/voicebox/effects/tail.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      188 2023-12-19 04:56:09.000000 voicebox_tts-0.0.8/src/voicebox/effects/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     6717 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/effects/vocoder.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.229105 voicebox_tts-0.0.8/src/voicebox/examples/
+-rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-10-17 01:14:20.000000 voicebox_tts-0.0.8/src/voicebox/examples/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1647 2023-12-28 18:47:35.000000 voicebox_tts-0.0.8/src/voicebox/examples/battle_droid.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1293 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/examples/demo.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2208 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/examples/glados.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1384 2023-12-28 18:47:35.000000 voicebox_tts-0.0.8/src/voicebox/examples/halo_spark.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.229105 voicebox_tts-0.0.8/src/voicebox/sinks/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      315 2023-12-22 05:11:06.000000 voicebox_tts-0.0.8/src/voicebox/sinks/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-20 01:46:44.000000 voicebox_tts-0.0.8/src/voicebox/sinks/distributor.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/sinks/sink.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1525 2023-12-20 02:01:04.000000 voicebox_tts-0.0.8/src/voicebox/sinks/sounddevice.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2614 2023-12-20 02:01:31.000000 voicebox_tts-0.0.8/src/voicebox/sinks/wavefile.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1066 2023-12-22 07:29:42.000000 voicebox_tts-0.0.8/src/voicebox/ssml.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.230105 voicebox_tts-0.0.8/src/voicebox/tts/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      678 2024-05-27 07:25:12.000000 voicebox_tts-0.0.8/src/voicebox/tts/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2463 2023-12-25 04:09:47.000000 voicebox_tts-0.0.8/src/voicebox/tts/amazonpolly.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     5698 2023-12-20 02:21:26.000000 voicebox_tts-0.0.8/src/voicebox/tts/cache.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2239 2024-05-27 08:07:41.000000 voicebox_tts-0.0.8/src/voicebox/tts/elevenlabs.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     3024 2023-12-22 05:46:10.000000 voicebox_tts-0.0.8/src/voicebox/tts/espeakng.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1691 2023-12-22 05:48:06.000000 voicebox_tts-0.0.8/src/voicebox/tts/googlecloudtts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1183 2023-12-25 05:18:45.000000 voicebox_tts-0.0.8/src/voicebox/tts/gtts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1767 2023-12-22 05:59:17.000000 voicebox_tts-0.0.8/src/voicebox/tts/picotts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     3513 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/tts/tts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2605 2024-05-27 08:06:38.000000 voicebox_tts-0.0.8/src/voicebox/tts/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      194 2023-11-18 03:18:52.000000 voicebox_tts-0.0.8/src/voicebox/types.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1383 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)       22 2024-05-27 08:10:52.000000 voicebox_tts-0.0.8/src/voicebox/version.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.230105 voicebox_tts-0.0.8/src/voicebox/voiceboxes/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      123 2023-12-28 18:37:25.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1684 2023-12-28 18:39:11.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/base.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     8219 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/parallel.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1587 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/queue.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1823 2023-12-28 18:39:11.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/simple.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     3673 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/splitter.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.231105 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/
+-rw-r--r--   0 austin    (1000) austin    (1000)    10058 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1693 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        1 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)      466 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/requires.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        9 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/top_level.txt
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.231105 voicebox_tts-0.0.8/tests/
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2931 2023-12-22 05:27:48.000000 voicebox_tts-0.0.8/tests/test_audio.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      646 2023-11-12 19:59:26.000000 voicebox_tts-0.0.8/tests/test_ssml.py
```

### Comparing `voicebox-tts-0.0.7/LICENSE` & `voicebox_tts-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/PKG-INFO` & `voicebox_tts-0.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-tts
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 Author-email: Austin Bowen <austin.bowen.314@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Austin Bowen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -85,15 +85,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/voicebox-tts)](https://pypi.org/project/voicebox-tts/)
 [![Documentation Status](https://readthedocs.org/projects/voicebox/badge/?version=latest)](https://voicebox.readthedocs.io/en/latest/?badge=latest)
 
 Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 
 | [GitHub](https://github.com/austin-bowen/voicebox/)
 | [Documentation 📘](https://voicebox.readthedocs.io)
-| [Audio Samples 🔉](https://voicebox.readthedocs.io/en/stable/samples.html)
+| [Audio Samples 🔉](samples)
 |
 
 ```python
 # Example: Use gTTS with a vocoder effect to speak in a robotic voice
 
 from voicebox import SimpleVoicebox
 from voicebox.tts import gTTS
@@ -113,90 +113,92 @@
 2. Install the `PortAudio` library for audio playback.
    - On Debian/Ubuntu: `sudo apt install libportaudio2`
 3. Install dependencies for whichever TTS engine(s) you want to use (see section below).
 
 ## Supported Text-to-Speech Engines
 
 Classes for supported TTS engines are located in the
-[`voicebox.tts.*`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts) modules.
+[`voicebox.tts`](voicebox.tts) package.
 
 ### Amazon Polly [🌐](https://aws.amazon.com/polly/)
 
 Online TTS engine from AWS.
 
-- Class: [`voicebox.tts.AmazonPolly`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/amazonpolly.py)
+- Class: [`voicebox.tts.AmazonPolly`](voicebox.tts.amazonpolly.AmazonPolly)
 - Setup: `pip install "voicebox-tts[amazon-polly]"`
 
 ### ElevenLabs [🌐](https://elevenlabs.io/)
 
 Online TTS engine with very realistic voices and support for voice cloning.
 
-- Class: [`voicebox.tts.ElevenLabs`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/elevenlabs.py)
+- Class: [`voicebox.tts.ElevenLabsTTS`](voicebox.tts.elevenlabs.ElevenLabsTTS)
 - Setup:
   1. `pip install "voicebox-tts[elevenlabs]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
-  3. Get an [API key](https://elevenlabs.io/docs/api-reference/authentication)
-     and do one of the following:
-     - Set environment variable `ELEVEN_API_KEY=<api-key>`; or
-     - Set with `import elevenlabs; elevenlabs.set_api_key('<api_key>')`; or
-     - Pass as parameter to class: `voicebox.tts.ElevenLabs(api_key='<api_key>')`
+  3. (Optional) Use an [API key](https://elevenlabs.io/docs/api-reference/authentication):
+     ```python
+     from elevenlabs.client import ElevenLabs
+     from voicebox.tts import ElevenLabsTTS
+
+     tts = ElevenLabsTTS(client=ElevenLabs(api_key='your-api-key'))
+     ```
 
 ### eSpeak NG [🌐](https://github.com/espeak-ng/espeak-ng)
 
 Offline TTS engine with a good number of options.
 
-- Class: [`voicebox.tts.ESpeakNG`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/espeakng.py)
+- Class: [`voicebox.tts.ESpeakNG`](voicebox.tts.espeakng.ESpeakNG)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install espeak-ng`
 
 ### Google Cloud Text-to-Speech [🌐](https://cloud.google.com/text-to-speech)
 
 Powerful online TTS engine offered by Google Cloud.
 
-- Class: [`voicebox.tts.GoogleCloudTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/googlecloudtts.py)
+- Class: [`voicebox.tts.GoogleCloudTTS`](voicebox.tts.googlecloudtts.GoogleCloudTTS)
 - Setup: `pip install "voicebox-tts[google-cloud-tts]"`
 
 ### gTTS [🌐](https://github.com/pndurette/gTTS)
 
 Online TTS engine used by Google Translate.
 
-- Class: [`voicebox.tts.gTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/gtts.py)
+- Class: [`voicebox.tts.gTTS`](voicebox.tts.gtts.gTTS)
 - Setup:
   1. `pip install "voicebox-tts[gtts]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
 
 ### Pico TTS
 
 Very basic offline TTS engine.
 
-- Class: [`voicebox.tts.PicoTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/picotts.py)
+- Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
 ## Effects
 
-Built-in effect classes are located in the [`voicebox.effects`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects) module,
+Built-in effect classes are located in the
+[`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
 from voicebox.effects import CoolEffect
 ```
 
 Here is a non-exhaustive list of fun effects:
-- [`Glitch`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/glitch.py)
+- [`Glitch`](voicebox.effects.glitch.Glitch)
   creates a glitchy sound by randomly repeating small chunks of audio.
-- [`RingMod`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/modulation.py)
+- [`RingMod`](voicebox.effects.modulation.RingMod)
   can be used to create choppy, Doctor Who Dalek-like effects.
-- [`Vocoder`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/vocoder.py)
+- [`Vocoder`](voicebox.effects.vocoder.Vocoder)
   is useful for making monotone, robotic voices.
 
 There is also support for all the awesome audio plugins in
 [Spotify's `pedalboard` library](https://spotify.github.io/pedalboard/index.html)
-using the special
-[`PedalboardEffect`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/pedalboard.py)
+using the special [`PedalboardEffect`](voicebox.effects.pedalboard.PedalboardEffect)
 wrapper, e.g.:
 
 ```python
 from voicebox import SimpleVoicebox
 from voicebox.effects import PedalboardEffect
 import pedalboard
 
@@ -218,57 +220,78 @@
 
 voicebox = SimpleVoicebox()
 voicebox.say('Hello, world!')
 ```
 
 ### Pre-built
 
-Some pre-built voiceboxes are available in the [`voicebox.examples`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/examples) package.
+Some pre-built voiceboxes are available in the
+[`voicebox.examples`](voicebox.examples) package.
 They can be imported into your own code, and you can run them to demo:
 
 ```bash
 # Voice of GLaDOS from the Portal video game series
 python -m voicebox.examples.glados "optional message"
 
 # Voice of the OOM-9 command battle droid from Star Wars: Episode I
 python -m voicebox.examples.battle_droid "optional message"
 ```
 
 ### Advanced
 
 ```python
 # Use eSpeak NG at 120 WPM and en-us voice as the TTS engine
-from voicebox.tts import ESpeakConfig, ESpeakNG
+from voicebox import reliable_tts
+from voicebox.tts import ESpeakConfig, ESpeakNG, gTTS
 
-tts = ESpeakNG(ESpeakConfig(speed=120, voice='en-us'))
+# Wrap multiple TTSs in retries and caches
+tts = reliable_tts(
+    ttss=[
+        # Prefer using online TTS first
+        gTTS(),
+        # Fall back to offline TTS if online TTS fails
+        ESpeakNG(ESpeakConfig(speed=120, voice='en-us')),
+    ],
+)
 
 # Add some voice effects
 from voicebox.effects import Vocoder, Glitch, Normalize
 
 effects = [
-    Vocoder.build(),  # Makes a very robotic, monotone voice
-    Glitch(),  # Randomly repeats small sections of audio
-    Normalize(),  # Remove DC and make volume consistent
+    Vocoder.build(),    # Make a robotic, monotone voice
+    Glitch(),           # Randomly repeat small sections of audio
+    Normalize(),        # Remove DC and make volume consistent
 ]
 
-# Send audio to playback device, and save to speech.wav file
+# Build audio sink
 from voicebox.sinks import Distributor, SoundDevice, WaveFile
 
 sink = Distributor([
-    SoundDevice(),
-    WaveFile('speech.wav'),
+    SoundDevice(),          # Send audio to playback device
+    WaveFile('speech.wav'), # Save audio to speech.wav file
 ])
 
 # Build the voicebox
-from voicebox import SimpleVoicebox
+from voicebox import ParallelVoicebox
+from voicebox.voiceboxes.splitter import SimpleSentenceSplitter
 
-voicebox = SimpleVoicebox(tts, effects, sink)
+# Parallel voicebox doesn't block the main thread
+voicebox = ParallelVoicebox(
+    tts,
+    effects,
+    sink,
+    # Split text into sentences to reduce time to first speech
+    text_splitter=SimpleSentenceSplitter(),
+)
 
-# eSpeak NG is used to say "Hello, world!" with a glitchy robot voice
+# Speak!
 voicebox.say('Hello, world!')
+
+# Wait for all audio to finish playing before exiting
+voicebox.wait_until_done()
 ```
 
 ### Command Line Demo
 
 ```bash
 python -m voicebox -h               # Print command help
 python -m voicebox "Hello, world!"  # Basic usage
```

### Comparing `voicebox-tts-0.0.7/README.md` & `voicebox_tts-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/voicebox-tts)](https://pypi.org/project/voicebox-tts/)
 [![Documentation Status](https://readthedocs.org/projects/voicebox/badge/?version=latest)](https://voicebox.readthedocs.io/en/latest/?badge=latest)
 
 Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 
 | [GitHub](https://github.com/austin-bowen/voicebox/)
 | [Documentation 📘](https://voicebox.readthedocs.io)
-| [Audio Samples 🔉](https://voicebox.readthedocs.io/en/stable/samples.html)
+| [Audio Samples 🔉](samples)
 |
 
 ```python
 # Example: Use gTTS with a vocoder effect to speak in a robotic voice
 
 from voicebox import SimpleVoicebox
 from voicebox.tts import gTTS
@@ -33,90 +33,92 @@
 2. Install the `PortAudio` library for audio playback.
    - On Debian/Ubuntu: `sudo apt install libportaudio2`
 3. Install dependencies for whichever TTS engine(s) you want to use (see section below).
 
 ## Supported Text-to-Speech Engines
 
 Classes for supported TTS engines are located in the
-[`voicebox.tts.*`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts) modules.
+[`voicebox.tts`](voicebox.tts) package.
 
 ### Amazon Polly [🌐](https://aws.amazon.com/polly/)
 
 Online TTS engine from AWS.
 
-- Class: [`voicebox.tts.AmazonPolly`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/amazonpolly.py)
+- Class: [`voicebox.tts.AmazonPolly`](voicebox.tts.amazonpolly.AmazonPolly)
 - Setup: `pip install "voicebox-tts[amazon-polly]"`
 
 ### ElevenLabs [🌐](https://elevenlabs.io/)
 
 Online TTS engine with very realistic voices and support for voice cloning.
 
-- Class: [`voicebox.tts.ElevenLabs`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/elevenlabs.py)
+- Class: [`voicebox.tts.ElevenLabsTTS`](voicebox.tts.elevenlabs.ElevenLabsTTS)
 - Setup:
   1. `pip install "voicebox-tts[elevenlabs]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
-  3. Get an [API key](https://elevenlabs.io/docs/api-reference/authentication)
-     and do one of the following:
-     - Set environment variable `ELEVEN_API_KEY=<api-key>`; or
-     - Set with `import elevenlabs; elevenlabs.set_api_key('<api_key>')`; or
-     - Pass as parameter to class: `voicebox.tts.ElevenLabs(api_key='<api_key>')`
+  3. (Optional) Use an [API key](https://elevenlabs.io/docs/api-reference/authentication):
+     ```python
+     from elevenlabs.client import ElevenLabs
+     from voicebox.tts import ElevenLabsTTS
+
+     tts = ElevenLabsTTS(client=ElevenLabs(api_key='your-api-key'))
+     ```
 
 ### eSpeak NG [🌐](https://github.com/espeak-ng/espeak-ng)
 
 Offline TTS engine with a good number of options.
 
-- Class: [`voicebox.tts.ESpeakNG`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/espeakng.py)
+- Class: [`voicebox.tts.ESpeakNG`](voicebox.tts.espeakng.ESpeakNG)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install espeak-ng`
 
 ### Google Cloud Text-to-Speech [🌐](https://cloud.google.com/text-to-speech)
 
 Powerful online TTS engine offered by Google Cloud.
 
-- Class: [`voicebox.tts.GoogleCloudTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/googlecloudtts.py)
+- Class: [`voicebox.tts.GoogleCloudTTS`](voicebox.tts.googlecloudtts.GoogleCloudTTS)
 - Setup: `pip install "voicebox-tts[google-cloud-tts]"`
 
 ### gTTS [🌐](https://github.com/pndurette/gTTS)
 
 Online TTS engine used by Google Translate.
 
-- Class: [`voicebox.tts.gTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/gtts.py)
+- Class: [`voicebox.tts.gTTS`](voicebox.tts.gtts.gTTS)
 - Setup:
   1. `pip install "voicebox-tts[gtts]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
 
 ### Pico TTS
 
 Very basic offline TTS engine.
 
-- Class: [`voicebox.tts.PicoTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/picotts.py)
+- Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
 ## Effects
 
-Built-in effect classes are located in the [`voicebox.effects`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects) module,
+Built-in effect classes are located in the
+[`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
 from voicebox.effects import CoolEffect
 ```
 
 Here is a non-exhaustive list of fun effects:
-- [`Glitch`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/glitch.py)
+- [`Glitch`](voicebox.effects.glitch.Glitch)
   creates a glitchy sound by randomly repeating small chunks of audio.
-- [`RingMod`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/modulation.py)
+- [`RingMod`](voicebox.effects.modulation.RingMod)
   can be used to create choppy, Doctor Who Dalek-like effects.
-- [`Vocoder`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/vocoder.py)
+- [`Vocoder`](voicebox.effects.vocoder.Vocoder)
   is useful for making monotone, robotic voices.
 
 There is also support for all the awesome audio plugins in
 [Spotify's `pedalboard` library](https://spotify.github.io/pedalboard/index.html)
-using the special
-[`PedalboardEffect`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/pedalboard.py)
+using the special [`PedalboardEffect`](voicebox.effects.pedalboard.PedalboardEffect)
 wrapper, e.g.:
 
 ```python
 from voicebox import SimpleVoicebox
 from voicebox.effects import PedalboardEffect
 import pedalboard
 
@@ -138,57 +140,78 @@
 
 voicebox = SimpleVoicebox()
 voicebox.say('Hello, world!')
 ```
 
 ### Pre-built
 
-Some pre-built voiceboxes are available in the [`voicebox.examples`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/examples) package.
+Some pre-built voiceboxes are available in the
+[`voicebox.examples`](voicebox.examples) package.
 They can be imported into your own code, and you can run them to demo:
 
 ```bash
 # Voice of GLaDOS from the Portal video game series
 python -m voicebox.examples.glados "optional message"
 
 # Voice of the OOM-9 command battle droid from Star Wars: Episode I
 python -m voicebox.examples.battle_droid "optional message"
 ```
 
 ### Advanced
 
 ```python
 # Use eSpeak NG at 120 WPM and en-us voice as the TTS engine
-from voicebox.tts import ESpeakConfig, ESpeakNG
+from voicebox import reliable_tts
+from voicebox.tts import ESpeakConfig, ESpeakNG, gTTS
 
-tts = ESpeakNG(ESpeakConfig(speed=120, voice='en-us'))
+# Wrap multiple TTSs in retries and caches
+tts = reliable_tts(
+    ttss=[
+        # Prefer using online TTS first
+        gTTS(),
+        # Fall back to offline TTS if online TTS fails
+        ESpeakNG(ESpeakConfig(speed=120, voice='en-us')),
+    ],
+)
 
 # Add some voice effects
 from voicebox.effects import Vocoder, Glitch, Normalize
 
 effects = [
-    Vocoder.build(),  # Makes a very robotic, monotone voice
-    Glitch(),  # Randomly repeats small sections of audio
-    Normalize(),  # Remove DC and make volume consistent
+    Vocoder.build(),    # Make a robotic, monotone voice
+    Glitch(),           # Randomly repeat small sections of audio
+    Normalize(),        # Remove DC and make volume consistent
 ]
 
-# Send audio to playback device, and save to speech.wav file
+# Build audio sink
 from voicebox.sinks import Distributor, SoundDevice, WaveFile
 
 sink = Distributor([
-    SoundDevice(),
-    WaveFile('speech.wav'),
+    SoundDevice(),          # Send audio to playback device
+    WaveFile('speech.wav'), # Save audio to speech.wav file
 ])
 
 # Build the voicebox
-from voicebox import SimpleVoicebox
+from voicebox import ParallelVoicebox
+from voicebox.voiceboxes.splitter import SimpleSentenceSplitter
 
-voicebox = SimpleVoicebox(tts, effects, sink)
+# Parallel voicebox doesn't block the main thread
+voicebox = ParallelVoicebox(
+    tts,
+    effects,
+    sink,
+    # Split text into sentences to reduce time to first speech
+    text_splitter=SimpleSentenceSplitter(),
+)
 
-# eSpeak NG is used to say "Hello, world!" with a glitchy robot voice
+# Speak!
 voicebox.say('Hello, world!')
+
+# Wait for all audio to finish playing before exiting
+voicebox.wait_until_done()
 ```
 
 ### Command Line Demo
 
 ```bash
 python -m voicebox -h               # Print command help
 python -m voicebox "Hello, world!"  # Basic usage
```

### Comparing `voicebox-tts-0.0.7/pyproject.toml` & `voicebox_tts-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/__main__.py` & `voicebox_tts-0.0.8/src/voicebox/__main__.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/audio.py` & `voicebox_tts-0.0.8/src/voicebox/audio.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/__init__.py` & `voicebox_tts-0.0.8/src/voicebox/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/chain.py` & `voicebox_tts-0.0.8/src/voicebox/effects/chain.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/delay.py` & `voicebox_tts-0.0.8/src/voicebox/effects/delay.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/effect.py` & `voicebox_tts-0.0.8/src/voicebox/effects/effect.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/eq.py` & `voicebox_tts-0.0.8/src/voicebox/effects/eq.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/flanger.py` & `voicebox_tts-0.0.8/src/voicebox/effects/flanger.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/glitch.py` & `voicebox_tts-0.0.8/src/voicebox/effects/glitch.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/modulation.py` & `voicebox_tts-0.0.8/src/voicebox/effects/modulation.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/normalize.py` & `voicebox_tts-0.0.8/src/voicebox/effects/normalize.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/pedalboard.py` & `voicebox_tts-0.0.8/src/voicebox/effects/pedalboard.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/tail.py` & `voicebox_tts-0.0.8/src/voicebox/effects/tail.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/effects/vocoder.py` & `voicebox_tts-0.0.8/src/voicebox/effects/vocoder.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/examples/battle_droid.py` & `voicebox_tts-0.0.8/src/voicebox/examples/battle_droid.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/examples/demo.py` & `voicebox_tts-0.0.8/src/voicebox/examples/demo.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/examples/glados.py` & `voicebox_tts-0.0.8/src/voicebox/examples/glados.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/examples/halo_spark.py` & `voicebox_tts-0.0.8/src/voicebox/examples/halo_spark.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/sinks/sounddevice.py` & `voicebox_tts-0.0.8/src/voicebox/sinks/sounddevice.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/sinks/wavefile.py` & `voicebox_tts-0.0.8/src/voicebox/sinks/wavefile.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/ssml.py` & `voicebox_tts-0.0.8/src/voicebox/ssml.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/__init__.py` & `voicebox_tts-0.0.8/src/voicebox/tts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except ImportError:
     pass
 
 from voicebox.tts.cache import CachedTTS, PrerecordedTTS
 from voicebox.tts.espeakng import ESpeakConfig, ESpeakNG
 
 try:
-    from voicebox.tts.elevenlabs import ElevenLabs
+    from voicebox.tts.elevenlabs import ElevenLabsTTS
 except ImportError:
     pass
 
 try:
     from voicebox.tts.googlecloudtts import GoogleCloudTTS
 except ImportError:
     pass
```

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/amazonpolly.py` & `voicebox_tts-0.0.8/src/voicebox/tts/amazonpolly.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/cache.py` & `voicebox_tts-0.0.8/src/voicebox/tts/cache.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/espeakng.py` & `voicebox_tts-0.0.8/src/voicebox/tts/espeakng.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/googlecloudtts.py` & `voicebox_tts-0.0.8/src/voicebox/tts/googlecloudtts.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/gtts.py` & `voicebox_tts-0.0.8/src/voicebox/tts/gtts.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/picotts.py` & `voicebox_tts-0.0.8/src/voicebox/tts/picotts.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/tts.py` & `voicebox_tts-0.0.8/src/voicebox/tts/tts.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/tts/utils.py` & `voicebox_tts-0.0.8/src/voicebox/tts/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,13 +82,15 @@
 
     dtype = sample_width_to_dtype[bytes_per_sample]
     samples = np.frombuffer(sample_bytes, dtype=dtype)
 
     return get_audio_from_samples(samples, sample_rate)
 
 
-def add_optional_items(d: dict, items: Iterable[Tuple[K, Optional[V]]]) -> None:
+def add_optional_items(d: dict, items: Iterable[Tuple[K, Optional[V]]]) -> dict:
     """Adds items with non-null values to the given dict."""
 
     for k, v in items:
         if v is not None:
             d[k] = v
+
+    return d
```

### Comparing `voicebox-tts-0.0.7/src/voicebox/utils.py` & `voicebox_tts-0.0.8/src/voicebox/utils.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/voiceboxes/base.py` & `voicebox_tts-0.0.8/src/voicebox/voiceboxes/base.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/voiceboxes/parallel.py` & `voicebox_tts-0.0.8/src/voicebox/voiceboxes/parallel.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/voiceboxes/queue.py` & `voicebox_tts-0.0.8/src/voicebox/voiceboxes/queue.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/voiceboxes/simple.py` & `voicebox_tts-0.0.8/src/voicebox/voiceboxes/simple.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox/voiceboxes/splitter.py` & `voicebox_tts-0.0.8/src/voicebox/voiceboxes/splitter.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/src/voicebox_tts.egg-info/PKG-INFO` & `voicebox_tts-0.0.8/src/voicebox_tts.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-tts
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 Author-email: Austin Bowen <austin.bowen.314@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Austin Bowen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -85,15 +85,15 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/voicebox-tts)](https://pypi.org/project/voicebox-tts/)
 [![Documentation Status](https://readthedocs.org/projects/voicebox/badge/?version=latest)](https://voicebox.readthedocs.io/en/latest/?badge=latest)
 
 Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 
 | [GitHub](https://github.com/austin-bowen/voicebox/)
 | [Documentation 📘](https://voicebox.readthedocs.io)
-| [Audio Samples 🔉](https://voicebox.readthedocs.io/en/stable/samples.html)
+| [Audio Samples 🔉](samples)
 |
 
 ```python
 # Example: Use gTTS with a vocoder effect to speak in a robotic voice
 
 from voicebox import SimpleVoicebox
 from voicebox.tts import gTTS
@@ -113,90 +113,92 @@
 2. Install the `PortAudio` library for audio playback.
    - On Debian/Ubuntu: `sudo apt install libportaudio2`
 3. Install dependencies for whichever TTS engine(s) you want to use (see section below).
 
 ## Supported Text-to-Speech Engines
 
 Classes for supported TTS engines are located in the
-[`voicebox.tts.*`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts) modules.
+[`voicebox.tts`](voicebox.tts) package.
 
 ### Amazon Polly [🌐](https://aws.amazon.com/polly/)
 
 Online TTS engine from AWS.
 
-- Class: [`voicebox.tts.AmazonPolly`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/amazonpolly.py)
+- Class: [`voicebox.tts.AmazonPolly`](voicebox.tts.amazonpolly.AmazonPolly)
 - Setup: `pip install "voicebox-tts[amazon-polly]"`
 
 ### ElevenLabs [🌐](https://elevenlabs.io/)
 
 Online TTS engine with very realistic voices and support for voice cloning.
 
-- Class: [`voicebox.tts.ElevenLabs`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/elevenlabs.py)
+- Class: [`voicebox.tts.ElevenLabsTTS`](voicebox.tts.elevenlabs.ElevenLabsTTS)
 - Setup:
   1. `pip install "voicebox-tts[elevenlabs]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
-  3. Get an [API key](https://elevenlabs.io/docs/api-reference/authentication)
-     and do one of the following:
-     - Set environment variable `ELEVEN_API_KEY=<api-key>`; or
-     - Set with `import elevenlabs; elevenlabs.set_api_key('<api_key>')`; or
-     - Pass as parameter to class: `voicebox.tts.ElevenLabs(api_key='<api_key>')`
+  3. (Optional) Use an [API key](https://elevenlabs.io/docs/api-reference/authentication):
+     ```python
+     from elevenlabs.client import ElevenLabs
+     from voicebox.tts import ElevenLabsTTS
+
+     tts = ElevenLabsTTS(client=ElevenLabs(api_key='your-api-key'))
+     ```
 
 ### eSpeak NG [🌐](https://github.com/espeak-ng/espeak-ng)
 
 Offline TTS engine with a good number of options.
 
-- Class: [`voicebox.tts.ESpeakNG`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/espeakng.py)
+- Class: [`voicebox.tts.ESpeakNG`](voicebox.tts.espeakng.ESpeakNG)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install espeak-ng`
 
 ### Google Cloud Text-to-Speech [🌐](https://cloud.google.com/text-to-speech)
 
 Powerful online TTS engine offered by Google Cloud.
 
-- Class: [`voicebox.tts.GoogleCloudTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/googlecloudtts.py)
+- Class: [`voicebox.tts.GoogleCloudTTS`](voicebox.tts.googlecloudtts.GoogleCloudTTS)
 - Setup: `pip install "voicebox-tts[google-cloud-tts]"`
 
 ### gTTS [🌐](https://github.com/pndurette/gTTS)
 
 Online TTS engine used by Google Translate.
 
-- Class: [`voicebox.tts.gTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/gtts.py)
+- Class: [`voicebox.tts.gTTS`](voicebox.tts.gtts.gTTS)
 - Setup:
   1. `pip install "voicebox-tts[gtts]"`
   2. Install ffmpeg or libav for `pydub` ([docs](https://github.com/jiaaro/pydub#getting-ffmpeg-set-up))
 
 ### Pico TTS
 
 Very basic offline TTS engine.
 
-- Class: [`voicebox.tts.PicoTTS`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/tts/picotts.py)
+- Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
 ## Effects
 
-Built-in effect classes are located in the [`voicebox.effects`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects) module,
+Built-in effect classes are located in the
+[`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
 from voicebox.effects import CoolEffect
 ```
 
 Here is a non-exhaustive list of fun effects:
-- [`Glitch`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/glitch.py)
+- [`Glitch`](voicebox.effects.glitch.Glitch)
   creates a glitchy sound by randomly repeating small chunks of audio.
-- [`RingMod`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/modulation.py)
+- [`RingMod`](voicebox.effects.modulation.RingMod)
   can be used to create choppy, Doctor Who Dalek-like effects.
-- [`Vocoder`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/vocoder.py)
+- [`Vocoder`](voicebox.effects.vocoder.Vocoder)
   is useful for making monotone, robotic voices.
 
 There is also support for all the awesome audio plugins in
 [Spotify's `pedalboard` library](https://spotify.github.io/pedalboard/index.html)
-using the special
-[`PedalboardEffect`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/effects/pedalboard.py)
+using the special [`PedalboardEffect`](voicebox.effects.pedalboard.PedalboardEffect)
 wrapper, e.g.:
 
 ```python
 from voicebox import SimpleVoicebox
 from voicebox.effects import PedalboardEffect
 import pedalboard
 
@@ -218,57 +220,78 @@
 
 voicebox = SimpleVoicebox()
 voicebox.say('Hello, world!')
 ```
 
 ### Pre-built
 
-Some pre-built voiceboxes are available in the [`voicebox.examples`](https://github.com/austin-bowen/voicebox/tree/main/src/voicebox/examples) package.
+Some pre-built voiceboxes are available in the
+[`voicebox.examples`](voicebox.examples) package.
 They can be imported into your own code, and you can run them to demo:
 
 ```bash
 # Voice of GLaDOS from the Portal video game series
 python -m voicebox.examples.glados "optional message"
 
 # Voice of the OOM-9 command battle droid from Star Wars: Episode I
 python -m voicebox.examples.battle_droid "optional message"
 ```
 
 ### Advanced
 
 ```python
 # Use eSpeak NG at 120 WPM and en-us voice as the TTS engine
-from voicebox.tts import ESpeakConfig, ESpeakNG
+from voicebox import reliable_tts
+from voicebox.tts import ESpeakConfig, ESpeakNG, gTTS
 
-tts = ESpeakNG(ESpeakConfig(speed=120, voice='en-us'))
+# Wrap multiple TTSs in retries and caches
+tts = reliable_tts(
+    ttss=[
+        # Prefer using online TTS first
+        gTTS(),
+        # Fall back to offline TTS if online TTS fails
+        ESpeakNG(ESpeakConfig(speed=120, voice='en-us')),
+    ],
+)
 
 # Add some voice effects
 from voicebox.effects import Vocoder, Glitch, Normalize
 
 effects = [
-    Vocoder.build(),  # Makes a very robotic, monotone voice
-    Glitch(),  # Randomly repeats small sections of audio
-    Normalize(),  # Remove DC and make volume consistent
+    Vocoder.build(),    # Make a robotic, monotone voice
+    Glitch(),           # Randomly repeat small sections of audio
+    Normalize(),        # Remove DC and make volume consistent
 ]
 
-# Send audio to playback device, and save to speech.wav file
+# Build audio sink
 from voicebox.sinks import Distributor, SoundDevice, WaveFile
 
 sink = Distributor([
-    SoundDevice(),
-    WaveFile('speech.wav'),
+    SoundDevice(),          # Send audio to playback device
+    WaveFile('speech.wav'), # Save audio to speech.wav file
 ])
 
 # Build the voicebox
-from voicebox import SimpleVoicebox
+from voicebox import ParallelVoicebox
+from voicebox.voiceboxes.splitter import SimpleSentenceSplitter
 
-voicebox = SimpleVoicebox(tts, effects, sink)
+# Parallel voicebox doesn't block the main thread
+voicebox = ParallelVoicebox(
+    tts,
+    effects,
+    sink,
+    # Split text into sentences to reduce time to first speech
+    text_splitter=SimpleSentenceSplitter(),
+)
 
-# eSpeak NG is used to say "Hello, world!" with a glitchy robot voice
+# Speak!
 voicebox.say('Hello, world!')
+
+# Wait for all audio to finish playing before exiting
+voicebox.wait_until_done()
 ```
 
 ### Command Line Demo
 
 ```bash
 python -m voicebox -h               # Print command help
 python -m voicebox "Hello, world!"  # Basic usage
```

### Comparing `voicebox-tts-0.0.7/src/voicebox_tts.egg-info/SOURCES.txt` & `voicebox_tts-0.0.8/src/voicebox_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/tests/test_audio.py` & `voicebox_tts-0.0.8/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `voicebox-tts-0.0.7/tests/test_ssml.py` & `voicebox_tts-0.0.8/tests/test_ssml.py`

 * *Files identical despite different names*

