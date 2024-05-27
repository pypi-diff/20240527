# Comparing `tmp/evo_framework-22024.5.5.tar.gz` & `tmp/evo_framework-22024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evo_framework-22024.5.5.tar", max compression
+gzip compressed data, was "evo_framework-22024.5.6.tar", max compression
```

## Comparing `evo_framework-22024.5.5.tar` & `evo_framework-22024.5.6.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0        0 2024-05-27 17:58:02.124599 evo_framework-22024.5.5/README.md
--rw-r--r--   0        0        0        0 2024-05-27 18:53:16.952349 evo_framework-22024.5.5/evo/__init__.py
--rwxr-xr-x   0        0        0      830 2024-04-17 13:11:06.786632 evo_framework-22024.5.5/evo/evo_framework/__init__.py
--rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-22024.5.5/evo/evo_framework/control/CObject.py
--rwxr-xr-x   0        0        0       55 2021-12-06 13:42:26.000000 evo_framework-22024.5.5/evo/evo_framework/control/__init__.py
--rw-r--r--   0        0        0      375 2024-05-24 09:08:18.009572 evo_framework-22024.5.5/evo/evo_framework/core/__init__.py
--rwxr-xr-x   0        0        0      172 2024-04-19 18:05:05.984591 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/__init__.py
--rw-r--r--   0        0        0     1234 2024-05-27 12:47:55.210401 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/automation/entity.yaml
--rw-r--r--   0        0        0     5727 2024-05-26 09:02:53.383654 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/control/CApi.py
--rw-r--r--   0        0        0    25938 2024-04-30 07:45:02.754389 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/control/CApiFlow.py
--rw-r--r--   0        0        0      139 2024-04-23 13:31:42.061922 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/control/__init__.py
--rw-r--r--   0        0        0     5302 2024-05-26 19:05:54.269516 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EAction.py
--rw-r--r--   0        0        0     3400 2024-04-30 07:46:43.021601 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EActionItem.py
--rw-r--r--   0        0        0     1318 2024-04-19 18:07:44.067267 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EActionTask.py
--rw-r--r--   0        0        0     5714 2024-05-26 09:05:02.361117 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApi.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727399 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py
--rw-r--r--   0        0        0     4025 2024-04-28 19:23:27.721336 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py
--rw-r--r--   0        0        0     4429 2024-04-27 00:31:04.310181 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiEntity.py
--rw-r--r--   0        0        0     1672 2024-05-27 13:15:44.726902 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiFile.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727081 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiImage.py
--rw-r--r--   0        0        0     1245 2024-05-24 13:13:40.128210 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiItem.py
--rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727247 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py
--rwxr-xr-x   0        0        0     2136 2024-04-20 18:47:45.597392 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/ERequest.py
--rwxr-xr-x   0        0        0      703 2024-04-15 20:02:21.126538 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EResponse.py
--rw-r--r--   0        0        0      176 2024-04-19 16:53:34.484658 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py
--rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
--rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
--rw-r--r--   0        0        0      260 2024-04-22 17:04:29.179000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EnumApiType.py
--rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EnumLanguage.py
--rwxr-xr-x   0        0        0     1723 2024-05-27 13:30:46.260548 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/__init__.py
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729616 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiAudio.cs
--rw-r--r--   0        0        0     1611 2024-05-27 13:15:44.729333 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiFile.cs
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729435 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiImage.cs
--rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729535 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiVideo.cs
--rw-r--r--   0        0        0     5283 2024-04-25 07:23:54.907302 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/evo_core_api_entity_pb2.py
--rwxr-xr-x   0        0        0      336 2024-04-14 16:10:28.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/proto/build_proto.sh
--rw-r--r--   0        0        0    78867 2024-04-25 07:23:54.933268 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/proto/entity/cs/EvoCoreApiEntity.cs
--rw-r--r--   0        0        0     2814 2024-04-25 07:23:37.891555 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/proto/evo_core_api_entity.proto
--rwxr-xr-x   0        0        0    11468 2024-04-29 01:29:38.849439 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/utility/IuApi.py
--rw-r--r--   0        0        0    14972 2024-04-11 12:54:19.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py
--rwxr-xr-x   0        0        0       68 2024-03-22 08:51:24.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/utility/__init__.py
--rwxr-xr-x   0        0        0      223 2024-03-29 21:27:12.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/__init__.py
--rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/entity/IBinary.py
--rwxr-xr-x   0        0        0     9101 2024-04-20 10:22:41.877540 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py
--rw-r--r--   0        0        0     6662 2024-04-22 18:30:35.211681 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
--rw-r--r--   0        0        0     7728 2024-04-22 18:30:35.215456 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/UBinary.py
--rw-r--r--   0        0        0     1360 2024-04-11 08:07:07.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_boot/control/CBoot.py
--rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_bridge/IBridge.py
--rw-r--r--   0        0        0       79 2024-04-11 08:42:37.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py
--rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/utility/__init__.py
--rw-r--r--   0        0        0      248 2024-03-29 21:12:01.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
--rwxr-xr-x   0        0        0     1471 2024-04-20 18:17:27.427816 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
--rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
--rw-r--r--   0        0        0     1344 2024-04-22 10:08:58.482611 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py
--rw-r--r--   0        0        0      707 2024-04-11 08:07:07.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_foundation/IFoundation.py
--rw-r--r--   0        0        0       67 2024-03-29 21:24:14.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_key/__init__.py
--rw-r--r--   0        0        0      897 2024-04-16 15:31:33.740160 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_key/utility/IuKey.py
--rw-r--r--   0        0        0       67 2024-03-29 18:12:11.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_log/__init__.py
--rw-r--r--   0        0        0     2154 2024-03-17 19:32:16.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_log/utility/IuLog.py
--rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_log/utility/ULogger.py
--rwxr-xr-x   0        0        0      154 2024-04-11 08:09:54.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/__init__.py
--rw-r--r--   0        0        0     2825 2024-04-20 18:51:28.692331 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/control/CSetting.py
--rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/control/__init__.py
--rw-r--r--   0        0        0     1205 2024-04-22 10:09:10.368909 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/entity/ESetting.py
--rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/entity/__init__.py
--rw-r--r--   0        0        0       76 2024-03-29 21:25:40.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_system/__init__.py
--rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_system/control/__init__.py
--rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_system/utility/IuSystem.py
--rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_system/utility/__init__.py
--rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_type/__init__.py
--rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_type/entity/EvoMap.py
--rw-r--r--   0        0        0       70 2024-04-11 08:44:35.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_yaml/__init__.py
--rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-22024.5.5/evo/evo_framework/core/evo_core_yaml/utility/IuYaml.py
--rwxr-xr-x   0        0        0     9317 2024-05-27 19:11:04.713901 evo_framework-22024.5.5/evo/evo_framework/entity/EObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-22024.5.5/evo/evo_framework/entity/IEObject.py
--rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-22024.5.5/evo/evo_framework/entity/IEvo.py
--rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-22024.5.5/evo/evo_framework/entity/Id.py
--rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-22024.5.5/evo/evo_framework/entity/Time.py
--rwxr-xr-x   0        0        0      185 2024-03-29 18:40:07.000000 evo_framework-22024.5.5/evo/evo_framework/entity/__init__.py
--rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-22024.5.5/evo/evo_framework/utility/__init__.py
--rw-r--r--   0        0        0      501 2024-05-27 19:11:11.375172 evo_framework-22024.5.5/pyproject.toml
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 evo_framework-22024.5.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-27 17:58:02.124599 evo_framework-22024.5.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 18:53:16.952349 evo_framework-22024.5.6/evo/__init__.py
+-rwxr-xr-x   0        0        0      830 2024-04-17 13:11:06.786632 evo_framework-22024.5.6/evo/evo_framework/__init__.py
+-rwxr-xr-x   0        0        0     4030 2024-04-14 21:01:20.000000 evo_framework-22024.5.6/evo/evo_framework/control/CObject.py
+-rwxr-xr-x   0        0        0       55 2021-12-06 13:42:26.000000 evo_framework-22024.5.6/evo/evo_framework/control/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-24 09:08:18.009572 evo_framework-22024.5.6/evo/evo_framework/core/__init__.py
+-rwxr-xr-x   0        0        0      172 2024-04-19 18:05:05.984591 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/__init__.py
+-rw-r--r--   0        0        0     1234 2024-05-27 12:47:55.210401 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/automation/entity.yaml
+-rw-r--r--   0        0        0     5727 2024-05-26 09:02:53.383654 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/control/CApi.py
+-rw-r--r--   0        0        0    25938 2024-04-30 07:45:02.754389 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/control/CApiFlow.py
+-rw-r--r--   0        0        0      139 2024-04-23 13:31:42.061922 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/control/__init__.py
+-rw-r--r--   0        0        0     5302 2024-05-26 19:05:54.269516 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EAction.py
+-rw-r--r--   0        0        0     3400 2024-04-30 07:46:43.021601 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EActionItem.py
+-rw-r--r--   0        0        0     1318 2024-04-19 18:07:44.067267 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EActionTask.py
+-rw-r--r--   0        0        0     5714 2024-05-26 09:05:02.361117 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApi.py
+-rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727399 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py
+-rw-r--r--   0        0        0     4025 2024-04-28 19:23:27.721336 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py
+-rw-r--r--   0        0        0     4429 2024-04-27 00:31:04.310181 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiEntity.py
+-rw-r--r--   0        0        0     1672 2024-05-27 13:15:44.726902 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiFile.py
+-rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727081 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiImage.py
+-rw-r--r--   0        0        0     1245 2024-05-24 13:13:40.128210 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiItem.py
+-rw-r--r--   0        0        0     1673 2024-05-27 13:15:44.727247 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py
+-rwxr-xr-x   0        0        0     2136 2024-04-20 18:47:45.597392 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/ERequest.py
+-rwxr-xr-x   0        0        0      703 2024-04-15 20:02:21.126538 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EResponse.py
+-rw-r--r--   0        0        0      176 2024-04-19 16:53:34.484658 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EnumApiAction.py
+-rw-r--r--   0        0        0      101 2024-03-22 09:24:36.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EnumApiCompress.py
+-rw-r--r--   0        0        0       97 2024-03-22 09:18:53.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EnumApiCrypto.py
+-rw-r--r--   0        0        0      260 2024-04-22 17:04:29.179000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EnumApiType.py
+-rw-r--r--   0        0        0        0 2024-05-27 12:52:18.397976 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EnumLanguage.py
+-rwxr-xr-x   0        0        0     1723 2024-05-27 13:30:46.260548 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/__init__.py
+-rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729616 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiAudio.cs
+-rw-r--r--   0        0        0     1611 2024-05-27 13:15:44.729333 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiFile.cs
+-rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729435 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiImage.cs
+-rw-r--r--   0        0        0     1612 2024-05-27 13:15:44.729535 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiVideo.cs
+-rw-r--r--   0        0        0     5283 2024-04-25 07:23:54.907302 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/evo_core_api_entity_pb2.py
+-rwxr-xr-x   0        0        0      336 2024-04-14 16:10:28.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/proto/build_proto.sh
+-rw-r--r--   0        0        0    78867 2024-04-25 07:23:54.933268 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/proto/entity/cs/EvoCoreApiEntity.cs
+-rw-r--r--   0        0        0     2814 2024-04-25 07:23:37.891555 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/proto/evo_core_api_entity.proto
+-rwxr-xr-x   0        0        0    11375 2024-05-27 20:14:36.152739 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/utility/IuApi.py
+-rw-r--r--   0        0        0    14972 2024-04-11 12:54:19.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py
+-rwxr-xr-x   0        0        0       68 2024-03-22 08:51:24.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/utility/__init__.py
+-rwxr-xr-x   0        0        0      223 2024-03-29 21:27:12.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/__init__.py
+-rwxr-xr-x   0        0        0      120 2021-11-24 10:46:35.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/entity/IBinary.py
+-rwxr-xr-x   0        0        0     9101 2024-04-20 10:22:41.877540 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py
+-rw-r--r--   0        0        0     6662 2024-04-22 18:30:35.211681 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py
+-rw-r--r--   0        0        0     7728 2024-04-22 18:30:35.215456 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/UBinary.py
+-rw-r--r--   0        0        0     1360 2024-04-11 08:07:07.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_boot/control/CBoot.py
+-rw-r--r--   0        0        0      281 2024-04-15 19:43:35.988232 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_bridge/IBridge.py
+-rw-r--r--   0        0        0       79 2024-04-11 08:42:37.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-14 09:37:12.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py
+-rw-r--r--   0        0        0      841 2024-04-12 09:23:48.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/utility/__init__.py
+-rw-r--r--   0        0        0      248 2024-03-29 21:12:01.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/__init__.py
+-rw-r--r--   0        0        0     1470 2024-03-26 15:03:45.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py
+-rwxr-xr-x   0        0        0     1471 2024-04-20 18:17:27.427816 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py
+-rwxr-xr-x   0        0        0      743 2024-03-17 11:26:36.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py
+-rw-r--r--   0        0        0     1344 2024-04-22 10:08:58.482611 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py
+-rw-r--r--   0        0        0      707 2024-04-11 08:07:07.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_foundation/IFoundation.py
+-rw-r--r--   0        0        0       67 2024-03-29 21:24:14.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_key/__init__.py
+-rw-r--r--   0        0        0      897 2024-04-16 15:31:33.740160 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_key/utility/IuKey.py
+-rw-r--r--   0        0        0       67 2024-03-29 18:12:11.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_log/__init__.py
+-rw-r--r--   0        0        0     2154 2024-03-17 19:32:16.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_log/utility/IuLog.py
+-rw-r--r--   0        0        0     2289 2024-03-22 09:09:45.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_log/utility/ULogger.py
+-rwxr-xr-x   0        0        0      154 2024-04-11 08:09:54.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/__init__.py
+-rw-r--r--   0        0        0     2825 2024-04-20 18:51:28.692331 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/control/CSetting.py
+-rwxr-xr-x   0        0        0        0 2024-01-05 09:11:06.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/control/__init__.py
+-rw-r--r--   0        0        0     1205 2024-04-22 10:09:10.368909 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/entity/ESetting.py
+-rw-r--r--   0        0        0        0 2024-01-05 20:57:13.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/entity/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-29 21:25:40.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_system/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:13:56.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_system/control/__init__.py
+-rw-r--r--   0        0        0     6742 2024-02-12 00:08:10.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_system/utility/IuSystem.py
+-rw-r--r--   0        0        0        0 2024-01-04 13:14:10.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_system/utility/__init__.py
+-rw-r--r--   0        0        0        0 2021-11-12 08:43:14.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_type/__init__.py
+-rwxr-xr-x   0        0        0      953 2024-04-22 18:31:06.740795 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_type/entity/EvoMap.py
+-rw-r--r--   0        0        0       70 2024-04-11 08:44:35.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_yaml/__init__.py
+-rw-r--r--   0        0        0      304 2024-03-02 18:03:59.000000 evo_framework-22024.5.6/evo/evo_framework/core/evo_core_yaml/utility/IuYaml.py
+-rwxr-xr-x   0        0        0     9317 2024-05-27 19:11:04.713901 evo_framework-22024.5.6/evo/evo_framework/entity/EObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:03:14.000000 evo_framework-22024.5.6/evo/evo_framework/entity/IEObject.py
+-rw-r--r--   0        0        0        0 2021-11-23 22:02:39.000000 evo_framework-22024.5.6/evo/evo_framework/entity/IEvo.py
+-rwxr-xr-x   0        0        0       64 2021-11-23 22:11:09.000000 evo_framework-22024.5.6/evo/evo_framework/entity/Id.py
+-rwxr-xr-x   0        0        0       62 2021-11-23 22:13:51.000000 evo_framework-22024.5.6/evo/evo_framework/entity/Time.py
+-rwxr-xr-x   0        0        0      185 2024-03-29 18:40:07.000000 evo_framework-22024.5.6/evo/evo_framework/entity/__init__.py
+-rwxr-xr-x   0        0        0        0 2024-01-14 01:56:17.000000 evo_framework-22024.5.6/evo/evo_framework/utility/__init__.py
+-rw-r--r--   0        0        0      501 2024-05-27 20:11:49.060791 evo_framework-22024.5.6/pyproject.toml
+-rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 evo_framework-22024.5.6/PKG-INFO
```

### Comparing `evo_framework-22024.5.5/evo/evo_framework/__init__.py` & `evo_framework-22024.5.6/evo/evo_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/control/CObject.py` & `evo_framework-22024.5.6/evo/evo_framework/control/CObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/automation/entity.yaml` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/automation/entity.yaml`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/control/CApi.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/control/CApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/control/CApiFlow.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/control/CApiFlow.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EAction.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EAction.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EActionItem.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EActionItem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EActionTask.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EActionTask.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApi.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApi.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiAudio.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiConfig.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiEntity.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiEntity.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiFile.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiFile.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiImage.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiImage.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiItem.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiItem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EApiVideo.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/ERequest.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/ERequest.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/EResponse.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/EResponse.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/__init__.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiAudio.cs` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiAudio.cs`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiFile.cs` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiFile.cs`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiImage.cs` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiImage.cs`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/cs/EApiVideo.cs` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/cs/EApiVideo.cs`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/entity/evo_core_api_entity_pb2.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/entity/evo_core_api_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/proto/entity/cs/EvoCoreApiEntity.cs` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/proto/entity/cs/EvoCoreApiEntity.cs`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/proto/evo_core_api_entity.proto` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/proto/evo_core_api_entity.proto`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/utility/IuApi.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/utility/IuApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from evo.evo_framework.core.evo_core_binary.utility.IuBinary import IuBinary
 from PIL import Image
 import importlib
 # ---------------------------------------------------------------------------------------------------------------------------------------
 class IuApi(object):
 
  # ---------------------------------------------------------------------------------------------------------------------------------------       
-    
+    @staticmethod
     def newEAction(action:str) -> EAction:
         try: 
             eAction = EAction()
             eAction.doGenerateID()
             eAction.doGenerateTime()
             eAction.action= action
             return eAction      
@@ -55,17 +55,14 @@
     @staticmethod
     def addCApi(module:str):
         from evo.evo_framework.core.evo_core_api.control.CApi import CApi
         
         if not module:
             raise Exception("ERROR_NONE_MODULE")
             
-        if not module.startswith("evo.evo_packages."):
-            module = f"evo.evo_packages.{module}"
-
         arrayModule= module.split(".")
         className = arrayModule[-1]
         IuLog.doDebug(__name__, f"{module} {className}")
         ClassCApiAction = getattr(importlib.import_module(module), className)
         if ClassCApiAction:
             cApi=ClassCApiAction.getInstance()
             if isinstance(cApi,CApi):
```

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_api/utility/IuApiPb.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/IuBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/IuBinaryAsync.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_binary/utility/UBinary.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_binary/utility/UBinary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_boot/control/CBoot.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_boot/control/CBoot.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/test_evo_core_binary.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_convert/utility/IuConvert.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptChacha.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptEC.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_crypto/utility/IuCryptHash.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_file/entity/EFileChunk.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_foundation/IFoundation.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_foundation/IFoundation.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_key/utility/IuKey.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_key/utility/IuKey.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_log/utility/IuLog.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_log/utility/IuLog.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_log/utility/ULogger.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_log/utility/ULogger.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/control/CSetting.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/control/CSetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_setting/entity/ESetting.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_setting/entity/ESetting.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_system/utility/IuSystem.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_system/utility/IuSystem.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/core/evo_core_type/entity/EvoMap.py` & `evo_framework-22024.5.6/evo/evo_framework/core/evo_core_type/entity/EvoMap.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/evo/evo_framework/entity/EObject.py` & `evo_framework-22024.5.6/evo/evo_framework/entity/EObject.py`

 * *Files identical despite different names*

### Comparing `evo_framework-22024.5.5/PKG-INFO` & `evo_framework-22024.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evo-framework
-Version: 22024.5.5
+Version: 22024.5.6
 Summary: evo framework python
 Author: cyborg-ai-git
 Author-email: 129898917+cyborg-ai-git@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

