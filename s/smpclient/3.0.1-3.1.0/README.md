# Comparing `tmp/smpclient-3.0.1.tar.gz` & `tmp/smpclient-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smpclient-3.0.1.tar", max compression
+gzip compressed data, was "smpclient-3.1.0.tar", max compression
```

## Comparing `smpclient-3.0.1.tar` & `smpclient-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11421 2024-05-25 20:27:12.100087 smpclient-3.0.1/LICENSE
--rw-r--r--   0        0        0     2501 2024-05-25 20:27:12.100087 smpclient-3.0.1/README.md
--rw-r--r--   0        0        0     1879 2024-05-25 20:27:12.124087 smpclient-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     7979 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/__init__.py
--rw-r--r--   0        0        0      188 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/extensions/__init__.py
--rw-r--r--   0        0        0     2473 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/extensions/intercreate.py
--rw-r--r--   0        0        0     2014 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/generics.py
--rw-r--r--   0        0        0     8321 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/mcuboot.py
--rw-r--r--   0        0        0        0 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/py.typed
--rw-r--r--   0        0        0        0 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/__init__.py
--rw-r--r--   0        0        0      637 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/image_management.py
--rw-r--r--   0        0        0     1229 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/os_management.py
--rw-r--r--   0        0        0      264 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/shell_management.py
--rw-r--r--   0        0        0        0 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/user/__init__.py
--rw-r--r--   0        0        0      236 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/requests/user/intercreate.py
--rw-r--r--   0        0        0     2308 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/transport/__init__.py
--rw-r--r--   0        0        0     7958 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/transport/ble.py
--rw-r--r--   0        0        0    10385 2024-05-25 20:27:12.124087 smpclient-3.0.1/smpclient/transport/serial.py
--rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 smpclient-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11421 2024-05-27 18:31:03.700463 smpclient-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2501 2024-05-27 18:31:03.700463 smpclient-3.1.0/README.md
+-rw-r--r--   0        0        0     1879 2024-05-27 18:31:03.724463 smpclient-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8505 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/__init__.py
+-rw-r--r--   0        0        0      188 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/extensions/__init__.py
+-rw-r--r--   0        0        0     2473 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/extensions/intercreate.py
+-rw-r--r--   0        0        0     2014 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/generics.py
+-rw-r--r--   0        0        0     8321 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/mcuboot.py
+-rw-r--r--   0        0        0        0 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/py.typed
+-rw-r--r--   0        0        0        0 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/__init__.py
+-rw-r--r--   0        0        0      637 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/image_management.py
+-rw-r--r--   0        0        0     1229 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/os_management.py
+-rw-r--r--   0        0        0      264 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/shell_management.py
+-rw-r--r--   0        0        0        0 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/user/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/requests/user/intercreate.py
+-rw-r--r--   0        0        0     2361 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/transport/__init__.py
+-rw-r--r--   0        0        0     9328 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/transport/ble.py
+-rw-r--r--   0        0        0    10385 2024-05-27 18:31:03.724463 smpclient-3.1.0/smpclient/transport/serial.py
+-rw-r--r--   0        0        0     3328 1970-01-01 00:00:00.000000 smpclient-3.1.0/PKG-INFO
```

### Comparing `smpclient-3.0.1/LICENSE` & `smpclient-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/README.md` & `smpclient-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/pyproject.toml` & `smpclient-3.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/__init__.py` & `smpclient-3.1.0/smpclient/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,18 +37,26 @@
         await self._transport.connect(self._address, timeout_s)
         await self._initialize()
 
     async def disconnect(self) -> None:
         """Disconnect from the SMP server."""
         await self._transport.disconnect()
 
-    async def request(self, request: SMPRequest[TRep, TEr0, TEr1]) -> TRep | TEr0 | TEr1:
+    async def request(
+        self, request: SMPRequest[TRep, TEr0, TEr1], timeout_s: float = 120.000
+    ) -> TRep | TEr0 | TEr1:
         """Make an `SMPRequest` to the SMP server."""
 
-        frame = await self._transport.send_and_receive(request.BYTES)
+        try:
+            async with timeout(timeout_s):
+                frame = await self._transport.send_and_receive(request.BYTES)
+        except asyncio.TimeoutError:
+            timeout_message: Final = f"Timeout ({timeout_s}s) waiting for request {request}"
+            logger.error(timeout_message)
+            raise TimeoutError(timeout_message)
 
         header = smpheader.Header.loads(frame[: smpheader.Header.SIZE])
 
         if header.sequence != request.header.sequence:  # type: ignore
             raise SMPBadSequence("Bad sequence")
 
         try:
@@ -66,15 +74,20 @@
                 f"Response could not by parsed as one of {request._Response}, "
                 f"{request._ErrorV0}, or {request._ErrorV1}. {header=} {frame=}"
             )
             logger.error(error_message)
             raise ValidationError(error_message)
 
     async def upload(
-        self, image: bytes, slot: int = 0, upgrade: bool = False
+        self,
+        image: bytes,
+        slot: int = 0,
+        upgrade: bool = False,
+        first_timeout_s: float = 40.000,
+        subsequent_timeout_s: float = 2.500,
     ) -> AsyncIterator[int]:
         """Iteratively upload an `image` to `slot`, yielding the offset."""
 
         if self._transport.max_unencoded_size < 23:
             raise Exception("Upload requires an MTU >=23.")
 
         response = await self.request(
@@ -84,30 +97,32 @@
                     data=b"",
                     image=slot,
                     len=len(image),
                     sha=sha256(image).digest(),
                     upgrade=upgrade,
                 ),
                 image,
-            )
+            ),
+            timeout_s=first_timeout_s,
         )
 
         if error(response):
             raise SMPUploadError(response)
         elif success(response):
             if response.off is None:
                 raise SMPUploadError(f"No offset received: {response=}")
             yield response.off
         else:  # pragma: no cover
             raise Exception("Unreachable")
 
         # send chunks until the SMP server reports that the offset is at the end of the image
         while response.off != len(image):
             response = await self.request(
-                self._maximize_packet(ImageUploadWrite(off=response.off, data=b""), image)
+                self._maximize_packet(ImageUploadWrite(off=response.off, data=b""), image),
+                timeout_s=subsequent_timeout_s,
             )
             if error(response):
                 raise SMPUploadError(response)
             elif success(response):
                 if response.off is None:
                     raise SMPUploadError(f"No offset received: {response=}")
                 yield response.off
```

### Comparing `smpclient-3.0.1/smpclient/extensions/intercreate.py` & `smpclient-3.1.0/smpclient/extensions/intercreate.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/generics.py` & `smpclient-3.1.0/smpclient/generics.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/mcuboot.py` & `smpclient-3.1.0/smpclient/mcuboot.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/requests/image_management.py` & `smpclient-3.1.0/smpclient/requests/image_management.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/requests/os_management.py` & `smpclient-3.1.0/smpclient/requests/os_management.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/smpclient/transport/__init__.py` & `smpclient-3.1.0/smpclient/transport/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 """Simple Management Protocol (SMP) Client Transport Protocol."""
 
 from __future__ import annotations
 
 from typing import Protocol
 
 
+class SMPTransportDisconnected(Exception):
+    ...
+
+
 class SMPTransport(Protocol):
     _smp_server_transport_buffer_size: int | None = None
     """The SMP server transport buffer size, in 8-bit bytes."""
 
     async def connect(self, address: str, timeout_s: float) -> None:  # pragma: no cover
         """Connect the `SMPTransport`."""
```

### Comparing `smpclient-3.0.1/smpclient/transport/ble.py` & `smpclient-3.1.0/smpclient/transport/ble.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from bleak import BleakClient, BleakGATTCharacteristic, BleakScanner
 from bleak.backends.client import BaseBleakClient
 from bleak.backends.device import BLEDevice
 from smp import header as smphdr
 from typing_extensions import TypeGuard, override
 
 from smpclient.exceptions import SMPClientException
-from smpclient.transport import SMPTransport
+from smpclient.transport import SMPTransport, SMPTransportDisconnected
 
 if sys.platform == "linux":
     from bleak.backends.bluezdbus.client import BleakClientBlueZDBus
 else:  # stub for mypy
 
     class BleakClientBlueZDBus:
         async def _acquire_mtu(self) -> None:
@@ -53,14 +53,16 @@
 logger = logging.getLogger(__name__)
 
 
 class SMPBLETransport(SMPTransport):
     def __init__(self) -> None:
         self._buffer = bytearray()
         self._notify_condition = asyncio.Condition()
+        self._disconnected_event = asyncio.Event()
+        self._disconnected_event.set()
 
         self._max_write_without_response_size = 20
         """Initially set to BLE minimum; may be mutated by the `connect()` method."""
 
         logger.debug(f"Initialized {self.__class__.__name__}")
 
     @override
@@ -69,32 +71,35 @@
         device: BLEDevice | None = (
             await BleakScanner.find_device_by_address(address, timeout=timeout_s)
             if MAC_ADDRESS_PATTERN.match(address) or UUID_PATTERN.match(address)
             else await BleakScanner.find_device_by_name(address)
         )
 
         if type(device) is BLEDevice:
-            self._client = BleakClient(device, services=(str(SMP_SERVICE_UUID),))
+            self._client = BleakClient(
+                device,
+                services=(str(SMP_SERVICE_UUID),),
+                disconnected_callback=self._set_disconnected_event,
+            )
         else:
             raise SMPBLETransportDeviceNotFound(f"Device '{address}' not found")
 
         logger.debug(f"Found device: {device=}, connecting...")
         await self._client.connect()
+        self._disconnected_event.clear()
         logger.debug(f"Connected to {device=}")
 
         smp_characteristic = self._client.services.get_characteristic(SMP_CHARACTERISTIC_UUID)
         if smp_characteristic is None:
             raise SMPBLETransportNotSMPServer("Missing the SMP characteristic UUID.")
 
         logger.debug(f"Found SMP characteristic: {smp_characteristic=}")
         logger.info(f"{smp_characteristic.max_write_without_response_size=}")
-        if (
-            platform.system() == "Windows"
-            and smp_characteristic.max_write_without_response_size == 20
-        ):
+        self._max_write_without_response_size = smp_characteristic.max_write_without_response_size
+        if platform.system() == "Windows" and self._max_write_without_response_size == 20:
             # https://github.com/hbldh/bleak/pull/1552#issuecomment-2105573291
             logger.warning(
                 "The SMP characteristic MTU is 20 bytes, possibly a Windows bug, checking again"
             )
             await asyncio.sleep(2)
             smp_characteristic._max_write_without_response_size = (
                 self._client._backend._session.max_pdu_size - 3  # type: ignore
@@ -134,15 +139,15 @@
     @override
     async def receive(self) -> bytes:
         # Note: self._buffer is mutated asynchronously by this method and self._notify_callback().
         #       self._notify_condition is used to synchronize access to self._buffer.
 
         async with self._notify_condition:  # wait for the header
             logger.debug(f"Waiting for notify on {SMP_CHARACTERISTIC_UUID=}")
-            await self._notify_condition.wait()
+            await self._notify_or_disconnect()
 
             if len(self._buffer) < smphdr.Header.SIZE:  # pragma: no cover
                 raise SMPBLETransportException(
                     f"Buffer contents not big enough for SMP header: {self._buffer=}"
                 )
 
             header: Final = smphdr.Header.loads(self._buffer[: smphdr.Header.SIZE])
@@ -156,15 +161,15 @@
                 if len(self._buffer) == message_length:
                     logger.debug(f"Finished receiving {message_length} byte response")
                     out = bytes(self._buffer)
                     self._buffer.clear()
                     return out
                 elif len(self._buffer) > message_length:  # pragma: no cover
                     raise SMPBLETransportException("Length of buffer passed expected message size.")
-                await self._notify_condition.wait()
+                await self._notify_or_disconnect()
 
     async def _notify_callback(self, sender: BleakGATTCharacteristic, data: bytes) -> None:
         if sender.uuid != str(SMP_CHARACTERISTIC_UUID):  # pragma: no cover
             raise SMPBLETransportException(f"Unexpected notify from {sender}; {data=}")
         async with self._notify_condition:
             logger.debug(f"Received {len(data)} bytes from {SMP_CHARACTERISTIC_UUID=}")
             self._buffer.extend(data)
@@ -191,7 +196,32 @@
         ]
         logger.debug(f"Found {len(smp_servers)} SMP devices: {smp_servers=}")
         return smp_servers
 
     @staticmethod
     def _bluez_backend(client_backend: BaseBleakClient) -> TypeGuard[BleakClientBlueZDBus]:
         return client_backend.__class__.__name__ == "BleakClientBlueZDBus"
+
+    def _set_disconnected_event(self, client: BleakClient) -> None:
+        if client is not self._client:
+            raise SMPBLETransportException(
+                f"Unexpected client disconnected: {client=}, {self._client=}"
+            )
+        logger.warning(f"Disconnected from {client.address}")
+        self._disconnected_event.set()
+
+    async def _notify_or_disconnect(self) -> None:
+        disconnected_task: Final = asyncio.create_task(self._disconnected_event.wait())
+        notify_task: Final = asyncio.create_task(self._notify_condition.wait())
+        done, pending = await asyncio.wait(
+            (disconnected_task, notify_task), return_when=asyncio.FIRST_COMPLETED
+        )
+        for task in pending:
+            task.cancel()
+        try:
+            await asyncio.gather(*pending)
+        except asyncio.CancelledError:
+            pass
+        if disconnected_task in done:
+            raise SMPTransportDisconnected(
+                f"{self.__class__.__name__} disconnected from {self._client.address}"
+            )
```

### Comparing `smpclient-3.0.1/smpclient/transport/serial.py` & `smpclient-3.1.0/smpclient/transport/serial.py`

 * *Files identical despite different names*

### Comparing `smpclient-3.0.1/PKG-INFO` & `smpclient-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smpclient
-Version: 3.0.1
+Version: 3.1.0
 Summary: Simple Management Protocol (SMP) Client for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

