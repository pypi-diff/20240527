# Comparing `tmp/PKDevTools-0.13.20240521.127.tar.gz` & `tmp/PKDevTools-0.13.20240527.128.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKDevTools-0.13.20240521.127.tar", last modified: Tue May 21 18:41:54 2024, max compression
+gzip compressed data, was "PKDevTools-0.13.20240527.128.tar", last modified: Mon May 27 20:59:35 2024, max compression
```

## Comparing `PKDevTools-0.13.20240521.127.tar` & `PKDevTools-0.13.20240527.128.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:54.246278 PKDevTools-0.13.20240521.127/
--rw-rw-rw-   0        0        0     1086 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:54.230653 PKDevTools-0.13.20240521.127/PKDevTools/
--rw-rw-rw-   0        0        0     1176 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:54.246278 PKDevTools-0.13.20240521.127/PKDevTools/classes/
--rw-rw-rw-   0        0        0     4960 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Archiver.py
--rw-rw-rw-   0        0        0     5178 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/ColorText.py
--rw-rw-rw-   0        0        0     3599 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Committer.py
--rw-rw-rw-   0        0        0     6376 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/CookieHelper.py
--rw-rw-rw-   0        0        0     8879 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Fetcher.py
--rw-rw-rw-   0        0        0     2608 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/FunctionTimeouts.py
--rw-rw-rw-   0        0        0    11963 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     5198 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/NSEMarketStatus.py
--rw-rw-rw-   0        0        0     2860 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/OutputControls.py
--rw-rw-rw-   0        0        0    16509 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKDateUtilities.py
--rw-rw-rw-   0        0        0     2988 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKGitFolderDownloader.py
--rw-rw-rw-   0        0        0     5243 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKJoinableQueue.py
--rw-rw-rw-   0        0        0    12875 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKMultiProcessorClient.py
--rw-rw-rw-   0        0        0    14334 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKPickler.py
--rw-rw-rw-   0        0        0     3433 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/PKTimer.py
--rw-rw-rw-   0        0        0     4548 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Singleton.py
--rw-rw-rw-   0        0        0     2004 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0    11301 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Telegram.py
--rw-rw-rw-   0        0        0    24543 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/Utils.py
--rw-rw-rw-   0        0        0     9984 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 18:41:49.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/__init__.py
--rw-rw-rw-   0        0        0     3738 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/githubutilities.py
--rw-rw-rw-   0        0        0    16136 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/log.py
--rw-rw-rw-   0        0        0     7430 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0     2864 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/squash.py
--rw-rw-rw-   0        0        0     4846 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/PKDevTools/classes/updater.py
-drwxrwxrwx   0        0        0        0 2024-05-21 18:41:54.230653 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/
--rw-rw-rw-   0        0        0     5204 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1199 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      363 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 18:41:47.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      189 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-21 18:41:54.000000 PKDevTools-0.13.20240521.127/PKDevTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5204 2024-05-21 18:41:54.246278 PKDevTools-0.13.20240521.127/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/README.md
--rw-rw-rw-   0        0        0       86 2024-05-21 18:41:54.246278 PKDevTools-0.13.20240521.127/setup.cfg
--rw-rw-rw-   0        0        0     4341 2024-05-21 18:40:33.000000 PKDevTools-0.13.20240521.127/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/
+-rw-rw-rw-   0        0        0     1086 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.315019 PKDevTools-0.13.20240527.128/PKDevTools/
+-rw-rw-rw-   0        0        0     1176 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/PKDevTools/classes/
+-rw-rw-rw-   0        0        0     4960 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Archiver.py
+-rw-rw-rw-   0        0        0     5178 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/ColorText.py
+-rw-rw-rw-   0        0        0     3599 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Committer.py
+-rw-rw-rw-   0        0        0     6376 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/CookieHelper.py
+-rw-rw-rw-   0        0        0     8879 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Fetcher.py
+-rw-rw-rw-   0        0        0     2608 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/FunctionTimeouts.py
+-rw-rw-rw-   0        0        0    11963 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     5261 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/NSEMarketStatus.py
+-rw-rw-rw-   0        0        0     2860 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/OutputControls.py
+-rw-rw-rw-   0        0        0    16509 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKDateUtilities.py
+-rw-rw-rw-   0        0        0     2988 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKGitFolderDownloader.py
+-rw-rw-rw-   0        0        0     5243 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKJoinableQueue.py
+-rw-rw-rw-   0        0        0    12875 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKMultiProcessorClient.py
+-rw-rw-rw-   0        0        0    14334 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKPickler.py
+-rw-rw-rw-   0        0        0     3433 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/PKTimer.py
+-rw-rw-rw-   0        0        0     4548 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Singleton.py
+-rw-rw-rw-   0        0        0     2004 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0    11301 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Telegram.py
+-rw-rw-rw-   0        0        0    24543 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/Utils.py
+-rw-rw-rw-   0        0        0     9984 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-27 20:59:30.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/__init__.py
+-rw-rw-rw-   0        0        0     3738 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/githubutilities.py
+-rw-rw-rw-   0        0        0    16136 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/log.py
+-rw-rw-rw-   0        0        0     7430 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0     2864 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/squash.py
+-rw-rw-rw-   0        0        0     4846 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/PKDevTools/classes/updater.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:59:35.315019 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/
+-rw-rw-rw-   0        0        0     5204 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1199 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      363 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-27 20:59:29.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      189 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 20:59:35.000000 PKDevTools-0.13.20240527.128/PKDevTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5204 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-27 20:59:35.330645 PKDevTools-0.13.20240527.128/setup.cfg
+-rw-rw-rw-   0        0        0     4341 2024-05-27 20:58:41.000000 PKDevTools-0.13.20240527.128/setup.py
```

### Comparing `PKDevTools-0.13.20240521.127/LICENSE` & `PKDevTools-0.13.20240527.128/LICENSE`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/__init__.py` & `PKDevTools-0.13.20240527.128/PKDevTools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Archiver.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/ColorText.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/ColorText.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Committer.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Committer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/CookieHelper.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/CookieHelper.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Fetcher.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/FunctionTimeouts.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/FunctionTimeouts.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/MenuOptions.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/NSEMarketStatus.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/NSEMarketStatus.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,18 +78,19 @@
         if next_bell is not None:
             return next_bell
         
         from PKDevTools.classes import Archiver
         fileName = "nse_next_bell.txt"
         next_bell, filePath, modifiedDateTime = Archiver.findFileInAppResultsDirectory(fileName)
         curr = datetime.datetime.now(pytz.timezone("Asia/Kolkata"))
-        lastBellDate = datetime.datetime.strptime(next_bell.split("T")[0],"%Y-%m-%d")
-        shouldFetch = next_bell is None or (next_bell is not None and (curr.date() > modifiedDateTime.date() or curr.date() > lastBellDate.date()))
+        dtPart = next_bell.replace("T"," ").split("+")[0]
+        lastBellDateTime = datetime.datetime.strptime(dtPart,"%Y-%m-%d %H:%M:%S").replace(tzinfo=curr.tzinfo)
+        shouldFetch = next_bell is None or (next_bell is not None and (curr.date() > modifiedDateTime.date() or curr > lastBellDateTime))
         if shouldFetch:
-            scraper = cloudscraper.create_scraper()          
+            scraper = cloudscraper.create_scraper()
             url = "https://www.tradinghours.com/markets/nse-india"
             res = scraper.get(url)
             try:
                 if res is None or res.status_code != 200:
                     return ""
                 marketResp = res.text
                 jsonDict = marketResp.split("window.Statuses = ")[1].split(";")[0]
```

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/OutputControls.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/OutputControls.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKDateUtilities.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKDateUtilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKGitFolderDownloader.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKGitFolderDownloader.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKJoinableQueue.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKJoinableQueue.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKMultiProcessorClient.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKMultiProcessorClient.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKPickler.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKPickler.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/PKTimer.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/PKTimer.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Singleton.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Singleton.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/SuppressOutput.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Telegram.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Telegram.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/Utils.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/Utils.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/WorkflowManager.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/githubutilities.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/githubutilities.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/log.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/log.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/multiprocessing_logging.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/squash.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/squash.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools/classes/updater.py` & `PKDevTools-0.13.20240527.128/PKDevTools/classes/updater.py`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools.egg-info/PKG-INFO` & `PKDevTools-0.13.20240527.128/PKDevTools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240521.127
+Version: 0.13.20240527.128
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240521.127.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240527.128.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240521.127/PKDevTools.egg-info/SOURCES.txt` & `PKDevTools-0.13.20240527.128/PKDevTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/PKG-INFO` & `PKDevTools-0.13.20240527.128/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKDevTools
-Version: 0.13.20240521.127
+Version: 0.13.20240527.128
 Summary: A general day-to-day toolset for repos
 Home-page: https://github.com/pkjmesra/PKDevTools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240521.127.zip
+Download-URL: https://github.com/pkjmesra/PKDevTools/archive/v0.13.20240527.128.zip
 Keywords: GitHub tools,Logging,Telegram,Fetcher
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKDevTools-0.13.20240521.127/README.md` & `PKDevTools-0.13.20240527.128/README.md`

 * *Files identical despite different names*

### Comparing `PKDevTools-0.13.20240521.127/setup.py` & `PKDevTools-0.13.20240527.128/setup.py`

 * *Files identical despite different names*

