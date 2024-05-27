# Comparing `tmp/halchat-0.0.2.2.tar.gz` & `tmp/halchat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halchat-0.0.2.2.tar", last modified: Wed May 22 19:26:23 2024, max compression
+gzip compressed data, was "halchat-0.0.3.tar", last modified: Mon May 27 13:09:00 2024, max compression
```

## Comparing `halchat-0.0.2.2.tar` & `halchat-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:26:23.870380 halchat-0.0.2.2/
--rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.2.2/LICENSE
--rw-rw-rw-   0        0        0      482 2024-05-22 19:26:23.869316 halchat-0.0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.2.2/README.md
--rw-rw-rw-   0        0        0      425 2024-05-22 19:26:18.000000 halchat-0.0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 19:26:23.870380 halchat-0.0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 19:26:23.862316 halchat-0.0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 19:26:23.869316 halchat-0.0.2.2/src/HalChat.egg-info/
--rw-rw-rw-   0        0        0      482 2024-05-22 19:26:23.000000 halchat-0.0.2.2/src/HalChat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-22 19:26:23.000000 halchat-0.0.2.2/src/HalChat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:26:23.000000 halchat-0.0.2.2/src/HalChat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 19:26:23.000000 halchat-0.0.2.2/src/HalChat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8113 2024-05-22 19:24:43.000000 halchat-0.0.2.2/src/HalChatAPI.py
--rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.2.2/src/HalEncryption.py
--rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.2.2/src/HalHash.py
--rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.2.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:09:00.709586 halchat-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-12 13:55:45.000000 halchat-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      480 2024-05-27 13:09:00.708582 halchat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2024-05-12 13:59:25.000000 halchat-0.0.3/README.md
+-rw-rw-rw-   0        0        0      423 2024-05-27 12:52:44.000000 halchat-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:09:00.709586 halchat-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 13:09:00.695567 halchat-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-27 13:09:00.708582 halchat-0.0.3/src/HalChat.egg-info/
+-rw-rw-rw-   0        0        0      480 2024-05-27 13:09:00.000000 halchat-0.0.3/src/HalChat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-27 13:09:00.000000 halchat-0.0.3/src/HalChat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:09:00.000000 halchat-0.0.3/src/HalChat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:09:00.000000 halchat-0.0.3/src/HalChat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8114 2024-05-27 13:08:48.000000 halchat-0.0.3/src/HalChatAPI.py
+-rw-rw-rw-   0        0        0     1702 2024-02-12 15:42:01.000000 halchat-0.0.3/src/HalEncryption.py
+-rw-rw-rw-   0        0        0     2724 2024-02-12 16:04:02.000000 halchat-0.0.3/src/HalHash.py
+-rw-rw-rw-   0        0        0        0 2024-05-12 13:57:45.000000 halchat-0.0.3/src/__init__.py
```

### Comparing `halchat-0.0.2.2/LICENSE` & `halchat-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `halchat-0.0.2.2/src/HalChatAPI.py` & `halchat-0.0.3/src/HalChatAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                     elif v['type']==6:
                         self.run_event('onClickButton',[v['fromChat'],v['fromId'],v['fromMsg'],v['data']])
             if self.check_bots_messages:
                 data=self.getBotsMessages()
                 if not data is None and data['errorCode']==0:
                     for msg in data['messages']:
                         self.run_event('onBotMessage',[msg['fromId'],msg['time'],msg['data']])
-            time.sleep(self.sleepTime)
+            #time.sleep(self.sleepTime)
 
     def close(self):
         self.isRun=False
 
     def addChatPassword(self,chatId:int,password:str):
         self.chatsPasswords[str(chatId)]=password
```

### Comparing `halchat-0.0.2.2/src/HalEncryption.py` & `halchat-0.0.3/src/HalEncryption.py`

 * *Files identical despite different names*

### Comparing `halchat-0.0.2.2/src/HalHash.py` & `halchat-0.0.3/src/HalHash.py`

 * *Files identical despite different names*

