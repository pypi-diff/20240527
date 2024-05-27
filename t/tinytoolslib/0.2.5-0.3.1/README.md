# Comparing `tmp/tinytoolslib-0.2.5.tar.gz` & `tmp/tinytoolslib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinytoolslib-0.2.5.tar", last modified: Wed Mar 20 07:32:41 2024, max compression
+gzip compressed data, was "tinytoolslib-0.3.1.tar", last modified: Mon May 27 13:21:18 2024, max compression
```

## Comparing `tinytoolslib-0.2.5.tar` & `tinytoolslib-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 07:32:41.304533 tinytoolslib-0.2.5/
--rw-rw-rw-   0        0        0     2520 2024-03-20 07:32:41.301533 tinytoolslib-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2024-03-13 13:27:22.000000 tinytoolslib-0.2.5/README.md
--rw-rw-rw-   0        0        0      744 2024-03-20 07:30:17.000000 tinytoolslib-0.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-20 07:32:41.304533 tinytoolslib-0.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-20 07:32:41.267528 tinytoolslib-0.2.5/tinytoolslib/
--rw-rw-rw-   0        0        0       36 2024-01-29 11:55:10.000000 tinytoolslib-0.2.5/tinytoolslib/__init__.py
--rw-rw-rw-   0        0        0       21 2024-03-20 07:30:18.000000 tinytoolslib-0.2.5/tinytoolslib/__version__.py
--rw-rw-rw-   0        0        0      443 2024-03-13 12:38:03.000000 tinytoolslib-0.2.5/tinytoolslib/constants.py
--rw-rw-rw-   0        0        0     6028 2024-03-13 12:48:15.000000 tinytoolslib-0.2.5/tinytoolslib/discovery.py
--rw-rw-rw-   0        0        0     1301 2024-03-13 12:48:15.000000 tinytoolslib-0.2.5/tinytoolslib/exceptions.py
--rw-rw-rw-   0        0        0    11882 2024-03-13 12:52:53.000000 tinytoolslib-0.2.5/tinytoolslib/flash.py
--rw-rw-rw-   0        0        0    60885 2024-03-18 12:00:11.000000 tinytoolslib-0.2.5/tinytoolslib/models.py
--rw-rw-rw-   0        0        0     2067 2024-03-13 12:42:29.000000 tinytoolslib-0.2.5/tinytoolslib/parsers.py
--rw-rw-rw-   0        0        0     7893 2024-03-13 12:37:58.000000 tinytoolslib-0.2.5/tinytoolslib/requests.py
-drwxrwxrwx   0        0        0        0 2024-03-20 07:32:41.299532 tinytoolslib-0.2.5/tinytoolslib.egg-info/
--rw-rw-rw-   0        0        0     2520 2024-03-20 07:32:41.000000 tinytoolslib-0.2.5/tinytoolslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-03-20 07:32:41.000000 tinytoolslib-0.2.5/tinytoolslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 07:32:41.000000 tinytoolslib-0.2.5/tinytoolslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-03-20 07:32:41.000000 tinytoolslib-0.2.5/tinytoolslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-20 07:32:41.000000 tinytoolslib-0.2.5/tinytoolslib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-27 13:21:18.730539 tinytoolslib-0.3.1/
+-rw-rw-rw-   0        0        0     1197 2024-05-27 13:21:18.728541 tinytoolslib-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-22 09:12:29.000000 tinytoolslib-0.3.1/README.md
+-rw-rw-rw-   0        0        0      744 2024-05-27 13:19:20.000000 tinytoolslib-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 13:21:18.730539 tinytoolslib-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 13:21:18.687538 tinytoolslib-0.3.1/tinytoolslib/
+-rw-rw-rw-   0        0        0      195 2024-05-21 13:23:16.000000 tinytoolslib-0.3.1/tinytoolslib/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-05-27 13:19:20.000000 tinytoolslib-0.3.1/tinytoolslib/__version__.py
+-rw-rw-rw-   0        0        0      884 2024-05-21 12:06:51.000000 tinytoolslib-0.3.1/tinytoolslib/constants.py
+-rw-rw-rw-   0        0        0     5170 2024-05-21 12:06:51.000000 tinytoolslib-0.3.1/tinytoolslib/discovery.py
+-rw-rw-rw-   0        0        0     1301 2024-03-13 12:48:15.000000 tinytoolslib-0.3.1/tinytoolslib/exceptions.py
+-rw-rw-rw-   0        0        0    14676 2024-05-27 13:11:18.000000 tinytoolslib-0.3.1/tinytoolslib/flash.py
+-rw-rw-rw-   0        0        0    61685 2024-05-21 12:34:01.000000 tinytoolslib-0.3.1/tinytoolslib/models.py
+-rw-rw-rw-   0        0        0     2067 2024-03-13 12:42:29.000000 tinytoolslib-0.3.1/tinytoolslib/parsers.py
+-rw-rw-rw-   0        0        0     8724 2024-05-27 12:27:05.000000 tinytoolslib-0.3.1/tinytoolslib/requests.py
+drwxrwxrwx   0        0        0        0 2024-05-27 13:21:18.727545 tinytoolslib-0.3.1/tinytoolslib.egg-info/
+-rw-rw-rw-   0        0        0     1197 2024-05-27 13:21:18.000000 tinytoolslib-0.3.1/tinytoolslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-05-27 13:21:18.000000 tinytoolslib-0.3.1/tinytoolslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 13:21:18.000000 tinytoolslib-0.3.1/tinytoolslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-27 13:21:18.000000 tinytoolslib-0.3.1/tinytoolslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-05-27 13:21:18.000000 tinytoolslib-0.3.1/tinytoolslib.egg-info/top_level.txt
```

### Comparing `tinytoolslib-0.2.5/pyproject.toml` & `tinytoolslib-0.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tinytoolslib"
-version = "0.2.5"
+version = "0.3.1"
 authors = [
     { name="Bartek Barszczewski", email="tinycontrol.software@gmail.com" },
 ]
 description = "Set of tools for use with Tinycontrol devices like LK2.X, LK3.X, LK4.X or tcPDU."
 requires-python = ">=3.7"
 classifiers = [
    "Programming Language :: Python :: 3",
```

### Comparing `tinytoolslib-0.2.5/tinytoolslib/exceptions.py` & `tinytoolslib-0.3.1/tinytoolslib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tinytoolslib-0.2.5/tinytoolslib/flash.py` & `tinytoolslib-0.3.1/tinytoolslib/flash.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,79 +1,113 @@
+"""Flash function for tinycontrol devices.
+
+Handles HTTP and TFTP methods.
+- HTTP method is for LK4, tcPDU
+- TFTP method is for LK3.5, LK3.0, LK2.5, LK2.0
+For details you can see .models.py as FW update method is part of device description.
+"""
+
 import logging
 import os
 import socket
 import time
 from functools import wraps
 from math import ceil
-from threading import Event
+from typing import Any, Callable, Dict, Tuple, Union
 
+import requests
 from tftpy import SOCK_TIMEOUT, TftpClient, TftpTimeout
 
-from tinytoolslib.constants import LK_UDP_BOOTLOADER_MSG, LK_UDP_PORT
-from tinytoolslib.requests import get, post
+from tinytoolslib.constants import LK_UDP_BOOTLOADER_MSG, LK_UDP_PORT, FWUpdateMethod
 from tinytoolslib.exceptions import TinyToolsFlashError, TinyToolsRequestError
 from tinytoolslib.models import (
     LK_HW_20,
     LK_HW_20_PS,
     LK_HW_25,
     LK_HW_25_PS,
     get_version,
 )
+from tinytoolslib.requests import get, post
 
 
 class Flasher:
     """Class with all flash related functions.
 
     Generally use as:
     flasher = Flasher()
     flasher.run(...)
     """
 
-    def __init__(self, callback=None):
-        """Initialize Flasher.
+    def __init__(self):
+        """Initialize Flasher."""
+        self.callback_progress: Callable[[int, int, float, str], None] = None
+        """Function called during flashing with progress info.
 
-        callback - None/function that will be called during flashing
-        with progress information. 4 parameters: current, total,
-        percent, unit ('packet', 'B').
+        Parameters are current, total, percent, unit(packet/B).
+        """
+        self.callback_cancel: Callable[[], bool] = None
+        """Function called before actual flashing has started.
+
+        If it returns True then flashing will be canceled.
         """
-        self.callback = callback
         self.context = {}
-        self.canceled = Event()
+        self._session = requests.Session()
 
     # region TFTP flashing
     @staticmethod
-    def get_optimal_number_of_attempts(version_info):
+    def get_optimal_number_of_attempts(version_info: Dict[str, Any]) -> int:
         """Return number of attempts, so for HW2.X it quits earlier.
 
+        version_info is expected to be return value of get_version().
         Each attempt takes SOCK_TIMEOUT*TIMEOUT_RETRIES
         """
         logging.debug("Getting optimal number of flash attempts (less for LK2.X)")
         lk_2X_models = [
             LK_HW_20_PS.info.model,
             LK_HW_20.info.model,
             LK_HW_25.info.model,
             LK_HW_25_PS.info.model,
         ]
         if version_info is not None and version_info["model"] in lk_2X_models:
             return 1
         return 4
 
-    def start_bootloader(self, host, username, password, schema, port):
+    def start_bootloader(
+        self, host: str, username: str, password: str, schema: str, port: int
+    ) -> bool:
         """Start bootloader mode on device (LK2.X, LK3.X)."""
         success = False
         # First try http method.
         try:
             # First check if upgrade is enabled else enable it
-            resp = get(host, "/xml/st.xml", schema, port, username, password)["parsed"]
+            resp = get(
+                host,
+                "/xml/st.xml",
+                schema,
+                port,
+                username,
+                password,
+                session=self._session,
+            )["parsed"]
             if resp.get("upgr") == "0":
                 logging.info("Upgrade is disabled on device - trying to enable it.")
                 cmd = "/stm.cgi?auth={}{}{}".format(resp["auth"], 1, resp["userpass"])
-                get(host, cmd, schema, port, username, password)["parsed"]
+                get(host, cmd, schema, port, username, password, session=self._session)[
+                    "parsed"
+                ]
             logging.info("Starting bootloader mode via HTTP...")
-            get(host, "/stm.cgi?upgrade=lkstart3", schema, port, username, password)
+            get(
+                host,
+                "/stm.cgi?upgrade=lkstart3",
+                schema,
+                port,
+                username,
+                password,
+                session=self._session,
+            )
             success = True
         except (KeyError, ValueError, TinyToolsRequestError) as exc:
             logging.error("Failed to enable bootloader via HTTP: %s", str(exc))
         if not success:
             # Try UDP method.
             logging.info("Starting bootloader mode via UDP...")
             with socket.socket(
@@ -82,29 +116,35 @@
                 sock.connect((host, LK_UDP_PORT))
                 sock.sendall(LK_UDP_BOOTLOADER_MSG)
             success = True
         return success
 
     def flash_hook(self, packet):
         """Display flashing progress."""
-        if self.canceled.is_set() and packet.opcode == 2:
-            # Cancel if stop flag set and still waiting for transfer.
+        # Cancel only while waiting for transfer
+        if (
+            packet.opcode == 2
+            and callable(self.callback_cancel)
+            and self.callback_cancel()
+        ):
             raise TinyToolsFlashError("Flash canceled by user")
         if packet.opcode == 3:
             logging.debug("Packet %d/%d", packet.blocknumber, self.context["packets"])
-            if callable(self.callback):
+            if callable(self.callback_progress):
                 # Call with <packet no>, <total packets>, <progress %>
-                self.callback(
+                self.callback_progress(
                     packet.blocknumber,
                     self.context["packets"],
                     packet.blocknumber / self.context["packets"] * 100,
                     "packet",
                 )
 
-    def flash_firmware_via_tftp(self, host, firmware_path, attempts_limit):
+    def flash_firmware_via_tftp(
+        self, host: str, firmware_path: str, attempts_limit: int
+    ) -> bool:
         """Try to flash firmware and display progress."""
         firmware_name = os.path.basename(firmware_path)
         bytes_size = os.stat(firmware_path).st_size
         self.context.update(
             {
                 "size": bytes_size,
                 "packets": ceil(bytes_size / 512),
@@ -118,15 +158,15 @@
         )
         client = TftpClient(host)
         attempt = 0
         flashed = False
         canceled = False
         while attempt < attempts_limit and not flashed:
             try:
-                if self.canceled.is_set():
+                if callable(self.callback_cancel) and self.callback_cancel():
                     # Stop before starting flash.
                     raise TinyToolsFlashError("Flash canceled by user")
                 client.upload(firmware_name, firmware_path, self.flash_hook)
             except TftpTimeout:
                 attempt += 1
             except (ConnectionError, socket.gaierror):
                 attempt += 1
@@ -149,16 +189,22 @@
                 client.context.metrics.kbps,
             )
             return True
 
     # endregion
 
     def update_firmware_via_http(
-        self, firmware_path, host, username, password, schema, port
-    ):
+        self,
+        firmware_path: str,
+        host: str,
+        username: str,
+        password: str,
+        schema: str,
+        port: int,
+    ) -> bool:
         """Update firmware via HTTP for LK4/tcPDU."""
         try:
             with open(firmware_path, "rb") as fread:
                 bytes_size = os.stat(firmware_path).st_size
                 self.context.update(
                     {
                         "size": bytes_size,
@@ -176,115 +222,148 @@
                         self.context["uploaded"] = self.context["size"]
                     logging.debug(
                         "Uploaded %.0f/%.0f kB (%.1f %%)",
                         self.context["uploaded"] / 1024,
                         self.context["size"] / 1024,
                         self.context["uploaded"] / self.context["size"] * 100,
                     )
-                    if callable(self.callback):
+                    if callable(self.callback_progress):
                         # Call with <uploaded B>, <total B>, <progress %>
-                        self.callback(
+                        self.callback_progress(
                             self.context["uploaded"],
                             self.context["size"],
                             self.context["uploaded"] / self.context["size"] * 100,
                             "B",
                         )
                     return res
 
                 setattr(fread, "read", read)
                 # Upload file
-                if callable(self.callback):
+                if callable(self.callback_progress):
                     # Call with <0 B>, <total B>, <0 %>
-                    self.callback(0, self.context["size"], 0, "B")
+                    self.callback_progress(0, self.context["size"], 0, "B")
                 resp = post(
                     host,
                     "/api/v1/upload_firmware/new_firmware",
-                    fread,
                     schema,
                     port,
                     username,
                     password,
+                    data=fread,
+                    session=self._session,
                 )
                 # Restart device
-                get(host, "/api/v1/save/?restart=1", schema, port, username, password)
+                get(
+                    host,
+                    "/api/v1/save/?restart=1",
+                    schema,
+                    port,
+                    username,
+                    password,
+                    session=self._session,
+                )
         except Exception as exc:
             logging.warning("Error occurred: %s. Try again.", str(exc))
             return False
         else:
             logging.info(
                 "Uploaded firmware in %.1fs with avg speed of %.0f kbps.",
-                resp.elapsed.total_seconds(),
-                self.context["size"] / 1024 * 8 / resp.elapsed.total_seconds(),
+                resp.get("elapsed", 1),
+                self.context["size"] / 1024 * 8 / resp.get("elapsed", 1),
             )
             return True
 
     def run(
-        self, firmware_path, host, username, password, port=80, progress_callback=None
-    ):
-        """Main entry to flashing.
+        self,
+        firmware_path: str,
+        host: str,
+        username: str,
+        password: str,
+        port: int = 80,
+        callback_progress: Union[Callable[[int, int, float, str], None], None] = None,
+        callback_cancel: Union[Callable[[], bool], None] = None,
+    ) -> bool:
+        """Flash given firmware to given address.
 
-        Depending on input and data found from device it will select
-        tftp or http method.
+        It automatically uses HTTP or TFTP method (latter one is used if device does not respond).
         """
-        if progress_callback is not None:
-            self.callback = progress_callback
+        self.callback_progress = callback_progress
+        self.callback_cancel = callback_cancel
         self.context = {}
         if (
             isinstance(firmware_path, str)
             and firmware_path
             and os.path.isfile(firmware_path)
         ):
-            # Try to check what device type are we working with. For now,
-            # assume that lk4/tcpdu always respond via HTTP.
-            version_info = get_version(host, port, username, password)
-            if version_info and version_info["network_info"].get("schema") == "https":
-                schema = "https"
-                port = 443
-            else:
-                schema = "http"
-            if version_info and version_info.get("http_update"):
-                return self.update_firmware_via_http(
-                    firmware_path, host, username, password, schema, port
-                )
-            else:
-                attempts = self.get_optimal_number_of_attempts(version_info)
-                logging.info("Preparing device for flashing...")
-                self.start_bootloader(host, username, password, schema, port)
-                return self.flash_firmware_via_tftp(host, firmware_path, attempts)
+            with self._session:
+                # Try to check what device type are we working with. For now,
+                # assume that lk4/tcpdu always respond via HTTP.
+                version_info = get_version(host, port, username, password)
+                if (
+                    version_info
+                    and version_info["network_info"].get("schema") == "https"
+                ):
+                    schema = "https"
+                    port = 443
+                else:
+                    schema = "http"
+                if (
+                    version_info
+                    and version_info.get("fw_update_method") == FWUpdateMethod.HTTP
+                ):
+                    return self.update_firmware_via_http(
+                        firmware_path, host, username, password, schema, port
+                    )
+                else:
+                    attempts = self.get_optimal_number_of_attempts(version_info)
+                    logging.info("Preparing device for flashing...")
+                    self.start_bootloader(host, username, password, schema, port)
+                    return self.flash_firmware_via_tftp(host, firmware_path, attempts)
         else:
             logging.warning("Invalid file for flashing.")
             return False
 
 
 # region getting new firmware file
-def check_for_latest_firmware(version_info):
-    """Check latest available version of firmware."""
-    if version_info["fw_url"] is None:
+def check_for_latest_firmware(fw_url: str) -> Tuple[bool, Union[Dict[str, Any], str]]:
+    """Check latest available version of firmware.
+
+    Returns:
+        (True, {name: str, description: {en: str, pl: str}, url: str, date: str})
+        (False, str) - str is an error message
+    """
+    if fw_url is None:
         return (
             False,
             "Cannot get firmware files for this device directly. "
             "You can look for it at https://tinycontrol.pl.",
         )
     try:
-        resp = get(version_info["fw_url"], None, timeout=5)
+        resp = get(fw_url, None, timeout=5)
     except TinyToolsRequestError as exc:
         return False, str(exc)
     else:
         result = resp["parsed"]
-        result.update({"hardware_version": version_info["hardware_version"]})
         return True, result
 
 
-def get_latest_firmware(host, username, password, firmware_directory):
-    """Get latest firmware for device."""
+def get_latest_firmware(
+    host: str, username: str, password: str, firmware_directory: str
+) -> Tuple[bool, Union[Dict[str, Any], str]]:
+    """Get latest firmware for device.
+
+    Returns:
+        (True, {**get_version(), path: str, new_sw: str})
+        (False, str) - str is an error message
+    """
     version_info = get_version(host, username=username, password=password)
     if version_info:
-        latest_version = check_for_latest_firmware(version_info)
+        latest_version = check_for_latest_firmware(version_info.get("fw_url"))
         if latest_version[0]:
-            # Check if downloaded else download
+            # Check if it's already downloaded else download
             firmware_name = latest_version[1]["url"].split("/")[-1]
             firmware_path = os.path.join(firmware_directory, firmware_name)
             if os.path.isfile(firmware_path) or download_firmware(
                 latest_version[1]["url"], firmware_path
             ):
                 version_info.update(
                     {
@@ -296,21 +375,43 @@
             else:
                 return False, "Failed to download file"
         else:
             return False, latest_version[1]
     return False, "Cannot get information about latest firmware"
 
 
-def download_firmware(download_url, save_location):
+def download_firmware(download_url: str, save_location: str) -> bool:
     """Download firmware from given url."""
     try:
         resp = get(download_url, None, timeout=5)
     except TinyToolsRequestError:
         return False
     else:
         os.makedirs(os.path.dirname(save_location), exist_ok=True)
         with open(save_location, "wb") as f:
             f.write(resp["_response"].content)
         return True
 
 
 # endregion
+
+
+def run_flash(
+    firmware_path: str,
+    host: str,
+    username: str,
+    password: str,
+    port: int = 80,
+    callback_progress: Union[Callable[[int, int, float, str], None], None] = None,
+    callback_cancel: Union[Callable[[], bool], None] = None,
+) -> bool:
+    """Run flashing firmware to given address."""
+    flasher = Flasher()
+    return flasher.run(
+        firmware_path,
+        host,
+        username,
+        password,
+        port,
+        callback_progress,
+        callback_cancel,
+    )
```

### Comparing `tinytoolslib-0.2.5/tinytoolslib/models.py` & `tinytoolslib-0.3.1/tinytoolslib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-from dataclasses import dataclass, field, asdict
+"""Device definitions along with methods for communicating with them."""
+
 import re
-from typing import Tuple, Union, Dict, List, ClassVar, Any
 import warnings
+from abc import ABC, abstractmethod
+from dataclasses import asdict, dataclass, field
+from typing import Any, ClassVar, Dict, List, Tuple, Union
 
-from tinytoolslib.parsers import (
-    int_inverted,
-    parse_version,
-    up_to_int,
-    float_div10,
-    float_div100,
-    float_div1000,
-    strint_to_int_list,
-    name_list,
-    list_map,
-)
-from tinytoolslib.requests import get, async_get
 from aiohttp import ClientSession
-from tinytoolslib.constants import (
-    FAMILY_DCDC,
-    FAMILY_LK,
-    FAMILY_PS,
-    FAMILY_TCPDU,
-    FW_URL_TEMPLATE,
-)
+
+from tinytoolslib.constants import FW_URL_TEMPLATE, DeviceFamily, FWUpdateMethod
 from tinytoolslib.exceptions import (
     TinyToolsRequestConnectionError,
     TinyToolsRequestError,
     TinyToolsRequestInternalServerError,
     TinyToolsRequestNotFound,
     TinyToolsRequestSSLError,
     TinyToolsRequestTimeout,
     TinyToolsUnsupported,
 )
+from tinytoolslib.parsers import (
+    float_div10,
+    float_div100,
+    float_div1000,
+    int_inverted,
+    list_map,
+    name_list,
+    parse_version,
+    strint_to_int_list,
+    up_to_int,
+)
+from tinytoolslib.requests import async_get, get
 
 
 @dataclass
 class DeviceInfo:
+    """General information about Device."""
+
     model: str
-    family: str
+    family: DeviceFamily
     fw_tag: Union[str, None] = None
     fw_url: Union[str, None] = field(init=False, default=None)
     fw_changelog: Union[str, None] = None
+    fw_update_method: Union[str, None] = None
     extras: Dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self):
         if self.fw_tag:
             self.fw_url = FW_URL_TEMPLATE.format(self.fw_tag)
 
 
 @dataclass
-class DeviceModel:
+class DeviceModel(ABC):
     """Base class for tinycontrol devices with common methods."""
 
     info: ClassVar[Union[DeviceInfo, None]] = None
     mapping: ClassVar[Dict[str, Dict]] = {}
     parsers: ClassVar[List[str]] = []
 
     host: str
@@ -72,19 +73,19 @@
         if self.schema == "https" and self.port != 443:
             warnings.warn(
                 "Devices (LK3.X, LK4.X, tcPDU) always use port 443 for https. "
                 f"You are about to use {self.port}."
             )
 
     @classmethod
+    @abstractmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         """Verifies if versions matches this Device model."""
-        raise NotImplementedError
 
     def _get(
         self,
         data: Dict[str, Any],
         path: str,
         skip_keys: Union[List[str], None] = None,
         remove_mapped_keys: bool = False,
@@ -132,85 +133,85 @@
             password=self.password,
             **kwargs,
         )
         return self._get(response.get("parsed"), path, skip_keys, remove_mapped_keys)
 
     def set_out(self, index, value=None):
         """Set output state to value or toggle if value is None."""
-        if hasattr(self, "_set_out") and callable(self._set_out):
+        if callable(getattr(self, "_set_out", None)):
             return self.get(self._set_out(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling OUTs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling OUTs"
         )
 
     def set_pwm(self, index, value):
         """Set pwm state to value or toggle if value is None."""
-        if hasattr(self, "_set_pwm") and callable(self._set_pwm):
+        if callable(getattr(self, "_set_pwm", None)):
             return self.get(self._set_pwm(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling PWMs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling PWMs"
         )
 
     def set_pwm_duty(self, index, value):
         """Set pwm duty to value."""
-        if hasattr(self, "_set_pwm_duty") and callable(self._set_pwm_duty):
+        if callable(getattr(self, "_set_pwm_duty", None)):
             return self.get(self._set_pwm_duty(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling PWM duty".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling PWM duty"
         )
 
     def set_pwm_freq(self, index, value):
         """Set pwm freq to value."""
-        if hasattr(self, "_set_pwm_freq") and callable(self._set_pwm_freq):
+        if callable(getattr(self, "_set_pwm_freq", None)):
             return self.get(self._set_pwm_freq(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling PWM freq".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling PWM freq"
         )
 
     def set_var(self, index, value):
         """Set VAR/EVENT variable to value."""
-        if hasattr(self, "_set_var") and callable(self._set_var):
+        if callable(getattr(self, "_set_var", None)):
             return self.get(self._set_var(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling VARs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling VARs"
         )
 
     def set_ds(self, index: int, value: str):
         """Set ID of DS on position to value."""
-        if hasattr(self, "_set_ds") and callable(self._set_ds):
+        if callable(getattr(self, "_set_ds", None)):
             return self.get(self._set_ds(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support setting DSs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support setting DSs"
         )
 
     def get_all(self) -> Dict[str, Any]:
         """Get set of all sensor/readings."""
-        if hasattr(self, "_get_all") and callable(self._get_all):
+        if callable(getattr(self, "_get_all", None)):
             data = {}
             for url in self._get_all():
                 data.update(self.get(url))
             return data
         raise TinyToolsUnsupported(
-            "{} does not support get_all command".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support get_all command"
         )
 
     def reset_to_defaults(self):
         """Reset settings to defaults."""
-        if hasattr(self, "_reset_to_defaults") and callable(self._reset_to_defaults):
+        if callable(getattr(self, "_reset_to_defaults", None)):
             return self.get(self._reset_to_defaults())
         raise TinyToolsUnsupported(
-            "{} does not support reset to defaults".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support reset to defaults"
         )
 
     def restart(self):
         """Restart device."""
-        if hasattr(self, "_restart") and callable(self._restart):
+        if callable(getattr(self, "_restart", None)):
             return self.get(self._restart())
         raise TinyToolsUnsupported(
-            "{} does not support restart command".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support restart command"
         )
 
     # region Async variants
     async def async_get(
         self,
         path: str,
         skip_keys: Union[List[str], None] = None,
@@ -230,42 +231,46 @@
             password=self.password,
             session=self.session,
             **kwargs,
         )
         return self._get(response.get("parsed"), path, skip_keys, remove_mapped_keys)
 
     async def async_set_out(self, index, value=None):
-        if hasattr(self, "_set_out") and callable(self._set_out):
+        """Async set_out."""
+        if callable(getattr(self, "_set_out", None)):
             return await self.async_get(self._set_out(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling OUTs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling OUTs"
         )
 
     async def async_set_pwm(self, index, value):
-        if hasattr(self, "_set_pwm") and callable(self._set_pwm):
+        """Async set_pwm."""
+        if callable(getattr(self, "_set_pwm", None)):
             return await self.async_get(self._set_pwm(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling PWMs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling PWMs"
         )
 
     async def async_set_var(self, index, value):
-        if hasattr(self, "_set_var") and callable(self._set_var):
+        """Async set_var."""
+        if callable(getattr(self, "_set_var", None)):
             return await self.async_get(self._set_var(index, value))
         raise TinyToolsUnsupported(
-            "{} does not support controlling VARs".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support controlling VARs"
         )
 
     async def async_get_all(self) -> Dict[str, Any]:
-        if hasattr(self, "_get_all") and callable(self._get_all):
+        """Async get_all."""
+        if callable(getattr(self, "_get_all", None)):
             data = {}
             for url in self._get_all():
                 data.update(await self.async_get(url))
             return data
         raise TinyToolsUnsupported(
-            "{} does not support get_all command".format(self.__class__.__name__)
+            f"{self.__class__.__name__} does not support get_all command"
         )
 
     # region Session handling for asyncio
     async def close(self) -> None:
         """Close open client session."""
         await self.session.close()
 
@@ -296,15 +301,16 @@
     """Methods for working with Power Socket on LK2.0.
 
     Note: for outputs it uses unified values 0 - off, 1 - on.
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "IP Power Socket v1 (LK2.0)",  # 5G10A/6G10A
-        FAMILY_PS,
+        DeviceFamily.PS,
+        fw_update_method=FWUpdateMethod.TFTP,
     )
     mapping: ClassVar[Dict[str, Dict]] = {
         # --- st0.xml
         "out0": {"name": "out0", "format": int_inverted},
         "out1": {"name": "out1", "format": int_inverted},
         "out2": {"name": "out2", "format": int_inverted},
         "out3": {"name": "out3", "format": int_inverted},
@@ -466,17 +472,18 @@
     """Methods for working with LK2.0.
 
     Note: for outputs it uses unified values 0 - off, 1 - on.
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 2.0",
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc20",
         "https://tinycontrol.pl/en/archives/lan-controller-20/#firmware",
+        fw_update_method=FWUpdateMethod.TFTP,
     )
     mapping: ClassVar[Dict[str, Dict]] = {
         # Overwrite PS mapping (there will be extra b30, b31)
         **LK_HW_20_PS.mapping,
         # --- st0.xml
         "di2": {"name": "iDValue3", "format": up_to_int},
         "di3": {"name": "iDValue4", "format": up_to_int},
@@ -600,15 +607,15 @@
         Arguments:
             index: not used (only one frequency)
             value: 2_600-4_000_000
         """
         return "/ind.cgi?pwmf={}".format(value)
 
     def _set_ds(self, index: int, value: Any = None) -> str:
-        """Set ID of DS on position to value.
+        """Prepare command for setting DS ID.
 
         Arguments:
             index - 1-6
             value - not used for LK2.X
         """
         cmd = "/ind.cgi?ds={}".format(index)
         return cmd
@@ -624,31 +631,33 @@
     """Methods for working with LK2.5.
 
     Note: for outputs it uses unified values 0 - off, 1 - on.
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 2.5",
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc25",
         "https://tinycontrol.pl/en/lan-controller-25/firmware-docs/#firmware",
+        fw_update_method=FWUpdateMethod.TFTP,
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return hardware_version == "2.5" and software_version != "6.15"
 
 
 @dataclass
 class LK_HW_25_PS(LK_HW_20_PS):
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "IP Power Socket v2 (LK2.5)",
-        FAMILY_PS,
+        DeviceFamily.PS,
+        fw_update_method=FWUpdateMethod.TFTP,
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return hardware_version == "2.5" and software_version == "6.15"
@@ -660,18 +669,19 @@
 
     Note that INPD/digital for HW 3.5+ SW 1.49+ includes negation
     right in response from LK. Previous SW and HW 3.0 do NOT.
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 3.0",
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc30",
         "https://tinycontrol.pl/en/archives/lan-controller-30/#firmware",
-        {"number_of_outputs": 6},
+        fw_update_method=FWUpdateMethod.TFTP,
+        extras={"number_of_outputs": 6},
     )
     mapping: ClassVar[Dict[str, Dict]] = {
         # OUTs - further parsed with _parse_outs
         "out0": {"name": "out0", "format": int},
         "out1": {"name": "out1", "format": int},
         "out2": {"name": "out2", "format": int},
         "out3": {"name": "out3", "format": int},
@@ -823,15 +833,17 @@
         if self.hardware_version == "3.0" or (
             self.hardware_version != "3.0" and self.software_version <= "1.31"
         ):
             # LK HW 3.0 or HW 3.5+ SW <=1.31 - Dict method for sdm1-sdm14, rest is unknown
             if "sdm1" not in data:
                 return
             for index in range(1, 15):
-                data["mValue{}".format(index)] = float_div100(data["sdm{}".format(index)])
+                data["mValue{}".format(index)] = float_div100(
+                    data["sdm{}".format(index)]
+                )
             for index in range(15, 31):
                 data["mValue{}".format(index)] = 0
         elif self.hardware_version != "3.0" and self.software_version < "1.33":
             # HW 3.5+ SW 1.32+ - List method for sdm1-sdm29
             if "modbusSensor" not in data or "sdm1" not in data:
                 return
             modbus_sensor = int(data.get("modbusSensor", 0))
@@ -963,15 +975,15 @@
             else:
                 cmd += "pwm{}={}".format(index, value)
         return cmd
 
     def _set_pwm_duty(
         self, index: Union[int, List[int]], value: Union[int, List[int]]
     ) -> str:
-        """Set pwm duty to value.
+        """Prepare command for setting PWM duty.
 
         Arguments:
             index: 0-3 (single or list)
             value: 0-100 (single or list)
         """
         cmd = "/stm.cgi?"
         if isinstance(index, list):
@@ -984,15 +996,15 @@
         else:
             cmd += "pwmd={}{}".format(index, int(value))
         return cmd
 
     def _set_pwm_freq(
         self, index: Union[int, List[int]], value: Union[int, List[int]]
     ) -> str:
-        """Set pwm freq to value.
+        """Prepare command for setting PWM freq.
 
         Arguments:
             index: 0-1 (single or list; 0 - pwm0, 1 - pwm1-3 shared)
             value: 1-1_000_000
         """
         cmd = "/stm.cgi?"
         if isinstance(index, list):
@@ -1005,15 +1017,15 @@
         else:
             cmd += "pwmf={}{}".format(index, int(value))
         return cmd
 
     def _set_ds(
         self, index: Union[int, List[int]], value: Union[str, List[str]]
     ) -> str:
-        """Set ID of DS on position to value.
+        """Prepare command for setting DS ID.
 
         Arguments:
             index: 1-8
             value: DS ID
         """
         cmd = "/stm.cgi?"
         if isinstance(index, list):
@@ -1036,19 +1048,19 @@
         """Prepare list of URLs to fetch data from."""
         urls = ["/json/all.json", "/json/pwmpid.json"]
         if self.hardware_version >= "3.5" and "1.50" > self.software_version >= "1.22b":
             urls.append("/json/events_per.json")
         return urls
 
     def _reset_to_defaults(self):
-        """Reset settings to defaults."""
+        """Prepare command to reset settings to default."""
         return "/stm.cgi?eeprom_reset=1"
 
     def _restart(self):
-        """Restart device."""
+        """Prepare command to restart device."""
         return "/stm.cgi?upgrade=lkstart3"
 
     def set_analog_input(
         self,
         index: Union[int, List[int]],
         sensor: Union[int, List[int]],
         calibration: Union[int, List[int], None] = None,
@@ -1109,18 +1121,19 @@
 
 @dataclass
 class LK_HW_35(LK_HW_30):
     """Methods for working with LK3.5."""
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 3.5",  # Covers HW 3.5, 3.6, 3.7, 3.8
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc35",
         "https://tinycontrol.pl/en/lan-controller-35/firmware/#firmware",
-        {"number_of_outputs": 6},
+        fw_update_method=FWUpdateMethod.TFTP,
+        extras={"number_of_outputs": 6},
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return (
@@ -1153,15 +1166,16 @@
 
 @dataclass
 class LK_HW_35_PS(LK_HW_35):
     """Methods for working with IP Power Socket v2 (LK3.5)."""
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "IP Power Socket v2 (LK3.5)",  # 5G10A/6G10A
-        FAMILY_PS,
+        DeviceFamily.PS,
+        fw_update_method=FWUpdateMethod.TFTP,
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return "3.5" <= hardware_version < "4.0" and software_version.endswith("ps")
@@ -1169,15 +1183,16 @@
 
 @dataclass
 class LK_HW_35_DCDC(LK_HW_35):
     """Methods for working with LK3.5."""
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "Converter DC/DC",
-        FAMILY_DCDC,
+        DeviceFamily.DCDC,
+        fw_update_method=FWUpdateMethod.TFTP,
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return "3.5" <= hardware_version < "4.0" and software_version.endswith("dcdc")
@@ -1189,18 +1204,19 @@
 
     For information about possible requests see:
     https://docs.tinycontrol.pl/en/lk4/api/commands/
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 4.0",
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc40",
         "https://tinycontrol.pl/en/lk4/downloads/#firmware",
-        {"number_of_outputs": 6},
+        fw_update_method=FWUpdateMethod.HTTP,
+        extras={"number_of_outputs": 6},
     )
     mapping: ClassVar[Dict[str, Dict]] = {
         "netMac": {"name": "mac", "format": str},
         "softwareVersion": {"name": "software_version", "format": str},
         "hardwareVersion": {"name": "hardware_version", "format": str},
     }
     parsers: ClassVar[List[str]] = ["_parse_outs"]
@@ -1335,15 +1351,15 @@
         else:
             cmd += "var{}={}".format(index, value)
         return cmd
 
     def _set_ds(
         self, index: Union[int, List[int]], value: Union[str, List[str]]
     ) -> str:
-        """Set ID of DS on position to value.
+        """Prepare command for setting DS ID.
 
         Arguments:
             index: 1-8
             value: DS ID
         """
         cmd = "/api/v1/save/?"
         if isinstance(index, list):
@@ -1366,36 +1382,37 @@
         """Prepare list of URLs to fetch data from."""
         return [
             "/api/v1/read/set/?generalConfig&outConfig&powerConfig&networkConfig",
             "/api/v1/read/status/?boardValues&statusValues&timeValues&outValues&pwmValues&iAValues&dsValues&i2cValues&otherSensorsValues&diffValues&iDValues&powerValues&mrValues&varValues",
         ]
 
     def _reset_to_defaults(self):
-        """Reset settings to defaults."""
+        """Prepare command to reset settings to default."""
         return "/api/v1/save/?eeprom_reset=1"
 
     def _restart(self):
-        """Restart device."""
+        """Prepare command to restart device."""
         return "/api/v1/save/?restart=1"
 
 
 @dataclass
 class TCPDU(LK_HW_40):
     """Device model for tcPDU.
 
     For information about possible requests see:
     https://docs.tinycontrol.pl/en/tcpdu/api/commands/
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "tcPDU",
-        FAMILY_TCPDU,
+        DeviceFamily.TCPDU,
         "tcpdu",
         "https://tinycontrol.pl/en/tcpdu/downloads/#firmware",
-        {"number_of_outputs": 7},
+        fw_update_method=FWUpdateMethod.HTTP,
+        extras={"number_of_outputs": 7},
     )
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
         return hardware_version in ["1.0", "1.1"] and software_version.endswith("tcPDU")
@@ -1422,18 +1439,19 @@
 
     It's basically the same as LK4 minus outputs, PWM outputs, analog
     inputs, digital inputs, power and energy, serial port.
     """
 
     info: ClassVar[Union[DeviceInfo, None]] = DeviceInfo(
         "LK HW 4.0 mini",
-        FAMILY_LK,
+        DeviceFamily.LK,
         "lc40mini",
         "https://tinycontrol.pl/en/lk4mini/downloads/#firmware",
-        {"number_of_outputs": 0},
+        fw_update_method=FWUpdateMethod.HTTP,
+        extras={"number_of_outputs": 0},
     )
     parsers: ClassVar[List[str]] = []
 
     @classmethod
     def check_version(
         cls, hardware_version: Union[str, None], software_version: str
     ) -> bool:
@@ -1442,17 +1460,18 @@
     # Unset few commands - there are no OUT, PWM in LK4 mini
     _set_out = None
     _set_pwm = None
     _set_pwm_duty = None
     _set_pwm_freq = None
 
     def _get_all(self) -> List[str]:
+        """Prepare list of URLs to fetch data from."""
         return [
             "/api/v1/read/set/?generalConfig&networkConfig",
-            "/api/v1/read/status/?boardValues&statusValues&timeValues&dsValues&i2cValues&otherSensorsValues&diffValues&mrValues&varValues"
+            "/api/v1/read/status/?boardValues&statusValues&timeValues&dsValues&i2cValues&otherSensorsValues&diffValues&mrValues&varValues",
         ]
 
 
 DEVICE_MODELS = [
     LK_HW_40_mini,
     TCPDU,
     LK_HW_40,
```

### Comparing `tinytoolslib-0.2.5/tinytoolslib/parsers.py` & `tinytoolslib-0.3.1/tinytoolslib/parsers.py`

 * *Files identical despite different names*

### Comparing `tinytoolslib-0.2.5/tinytoolslib/requests.py` & `tinytoolslib-0.3.1/tinytoolslib/requests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
+"""Functions to send HTTP requests via requests and aiohttp modules."""
+
+import asyncio
 import json
-from typing import Union
 import socket
+from functools import wraps
+from typing import Any, Dict, Union
 from xml.etree import ElementTree
+
 import requests
-from functools import wraps
-import asyncio
-from .exceptions import (
-    TinyToolsRequestConnectionError,
-    TinyToolsRequestError,
-    TinyToolsRequestHTTPError,
-    TinyToolsRequestInternalServerError,
-    TinyToolsRequestNotFound,
-    TinyToolsRequestSSLError,
-    TinyToolsRequestTimeout,
-    TinyToolsRequestUnauthenticated,
-)
 from aiohttp import (
-    ClientSession,
     BasicAuth,
-    ClientTimeout,
     ClientConnectionError,
     ClientConnectorCertificateError,
     ClientOSError,
     ClientResponseError,
+    ClientSession,
+    ClientTimeout,
     InvalidURL,
     ServerDisconnectedError,
 )
 
+from .exceptions import (
+    TinyToolsRequestConnectionError,
+    TinyToolsRequestError,
+    TinyToolsRequestHTTPError,
+    TinyToolsRequestInternalServerError,
+    TinyToolsRequestNotFound,
+    TinyToolsRequestSSLError,
+    TinyToolsRequestTimeout,
+    TinyToolsRequestUnauthenticated,
+)
 
 DEFAULT_TIMEOUT = 3
 DEFAULT_RETRIES = 1
 
 
 def _parse_parameters(
     host, path, schema, port, username, password, timeout, retries, verify
@@ -98,15 +101,16 @@
     """Handle response content and pack it into TinyToolsResponse."""
     result = {
         "_response": response,
         "parsed": None,
     }
     # TODO: Add ping for requests method (ATM missing for aiohttp).
     if hasattr(response, "elapsed"):
-        result["ping"] = round(response.elapsed.total_seconds() * 1000, 3)
+        result["elapsed"] = response.elapsed.total_seconds()
+        result["ping"] = round(result["elapsed"] * 1000, 3)
     try:
         if content_type == "application/json":
             result["parsed"] = json.loads(content)
         elif content_type == "text/html":
             result["parsed"] = {}
         elif content_type == "text/xml":
             result["parsed"] = {
@@ -114,34 +118,39 @@
             }
     except (ElementTree.ParseError, ValueError) as exc:
         raise TinyToolsRequestError("Cannot parse response") from exc
     return result
 
 
 def request(
-    method,
-    host,
-    path,
-    schema="http",
-    port=80,
-    username="",
-    password="",
-    timeout=None,
-    retries=None,
-    verify=None,
-    data=None,
-    headers=None,
+    method: str,
+    host: str,
+    path: str,
+    schema: str = "http",
+    port: int = 80,
+    username: str = "",
+    password: str = "",
+    timeout: Union[int, None] = None,
+    retries: Union[int, None] = None,
+    verify: Union[bool, None] = None,
+    data: Union[Any, None] = None,
+    headers: Union[Dict[str, str], None] = None,
+    session: Union[requests.Session, None] = None,
 ):
     """Send request to device and return dict with response or errors."""
     url, auth, timeout, retries, verify = _parse_parameters(
         host, path, schema, port, username, password, timeout, retries, verify
     )
     response = None
     try:
-        response = requests.request(
+        if session is not None:
+            _request = session.request
+        else:
+            _request = requests.request
+        response = _request(
             method,
             url,
             auth=auth,
             data=data,
             headers=headers,
             timeout=timeout,
             verify=verify,
@@ -170,26 +179,34 @@
         return _handle_content(
             response.headers.get("content-type"), response.content, response
         )
 
 
 @wraps(request)
 def get(*args, silent=False, **kwargs):
-    """Send GET request."""
+    """Send GET request.
+
+    Accepts the same parameters as request(), except method (GET).
+    Also accepts param `silent`, defining whether to raise errors.
+    """
     try:
         return request("GET", *args, **kwargs)
     except TinyToolsRequestError:
         if silent:
             return None
         raise
 
 
 @wraps(request)
 def post(*args, **kwargs):
-    """Send POST request."""
+    """Send POST request.
+
+    Accepts the same parameters as request(), except method (POST).
+    Also sets headers.
+    """
     return request(
         "POST",
         *args,
         headers={"Content-Type": "application/x-www-form-urlencoded; charset=UTF-8"},
         **kwargs,
     )
 
@@ -255,14 +272,18 @@
     except Exception as exc:
         _handle_errors(exc, response)
     return _handle_content(response.content_type, content, response)
 
 
 @wraps(async_request)
 async def async_get(*args, silent=False, **kwargs):
-    """Send async GET request."""
+    """Send async GET request.
+
+    Accepts the same parameters as request(), except method (GET).
+    Also accepts param `silent`, defining whether to raise errors.
+    """
     try:
         return await async_request("GET", *args, **kwargs)
     except TinyToolsRequestError:
         if silent:
             return None
         raise
```

