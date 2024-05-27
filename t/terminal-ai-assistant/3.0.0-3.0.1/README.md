# Comparing `tmp/terminal_ai_assistant-3.0.0.tar.gz` & `tmp/terminal_ai_assistant-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminal_ai_assistant-3.0.0.tar", last modified: Mon May 27 07:30:10 2024, max compression
+gzip compressed data, was "terminal_ai_assistant-3.0.1.tar", last modified: Mon May 27 16:45:03 2024, max compression
```

## Comparing `terminal_ai_assistant-3.0.0.tar` & `terminal_ai_assistant-3.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 07:30:10.766692 terminal_ai_assistant-3.0.0/
--rw-r--r--   0 ob907      (502) staff       (20)     2650 2024-05-27 07:30:10.766482 terminal_ai_assistant-3.0.0/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     2410 2024-05-27 07:24:47.000000 terminal_ai_assistant-3.0.0/README.md
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-27 07:30:10.766735 terminal_ai_assistant-3.0.0/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      465 2024-05-27 07:25:06.000000 terminal_ai_assistant-3.0.0/setup.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 07:30:10.765024 terminal_ai_assistant-3.0.0/tai/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 terminal_ai_assistant-3.0.0/tai/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     4191 2024-05-27 07:22:31.000000 terminal_ai_assistant-3.0.0/tai/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 07:30:10.766264 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2650 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      317 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-27 07:30:10.000000 terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/top_level.txt
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 16:45:03.891310 terminal_ai_assistant-3.0.1/
+-rw-r--r--   0 ob907      (502) staff       (20)     2636 2024-05-27 16:45:03.891082 terminal_ai_assistant-3.0.1/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2396 2024-05-27 07:42:48.000000 terminal_ai_assistant-3.0.1/README.md
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-27 16:45:03.891356 terminal_ai_assistant-3.0.1/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      465 2024-05-27 16:44:47.000000 terminal_ai_assistant-3.0.1/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 16:45:03.889602 terminal_ai_assistant-3.0.1/tai/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 terminal_ai_assistant-3.0.1/tai/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     4191 2024-05-27 16:44:24.000000 terminal_ai_assistant-3.0.1/tai/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 16:45:03.890851 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2636 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      317 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-27 16:45:03.000000 terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/top_level.txt
```

### Comparing `terminal_ai_assistant-3.0.0/PKG-INFO` & `terminal_ai_assistant-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-ai-assistant
-Version: 3.0.0
+Version: 3.0.1
 Summary: TAI [Terminal AI], a terminal AI assistant
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 <h1 align="center">TAI [Terminal AI], a terminal AI assistant</h1>
@@ -57,15 +57,14 @@
 export OPENAI_API_KEY={replace_me}
 ```
 
 You can use either of these commands
 
 ```bash
 $ tai <query>
-$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
 $ tai kill port 3000
```

### Comparing `terminal_ai_assistant-3.0.0/README.md` & `terminal_ai_assistant-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 export OPENAI_API_KEY={replace_me}
 ```
 
 You can use either of these commands
 
 ```bash
 $ tai <query>
-$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
 $ tai kill port 3000
```

### Comparing `terminal_ai_assistant-3.0.0/tai/cli.py` & `terminal_ai_assistant-3.0.1/tai/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def main():
     """Initializes the OpenAI client, and processes the query."""
 
     signal.signal(signal.SIGINT, handle_sigint)
 
     if len(sys.argv) < 2:
-        print("Usage: ask <query>")
+        print("Usage: tai <query>")
 
         sys.exit(1)
 
     query = " ".join(sys.argv[1:])
 
     try:
         client = get_openai_client()
```

### Comparing `terminal_ai_assistant-3.0.0/terminal_ai_assistant.egg-info/PKG-INFO` & `terminal_ai_assistant-3.0.1/terminal_ai_assistant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terminal-ai-assistant
-Version: 3.0.0
+Version: 3.0.1
 Summary: TAI [Terminal AI], a terminal AI assistant
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 <h1 align="center">TAI [Terminal AI], a terminal AI assistant</h1>
@@ -57,15 +57,14 @@
 export OPENAI_API_KEY={replace_me}
 ```
 
 You can use either of these commands
 
 ```bash
 $ tai <query>
-$ ask <query>
 ```
 
 Now you can use the executable
 
 ```bash
 $ tai kill port 3000
```

