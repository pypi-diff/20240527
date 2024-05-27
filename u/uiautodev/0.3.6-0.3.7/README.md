# Comparing `tmp/uiautodev-0.3.6.tar.gz` & `tmp/uiautodev-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautodev-0.3.6.tar", max compression
+gzip compressed data, was "uiautodev-0.3.7.tar", max compression
```

## Comparing `uiautodev-0.3.6.tar` & `uiautodev-0.3.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1068 2024-05-10 02:46:46.318986 uiautodev-0.3.6/LICENSE
--rw-r--r--   0        0        0     1191 2024-05-10 02:46:46.318986 uiautodev-0.3.6/README.md
--rw-r--r--   0        0        0     1126 2024-05-10 02:47:05.511257 uiautodev-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      267 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/__init__.py
--rw-r--r--   0        0        0      176 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/__main__.py
--rw-r--r--   0        0        0     2498 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/app.py
--rw-r--r--   0        0        0     1773 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/appium_proxy.py
--rw-r--r--   0        0        0     3919 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/case.py
--rw-r--r--   0        0        0     6234 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/cli.py
--rw-r--r--   0        0        0     4562 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/command_proxy.py
--rw-r--r--   0        0        0     1587 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/command_types.py
--rw-r--r--   0        0        0      552 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/common.py
--rw-r--r--   0        0        0     7064 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/driver/android.py
--rw-r--r--   0        0        0     5308 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/driver/appium.py
--rw-r--r--   0        0        0     2048 2024-05-10 02:46:46.318986 uiautodev-0.3.6/uiautodev/driver/base_driver.py
--rw-r--r--   0        0        0     4353 2024-05-10 02:46:46.322986 uiautodev-0.3.6/uiautodev/driver/ios.py
--rw-r--r--   0        0        0     2422 2024-05-10 02:46:46.322986 uiautodev-0.3.6/uiautodev/driver/mock.py
--rw-r--r--   0        0        0  3675062 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
--rw-r--r--   0        0        0     8351 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/driver/udt/udt.py
--rw-r--r--   0        0        0      465 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/exceptions.py
--rw-r--r--   0        0        0      717 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/model.py
--rw-r--r--   0        0        0     2370 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/provider.py
--rw-r--r--   0        0        0     4116 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/router/device.py
--rw-r--r--   0        0        0      891 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/router/xml.py
--rw-r--r--   0        0        0     1240 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/static/demo.html
--rw-r--r--   0        0        0     4785 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/utils/common.py
--rw-r--r--   0        0        0      637 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/utils/exceptions.py
--rw-r--r--   0        0        0    17386 2024-05-10 02:46:46.330986 uiautodev-0.3.6/uiautodev/utils/usbmux.py
--rw-r--r--   0        0        0     2329 1970-01-01 00:00:00.000000 uiautodev-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-27 09:06:49.988979 uiautodev-0.3.7/LICENSE
+-rw-r--r--   0        0        0     1191 2024-05-27 09:06:49.988979 uiautodev-0.3.7/README.md
+-rw-r--r--   0        0        0     1144 2024-05-27 09:07:03.937050 uiautodev-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      267 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/__main__.py
+-rw-r--r--   0        0        0     2498 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/app.py
+-rw-r--r--   0        0        0     1773 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/appium_proxy.py
+-rw-r--r--   0        0        0     3919 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/case.py
+-rw-r--r--   0        0        0     6234 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/cli.py
+-rw-r--r--   0        0        0     4562 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/command_proxy.py
+-rw-r--r--   0        0        0     1587 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/command_types.py
+-rw-r--r--   0        0        0      552 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/common.py
+-rw-r--r--   0        0        0     6827 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/android.py
+-rw-r--r--   0        0        0     5308 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/appium.py
+-rw-r--r--   0        0        0     2048 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/base_driver.py
+-rw-r--r--   0        0        0     4353 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/ios.py
+-rw-r--r--   0        0        0     2422 2024-05-27 09:06:49.992979 uiautodev-0.3.7/uiautodev/driver/mock.py
+-rw-r--r--   0        0        0  3675062 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk
+-rw-r--r--   0        0        0     8351 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/driver/udt/udt.py
+-rw-r--r--   0        0        0      465 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/exceptions.py
+-rw-r--r--   0        0        0      827 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/model.py
+-rw-r--r--   0        0        0     2370 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/provider.py
+-rw-r--r--   0        0        0     4425 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/router/device.py
+-rw-r--r--   0        0        0      891 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/router/xml.py
+-rw-r--r--   0        0        0     1240 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/static/demo.html
+-rw-r--r--   0        0        0     4785 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/common.py
+-rw-r--r--   0        0        0      637 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/exceptions.py
+-rw-r--r--   0        0        0    17386 2024-05-27 09:06:50.004979 uiautodev-0.3.7/uiautodev/utils/usbmux.py
+-rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 uiautodev-0.3.7/PKG-INFO
```

### Comparing `uiautodev-0.3.6/LICENSE` & `uiautodev-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/README.md` & `uiautodev-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/pyproject.toml` & `uiautodev-0.3.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uiautodev"
-version = "0.3.6"
+version = "0.3.7"
 description = "Mobile UI Automation, include UI hierarchy inspector, script recorder"
 homepage = "https://uiauto.dev"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
@@ -18,14 +18,15 @@
 httpretty = {version = "^1.1.4", optional = true}
 appium-python-client = {version = "^4.0.0", optional = true}
 uiautomator2 = ">=2"
 httpx = "*"
 fastapi = "^0.111.0"
 uvicorn = {version = "*", extras = ["standard"]}
 poetry = "^1.8.2"
+pydantic = "^2.6"
 
 [tool.poetry.extras]
 appium = ["appium-python-client", "httppretty"]
 
 [tool.poetry.scripts]
 "uiauto.dev" = "uiautodev.__main__:main"
 "uiautodev" = "uiautodev.__main__:main"
```

### Comparing `uiautodev-0.3.6/uiautodev/app.py` & `uiautodev-0.3.7/uiautodev/app.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/appium_proxy.py` & `uiautodev-0.3.7/uiautodev/appium_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/case.py` & `uiautodev-0.3.7/uiautodev/case.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/cli.py` & `uiautodev-0.3.7/uiautodev/cli.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/command_proxy.py` & `uiautodev-0.3.7/uiautodev/command_proxy.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/command_types.py` & `uiautodev-0.3.7/uiautodev/command_types.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/common.py` & `uiautodev-0.3.7/uiautodev/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/android.py` & `uiautodev-0.3.7/uiautodev/driver/android.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 """
 
 import json
 import logging
 import re
 import time
 from functools import cached_property, partial
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 from xml.etree import ElementTree
 
 import adbutils
 import uiautomator2 as u2
 from PIL import Image
 
 from uiautodev.command_types import CurrentAppResponse
 from uiautodev.driver.base_driver import BaseDriver
 from uiautodev.driver.udt.udt import UDT, UDTError
 from uiautodev.exceptions import AndroidDriverException, RequestError
-from uiautodev.model import Node, ShellResponse, WindowSize
+from uiautodev.model import Node, Rect, ShellResponse, WindowSize
 from uiautodev.utils.common import fetch_through_socket
 
 logger = logging.getLogger(__name__)
 
 class AndroidDriver(BaseDriver):
     def __init__(self, serial: str):
         super().__init__(serial)
         self.adb_device = adbutils.device(serial)
         self._try_dump_list = [
             self._get_u2_hierarchy,
-            self._get_appium_hierarchy,
             self._get_udt_dump_hierarchy,
+            # self._get_appium_hierarchy,
         ]
     
     @cached_property
     def udt(self) -> UDT:    
         return UDT(self.adb_device)
 
     @cached_property
@@ -60,24 +60,24 @@
             else:
                 return ShellResponse(
                     output="", error=f"exit:{ret.returncode}, output:{ret.output}"
                 )
         except Exception as e:
             return ShellResponse(output="", error=f"adb error: {str(e)}")
 
-    def dump_hierarchy(self) -> Tuple[str, Node]:
+    def dump_hierarchy(self, display_id: Optional[int] = 0) -> Tuple[str, Node]:
         """returns xml string and hierarchy object"""
-        wsize = self.adb_device.window_size()
-        logger.debug("window size: %s", wsize)
         start = time.time()
         xml_data = self._dump_hierarchy_raw()
         logger.debug("dump_hierarchy cost: %s", time.time() - start)
 
+        wsize = self.adb_device.window_size()
+        logger.debug("window size: %s", wsize)
         return xml_data, parse_xml(
-            xml_data, WindowSize(width=wsize[0], height=wsize[1])
+            xml_data, WindowSize(width=wsize[0], height=wsize[1]), display_id
         )
 
     def _dump_hierarchy_raw(self) -> str:
         """
         uiautomator2 server is conflict with "uiautomator dump" command.
 
         uiautomator dump errors:
@@ -95,36 +95,14 @@
             except Exception as e:
                 logger.exception("unexpected dump error: %s", e)
         raise AndroidDriverException("Failed to dump hierarchy")
     
     def _get_u2_hierarchy(self) -> str:
         d = u2.connect_usb(self.serial)
         return d.dump_hierarchy()
-        # c = self.device.create_connection(adbutils.Network.TCP, 9008)
-        # try:
-        #     compressed = False
-        #     payload = {
-        #         "jsonrpc": "2.0",
-        #         "method": "dumpWindowHierarchy",
-        #         "params": [compressed],
-        #         "id": 1,
-        #     }
-        #     content = fetch_through_socket(
-        #         c, "/jsonrpc/0", method="POST", json=payload, timeout=5
-        #     )
-        #     json_resp = json.loads(content)
-        #     if "error" in json_resp:
-        #         raise AndroidDriverException(json_resp["error"])
-        #     return json_resp["result"]
-        # except adbutils.AdbError as e:
-        #     raise AndroidDriverException(
-        #         f"Failed to get hierarchy from u2 server: {str(e)}"
-        #     )
-        # finally:
-        #     c.close()
 
     def _get_appium_hierarchy(self) -> str:
         c = self.adb_device.create_connection(adbutils.Network.TCP, 6790)
         try:
             content = fetch_through_socket(c, "/wd/hub/session/0/source", timeout=10)
             return json.loads(content)["value"]
         except (adbutils.AdbError, RequestError) as e:
@@ -164,47 +142,59 @@
     def home(self):
         self.adb_device.keyevent("HOME")
     
     def wake_up(self):
         self.adb_device.keyevent("WAKEUP")
 
 
-def parse_xml(xml_data: str, wsize: WindowSize) -> Node:
+def parse_xml(xml_data: str, wsize: WindowSize, display_id: Optional[int] = None) -> Node:
     root = ElementTree.fromstring(xml_data)
-    return parse_xml_element(root, wsize)
+    node = parse_xml_element(root, wsize, display_id)
+    if node is None:
+        raise AndroidDriverException("Failed to parse xml")
+    return node
 
 
-def parse_xml_element(
-    element, wsize: WindowSize, indexes: List[int] = [0]
-) -> Node:
+def parse_xml_element(element, wsize: WindowSize, display_id: Optional[int], indexes: List[int] = [0]) -> Optional[Node]:
     """
     Recursively parse an XML element into a dictionary format.
     """
     name = element.tag
     if name == "node":
         name = element.attrib.get("class", "node")
+    if display_id is not None:
+        elem_display_id = int(element.attrib.get("display-id", display_id))
+        if elem_display_id != display_id:
+            return
+
     bounds = None
+    rect = None
     # eg: bounds="[883,2222][1008,2265]"
     if "bounds" in element.attrib:
         bounds = element.attrib["bounds"]
         bounds = list(map(int, re.findall(r"\d+", bounds)))
         assert len(bounds) == 4
+        rect = Rect(x=bounds[0], y=bounds[1], width=bounds[2] - bounds[0], height=bounds[3] - bounds[1])
         bounds = (
             bounds[0] / wsize.width,
             bounds[1] / wsize.height,
             bounds[2] / wsize.width,
             bounds[3] / wsize.height,
         )
         bounds = map(partial(round, ndigits=4), bounds)
+        
     elem = Node(
         key="-".join(map(str, indexes)),
         name=name,
         bounds=bounds,
+        rect=rect,
         properties={key: element.attrib[key] for key in element.attrib},
         children=[],
     )
 
     # Construct xpath for children
     for index, child in enumerate(element):
-        elem.children.append(parse_xml_element(child, wsize, indexes + [index]))
+        child_node = parse_xml_element(child, wsize, display_id, indexes + [index])
+        if child_node:
+            elem.children.append(child_node)
 
     return elem
```

### Comparing `uiautodev-0.3.6/uiautodev/driver/appium.py` & `uiautodev-0.3.7/uiautodev/driver/appium.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/base_driver.py` & `uiautodev-0.3.7/uiautodev/driver/base_driver.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/ios.py` & `uiautodev-0.3.7/uiautodev/driver/ios.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/mock.py` & `uiautodev-0.3.7/uiautodev/driver/mock.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk` & `uiautodev-0.3.7/uiautodev/driver/udt/appium-uiautomator2-v5.12.4-light.apk`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/driver/udt/udt.py` & `uiautodev-0.3.7/uiautodev/driver/udt/udt.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/model.py` & `uiautodev-0.3.7/uiautodev/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,18 +20,26 @@
 
 
 class ShellResponse(BaseModel):
     output: str
     error: Optional[str] = ""
 
 
+class Rect(BaseModel):
+    x: int
+    y: int
+    width: int
+    height: int
+
+
 class Node(BaseModel):
     key: str
     name: str
     bounds: Optional[Tuple[float, float, float, float]] = None
+    rect: Optional[Rect] = None
     properties: Dict[str, Union[str, bool]] = []
     children: List[Node] = []
 
 
 class WindowSize(typing.NamedTuple):
     width: int
     height: int
```

### Comparing `uiautodev-0.3.6/uiautodev/provider.py` & `uiautodev-0.3.7/uiautodev/provider.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/router/device.py` & `uiautodev-0.3.7/uiautodev/router/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from pydantic import BaseModel
 
 from uiautodev import command_proxy
 from uiautodev.command_types import Command, CurrentAppResponse, InstallAppRequest, InstallAppResponse, TapRequest
 from uiautodev.model import DeviceInfo, Node, ShellResponse
 from uiautodev.provider import BaseProvider
 
-
 logger = logging.getLogger(__name__)
 
 class AndroidShellPayload(BaseModel):
     command: str
 
 
 def make_router(provider: BaseProvider) -> APIRouter:
@@ -54,30 +53,35 @@
         responses={200: {"content": {"image/jpeg": {}}}},
         response_class=Response,
     )
     def _screenshot(serial: str, id: int) -> Response:
         """Take a screenshot of device"""
         try:
             driver = provider.get_device_driver(serial)
-            pil_img = driver.screenshot(id)
+            pil_img = driver.screenshot(id).convert("RGB")
             buf = io.BytesIO()
             pil_img.save(buf, format="JPEG")
             image_bytes = buf.getvalue()
             return Response(content=image_bytes, media_type="image/jpeg")
         except Exception as e:
             logger.exception("screenshot failed")
             return Response(content=str(e), media_type="text/plain", status_code=500)
 
     @router.get("/{serial}/hierarchy")
-    def dump_hierarchy(serial: str) -> Node:
+    def dump_hierarchy(serial: str, format: str = "json") -> Node:
         """Dump the view hierarchy of an Android device"""
         try:
             driver = provider.get_device_driver(serial)
             xml_data, hierarchy = driver.dump_hierarchy()
-            return hierarchy
+            if format == "xml":
+                return Response(content=xml_data, media_type="text/xml")
+            elif format == "json":
+                return hierarchy
+            else:
+                return Response(content=f"Invalid format: {format}", media_type="text/plain", status_code=400)
         except Exception as e:
             logger.exception("dump_hierarchy failed")
             return Response(content=str(e), media_type="text/plain", status_code=500)
     
     @router.post('/{serial}/command/tap')
     def command_tap(serial: str, params: TapRequest):
         """Run a command on the device"""
```

### Comparing `uiautodev-0.3.6/uiautodev/router/xml.py` & `uiautodev-0.3.7/uiautodev/router/xml.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/static/demo.html` & `uiautodev-0.3.7/uiautodev/static/demo.html`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/utils/common.py` & `uiautodev-0.3.7/uiautodev/utils/common.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/utils/exceptions.py` & `uiautodev-0.3.7/uiautodev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/uiautodev/utils/usbmux.py` & `uiautodev-0.3.7/uiautodev/utils/usbmux.py`

 * *Files identical despite different names*

### Comparing `uiautodev-0.3.6/PKG-INFO` & `uiautodev-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiautodev
-Version: 0.3.6
+Version: 0.3.7
 Summary: Mobile UI Automation, include UI hierarchy inspector, script recorder
 Home-page: https://uiauto.dev
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 Requires-Dist: construct
 Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: httpretty (>=1.1.4,<2.0.0)
 Requires-Dist: httpx
 Requires-Dist: lxml
 Requires-Dist: pillow
 Requires-Dist: poetry (>=1.8.2,<2.0.0)
+Requires-Dist: pydantic (>=2.6,<3.0)
 Requires-Dist: pygments (>=2)
 Requires-Dist: uiautomator2 (>=2)
 Requires-Dist: uvicorn[standard]
 Description-Content-Type: text/markdown
 
 # uiautodev
 [![codecov](https://codecov.io/gh/codeskyblue/appinspector/graph/badge.svg?token=aLTg4VOyQH)](https://codecov.io/gh/codeskyblue/appinspector)
```

