# Comparing `tmp/lfg_llama-2.2.3.tar.gz` & `tmp/lfg_llama-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-2.2.3.tar", last modified: Tue May 21 19:29:31 2024, max compression
+gzip compressed data, was "lfg_llama-2.3.0.tar", last modified: Mon May 27 05:20:23 2024, max compression
```

## Comparing `lfg_llama-2.2.3.tar` & `lfg_llama-2.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.910034 lfg_llama-2.2.3/
--rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:29:31.909832 lfg_llama-2.2.3/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     2287 2024-05-21 19:24:54.000000 lfg_llama-2.2.3/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.908555 lfg_llama-2.2.3/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.2.3/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     2981 2024-05-21 19:27:49.000000 lfg_llama-2.2.3/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-21 19:29:31.909587 lfg_llama-2.2.3/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     2526 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-21 19:29:31.000000 lfg_llama-2.2.3/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-21 19:29:31.910086 lfg_llama-2.2.3/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-21 19:29:14.000000 lfg_llama-2.2.3/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 05:20:23.964317 lfg_llama-2.3.0/
+-rw-r--r--   0 ob907      (502) staff       (20)     2464 2024-05-27 05:20:23.964111 lfg_llama-2.3.0/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     2225 2024-05-27 05:19:10.000000 lfg_llama-2.3.0/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 05:20:23.962355 lfg_llama-2.3.0/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.3.0/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     4191 2024-05-27 05:13:39.000000 lfg_llama-2.3.0/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-27 05:20:23.963809 lfg_llama-2.3.0/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2464 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       56 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        7 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-27 05:20:23.000000 lfg_llama-2.3.0/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-27 05:20:23.964372 lfg_llama-2.3.0/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      484 2024-05-27 05:06:43.000000 lfg_llama-2.3.0/setup.py
```

### Comparing `lfg_llama-2.2.3/PKG-INFO` & `lfg_llama-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-Metadata-Version: 2.1
-Name: lfg-llama
-Version: 2.2.3
-Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
-Author: Bjarne Oeverli
-Author-email: bjarneocodes@gmail.com
-Description-Content-Type: text/markdown
-Requires-Dist: openai
-
 <div align="center">
   <img src="logo.png" alt="logo" />
 </div>
 
 <h1 align="center">LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙</h1>
 
 <div align="center">
   LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 </div>
 <br />
 
 ![Demo](example.png)
 
-## Why?
+## What?
 
-- Firstly, this was created to test Ollama -> Groq
-- I do not like the Github Copilot command-line
+- I do not like the syntax of the Github Copilot command-line
 - Quicker than using Gemini/ChatGPT/Google directly via the browser interface
 - Easier to find what needed without opening man pages
 - NEW: Changing to GPT-4o model which is free
+- NEW: Execute the command directly from this CLI
 
 However, never trust the output entirely.
 
 ## Installation
 
 ```bash
 # install pipx
@@ -71,28 +62,30 @@
 fuser -k 3000/tcp
 
 Explanation:
 The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
 ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
 any process currently using port 3000.
 
+> Execute the command? (N/y):
 ```
 
 Change the LLM
 
 ```bash
-$ ask list ec2 pipe json jq get name
+$ ask get pods from all namespaces
+
+kubectl get pods --all-namespaces
 
-aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
- --output json | jq -r '.[].Name'
 
 Explanation:
-This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
-ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
-, and `jq` is used to parse and extract the 'Name' values.%
+The `kubectl get pods --all-namespaces` command lists all the pods across all namespaces in a Kuber
+netes cluster. The `--all-namespaces` flag is used to fetch the pods from every namespace instead of the default namespace.
+
+> Execute the command? (N/y):
 ```
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
```

### Comparing `lfg_llama-2.2.3/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 2.2.3
+Version: 2.3.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: openai
 
 <div align="center">
@@ -16,21 +16,21 @@
 <div align="center">
   LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 </div>
 <br />
 
 ![Demo](example.png)
 
-## Why?
+## What?
 
-- Firstly, this was created to test Ollama -> Groq
-- I do not like the Github Copilot command-line
+- I do not like the syntax of the Github Copilot command-line
 - Quicker than using Gemini/ChatGPT/Google directly via the browser interface
 - Easier to find what needed without opening man pages
 - NEW: Changing to GPT-4o model which is free
+- NEW: Execute the command directly from this CLI
 
 However, never trust the output entirely.
 
 ## Installation
 
 ```bash
 # install pipx
@@ -71,28 +71,30 @@
 fuser -k 3000/tcp
 
 Explanation:
 The `fuser` command identifies processes using files or sockets. The `-k` option is used to kill th
 ose processes. Here, `3000/tcp` specifies the TCP port number 3000. This command effectively kills
 any process currently using port 3000.
 
+> Execute the command? (N/y):
 ```
 
 Change the LLM
 
 ```bash
-$ ask list ec2 pipe json jq get name
+$ ask get pods from all namespaces
+
+kubectl get pods --all-namespaces
 
-aws ec2 describe-instances --query "Reservations[].Instances[].{Name:Tags[?Key=='Name']|[0].Value}"
- --output json | jq -r '.[].Name'
 
 Explanation:
-This command uses the AWS CLI to list EC2 instances and their corresponding 'Name' tag values in JS
-ON format. The `--query` option filters the output to only include the 'Name' tag for each instance
-, and `jq` is used to parse and extract the 'Name' values.%
+The `kubectl get pods --all-namespaces` command lists all the pods across all namespaces in a Kuber
+netes cluster. The `--all-namespaces` flag is used to fetch the pods from every namespace instead of the default namespace.
+
+> Execute the command? (N/y):
 ```
 
 ### Development
 
 ```bash
 pip install --user pipenv
 pipenv --python 3.11
```

