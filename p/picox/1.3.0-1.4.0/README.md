# Comparing `tmp/picox-1.3.0.tar.gz` & `tmp/picox-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picox-1.3.0.tar", last modified: Fri May  3 20:14:54 2024, max compression
+gzip compressed data, was "picox-1.4.0.tar", last modified: Mon May 27 13:50:54 2024, max compression
```

## Comparing `picox-1.3.0.tar` & `picox-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-03 20:14:49.000000 picox-1.3.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-03 20:14:54.471385 picox-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-03 20:14:49.000000 picox-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-03 20:14:49.000000 picox-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 20:14:54.471385 picox-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.467384 picox-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/src/picox/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/logconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-05-03 20:14:49.000000 picox-1.3.0/src/picox/upy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 20:14:54.471385 picox-1.3.0/src/picox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-03 20:14:54.000000 picox-1.3.0/src/picox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.127474 picox-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-27 13:50:49.000000 picox-1.4.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-27 13:50:54.127474 picox-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-27 13:50:49.000000 picox-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-27 13:50:49.000000 picox-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 13:50:54.127474 picox-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.123474 picox-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.127474 picox-1.4.0/src/picox/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.127474 picox-1.4.0/src/picox/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/commands/compiled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/logconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14190 2024-05-27 13:50:49.000000 picox-1.4.0/src/picox/upy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.127474 picox-1.4.0/src/picox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-27 13:50:54.000000 picox-1.4.0/src/picox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 13:50:54.127474 picox-1.4.0/src/raw_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 13:50:49.000000 picox-1.4.0/src/raw_commands/DOWNLOAD_FILE.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-27 13:50:49.000000 picox-1.4.0/src/raw_commands/UPLOAD_FILE.py
```

### Comparing `picox-1.3.0/LICENCE` & `picox-1.4.0/LICENCE`

 * *Files identical despite different names*

### Comparing `picox-1.3.0/PKG-INFO` & `picox-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picox
-Version: 1.3.0
+Version: 1.4.0
 Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
 Author: Harvey
 License: MIT License
         
         Copyright (c) 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `picox-1.3.0/README.md` & `picox-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `picox-1.3.0/pyproject.toml` & `picox-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "picox"
-version = "1.3.0"
+version = "1.4.0"
 authors = [{name = "Harvey"}]
 description = "Tools for working with a Rasbperry Pi Pico running MicroPython"
 readme = "README.md"
 license = {file = "LICENCE"}
 dependencies = [
     "pyserial == 3.5",
     'pyreadline3 == 3.4.1 ; platform_system == "Windows"',
```

### Comparing `picox-1.3.0/src/picox/cli.py` & `picox-1.4.0/src/picox/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import argparse
 import logging
+import sys
+from pathlib import Path
 
 from .upy import Pico
-from .logconfig import LOGGER
 from .detect import get_all_pico_serial, get_first_pico_serial
+from .logconfig import LOGGER
 
-import argparse
 
 def get_args():
     parser = argparse.ArgumentParser(description="picox")
     parser.add_argument("-v", "--verbose", action="store_true")
 
     # parse global flags first
     args, remaining_argv = parser.parse_known_args()
@@ -80,18 +81,26 @@
         case "ls":
             for file in pico.get_file_list():
                 print(file) # Print to stdout
         case "stop":
             pass # Technically just opening it successfully will stop it
         case "upload":
             with open(args.read_file, "rb") as read_file:
-                pico.upload_file(read_file, args.file, overwrite=args.overwrite)
+                try:
+                    pico.upload_file(read_file, args.file, overwrite=args.overwrite)
+                except FileExistsError as err:
+                    LOGGER.error(err)
+                    sys.exit(2)
         case "download":
-            with open(args.save_file, "w") as save_file:
-                pico.download_file(args.file, save_file)
+            try:
+                with open(args.save_file, "w") as save_file:
+                    pico.download_file(args.file, save_file)
+            except FileNotFoundError as err:
+                LOGGER.error(err)
+                sys.exit(1)
         case "exec":
             LOGGER.debug(f"Executing {args.file}")
             pico.execute_file(args.file)
         case "detect":
             if args.all:
                 detected = get_all_pico_serial()
             else:
```

### Comparing `picox-1.3.0/src/picox/detect.py` & `picox-1.4.0/src/picox/detect.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,19 +22,21 @@
         case "Linux":
             return glob.glob('/dev/ttyACM*')
         case "Darwin":
             return glob.glob('/dev/tty.usb*')
         case _:
             raise NotImplementedError("Unsupported OS")
 
-def is_pico(device: str):
+def is_pico(device: str) -> bool:
     """
     Try to determine if USB serial device is a Pi Pico device
     args:
         device (str): USB serial device to test
+    returns:
+        bool : True/False if MicroPython passed the coms test
     """
     try:
         Pico(
             device,
             serial_read_timeout=1,
             serial_write_timeout=1,
         )
@@ -64,17 +66,19 @@
     serial_devices = get_serial_ports()
     for device in serial_devices:
         if is_pico(device):
             return device
     else:
         return None
 
-def get_all_pico_serial() -> List:
+def get_all_pico_serial() -> List[str]:
     """
     Get ports then return all detected pico devices
+    returns:
+        List[str] : List of potential Pico serial devices
     """
     serial_devices = get_serial_ports()
     pico_devices = []
     for serial_device in serial_devices:
         if is_pico(serial_device):
             pico_devices.append(serial_device)
     return pico_devices
```

### Comparing `picox-1.3.0/src/picox/upy.py` & `picox-1.4.0/src/picox/upy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import ast
 import time
 import re
 import platform
 from enum import Enum
-from typing import IO, Optional
-from itertools import cycle
+from typing import IO, Optional, List
+from pathlib import Path
+from io import StringIO
 
 import serial
 
+from .exceptions import RemotePicoException
 from .logconfig import LOGGER
-
+from .commands.compiled import DOWNLOAD_FILE, UPLOAD_FILE
 
 # Constants for communication patterns
 TERMINATOR = '\r\n'  
 UPY_PROMPT = "\r\n>>>"  
 BLOCK_PROMPT = "..."  
 EOR_MARKER = "---f81b734f-7be3-4747-ae0b-c449006b33dd---"
 EOR_TOKEN  = f"{EOR_MARKER}{UPY_PROMPT}"
 EOR_MARKER_COMMAND = f";print('{EOR_MARKER}')"
 EOM_MARKER = f';pass;pass;pass;pass{EOR_MARKER_COMMAND}'
+FAILED_MARKER = f"FAILED---0dfe99a5-4543-4fc0-8986-5d7fd5e51d7b---ERROR"
 RE_MATCH_BACKSPACE_BEGINNING = re.compile('^' + re.escape("\x08") + '+')
 
+
 class MicroPython_Version(Enum):
     """Enumeration of supported MicroPython versions."""
     v1_21_0 = "1.21.0"
 
 
 class Pico:
     """Manage communications with a MicroPython RP2040 device via serial."""
@@ -56,14 +60,16 @@
         if not start_closed:
             # Open the serial device here
             self._open_serial()
 
             # Send stop and reboot to reset Pico state
             if not skip_stop_exec:
                 self.stop_exec()
+                self._serial.reset_output_buffer()
+                self._serial.reset_input_buffer()
 
             # Run a sanity test to ensure the serial device responds as expected (e.g. does it run micropython)
             if not skip_coms_test:
                 if not self.coms_test():
                     raise IOError("Did not get expected response from device during coms test")
 
     def _open_serial(self):
@@ -71,58 +77,61 @@
         self._serial = serial.Serial(
             port=self._serial_port, 
             baudrate=115200, 
             timeout=self._serial_read_timeout,
             write_timeout=0.5
         )
 
-    def _serial_read(self, eor_token: str = EOR_TOKEN) -> bytearray:
-        """Reads from serial until the end-of-response token is encountered."""
-        response = self._serial.read_until(eor_token.encode("utf8")).strip()
-        LOGGER.debug(f"RECV {self._serial_port} :: {response}")
-        return response
+    def _serial_read(self, end_markers: List[str] = None, command_failed_marker: str = FAILED_MARKER) -> bytearray:
+        """
+        Read from serial byte-by-byte and check if we hit an end marker
+        """
+        if not end_markers:
+            end_markers = [EOR_TOKEN] # Default to end of response marker
+
+        max_failed_marker_occurances = 2 # Failure marker will show once in the command and once again if failed
+        failed_marker_occurances = 0 # Count times encountered failure markers
+
+        end_markers_encoded = list(map(lambda marker: marker.encode('utf-8'), end_markers))
+        failed_marker_encoded = command_failed_marker.encode('utf-8')
+
+        recv_buffer = b''
+        while True:
+            recv_bytes = self._serial.read()
+            if not recv_bytes:
+                break # did not recv any bytes
+
+            recv_buffer += recv_bytes
+            LOGGER.debug(f"RECV(part) {self._serial_port} :: {recv_buffer}")
+
+            # Check if the buffer ends with any of the markers
+            if any(recv_buffer.endswith(end_marker) for end_marker in end_markers_encoded):
+                break
+
+            # Check if the error marker has been hit
+            if recv_buffer.endswith(failed_marker_encoded):
+                failed_marker_occurances += 1
+                if failed_marker_occurances >= max_failed_marker_occurances:
+                    break
+    
+        recv_buffer = recv_buffer.strip()
+        LOGGER.debug(f"RECV {self._serial_port} :: {recv_buffer}")
+        return recv_buffer
     
     def _serial_read_endless(self):
         """Endless read from serial, useful for viewing all console output"""
         self._serial.timeout = 0
         while True:
-            bytes_to_read = self._serial.in_waiting
-            if data_from_serial := self._serial.read(bytes_to_read).decode("utf-8"):
+            if data_from_serial := self._serial.read(self._serial.in_waiting or 1).decode("utf-8"):
                 print(f"{data_from_serial}")
             else:
-                time.sleep(0.1)
-
-    def _repl_read(self, wait_interval: float = 0.2) -> str:
-        """Attempts to read from the REPL prompt"""
-        response = ""
-        end_markers = (UPY_PROMPT, BLOCK_PROMPT)
-        self._serial.timeout = wait_interval
-        start_time = time.monotonic()
-
-        for end_marker in cycle(end_markers):
-            if (time.monotonic() - start_time) > self._serial_read_timeout:
-                break
-            try:
-                response += self._serial_read(eor_token=end_marker).decode("utf-8")
-            except serial.SerialTimeoutException:
-                pass
-            else:
-                time.sleep(0.1)
-                if not self._serial.in_waiting:
-                    break
-
-        self._serial.timeout = self._serial_read_timeout
-        if not response:
-            raise serial.SerialTimeoutException("Timeout while reading from serial.")
-        return response
+                time.sleep(0.05)
 
     def _serial_write(self, command: bytes):
         """Writes a command to the serial port after clearing the input and output buffers."""
-        self._serial.reset_output_buffer()
-        self._serial.reset_input_buffer()
         LOGGER.debug(f"SEND {self._serial_port} :: {command}")
         self._serial.write(command)
 
     def _extract_response_payload(self, response: str, start_marker: str, end_marker: str) -> Optional[str]:
         """Extracts a payload from a response delimited by specified start and end markers."""
         last_start_index = response.rfind(start_marker)
         if last_start_index == -1:
@@ -167,18 +176,26 @@
                      ignore_response: bool = False
                      ) -> Optional[str]:
         """Handles the sending and receiving of a command to/from the MicroPython device."""
         command += EOM_MARKER + TERMINATOR
         if is_block_command:
             command += TERMINATOR
 
+        self._serial.reset_output_buffer()
+        self._serial.reset_input_buffer()
+
         self._serial_write(command.encode("utf8"))
 
         if not ignore_response:
             if response := self._serial_read().decode():
+                # Did the response show an exception on the Pico?
+                if response.endswith(FAILED_MARKER):
+                    raise RemotePicoException("Detected exception from device", response)
+                
+                # Good response, Get the payload and return it
                 return self._clean_response(response)
             else:
                 raise Exception("No response when expected")
         return None
 
     def get_file_list(self):
         """ Get a list of files stored on the device """
@@ -196,16 +213,14 @@
         """ Stop execution by a combinatino of reboot and Ctrl+C. Flushes buffers afterwards to get device in known state """
         self._send_stop_exec(quantity=5)
         self.send_soft_reboot()
         time.sleep(0.2)
         self._send_stop_exec(quantity=5) # If there is an auto boot script, this will clear it
         time.sleep(0.2)
         self._send_enter()
-        self._serial.reset_input_buffer()
-        self._serial.reset_output_buffer()
 
     def _send_stop_exec(self, quantity=1):
         """ Send keyboard interrupt to stop execution 
         args:
             quantity (int) : How many Ctrl+C to send
         """
         LOGGER.debug("Sending stop exec (Ctrl+C) to Pico")
@@ -227,72 +242,104 @@
 
     def run_python_command(self, command, block_command=False):
         """ Run a generic python command """
         return self._communicate(command, block_command)
 
     def download_file(self, pico_filename, save_fp: IO[str]):
         """ Download a file from the Pico to the host """
-        download_failed_marker = f"DOWNLOAD{EOR_MARKER}ERROR"
 
         if pico_filename not in self.get_file_list():
             raise FileNotFoundError(f"File '{pico_filename}' does not exist on Pico")
 
-        file_data = self._communicate(
-            f"exec(\"try:\\n  with open('{pico_filename}', 'r') as f: print(f.read(), end='')\\nexcept Exception as e: print(f'{download_failed_marker}{{str(e)}}')\")",
-            is_block_command=True
-        )
-        if file_data.startswith(download_failed_marker):
-            LOGGER.error(f"Upload was not successful: {file_data.replace(download_failed_marker, '')}")
-        save_fp.write(file_data)
+        try:
+            file_data = self._communicate(
+                DOWNLOAD_FILE(pico_filename)
+            )
+        except RemotePicoException as err:
+            LOGGER.error(f"Upload was not successful: {err}")
+        else:
+            # Fix line endings to \n and write to file!
+            source = StringIO(file_data)
+            normalized_lines = []
+            for line in source:
+                line = line.rstrip('\r\n') + '\n'
+                normalized_lines.append(line)
+            save_fp.write(''.join(normalized_lines))
+
+    def create_directory(self, path: Path, overwrite=False):
+        if str(path) in self.get_file_list():
+            if not overwrite:
+                raise FileExistsError(f"'{path}' already exists on the Pico. Set overwrite=True to overwrite.")
+        
+        result = self._communicate(f"import os; os.mkdir('{path}')")
+        LOGGER.debug(f"Response from mkdir: {result}")
+        if "Traceback" in result:
+            LOGGER.error(f"Pico raised Exception during upload :: {result}")
 
-    def upload_file(self, local_fp: IO[bytes], pico_file_path, overwrite=False):
+    def upload_file(self, local_fp: IO[str], pico_file_path, overwrite=False):
         """ Upload a file from the host to the Pico """
         if pico_file_path in self.get_file_list():
             if not overwrite:
                 raise FileExistsError(f"File '{pico_file_path}' already exists on the Pico. Set overwrite=True to overwrite.")
-            else:
-                self._communicate(f"import os; os.remove('{pico_file_path}')")
 
         # Read the file data from the host
         local_data = local_fp.read()
-
+        if not isinstance(local_data, bytes):
+            raise ValueError(f"File is not open in binary format got {type(local_data)}")
+        
         # Upload the file to the pico
-        result = self._communicate(
-            f'with open("{pico_file_path}", "wb") as f: f.write({local_data})',
-            is_block_command=True
-        )
-        LOGGER.debug(f"Response from upload: {result}")
-        if "Traceback" in result:
-            LOGGER.error(f"Pico raised Exception during upload :: {result}")
+        try:
+            result = self._communicate(
+                UPLOAD_FILE(local_data.hex(), pico_file_path)
+            )
+        except RemotePicoException as err:
+            LOGGER.error(f"Upload was not successful: {err}")
+            raise
+        return result
 
     def execute_file(self, file_name):
         LOGGER.debug(f"Executing file {file_name}")
         self.stop_exec()
         return self._communicate(f'exec(open("{file_name}").read())', ignore_response=True)
 
     def start_console_attach(self):
         LOGGER.info(f"Starting console read from device {self._serial_port}...")
         self._serial_read_endless()
 
     def start_repl(self):
+        end_markers = (UPY_PROMPT, BLOCK_PROMPT)
+
         # import readline to support familiar command input (arrows, history)
         if platform.system == "Windows":
             import pyreadline3
         else:
             import readline
 
+        # Get the Pico in a known state
         self.stop_exec()
+        self.send_soft_reboot()
+        time.sleep(0.5)
+        self._serial.reset_output_buffer()
+        self._serial.reset_input_buffer()
+        self.stop_exec()
+        time.sleep(0.5)
 
-        # Read serial here to get prompt
-        prompt = self._serial_read(eor_token=UPY_PROMPT).decode("utf-8")
+        prompt = self._serial_read(end_markers=[UPY_PROMPT]).decode("utf-8")
+        self._serial.reset_output_buffer()
+        self._serial.reset_input_buffer()
         while True:
             raw_command = input(f"{prompt} ")
             if raw_command == "exit()":
                 raise SystemExit
-
+            
             command = f"{raw_command}\r" # Add an enter to submit
             self._serial_write(command.encode("utf-8"))
-            prompt = self._repl_read()
+
+            prompt = self._serial_read(end_markers=end_markers).decode("utf-8")
+            
             # Sometimes a backspace character appears at the left, remove it
             prompt = re.sub(RE_MATCH_BACKSPACE_BEGINNING, "", prompt)
             # Remove the command from the response
-            prompt = prompt.replace(raw_command.strip(), "").strip()
+            prompt = prompt.replace(raw_command.strip(), "", 1).strip()
+
+            self._serial.reset_output_buffer()
+            self._serial.reset_input_buffer()
```

### Comparing `picox-1.3.0/src/picox.egg-info/PKG-INFO` & `picox-1.4.0/src/picox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picox
-Version: 1.3.0
+Version: 1.4.0
 Summary: Tools for working with a Rasbperry Pi Pico running MicroPython
 Author: Harvey
 License: MIT License
         
         Copyright (c) 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

