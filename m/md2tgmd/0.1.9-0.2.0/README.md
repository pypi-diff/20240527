# Comparing `tmp/md2tgmd-0.1.9.tar.gz` & `tmp/md2tgmd-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "md2tgmd-0.1.9.tar", last modified: Wed May  8 18:23:27 2024, max compression
+gzip compressed data, was "md2tgmd-0.2.0.tar", last modified: Mon May 27 04:35:29 2024, max compression
```

## Comparing `md2tgmd-0.1.9.tar` & `md2tgmd-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:23:27.297251 md2tgmd-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-08 18:23:17.000000 md2tgmd-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 18:23:27.297251 md2tgmd-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-08 18:23:17.000000 md2tgmd-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:23:27.297251 md2tgmd-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-08 18:23:17.000000 md2tgmd-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:23:27.297251 md2tgmd-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:23:27.297251 md2tgmd-0.1.9/src/md2tgmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-08 18:23:27.000000 md2tgmd-0.1.9/src/md2tgmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-08 18:23:27.000000 md2tgmd-0.1.9/src/md2tgmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:23:27.000000 md2tgmd-0.1.9/src/md2tgmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 18:23:27.000000 md2tgmd-0.1.9/src/md2tgmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-05-08 18:23:17.000000 md2tgmd-0.1.9/src/md2tgmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:35:29.710126 md2tgmd-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-27 04:35:22.000000 md2tgmd-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-27 04:35:29.710126 md2tgmd-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-27 04:35:22.000000 md2tgmd-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 04:35:29.710126 md2tgmd-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-27 04:35:22.000000 md2tgmd-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:35:29.710126 md2tgmd-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 04:35:29.710126 md2tgmd-0.2.0/src/md2tgmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-27 04:35:29.000000 md2tgmd-0.2.0/src/md2tgmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-27 04:35:29.000000 md2tgmd-0.2.0/src/md2tgmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 04:35:29.000000 md2tgmd-0.2.0/src/md2tgmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 04:35:29.000000 md2tgmd-0.2.0/src/md2tgmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-05-27 04:35:22.000000 md2tgmd-0.2.0/src/md2tgmd.py
```

### Comparing `md2tgmd-0.1.9/LICENSE` & `md2tgmd-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.9/PKG-INFO` & `md2tgmd-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.9
+Version: 0.2.0
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.9/README.md` & `md2tgmd-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `md2tgmd-0.1.9/src/md2tgmd.egg-info/PKG-INFO` & `md2tgmd-0.2.0/src/md2tgmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: md2tgmd
-Version: 0.1.9
+Version: 0.2.0
 Summary: md2tgmd is a Markdown to Telegram-specific-markdown converter.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # md2tgmd
 
 md2tgmd is a Markdown to [Telegram-specific-markdown](https://core.telegram.org/bots/api#formatting-options) converter.
```

### Comparing `md2tgmd-0.1.9/src/md2tgmd.py` & `md2tgmd-0.2.0/src/md2tgmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
 def escapeshape(text):
     return '▎*' + " ".join(text.split()[1:]) + '*'
 
 def escapeminus(text):
     return '\\' + text
 
+def escapeminus2(text):
+    return r'@->@'
+
 def escapebackquote(text):
     return r'\`\`'
 
 def escapebackquoteincode(text):
     return r'@->@'
 
 def escapeplus(text):
@@ -97,25 +100,30 @@
     text = re.sub(r"\@\<\-\-\@", '\)', text)
     text = re.sub(r"\@{3}(.*?)\@{3}\^{3}(.*?)\^{3}", '[\\1](\\2)', text)
     text = re.sub(r"~", '\~', text)
     text = re.sub(r">", '\>', text)
     text = replace_all(text, r"(^#+\s.+?$)|```[\D\d\s]+?```", escapeshape)
     text = re.sub(r"#", '\#', text)
     text = replace_all(text, r"(\+)|\n[\s]*-\s|```[\D\d\s]+?```|`[\D\d\s]*?`", escapeplus)
-    text = re.sub(r"\n{1,2}(\s*)-\s", '\n\n\\1• ', text)
     text = re.sub(r"\n{1,2}(\s*\d{1,2}\.\s)", '\n\n\\1', text)
+    # # 把 code block 以外的 - 替换掉
+    text = replace_all(text, r"```[\D\d\s]+?```|(-)", escapeminus2)
+    text = re.sub(r"-", '@<-@', text)
+    text = re.sub(r"\@\-\>\@", '-', text)
+
+    text = re.sub(r"\n{1,2}(\s*)-\s", '\n\n\\1• ', text)
+    text = re.sub(r"\@\<\-\@", '\-', text)
     text = replace_all(text, r"(-)|\n[\s]*-\s|```[\D\d\s]+?```|`[\D\d\s]*?`", escapeminus)
     text = re.sub(r"```([\D\d\s]+?)```", '@@@\\1@@@', text)
     # 把 code block 里面的`替换掉
     text = replace_all(text, r"\@\@\@[\s\d\D]+?\@\@\@|(`)", escapebackquoteincode)
     text = re.sub(r"`", '\`', text)
     text = re.sub(r"\@\<\@", '\`', text)
     text = re.sub(r"\@\-\>\@", '`', text)
 
-
     # text = replace_all(text, r"`.*?`{1,2}|(`)", escapebackquoteincode)
     # text = re.sub(r"`", '\`', text)
     # text = re.sub(r"\@\-\>\@", '`', text)
     # print(text)
 
     text = replace_all(text, r"(``)", escapebackquote)
     text = re.sub(r"\@{3}([\D\d\s]+?)\@{3}", '```\\1```', text)
@@ -164,14 +172,15 @@
 sudo apt install mesa-utils # 安装
 
 ```python
 
 # comment
 print("1.1\n")_
 \subsubsection{1.1}
+- item 1 -
 ```
 \subsubsection{1.1}
 
 And simple text `with-ten`  `with+ten` + some - **symbols**. # `with-ten`里面的`-`不会被转义
 
 
 ```
```

