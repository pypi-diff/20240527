# Comparing `tmp/bilifm-0.2.1.tar.gz` & `tmp/bilifm-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bilifm-0.2.1.tar", last modified: Thu Mar 14 10:29:20 2024, max compression
+gzip compressed data, was "bilifm-0.2.2.tar", last modified: Mon May 27 07:30:24 2024, max compression
```

## Comparing `bilifm-0.2.1.tar` & `bilifm-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35148 2023-08-17 14:04:07.364742 bilifm-0.2.1/LICENSE
--rw-r--r--   0        0        0     3464 2024-03-05 13:14:08.109143 bilifm-0.2.1/README.md
--rw-r--r--   0        0        0      857 2024-03-14 10:29:20.940524 bilifm-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       25 2024-03-14 10:20:20.590921 bilifm-0.2.1/src/bilifm/__init__.py
--rw-r--r--   0        0        0     4933 2024-03-14 10:20:20.590921 bilifm-0.2.1/src/bilifm/audio.py
--rw-r--r--   0        0        0      664 2024-03-14 10:20:20.590921 bilifm-0.2.1/src/bilifm/command.py
--rw-r--r--   0        0        0     1247 2024-03-14 10:20:20.590921 bilifm-0.2.1/src/bilifm/fav.py
--rw-r--r--   0        0        0     1035 2024-03-14 10:20:20.590921 bilifm-0.2.1/src/bilifm/user.py
--rw-r--r--   0        0        0     3903 2024-03-05 13:13:32.736342 bilifm-0.2.1/src/bilifm/util.py
--rw-r--r--   0        0        0        0 2023-12-17 06:43:23.900276 bilifm-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 bilifm-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-08-17 14:04:07.364742 bilifm-0.2.2/LICENSE
+-rw-r--r--   0        0        0     4330 2024-05-27 06:57:42.479912 bilifm-0.2.2/README.md
+-rw-r--r--   0        0        0      857 2024-05-27 07:30:24.447346 bilifm-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       25 2024-03-14 10:20:20.590921 bilifm-0.2.2/src/bilifm/__init__.py
+-rw-r--r--   0        0        0     5788 2024-05-27 07:21:21.036254 bilifm-0.2.2/src/bilifm/audio.py
+-rw-r--r--   0        0        0     2326 2024-05-27 07:21:21.036254 bilifm-0.2.2/src/bilifm/command.py
+-rw-r--r--   0        0        0     1247 2024-03-14 10:20:20.590921 bilifm-0.2.2/src/bilifm/fav.py
+-rw-r--r--   0        0        0     2701 2024-05-27 06:57:42.479912 bilifm-0.2.2/src/bilifm/season.py
+-rw-r--r--   0        0        0     2182 2024-05-27 06:57:42.479912 bilifm-0.2.2/src/bilifm/series.py
+-rw-r--r--   0        0        0     1035 2024-03-14 10:20:20.590921 bilifm-0.2.2/src/bilifm/user.py
+-rw-r--r--   0        0        0     5637 2024-05-27 07:21:21.036254 bilifm-0.2.2/src/bilifm/util.py
+-rw-r--r--   0        0        0     4945 1970-01-01 00:00:00.000000 bilifm-0.2.2/PKG-INFO
```

### Comparing `bilifm-0.2.1/LICENSE` & `bilifm-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bilifm-0.2.1/README.md` & `bilifm-0.2.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -71,15 +71,59 @@
 
 ![media_id](./assets/fav.png)
 
 cookies 的获取：
 
 - 在开发者工具的控制台中输入 `document.cookie`
 
-- cookies 转换为json：[在线 cookies 转换](https://uutool.cn/cookie2json/)
+- cookies 转换为 json：[在线 cookies 转换](https://uutool.cn/cookie2json/)
+
+### season 模式
+
+下载视频合集
+
+```bash
+bilifm season $uid $sid [OPTIONS]
+```
+
+- uid, sid 的获取:
+  打开视频合集网页, 从 URL 中获取
+
+https://space.bilibili.com/23263470/channel/collectiondetail?sid=1855309
+
+例如上面链接, uid 为 23263470, sid 为 1855309 (目前 uid 可以随意填写)
+
+```bash
+bilifm season 23263470 1855309
+```
+
+- Options:
+  - -o, --directory 选择音频保存地址
+
+### series 模式
+
+下载视频列表
+
+```bash
+bilifm series $uid $sid [OPTIONS]
+```
+
+- uid, sid 的获取:
+  打开用户空间中的合集和列表, 找到列表点击更多, 然后从URL中获取
+
+https://space.bilibili.com/488978908/channel/seriesdetail?sid=888434
+
+例如上面链接, uid 为 488978908, sid 为 888434. 使用下面命令
+
+```bash
+bilifm series 488978908 888434
+```
+
+- Options:
+  - -o, --directory 选择音频保存地址
 
 ## Features
 
 - ~~python 版本限制未知~~
   - 在函数定义时使用了类型注解，故不建议使用 3.5 以下版本
 
 - 接口简洁方便调用
@@ -101,15 +145,15 @@
         audio.download()
 
     typer.echo("Download complete")
 ```
 
 ## Issues
 
-- 获取up主视频列表时会出现 UnicodeDecodeError，~~原因未知~~
+- 获取 UP 主视频列表时会出现 UnicodeDecodeError，~~原因未知~~
   - 初步判断是网络不稳定所致，在稳定的网络环境下没有出现此问题
   - 暂时采用 try-except 跳过这一过程
 - 在使用前需关闭代理
 
 ## Licence
 
 - ~~bilibiliaudioDownloader 的作者没有选取许可证，暂时选择 MIT License~~
```

### Comparing `bilifm-0.2.1/pyproject.toml` & `bilifm-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bilifm"
-version = "0.2.1"
+version = "0.2.2"
 description = "Download Bilibili videos as audios."
 authors = [
     { name = "jingfelix", email = "jingfelix@outlook.com" },
     { name = "Felix Jing", email = "jingfelix@outlook.com" },
 ]
 dependencies = [
     "requests",
```

### Comparing `bilifm-0.2.1/src/bilifm/audio.py` & `bilifm-0.2.2/src/bilifm/audio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import sys
 import time
 
 import requests
 import typer
 
-from .util import get_signed_params
+from .util import AudioQualityEnums, get_signed_params
 
 
 class Audio:
     bvid = ""
     title = ""
     playUrl = "http://api.bilibili.com/x/player/wbi/playurl"
     part_list = []
 
     headers = {}
 
-    def __init__(self, bvid: str) -> None:
+    def __init__(self, bvid: str, audio_quality: AudioQualityEnums) -> None:
         if bvid is None:
             raise ValueError("bvid is None")
 
         self.bvid = bvid
         self.headers = {
             "authority": "api.bilibili.com",
             "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
@@ -36,14 +36,16 @@
             "sec-fetch-site": "none",
             "sec-fetch-user": "?1",
             "upgrade-insecure-requests": "1",
             "user-agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36",
             "Referer": "https://www.bilibili.com/video/{bvid}".format(bvid=self.bvid),
         }
 
+        self.audio_quality = audio_quality.quality_id
+
         # 获取cid和title
         if len(bvid) == 12:
             # BV号
             self.__get_cid_title(bvid)
         else:
             # AV号
             self.__get_cid_title(bvid[:12])
@@ -72,17 +74,37 @@
                         "cid": cid,
                     }
                 )
                 json = requests.get(
                     self.playUrl, params=params, headers=self.headers
                 ).json()
 
-                baseUrl = json["data"]["dash"]["audio"][0]["baseUrl"]
+                if json["data"] is None:
+                    typer.echo(
+                        f" `data` field is not valid with url: {self.playUrl} and params : {params}"
+                    )
+                    return
+
+                audio = json["data"]["dash"]["audio"]
+                if not audio:
+                    typer.echo(
+                        f" `audio` field is empty with url: {self.playUrl} and params : {params}"
+                    )
+                    return
+
+                base_url = None
+                for au in audio:
+                    if au["id"] == self.audio_quality:
+                        base_url = au["baseUrl"]
+
+                # no audio url corresponding to current audio quality
+                if base_url is None:
+                    base_url = audio[0]["baseUrl"]
 
-                response = requests.get(url=baseUrl, headers=self.headers, stream=True)
+                response = requests.get(url=base_url, headers=self.headers, stream=True)
 
                 total_size = int(response.headers.get("content-length", 0))
                 temp_size = 0
 
                 with open(file_path, "wb") as f:
                     for chunk in response.iter_content(chunk_size=1024):
                         if chunk:
```

### Comparing `bilifm-0.2.1/src/bilifm/fav.py` & `bilifm-0.2.2/src/bilifm/fav.py`

 * *Files identical despite different names*

### Comparing `bilifm-0.2.1/src/bilifm/user.py` & `bilifm-0.2.2/src/bilifm/user.py`

 * *Files identical despite different names*

### Comparing `bilifm-0.2.1/PKG-INFO` & `bilifm-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilifm
-Version: 0.2.1
+Version: 0.2.2
 Summary: Download Bilibili videos as audios.
 Author-Email: jingfelix <jingfelix@outlook.com>, Felix Jing <jingfelix@outlook.com>
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/jingfelix/bilifm
@@ -87,15 +87,59 @@
 
 ![media_id](./assets/fav.png)
 
 cookies 的获取：
 
 - 在开发者工具的控制台中输入 `document.cookie`
 
-- cookies 转换为json：[在线 cookies 转换](https://uutool.cn/cookie2json/)
+- cookies 转换为 json：[在线 cookies 转换](https://uutool.cn/cookie2json/)
+
+### season 模式
+
+下载视频合集
+
+```bash
+bilifm season $uid $sid [OPTIONS]
+```
+
+- uid, sid 的获取:
+  打开视频合集网页, 从 URL 中获取
+
+https://space.bilibili.com/23263470/channel/collectiondetail?sid=1855309
+
+例如上面链接, uid 为 23263470, sid 为 1855309 (目前 uid 可以随意填写)
+
+```bash
+bilifm season 23263470 1855309
+```
+
+- Options:
+  - -o, --directory 选择音频保存地址
+
+### series 模式
+
+下载视频列表
+
+```bash
+bilifm series $uid $sid [OPTIONS]
+```
+
+- uid, sid 的获取:
+  打开用户空间中的合集和列表, 找到列表点击更多, 然后从URL中获取
+
+https://space.bilibili.com/488978908/channel/seriesdetail?sid=888434
+
+例如上面链接, uid 为 488978908, sid 为 888434. 使用下面命令
+
+```bash
+bilifm series 488978908 888434
+```
+
+- Options:
+  - -o, --directory 选择音频保存地址
 
 ## Features
 
 - ~~python 版本限制未知~~
   - 在函数定义时使用了类型注解，故不建议使用 3.5 以下版本
 
 - 接口简洁方便调用
@@ -117,15 +161,15 @@
         audio.download()
 
     typer.echo("Download complete")
 ```
 
 ## Issues
 
-- 获取up主视频列表时会出现 UnicodeDecodeError，~~原因未知~~
+- 获取 UP 主视频列表时会出现 UnicodeDecodeError，~~原因未知~~
   - 初步判断是网络不稳定所致，在稳定的网络环境下没有出现此问题
   - 暂时采用 try-except 跳过这一过程
 - 在使用前需关闭代理
 
 ## Licence
 
 - ~~bilibiliaudioDownloader 的作者没有选取许可证，暂时选择 MIT License~~
```

