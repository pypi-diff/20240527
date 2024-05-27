# Comparing `tmp/requeue-0.3.0.tar.gz` & `tmp/requeue-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requeue-0.3.0.tar", max compression
+gzip compressed data, was "requeue-0.4.0.tar", max compression
```

## Comparing `requeue-0.3.0.tar` & `requeue-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.3.0/LICENSE
--rw-r--r--   0        0        0     1318 2024-05-03 12:10:34.112347 requeue-0.3.0/README.md
--rw-r--r--   0        0        0      391 2024-05-03 11:50:51.082351 requeue-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3087 2024-05-03 12:15:51.593431 requeue-0.3.0/requeue/__init__.py
--rw-r--r--   0        0        0     1921 1970-01-01 00:00:00.000000 requeue-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-03-10 22:34:57.217631 requeue-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1320 2024-05-27 00:20:24.122941 requeue-0.4.0/README.md
+-rw-r--r--   0        0        0      391 2024-05-27 00:20:40.806041 requeue-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3736 2024-05-27 01:48:18.147420 requeue-0.4.0/requeue/__init__.py
+-rw-r--r--   0        0        0     1872 1970-01-01 00:00:00.000000 requeue-0.4.0/PKG-INFO
```

### Comparing `requeue-0.3.0/LICENSE` & `requeue-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requeue-0.3.0/README.md` & `requeue-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
 @client.callback
 async def on_message(message):
     # An example of a knock knock joke back-and-forth,
     # using the request queue to pick out the responses
 
     if message == 'Knock knock!':
         await client.send("Who's there?")
-        who = await queue.wait_for()
+        who, = await queue.wait_for()
         await client.send(f'{who} who?')
-        punchline = await queue.wait_for()
+        punchline, = await queue.wait_for()
         await punchline.react('😂')
 ```
```

### Comparing `requeue-0.3.0/PKG-INFO` & `requeue-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: requeue
-Version: 0.3.0
+Version: 0.4.0
 Summary: An asynchronous queue for requesting data
 Home-page: https://gitlab.com/deepadmax/requeue
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://gitlab.com/deepadmax/requeue
 Description-Content-Type: text/markdown
 
 # Requeue
 
 In applications that receive messages, like chat bots, where you run callbacks
@@ -49,13 +48,13 @@
 @client.callback
 async def on_message(message):
     # An example of a knock knock joke back-and-forth,
     # using the request queue to pick out the responses
 
     if message == 'Knock knock!':
         await client.send("Who's there?")
-        who = await queue.wait_for()
+        who, = await queue.wait_for()
         await client.send(f'{who} who?')
-        punchline = await queue.wait_for()
+        punchline, = await queue.wait_for()
         await punchline.react('😂')
 ```
```

