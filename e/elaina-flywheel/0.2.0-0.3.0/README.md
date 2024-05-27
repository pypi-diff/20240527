# Comparing `tmp/elaina_flywheel-0.2.0.tar.gz` & `tmp/elaina_flywheel-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elaina_flywheel-0.2.0.tar", last modified: Tue Mar 19 10:55:21 2024, max compression
+gzip compressed data, was "elaina_flywheel-0.3.0.tar", last modified: Mon May 27 06:54:21 2024, max compression
```

## Comparing `elaina_flywheel-0.2.0.tar` & `elaina_flywheel-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0    13250 2024-03-19 10:54:51.040150 elaina_flywheel-0.2.0/README.md
--rw-r--r--   0        0        0      537 2024-03-19 10:55:21.235282 elaina_flywheel-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      720 2024-03-18 10:03:02.078491 elaina_flywheel-0.2.0/src/flywheel/__init__.py
--rw-r--r--   0        0        0     1911 2024-03-19 10:53:31.497957 elaina_flywheel-0.2.0/src/flywheel/context.py
--rw-r--r--   0        0        0     1652 2024-03-16 15:32:30.414665 elaina_flywheel-0.2.0/src/flywheel/entity.py
--rw-r--r--   0        0        0      328 2024-03-18 10:03:19.543745 elaina_flywheel-0.2.0/src/flywheel/fn/__init__.py
--rw-r--r--   0        0        0      915 2024-03-16 15:32:30.419216 elaina_flywheel-0.2.0/src/flywheel/fn/__pycache__/base.d.er
--rw-r--r--   0        0        0     1088 2024-03-16 15:32:30.421331 elaina_flywheel-0.2.0/src/flywheel/fn/__pycache__/compose.d.er
--rw-r--r--   0        0        0      592 2024-03-16 15:32:30.429708 elaina_flywheel-0.2.0/src/flywheel/fn/__pycache__/overload.d.er
--rw-r--r--   0        0        0      614 2024-03-16 15:32:30.439283 elaina_flywheel-0.2.0/src/flywheel/fn/__pycache__/record.d.er
--rw-r--r--   0        0        0     2226 2024-03-19 06:39:09.426716 elaina_flywheel-0.2.0/src/flywheel/fn/base.py
--rw-r--r--   0        0        0     2289 2024-03-16 15:32:30.444993 elaina_flywheel-0.2.0/src/flywheel/fn/compose.py
--rw-r--r--   0        0        0     2383 2024-03-19 01:03:19.133667 elaina_flywheel-0.2.0/src/flywheel/fn/implement.py
--rw-r--r--   0        0        0     1675 2024-03-16 15:32:30.454282 elaina_flywheel-0.2.0/src/flywheel/fn/overload.py
--rw-r--r--   0        0        0      504 2024-03-16 15:37:36.381806 elaina_flywheel-0.2.0/src/flywheel/fn/record.py
--rw-r--r--   0        0        0     1758 2024-03-16 15:32:30.459371 elaina_flywheel-0.2.0/src/flywheel/globals.py
--rw-r--r--   0        0        0      656 2024-03-16 15:32:30.459873 elaina_flywheel-0.2.0/src/flywheel/instance_of.py
--rw-r--r--   0        0        0     2643 2024-03-16 15:32:30.461900 elaina_flywheel-0.2.0/src/flywheel/overloads.py
--rw-r--r--   0        0        0     3519 2024-03-18 15:32:38.353908 elaina_flywheel-0.2.0/src/flywheel/scoped.py
--rw-r--r--   0        0        0     1611 2024-03-19 10:49:13.365450 elaina_flywheel-0.2.0/src/flywheel/typing.py
--rw-r--r--   0        0        0    13473 1970-01-01 00:00:00.000000 elaina_flywheel-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13409 2024-05-27 06:49:30.463543 elaina_flywheel-0.3.0/README.md
+-rw-r--r--   0        0        0      537 2024-05-27 06:54:21.770278 elaina_flywheel-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      624 2024-05-27 01:01:08.379222 elaina_flywheel-0.3.0/src/flywheel/__init__.py
+-rw-r--r--   0        0        0     1911 2024-05-27 06:31:35.142272 elaina_flywheel-0.3.0/src/flywheel/context.py
+-rw-r--r--   0        0        0     1644 2024-05-27 01:33:11.701896 elaina_flywheel-0.3.0/src/flywheel/entity.py
+-rw-r--r--   0        0        0      384 2024-05-27 01:01:08.380685 elaina_flywheel-0.3.0/src/flywheel/fn/__init__.py
+-rw-r--r--   0        0        0     1245 2024-05-27 06:35:13.160091 elaina_flywheel-0.3.0/src/flywheel/fn/base.py
+-rw-r--r--   0        0        0      575 2024-05-27 06:30:59.379275 elaina_flywheel-0.3.0/src/flywheel/fn/compose.py
+-rw-r--r--   0        0        0     2720 2024-05-27 06:33:50.358207 elaina_flywheel-0.3.0/src/flywheel/fn/endpoint.py
+-rw-r--r--   0        0        0     2013 2024-05-27 06:31:44.100467 elaina_flywheel-0.3.0/src/flywheel/fn/harvest.py
+-rw-r--r--   0        0        0     1691 2024-05-27 01:33:11.702096 elaina_flywheel-0.3.0/src/flywheel/fn/implement.py
+-rw-r--r--   0        0        0     1755 2024-05-27 01:19:13.351484 elaina_flywheel-0.3.0/src/flywheel/fn/overload.py
+-rw-r--r--   0        0        0      649 2024-05-27 01:33:11.702247 elaina_flywheel-0.3.0/src/flywheel/fn/record.py
+-rw-r--r--   0        0        0     2007 2024-04-30 15:33:51.950821 elaina_flywheel-0.3.0/src/flywheel/globals.py
+-rw-r--r--   0        0        0      640 2024-05-27 01:33:11.700885 elaina_flywheel-0.3.0/src/flywheel/instance_of.py
+-rw-r--r--   0        0        0     2639 2024-05-27 01:33:11.700777 elaina_flywheel-0.3.0/src/flywheel/overloads.py
+-rw-r--r--   0        0        0     2759 2024-05-27 06:47:07.038627 elaina_flywheel-0.3.0/src/flywheel/scoped.py
+-rw-r--r--   0        0        0      552 2024-05-27 06:39:50.190922 elaina_flywheel-0.3.0/src/flywheel/typing.py
+-rw-r--r--   0        0        0    13632 1970-01-01 00:00:00.000000 elaina_flywheel-0.3.0/PKG-INFO
```

### Comparing `elaina_flywheel-0.2.0/README.md` & `elaina_flywheel-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,70 @@
 # Ryanvk Flywheel
 
-Ryanvk Flywheel 是一个 Ryanvk-style 的 utility，其提供强大的 `Fn`、`FnOverload`，实现了在单一入口点上的几近*完美*的自由重载。  
-...而更为可贵的是，Flywheel 具有*前沿级*的类型支持。
+Ryanvk Flywheel 是一个 Ryanvk-style 的 utility。
 
-这个库是专门为 Avilla 轻量化定制的，你可以在[这里](https://github.com/GraiaProject/Avilla/tree/master/avilla/core/flywheel) 找到与本仓库相同的内容，相比标准版的 Ryanvk，其体量仅为其一半不到。  
-本仓库中的内容预计不会在 PyPI 上发布单独的 `flywheel` 包，请自行使用 VcsRequirement 方式导入你的项目。
+- 在单一入口点上的*几近完美*的自由重载；
+- 简单灵活的重载机制；
+- *前沿级*的类型支持[^1]；
+- 可切换上下文。
+
+Available on PyPI: `elaina-flywheel`。
+
+[^1]: 仅在 Pyright / Basedpyright 上可用。
 
 ## 使用
 
 Flywheel 着重于围绕 `Fn` 建设，以提供强大的重载功能为目的。
 
 可以通过这种方法创建一个使用*简单重载*(`SimpleOverload`)的 `Fn`。
 
 ```python
 from typing import Protocol
 
-from flywheel import Fn, FnCompose, OverloadRecorder, FnRecord, SimpleOverload
+from flywheel import Fn, FnCompose, FnRecord, SimpleOverload, FnCollectEndpoint
 
-@Fn.declare
+@Fn
 class greet(FnCompose):
     name = SimpleOverload("name")
 
-    def call(self, record: FnRecord, name: str) -> str:
-        entities = self.load(self.name.dig(record, name))
-        # entities 会自动读取到 collect 中对于 implement 参数的类型。
+    def call(self, records, name: str) -> str:
+        # 我们不关心 records 的类型。
+        # 如果你在乎，它的类型是 dict[FnCollectEndpoint, FnImplementEntity]
 
+        entities = self.someone(records).use(self.name, name)
         return entities.first(name)
-    
-    # 定义 Fn 面向的具体实现的类型...
-    class ShapeCall(Protocol):
-        def __call__(self, name: str) -> str:
-            ...
-
-    # ...并在 collect 方法中引用，这是可选的，仅影响 load 方法的返回类型。
-    def collect(self, recorder: OverloadRecorder[ShapeCall], *, name: str):
-        recorder.use(self.name, name)
+
+    @FnCollectEndpoint
+    @classmethod
+    def someone(cls, *, name: str):
+        yield cls.name.hold(name)
+
+        # 可选的，你可以给出实现的类型，运行时中我们不关心这个，所以你可以放在 if TYPE_CHECKING 中。
+        def shape(name: str) -> str: ...
+        return shape
 ```
 
 然后我们为 `greet` 提出两个实现：
 
 - 当 `name` 是 `Teague` 的时候返回 `"Stargaztor, but in name only."`；
 - 当 `name` 是 `Grey` 的时候返回 `"Symbol, the Founder."`：
 
 当提出实现后，我们还得将其收集起来，这样 Flywheel 的内部系统才能调用的到这些实现。
 在这里，我们使用 `global_collect` 函数，将实现收集到全局上下文中。
 
 ```python
 from flywheel import global_collect
 
 @global_collect
-@greet.impl(name="Teague")
+@greet._.someone(name="Teague")
 def greet_teague(name: str) -> str:
     return "Stargaztor, but in name only."
 
 @global_collect
-@greet.impl(name="Grey")
+@greet._.someone(name="Grey")
 def greet_grey(name: str) -> str:
     return "Symbol, the Founder."
 ```
 
 然后我们调用。
 
 ```python
@@ -76,19 +82,21 @@
 ```
 
 显然，我们并没有面向 `"Hizuki"` 实现一个 `greet`。为了使我们的程序能处理这种情况，我们可以这样修改 `greet` 的声明：
 
 ```python
 @Fn.declare
 class greet(FnCompose):
-    name = SimpleOverload("name")
+    name = SimpleOverload("name")  # 指定 name 是必要的。
 
-    def call(self, record: FnRecord, name: str) -> str:
-        entities = self.load(self.name.dig(record, name))
-        # entities 会自动读取到 collect 中对于 implement 参数的类型。
+    def call(self, records, name: str) -> str:
+        # 我们不关心 records 的类型。
+        # 如果你在乎，它的类型是 dict[FnCollectEndpoint, FnImplementEntity]
+
+        entities = self.someone(records).use(self.name, name)
 
         if not entities:  # 判断是否存在符合条件的实现
             return f"Ordinary, {name}."
 
         return entities.first(name)
 ```
 
@@ -151,14 +159,25 @@
             return scope[signature.value]
 ```
 
 你可以尝试借由这个例子来实现一个依据调用时值 (`call_value`) 的类型来找到对应的实现的 `TypeOverload`，作为参考答案，你可以在 `flywheel.overloads` 模块中找到同名的实现。
 
 对于 `FnOverload` 来说，他不一定要搜索尽可能多的实现 —— 这根据实际情况来决定：如果你希望你的 Fn 表现的像是个事件系统，这种情况下你最好找到尽可能多的实现 —— 不幸的，我们没有提供什么 `greed` 参数，因此你需要自己实现。
 
+你可以添加构造器参数，并继承现有的其他重载实现。
+
+```python
+class SomeMaybeGreedOverload(FnOverload):
+    def __init__(self, name: str, greed: bool):
+        self.name = name
+        self.greed = greed
+
+    ...  # 你的实际逻辑
+```
+
 ## 上下文
 
 Flywheel 提供了一个 `global_collect` 函数，用于将实现收集到全局上下文中。自然，上下文不会只有一个，Flywheel 允许你创建自己的上下文，并在你期望的时候应用。
 
 相应的，全局上下文存储在 `flywheel.globals.GLOBAL_COLLECT_CONTEXT`，如果你知道你在做什么有所必要的事情，这一信息可能对你有用。但我想大多数情况下你都不会使用到这一技巧。
 
 ```python
@@ -180,20 +199,20 @@
 
 需要注意的是，`global_collect` 函数的行为并不会因为上下文的存在而改变，为此，你需要考虑使用 `local_collect` 来将实现收集到你的上下文中。
 
 ```python
 from flywheel import local_collect
 
 @local_collect
-@greet.impl(name="Teague")
+@greet._.someone(name="Teague")
 def greet_teague(name: str) -> str:
     return "Stargaztor, but in name only."
 
 @local_collect
-@greet.impl(name="Grey")
+@greet._.someone(name="Grey")
 def greet_grey(name: str) -> str:
     return "Symbol, the Founder."
 ```
 
 如果你在这之前并没有使用过 `collect_scope`，`local_collect` 会采用默认行为，将实现收集到全局上下文中。
 
 但我们不建议在所有情况下都使用 `local_collect`，而是尽可能的使用 `global_collect`，
@@ -204,73 +223,58 @@
 如果你希望你的模块保持命名空间的整洁，采用 `scoped_collect` 或许是不错的主意。只是他还有其他更重要的应用，且听我娓娓道来。
 
 ```python
 from flywheel import scoped_collect
 
 class greet_implements(m := scoped_collect.globals().target, static=True):
     @m.collect
-    @greet.impl(name="Teague")
+    @greet._.someone(name="Teague")
     @m.ensure_self
     def greet_teague(self, name: str) -> str:
         return "Stargaztor, but in name only."
 
-    # 上面的写法未免过于冗长，可以考虑使用这种写法，基本等效。
-
-    @m.impl(greet, name="Grey")
-    def greet_grey(self, name: str) -> str:
-        return "Symbol, the Founder."
+    # 上面的写法未免过于冗长，我们正在考虑更好的办法。
 ```
 
 这段代码使用 `scoped_collect` 实现了和我们最初给出的两个 `greet_xxx` 一样的效果。
 
 ```python
 >>> greet("Teague")
 'Stargaztor, but in name only.'
 >>> greet("Grey")
 'Symbol, the Founder.'
 ```
 
-这段代码使用 `scoped_collect.globals()` 方法连接到了全局上下文。如果你不想这样，需要换成 `scoped_collect.env()`。
+这段代码使用 `scoped_collect.globals()` 方法连接到了全局上下文。如果你不想这样，需要换成 `scoped_collect.locals()`。
 
 ```python
 from flywheel import scoped_collect
 
-class greet_implements(m := scoped_collect.env().target, static=True):
+class greet_implements(m := scoped_collect.locals().target, static=True):
     ...
 ```
 
 `static=True` 时，`greet_implements` 会被实例化并保存到全局中的*实例上下文* (Instance Context) 中。  
 如果你自定义了你的构造方法 (即 `__init__` 或 `__new__`)，则会在启动时报错，此时你需要自己实现对 `InstanceContext` 的生成与应用。
 
 ## 叠加
 
 Flywheel 允许你这么做...：
 
 ```python
 @global_collect
-@greet.impl(name="Teague")
-@greet.impl(name="Grey")
+@greet._.someone(name="Teague")
+@greet._.someone(name="Grey")
 def greet_stargaztor(name: str) -> str:
     return f"Stargaztor"
 ```
 
-他等同于分别调用 `Fn.impl` 方法，但写的更简短，同时你依旧能获得 Flywheel 前沿级的类型支持。
+他等同于分别调用 `FnCollectEntity`，但写的更简短，同时你依旧能获得 Flywheel 前沿级的类型支持。
 
-当你配合 `scoped_collect` 使用时，可以直接使用 `m.impl` 方法，其将自动处理 `m.collect` 与 `m.ensure_self`。
-
-```python
-# 不需要手动调用 `m.collect` 与 `m.ensure_self`。
-
-@m.impl(greet, name="Teague")
-@m.impl(greet, name="Grey")
-def greet_stargaztor(self, name: str) -> str:
-    return "Stargaztor"
-```
-
-如果执意想要使用原始的方式，请注意将 `Fn.impl` 调用*夹*在 `m.collect` 与 `m.ensure_self` 中间：
+如果需配合 `scoped_collect` 使用，注意将 `Fn.impl` 调用*夹*在 `m.collect` 与 `m.ensure_self` 中间：
 
 ```python
 @m.collect
 @greet.impl(name="Teague")
 @greet.impl(name="Grey")
 @m.ensure_self
 def greet_teague(self, name: str) -> str:
@@ -322,15 +326,15 @@
 我们提供了可以自动访问当前实例上下文的描述符 `InstanceOf`，通过这一措施，你可以方便的访问实例上下文中的内容。
 
 ```python
 from flywheel import InstanceOf
 
 from aiohttp import ClientSession
 
-class sth_implements(m := scoped_collect.env().target, static=True):
+class sth_implements(m := scoped_collect.locals().target, static=True):
     session = InstanceOf(ClientSession)
 
     @m.impl(...)
     async def something(self, num: int):
         await self.session.get(f"http://example.com/", params={"num": num})
 
 # -----
@@ -339,14 +343,35 @@
     instance_cx.instances[ClientSession] = self.aiohttp_session
 
     await fn(10)
 ```
 
 从该示例中你也可以了解到 Flywheel 对异步的支持，理论上也能一并支持生成器，异步生成器甚至 `contextlib.contextmanager`，但如果出了问题，欢迎汇报至 issues.
 
+### 重写 static 实例化行为
+
+通过重写类方法 (classmethod) `build_static`，你可以自定义 `static` 参数的实例化行为。
+
+```python
+class sth_implements(m := scoped_collect.locals().target, static=True):
+    session = InstanceOf(ClientSession)
+
+    def __init__(self, session: ClientSession):
+        self.session = session
+
+    @m.impl(...)
+    async def something(self, num: int):
+        await self.session.get(f"http://example.com/", params={"num": num})
+
+    @classmethod
+    def build_static(cls):
+        return cls(GLOBAL_AIOHTTP_SESSION)
+```
+
+
 ### 全局上下文
 
 Flywheel 同样提供了全局的实例上下文。
 
 ```python
 from flywheel.globals import GLOBAL_INSTANCE_CONTEXT
```

### Comparing `elaina_flywheel-0.2.0/pyproject.toml` & `elaina_flywheel-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elaina-flywheel"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = [
     { name = "Elaina", email = "GreyElaina@outlook.com" },
 ]
 dependencies = [
     "typing-extensions>=4.10.0",
 ]
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/__init__.py` & `elaina_flywheel-0.3.0/src/flywheel/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from .context import CollectContext as CollectContext
 from .context import InstanceContext as InstanceContext
 from .fn import Fn as Fn
 from .fn import FnCompose as FnCompose
-from .fn import FnImplement as FnImplement
 from .fn import FnImplementEntity as FnImplementEntity
 from .fn import FnOverload as FnOverload
 from .fn import FnRecord as FnRecord
-from .fn import OverloadRecorder as OverloadRecorder
 from .globals import global_collect as global_collect
 from .globals import local_collect as local_collect
 from .instance_of import InstanceOf as InstanceOf
 from .overloads import SimpleOverload as SimpleOverload
 from .overloads import TypeOverload as TypeOverload
 from .scoped import scoped_collect as scoped_collect
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/context.py` & `elaina_flywheel-0.3.0/src/flywheel/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from collections import ChainMap
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Mapping, MutableMapping
 
-from .typing import TEntity
+from .typing import RecordsT, TEntity
 
 if TYPE_CHECKING:
-    from .fn.record import FnImplement, FnRecord
+    from .fn.record import FnImplement
 
 
 class CollectContext:
-    fn_implements: dict[FnImplement, FnRecord]
+    fn_implements: dict[FnImplement, RecordsT]
 
     def __init__(self):
         self.fn_implements = {}
 
     def collect(self, entity: TEntity) -> TEntity:
         return entity.collect(self)
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/entity.py` & `elaina_flywheel-0.3.0/src/flywheel/entity.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,16 +21,15 @@
         self.collect_context = collector
 
         if isinstance(self.collect_context, scoped_collect):
             self.collect_context.on_collected(self._fallback_collected_callback)
 
         return self
 
-    def assign_callback(self, info: EntityAssignInfo):
-        ...
+    def assign_callback(self, info: EntityAssignInfo): ...
 
     @final
     def _fallback_collected_callback(self, collector):
         self.assign_callback({})
 
     def __set_name__(self, owner: type, name: str):
         if self.collect_context is None:
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/fn/implement.py` & `elaina_flywheel-0.3.0/src/flywheel/fn/endpoint.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,90 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Any, Callable, Generic
+from dataclasses import dataclass
+from typing import TYPE_CHECKING, Any, Callable, Generator, Generic, Protocol, TypeVar, overload
 
-from typing_extensions import Concatenate
+from typing_extensions import Concatenate, ParamSpec
 
-from ..context import CollectContext
-from ..entity import BaseEntity
-from ..typing import CR, P
-from .record import FnRecord
+from ..typing import RecordsT
+from .compose import FnCompose
+from .harvest import FnHarvestControl
+from .implement import FnImplementEntity
+from .record import FnOverloadSignal
+
+T = TypeVar("T")
+T_contra = TypeVar("T_contra", contravariant=True)
+C = TypeVar("C", bound=Callable)
+C_contra = TypeVar("C_contra", contravariant=True, bound=Callable)
+P = ParamSpec("P")
+K = TypeVar("K")
+
+K1 = TypeVar("K1")
+P1 = ParamSpec("P1")
+R = TypeVar("R", covariant=True)
+P2 = ParamSpec("P2")
+
+CollectEndpointTarget = Generator[FnOverloadSignal, None, T]
+
+
+class EndpointCollectReceiver(Protocol[C]):
+    @overload
+    def __call__(self, value: FnImplementEntity[C]) -> FnImplementEntity[C]: ...
+    @overload
+    def __call__(self, value: C) -> FnImplementEntity[C]: ...
+
+
+@dataclass(init=False, eq=True, unsafe_hash=True)
+class FnCollectEndpoint(Generic[P, C_contra]):  # FIXME: should <: classmethod.
+    @overload
+    def __init__(
+        self: FnCollectEndpoint[P1, Callable],
+        target: Callable[Concatenate[Any, P1], CollectEndpointTarget[T]],
+    ): ...
+
+    @overload
+    def __init__(
+        self: FnCollectEndpoint[P1, Callable[P2, R]],
+        target: Callable[Concatenate[Any, P1], CollectEndpointTarget[Callable[P2, R] | Any]],
+    ) -> None: ...
+
+    def __init__(self, target):
+        if TYPE_CHECKING:
+            self.target = target
+        else:
+            self.target = target.__func__
 
-if TYPE_CHECKING:
-    from .base import Fn
-    from .overload import FnOverload, TCollectValue
+    def __set_name__(self, owner: type[FnCompose], name: str):
+        self.compose = owner
 
+    @property
+    def fn(self):
+        return self.compose.fn
 
-@dataclass
-class OverloadRecorder(Generic[CR]):
-    target: FnRecord
-    implement: CR
-    operators: list[tuple[str, FnOverload, Any]] = field(default_factory=list)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.done()
-
-    def done(self):
-        entity_identity = []
-
-        for name, rule, value in self.operators:
-            rule.lay(self.target, value, self.implement, name=name)
-            entity_identity.append((name, rule, rule.digest(value)))
-
-        self.target.entities[frozenset(entity_identity)] = self.implement
-
-    def use(self, target: FnOverload[Any, TCollectValue, Any], value: TCollectValue, *, name: str | None = None):
-        self.operators.append((name or target.name, target, value))
-        return self
-
-
-class FnImplementEntity(Generic[CR], BaseEntity):
-    targets: list[tuple[Fn, tuple[Any, ...], dict[str, Any]]]
-    impl: CR
-
-    def __init__(self, impl: CR):
-        self.targets = []
-        self.impl = impl
+    @overload
+    def __get__(self, instance: None, owner: type[K]) -> Callable[P, EndpointCollectReceiver[C_contra]]:
+        ...
 
-    def add_target(self, fn: Fn[Callable[Concatenate[Any, P], Any], Any], *args: P.args, **kwargs: P.kwargs):
-        self.targets.append((fn, args, kwargs))
+    @overload
+    def __get__(
+        self, instance: FnCompose, owner: Any
+    ) -> Callable[[RecordsT], FnHarvestControl[C_contra]]: ...
 
-    def collect(self, collector: CollectContext):
-        super().collect(collector)
+    def __get__(self, instance, owner) -> Any:
+        if instance is None:
 
-        for fn, args, kwargs in self.targets:
-            record_signature = fn.desc.signature()
-            if record_signature in collector.fn_implements:
-                record = collector.fn_implements[record_signature]
-            else:
-                record = collector.fn_implements[record_signature] = FnRecord(fn)
+            def collect_wrapper(*args: P.args, **kwargs: P.kwargs):
+                def receive(entity: C | FnImplementEntity) -> FnImplementEntity[C]:
+                    if not isinstance(entity, FnImplementEntity):
+                        entity = FnImplementEntity(entity)
 
-            with OverloadRecorder(record, self.impl) as recorder:
-                fn.desc.collect(recorder, *args, **kwargs)
+                    entity.add_target(self, owner, *args, **kwargs)
+                    return entity
 
-        return self
+                return receive
 
-    def _call(self, *args, **kwargs):
-        return self.impl(*args, **kwargs)
+            return collect_wrapper
 
-    @property
-    def __call__(self) -> CR:
-        return self._call  # type: ignore
+        def harvest_wrapper(records: RecordsT):
+            return FnHarvestControl(self, instance, records)
 
-    @property
-    def super(self) -> CR:
-        return self.targets[0][0].__call__
+        return harvest_wrapper
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/fn/overload.py` & `elaina_flywheel-0.3.0/src/flywheel/fn/overload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Generic, TypeVar
+from typing import Callable, Generic, TypeVar
 
 from typing_extensions import final
 
-if TYPE_CHECKING:
-    from .record import FnRecord
+from .record import FnOverloadSignal, FnRecord
 
 TOverload = TypeVar("TOverload", bound="FnOverload", covariant=True)
 TCallValue = TypeVar("TCallValue")
 TCollectValue = TypeVar("TCollectValue")
 TSignature = TypeVar("TSignature")
 
 
 class FnOverload(Generic[TSignature, TCollectValue, TCallValue]):
     def __init__(self, name: str) -> None:
         self.name = name
 
     @final
+    def hold(self, value: TCollectValue):
+        return FnOverloadSignal(self, value)
+
+    @final
     def dig(self, record: FnRecord, call_value: TCallValue, *, name: str | None = None) -> dict[Callable, None]:
         name = name or self.name
         if name not in record.scopes:
             raise NotImplementedError("cannot lookup any implementation with given arguments")
 
         return self.harvest(record.scopes[name], call_value)
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/globals.py` & `elaina_flywheel-0.3.0/src/flywheel/globals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import functools
 from collections import defaultdict
+from contextlib import contextmanager
 from contextvars import ContextVar, copy_context
 from typing import Any, Callable, Generator, Tuple
 
 from .context import CollectContext, InstanceContext
 from .typing import P, R, TEntity
 
 GLOBAL_COLLECT_CONTEXT = CollectContext()
@@ -51,7 +52,17 @@
 
 def global_collect(entity: TEntity) -> TEntity:
     return GLOBAL_COLLECT_CONTEXT.collect(entity)
 
 
 def local_collect(entity: TEntity) -> TEntity:
     return COLLECTING_CONTEXT_VAR.get().collect(entity)
+
+
+@contextmanager
+def union_scope(*contexts: CollectContext):
+    token = LOOKUP_LAYOUT_VAR.set((*contexts, *LOOKUP_LAYOUT_VAR.get()))
+
+    try:
+        yield
+    finally:
+        LOOKUP_LAYOUT_VAR.reset(token)
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/instance_of.py` & `elaina_flywheel-0.3.0/src/flywheel/instance_of.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,17 @@
 class InstanceOf(Generic[T]):
     target: type[T]
 
     def __init__(self, target: type[T]) -> None:
         self.target = target
 
     @overload
-    def __get__(self, instance: None, owner: type) -> Self:
-        ...
+    def __get__(self, instance: None, owner: type) -> Self: ...
 
     @overload
-    def __get__(self, instance: Any, owner: type) -> T:
-        ...
+    def __get__(self, instance: Any, owner: type) -> T: ...
 
     def __get__(self, instance: Any, owner: type):
         if instance is None:
             return self
 
         return INSTANCE_CONTEXT_VAR.get().instances[self.target]
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/overloads.py` & `elaina_flywheel-0.3.0/src/flywheel/overloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         return {}
 
     def access(self, scope: dict, signature: TypeOverloadSignature) -> dict[Callable, None] | None:
         if signature.type in scope:
             return scope[signature.type]
 
 
-class _SingletonOverloadSignature:
-    ...
+class _SingletonOverloadSignature: ...
 
 
 SINGLETON_SIGN = _SingletonOverloadSignature()
 
 
 class SingletonOverload(FnOverload[_SingletonOverloadSignature, None, None]):
     SIGNATURE = SINGLETON_SIGN
```

### Comparing `elaina_flywheel-0.2.0/src/flywheel/scoped.py` & `elaina_flywheel-0.3.0/src/flywheel/scoped.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 import functools
 from typing import Any, Callable
+from typing_extensions import Self
 
 from .context import CollectContext
 from .globals import COLLECTING_CONTEXT_VAR, GLOBAL_COLLECT_CONTEXT, GLOBAL_INSTANCE_CONTEXT, INSTANCE_CONTEXT_VAR
-from .typing import TYPE_CHECKING, AssignKeeperCls, P, R, TEntity
+from .typing import TYPE_CHECKING, P, R, TEntity
 
 if TYPE_CHECKING:
     from typing_extensions import Concatenate
 
-    from .fn.base import Call, Fn
-    from .fn.implement import FnImplementEntity, OverloadRecorder
+    from .fn.endpoint import FnCollectEndpoint
+    from .fn.implement import FnImplementEntity
     from .fn.record import FnImplement, FnRecord
-    from .typing import CR, OutP
 
 
 class scoped_collect(CollectContext):
-    fn_implements: dict[FnImplement, FnRecord]
+    fn_implements: dict[FnImplement, dict[FnCollectEndpoint, FnRecord]]
     _tocollect_list: dict[FnImplementEntity, None]
     finalize_cbs: list[Callable[[scoped_collect], Any]]
     cls: type | None = None
 
     def __init__(self) -> None:
         self.fn_implements = {}
         self.finalize_cbs = []
@@ -30,15 +30,15 @@
     @classmethod
     def globals(cls):
         instance = cls()
         instance.fn_implements = GLOBAL_COLLECT_CONTEXT.fn_implements
         return instance
 
     @classmethod
-    def env(cls):
+    def locals(cls):
         instance = cls()
         instance.fn_implements = COLLECTING_CONTEXT_VAR.get().fn_implements
         return instance
 
     def finalize(self):
         for cb in self.finalize_cbs:
             cb(self)
@@ -52,25 +52,29 @@
 
     def remove_collected_callback(self, func: Callable[[scoped_collect], Any]):
         self.finalize_cbs.remove(func)
         return func
 
     @property
     def target(self):
-        from .fn.implement import FnImplementEntity
+        # from .fn.implement import FnImplementEntity
 
         class LocalEndpoint:
             collector = self
 
+            @classmethod
+            def build_static(cls) -> Self:
+                return cls()
+
             def __init_subclass__(cls, *, static: bool = False) -> None:
                 self.cls = cls
                 self.finalize()
 
                 if static:
-                    GLOBAL_INSTANCE_CONTEXT.instances[cls] = cls()
+                    GLOBAL_INSTANCE_CONTEXT.instances[cls] = cls.build_static()
 
             @staticmethod
             def collect(entity: TEntity) -> TEntity:  # type: ignore
                 return entity.collect(self)
 
             @staticmethod
             def ensure_self(func: Callable[Concatenate[Any, P], R]) -> Callable[P, R]:
@@ -79,27 +83,8 @@
                     assert self.cls is not None
 
                     instance = INSTANCE_CONTEXT_VAR.get().instances[self.cls]
                     return func(instance, *args, **kwargs)
 
                 return wrapper
 
-            @staticmethod
-            def impl(
-                fn: Fn[Callable[Concatenate[OverloadRecorder[CR], OutP], Any], Any], *args: OutP.args, **kwargs: OutP.kwargs
-            ) -> AssignKeeperCls[Call[..., CR]]:
-                def inner(impl: Callable[Concatenate[Any, P], R] | FnImplementEntity[Callable[P, R]]):
-                    if not isinstance(impl, FnImplementEntity):
-                        if not hasattr(impl, "__wrapped__"):
-                            impl_call = LocalEndpoint.ensure_self(impl)
-                        else:
-                            impl_call: Callable[P, R] = impl  # type: ignore
-
-                        impl = FnImplementEntity(impl_call)
-
-                    impl.add_target(fn, *args, **kwargs)
-                    self._tocollect_list[impl] = None
-                    return impl
-
-                return inner  # type: ignore
-
         return LocalEndpoint
```

### Comparing `elaina_flywheel-0.2.0/PKG-INFO` & `elaina_flywheel-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 Metadata-Version: 2.1
 Name: elaina-flywheel
-Version: 0.2.0
+Version: 0.3.0
 Author-Email: Elaina <GreyElaina@outlook.com>
 License: MIT
 Requires-Python: >=3.9
 Requires-Dist: typing-extensions>=4.10.0
 Description-Content-Type: text/markdown
 
 # Ryanvk Flywheel
 
-Ryanvk Flywheel 是一个 Ryanvk-style 的 utility，其提供强大的 `Fn`、`FnOverload`，实现了在单一入口点上的几近*完美*的自由重载。  
-...而更为可贵的是，Flywheel 具有*前沿级*的类型支持。
+Ryanvk Flywheel 是一个 Ryanvk-style 的 utility。
 
-这个库是专门为 Avilla 轻量化定制的，你可以在[这里](https://github.com/GraiaProject/Avilla/tree/master/avilla/core/flywheel) 找到与本仓库相同的内容，相比标准版的 Ryanvk，其体量仅为其一半不到。  
-本仓库中的内容预计不会在 PyPI 上发布单独的 `flywheel` 包，请自行使用 VcsRequirement 方式导入你的项目。
+- 在单一入口点上的*几近完美*的自由重载；
+- 简单灵活的重载机制；
+- *前沿级*的类型支持[^1]；
+- 可切换上下文。
+
+Available on PyPI: `elaina-flywheel`。
+
+[^1]: 仅在 Pyright / Basedpyright 上可用。
 
 ## 使用
 
 Flywheel 着重于围绕 `Fn` 建设，以提供强大的重载功能为目的。
 
 可以通过这种方法创建一个使用*简单重载*(`SimpleOverload`)的 `Fn`。
 
 ```python
 from typing import Protocol
 
-from flywheel import Fn, FnCompose, OverloadRecorder, FnRecord, SimpleOverload
+from flywheel import Fn, FnCompose, FnRecord, SimpleOverload, FnCollectEndpoint
 
-@Fn.declare
+@Fn
 class greet(FnCompose):
     name = SimpleOverload("name")
 
-    def call(self, record: FnRecord, name: str) -> str:
-        entities = self.load(self.name.dig(record, name))
-        # entities 会自动读取到 collect 中对于 implement 参数的类型。
+    def call(self, records, name: str) -> str:
+        # 我们不关心 records 的类型。
+        # 如果你在乎，它的类型是 dict[FnCollectEndpoint, FnImplementEntity]
 
+        entities = self.someone(records).use(self.name, name)
         return entities.first(name)
-    
-    # 定义 Fn 面向的具体实现的类型...
-    class ShapeCall(Protocol):
-        def __call__(self, name: str) -> str:
-            ...
-
-    # ...并在 collect 方法中引用，这是可选的，仅影响 load 方法的返回类型。
-    def collect(self, recorder: OverloadRecorder[ShapeCall], *, name: str):
-        recorder.use(self.name, name)
+
+    @FnCollectEndpoint
+    @classmethod
+    def someone(cls, *, name: str):
+        yield cls.name.hold(name)
+
+        # 可选的，你可以给出实现的类型，运行时中我们不关心这个，所以你可以放在 if TYPE_CHECKING 中。
+        def shape(name: str) -> str: ...
+        return shape
 ```
 
 然后我们为 `greet` 提出两个实现：
 
 - 当 `name` 是 `Teague` 的时候返回 `"Stargaztor, but in name only."`；
 - 当 `name` 是 `Grey` 的时候返回 `"Symbol, the Founder."`：
 
 当提出实现后，我们还得将其收集起来，这样 Flywheel 的内部系统才能调用的到这些实现。
 在这里，我们使用 `global_collect` 函数，将实现收集到全局上下文中。
 
 ```python
 from flywheel import global_collect
 
 @global_collect
-@greet.impl(name="Teague")
+@greet._.someone(name="Teague")
 def greet_teague(name: str) -> str:
     return "Stargaztor, but in name only."
 
 @global_collect
-@greet.impl(name="Grey")
+@greet._.someone(name="Grey")
 def greet_grey(name: str) -> str:
     return "Symbol, the Founder."
 ```
 
 然后我们调用。
 
 ```python
@@ -85,19 +91,21 @@
 ```
 
 显然，我们并没有面向 `"Hizuki"` 实现一个 `greet`。为了使我们的程序能处理这种情况，我们可以这样修改 `greet` 的声明：
 
 ```python
 @Fn.declare
 class greet(FnCompose):
-    name = SimpleOverload("name")
+    name = SimpleOverload("name")  # 指定 name 是必要的。
 
-    def call(self, record: FnRecord, name: str) -> str:
-        entities = self.load(self.name.dig(record, name))
-        # entities 会自动读取到 collect 中对于 implement 参数的类型。
+    def call(self, records, name: str) -> str:
+        # 我们不关心 records 的类型。
+        # 如果你在乎，它的类型是 dict[FnCollectEndpoint, FnImplementEntity]
+
+        entities = self.someone(records).use(self.name, name)
 
         if not entities:  # 判断是否存在符合条件的实现
             return f"Ordinary, {name}."
 
         return entities.first(name)
 ```
 
@@ -160,14 +168,25 @@
             return scope[signature.value]
 ```
 
 你可以尝试借由这个例子来实现一个依据调用时值 (`call_value`) 的类型来找到对应的实现的 `TypeOverload`，作为参考答案，你可以在 `flywheel.overloads` 模块中找到同名的实现。
 
 对于 `FnOverload` 来说，他不一定要搜索尽可能多的实现 —— 这根据实际情况来决定：如果你希望你的 Fn 表现的像是个事件系统，这种情况下你最好找到尽可能多的实现 —— 不幸的，我们没有提供什么 `greed` 参数，因此你需要自己实现。
 
+你可以添加构造器参数，并继承现有的其他重载实现。
+
+```python
+class SomeMaybeGreedOverload(FnOverload):
+    def __init__(self, name: str, greed: bool):
+        self.name = name
+        self.greed = greed
+
+    ...  # 你的实际逻辑
+```
+
 ## 上下文
 
 Flywheel 提供了一个 `global_collect` 函数，用于将实现收集到全局上下文中。自然，上下文不会只有一个，Flywheel 允许你创建自己的上下文，并在你期望的时候应用。
 
 相应的，全局上下文存储在 `flywheel.globals.GLOBAL_COLLECT_CONTEXT`，如果你知道你在做什么有所必要的事情，这一信息可能对你有用。但我想大多数情况下你都不会使用到这一技巧。
 
 ```python
@@ -189,20 +208,20 @@
 
 需要注意的是，`global_collect` 函数的行为并不会因为上下文的存在而改变，为此，你需要考虑使用 `local_collect` 来将实现收集到你的上下文中。
 
 ```python
 from flywheel import local_collect
 
 @local_collect
-@greet.impl(name="Teague")
+@greet._.someone(name="Teague")
 def greet_teague(name: str) -> str:
     return "Stargaztor, but in name only."
 
 @local_collect
-@greet.impl(name="Grey")
+@greet._.someone(name="Grey")
 def greet_grey(name: str) -> str:
     return "Symbol, the Founder."
 ```
 
 如果你在这之前并没有使用过 `collect_scope`，`local_collect` 会采用默认行为，将实现收集到全局上下文中。
 
 但我们不建议在所有情况下都使用 `local_collect`，而是尽可能的使用 `global_collect`，
@@ -213,73 +232,58 @@
 如果你希望你的模块保持命名空间的整洁，采用 `scoped_collect` 或许是不错的主意。只是他还有其他更重要的应用，且听我娓娓道来。
 
 ```python
 from flywheel import scoped_collect
 
 class greet_implements(m := scoped_collect.globals().target, static=True):
     @m.collect
-    @greet.impl(name="Teague")
+    @greet._.someone(name="Teague")
     @m.ensure_self
     def greet_teague(self, name: str) -> str:
         return "Stargaztor, but in name only."
 
-    # 上面的写法未免过于冗长，可以考虑使用这种写法，基本等效。
-
-    @m.impl(greet, name="Grey")
-    def greet_grey(self, name: str) -> str:
-        return "Symbol, the Founder."
+    # 上面的写法未免过于冗长，我们正在考虑更好的办法。
 ```
 
 这段代码使用 `scoped_collect` 实现了和我们最初给出的两个 `greet_xxx` 一样的效果。
 
 ```python
 >>> greet("Teague")
 'Stargaztor, but in name only.'
 >>> greet("Grey")
 'Symbol, the Founder.'
 ```
 
-这段代码使用 `scoped_collect.globals()` 方法连接到了全局上下文。如果你不想这样，需要换成 `scoped_collect.env()`。
+这段代码使用 `scoped_collect.globals()` 方法连接到了全局上下文。如果你不想这样，需要换成 `scoped_collect.locals()`。
 
 ```python
 from flywheel import scoped_collect
 
-class greet_implements(m := scoped_collect.env().target, static=True):
+class greet_implements(m := scoped_collect.locals().target, static=True):
     ...
 ```
 
 `static=True` 时，`greet_implements` 会被实例化并保存到全局中的*实例上下文* (Instance Context) 中。  
 如果你自定义了你的构造方法 (即 `__init__` 或 `__new__`)，则会在启动时报错，此时你需要自己实现对 `InstanceContext` 的生成与应用。
 
 ## 叠加
 
 Flywheel 允许你这么做...：
 
 ```python
 @global_collect
-@greet.impl(name="Teague")
-@greet.impl(name="Grey")
+@greet._.someone(name="Teague")
+@greet._.someone(name="Grey")
 def greet_stargaztor(name: str) -> str:
     return f"Stargaztor"
 ```
 
-他等同于分别调用 `Fn.impl` 方法，但写的更简短，同时你依旧能获得 Flywheel 前沿级的类型支持。
+他等同于分别调用 `FnCollectEntity`，但写的更简短，同时你依旧能获得 Flywheel 前沿级的类型支持。
 
-当你配合 `scoped_collect` 使用时，可以直接使用 `m.impl` 方法，其将自动处理 `m.collect` 与 `m.ensure_self`。
-
-```python
-# 不需要手动调用 `m.collect` 与 `m.ensure_self`。
-
-@m.impl(greet, name="Teague")
-@m.impl(greet, name="Grey")
-def greet_stargaztor(self, name: str) -> str:
-    return "Stargaztor"
-```
-
-如果执意想要使用原始的方式，请注意将 `Fn.impl` 调用*夹*在 `m.collect` 与 `m.ensure_self` 中间：
+如果需配合 `scoped_collect` 使用，注意将 `Fn.impl` 调用*夹*在 `m.collect` 与 `m.ensure_self` 中间：
 
 ```python
 @m.collect
 @greet.impl(name="Teague")
 @greet.impl(name="Grey")
 @m.ensure_self
 def greet_teague(self, name: str) -> str:
@@ -331,15 +335,15 @@
 我们提供了可以自动访问当前实例上下文的描述符 `InstanceOf`，通过这一措施，你可以方便的访问实例上下文中的内容。
 
 ```python
 from flywheel import InstanceOf
 
 from aiohttp import ClientSession
 
-class sth_implements(m := scoped_collect.env().target, static=True):
+class sth_implements(m := scoped_collect.locals().target, static=True):
     session = InstanceOf(ClientSession)
 
     @m.impl(...)
     async def something(self, num: int):
         await self.session.get(f"http://example.com/", params={"num": num})
 
 # -----
@@ -348,14 +352,35 @@
     instance_cx.instances[ClientSession] = self.aiohttp_session
 
     await fn(10)
 ```
 
 从该示例中你也可以了解到 Flywheel 对异步的支持，理论上也能一并支持生成器，异步生成器甚至 `contextlib.contextmanager`，但如果出了问题，欢迎汇报至 issues.
 
+### 重写 static 实例化行为
+
+通过重写类方法 (classmethod) `build_static`，你可以自定义 `static` 参数的实例化行为。
+
+```python
+class sth_implements(m := scoped_collect.locals().target, static=True):
+    session = InstanceOf(ClientSession)
+
+    def __init__(self, session: ClientSession):
+        self.session = session
+
+    @m.impl(...)
+    async def something(self, num: int):
+        await self.session.get(f"http://example.com/", params={"num": num})
+
+    @classmethod
+    def build_static(cls):
+        return cls(GLOBAL_AIOHTTP_SESSION)
+```
+
+
 ### 全局上下文
 
 Flywheel 同样提供了全局的实例上下文。
 
 ```python
 from flywheel.globals import GLOBAL_INSTANCE_CONTEXT
```

