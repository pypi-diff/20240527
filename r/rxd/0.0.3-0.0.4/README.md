# Comparing `tmp/rxd-0.0.3.tar.gz` & `tmp/rxd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxd-0.0.3.tar", last modified: Sun May 26 23:34:46 2024, max compression
+gzip compressed data, was "rxd-0.0.4.tar", last modified: Sun May 26 23:40:41 2024, max compression
```

## Comparing `rxd-0.0.3.tar` & `rxd-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.373052 rxd-0.0.3/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:34:46.372737 rxd-0.0.3/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.3/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.368097 rxd-0.0.3/rxd/
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.3/rxd/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     5733 2024-05-26 21:17:07.000000 rxd-0.0.3/rxd/app_manager.py
--rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.3/rxd/ask.py
--rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.3/rxd/cmd.py
--rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.3/rxd/cmd_app.py
--rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.3/rxd/cmd_responder.py
--rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.3/rxd/cmd_setup.py
--rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.3/rxd/cmd_worker_daemon.py
--rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.3/rxd/codex.py
--rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.3/rxd/messages.py
--rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.3/rxd/worker.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:34:46.372058 rxd-0.0.3/rxd.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.3/rxd.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-26 23:34:46.000000 rxd-0.0.3/rxd.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:34:46.373252 rxd-0.0.3/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-26 22:11:27.000000 rxd-0.0.3/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:40:41.718421 rxd-0.0.4/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:40:41.718049 rxd-0.0.4/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.4/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:40:41.713393 rxd-0.0.4/rxd/
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.4/rxd/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5721 2024-05-26 23:40:23.000000 rxd-0.0.4/rxd/app_manager.py
+-rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.4/rxd/ask.py
+-rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.4/rxd/cmd.py
+-rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.4/rxd/cmd_app.py
+-rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.4/rxd/cmd_responder.py
+-rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.4/rxd/cmd_setup.py
+-rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.4/rxd/cmd_worker_daemon.py
+-rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.4/rxd/codex.py
+-rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.4/rxd/messages.py
+-rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.4/rxd/worker.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-26 23:40:41.717042 rxd-0.0.4/rxd.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.4/rxd.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-26 23:40:41.000000 rxd-0.0.4/rxd.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-26 23:40:41.718922 rxd-0.0.4/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-26 23:40:35.000000 rxd-0.0.4/setup.py
```

### Comparing `rxd-0.0.3/rxd/app_manager.py` & `rxd-0.0.4/rxd/app_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,16 +167,15 @@
             Restart=always
             RestartSec=5
 
             [Install]
             WantedBy=default.target
             """
         systemd_service_file = textwrap.dedent(systemd_service_file)
-        systemd_service_install_path = Path(
-            '/etc/systemd/system/{self.name}.service')
+        systemd_service_install_path = Path(f'/etc/systemd/system/{self.name}.service')
         print(f'Writing {self.systemd_services_definition_path}')
         with open(self.systemd_services_definition_path, "w") as fh:
             fh.write(systemd_service_file)
 
         if Path('/etc/systemd/system').exists():
             if not systemd_service_install_path.exists():
                 print("Symlinking %s -> %s" % (systemd_service_install_path,
```

### Comparing `rxd-0.0.3/rxd/cmd.py` & `rxd-0.0.4/rxd/cmd.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.3/rxd/cmd_app.py` & `rxd-0.0.4/rxd/cmd_app.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.3/rxd/cmd_responder.py` & `rxd-0.0.4/rxd/cmd_responder.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.3/rxd/codex.py` & `rxd-0.0.4/rxd/codex.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.3/setup.py` & `rxd-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='rxd',
-      version='0.0.3',
+      version='0.0.4',
       description='A reactive application manager',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['rxd'],
       entry_points={
```
