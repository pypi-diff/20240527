# Comparing `tmp/cadziu-0.4.tar.gz` & `tmp/cadziu-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cadziu-0.4.tar", last modified: Sun May 26 12:33:16 2024, max compression
+gzip compressed data, was "cadziu-0.5.tar", last modified: Sun May 26 12:36:38 2024, max compression
```

## Comparing `cadziu-0.4.tar` & `cadziu-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.859789 cadziu-0.4/
--rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:33:16.855789 cadziu-0.4/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-26 12:11:59.000000 cadziu-0.4/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.843789 cadziu-0.4/app/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-26 12:32:11.000000 cadziu-0.4/app/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     1839 2024-05-26 12:32:42.000000 cadziu-0.4/app/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     2175 2024-05-26 12:32:50.000000 cadziu-0.4/app/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:33:16.851789 cadziu-0.4/cadziu.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      241 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       41 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       23 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 12:33:16.000000 cadziu-0.4/cadziu.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 12:33:16.859789 cadziu-0.4/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      802 2024-05-26 12:32:29.000000 cadziu-0.4/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:36:38.968236 cadziu-0.5/
+-rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:36:38.964236 cadziu-0.5/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-26 12:11:59.000000 cadziu-0.5/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:36:38.948236 cadziu-0.5/app/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-26 12:32:11.000000 cadziu-0.5/app/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2128 2024-05-26 12:36:11.000000 cadziu-0.5/app/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     2175 2024-05-26 12:36:21.000000 cadziu-0.5/app/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-26 12:36:38.960235 cadziu-0.5/cadziu.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      502 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      241 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       41 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       23 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        4 2024-05-26 12:36:38.000000 cadziu-0.5/cadziu.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-26 12:36:38.968236 cadziu-0.5/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      802 2024-05-26 12:36:33.000000 cadziu-0.5/setup.py
```

### Comparing `cadziu-0.4/app/main.py` & `cadziu-0.5/app/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 import os
 import sys
 import time
 from .utils import add_dns_record, is_resolvable, execute_docker_command
 from dotenv import load_dotenv
 
 def main():
-    load_dotenv()
+    # Load environment variables from the .env file in the current directory
+    load_dotenv(os.path.join(os.getcwd(), '.env'))
     
+    # Load environment variables from the home directory .env file
+    home = os.path.expanduser("~")
+    load_dotenv(os.path.join(home, '.env'))
+
     parser = argparse.ArgumentParser(description='Cadziu Command Line Tool')
     parser.add_argument('command', choices=['add'], help='Command to execute')
     parser.add_argument('subdomain', help='Subdomain to add')
     parser.add_argument('-p', '--port', required=True, help='Backend server port')
 
     args = parser.parse_args()
 
     if args.command == 'add':
         subdomain = args.subdomain
         port = args.port
         api_token = os.getenv('CLOUDFLARE_API_TOKEN')
         zone_id = os.getenv('CLOUDFLARE_ZONE_ID')
         
         if not api_token or not zone_id:
-            print("Error: CLOUDFLARE_API_TOKEN and CLOUDFLARE_ZONE_ID must be set in the .env file")
+            print("Error: CLOUDFLARE_API_TOKEN and CLOUDFLARE_ZONE_ID must be set in the environment variables or in the .env file")
             sys.exit(1)
 
         external_ip = "172.17.0.1"  # Docker network IP
 
         if add_dns_record(subdomain, external_ip, api_token, zone_id):
             for attempt in range(10):
                 if is_resolvable(subdomain):
```

### Comparing `cadziu-0.4/app/utils.py` & `cadziu-0.5/app/utils.py`

 * *Files identical despite different names*

### Comparing `cadziu-0.4/setup.py` & `cadziu-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cadziu',
-    version='0.4',
+    version='0.5',
     author='Your Name',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cadziu',
     packages=find_packages(),
```

