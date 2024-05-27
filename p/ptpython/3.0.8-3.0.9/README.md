# Comparing `tmp/ptpython-3.0.8.tar.gz` & `tmp/ptpython-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ptpython-3.0.8.tar", last modified: Tue Jan  5 09:53:34 2021, max compression
+gzip compressed data, was "dist/ptpython-3.0.9.tar", last modified: Fri Jan  8 11:41:27 2021, max compression
```

## Comparing `ptpython-3.0.8.tar` & `ptpython-3.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.211146 ptpython-3.0.8/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      675 2020-01-12 17:01:50.000000 ptpython-3.0.8/.gitignore
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      572 2021-01-05 08:50:24.000000 ptpython-3.0.8/.travis.yml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9768 2021-01-05 09:52:04.000000 ptpython-3.0.8/CHANGELOG
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1493 2020-01-12 17:01:50.000000 ptpython-3.0.8/LICENSE
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      104 2020-01-12 17:01:50.000000 ptpython-3.0.8/MANIFEST.in
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9731 2021-01-05 09:53:34.211146 ptpython-3.0.8/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7192 2021-01-05 08:51:29.000000 ptpython-3.0.8/README.rst
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.179146 ptpython-3.0.8/docs/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.195146 ptpython-3.0.8/docs/images/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/example1.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    37364 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/file-completion.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    36967 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/ipython.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    33129 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/multiline.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   103337 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/ptpython-history-help.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    60225 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/ptpython-menu.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/ptpython.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17124 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/validation.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18368 2020-01-12 17:01:50.000000 ptpython-3.0.8/docs/images/windows.png
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.199146 ptpython-3.0.8/examples/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1508 2021-01-05 08:51:29.000000 ptpython-3.0.8/examples/asyncio-python-embed.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1416 2020-01-29 21:23:48.000000 ptpython-3.0.8/examples/asyncio-ssh-python-embed.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.199146 ptpython-3.0.8/examples/ptpython_config/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6307 2021-01-05 08:51:29.000000 ptpython-3.0.8/examples/ptpython_config/config.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1063 2020-09-14 23:27:10.000000 ptpython-3.0.8/examples/python-embed-with-custom-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      162 2020-09-14 23:27:10.000000 ptpython-3.0.8/examples/python-embed.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      217 2020-09-14 23:27:10.000000 ptpython-3.0.8/examples/python-input.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1392 2020-09-23 18:00:44.000000 ptpython-3.0.8/examples/ssh-and-telnet-embed.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.207146 ptpython-3.0.8/ptpython/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.8/ptpython/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      119 2020-01-29 21:23:48.000000 ptpython-3.0.8/ptpython/__main__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21081 2021-01-05 08:51:29.000000 ptpython-3.0.8/ptpython/completer.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.211146 ptpython-3.0.8/ptpython/contrib/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.8/ptpython/contrib/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3902 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/contrib/asyncssh_repl.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.211146 ptpython-3.0.8/ptpython/entry_points/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.8/ptpython/entry_points/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2363 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/entry_points/run_ptipython.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6740 2021-01-05 08:51:29.000000 ptpython-3.0.8/ptpython/entry_points/run_ptpython.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2252 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/eventloop.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      903 2020-01-29 21:23:48.000000 ptpython-3.0.8/ptpython/filters.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21649 2021-01-04 17:20:35.000000 ptpython-3.0.8/ptpython/history_browser.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9250 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/ipython.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9492 2020-09-23 18:00:44.000000 ptpython-3.0.8/ptpython/key_bindings.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    27934 2021-01-05 09:47:44.000000 ptpython-3.0.8/ptpython/layout.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1996 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/prompt_style.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    39405 2021-01-05 09:47:44.000000 ptpython-3.0.8/ptpython/python_input.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18463 2021-01-05 09:47:44.000000 ptpython-3.0.8/ptpython/repl.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6522 2021-01-05 09:47:44.000000 ptpython-3.0.8/ptpython/style.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4691 2021-01-05 08:51:29.000000 ptpython-3.0.8/ptpython/utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1855 2020-09-14 23:27:10.000000 ptpython-3.0.8/ptpython/validator.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.211146 ptpython-3.0.8/ptpython.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9731 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1290 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      333 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/entry_points.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      132 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        9 2021-01-05 09:53:34.000000 ptpython-3.0.8/ptpython.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      305 2020-01-29 21:23:48.000000 ptpython-3.0.8/pyproject.toml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       67 2021-01-05 09:53:34.211146 ptpython-3.0.8/setup.cfg
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1701 2021-01-05 09:52:19.000000 ptpython-3.0.8/setup.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:53:34.211146 ptpython-3.0.8/tests/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      545 2020-01-29 21:23:48.000000 ptpython-3.0.8/tests/run_tests.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      675 2020-01-12 17:01:50.000000 ptpython-3.0.9/.gitignore
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      572 2021-01-05 08:50:24.000000 ptpython-3.0.9/.travis.yml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9949 2021-01-08 11:40:19.000000 ptpython-3.0.9/CHANGELOG
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1493 2020-01-12 17:01:50.000000 ptpython-3.0.9/LICENSE
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      104 2020-01-12 17:01:50.000000 ptpython-3.0.9/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9731 2021-01-08 11:41:27.914895 ptpython-3.0.9/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7192 2021-01-05 09:55:00.000000 ptpython-3.0.9/README.rst
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.898895 ptpython-3.0.9/docs/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.906895 ptpython-3.0.9/docs/images/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/example1.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    37364 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/file-completion.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    36967 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/ipython.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    33129 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/multiline.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   103337 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/ptpython-history-help.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    60225 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/ptpython-menu.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/ptpython.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17124 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/validation.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18368 2020-01-12 17:01:50.000000 ptpython-3.0.9/docs/images/windows.png
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.906895 ptpython-3.0.9/examples/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1508 2021-01-05 09:55:00.000000 ptpython-3.0.9/examples/asyncio-python-embed.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1416 2020-01-29 21:23:48.000000 ptpython-3.0.9/examples/asyncio-ssh-python-embed.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.906895 ptpython-3.0.9/examples/ptpython_config/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6307 2021-01-05 09:55:00.000000 ptpython-3.0.9/examples/ptpython_config/config.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1063 2021-01-08 11:41:03.000000 ptpython-3.0.9/examples/python-embed-with-custom-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      162 2020-09-14 23:27:10.000000 ptpython-3.0.9/examples/python-embed.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      217 2020-09-14 23:27:10.000000 ptpython-3.0.9/examples/python-input.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1392 2020-09-23 18:00:44.000000 ptpython-3.0.9/examples/ssh-and-telnet-embed.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/ptpython/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.9/ptpython/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      119 2020-01-29 21:23:48.000000 ptpython-3.0.9/ptpython/__main__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21081 2021-01-05 09:55:00.000000 ptpython-3.0.9/ptpython/completer.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/ptpython/contrib/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.9/ptpython/contrib/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3902 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/contrib/asyncssh_repl.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/ptpython/entry_points/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:50.000000 ptpython-3.0.9/ptpython/entry_points/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2363 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/entry_points/run_ptipython.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6740 2021-01-05 09:55:00.000000 ptpython-3.0.9/ptpython/entry_points/run_ptpython.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2252 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/eventloop.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      903 2020-01-29 21:23:48.000000 ptpython-3.0.9/ptpython/filters.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21649 2021-01-04 17:20:35.000000 ptpython-3.0.9/ptpython/history_browser.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9250 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/ipython.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9492 2020-09-23 18:00:44.000000 ptpython-3.0.9/ptpython/key_bindings.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    27934 2021-01-05 09:55:00.000000 ptpython-3.0.9/ptpython/layout.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1996 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/prompt_style.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    39467 2021-01-08 11:39:54.000000 ptpython-3.0.9/ptpython/python_input.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18689 2021-01-08 11:39:54.000000 ptpython-3.0.9/ptpython/repl.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6522 2021-01-05 09:55:00.000000 ptpython-3.0.9/ptpython/style.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4691 2021-01-05 09:55:00.000000 ptpython-3.0.9/ptpython/utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1855 2020-09-14 23:27:10.000000 ptpython-3.0.9/ptpython/validator.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/ptpython.egg-info/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9731 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1290 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      333 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/entry_points.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      132 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        9 2021-01-08 11:41:27.000000 ptpython-3.0.9/ptpython.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      305 2020-01-29 21:23:48.000000 ptpython-3.0.9/pyproject.toml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       67 2021-01-08 11:41:27.914895 ptpython-3.0.9/setup.cfg
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1701 2021-01-08 11:40:19.000000 ptpython-3.0.9/setup.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-08 11:41:27.914895 ptpython-3.0.9/tests/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      545 2020-01-29 21:23:48.000000 ptpython-3.0.9/tests/run_tests.py
```

### Comparing `ptpython-3.0.8/.gitignore` & `ptpython-3.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/.travis.yml` & `ptpython-3.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/CHANGELOG` & `ptpython-3.0.9/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGELOG
 =========
 
+3.0.9: 2020-01-10
+-----------------
+
+New features:
+- Allow replacing `PythonInput.completer` at runtime (useful for tools build on
+  top of ptpython).
+- Show REPL title in pager.
+
+
 3.0.8: 2020-01-05
 -----------------
 
 New features:
 - Optional output formatting using Black.
 - Optional pager for displaying outputs that don't fit on the screen.
 - Added --light-bg and --dark-bg flags to automatically optimize the brightness
```

### Comparing `ptpython-3.0.8/LICENSE` & `ptpython-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/PKG-INFO` & `ptpython-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptpython
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python REPL build on top of prompt_toolkit
 Home-page: https://github.com/prompt-toolkit/ptpython
 Author: Jonathan Slenders
 License: UNKNOWN
 Description: ptpython
         ========
```

### Comparing `ptpython-3.0.8/README.rst` & `ptpython-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/example1.png` & `ptpython-3.0.9/docs/images/example1.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/file-completion.png` & `ptpython-3.0.9/docs/images/file-completion.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/ipython.png` & `ptpython-3.0.9/docs/images/ipython.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/multiline.png` & `ptpython-3.0.9/docs/images/multiline.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/ptpython-history-help.png` & `ptpython-3.0.9/docs/images/ptpython-history-help.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/ptpython-menu.png` & `ptpython-3.0.9/docs/images/ptpython-menu.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/ptpython.png` & `ptpython-3.0.9/docs/images/ptpython.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/validation.png` & `ptpython-3.0.9/docs/images/validation.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/docs/images/windows.png` & `ptpython-3.0.9/docs/images/windows.png`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/examples/asyncio-python-embed.py` & `ptpython-3.0.9/examples/asyncio-python-embed.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/examples/asyncio-ssh-python-embed.py` & `ptpython-3.0.9/examples/asyncio-ssh-python-embed.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/examples/ptpython_config/config.py` & `ptpython-3.0.9/examples/ptpython_config/config.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/examples/python-embed-with-custom-prompt.py` & `ptpython-3.0.9/examples/python-embed-with-custom-prompt.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/examples/ssh-and-telnet-embed.py` & `ptpython-3.0.9/examples/ssh-and-telnet-embed.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/completer.py` & `ptpython-3.0.9/ptpython/completer.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/contrib/asyncssh_repl.py` & `ptpython-3.0.9/ptpython/contrib/asyncssh_repl.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/entry_points/run_ptipython.py` & `ptpython-3.0.9/ptpython/entry_points/run_ptipython.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/entry_points/run_ptpython.py` & `ptpython-3.0.9/ptpython/entry_points/run_ptpython.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/eventloop.py` & `ptpython-3.0.9/ptpython/eventloop.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/filters.py` & `ptpython-3.0.9/ptpython/filters.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/history_browser.py` & `ptpython-3.0.9/ptpython/history_browser.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/ipython.py` & `ptpython-3.0.9/ptpython/ipython.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/key_bindings.py` & `ptpython-3.0.9/ptpython/key_bindings.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/layout.py` & `ptpython-3.0.9/ptpython/layout.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/prompt_style.py` & `ptpython-3.0.9/ptpython/prompt_style.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/python_input.py` & `ptpython-3.0.9/ptpython/python_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 from prompt_toolkit.application import Application, get_app
 from prompt_toolkit.auto_suggest import (
     AutoSuggestFromHistory,
     ConditionalAutoSuggest,
     ThreadedAutoSuggest,
 )
 from prompt_toolkit.buffer import Buffer
-from prompt_toolkit.completion import Completer, FuzzyCompleter, ThreadedCompleter
+from prompt_toolkit.completion import (
+    Completer,
+    DynamicCompleter,
+    FuzzyCompleter,
+    ThreadedCompleter,
+)
 from prompt_toolkit.document import Document
 from prompt_toolkit.enums import DEFAULT_BUFFER, EditingMode
 from prompt_toolkit.filters import Condition
 from prompt_toolkit.formatted_text import AnyFormattedText
 from prompt_toolkit.history import (
     FileHistory,
     History,
@@ -187,22 +192,23 @@
         _extra_toolbars=None,
         _input_buffer_height=None,
     ) -> None:
 
         self.get_globals: _GetNamespace = get_globals or (lambda: {})
         self.get_locals: _GetNamespace = get_locals or self.get_globals
 
+        self.completer = _completer or PythonCompleter(
+            self.get_globals,
+            self.get_locals,
+            lambda: self.enable_dictionary_completion,
+        )
+
         self._completer = HidePrivateCompleter(
-            _completer
-            or FuzzyCompleter(
-                PythonCompleter(
-                    self.get_globals,
-                    self.get_locals,
-                    lambda: self.enable_dictionary_completion,
-                ),
+            FuzzyCompleter(
+                DynamicCompleter(lambda: self.completer),
                 enable_fuzzy=Condition(lambda: self.enable_fuzzy_completion),
             ),
             lambda: self.complete_private_attributes,
         )
         self._validator = _validator or PythonValidator(self.get_compiler_flags)
         self._lexer = _lexer or PygmentsLexer(PythonLexer)
```

### Comparing `ptpython-3.0.8/ptpython/repl.py` & `ptpython-3.0.9/ptpython/repl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from enum import Enum
 from typing import Any, Callable, ContextManager, Dict, Optional
 
 import black
 from prompt_toolkit.document import Document
 from prompt_toolkit.formatted_text import (
     HTML,
+    AnyFormattedText,
     FormattedText,
     PygmentsTokens,
     StyleAndTextTuples,
     fragment_list_width,
     merge_formatted_text,
     to_formatted_text,
 )
@@ -334,15 +335,15 @@
 
         flush_page()
 
     def create_pager_prompt(self) -> PromptSession["PagerResult"]:
         """
         Create pager --MORE-- prompt.
         """
-        return create_pager_prompt(self._current_style)
+        return create_pager_prompt(self._current_style, self.title)
 
     def _handle_exception(self, e: Exception) -> None:
         output = self.app.output
 
         # Instead of just calling ``traceback.format_exc``, we take the
         # traceback and skip the bottom calls of this framework.
         t, v, tb = sys.exc_info()
@@ -524,15 +525,17 @@
 
 class PagerResult(Enum):
     ABORT = "ABORT"
     NEXT_LINE = "NEXT_LINE"
     NEXT_PAGE = "NEXT_PAGE"
 
 
-def create_pager_prompt(style: BaseStyle) -> PromptSession[PagerResult]:
+def create_pager_prompt(
+    style: BaseStyle, title: AnyFormattedText = ""
+) -> PromptSession[PagerResult]:
     """
     Create a "continue" prompt for paginated output.
     """
     bindings = KeyBindings()
 
     @bindings.add("enter")
     @bindings.add("down")
@@ -554,20 +557,25 @@
     def _(event: KeyPressEvent) -> None:
         " Disallow inserting other text. "
         pass
 
     style
 
     session: PromptSession[PagerResult] = PromptSession(
-        HTML(
-            "<status-toolbar>"
-            "<more> -- MORE -- </more> "
-            "<key>[Enter]</key> Scroll "
-            "<key>[Space]</key> Next page "
-            "<key>[q]</key> Quit "
-            "</status-toolbar>: "
+        merge_formatted_text(
+            [
+                title,
+                HTML(
+                    "<status-toolbar>"
+                    "<more> -- MORE -- </more> "
+                    "<key>[Enter]</key> Scroll "
+                    "<key>[Space]</key> Next page "
+                    "<key>[q]</key> Quit "
+                    "</status-toolbar>: "
+                ),
+            ]
         ),
         key_bindings=bindings,
         erase_when_done=True,
         style=style,
     )
     return session
```

### Comparing `ptpython-3.0.8/ptpython/style.py` & `ptpython-3.0.9/ptpython/style.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/utils.py` & `ptpython-3.0.9/ptpython/utils.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython/validator.py` & `ptpython-3.0.9/ptpython/validator.py`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/ptpython.egg-info/PKG-INFO` & `ptpython-3.0.9/ptpython.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptpython
-Version: 3.0.8
+Version: 3.0.9
 Summary: Python REPL build on top of prompt_toolkit
 Home-page: https://github.com/prompt-toolkit/ptpython
 Author: Jonathan Slenders
 License: UNKNOWN
 Description: ptpython
         ========
```

### Comparing `ptpython-3.0.8/ptpython.egg-info/SOURCES.txt` & `ptpython-3.0.9/ptpython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ptpython-3.0.8/setup.py` & `ptpython-3.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.dirname(__file__), "README.rst")) as f:
     long_description = f.read()
 
 
 setup(
     name="ptpython",
     author="Jonathan Slenders",
-    version="3.0.8",
+    version="3.0.9",
     url="https://github.com/prompt-toolkit/ptpython",
     description="Python REPL build on top of prompt_toolkit",
     long_description=long_description,
     packages=find_packages("."),
     install_requires=[
         "appdirs",
         "importlib_metadata;python_version<'3.8'",
```

### Comparing `ptpython-3.0.8/tests/run_tests.py` & `ptpython-3.0.9/tests/run_tests.py`

 * *Files identical despite different names*

