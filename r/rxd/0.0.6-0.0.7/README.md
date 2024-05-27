# Comparing `tmp/rxd-0.0.6.tar.gz` & `tmp/rxd-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxd-0.0.6.tar", last modified: Mon May 27 00:15:27 2024, max compression
+gzip compressed data, was "rxd-0.0.7.tar", last modified: Mon May 27 00:20:08 2024, max compression
```

## Comparing `rxd-0.0.6.tar` & `rxd-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:15:27.948308 rxd-0.0.6/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:15:27.948067 rxd-0.0.6/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.6/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:15:27.944892 rxd-0.0.6/rxd/
--rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.6/rxd/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)     5935 2024-05-27 00:15:10.000000 rxd-0.0.6/rxd/app_manager.py
--rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.6/rxd/ask.py
--rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.6/rxd/cmd.py
--rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.6/rxd/cmd_app.py
--rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.6/rxd/cmd_responder.py
--rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.6/rxd/cmd_setup.py
--rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.6/rxd/cmd_worker_daemon.py
--rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.6/rxd/codex.py
--rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.6/rxd/messages.py
--rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.6/rxd/worker.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:15:27.947711 rxd-0.0.6/rxd.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/entry_points.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.6/rxd.egg-info/not-zip-safe
--rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/requires.txt
--rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-27 00:15:27.000000 rxd-0.0.6/rxd.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:15:27.948400 rxd-0.0.6/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-27 00:15:21.000000 rxd-0.0.6/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:20:08.421877 rxd-0.0.7/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:20:08.421487 rxd-0.0.7/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:51:53.000000 rxd-0.0.7/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:20:08.417243 rxd-0.0.7/rxd/
+-rw-r--r--   0 huy        (501) staff       (20)        0 2024-05-24 16:58:36.000000 rxd-0.0.7/rxd/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)     5882 2024-05-27 00:19:38.000000 rxd-0.0.7/rxd/app_manager.py
+-rwxr-xr-x   0 huy        (501) staff       (20)      410 2024-05-25 23:57:42.000000 rxd-0.0.7/rxd/ask.py
+-rw-r--r--   0 huy        (501) staff       (20)      939 2024-05-26 23:27:05.000000 rxd-0.0.7/rxd/cmd.py
+-rw-r--r--   0 huy        (501) staff       (20)     1815 2024-05-26 20:22:11.000000 rxd-0.0.7/rxd/cmd_app.py
+-rw-r--r--   0 huy        (501) staff       (20)     1148 2024-05-26 20:16:36.000000 rxd-0.0.7/rxd/cmd_responder.py
+-rw-r--r--   0 huy        (501) staff       (20)      358 2024-05-25 12:54:20.000000 rxd-0.0.7/rxd/cmd_setup.py
+-rw-r--r--   0 huy        (501) staff       (20)      111 2024-05-26 20:17:01.000000 rxd-0.0.7/rxd/cmd_worker_daemon.py
+-rw-r--r--   0 huy        (501) staff       (20)     2794 2024-05-25 22:31:16.000000 rxd-0.0.7/rxd/codex.py
+-rw-r--r--   0 huy        (501) staff       (20)      143 2024-05-26 16:11:09.000000 rxd-0.0.7/rxd/messages.py
+-rw-r--r--   0 huy        (501) staff       (20)      113 2024-05-25 23:36:37.000000 rxd-0.0.7/rxd/worker.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-27 00:20:08.420889 rxd-0.0.7/rxd.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)      294 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      386 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/entry_points.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-25 05:12:36.000000 rxd-0.0.7/rxd.egg-info/not-zip-safe
+-rw-r--r--   0 huy        (501) staff       (20)       12 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/requires.txt
+-rw-r--r--   0 huy        (501) staff       (20)        4 2024-05-27 00:20:08.000000 rxd-0.0.7/rxd.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-27 00:20:08.422636 rxd-0.0.7/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)      788 2024-05-27 00:19:54.000000 rxd-0.0.7/setup.py
```

### Comparing `rxd-0.0.6/rxd/app_manager.py` & `rxd-0.0.7/rxd/app_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,15 +152,14 @@
 
     def daemonize(self):
         screen_name = self.name
         python_path = sys.executable
         user = getpass.getuser()
         systemd_service_file = \
             f"""
-            # save this into /etc/systemd/system/rxd.service
             [Unit]
             Description=rxd
             After=network.target
             StartLimitIntervalSec=30
             StartLimitBurst=5
 
             [Service]
@@ -171,15 +170,15 @@
             RestartSec=5
 
             [Install]
             WantedBy=default.target
             """
         systemd_service_file = textwrap.dedent(systemd_service_file)
         systemd_service_install_path = Path(
-            f'/etc/systemd/system/{self.name}.service')
+            f'/etc/systemd/system/rxd-app-{self.name}.service')
         print(f'Writing {self.systemd_services_definition_path}')
         with open(self.systemd_services_definition_path, "w") as fh:
             fh.write(systemd_service_file)
 
         if Path('/etc/systemd/system').exists():
             if not systemd_service_install_path.exists():
```

### Comparing `rxd-0.0.6/rxd/cmd.py` & `rxd-0.0.7/rxd/cmd.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.6/rxd/cmd_app.py` & `rxd-0.0.7/rxd/cmd_app.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.6/rxd/cmd_responder.py` & `rxd-0.0.7/rxd/cmd_responder.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.6/rxd/codex.py` & `rxd-0.0.7/rxd/codex.py`

 * *Files identical despite different names*

### Comparing `rxd-0.0.6/setup.py` & `rxd-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='rxd',
-      version='0.0.6',
+      version='0.0.7',
       description='A reactive application manager',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Huy Nguyen',
       author_email='121183+huyng@users.noreply.github.com',
       packages=['rxd'],
       entry_points={
```

