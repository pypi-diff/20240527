# Comparing `tmp/anydi-0.25.2.tar.gz` & `tmp/anydi-0.26.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.25.2.tar", max compression
+gzip compressed data, was "anydi-0.26.0a0.tar", max compression
```

## Comparing `anydi-0.25.2.tar` & `anydi-0.26.0a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.25.2/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.25.2/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.25.2/anydi/__init__.py
--rw-r--r--   0        0        0    27996 2024-05-09 08:20:34.172615 anydi-0.25.2/anydi/_container.py
--rw-r--r--   0        0        0    10215 2024-05-08 12:47:28.300076 anydi-0.25.2/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.25.2/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.25.2/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.25.2/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.25.2/anydi/_types.py
--rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.25.2/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.25.2/anydi/ext/__init__.py
--rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.25.2/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.25.2/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.25.2/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.25.2/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.25.2/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.25.2/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.25.2/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.25.2/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.25.2/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.25.2/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     4043 2024-05-20 11:14:22.992471 anydi-0.25.2/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.25.2/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.25.2/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.25.2/anydi/py.typed
--rw-r--r--   0        0        0     3107 2024-05-20 11:14:36.707323 anydi-0.25.2/pyproject.toml
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 anydi-0.25.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.26.0a0/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.26.0a0/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.26.0a0/anydi/__init__.py
+-rw-r--r--   0        0        0    29168 2024-05-27 09:31:21.256185 anydi-0.26.0a0/anydi/_container.py
+-rw-r--r--   0        0        0    10815 2024-05-27 09:28:37.965546 anydi-0.26.0a0/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.26.0a0/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.26.0a0/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.26.0a0/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.26.0a0/anydi/_types.py
+-rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.26.0a0/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.26.0a0/anydi/ext/__init__.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.26.0a0/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.26.0a0/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.26.0a0/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.26.0a0/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.26.0a0/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.26.0a0/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.26.0a0/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.26.0a0/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.26.0a0/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.26.0a0/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     4043 2024-05-20 11:14:22.992471 anydi-0.26.0a0/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.26.0a0/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.26.0a0/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.26.0a0/anydi/py.typed
+-rw-r--r--   0        0        0     3109 2024-05-27 10:07:03.964236 anydi-0.26.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 anydi-0.26.0a0/PKG-INFO
```

### Comparing `anydi-0.25.2/LICENSE` & `anydi-0.26.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/README.md` & `anydi-0.26.0a0/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/__init__.py` & `anydi-0.26.0a0/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/_container.py` & `anydi-0.26.0a0/anydi/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import contextlib
 import inspect
 import types
 import uuid
+from collections import defaultdict
 from contextvars import ContextVar
 from functools import wraps
 from typing import (
     Any,
     AsyncContextManager,
     AsyncIterator,
     Awaitable,
@@ -20,15 +21,15 @@
     Mapping,
     Sequence,
     TypeVar,
     cast,
     overload,
 )
 
-from typing_extensions import ParamSpec, final, get_args, get_origin
+from typing_extensions import ParamSpec, Self, final, get_args, get_origin
 
 try:
     from types import NoneType
 except ImportError:
     NoneType = type(None)  # type: ignore[misc]
 
 
@@ -81,14 +82,15 @@
 
         Args:
             providers: Optional mapping of providers to register during initialization.
             modules: Optional sequence of modules to register during initialization.
             strict: Whether to enable strict mode. Defaults to False.
         """
         self._providers: dict[type[Any], Provider] = {}
+        self._providers_cache: dict[Scope, list[type[Any]]] = defaultdict(list)
         self._singleton_context = SingletonContext(self)
         self._transient_context = TransientContext(self)
         self._request_context_var: ContextVar[RequestContext | None] = ContextVar(
             "request_context", default=None
         )
         self._override_instances: dict[type[Any], Any] = {}
         self._strict = strict
@@ -166,32 +168,32 @@
               as the interface.
             - The provider will be validated for its scope, type, and matching scopes.
         """
         provider = Provider(obj=obj, scope=scope)
 
         # Create Event type
         if provider.is_resource and (interface is NoneType or interface is None):
-            interface = type(f"Event{uuid.uuid4().hex}", (), {})
+            interface = type(f"Event_{uuid.uuid4().hex}", (), {})
 
         if interface in self._providers:
             if override:
-                self._providers[interface] = provider
+                self._set_provider(interface, provider)
                 return provider
 
             raise LookupError(
                 f"The provider interface `{get_full_qualname(interface)}` "
                 "already registered."
             )
 
         # Validate provider
         self._validate_provider_scope(provider)
         self._validate_provider_type(provider)
         self._validate_provider_match_scopes(interface, provider)
 
-        self._providers[interface] = provider
+        self._set_provider(interface, provider)
         return provider
 
     def unregister(self, interface: AnyInterface) -> None:
         """Unregister a provider by interface.
 
         Args:
             interface: The interface of the provider to unregister.
@@ -271,14 +273,25 @@
                 scope = getattr(interface, "__scope__", None)
                 # Try to detect scope
                 if scope is None:
                     scope = self._detect_scope(interface)
                 return self.register(interface, interface, scope=scope or "transient")
             raise
 
+    def _set_provider(self, interface: AnyInterface, provider: Provider) -> None:
+        """Set a provider by interface.
+
+        Args:
+            interface: The interface for which to set the provider.
+            provider: The provider object to set.
+        """
+        self._providers[interface] = provider
+        if provider.is_resource:
+            self._providers_cache[provider.scope].append(interface)
+
     def _validate_provider_scope(self, provider: Provider) -> None:
         """Validate the scope of a provider.
 
         Args:
             provider: The provider to validate.
 
         Raises:
@@ -394,19 +407,31 @@
         """Register a module as a callable, module type, or module instance.
 
         Args:
             module: The module to register.
         """
         self._modules.register(module)
 
+    def __enter__(self) -> Self:
+        """Enter the singleton context."""
+        self.start()
+        return self
+
+    def __exit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: types.TracebackType | None,
+    ) -> None:
+        """Exit the singleton context."""
+        self.close()
+
     def start(self) -> None:
         """Start the singleton context."""
-        for interface, provider in self._providers.items():
-            if provider.scope == "singleton":
-                self.resolve(interface)  # noqa
+        self._singleton_context.start()
 
     def close(self) -> None:
         """Close the singleton context."""
         self._singleton_context.close()
 
     def request_context(self) -> ContextManager[None]:
         """Obtain a context manager for the request-scoped context.
@@ -424,14 +449,28 @@
         """
         context = RequestContext(self)
         token = self._request_context_var.set(context)
         with context:
             yield
             self._request_context_var.reset(token)
 
+    async def __aenter__(self) -> Self:
+        """Enter the singleton context."""
+        await self.astart()
+        return self
+
+    async def __aexit__(
+        self,
+        exc_type: type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: types.TracebackType | None,
+    ) -> None:
+        """Exit the singleton context."""
+        await self.aclose()
+
     async def astart(self) -> None:
         """Start the singleton context asynchronously."""
         for interface, provider in self._providers.items():
             if provider.scope == "singleton":
                 await self.aresolve(interface)  # noqa
 
     async def aclose(self) -> None:
```

### Comparing `anydi-0.25.2/anydi/_context.py` & `anydi-0.26.0a0/anydi/_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from __future__ import annotations
 
 import abc
 import contextlib
 from types import TracebackType
-from typing import TYPE_CHECKING, Any, TypeVar, cast
+from typing import TYPE_CHECKING, Any, ClassVar, TypeVar, cast
 
 from typing_extensions import Self, final
 
-from ._types import AnyInterface, Interface, Provider
+from ._types import AnyInterface, Interface, Provider, Scope
 from ._utils import run_async
 
 if TYPE_CHECKING:
     from ._container import Container
 
 T = TypeVar("T")
 
 
 class ScopedContext(abc.ABC):
     """ScopedContext base class."""
 
+    scope: ClassVar[Scope]
+
     def __init__(self, container: Container) -> None:
         self.container = container
 
     @abc.abstractmethod
     def get(self, interface: Interface[T], provider: Provider) -> T:
         """Get an instance of a dependency from the scoped context.
 
@@ -229,14 +231,15 @@
 
     def __enter__(self) -> Self:
         """Enter the context.
 
         Returns:
             The scoped context.
         """
+        self.start()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
@@ -247,24 +250,30 @@
             exc_type: The type of the exception, if any.
             exc_val: The exception instance, if any.
             exc_tb: The traceback, if any.
         """
         self.close()
         return
 
+    def start(self) -> None:
+        """Start the scoped context."""
+        for interface in self.container._providers_cache.get(self.scope, []):  # noqa
+            self.container.resolve(interface)
+
     def close(self) -> None:
         """Close the scoped context."""
         self._stack.close()
 
     async def __aenter__(self) -> Self:
         """Enter the context asynchronously.
 
         Returns:
             The scoped context.
         """
+        await self.astart()
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
@@ -275,34 +284,45 @@
             exc_type: The type of the exception, if any.
             exc_val: The exception instance, if any.
             exc_tb: The traceback, if any.
         """
         await self.aclose()
         return
 
+    async def astart(self) -> None:
+        """Start the scoped context asynchronously."""
+        for interface in self.container._providers_cache.get(self.scope, []):  # noqa
+            await self.container.aresolve(interface)
+
     async def aclose(self) -> None:
         """Close the scoped context asynchronously."""
         await run_async(self._stack.close)
         await self._async_stack.aclose()
 
 
 @final
 class SingletonContext(ResourceScopedContext):
     """A scoped context representing the "singleton" scope."""
 
+    scope = "singleton"
+
 
 @final
 class RequestContext(ResourceScopedContext):
     """A scoped context representing the "request" scope."""
 
+    scope = "request"
+
 
 @final
 class TransientContext(ScopedContext):
     """A scoped context representing the "transient" scope."""
 
+    scope = "transient"
+
     def get(self, interface: Interface[T], provider: Provider) -> T:
         """Get an instance of a dependency from the transient context.
 
         Args:
             interface: The interface of the dependency.
             provider: The provider for the instance.
```

### Comparing `anydi-0.25.2/anydi/_module.py` & `anydi-0.26.0a0/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/_scanner.py` & `anydi-0.26.0a0/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/_types.py` & `anydi-0.26.0a0/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/_utils.py` & `anydi-0.26.0a0/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/_settings.py` & `anydi-0.26.0a0/anydi/ext/django/_settings.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/_utils.py` & `anydi-0.26.0a0/anydi/ext/django/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/apps.py` & `anydi-0.26.0a0/anydi/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/middleware.py` & `anydi-0.26.0a0/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/ninja/__init__.py` & `anydi-0.26.0a0/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/ninja/_operation.py` & `anydi-0.26.0a0/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/django/ninja/_signature.py` & `anydi-0.26.0a0/anydi/ext/django/ninja/_signature.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/fastapi.py` & `anydi-0.26.0a0/anydi/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/pytest_plugin.py` & `anydi-0.26.0a0/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/anydi/ext/starlette/middleware.py` & `anydi-0.26.0a0/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.25.2/pyproject.toml` & `anydi-0.26.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.25.2"
+version = "0.26.0a0"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
```

### Comparing `anydi-0.25.2/PKG-INFO` & `anydi-0.26.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.25.2
+Version: 0.26.0a0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```

