# Comparing `tmp/markdown_text_clean-1.0.2.tar.gz` & `tmp/markdown_text_clean-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_text_clean-1.0.2.tar", last modified: Thu May 23 04:44:21 2024, max compression
+gzip compressed data, was "markdown_text_clean-1.0.3.tar", last modified: Mon May 27 04:49:39 2024, max compression
```

## Comparing `markdown_text_clean-1.0.2.tar` & `markdown_text_clean-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 04:44:21.511555 markdown_text_clean-1.0.2/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     2115 2024-05-23 04:44:21.511362 markdown_text_clean-1.0.2/PKG-INFO
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     1590 2024-05-23 04:44:12.000000 markdown_text_clean-1.0.2/README.md
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 04:44:21.506411 markdown_text_clean-1.0.2/markdown_text_clean/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       34 2024-05-22 15:41:03.000000 markdown_text_clean-1.0.2/markdown_text_clean/__init__.py
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      540 2024-05-22 15:40:51.000000 markdown_text_clean-1.0.2/markdown_text_clean/text_clean.py
-drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-23 04:44:21.511007 markdown_text_clean-1.0.2/markdown_text_clean.egg-info/
--rw-r--r--   0 yoshiiakane   (501) staff       (20)     2115 2024-05-23 04:44:21.000000 markdown_text_clean-1.0.2/markdown_text_clean.egg-info/PKG-INFO
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      256 2024-05-23 04:44:21.000000 markdown_text_clean-1.0.2/markdown_text_clean.egg-info/SOURCES.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)        1 2024-05-23 04:44:21.000000 markdown_text_clean-1.0.2/markdown_text_clean.egg-info/dependency_links.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       20 2024-05-23 04:44:21.000000 markdown_text_clean-1.0.2/markdown_text_clean.egg-info/top_level.txt
--rw-r--r--   0 yoshiiakane   (501) staff       (20)       38 2024-05-23 04:44:21.511646 markdown_text_clean-1.0.2/setup.cfg
--rw-r--r--   0 yoshiiakane   (501) staff       (20)      537 2024-05-23 04:43:54.000000 markdown_text_clean-1.0.2/setup.py
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-27 04:49:39.218012 markdown_text_clean-1.0.3/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     2214 2024-05-27 04:49:39.217821 markdown_text_clean-1.0.3/PKG-INFO
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     1590 2024-05-23 04:44:12.000000 markdown_text_clean-1.0.3/README.md
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-27 04:49:39.214340 markdown_text_clean-1.0.3/markdown_text_clean/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       34 2024-05-22 15:41:03.000000 markdown_text_clean-1.0.3/markdown_text_clean/__init__.py
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      540 2024-05-22 15:40:51.000000 markdown_text_clean-1.0.3/markdown_text_clean/text_clean.py
+drwxr-xr-x   0 yoshiiakane   (501) staff       (20)        0 2024-05-27 04:49:39.217498 markdown_text_clean-1.0.3/markdown_text_clean.egg-info/
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)     2214 2024-05-27 04:49:38.000000 markdown_text_clean-1.0.3/markdown_text_clean.egg-info/PKG-INFO
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      256 2024-05-27 04:49:39.000000 markdown_text_clean-1.0.3/markdown_text_clean.egg-info/SOURCES.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)        1 2024-05-27 04:49:38.000000 markdown_text_clean-1.0.3/markdown_text_clean.egg-info/dependency_links.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       20 2024-05-27 04:49:38.000000 markdown_text_clean-1.0.3/markdown_text_clean.egg-info/top_level.txt
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)       38 2024-05-27 04:49:39.218106 markdown_text_clean-1.0.3/setup.cfg
+-rw-r--r--   0 yoshiiakane   (501) staff       (20)      667 2024-05-27 04:49:12.000000 markdown_text_clean-1.0.3/setup.py
```

### Comparing `markdown_text_clean-1.0.2/PKG-INFO` & `markdown_text_clean-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: markdown_text_clean
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to clean markdown text
-Home-page: UNKNOWN
+Home-page: https://github.com/pompom7776/markdown-text-clean
+Author: pom
+Author-email: s2222059@stu.musashino-u.ac.jp
 License: UNKNOWN
 Description: # 概要 (Overview)
         
         markdown-text-clean is a Python library that cleans up text by removing Markdown formatting such as bold, italic, inline code, and strikethrough.
         
         markdown-text-cleanは、太字、斜体、インラインコード、取り消し線などのマークダウン書式を削除してテキストをきれいにするPythonライブラリです。
```

### Comparing `markdown_text_clean-1.0.2/README.md` & `markdown_text_clean-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `markdown_text_clean-1.0.2/markdown_text_clean/text_clean.py` & `markdown_text_clean-1.0.3/markdown_text_clean/text_clean.py`

 * *Files identical despite different names*

### Comparing `markdown_text_clean-1.0.2/markdown_text_clean.egg-info/PKG-INFO` & `markdown_text_clean-1.0.3/markdown_text_clean.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: markdown-text-clean
-Version: 1.0.2
+Version: 1.0.3
 Summary: A package to clean markdown text
-Home-page: UNKNOWN
+Home-page: https://github.com/pompom7776/markdown-text-clean
+Author: pom
+Author-email: s2222059@stu.musashino-u.ac.jp
 License: UNKNOWN
 Description: # 概要 (Overview)
         
         markdown-text-clean is a Python library that cleans up text by removing Markdown formatting such as bold, italic, inline code, and strikethrough.
         
         markdown-text-cleanは、太字、斜体、インラインコード、取り消し線などのマークダウン書式を削除してテキストをきれいにするPythonライブラリです。
```

### Comparing `markdown_text_clean-1.0.2/setup.py` & `markdown_text_clean-1.0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="markdown_text_clean",
-    version="1.0.2",
+    version="1.0.3",
     LICENSE = 'MIT',
+    author="pom",
+    author_email="s2222059@stu.musashino-u.ac.jp",
     description="A package to clean markdown text",
     long_description=long_description,
     long_description_content_type="text/markdown", 
+    url="https://github.com/pompom7776/markdown-text-clean",
     packages=find_packages(),
     CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6'
     ],
 )
```

