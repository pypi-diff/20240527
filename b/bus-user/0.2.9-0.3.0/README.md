# Comparing `tmp/bus_user-0.2.9.tar.gz` & `tmp/bus_user-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.2.9.tar", last modified: Tue Mar 19 09:20:17 2024, max compression
+gzip compressed data, was "bus_user-0.3.0.tar", last modified: Mon May 27 14:42:29 2024, max compression
```

## Comparing `bus_user-0.2.9.tar` & `bus_user-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.435155 bus_user-0.2.9/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.2.9/LICENSE
--rw-rw-rw-   0        0        0     4094 2024-03-19 09:20:17.434563 bus_user-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     3129 2024-03-19 08:55:33.000000 bus_user-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.423863 bus_user-0.2.9/bus_user/
--rw-rw-rw-   0        0        0      301 2024-03-19 06:40:12.000000 bus_user-0.2.9/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.2.9/bus_user/history.py
--rw-rw-rw-   0        0        0     3759 2024-01-31 08:51:20.000000 bus_user-0.2.9/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0    35352 2024-03-19 09:17:30.000000 bus_user-0.2.9/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      697 2024-03-19 06:40:12.000000 bus_user-0.2.9/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    23919 2024-03-19 09:18:31.000000 bus_user-0.2.9/bus_user/serial_server.py
-drwxrwxrwx   0        0        0        0 2024-03-19 09:20:17.432957 bus_user-0.2.9/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4094 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      311 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-19 09:20:17.000000 bus_user-0.2.9/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-19 09:20:17.436686 bus_user-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.898213 bus_user-0.3.0/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4169 2024-05-27 14:42:29.897215 bus_user-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2024-05-27 14:27:59.000000 bus_user-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.885728 bus_user-0.3.0/bus_user/
+-rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.0/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.0/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.0/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.0/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    39994 2024-05-27 14:36:43.000000 bus_user-0.3.0/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.0/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    19389 2024-05-27 14:25:04.000000 bus_user-0.3.0/bus_user/serial_server.py
+-rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.0/bus_user/values.py
+drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.896219 bus_user-0.3.0/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 14:42:29.899209 bus_user-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.0/setup.py
```

### Comparing `bus_user-0.2.9/LICENSE` & `bus_user-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.9/PKG-INFO` & `bus_user-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.2.9
+Version: 0.3.0
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,21 +16,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.2.9)
+# bus_user (v0.3.0)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
-### !. MOST APPROPRIATE COMMAND PROTOCOL
+###
+NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
+    
+!. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
 
 1. all cmds must be as params (preferred) in equipment or as special command
 2. [<CMD_NAME>] - read param value or run special command  
     [IDN] - read value IDN  
     [DUMP] - run special command 
 3. [<CMD_NAME> <VALUE>] - write value in parameter or run special cmd with param  
@@ -44,15 +47,15 @@
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
 1. Serial:  
 	- Client+Server  
-	- connect with AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
+	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
 2. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results
```

### Comparing `bus_user-0.2.9/README.md` & `bus_user-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
-# bus_user (v0.2.9)
+# bus_user (v0.3.0)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
-### !. MOST APPROPRIATE COMMAND PROTOCOL
+###
+NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
+    
+!. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
 
 1. all cmds must be as params (preferred) in equipment or as special command
 2. [<CMD_NAME>] - read param value or run special command  
     [IDN] - read value IDN  
     [DUMP] - run special command 
 3. [<CMD_NAME> <VALUE>] - write value in parameter or run special cmd with param  
@@ -22,15 +25,15 @@
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
 1. Serial:  
 	- Client+Server  
-	- connect with AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
+	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
 2. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results
```

### Comparing `bus_user-0.2.9/bus_user/history.py` & `bus_user-0.3.0/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.2.9/bus_user/i2c_client.py` & `bus_user-0.3.0/bus_user/i2c_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # REQUIREMENTS ========================================================================================================
 # decide what to do with it!!!
 from requirements_checker import ReqCheckStr_Os
-ReqCheckStr_Os.check_is__LINUX()
+ReqCheckStr_Os.raise_if__WINDOWS()
 
 
 # IMPORT ==============================================================================================================
-from smbus2 import SMBus
-import re
 from typing import *
+import re
+from smbus2 import SMBus
 
 from object_info import ObjectInfo
 from cli_user import CliUser
 
 
 # =====================================================================================================================
 class Exx_I2cConnection(Exception):
```

### Comparing `bus_user-0.2.9/bus_user/serial_client.py` & `bus_user-0.3.0/bus_user/serial_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 import re
 import sys
 import glob
 import time
 from typing import *
 from enum import Enum, auto
 
+from object_info import ObjectInfo
+from logger_aux import Logger
+
 from serial import Serial
 from serial.tools import list_ports
 
-from object_info import ObjectInfo
-
-from .history import HistoryIO
+from . import HistoryIO
 
 
 # =====================================================================================================================
 class Exx_SerialAddress_NotConfigured(Exception):
     """
         raise SerialException("Port must be configured before it can be used.")
     serial.serialutil.SerialException: Port must be configured before it can be used.
@@ -41,14 +42,21 @@
 class Exx_SerialAddress_AlreadyOpened(Exception):
     """
     SerialException("could not open port 'COM7': PermissionError(13, 'Отказано в доступе.', None, 5)")
     """
     pass
 
 
+class Exx_SerialAddress_AlreadyOpened_InOtherObject(Exception):
+    """
+    SerialException("could not open port 'COM7': PermissionError(13, 'Отказано в доступе.', None, 5)")
+    """
+    pass
+
+
 class Exx_SerialAddress_OtherError(Exception):
     """
     SerialException("could not open port 'COM7': OSError(22, 'Указано несуществующее устройство.', None, 433)") - порт есть, но получена ошибка при открытии!!!
     """
     pass
 
 
@@ -59,75 +67,91 @@
 class Exx_SerialRead_FailPattern(Exception):
     """
     if read string which match error pattern
     """
     pass
 
 
+class Exx_SerialRead_FailDecoding(Exception):
+    """
+    REASON
+    ------
+    some serial devices (depends on microchips model) not always give correct reading bytes
+
+    SOLVATION
+    ---------
+    1. [BESTandONLY] just use other device on other appropriate microchip!
+    """
+
+
 class Exx_SerialPL2303IncorrectDriver(Exception):
     """
     REASON
-    ======
+    ------
     typical for windows
 
     SOLVATION
-    ===========
-    install last drivers
-    manually select other more OLD driver in manager (see from PC)
+    ---------
+    1. [BEST] just use other device on other microchip
+    2. manually select other more OLD driver in driver/device manager
         version 3.3.2.105/27.10.2008 - is good!
         version 3.8.22.0/22.02.2023 - is not good!!!
     """
     MARKER: str = "PL2303HXA PHASED OUT SINCE 2012. PLEASE CONTACT YOUR SUPPLIER"
 
 
 # =====================================================================================================================
 TYPE__RW_ANSWER = Union[None, str, List[str]]
 
 
-class TypeWrReturn(Enum):
+class Type__WrReturn(Enum):
     ALL_OUTPUT = auto()
     HISTORY_IO = auto()
     DICT = auto()
 
 
-class AddressAutoAcceptVariant(Enum):
+class Type__AddressAutoAcceptVariant(Enum):
     FIRST_FREE = auto()
     FIRST_FREE__SHORTED = auto()
+    FIRST_FREE__PAIRED = auto()
     FIRST_FREE__ANSWER_VALID = auto()
-    FIRST_FREE__PAIRED_FOR_EMU = auto()
 
 
-TYPE__ADDRESS = Union[None, AddressAutoAcceptVariant, str]
+TYPE__ADDRESS = Union[None, Type__AddressAutoAcceptVariant, str]
 
 
 # =====================================================================================================================
-class SerialClient:
+class SerialClient(Logger):
     """
 
     NOTE:
     1. use good COM-port adapters!!!
         some bites may be lost (usually on started byte) or added extra chars (usually to start and end of line)!!!
 
+        DECODING APPROPRIATE MODELS
+        ---------------------------
         =WRONG=
-        - PROFILIC - often!
-        - FTDI FT232RL - sometimes but less than on Profilic
+        - PROFILIC - often +wrong driver
+        - FTDI FT232RL - sometimes but less than on Profilic=fail on step 0/11/20/3 3/9/95!!!
+        - CP2102 - fail on step 3392/877/1141/!!! sometimes on step 1715 get SerialTimeoutException
 
         =GOOD=
         - CH340 - no one error so far!
-        - CH341A (big universal) - no one error so far!
+        - CH341A (big universal) - no one error so far! more then steps about 50 minutes!!! tired of waiting
 
-        =NOT TESTED= wait postage from Aliexpress
-        - CP2102
+        =NOT TESTED= wait postage from Aliexpress - already get! need tests!!! use Test__Shorted_validateModel_InfinitRW!!!!
         - CH341T
     """
-    # TODO: use thread!???
     pass
     pass
     pass
 
+    # LOGGER --------------------------------------------------
+    # LOG_ENABLE = True
+
     # SETTINGS ------------------------------------------------
     ADDRESS: TYPE__ADDRESS = None
 
     TIMEOUT__READ: float = 0.3       # 0.2 is too short!!! dont touch! in case of reading char by char 0.5 is the best!!! 0.3 is not enough!!!
     # need NONE NOT 0!!! if wait always!!
     BAUDRATE: int = 9600        # 115200
 
@@ -145,16 +169,17 @@
     ENCODING: str = "utf8"
     EOL__SEND: bytes = b"\r\n"      # "\r"=ENTER in PUTTY  but "\r\n"=is better in read Putty!
     EOL__UNI_SET: bytes = b"\r\n"
 
     _GETATTR_STARTSWITH__SEND: str = "send__"
 
     # test purpose EMULATOR -----------------
-    _EMULATOR: 'SerialServer_Base' = None    # IF USED - START it on PAIRED - it is exactly Emulator/Server! no need to use just another serialClient! _EMULATOR could be used for test reason and check values in realtime!!
-    _EMULATOR_START: bool = None    # DONT DELETE! it need when you reconnecting! cause of ADDRESS replaced after disconnecting by exact str after PAIRED*
+    _EMULATOR__CLS: Type['SerialServer_Base'] = None    # IF USED - START it on PAIRED - it is exactly Emulator/Server! no need to use just another serialClient! _EMULATOR__INST could be used for test reason and check values in realtime!!
+    _EMULATOR__INST: 'SerialServer_Base' = None
+    _EMULATOR__START: bool = None    # DONT DELETE! it need when you reconnecting! cause of ADDRESS replaced after disconnecting by exact str after PAIRED*
 
     # AUX -----------------------------------------------------
     history: HistoryIO = None
     _SERIAL: Serial
 
     ADDRESSES__SYSTEM: List[str] = []
     ADDRESSES__SHORTED: List[str] = []
@@ -178,19 +203,21 @@
         # self.addresses_system__detect()   # DONT USE in init!!!
         # self.addresses_shorted__detect()   # DONT USE in init!!!
         # self.addresses_paired__detect()   # DONT USE in init!!!
 
     def __del__(self):
         self.disconnect()
 
-    # MSG =============================================================================================================
-    def msg_log(self, msg: str = None) -> None:
-        msg = f"[{self._SERIAL.port}]{msg}"
-        print(msg)
+    def check__connected(self) -> bool:
+        try:
+            return self._SERIAL.is_open
+        except:
+            return False
 
+    # =================================================================================================================
     def cmd_prefix__set(self) -> None:
         """
         OVERWRITE IF NEED/USED!
         """
         # self.PREFIX = ""
         return
 
@@ -204,66 +231,75 @@
     def disconnect(self) -> None:
         try:
             self._SERIAL.close()
         except:
             pass
 
         try:
-            self._EMULATOR.disconnect()
+            self._EMULATOR__INST.disconnect()
         except:
             pass
 
     def connect(
             self,
             address: Optional[str] = None,
             _raise: Optional[bool] = None,
-            _silent: Optional[bool] = None,
-            _dont_start_emu: bool = None    # specially keep ability to connect without Emu on cls main perpose (search ports)!
+            _touch_connection: bool | None = None    # no final connection! specially keep ability to connect without Emu on cls main perpose (search ports)!
     ) -> Union[bool, NoReturn]:
         msg = None
         exx = None
 
         # SETTINGS ---------------------------------
         if _raise is None:
             _raise = self.RAISE_CONNECT
 
-        address = address or self.ADDRESS
+        if address is None:
+            address = self.ADDRESS
 
+        # AUTOAPPLY ---------------------------------
         if address is None:
-            msg = Exx_SerialAddress_NotConfigured
+            msg = "Exx_SerialAddress_NotConfigured"
             exx = Exx_SerialAddress_NotConfigured()
-        elif address == AddressAutoAcceptVariant.FIRST_FREE:
-            return self._address_apply__first_free()
-        elif address == AddressAutoAcceptVariant.FIRST_FREE__SHORTED:
-            return self._address_apply__first_free__shorted()
-        elif address == AddressAutoAcceptVariant.FIRST_FREE__ANSWER_VALID:
-            return self._address_apply__first_free__answer_valid()
-        elif address == AddressAutoAcceptVariant.FIRST_FREE__PAIRED_FOR_EMU:
-            return self._address_apply__first_free__paired_for_emu()
-
-        elif isinstance(address, str):
-            # CHANGE PORT OR USE SAME ---------------------------------
-            if self._SERIAL.port != address:
-                if self._SERIAL.is_open:
-                    self._SERIAL.close()
-                self._SERIAL.port = address
-                if self._SERIAL.is_open:
-                    self._SERIAL.port = None
-                    # this is Attempt to connect to already opened port
-                    return False
 
-            else:
-                if self._SERIAL.is_open:
-                    return True
+        elif address == Type__AddressAutoAcceptVariant.FIRST_FREE:
+            address = self.address_get__first_free()
+        elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__SHORTED:
+            address = self.address_get__first_free__shorted()
+        elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__ANSWER_VALID:
+            address = self.address_get__first_free__answer_valid()
+        elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED:
+            address = self.address_get__first_free__paired()
+
+        # need_open ==========================================================
+        # CHANGE PORT OR USE SAME ---------------------------------
+        need_open = True
+        if self._SERIAL.port != address:
+            # close old
+            if self._SERIAL.is_open:
+                self._SERIAL.close()
+
+            # set new
+            self._SERIAL.port = address
+            if self._SERIAL.is_open:
+                self._SERIAL.port = None
+                msg = f"[ERROR] Attempt to connect to already opened port IN OTHER OBJECT {self._SERIAL}"
+                exx = Exx_SerialAddress_AlreadyOpened_InOtherObject(msg)
 
+                need_open = False
+        else:
+            if self._SERIAL.is_open:
+                need_open = False
+
+        # Try OPEN ===================================================================
+        if need_open:
             try:
                 self._SERIAL.open()
             except Exception as _exx:
-                if not _silent:
-                    self.msg_log(f"{_exx!r}")
+                if not _touch_connection:
+                    self.LOGGER.error(f"[{self._SERIAL.port}]{_exx!r}")
 
                 if "FileNotFoundError" in str(_exx):
                     msg = f"[ERROR] PORT NOT EXISTS IN SYSTEM {self._SERIAL}"
                     exx = Exx_SerialAddress_NotExists(repr(_exx))
 
                     # self.detect_available_ports()
 
@@ -278,95 +314,137 @@
                 else:
                     msg = f"[ERROR] PORT OTHER ERROR {self._SERIAL}"
                     exx = Exx_SerialAddress_OtherError(repr(_exx))
 
         # FINISH -----------------------------------------------
         # FAIL -----------------------------
         if exx:
-            if not _silent:
-                self.msg_log(msg)
+            if not _touch_connection:
+                self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
 
             if _raise:
                 raise exx
             else:
                 return False
 
         # OK -----------------------------
-        if not _silent:
-            msg = f"[OK] connected {self._SERIAL}"
-            self.msg_log(msg)
-
-        self.cmd_prefix__set()
-        # ObjectInfo(self._SERIAL, log_iter=True).print()
-        # exit()
         self.ADDRESS = self._SERIAL.port
 
-        if not _dont_start_emu:
+        if not _touch_connection:
+            if not self.connect__validation():
+                self.disconnect()
+                return False
+            self.LOGGER.info(f"[{self._SERIAL.port}][OK] connected {self._SERIAL}")
             self.emulator_start()
 
-        self._clear_buffer_read()
+        self.cmd_prefix__set()
         return True
 
-    def emulator_start(self):
-        if self._EMULATOR and self._EMULATOR_START:
-            pair_used = self.addresses_paired__get_used()
-            if pair_used:
-                self._EMULATOR.SERIAL_CLIENT.ADDRESS = pair_used[1]
-                self._EMULATOR.start()
-                self._EMULATOR.wait__monitor_ready()
+    def connect__validation(self) -> bool:
+        """
+        DIFFERENCE
+        ----------
+        connect validation used always!
+        address validation used only in step of detecting address (after execution address would be set to exact string value)
+        """
+        return True
+
+    def emulator_start(self) -> None:
+        if not self._EMULATOR__START:
+            return
+
+        if self._EMULATOR__CLS:
+            self._EMULATOR__INST = self._EMULATOR__CLS(self.address_paired__get())
+
+        if self._EMULATOR__INST.connect():
+            self._EMULATOR__INST.start()
+            self._EMULATOR__INST.wait__cycle_active()
+            self._clear_buffer_read()
 
     # ADDRESS =========================================================================================================
+    """
+    THIS IS USED for applying by SIMPLE WAY just exact address! 
+    """
     pass
     pass
     pass
     pass
     pass
     pass
     pass
 
-    def _address_apply__first_free(self) -> bool:
+    # dont move to CLASSMETHOD!!!
+    def address_get__first_free(self) -> str | None:
+        result = None
         for address in self.addresses_system__detect():
-            if self.connect(address=address, _raise=False):
-                return True
+            if self.connect(address=address, _raise=False, _touch_connection=True):
+                result = address
+
+            self.disconnect()
+            if result:
+                break
+
+        msg = f"[{result=}]_address_apply__first_free"
+        if result:
+            self.LOGGER.info(msg)
+        else:
+            self.LOGGER.warn(msg)
 
-        msg = Exx_SerialAddresses_NoVacant
-        print(msg)
+        return result
 
-    def _address_apply__first_free__shorted(self) -> bool:
+    def address_get__first_free__shorted(self) -> str | None:
         """
         dont overwrite! dont mess with address__autodetect_logic!
         used to find exact device in all comport by some special logic like IDN/NAME value
         """
+        result = None
         for address in self.addresses_shorted__detect():
-            if self.connect(address=address, _raise=False, _dont_start_emu=True):
-                return True
+            if self.connect(address=address, _raise=False, _touch_connection=True):
+                result = address
 
-        # FINISH -------------
-        msg = Exx_SerialAddresses_NoAutodetected
-        print(msg)
+            self.disconnect()
+            if result:
+                break
+
+        msg = f"[{result=}]_address_apply__first_free__shorted"
+        if result:
+            self.LOGGER.info(msg)
+        else:
+            self.LOGGER.warn(msg)
 
-    def _address_apply__first_free__answer_valid(self) -> bool:
+        return result
+
+    def address_get__first_free__answer_valid(self) -> str | None:
         """
         dont overwrite! dont mess with address__autodetect_logic!
         used to find exact device in all comport by some special logic like IDN/NAME value
         """
+        result = None
         for address in self.addresses_system__detect():
-            if self.connect(address=address, _raise=False):
+            if self.connect(address=address, _raise=False, _touch_connection=True):
                 try:
                     if self.address__answer_validation():
-                        return True
-                except:
+                        result = address
+                except Exception as exx:
+                    print(f"finding address {exx!r}")
                     pass
+
                 self.disconnect()
+                if result:
+                    break
 
-        # FINISH -------------
-        msg = Exx_SerialAddresses_NoAutodetected
-        print(msg)
+        msg = f"[{result=}]_address_apply__first_free__answer_valid"
+        if result:
+            self.LOGGER.info(msg)
+        else:
+            self.LOGGER.warn(msg)
+
+        return result
 
-    def _address_apply__first_free__paired_for_emu(self) -> bool:
+    def address_get__first_free__paired(self) -> str | None:
         """
         # FIXME: exists weakness - you need connect at once whole pair!
             if you would use several pairs and delay connecting secondary devices - it will be incorrect pairing!
             may be need using naming pairs! and set pair name with connecting first
             first connects on free port, second connect by pair name??? feels good
         cls.pairs = {
             0: (COM1, COM2),
@@ -374,51 +452,61 @@
         }
 
         cls.pairs = {
             "ATC": (COM1, COM2),    # change name
             1: (COM3, COM4),
         }
         """
+        result = None
         for pair in self.addresses_paired__detect():
-            address = pair[0]
-            if self.connect(address=address, _raise=False):
-                return True
+            for address in pair:
+                if self.connect(address=address, _raise=False, _touch_connection=True):
+                    result = address
+
+                self.disconnect()
+                if result:
+                    break
 
         # FINISH -------------
-        msg = Exx_SerialAddresses_NoAutodetected
-        print(msg)
+        msg = f"[{result=}]address_get__first_free__paired"
+        if result:
+            self.LOGGER.info(msg)
+        else:
+            self.LOGGER.warn(msg)
+
+        return result
 
     # -----------------------------------------------------------------------------------------------------------------
-    def address__answer_validation(self) -> Union[bool, NoReturn]:
+    def address__answer_validation(self) -> bool | None | NoReturn:
         """
         overwrite for you case!
         used to find exact device in all comport by some special logic like IDN/NAME value.
 
         IDEA:
         1. this func will exec on every accessible address
         2. if this func return True - address would be accepted!
         3. raiseExx/NoReturn - equivalent as False!
         """
 
-    def address__answer_validation__shorted(self) -> Union[bool, NoReturn]:
-        LOAD = "CHECK_SHORTED"
-        return self.write_read_line_last(LOAD) == LOAD
+    def address__answer_validation__shorted(self) -> bool | None:
+        load = "EXPECT_ANSWER__SHORTED"
+        return self.write_read_line_last(load) == load
 
     # DETECT PORTS ====================================================================================================
     pass
     pass
     pass
     pass
     pass
     pass
     pass
 
     def address__check_exists(self) -> bool:
         try:
-            self.connect(_raise=True, _silent=True, _dont_start_emu=True)
+            self.connect(_raise=True, _touch_connection=True)
             self.disconnect()
         except Exx_SerialAddress_NotExists:
             return False
         except:
             return False
         return True
 
@@ -503,15 +591,15 @@
             ====================================================================================================
         """
         result: List[str] = []
 
         # find not opened ports ----------------------------------------
         for obj in list_ports.comports():
             # ObjectInfo(obj).print(hide_skipped=True, hide_build_in=True)
-            result.append(obj.name)
+            result.append(obj.device)
             if Exx_SerialPL2303IncorrectDriver.MARKER in str(obj):
                 msg = f'[WARN] incorrect driver [{Exx_SerialPL2303IncorrectDriver.MARKER}]'
                 print(msg)
                 raise Exx_SerialPL2303IncorrectDriver(msg)
         return result
 
     @staticmethod
@@ -546,63 +634,80 @@
         if SerialClient.ADDRESSES__SHORTED:
             return SerialClient.ADDRESSES__SHORTED
 
         # WORK ----------------------------------------------
         result = []
         for address in cls.addresses_system__detect():
             obj = cls()
-            if obj.connect(address=address, _raise=False, _dont_start_emu=True):
+            if obj.connect(address=address, _raise=False, _touch_connection=True):
                 if obj.address__answer_validation__shorted():
                     result.append(address)
                 obj.disconnect()
 
         SerialClient.ADDRESSES__SHORTED = result
         print(f"{cls.ADDRESSES__SHORTED=}")
         return result
 
     @classmethod
-    def addresses_paired__detect(cls) -> List[Tuple[str, str]]:
+    def addresses_paired__detect(cls) -> list[tuple[str, str]]:
         # print(f"111111{cls.ADDRESSES__PAIRED=}")
 
         if SerialClient.ADDRESSES__PAIRED:
             return SerialClient.ADDRESSES__PAIRED
 
         # WORK ----------------------------------------------
-        echo_load = "ECHO_LOAD"
+        load = "EXPECT_ANSWER__PAIRED"
         result = []
         instances_free = []
-        for address in cls.addresses_system__detect():
+
+        addresses__system = cls.addresses_system__detect()
+        for address in addresses__system:
             instance = cls(address)
-            if instance.connect(_raise=False, _dont_start_emu=True):
+            if instance.connect(_raise=False, _touch_connection=True):
                 instances_free.append(instance)
 
-        while instances_free:
+        while len(instances_free) > 1:
             main = instances_free.pop(0)
-            main._write_line(echo_load)
+            main._write_line(load)
+            main.disconnect()
+
             for index, slave in enumerate(instances_free):
-                if slave.read_line(_timeout=0.3) == echo_load:
+                if slave.read_line(_timeout=0.3) == load:
                     result.append((main.ADDRESS, slave.ADDRESS))
                     slave.disconnect()
                     instances_free.pop(index)
                     break
 
-            main.disconnect()
-
         for remain in instances_free:
             remain.disconnect()
 
-        SerialClient.ADDRESSES__PAIRED = result
+        cls.ADDRESSES__PAIRED = result
         print(f"{cls.ADDRESSES__PAIRED=}")
         return result
 
     def addresses_paired__get_used(self) -> Optional[Tuple[str, str]]:
         for pair in self.addresses_paired__detect():
             if self._SERIAL.port in pair:
                 return pair
 
+    def address_paired__get(self) -> str | None:
+        if not self.ADDRESSES__PAIRED:
+            self.addresses_paired__detect()
+
+        if not isinstance(self.ADDRESS, str):
+            return
+
+        for pair in self.ADDRESSES__PAIRED:
+            if self.ADDRESS in pair:
+                addr1, addr2 = pair
+                if self.ADDRESS == addr1:
+                    return addr2
+                else:
+                    return addr1
+
     # COUNTS -----------------------------------------
     @classmethod
     def addresses_system__count(cls) -> int:
         return len(cls.addresses_system__detect())
 
     @classmethod
     def addresses_shorted__count(cls) -> int:
@@ -617,14 +722,37 @@
     pass
     pass
     pass
     pass
     pass
     pass
 
+    # CMD -------------------------------------------------------------------------------------------------------------
+    def _create_cmd_line(self, cmd: Any, prefix: Optional[str] = None, args: List[Any] = None, kwargs: Dict[str, Any] = None) -> str:
+        result = ""
+
+        cmd = str(cmd)
+
+        if prefix is None:
+            prefix = self.PREFIX
+
+        if prefix and not cmd.startswith(prefix):
+            result += f"{prefix}"
+
+        result += f"{cmd}"
+
+        if args:
+            for arg in args:
+                result += f" {arg}"
+
+        if kwargs:
+            for name, value in kwargs.items():
+                result += f" {name}={value}"
+        return result
+
     # SUCCESS ---------------------------------------------------------------------------------------------------------
     def answer_is_success(self, data: AnyStr) -> bool:
         data = self._data_ensure__string(data)
         return self.ANSWER_SUCCESS.upper() == data.upper()
 
     def answer_is_fail(self, data: AnyStr, _raise: Optional[bool] = None) -> Union[bool, NoReturn]:
         if _raise is None:
@@ -636,22 +764,22 @@
         else:
             patterns = self.ANSWER_FAIL_PATTERN
 
         for pattern in patterns:
             if re.search(pattern, data, flags=re.IGNORECASE):
                 if _raise:
                     msg = f"[ERROR] match fail [{pattern=}/{data=}]"
-                    self.msg_log(msg)
+                    self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
                     raise Exx_SerialRead_FailPattern(msg)
                 else:
                     return True
 
         return False
 
-    # BYTES -------------------------------------------------------------------------------------------------------
+    # BYTES -----------------------------------------------------------------------------------------------------------
     @classmethod
     def _bytes_eol__ensure(cls, data: bytes) -> bytes:
         if not data.endswith(cls.EOL__SEND):
             data = data + cls.EOL__SEND
         return data
 
     @classmethod
@@ -678,20 +806,38 @@
         if isinstance(data, bytes):
             return data
         else:
             return bytes(data, encoding=cls.ENCODING)
 
     @classmethod
     def _data_ensure__string(cls, data: AnyStr) -> Union[str, NoReturn]:
-        if isinstance(data, bytes):
-            return data.decode(encoding=cls.ENCODING)
-        else:
-            return str(data)
+        """
+        EXCEPTION ORIGINAL VARIANT
+        --------------------------
+            cls = <class 'test__serial_server.Victim'>, data = b'\x85RR__NAME_CMD_OR_PARAM'
+
+                @classmethod
+                def _data_ensure__string(cls, data: AnyStr) -> Union[str, NoReturn]:
+                    if isinstance(data, bytes):
+            >           return data.decode(encoding=cls.ENCODING)
+            E           UnicodeDecodeError: 'utf-8' codec can't decode byte 0x85 in position 0: invalid start byte
+
+            bus_user\serial_client.py:722: UnicodeDecodeError
+        """
+        try:
+            if isinstance(data, bytes):
+                return data.decode(encoding=cls.ENCODING)
+            else:
+                return str(data)
+        except Exception as exx:
+            print(f"{exx!r}")
+            msg = f"[FAIL] decoding {data=}"
+            raise Exx_SerialRead_FailDecoding(msg)
 
-    # RW --------------------------------------------------------------------------------------------------------------
+    # R ---------------------------------------------------------------------------------------------------------------
     # TODO: use wrapper for connect/disconnect!??? - NO!
     def read_lines(self, _timeout: Optional[float] = None) -> Union[List[str], NoReturn]:
         result: List[str] = []
         while True:
             line = self.read_line(_timeout)
             if line:
                 result.append(line)
@@ -741,32 +887,35 @@
             else:
                 msg = f"[OK]read_line={data}"
 
         else:
             msg = f"[WARN]BLANK read_line={data}"
 
         if data:
-            self.msg_log(msg)
+            self.LOGGER.info(f"[{self._SERIAL.port}]{msg}")
 
         data = self._bytes_edition__apply(data)
         data = self._bytes_eol__clear(data)
         data = self._data_ensure__string(data)
         self.history.add_output(data)
         self.answer_is_fail(data)
         return data
 
+    # W ---------------------------------------------------------------------------------------------------------------
     def _write_line(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None
     ) -> bool:
         """
         just send data into bus!
+        usually we dont need just send without reading! so it useful for debugging
+
         :return: result of sent
 
         args/kwargs - used only for single line!!!
         """
         args = args or []
         kwargs = kwargs or {}
 
@@ -787,21 +936,21 @@
         self.history.add_input(self._data_ensure__string(data))
 
         data = self._data_ensure__bytes(data)
         data = self._bytes_eol__ensure(data)
 
         data_length = self._SERIAL.write(data)
         msg = f"[OK]write_line={data}/{data_length=}"
-        self.msg_log(msg)
+        self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
 
         if data_length > 0:
             return True
         else:
             msg = f"[ERROR] data not write"
-            self.msg_log(msg)
+            self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
             return False
 
     def write_read_line(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
@@ -846,37 +995,14 @@
         if you need to read all params from device!
         """
         cmds = cmds or self.CMDS_DUMP
         history = self.write_read_line(cmds)
         history.print_io()
         return history
 
-    # CMD =============================================================================================================
-    def _create_cmd_line(self, cmd: Any, prefix: Optional[str] = None, args: List[Any] = None, kwargs: Dict[str, Any] = None) -> str:
-        result = ""
-
-        cmd = str(cmd)
-
-        if prefix is None:
-            prefix = self.PREFIX
-
-        if prefix and not cmd.startswith(prefix):
-            result += f"{prefix}"
-
-        result += f"{cmd}"
-
-        if args:
-            for arg in args:
-                result += f" {arg}"
-
-        if kwargs:
-            for name, value in kwargs.items():
-                result += f" {name}={value}"
-        return result
-
     # =================================================================================================================
     def __getattr__(self, item: str) -> Callable[..., Union[str, NoReturn]]:
         """if no exists attr/meth
 
         USAGE COMMANDS MAP
         ==================
```

### Comparing `bus_user-0.2.9/bus_user/serial_derivatives.py` & `bus_user-0.3.0/bus_user/serial_derivatives.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import *
 
 
-from .serial_client import SerialClient, AddressAutoAcceptVariant
+from .serial_client import SerialClient, Type__AddressAutoAcceptVariant
 from .serial_server import SerialServer_Base, SerialServer_Example
 
 
 # =====================================================================================================================
 class SerialClient_Shorted(SerialClient):
-    ADDRESS = AddressAutoAcceptVariant.FIRST_FREE__SHORTED
+    ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__SHORTED
 
 
 class SerialClient_Emulated(SerialClient):
-    ADDRESS = AddressAutoAcceptVariant.FIRST_FREE__PAIRED_FOR_EMU
-    _EMULATOR = SerialServer_Example()
-    _EMULATOR_START = True
+    ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED
+    _EMULATOR__CLS = SerialServer_Example
+    _EMULATOR__START = True
 
 
 # =====================================================================================================================
```

### Comparing `bus_user-0.2.9/bus_user/serial_server.py` & `bus_user-0.3.0/bus_user/serial_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,198 +1,25 @@
-from .serial_client import SerialClient, AddressAutoAcceptVariant, TYPE__ADDRESS
+from bus_user import *
 
 from typing import *
 import time
 import re
-from enum import Enum
+import logging
+import datetime
+
 from object_info import ObjectInfo
 from PyQt5.QtCore import QThread
 
-
 import funcs_aux
 
 
 # =====================================================================================================================
 TYPE__CMD_RESULT = Union[str, List[str]]
 
 
-class Value_NotPassed:
-    """
-    resolve not passed parameters in case of None value!
-
-    special object used as value to show that parameter was not passed!
-    dont pass it directl! keep it only as default parameter in class and in methods instead of None Value!
-    it used only in special cases! not always even in one method!!!
-    """
-    pass
-    # @classmethod
-    # def __str__(self):
-    #     return ""     # it used as direct Class! without any instantiation!
-
-
-# =====================================================================================================================
-class Value_WithUnit:
-    """
-    used to keep separated value and measure unit
-    """
-    value: Union[int, float] = 0
-    UNIT: str = ""
-    SEPARATOR: str = ""
-
-    # TODO: add arithmetic/comparing magic methods like SUM/...
-    # TODO: move to funcs_aux
-
-    def __init__(self, value: Union[int, float, Any] = None, unit: str = None, separator: str = None):
-        """
-        :param value: expecting number (int/float) in any form (str/any other object)!
-        """
-        # FIXME: create class without INIT! with changeable type!!!
-        if value is not None:
-            self.value = float(value)
-            try:
-                if float(value) == int(value):
-                    self.value = int(value)
-            except:
-                pass
-        if unit is not None:
-            self.UNIT = unit
-        if separator is not None:
-            self.SEPARATOR = separator
-
-    def __str__(self) -> str:
-        return f"{self.value}{self.SEPARATOR}{self.UNIT}"
-
-    def __repr__(self) -> str:
-        """
-        used as help
-        """
-        return f"{self.value}'{self.UNIT}'"
-
-    def __eq__(self, other):
-        # DONT USE JUST str()=str() separator is not valuable! especially for digital values
-        if isinstance(other, Value_WithUnit):
-            return (self.value == other.value) and (self.UNIT == other.UNIT)
-        else:
-            return self.value == other
-
-    def __ne__(self, other):
-        return not self == other
-
-
-# =====================================================================================================================
-class Exx__ValueNotInVariants(Exception):
-    pass
-
-
-class Exx__VariantsIncompatible(Exception):
-    pass
-
-
-class Value_FromVariants:
-    """
-    used to keep separated value and measure unit
-    """
-    # TODO: move to funcs_aux
-    # TODO: combine with Value_WithUnit - just add ACCEPTABLE(*VARIANTS) and rename UNIT just as SUFFIX!
-
-    # SETTINGS -----------------------
-    CASE_INSENSITIVE: bool = True
-    VARIANTS: List[Any] = None
-
-    # DATA ---------------------------
-    __value: Any = Value_NotPassed   # changeable   # TODO: default as first in variant! or pass exact value!
-
-    def __init__(self, value: Union[str, Any] = Value_NotPassed, variants: List[Union[str, Any]] = None, case_insensitive: bool = None):
-        """
-        :param value: None mean NotSelected/NotSet!
-            if you need set None - use string value in any case! 'None'/NONE/none
-        """
-        # FIXME: need think about None value!
-        # settings ---------------
-        if case_insensitive is not None:
-            self.CASE_INSENSITIVE = case_insensitive
-        if variants is not None:
-            self.VARIANTS = variants
-
-        # work ---------------
-        self._variants_validate()
-
-        if value != Value_NotPassed:
-            self.value = value
-
-    def __str__(self) -> str:
-        return f"{self.value}"
-
-    def __repr__(self) -> str:
-        """
-        used as help
-        """
-        return f"{self.value}{self.VARIANTS}"
-
-    def __eq__(self, other):
-        if isinstance(other, Value_FromVariants):
-            other = other.value
-
-        # todo: decide is it correct using comparing by str()??? by now i think it is good enough! but maybe add it as parameter
-        if self.CASE_INSENSITIVE:
-            return (self.value == other) or (str(self.value).lower() == str(other).lower())
-        else:
-            return (self.value == other) or (str(self.value) == str(other))
-
-    def __ne__(self, other):
-        return not self == other
-
-    def __len__(self):
-        return len(self.VARIANTS)
-
-    def __iter__(self):
-        yield from self.VARIANTS
-
-    def __contains__(self, item):
-        """
-        used to check compatibility
-        """
-        for variant in self.VARIANTS:
-            if self.CASE_INSENSITIVE:
-                result = str(variant).lower() == str(item).lower()
-            else:
-                result = str(variant) == str(item)
-            if result:
-                return True
-
-        return False
-
-    def _variants_validate(self) -> Optional[NoReturn]:
-        if self.CASE_INSENSITIVE:
-            real_len = len(set(map(lambda item: str(item).lower(), self.VARIANTS)))
-        else:
-            real_len = len(set(self.VARIANTS))
-
-        result = real_len == len(self.VARIANTS)
-        if not result:
-            raise Exx__VariantsIncompatible()
-
-    @property
-    def value(self) -> Any:
-        return self.__value
-
-    @value.setter
-    def value(self, value: Any) -> None:
-        for variant in self.VARIANTS:
-            if self.CASE_INSENSITIVE:
-                result = str(variant).lower() == str(value).lower()
-            else:
-                result = str(variant) == str(value)
-            if result:
-                self.__value = variant
-                return
-
-        raise Exx__ValueNotInVariants()
-
-
 # =====================================================================================================================
 class AnswerVariants:
     SUCCESS: str = "OK"
     FAIL: str = "FAIL"
     UNSUPPORTED: str = "UNSUPPORTED"
 
     ERR__NAME_CMD_OR_PARAM: str = "ERR__NAME_CMD_OR_PARAM"
@@ -200,75 +27,15 @@
     ERR__VALUE_INCOMPATIBLE: str = "ERR__VALUE_INCOMPATIBLE"
     ERR__ARGS_VALIDATION: str = "ERR__ARGS_VALIDATION"
 
     ERR__ENCODING_OR_DEVICE: str = "ERR__ENCODING_OR_DEVICE"
     ERR__SYNTAX: str = "ERR__SYNTAX"
     ERR__PARAM_CALLING: str = "ERR__PARAM_CALLING"
 
-
-class LineParsed:
-    """
-    ALL RESULTS IN LOWERCASE! (EXCEPT ORIGINAL ORIGINAL!)
-    """
-    # REAL STATE --------------
-    ORIGINAL: str
-    PREFIX: str
-    CMD: str
-    ARGS: List[str]
-    KWARGS: Dict[str, str]
-
-    # AUX ---------------------
-    _PREFIX_EXPECTED: str
-
-    def __init__(self, line: str, _prefix_expected: Optional[str] = None):
-        line = str(line)
-
-        # INIT ----------------
-        self.ORIGINAL = line
-        self.PREFIX = ""
-        self.CMD = ""
-        self.ARGS = []
-        self.KWARGS = {}
-
-        line_lower = line.lower()
-
-        # PREFIX ----------------
-        _prefix_expected = _prefix_expected or ""
-        _prefix_expected = _prefix_expected.lower()
-        self._PREFIX_EXPECTED = _prefix_expected
-        if _prefix_expected and line_lower.startswith(_prefix_expected):
-            self.PREFIX = _prefix_expected
-            line_lower = line_lower.replace(_prefix_expected, "", 1)
-
-        # BLANK ----------------------
-        if not line_lower:
-            return
-        line_lower = re.sub(r"\s*=+\s*", "=", line_lower)
-        line_parts = line_lower.split()
-        if not line_parts:
-            return
-
-        # ARGS/KWARGS ----------------
-        for part in line_parts:
-            if "=" not in part:
-                self.ARGS.append(part)
-            else:
-                part__key_value = part.split("=")
-                self.KWARGS.update(dict([part__key_value, ]))
-
-        # CMD ------------------------
-        if self.ARGS:
-            self.CMD = self.ARGS[0]
-            self.ARGS = self.ARGS[1:]
-
-    def ARGS_count(self) -> int:
-        return len(self.ARGS)
-
-    def KWARGS_count(self) -> int:
-        return len(self.KWARGS)
+    EXIT: str = "EXIT"
 
 
 # =====================================================================================================================
 class SerialServer_Base(QThread):
     # TODO: not realized - ACCESS RULES for PARAMS - may be not need in this case of class/situation!!!
     # TODO: not realised list access - best way to use pattern "name/index" and change same access with Dict "name/key"
 
@@ -283,27 +50,29 @@
         "SerialServer_Base hello line 2",
     ]
 
     PARAMS: Dict[str, Union[Any, Dict[Union[str, int], Any]]] = None
     ANSWER: Type[AnswerVariants] = AnswerVariants
 
     # AUX -----------------------------------------------------
-    _GETATTR_STARTSWITH__CMD: str = "cmd__"
-    _GETATTR_STARTSWITH__SCRIPT: str = "script__"
+    _STARTSWITH__CMD: str = "cmd__"
+    _STARTSWITH__SCRIPT: str = "script__"
 
     _LIST__CMDS: List[str]
     _LIST__SCRIPTS: List[str]
 
-    MONITOR_READY: bool = None  # active working state on ReadingWriting - used for waiting active state!
+    CYCLE_ACTIVE: bool = None  # active working state on ReadingWriting - used for waiting active state!
 
-    def wait__monitor_ready(self) -> None:
+    def wait__cycle_active(self) -> None:
         """
         ALWAYS WAIT IT BEFORE START EXPLUATATION!
         """
-        while not self.MONITOR_READY:
+        self.logger.debug("")
+
+        while not self.CYCLE_ACTIVE:
             time.sleep(0.5)
 
     @property
     def _LIST__HELP(self) -> List[str]:
         params_dump = []
         for name, value in self.PARAMS.items():
             if isinstance(value, dict):
@@ -313,25 +82,29 @@
             elif isinstance(value, (Value_WithUnit, Value_FromVariants)):
                 params_dump.append(" "*2 + f"|{name}={repr(value)}")
             else:
                 params_dump.append(" "*2 + f"|{name}={value}")
 
         # WORK --------------------------------
         result = [
-            "-"*50,
+            "="*50,
             *self.HELLO_MSG,
+            "-" * 50,
             "[PARAMS]:",
             *params_dump,
+            "-" * 50,
             "[CMDS]:",
             *[f"  |{name}" for name in self._LIST__CMDS],
+            "-" * 50,
             "[SCRIPTS]:",
             *[f"  |{name}" for name in self._LIST__SCRIPTS],
+            "-" * 50,
             "[ANSWER_VARIANTS]:",
             *[f"  |{name}" for name in dir(self.ANSWER) if not name.startswith("__")],
-            "-" * 50,
+            "=" * 50,
         ]
         return result
 
     def list_param_results(self, lines: List[str]) -> List[str]:
         """
         used to show several PARAMS and CMD results (ready to pretty sent in serial port)
         cmds used as params in just case if cmd returns exact value! (not for any cmd and not used for results as Answer)
@@ -345,104 +118,161 @@
         return result
 
     # -----------------------------------------------------------------------------------------------------------------
     def __init__(self, params: Dict[str, Any] = None):
         # FIXME: deprecate param params??? used for tests?
         super().__init__()
 
+        self._init__logger()
+        self.logger.debug('init SerialServer')
+
         if params:
             self.PARAMS = params
         elif not self.PARAMS:
             self.PARAMS = {}
         else:
             pass
 
-        self._init_lists()
+        self._init__lists()
 
         self.SERIAL_CLIENT = self._SERIAL_CLIENT__CLS()
         self.SERIAL_CLIENT.RAISE_READ_FAIL_PATTERN = False
         self.SERIAL_CLIENT.TIMEOUT__READ = None
         if self.ADDRESS:
             self.SERIAL_CLIENT.ADDRESS = self.ADDRESS
         if not self.SERIAL_CLIENT.ADDRESS:
-            self.SERIAL_CLIENT.ADDRESS = AddressAutoAcceptVariant.FIRST_FREE__PAIRED_FOR_EMU   # here keep only FIRST_FREE__PAIRED_FOR_EMU! as default!
+            self.SERIAL_CLIENT.ADDRESS = Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED   # here keep only FIRST_FREE__PAIRED! as default!
 
-    def _init_lists(self) -> None:
+    def _init__lists(self) -> None:
         self._LIST__CMDS = []
         self._LIST__SCRIPTS = []
 
         for name in dir(self):
             name = name.lower()
-            if name.startswith(self._GETATTR_STARTSWITH__CMD):
-                self._LIST__CMDS.append(name.replace(self._GETATTR_STARTSWITH__CMD, "", 1))
-            if name.startswith(self._GETATTR_STARTSWITH__SCRIPT):
-                self._LIST__SCRIPTS.append(name.replace(self._GETATTR_STARTSWITH__SCRIPT, "", 1))
+            if name.startswith(self._STARTSWITH__CMD):
+                self._LIST__CMDS.append(name.replace(self._STARTSWITH__CMD, "", 1))
+            if name.startswith(self._STARTSWITH__SCRIPT):
+                self._LIST__SCRIPTS.append(name.replace(self._STARTSWITH__SCRIPT, "", 1))
+
+    def _init__logger(self) -> None:
+        logger = logging.getLogger()
+        logger.setLevel(logging.DEBUG)
+        _formatter = logging.Formatter(
+            '%(asctime)s[%(levelname)s/thread%(thread)s]%(name)s(%(filename)s).%(funcName)s(line%(lineno)d)%(msg)s')
+
+        # _handler_file = logging.FileHandler(f"SerialServer_Base{datetime.datetime.now()}.log")
+        _handler_file = logging.FileHandler(f"SerialServer_Base.log")
+        _handler_file.setFormatter(_formatter)
+
+        _handler_std = logging.StreamHandler()
+        _handler_std.setFormatter(_formatter)
+
+        logger.addHandler(_handler_file)
+        logger.addHandler(_handler_std)
+
+        logger.debug('LOGGER INITED')
+        self.logger = logger
 
     # -----------------------------------------------------------------------------------------------------------------
     def run(self) -> None:
+        self.logger.debug("")
+
+        if self.CYCLE_ACTIVE:
+            # just for sure
+            msg = f"[WARN] ALREADY STARTED={self.__class__.__name__}"
+            print(msg)
+            return
+
         if not self.SERIAL_CLIENT.connect(_raise=False):
             msg = f"[ERROR]NOT STARTED={self.__class__.__name__}"
             print(msg)
             return
 
         if self.HELLO_MSG__SEND_ON_START:
-            self.HELLO_MSG.append(f"Started on [{self.SERIAL_CLIENT._SERIAL.port}]")
+            additional_line = f"Started on [{self.SERIAL_CLIENT._SERIAL.port}]"
+            if additional_line not in self.HELLO_MSG:
+                self.HELLO_MSG.append(additional_line)
             self.SERIAL_CLIENT._write_line("")
             self.SERIAL_CLIENT._write_line("="*50)
             # self._execute_line("hello")
             self.SERIAL_CLIENT._write_line(self.HELLO_MSG)
 
+        self._cycle__activate()
+
+    def _cycle__activate(self) -> Never:
+        self.logger.debug("")
+
         while True:
-            self.MONITOR_READY = True
+            self.CYCLE_ACTIVE = True
             line = None
             try:
                 line = self.SERIAL_CLIENT.read_line()
             except:
                 self.SERIAL_CLIENT._write_line(self.ANSWER.ERR__ENCODING_OR_DEVICE)
 
             if line:
                 self._execute_line(line)
 
+    def connect(self) -> None:
+        self.logger.debug("")
+
+        # if not self.isRunning():
+        self.start()
+        self.wait__cycle_active()
+
     def disconnect(self):
-        self.SERIAL_CLIENT.disconnect()
+        self.logger.debug("")
+
         self.terminate()
-        self.MONITOR_READY = False
+        # self.SERIAL_CLIENT.disconnect()
+        # self.CYCLE_ACTIVE = False
 
     def terminate(self):
-        super().terminate()
-        self.MONITOR_READY = False
+        # if self.SERIAL_CLIENT.CONNECTED:
+        #     self.SERIAL_CLIENT.send__(self.ANSWER.EXIT)
+
+        self.SERIAL_CLIENT.disconnect()
+
+        if self.isRunning():
+            self.logger.debug("")
+            super().terminate()
+        self.CYCLE_ACTIVE = False
 
     # -----------------------------------------------------------------------------------------------------------------
     def _execute_line(self, line: str) -> bool:
+        self.logger.debug("")
+
         line_parsed = LineParsed(line, _prefix_expected=self.SERIAL_CLIENT.PREFIX)
         cmd_result = self._cmd__(line_parsed)
 
         # blank line - SEND!!! because value may be BLANK!!!!
         # if not cmd_result:
         #     return True
 
         write_result = self.SERIAL_CLIENT._write_line(cmd_result)
         return write_result
 
     # CMD - ENTRY POINT -----------------------------------------------------------------------------------------------
     def _cmd__(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
-        meth_name__expected = f"{self._GETATTR_STARTSWITH__CMD}{line_parsed.CMD}"
+        self.logger.debug("")
+
+        meth_name__expected = f"{self._STARTSWITH__CMD}{line_parsed.CMD}"
         meth_name__original = funcs_aux.Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
         # GET METHOD --------------------
         if meth_name__original:
-            meth_cmd = getattr(self, meth_name__original.VALUE)
+            meth = getattr(self, meth_name__original.VALUE)
         else:
-            meth_cmd = self._cmd__param_as_cmd
+            meth = self._cmd__param_as_cmd
 
         # EXEC METHOD --------------------
         try:
-            result = meth_cmd(line_parsed)
+            result = meth(line_parsed)
         except TypeError as exx:
             try:
-                result = meth_cmd()
+                result = meth()
             except:
                 result = self.ANSWER.FAIL
         except:
             result = self.ANSWER.FAIL
 
         if result is None:
             result = self.ANSWER.SUCCESS
@@ -573,27 +403,51 @@
         # ERR__ARGS_VALIDATION --------------------------------
         pass
 
         # WORK --------------------------------
         return line_parsed.ORIGINAL
 
     # CMDS - SCRIPTS --------------------------------------------------------------------------------------------------
-    def cmd__run(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
+    def cmd__script(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
+        """
+        it is as template! you can create/use your awn script-run cmd!
+        """
+        return self._script__(line_parsed)
+
+    def _script__(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         # ERR__ARGS_VALIDATION --------------------------------
         if line_parsed.ARGS_count() == 0:
             return self.ANSWER.ERR__ARGS_VALIDATION
 
         # WORK --------------------------------
-        meth_name__expected = f"{self._GETATTR_STARTSWITH__SCRIPT}{line_parsed.ARGS[0]}"
+        meth_name__expected = f"{self._STARTSWITH__SCRIPT}{line_parsed.ARGS[0]}"
         meth_name__original = funcs_aux.Iterables().item__get_original__case_insensitive(meth_name__expected, dir(self))
         if not meth_name__original:
             return self.ANSWER.ERR__NAME_SCRIPT
 
-        meth_cmd = getattr(self, meth_name__original.VALUE)
-        return meth_cmd(line_parsed)
+        meth = getattr(self, meth_name__original.VALUE)
+
+        # EXEC METHOD --------------------
+        try:
+            result = meth(line_parsed)
+        except TypeError as exx:
+            try:
+                result = meth()
+            except:
+                result = self.ANSWER.FAIL
+        except:
+            result = self.ANSWER.FAIL
+
+        if result is None:
+            result = self.ANSWER.SUCCESS
+        return result
+
+    # def cmd__exit(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
+    #     self.disconnect()
+    #     exit()
 
 
 # =====================================================================================================================
 class SerialServer_Echo(SerialServer_Base):
     HELLO_MSG: List[str] = [
         "SerialServer_Echo",
         "started!",
@@ -638,14 +492,21 @@
                 2: 32,
             },
         },
         "UNIT": Value_WithUnit(1, unit="V"),
         "VARIANT": Value_FromVariants(220, variants=[220, 380]),
     }
 
+    def cmd__upper(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
+        # usefull for tests
+        return line_parsed.ORIGINAL.upper()
+
+    def cmd__lower(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
+        return line_parsed.ORIGINAL.lower()
+
     def cmd__cmd(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         # NOTE: NONE is equivalent for SUCCESS
         # do smth
         pass
 
     def cmd__cmd_no_line(self) -> TYPE__CMD_RESULT:
         # NOTE: NONE is equivalent for SUCCESS
@@ -655,7 +516,12 @@
     # -----------------------------------------------------------------------------------------------------------------
     def script__script1(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         # do smth
         pass
 
 
 # =====================================================================================================================
+if __name__ == "__main__":
+    SerialServer_Example().run()
+
+
+# =====================================================================================================================
```

### Comparing `bus_user-0.2.9/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.0/bus_user.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.2.9
+Version: 0.3.0
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,21 +16,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.2.9)
+# bus_user (v0.3.0)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
-### !. MOST APPROPRIATE COMMAND PROTOCOL
+###
+NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
+    
+!. MOST APPROPRIATE COMMAND PROTOCOL
 other protocols mot recommended
 
 1. all cmds must be as params (preferred) in equipment or as special command
 2. [<CMD_NAME>] - read param value or run special command  
     [IDN] - read value IDN  
     [DUMP] - run special command 
 3. [<CMD_NAME> <VALUE>] - write value in parameter or run special cmd with param  
@@ -44,15 +47,15 @@
     [FAIL 0123] - any specified error without description
     [FAIL 02 VALUE OUT OF RANGE] - any specified error with description (full variant)
 
 
 ## Features
 1. Serial:  
 	- Client+Server  
-	- connect with AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
+	- connect with Type__AddressAutoAcceptVariant FIRST_FREE/FIRST_FREE__ANSWER_VALID  
 	- set/get params by SlashOrSpacePath addressing  
 	- handle BackSpace send manually from terminal  
 2. SerialServer values:  
 	- as Callable  
 	- Value_WithUnit  
 	- Value_FromVariants  
 	- list_results
```

### Comparing `bus_user-0.2.9/setup.py` & `bus_user-0.3.0/setup.py`

 * *Files identical despite different names*

