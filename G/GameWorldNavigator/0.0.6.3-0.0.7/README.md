# Comparing `tmp/GameWorldNavigator-0.0.6.3.tar.gz` & `tmp/GameWorldNavigator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GameWorldNavigator-0.0.6.3.tar", last modified: Sun Nov 19 03:06:22 2023, max compression
+gzip compressed data, was "GameWorldNavigator-0.0.7.tar", last modified: Mon May 27 06:03:14 2024, max compression
```

## Comparing `GameWorldNavigator-0.0.6.3.tar` & `GameWorldNavigator-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-11-19 03:06:22.899751 GameWorldNavigator-0.0.6.3/
-drwxrwxrwx   0        0        0        0 2023-11-19 03:06:22.881215 GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/
--rw-rw-rw-   0        0        0      790 2023-11-19 03:06:22.000000 GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-11-19 03:06:22.000000 GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-19 03:06:22.000000 GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-11-19 03:06:22.000000 GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.6.3/LICENSE
--rw-rw-rw-   0        0        0      790 2023-11-19 03:06:22.898716 GameWorldNavigator-0.0.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-11-19 03:06:22.893246 GameWorldNavigator-0.0.6.3/gamenavigator/
--rw-rw-rw-   0        0        0      473 2023-11-19 03:00:24.000000 GameWorldNavigator-0.0.6.3/gamenavigator/__init__.py
--rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.6.3/gamenavigator/config.py
-drwxrwxrwx   0        0        0        0 2023-11-19 03:06:22.897711 GameWorldNavigator-0.0.6.3/gamenavigator/core/
--rw-rw-rw-   0        0        0       95 2023-11-18 16:07:33.000000 GameWorldNavigator-0.0.6.3/gamenavigator/core/__init__.py
--rw-rw-rw-   0        0        0     3597 2023-11-18 16:10:58.000000 GameWorldNavigator-0.0.6.3/gamenavigator/core/interface.py
--rw-rw-rw-   0        0        0     1522 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.6.3/gamenavigator/core/pos.py
--rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.6.3/gamenavigator/core/rect.py
--rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.6.3/gamenavigator/exception.py
--rw-rw-rw-   0        0        0    15617 2023-11-19 02:59:33.000000 GameWorldNavigator-0.0.6.3/gamenavigator/game_controller.py
--rw-rw-rw-   0        0        0     3962 2023-11-16 05:11:35.000000 GameWorldNavigator-0.0.6.3/gamenavigator/image_recognition.py
--rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.6.3/gamenavigator/keyboard_mouse_simulation.py
--rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.6.3/gamenavigator/listener.py
--rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.6.3/gamenavigator/log.py
--rw-rw-rw-   0        0        0     1427 2023-11-18 10:42:34.000000 GameWorldNavigator-0.0.6.3/gamenavigator/ocr_recognition.py
--rw-rw-rw-   0        0        0       42 2023-11-19 03:06:22.899751 GameWorldNavigator-0.0.6.3/setup.cfg
--rw-rw-rw-   0        0        0      672 2023-11-18 13:46:18.000000 GameWorldNavigator-0.0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.011303 GameWorldNavigator-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-27 06:03:13.979457 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/
+-rw-rw-rw-   0        0        0      788 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      677 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-27 06:03:13.000000 GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1084 2023-11-14 15:46:54.000000 GameWorldNavigator-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      788 2024-05-27 06:03:14.010188 GameWorldNavigator-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-11-15 07:38:05.000000 GameWorldNavigator-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.003390 GameWorldNavigator-0.0.7/gamenavigator/
+-rw-rw-rw-   0        0        0      575 2024-05-25 01:28:35.000000 GameWorldNavigator-0.0.7/gamenavigator/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-11-14 15:30:21.000000 GameWorldNavigator-0.0.7/gamenavigator/config.py
+-rw-rw-rw-   0        0        0     3376 2024-05-26 15:31:33.000000 GameWorldNavigator-0.0.7/gamenavigator/controller.py
+drwxrwxrwx   0        0        0        0 2024-05-27 06:03:14.009181 GameWorldNavigator-0.0.7/gamenavigator/core/
+-rw-rw-rw-   0        0        0      136 2024-05-26 04:08:20.000000 GameWorldNavigator-0.0.7/gamenavigator/core/__init__.py
+-rw-rw-rw-   0        0        0      609 2024-05-26 04:19:24.000000 GameWorldNavigator-0.0.7/gamenavigator/core/image.py
+-rw-rw-rw-   0        0        0     3396 2024-05-26 04:26:37.000000 GameWorldNavigator-0.0.7/gamenavigator/core/interface.py
+-rw-rw-rw-   0        0        0     1811 2024-05-26 14:20:48.000000 GameWorldNavigator-0.0.7/gamenavigator/core/pos.py
+-rw-rw-rw-   0        0        0      758 2023-11-19 02:27:01.000000 GameWorldNavigator-0.0.7/gamenavigator/core/rect.py
+-rw-rw-rw-   0        0        0      372 2023-11-16 09:39:18.000000 GameWorldNavigator-0.0.7/gamenavigator/exception.py
+-rw-rw-rw-   0        0        0    17020 2024-05-27 04:37:24.000000 GameWorldNavigator-0.0.7/gamenavigator/game_controller.py
+-rw-rw-rw-   0        0        0     3183 2024-05-26 09:31:01.000000 GameWorldNavigator-0.0.7/gamenavigator/game_interface_controller.py
+-rw-rw-rw-   0        0        0     4148 2024-05-26 11:24:27.000000 GameWorldNavigator-0.0.7/gamenavigator/image_recognition.py
+-rw-rw-rw-   0        0        0     4325 2023-11-19 02:56:31.000000 GameWorldNavigator-0.0.7/gamenavigator/keyboard_mouse_simulation.py
+-rw-rw-rw-   0        0        0      778 2023-11-15 07:05:17.000000 GameWorldNavigator-0.0.7/gamenavigator/listener.py
+-rw-rw-rw-   0        0        0      703 2023-11-15 09:41:12.000000 GameWorldNavigator-0.0.7/gamenavigator/log.py
+-rw-rw-rw-   0        0        0     1974 2024-05-26 09:59:22.000000 GameWorldNavigator-0.0.7/gamenavigator/ocr_recognition.py
+-rw-rw-rw-   0        0        0       42 2024-05-27 06:03:14.011303 GameWorldNavigator-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      672 2024-05-27 06:02:08.000000 GameWorldNavigator-0.0.7/setup.py
```

### Comparing `GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/PKG-INFO` & `GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.6.3
+Version: 0.0.7
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.6.3/GameWorldNavigator.egg-info/SOURCES.txt` & `GameWorldNavigator-0.0.7/GameWorldNavigator.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 setup.py
 GameWorldNavigator.egg-info/PKG-INFO
 GameWorldNavigator.egg-info/SOURCES.txt
 GameWorldNavigator.egg-info/dependency_links.txt
 GameWorldNavigator.egg-info/top_level.txt
 gamenavigator/__init__.py
 gamenavigator/config.py
+gamenavigator/controller.py
 gamenavigator/exception.py
 gamenavigator/game_controller.py
+gamenavigator/game_interface_controller.py
 gamenavigator/image_recognition.py
 gamenavigator/keyboard_mouse_simulation.py
 gamenavigator/listener.py
 gamenavigator/log.py
 gamenavigator/ocr_recognition.py
 gamenavigator/core/__init__.py
+gamenavigator/core/image.py
 gamenavigator/core/interface.py
 gamenavigator/core/pos.py
 gamenavigator/core/rect.py
```

### Comparing `GameWorldNavigator-0.0.6.3/LICENSE` & `GameWorldNavigator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.6.3/PKG-INFO` & `GameWorldNavigator-0.0.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GameWorldNavigator
-Version: 0.0.6.3
+Version: 0.0.7
 Summary: A framework for game automation
 Home-page: https://github.com/JunNanLYS/GameWorldNavigator
 Author: NanJunLYS
 Author-email: 18906571516@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/core/interface.py` & `GameWorldNavigator-0.0.7/gamenavigator/core/interface.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,113 +1,105 @@
 """界面类
 通过创建一个个游戏界面类从而达到操控游戏的目的
 """
-from abc import ABC, abstractmethod
-from typing import Dict, Optional, Union, Callable
 
-from cv2.typing import MatLike
+from enum import Enum
+from typing import Dict, Union, List, Tuple
 
+from .image import Image
+from .pos import Pos
 
 
-class InterfaceBase(ABC):
-    def __init__(self, obj_name: str) -> None:
-        self.__obj_name = obj_name
+class InterfaceAction(Enum):
+    MOUSE_CLICK = 0  # 鼠标点击
+    MOUSE_MOVE = 1  # 鼠标移动
+    MOUSE_DRAG = 2  # 鼠标拖拽
+    KEYBOARD = 3  # 键盘输入
+
+
+DownTime = Union[int, float]
+InterfaceStep = List[
+    Tuple[InterfaceAction, Union[Image, str, Pos, Tuple[str, DownTime]]]
+]
+
+
+class Interface(object):
+    def __init__(
+        self,
+        id_: Union[Image, str],
+        only_name: str,
+        to_parent_steps,
+        to_child_steps,
+        root=False,
+    ):
+        """界面类
+
+        Args:
+            id_ (Union[Image, str]): 界面的唯一标识, 可以是图片也可以是字符串
+            only_name (str): 唯一名称, 不该出现重复名称
+            to_parent_steps (Union[Dict[Interface, InterfaceStep], None]): 前往父界面的步骤
+            to_child_steps (Union[Dict[Interface, InterfaceStep], None]): 前往子界面的步骤
+            root (bool, optional): 用于标识是否为根界面. Defaults to False.
+        """
+        self._id: Image | str = id_  # 用来判断当前是不是这个界面
+        self._root: bool = root  # 根界面标识
+        self._name: str = only_name  # 界面名称
+        self._to_parent_steps: Dict[Interface, InterfaceStep] = (
+            dict() if to_parent_steps is None else to_parent_steps
+        )
+        self._to_child_steps: Dict[Interface, InterfaceStep] = (
+            dict() if to_child_steps is None else to_child_steps
+        )
+
+    def add_interface(
+        self, inf: "Interface", step: InterfaceStep, is_parent: bool
+    ) -> None:
+        """添加一个界面
+
+        Args:
+            inf (Interface): 界面
+            step (InterfaceStep): 前往该新界面的步骤
+            is_parent (bool): 是否为父界面
+        """
+        if inf in self._to_parent_steps or inf in self._to_child_steps:
+            raise ValueError(f"界面{self.name}已经存在前往{inf.name}的步骤")
+        if is_parent:
+            self._to_parent_steps[inf] = step
+        else:
+            self._to_child_steps[inf] = step
 
     @property
-    def name(self) -> str:
-        return self.__obj_name
-    
-    @abstractmethod
-    def subinterface(self) -> list:
-        pass
-    
-    def __str__(self) -> str:
-        return f"<Interface : {self.__obj_name}>"
-    
-    def __repr__(self) -> str:
-        return self.__str__()
-
-
-class Interface(InterfaceBase):
-    def __init__(self, i_name: str) -> None:
-        super().__init__(i_name)
-        self.__current: "Interface" = self
-        self.__callable: Optional[Callable] = None
-        self.__items: Dict[str, "Interface"] = dict()
-        self.__parent: Optional["Interface"] = None
-    
-    def add_subinterface(self, i_obj: "Interface", callable: Callable) -> None:
-        """ 添加新的子界面 """
-        if not isinstance(i_obj, self.__class__):
-            raise TypeError("The added object must be of the same type as the current object.")
-        i_name = i_obj.name
-        if i_name in self.__items:
-            raise ValueError(f"A sub-interface named '{i_name}' already exists. Duplicate addition is not allowed.")
-        self.__items[i_name] = i_obj
-        i_obj._set_parent(self)
-        i_obj._set_callable(callable)
-    
-    def back(self) -> None:
-        if self.current() is self:
-            pass
+    def children(self) -> list["Interface"]:
+        return list(self._to_child_steps.keys())
+
+    def get_interface(self, name: str) -> Union["Interface", None]:
+        for p in self.parents:
+            if p.name == name:
+                return p
+        for c in self.children:
+            if c.name == name:
+                return c
+        return None
+
+    def get_step(self, inf: "Interface") -> InterfaceStep:
+        if inf in self._to_parent_steps:
+            return self._to_parent_steps[inf]
+        elif inf in self._to_child_steps:
+            return self._to_child_steps[inf]
         else:
-            pass
-    
-    def callable(self) -> Union[Callable, None]:
-        return self.__callable
-    
-    def current(self) -> "Interface":
-        """ 返回当前界面 """
-        return self.__current
+            raise ValueError(f"在界面{self.name}中找不到前往{inf.name}的步骤")
 
-    def get_subinterface(self, i_name: str) -> "Interface":
-        """获取界面
+    @property
+    def id(self) -> Union[Image, str]:
+        return self._id
 
-        Args:
-            i_name (str): 界面名称
-        
-        Returns:
-            Interface
-        """
-        if not isinstance(i_name, str):
-            raise TypeError("i_name type must is str")
-        if i_name not in self.__items:
-            raise KeyError(f"not have {i_name}")
-        return self.__items[i_name]
-    
-    def parent(self) -> Union["Interface", None]:
-        """ 返回父界面, 若为None则不存在父界面 """
-        return self.__parent
-    
-    def subinterface(self) -> list:
-        """ 返回所有子界面 """
-        return list(self.__items.values())
-    
-    def _set_current(self, interface: "Interface") -> None:
-        """设置当前界面
-        
-        当前界面的父界面也会被设置一直递归直至到达顶层父界面
-        
-        这么做的目的是保证顶层界面的能通过self.current()知道现在是什么界面
-        """
-        self.__current = interface
-        parent = self.parent()
-        if parent is None:
-            return
-        parent._set_current(interface)
-    
-    def _set_callable(self, callable: Callable) -> None:
-        """ 设置callable """
-        self.__callable = callable
-    
-    def _set_parent(self, interface: "Interface") -> None:
-        """ 设置父界面 """
-        self.__parent = interface
-    
-    def to_subinterface(self, i_name: str) -> None:
-        """ 前往子界面 """
-        interface = self.get_subinterface(i_name)
-        call = interface.callable()
-        if call is None:
-            raise ValueError()
-        call()
-        self._set_current(interface)
+    @property
+    def is_root(self) -> bool:
+        return self._root
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def parents(self) -> list["Interface"]:
+        return list(self._to_parent_steps.keys())
```

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/core/pos.py` & `GameWorldNavigator-0.0.7/gamenavigator/core/pos.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,64 @@
 """ 这里定义了坐标类 """
 
+from typing import overload
+
 
 class Pos:
-    def __init__(self, *args) -> None:
-        """
-        Initialize a new Pos object.
+    @overload
+    def __init__(self, pos: tuple): ...
 
-        * Pos(tuple): where tuple is of the form (x, y)
-        * Pos(x, y): where x and y are integers
+    @overload
+    def __init__(self, x: int, y: int): ...
+
+    def __init__(self, *args, **kwargs) -> None:
+        """
+        Initialization:
+            * Pos(tuple)
+            * Pos(x, y)
         """
         if len(args) == 1:
             arg = args[0]
             if isinstance(arg, tuple):
-                if len(arg) != 2:
-                    raise TypeError("Tuple must have exactly two elements")
+                if len(arg) != 2 or not all(isinstance(i, int) for i in arg):
+                    raise TypeError(
+                        "If a single argument is provided, it must be a tuple of two integers"
+                    )
                 self._x, self._y = arg
             else:
-                raise TypeError("If a single argument is provided, it must be a tuple of two integers")
+                raise TypeError(
+                    "If a single argument is provided, it must be a tuple of two integers"
+                )
         elif len(args) == 2:
             if isinstance(args[0], int) and isinstance(args[1], int):
                 self._x, self._y = args
             else:
                 raise TypeError("If two arguments are provided, they must be integers")
         else:
             raise TypeError("Pos takes either one tuple or two integers as arguments")
 
-        self.is_game = False
+        self.is_global = False
 
     @property
     def x(self) -> int:
         return self._x
 
     @property
     def y(self) -> int:
         return self._y
 
-    def __add__(self, other):
+    def __add__(self, other: "Pos") -> "Pos":
         return Pos(self.x + other.x, self.y + other.y)
 
-    def __sub__(self, other):
+    def __sub__(self, other: "Pos") -> "Pos":
         return Pos(self.x - other.x, self.y - other.y)
 
     def __str__(self):
         return f"Pos({self._x}, {self._y})"
 
     def __repr__(self):
         return self.__str__()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     p = Pos(1, 2)
     print(p)
```

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/core/rect.py` & `GameWorldNavigator-0.0.7/gamenavigator/core/rect.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/game_controller.py` & `GameWorldNavigator-0.0.7/gamenavigator/game_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import os.path
-import time
 import ctypes
-from datetime import datetime
-from typing import Union
+import time
 from threading import Thread
+from typing import Union, Optional
 
+import cv2
 import win32api
 import win32con
 import win32gui
 import win32print
-import cv2
 from PIL import ImageGrab
 from cv2.typing import MatLike
 from numpy import ndarray, array
 
+from . import log
 from .core import Pos, Rect
+from .exception import TemplateMathingFailure, WindowOutOfBoundsError, TextMatchingFailure
+from .image_recognition import match_template
 from .keyboard_mouse_simulation import (mouse_click_position, mouse_move_to, mouse_scroll,
                                         keyboard_press, keyboard_down, keyboard_up, mouse_drag)
-from .image_recognition import match_template
-from .ocr_recognition import get_text_position
-from .exception import TemplateMathingFailure, WindowOutOfBoundsError, TextMatchingFailure
-from . import log
+from .ocr_recognition import (get_text_position, get_text_direction_position)
 
 
 def _get_screen_size():
     """ 电脑缩放后的分辨率 """
     w = win32api.GetSystemMetrics(0)
     h = win32api.GetSystemMetrics(1)
     return w, h
@@ -45,15 +43,15 @@
 
 class Game:
     def __init__(self, game_class: Union[str, None], game_name: str):
         """
         :param game_class: 游戏类名
         :param game_name: 游戏名称
         """
-        self.screenshot: ndarray
+        self.screenshot: Optional[ndarray] = None
         self._game_class = game_class
         self._game_name = game_name
         self._hwnd = win32gui.FindWindow(game_class, game_name)
 
         log.debug(f"class : {game_class}, name : {game_name}, hwnd : {self._hwnd}")
 
     @property
@@ -104,42 +102,59 @@
     def get_rect(self) -> Rect:
         """ 获取游戏的矩形 """
         x1, y1, x2, y2 = win32gui.GetWindowRect(self._hwnd)
         s = _get_scaling()  # 电脑缩放率
         x1, y1 = int(x1 * s), int(y1 * s)
         x2, y2 = int(x2 * s), int(y2 * s)
         return Rect(x1, y1, x2, y2)
+    
+    def get_image_pos(self, image: Union[str, ndarray]) -> Pos:
+        """获取游戏内图片位置API
+
+        Args:
+            image (Union[str, ndarray]): 模板图
+        """
+        _, _, _, max_loc = match_template(self.get_screenshot(), image)
+        pos = Pos(max_loc[0], max_loc[1])
+        return pos
+    
+    def get_text_pos(self, text: str, direction: str = "center") -> Pos:
+        """获取游戏内文字位置API
+
+        Args:
+            text (str): 文字
+            direction (str, optional): 文字的位置方向 [left, center, right]. Defaults to "center".
+        """
+        positions = get_text_position(self.get_screenshot(), text)
+        pos = get_text_direction_position(positions, direction)
+        return pos
+        
 
 
 class GameController:
-    def __init__(self, game_class: Union[str, None], game_name: str, debug=False, filename=""):
+    def __init__(self, game_class: Union[str, None], game_name: str):
         """
         将debug设置为True后需要设置filename才会将调试信息保存
 
         Args:
             game_class (str, None): 游戏类型
             game_name (str): 游戏名称
-            debug (bool): 调试模式
-            filename (str): 调试模式存储的文件路径
         """
         self.game = Game(game_class, game_name)
-        self.debug = debug
-        self.filename = filename
 
     def click_pos(self, pos: Pos) -> None:
         """模拟鼠标点击游戏内坐标API
 
         Args:
             pos (Pos): 坐标
         """
         self.set_foreground()
         try:
             self._click_pos(pos)
         except WindowOutOfBoundsError:
-            self.image_debug("Error")
             raise
 
     def click_image(self, *images: Union[str, ndarray, MatLike], **kwargs):
         """模拟鼠标点击游戏内图片API
 
         鼠标点击图片中心位置，若传入多个图像则只会点击一个
 
@@ -152,15 +167,14 @@
             x (int): x偏移 (default 0)
             y (int): y偏移 (default 0)
         """
         self.set_foreground()
         try:
             self._click_image(*images, **kwargs)
         except TemplateMathingFailure:
-            self.image_debug("Error")
             raise
 
     def click_text(self, text: str, position: str = "center", **kwargs) -> None:
         """模拟鼠标点击游戏内文字API
 
         Args:
             text (str): 文字
@@ -173,15 +187,14 @@
         if not isinstance(text, str):
             raise TypeError("text must is str type")
         if not isinstance(position, str):
             raise TypeError("position must is str type")
         try:
             self._click_text(text, position, **kwargs)
         except TextMatchingFailure:
-            self.image_debug("Error")
             raise
 
     def down_keyboard_time(self, key: str, stop_time: float, thread=False) -> Union[None, Thread]:
         """模拟按压键盘的时间
 
         开启线程后将在子线程中运行从而不阻塞主线程，因为这个按压时间是通过time.sleep()实现的
 
@@ -213,63 +226,53 @@
         # 阻塞当前线程直到达到按压时长
         return None
 
     def get_screenshot(self) -> ndarray:
         """ 获取游戏截图 """
         return self.game.get_screenshot()
 
-    def image_debug(self, level="Debug") -> None:
-        """ 保存调试照片 """
-        if not isinstance(level, str):
-            raise TypeError("param level must is str type")
-        if self.debug and self.filename:
-            filename = self.__image_filename(level)
-            cv2.imwrite(filename, self.game.screenshot)
-
     def press(self, key: str) -> None:
         """ 模拟键盘按键按压API """
         self.set_foreground()
         keyboard_press(key)
 
     def set_foreground(self) -> None:
         """ 设置游戏到前台 """
         hwnd = win32gui.GetForegroundWindow()
         text = win32gui.GetWindowText(hwnd)
         if text != self.game.name:
             self.game.set_foreground()
             time.sleep(1)
 
     @property
-    def screenshot(self) -> ndarray:
+    def screenshot(self) -> Union[ndarray, None]:
         return self.game.screenshot
 
-    def mouse_move_to(self, pos: Pos, duration: float) -> None:
+    def mouse_move_to(self, target: Union[str, ndarray, Pos], duration: float) -> None:
         """模拟鼠标移动API
 
         鼠标从当前位置移动到pos持续duration
 
         Args:
-            pos (Pos): 坐标
+            target (Union[str, ndarray, Pos]): 坐标
             duration (float): 持续时间
         """
         self.set_foreground()
         try:
-            self._mouse_move_to(pos, duration)
+            self._mouse_move_to(target, duration)
         except WindowOutOfBoundsError:
-            self.image_debug("Error")
             raise
 
     def mouse_drag(self, start: Pos, end: Pos, button="left") -> None:
         """按压鼠标并移动到end松开API"""
         self.set_foreground()
         try:
-            start = self._to_game_pos(start)
-            end = self._to_game_pos(end)
+            start = self._to_global_pos(start)
+            end = self._to_global_pos(end)
         except WindowOutOfBoundsError:
-            self.image_debug("Error")
             raise
         mouse_drag(start, end, button)
 
     def mouse_scroll(self, pos: Pos, scale: int, count: int, duration=0.0):
         """鼠标移动至pos滚动scale刻度count次
         Args:
             pos (Pos): 坐标
@@ -297,20 +300,19 @@
         Raises:
             TimeoutError: 超时
         """
         self.set_foreground()
         try:
             self._wait_image(*images, **kwargs)
         except TimeoutError:
-            self.image_debug("Error")
             raise
 
     def _click_pos(self, pos: Pos) -> None:
         """ 点击游戏内某个坐标 """
-        game_pos = self._to_game_pos(pos)
+        game_pos = self._to_global_pos(pos)
         mouse_click_position(game_pos)
 
     def _click_image(self, *images: Union[str, ndarray, MatLike], **kwargs) -> None:
         """ 点击游戏内图片 """
         x = kwargs.get("x", 0)
         y = kwargs.get("y", 0)
         threshold = kwargs.get("threshold", 0.8)
@@ -331,15 +333,15 @@
                 raise TypeError("param image must is str or ndarray type")
             if isinstance(image, str):
                 image = cv2.imread(image)
             _, max_val, _, max_loc = match_template(screenshot, image, mode=mode)
             if max_val < threshold:
                 if max_val > v:
                     v = max_val
-                    p = Pos(max_loc)
+                    p = Pos(max_loc[0], max_loc[1])
                 continue
                 # 低于阈值的跳过
             else:
                 log.debug(f"max_val={max_val}, threshold={threshold}")
                 h, w = image.shape[:2]
                 center = Pos(max_loc[0] + w // 2, max_loc[1] + h // 2)
                 center += Pos(x, y)
@@ -365,38 +367,77 @@
         elif position == "right":
             index = -1
         position = positions[index]
         x, y = position
         pos = Pos(int(x), int(y)) + add_pos
         self.click_pos(pos)
 
-    def _mouse_move_to(self, pos: Pos, duration: float) -> None:
-        """ 将鼠标移动至某坐标点上 """
-        game_pos = self._to_game_pos(pos)
-        mouse_move_to(game_pos, duration)
-
-    def _to_game_pos(self, pos: Pos) -> Pos:
-        """ 将坐标转换成游戏坐标 """
-        if pos.is_game:
+    def _mouse_move_to(self, target: Union[str, ndarray, Pos], duration: float) -> None:
+        """鼠标移动到目标位置
+
+        Args:
+            target (Union[str, ndarray, Pos]): 目标位置,文本,图片,坐标
+            duration (float): 从当前鼠标位置移动到目标位置的时间
+        """
+        if isinstance(target, str):
+            positions = get_text_position(self.game.get_screenshot(), target)
+            pos = get_text_direction_position(positions, "center")
+        elif isinstance(target, ndarray):
+            _, _, _, max_loc = match_template(self.game.get_screenshot(), target)
+            pos = Pos(max_loc[0], max_loc[1])
+        elif isinstance(target, Pos):
+            pos = target
+        else:
+            raise TypeError("param target must is str, ndarray or Pos type")
+        global_pos = self._to_global_pos(pos)
+        mouse_move_to(global_pos, duration)
+
+    def _to_global_pos(self, pos: Pos) -> Pos:
+        """将游戏相对坐标转化成全局坐标
+
+        Args:
+            pos (Pos): 游戏内坐标
+
+        Raises:
+            WindowOutOfBoundsError: 给出的坐标超出游戏窗口范围
+
+        Returns:
+            Pos: 全局坐标
+        """
+        if pos.is_global:
             return pos
         rect = self.game.get_rect()
         x1, y1 = pos.x, pos.y
         x2, y2 = x1 + rect.left, y1 + rect.top
-        game_pos = Pos(x2, y2)
         # 坐标转换成游戏内坐标
         if x2 < rect.left or x2 > rect.right or y2 < rect.top or y2 > rect.bottom:
             log.error(f"The given coordinate ({x2}, {y2}) is outside")
             raise WindowOutOfBoundsError(f"The given coordinate ({x2}, {y2}) is outside "
                                          f"the game window bounds "
                                          f"({rect.left}, {rect.top}) - ({rect.right}, {rect.bottom})")
             # 给出的坐标超出游戏窗口范围
-        return game_pos
+        global_pos = Pos(x2, y2)
+        return global_pos
+
+    def _wait_image(self, *images: Union[str, ndarray], **kwargs) -> None:
+        """等待图片
+        阻塞线程等待图片出现或者超市
+        
+        Args:
+            *images (Union[str, ndarray]): 图片路径,图片,图片模板
+            all (bool, optional): 是否需要所有图片同时出现. Defaults to False.
+            threshold (float, optional): 匹配阈值. Defaults to 0.8.
+            mode (str, optional): 匹配模式. Defaults to "color".
+            timeout (int, optional): 超时时间. Defaults to 60.
+            spacing (int, optional): 图片间隔时间. Defaults to 1.
 
-    def _wait_image(self, *images: Union[str, ndarray, MatLike], **kwargs) -> None:
-        """ 等待图片 """
+        Raises:
+            TypeError: 参数类型错误
+            TimeoutError: 超时
+        """
         all_ = kwargs.get("all", False)
         threshold = kwargs.get("threshold", 0.8)
         mode = kwargs.get("mode", "color")
         timeout = kwargs.get("timeout", 60)  # second
         spacing = kwargs.get("spacing", 1)  # second
         start_time = time.time()
         length = len(images)
@@ -423,14 +464,7 @@
                         return
                 if count == length:
                     # 全部匹配成功
                     return
             time.sleep(spacing)
         log.error(f"Wait timeout: timeout={timeout}, spacing={spacing}")
         raise TimeoutError(f"Wait timeout")
-
-    def __image_filename(self, level: str) -> str:
-        """ 获取图片保存名称 """
-        return os.path.join(self.filename,
-                            f"[{level}]" +
-                            datetime.now().strftime("%Y-%m-%d (%H-%M-%S)") +
-                            ".png")
```

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/image_recognition.py` & `GameWorldNavigator-0.0.7/gamenavigator/image_recognition.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,98 +1,105 @@
+from ast import Tuple
 import cv2
 import numpy as np
 from typing import Union
-from cv2.typing import MatLike
+from cv2.typing import MatLike, Point
 
 
 def __to_ndarray(img: Union[str, np.ndarray, MatLike]) -> Union[np.ndarray, MatLike]:
-    """ 若img是图像路径则读取后返回，否则直接返回 """
+    """若img是图像路径则读取后返回，否则直接返回"""
     if isinstance(img, str):
         img = cv2.imread(img)
     return img
 
 
-def match_template(img: Union[str, np.ndarray, MatLike], template: Union[str, np.ndarray, MatLike], **kwargs) -> tuple:
+def match_template(
+    img: Union[str, np.ndarray], template: Union[str, np.ndarray], **kwargs
+) -> tuple[float, float, Point, Point]:
     """图像匹配
     使用的是cv2的模板匹配，必须要保证 img 和 template 是属于同一种类型图像，即都是灰度图或彩色图，且大小一致。
     使用的是cv2.TM_CCOEFF_NORMED进行模板匹配，可以通过修改method来自定义模板匹配。图像必须是BGR格式
 
     Keyword Arguments:
         method (str): 模板匹配方法，默认是TM_CCOEFF_NORMED  str类型
         mode (str): 匹配模式 color binary gray (default color)
         thresh (int): 只有在二值图模式下才有用  int类型
         max_val (int): 只有在二值图模式下才有用  int类型
 
     Returns:
         min_val, max_val, min_loc, max_loc
     """
-    if not isinstance(img, (str, np.ndarray, MatLike)):
+    if not isinstance(img, (str, np.ndarray)):
         raise TypeError("only accept str or np.ndarray or MatLike")
-    elif not isinstance(template, (str, np.ndarray, MatLike)):
+    elif not isinstance(template, (str, np.ndarray)):
         raise TypeError("only accept str or np.ndarray or MatLike")
 
     img = __to_ndarray(img)
     template = __to_ndarray(template)
 
     method = kwargs.get("method", "TM_CCOEFF_NORMED")
-    methods = ("TM_SQDIFF", "TM_SQDIFF_NORMED", "TM_CCOEFF_NORMED",
-               "TM_CCORR_NORMED", "TM_CCORR", "TM_CCOEFF")
+    methods = (
+        "TM_SQDIFF",
+        "TM_SQDIFF_NORMED",
+        "TM_CCOEFF_NORMED",
+        "TM_CCORR_NORMED",
+        "TM_CCORR",
+        "TM_CCOEFF",
+    )
     mode = kwargs.get("mode", "color")
     modes = ("color", "gray", "binary")
 
     # 判断传入的关键词是否支持
     if method not in methods:
         raise ValueError(f"method must in {methods}")
     elif mode not in modes:
         raise ValueError(f"mode must in {modes}")
 
-    method = getattr(cv2, method)
     i_channel = img.ndim
     t_channel = template.ndim
+    
+    match mode:
+        case "color":
+            if i_channel != 3 or t_channel != 3:
+                raise ValueError("Image or template channels not equal to 3")
+            res = cv2.matchTemplate(img, template, method)
+            return cv2.minMaxLoc(res)
+        case "gray":
+            img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) if i_channel == 3 else img
+            template_gray = cv2.cvtColor(template, cv2.COLOR_BGR2GRAY) if t_channel == 3 else template
+            res = cv2.matchTemplate(img_gray, template_gray, method)
+            return cv2.minMaxLoc(res)
+        case "binary":
+            img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) if i_channel == 3 else img
+            template_gray = cv2.cvtColor(template, cv2.COLOR_BGR2GRAY) if t_channel == 3 else template
+            thresh = kwargs.get("thresh", 127)
+            max_val = kwargs.get("max_val", 255)
+            _, img_binary = cv2.threshold(img_gray, thresh, max_val, cv2.THRESH_BINARY)
+            _, template_binary = cv2.threshold(
+                template_gray, thresh, max_val, cv2.THRESH_BINARY
+            )
+            res = cv2.matchTemplate(img_binary, template_binary, method)
+            return cv2.minMaxLoc(res)
+        case _:
+            raise ValueError("mode must in ('color', 'gray', 'binary')")
+
+
+def where_img(
+    img: Union[str, np.ndarray],
+    template: Union[str, np.ndarray],
+    threshold=0.8,
+) -> tuple:
+    """查找所有匹配的图片
+
+    Args:
+        img (Union[str, np.ndarray]): 要检测的图片
+        template (Union[str, np.ndarray]): 模板图片
+        threshold (float, optional): 阈值,大于等于该阈值的对象被视为是类似图片. Defaults to 0.8.
 
-    if mode == "gray" or mode == "binary":
-        if i_channel == 3:
-            img_gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-        else:
-            img_gray = img
-        if t_channel == 3:
-            template_gray = cv2.cvtColor(template, cv2.COLOR_BGR2GRAY)
-        else:
-            template_gray = template
-    else:
-        img_gray = None
-        template_gray = None
-    # 若模式需要灰度图则先将彩色图转换成灰度图
-
-    if mode == "color":
-        if i_channel != 3 or t_channel != 3:
-            raise ValueError("Image or template channels not equal to 3")
-        res = cv2.matchTemplate(img, template, method)
-        return cv2.minMaxLoc(res)
-        # 彩色图模式
-    elif mode == "gray":
-        res = cv2.matchTemplate(img_gray, template_gray, method)
-        return cv2.minMaxLoc(res)
-        # 灰度图模式
-    else:
-        thresh = kwargs.get("thresh", 127)
-        max_val = kwargs.get("max_val", 255)
-        _, img_binary = cv2.threshold(img_gray, thresh, max_val, cv2.THRESH_BINARY)
-        _, template_binary = cv2.threshold(template_gray, thresh, max_val, cv2.THRESH_BINARY)
-        res = cv2.matchTemplate(img_binary, template_binary, method)
-        return cv2.minMaxLoc(res)
-        # 二值图模式
-
-
-def where_img(img: Union[str, np.ndarray, MatLike], template: Union[str, np.ndarray, MatLike], threshold=0.8) -> tuple:
-    """
-    查找目标图中所有符合阈值的模板图位置，暂时只支持cv2.TM_CCOEFF_NORMED。
-    :param img: 目标图
-    :param template: 模板图
-    :param threshold: 符合该阈值的留下
-    :return: tuple[(x, y), (x, y)]
+    Returns:
+        tuple: 一个元组,包含所有匹配的图片坐标
     """
     img = __to_ndarray(img)
     template = __to_ndarray(template)
     res = cv2.matchTemplate(img, template, cv2.TM_CCOEFF_NORMED)
     positions = np.where(res >= threshold)
     return tuple(zip(*positions[::-1]))
```

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/keyboard_mouse_simulation.py` & `GameWorldNavigator-0.0.7/gamenavigator/keyboard_mouse_simulation.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/listener.py` & `GameWorldNavigator-0.0.7/gamenavigator/listener.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.6.3/gamenavigator/log.py` & `GameWorldNavigator-0.0.7/gamenavigator/log.py`

 * *Files identical despite different names*

### Comparing `GameWorldNavigator-0.0.6.3/setup.py` & `GameWorldNavigator-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="GameWorldNavigator",
-    version="0.0.6.3",
+    version="0.0.7",
     author="NanJunLYS",
     author_email="18906571516@163.com",
     description="A framework for game automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/JunNanLYS/GameWorldNavigator",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
+
```

