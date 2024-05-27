# Comparing `tmp/abeewayconfig-0.2.3.tar.gz` & `tmp/abeewayconfig-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.3.tar", last modified: Fri May 24 13:18:18 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.5.tar", last modified: Mon May 27 18:49:18 2024, max compression
```

## Comparing `abeewayconfig-0.2.3.tar` & `abeewayconfig-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-24 13:18:18.802612 abeewayconfig-0.2.3/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    35149 2024-05-19 01:48:12.000000 abeewayconfig-0.2.3/LICENSE
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1717 2024-05-24 13:18:18.802612 abeewayconfig-0.2.3/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1307 2024-05-23 03:01:08.000000 abeewayconfig-0.2.3/README.md
--rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2024-05-24 13:18:18.805946 abeewayconfig-0.2.3/setup.cfg
--rw-r--r--   0 lucas     (1000) lucas     (1000)      869 2024-05-24 13:17:31.000000 abeewayconfig-0.2.3/setup.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-24 13:18:18.802612 abeewayconfig-0.2.3/src/
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-24 13:18:18.802612 abeewayconfig-0.2.3/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     7833 2024-05-24 13:13:58.000000 abeewayconfig-0.2.3/src/AbeewayConfig/CSVFile.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3492 2024-05-24 00:55:56.000000 abeewayconfig-0.2.3/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2906 2024-05-24 01:22:59.000000 abeewayconfig-0.2.3/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)       32 2024-05-19 01:48:12.000000 abeewayconfig-0.2.3/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     6230 2024-05-24 13:15:25.000000 abeewayconfig-0.2.3/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4026 2024-05-19 01:48:12.000000 abeewayconfig-0.2.3/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-24 13:18:18.802612 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1717 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)      463 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)      121 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       21 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       14 2024-05-24 13:18:18.000000 abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.5/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1321 2024-05-27 17:40:44.000000 abeewayconfig-0.2.5/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      801 2024-05-27 18:48:55.000000 abeewayconfig-0.2.5/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.067961 abeewayconfig-0.2.5/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.067961 abeewayconfig-0.2.5/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     8088 2024-05-27 18:43:27.000000 abeewayconfig-0.2.5/src/AbeewayConfig/CSVFile.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3479 2024-05-27 18:47:25.000000 abeewayconfig-0.2.5/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3034 2024-05-24 18:45:21.000000 abeewayconfig-0.2.5/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       74 2024-05-27 18:38:48.000000 abeewayconfig-0.2.5/src/AbeewayConfig/GUI_setup.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.5/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     6100 2024-05-27 18:47:25.000000 abeewayconfig-0.2.5/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.5/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      494 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       21 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.3/LICENSE` & `abeewayconfig-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.3/PKG-INFO` & `abeewayconfig-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.3
+Version: 0.2.5
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -27,21 +27,21 @@
 ```bash
   pip install abeewayconfig
 ```
 
 ## Usage
 
 ```bash
-  abeewayconfig
+  abeewayconfig config
 ```
 
 Run this command to open the GUI related to device configuring.
 
 ```bash
- abeewayupload
+ abeewayconfig upload
 ```
 
 Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
 
 ## Compatibility
 
 ### Operating Systems
```

### Comparing `abeewayconfig-0.2.3/README.md` & `abeewayconfig-0.2.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 ```bash
   pip install abeewayconfig
 ```
 
 ## Usage
 
 ```bash
-  abeewayconfig
+  abeewayconfig config
 ```
 
 Run this command to open the GUI related to device configuring.
 
 ```bash
- abeewayupload
+ abeewayconfig upload
 ```
 
 Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
 
 ## Compatibility
 
 ### Operating Systems
```

### Comparing `abeewayconfig-0.2.3/setup.py` & `abeewayconfig-0.2.5/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.3",
+    version="0.2.5",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
         "tk",
         "requests",
     ],
     entry_points={
         "console_scripts": [
             "abeewayconfig = AbeewayConfig.abeewayconfig:main",
-            "abeewayupload = AbeewayConfig.abeewayconfig:nw_sv_gui"
         ],
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     python_requires='>=3.0',
```

### Comparing `abeewayconfig-0.2.3/src/AbeewayConfig/CSVFile.py` & `abeewayconfig-0.2.5/src/AbeewayConfig/CSVFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import csv
 import os
 import re
 import shutil
 import tkinter as tk
+import kapak.error
 import requests
 
 from dataclasses import dataclass
-from tkinter import Text, filedialog
+from io import BytesIO
+from tkinter import filedialog
+from tkinter import simpledialog
 from typing import Any
+from kapak.aes import decrypt
+
+from .GUI_setup import root, console
 
 
 @dataclass
 class DevStruct:
     deveui: str = ""
     join_eui: str = ""
     app_key: str = ""
@@ -64,15 +70,15 @@
                     writer.writerows(data)
         except FileNotFoundError:
             with open(csv_file, mode='w', newline='') as file:
                 writer = csv.writer(file)
                 writer.writerows(data)
 
     @staticmethod
-    def retrieve_app_id(console_output: Text):
+    def retrieve_app_id():
         # todo choose app id for csv_templater
         response = requests.post(url='https://community.thingpark.io/thingpark/wireless/'
                                      'rest/subscriptions/mine/appServers',
                                  headers={
                                      'Authorization': f'Bearer {CSVFile.retrieve_token()}',
                                      'accept': 'application/json',
                                  })
@@ -82,101 +88,110 @@
         with open(os.path.join(os.path.dirname(__file__), "utils", "appids.txt"), 'a') as output:
             for match in matches:
                 output.write(match)
 
     # Name might be a little misleading since it doesn't grab the app_id,
     # but it's the only field where it has to be retrieved from the already set up network server
     @staticmethod
-    def grab_dev_info(deveui: str, console_output: Text) -> DevStruct:
+    def grab_dev_info(deveui: str) -> DevStruct:
         devstruct = DevStruct()
 
         with open('values.csv', 'r', newline='') as values:
             csv_reader = csv.reader(values, dialect='excel', delimiter=',')
             for row in csv_reader:
                 if row[0].strip().lower() == deveui:
                     devstruct.deveui = deveui
                     devstruct.join_eui = row[1]
                     devstruct.app_key = row[2]
                 elif row == csv_reader.line_num - 1:
-                    console_output.insert(tk.END, f"{deveui} not found in values.csv.\n")
+                    console.insert(tk.END, f"{deveui} not found in values.csv.\n")
                     return devstruct
 
         return devstruct
 
     @staticmethod
     def build_deveui_array_from_log() -> list[str]:
         deveui_array = []
-        with open('deveui.txt', 'r') as deveui_file:
+        with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils", "deveui.txt"), 'r') as deveui_file:
             for line in deveui_file:
                 deveui = re.search('(.*)\n', line).group(1).strip().lower()
                 if deveui is not None:
                     deveui_array.append(deveui)
         return deveui_array
 
     @staticmethod
-    def export_devices_from_csv(console_output: Text):
+    def export_devices_from_csv():
         with open(CSVFile.csv_file, 'rb') as csvfile:
             response = requests.post(url='https://community.thingpark.io/thingpark/wireless/rest/subscriptions/mine'
                                          '/devices/import?async=true&forceDevAddrs=false'
                                          '&networkSubscriptionsHandlingMode'
                                          '=ADVANCED',
                                      headers={
                                          'Authorization': f'Bearer {CSVFile.retrieve_token()}',
                                          'accept': 'application/json',
                                      },
                                      files={'csv': ('output.csv', csvfile, 'text/csv')}
                                      )
         match response.status_code:
             case 200:
-                console_output.insert(tk.END, f"Success.\n")
+                console.insert(tk.END, f"Success.\n")
             case 403:
-                console_output.insert(tk.END, f"Token error.\n")
+                console.insert(tk.END, f"Token error.\n")
 
-        console_output.insert(tk.END, f"{response.text}")
+        console.insert(tk.END, f"{response.text}")
 
     @staticmethod
-    def csv_builder(console_output: Text) -> None:
+    def csv_builder() -> None:
         deveui_array = CSVFile.build_deveui_array_from_log()
         for deveui in deveui_array:
-            dev_info = CSVFile.grab_dev_info(deveui=deveui,
-                                             console_output=console_output)
+            dev_info = CSVFile.grab_dev_info(deveui=deveui)
             dev_struct = CSVFile.csv_templater(deveui=dev_info.deveui,
                                                join_eui=dev_info.join_eui,
                                                app_key=dev_info.app_key,
                                                name=dev_info.name,
                                                app_id=dev_info.app_id)
             CSVFile.write_to_csv(data=dev_struct)
 
-        console_output.insert(tk.END, f"CSV file created.\n"
+        console.insert(tk.END, f"CSV file created.\n"
                                       f"There are {len(deveui_array)} devices. \n")
         # todo popup here
 
     @staticmethod
-    def import_values(console_output: Text) -> None:
+    def import_values() -> None:
         from .abeewayconfig import define_os_specific_startingdir
         filename = filedialog.askopenfilename(initialdir=define_os_specific_startingdir(),
                                               filetypes=[("CSV", "*.csv")])
         if filename:
             destination_dir = os.path.join(os.path.dirname(__file__), "utils")
             os.makedirs(destination_dir, exist_ok=True)
             destination_file = os.path.join(destination_dir, "values.csv")
             try:
                 shutil.copy(filename, destination_file)
-                console_output.insert(tk.END, "CSV file imported successfully.\n")
+                console.insert(tk.END, "CSV file imported successfully.\n")
             except Exception as e:
-                console_output.insert(tk.END, "Error:" + str(e) + "\n")
+                console.insert(tk.END, "Error:" + str(e) + "\n")
         else:
-            console_output.insert(tk.END, "No file selected.\n")
+            console.insert(tk.END, "No file selected.\n")
 
     @staticmethod
-    def retrieve_token() -> str:
+    def retrieve_token() -> str | None:
+        api = open(os.path.join(os.path.dirname(__file__), "utils", "secret.txt.bin"), "rb")
+        out = BytesIO()
+        password = simpledialog.askstring(title='Password', prompt='Insert password: ')
+        try:
+            for progress in decrypt(src=api, dst=out, password=password):
+                print(progress)
+        except kapak.error.KapakError as e:
+            console.insert(tk.END, f"Error: {e}\n")
+            return
+        out.seek(0)
+        decrypted_content = out.read().decode().splitlines()
         response = requests.post(url='https://community.thingpark.io/users-auth/protocol/openid-connect/token',
                                  data={
-                                     'client_id': f'{open(os.path.join(os.path.dirname(__file__),
-                                                                       "utils", "client.txt"), "r").read()}',
-                                     'client_secret': f'{open(os.path.join(os.path.dirname(__file__),
-                                                                           "utils", "secret.txt"), "r").read()}',
+                                     'client_id': f'{decrypted_content[0]}',
+                                     'client_secret': f'{decrypted_content[1]}',
                                      'grant_type': 'client_credentials'
                                  },
                                  headers={"content-type": "application/x-www-form-urlencoded"}
                                  ).json()
+        print(response)
         return response['access_token']
```

### Comparing `abeewayconfig-0.2.3/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.5/src/AbeewayConfig/Config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-import re
 import os
+import re
 import shutil
-from tkinter import Text, filedialog
 import tkinter as tk
+from tkinter import filedialog
+
 from .Device import Device
+from .GUI_setup import console
 from .smartbadgecfgdict import config_dict
 
 
 class Config:
     def get_config_value_from_cfg(parameter: int, line: str) -> int:
         if parameter is not None:
             pattern = r"config set %d (.*)" % parameter
@@ -18,53 +20,55 @@
 
     def get_config_parameter_from_cfg(line: str) -> int:
         p = re.compile("config set (.*) ")
         match = p.search(line)
         if match:
             return int(match.group(1))
 
-    def check_config_discrepancy(serial_port: str, br: int, console_output: Text) -> bool:
+    def check_config_discrepancy(serial_port: str, br: int) -> bool:
         device_config = Device.config_show_at_device(serial_port=serial_port, br=br)
         deveui = str(Device.get_deveui(serial_port=serial_port, br=br))
         config_file = os.path.join(os.path.join(os.path.dirname(__file__), "utils"), "config.cfg")
         try:
             with open(config_file, 'r') as config:
                 for line in config:
                     config_parameter_cfg = Config.get_config_parameter_from_cfg(line)
                     config_value_cfg = Config.get_config_value_from_cfg(config_parameter_cfg, line)
                     config_name = config_dict.get(config_parameter_cfg)
                     if config_parameter_cfg is not None or config_value_cfg is not None:
                         config_value_dev = Device.get_config_value_from_dev(device_config, config_name)
 
                         if config_parameter_cfg == 249 and config_value_dev == 5:
-                            console_output.insert(tk.END, f"Config error: {deveui} \n")
-                            console_output.insert(tk.END, f"An error occurred. Please try starting the device, "
-                                                          f"then configuring again. \n")
+                            console.insert(tk.END, f"Config error: {deveui} \n")
+                            console.insert(tk.END, f"An error occurred. Please try starting the device, "
+                                                   f"then configuring again. \n")
                             return False
 
                         if config_value_cfg != config_value_dev:
-                            console_output.insert(tk.END, f"Config error: {deveui} \n")
-                            console_output.insert(tk.END, f"[Parameter : {config_name}] - Current: [{config_value_dev}] | Correct: [{config_value_cfg}] \n")
+                            console.insert(tk.END, f"Config error: {deveui} \n")
+                            console.insert(tk.END, f"[Parameter : {config_name}] - Current: [{config_value_dev}] | "
+                                                   f"Correct: [{config_value_cfg}] \n")
                             return False
         except FileNotFoundError:
-            console_output.insert(tk.END, f"Config file not found.\n")
+            console.insert(tk.END, f"Config file not found.\n")
             return False
 
-        console_output.insert(tk.END, f"Done: {deveui} \n")
+        console.insert(tk.END, f"Done: {deveui} \n")
         return True
 
-    def import_config(console_output: Text) -> None:
+    @staticmethod
+    def import_config() -> None:
         from .abeewayconfig import define_os_specific_startingdir
         filename = filedialog.askopenfilename(initialdir=define_os_specific_startingdir(),
                                               filetypes=[("Text files", "*.txt"),
                                                          ("Config files", "*.cfg")])
         if filename:
             destination_dir = os.path.join(os.path.dirname(__file__), "utils")
             os.makedirs(destination_dir, exist_ok=True)
             destination_file = os.path.join(destination_dir, "config.cfg")
             try:
                 shutil.copy(filename, destination_file)
-                console_output.insert(tk.END, "Config file imported successfully.\n")
+                console.insert(tk.END, "Config file imported successfully.\n")
             except Exception as e:
-                console_output.insert(tk.END, "Error:" + str(e) + "\n")
+                console.insert(tk.END, "Error:" + str(e) + "\n")
         else:
-            console_output.insert(tk.END, "No file selected.\n")
+            console.insert(tk.END, "No file selected.\n")
```

### Comparing `abeewayconfig-0.2.3/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.5/src/AbeewayConfig/Device.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from serial import Serial
 
 
 class Device:
     def reset_dev(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
+            ser.write(b'123\r')
             ser.write(b'system reset\r')
             ser.close()
 
     def start_dev(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
+            ser.write(b'123\r')
             ser.write(b'system skip\r')
             sleep(6)
             ser.write(b'system log off\r')
             ser.close()
 
     def get_deveui(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
@@ -40,14 +42,15 @@
                     with open(deveui_file, 'a') as deveui_log:
                         deveui_log.write(deveui + "\n")
                 return deveui
 
     def set_config_on_device(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
+            ser.write(b'123\r')
             config_file = os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils"), "config.cfg")
             with open(config_file, 'rb') as config:
                 for line in config:
                     ser.write(line.strip())
                     ser.write(b'\r')
             ser.write(b'config save\r')
             ser.write(b'system buzzer 6\r')
@@ -60,12 +63,13 @@
             match_line = re.search(r".*\s+%s\s*=\s*(-?\d+)" % parameter, config_name)
             if match_line is not None:
                 return int(match_line.group(1))
 
     def config_show_at_device(serial_port: str, br: int) -> str:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
+            ser.write(b'123\r')
             ser.write(b'system log off\r')
             ser.write(b'config show\r')
             output = ser.read(16000)
             ser.close()
             return output.decode('utf-8')
```

### Comparing `abeewayconfig-0.2.3/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.5/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.3/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.3
+Version: 0.2.5
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
@@ -27,21 +27,21 @@
 ```bash
   pip install abeewayconfig
 ```
 
 ## Usage
 
 ```bash
-  abeewayconfig
+  abeewayconfig config
 ```
 
 Run this command to open the GUI related to device configuring.
 
 ```bash
- abeewayupload
+ abeewayconfig upload
 ```
 
 Run this command to open the GUI related to building a CSV to upload info about the configured devices to a cloud service, in this case, ThingPark.
 
 ## Compatibility
 
 ### Operating Systems
```

