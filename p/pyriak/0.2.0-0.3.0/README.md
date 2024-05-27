# Comparing `tmp/pyriak-0.2.0.tar.gz` & `tmp/pyriak-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriak-0.2.0.tar", max compression
+gzip compressed data, was "pyriak-0.3.0.tar", max compression
```

## Comparing `pyriak-0.2.0.tar` & `pyriak-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1083 2024-05-04 21:26:50.483291 pyriak-0.2.0/LICENSE
--rw-r--r--   0        0        0      948 2024-05-17 03:34:47.669779 pyriak-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4002 2024-05-17 01:56:40.828708 pyriak-0.2.0/README.md
--rw-r--r--   0        0        0     4476 2024-05-17 01:03:05.389730 pyriak-0.2.0/src/pyriak/__init__.py
--rw-r--r--   0        0        0     3364 2024-05-15 05:27:35.698514 pyriak-0.2.0/src/pyriak/_importer.py
--rw-r--r--   0        0        0     5265 2024-05-17 01:36:17.343647 pyriak-0.2.0/src/pyriak/entity.py
--rw-r--r--   0        0        0     4565 2024-05-17 01:11:40.294812 pyriak-0.2.0/src/pyriak/eventkey.py
--rw-r--r--   0        0        0     4691 2024-05-17 03:18:22.514876 pyriak-0.2.0/src/pyriak/events.py
--rw-r--r--   0        0        0      188 2024-05-04 21:26:50.490288 pyriak-0.2.0/src/pyriak/managers/__init__.py
--rw-r--r--   0        0        0    10388 2024-05-15 05:27:35.702513 pyriak-0.2.0/src/pyriak/managers/entitymanager.py
--rw-r--r--   0        0        0     4002 2024-05-17 01:36:29.474375 pyriak-0.2.0/src/pyriak/managers/statemanager.py
--rw-r--r--   0        0        0    18739 2024-05-17 01:41:58.456283 pyriak-0.2.0/src/pyriak/managers/systemmanager.py
--rw-r--r--   0        0        0        0 2024-05-15 05:27:35.705512 pyriak-0.2.0/src/pyriak/py.typed
--rw-r--r--   0        0        0     6473 2024-05-17 03:15:01.879124 pyriak-0.2.0/src/pyriak/query.py
--rw-r--r--   0        0        0     3260 2024-05-17 03:07:55.524384 pyriak-0.2.0/src/pyriak/space.py
--rw-r--r--   0        0        0     6048 2024-05-17 03:05:14.375655 pyriak-0.2.0/src/pyriak/system.py
--rw-r--r--   0        0        0     4543 1970-01-01 00:00:00.000000 pyriak-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-27 02:18:05.764877 pyriak-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4136 2024-05-27 02:18:05.764877 pyriak-0.3.0/README.md
+-rw-r--r--   0        0        0      983 2024-05-27 02:18:05.764877 pyriak-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4207 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/__init__.py
+-rw-r--r--   0        0        0     5099 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/entity.py
+-rw-r--r--   0        0        0     4383 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/eventkey.py
+-rw-r--r--   0        0        0     4516 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/events.py
+-rw-r--r--   0        0        0      183 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/managers/__init__.py
+-rw-r--r--   0        0        0     9688 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/managers/entitymanager.py
+-rw-r--r--   0        0        0     3862 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/managers/statemanager.py
+-rw-r--r--   0        0        0    19781 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/managers/systemmanager.py
+-rw-r--r--   0        0        0        0 2024-05-27 02:18:05.764877 pyriak-0.3.0/src/pyriak/py.typed
+-rw-r--r--   0        0        0     6061 2024-05-27 02:18:05.768877 pyriak-0.3.0/src/pyriak/query.py
+-rw-r--r--   0        0        0     2780 2024-05-27 02:18:05.768877 pyriak-0.3.0/src/pyriak/space.py
+-rw-r--r--   0        0        0     2814 2024-05-27 02:18:05.768877 pyriak-0.3.0/src/pyriak/system.py
+-rw-r--r--   0        0        0     4790 1970-01-01 00:00:00.000000 pyriak-0.3.0/PKG-INFO
```

### Comparing `pyriak-0.2.0/LICENSE` & `pyriak-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 aatle
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 aatle
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pyriak-0.2.0/README.md` & `pyriak-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,116 @@
-# pyriak
-A lightweight implementation of Entity Component System architecture for Python.
-
-(Originally created August 2, 2022.)
-
-
-## Concepts
-
-
-
-## Usage
-
-
-
-### Entity creation
-Any entity must first be created and populated with components.
-
-A system can directly create and populate an entity.
-This system may decide itself to create an entity, or handle an event that
-directly tells it to create one.
-```py
-player = space.entities.create(
-  components.Player(),
-  components.CameraFocus(),
-  components.Sprite(),
-)
-```
-A listening system can extend a created entity.
-```py
-@bind(ComponentAdded, 200, RocketBooster):
-def add_rocket_exhaust(space, event):
-  event.entity.add(ParticleEmitter(rocket_particles))
-```
-
-Often, multiple systems will need to create a certain set of components that are not
-related enough to put under a single component, but common enough to necessitate code reuse.
-A dedicated module can provide functions that
-produce a "batch", a set of components, sometimes with parameters for customization.
-```py
-# batches.py
-def spaceship(radius=20):
-  body = components.Body(radius)
-  body.collision_type = 'spaceship'
-  return body, components.Engine(), components.Sprite(spaceship_sprite)
-...
-```
-```py
-# systems/player.py
-import batches
-...
-player = space.entities.create(
-  *batches.spaceship(),
-  components.CameraFocus(),
-  components.PlayerController()
-)
-enemy = space.entities.create(
-  *batches.spaceship(),
-  components.AIController()
-)
-```
-It is also easy to customize or initialize the components after the entity and batch have been created
-as opposed to passing in customization parameters to the batch function.
-
-Small, individual components may be created directly by systems.
-Batch functions should only be made when necessary, for when it is likely to be reused:
-repeated at least twice, lots of boilerplate.
-Batch functions should not be made for a large, unique set of components for a specific entity.
-It is preferable to have smaller batches to allow for more control in choosing which components to use.
-
-A batch function that calls another batch function mimics inheritance, which can lead to
-avoidable problems.
-Batches should be considered large components, not a standalone pseudo-class.
-(However, a batch function that *only* calls other batch functions is fine because it
-does not create any components itself, so its use is not directly required by anything.)
-
-Also note that the components should represent one, indivisible thing.
-Components can be created large and then later broken down into a batch of multiple components.
- 
-
-## TO DO:
-- dynamic handlers?
-- 3.11 typing features
-- fix multibinding typing
-- system "new" method instantiation
-- `__future__.annotations`
-- type aliases
-- 'direct', 'indirect', 'strict', 'immediate' vocab docs
-- validate subclasses: hash, mro
-- sys mgr expose handlers + bind predicate/filter + _Binding public
-- `__contains__` TypeError raise?
-- picklable `__setstate__ __getstate__ __copy__` classes
-- 'processor' game pump generator yield event method, 'event loop'
-- discard method
-- keys method (for dict protocol)
-- improve error messages
-- raise from None bad
-- views, items methods: mappingproxy
-- `__eq__`, remove `__hash__`: mgrs
-- types(*types) method functionality all mgrs+entity ?
-- entities from ids: itertools helpers in entitymgr
-- 'add', 'remove' methods return value
-- entity mgr garbage collection behavior (currently undefined?)
-- game `__call__` use ?
-- more container (set) dunder methods, operations
-- copy methods
-- more positional only arguments
-- more system config
-- str and repr methods all
-- place documentation in code, along with all rules (style guide first)
-- optimization through profiling, scalene (in a game)
-- make imported module variables private (consistency)
-- python version lower in poetry dependencies ? find min python version
-- review and rewrite readme.txt
+# pyriak
+A lightweight implementation of Entity Component System architecture for Python.
+
+(Originally created August 2, 2022.)
+
+
+## Concepts
+Object oriented programming is used for many projects.
+In larger, more complex projects, it can have some shortcomings.
+The inheritance hierarchies can become messy and inflexible,
+forcing the base classes to grow in size when code reuse is needed.
+
+
+## Usage
+
+
+
+### Entity creation
+Any entity must first be created and populated with components.
+
+A system can directly create and populate an entity.
+This system may decide itself to create an entity, or handle an event that
+directly tells it to create one.
+```py
+player = space.entities.create(
+  components.Player(),
+  components.CameraFocus(),
+  components.Sprite(),
+)
+```
+A listening system can extend a created entity.
+```py
+@bind(ComponentAdded, 200, RocketBooster)
+def add_rocket_exhaust(space, event):
+  event.entity.add(ParticleEmitter(rocket_particles))
+```
+
+Often, multiple systems will need to create a certain set of components that are not
+related enough to put under a single component, but common enough to necessitate code reuse.
+A dedicated module can provide functions that
+produce a "batch", a set of components, sometimes with parameters for customization.
+```py
+# batches.py
+def spaceship(radius=20):
+  body = components.Body(radius)
+  body.collision_type = 'spaceship'
+  return body, components.Engine(), components.Sprite(spaceship_sprite)
+...
+```
+```py
+# systems/player.py
+import batches
+...
+player = space.entities.create(
+  *batches.spaceship(),
+  components.CameraFocus(),
+  components.PlayerController()
+)
+enemy = space.entities.create(
+  *batches.spaceship(),
+  components.AIController()
+)
+```
+It is also easy to customize or initialize the components after the entity and batch have been created
+as opposed to passing in customization parameters to the batch function.
+
+Small, individual components may be created directly by systems.
+Batch functions should only be made when necessary, for when it is likely to be reused:
+repeated at least twice, lots of boilerplate.
+Batch functions should not be made for a large, unique set of components for a specific entity.
+It is preferable to have smaller batches to allow for more control in choosing which components to use.
+
+A batch function that calls another batch function mimics inheritance, which can lead to
+avoidable problems.
+Batches should be considered large components, not a standalone pseudo-class.
+(However, a batch function that *only* calls other batch functions is fine because it
+does not create any components itself, so its use is not directly required by anything.)
+
+Also note that the components should represent one, indivisible thing.
+Components can be created large and then later broken down into a batch of multiple components.
+ 
+
+## TO DO:
+- dynamic handlers?
+- 3.11 typing features
+- fix multibinding typing
+- system "new" method instantiation
+- `__future__.annotations`
+- type aliases
+- 'direct', 'indirect', 'strict', 'immediate' vocab docs
+- validate subclasses: hash, mro
+- sys mgr expose handlers + bind predicate/filter + _Binding public
+- `__contains__` TypeError raise?
+- picklable `__setstate__ __getstate__ __copy__` classes
+- 'processor' game pump generator yield event method, 'event loop'
+- discard method
+- keys method (for dict protocol)
+- improve error messages
+- raise from None bad
+- views, items methods: mappingproxy
+- `__eq__`, remove `__hash__`: mgrs
+- types(*types) method functionality all mgrs+entity ?
+- entities from ids: itertools helpers in entitymgr
+- 'add', 'remove' methods return value
+- entity mgr garbage collection behavior (currently undefined?)
+- game `__call__` use ?
+- more container (set) dunder methods, operations
+- copy methods
+- more positional only arguments
+- more system config
+- str and repr methods all
+- place documentation in code, along with all rules (style guide first)
+- optimization through profiling, scalene (in a game)
+- make imported module variables private (consistency)
+- python version lower in poetry dependencies ? find min python version
+- review and rewrite readme.txt
```

### Comparing `pyriak-0.2.0/src/pyriak/entity.py` & `pyriak-0.3.0/src/pyriak/entity.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-__all__ = ['Entity']
-
-from collections.abc import Iterable
-from typing import TYPE_CHECKING, NewType, TypeVar, overload
-from uuid import uuid4
-
-from pyriak import _SENTINEL, dead_weakref, strict_subclasses, subclasses
-from pyriak.events import ComponentAdded, ComponentRemoved
-
-
-if TYPE_CHECKING:
-  from weakref import ref as weakref
-
-  from pyriak.managers import EntityManager
-
-
-EntityId = NewType('EntityId', int)
-
-
-_T = TypeVar('_T')
-_D = TypeVar('_D')
-
-
-class Entity:
-  __slots__ = 'id', '_components', '_manager', '__weakref__'
-
-  def __init__(self, components: Iterable[object] = (), /):
-    self.id: EntityId = self.new_id()
-    self._manager: weakref[EntityManager] = dead_weakref
-    comp_dict: dict[type, object] = {}
-    for comp in components:
-      comp_type = type(comp)
-      if comp_type in comp_dict and (
-          (other := comp_dict[comp_type]) is comp or other == comp):
-        continue
-      comp_dict[comp_type] = comp
-    self._components: dict[type, object] = comp_dict
-
-  def add(self, *components: object) -> None:
-    self_components = self._components
-    events: list[ComponentAdded | ComponentRemoved] = []
-    append_event = events.append
-    for component in components:
-      component_type = type(component)
-      if component_type in self_components:
-        other_component = self_components[component_type]
-        if other_component is component or other_component == component:
-          continue
-        append_event(ComponentRemoved(self, other_component))
-      self_components[component_type] = component
-      append_event(ComponentAdded(self, component))
-    manager = self._manager()
-    if manager is not None:
-      manager._components_added(self.id, components, events)
-
-  def remove(self, *components: object) -> None:
-    self_components = self._components
-    manager = self._manager()
-    for i, component in enumerate(components):
-      component_type = type(component)
-      try:
-        other_component = self_components[component_type]
-      except KeyError:
-        pass
-      else:
-        if other_component is component or other_component == component:
-          del self_components[component_type]
-          continue
-      if manager is not None:
-        manager._components_removed(self, components[:i])
-      raise ValueError(component)
-    if manager is not None:
-      manager._components_removed(self, components)
-
-  def __call__(self, *component_types: type[_T]) -> list[_T]:
-    components = self._components
-    return [
-      components[component_type]  # type: ignore
-      for component_type in {
-        comp_type: None for cls in component_types for comp_type in subclasses(cls)
-      }  # dict instead of set to guarantee stable ordering while still removing dupes
-      if component_type in components
-    ]
-
-  def __getitem__(self, component_type: type[_T], /) -> _T:
-    try:
-      return self._components[component_type]  # type: ignore[return-value]
-    except KeyError:
-      components = self._components
-      for cls in strict_subclasses(component_type):
-        if cls in components:
-          return components[cls]  # type: ignore[return-value]
-      raise
-
-  def __setitem__(self, component_type: type[_T], component: _T, /):
-    self.pop(component_type, None)
-    self.add(component)
-
-  def __delitem__(self, component_type: type, /):
-    self.remove(self[component_type])
-
-  @overload
-  def get(self, component_type: type[_T], /) -> _T | None: ...
-  @overload
-  def get(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
-  def get(self, component_type, default=None, /):
-    try:
-      return self._components[component_type]
-    except KeyError:
-      pass
-    components = self._components
-    for cls in strict_subclasses(component_type):
-      if cls in components:
-        return components[cls]
-    return default
-
-  @overload
-  def pop(self, component_type: type[_T], /) -> _T: ...
-  @overload
-  def pop(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
-  def pop(self, component_type, default=_SENTINEL, /):
-    try:
-      component = self[component_type]
-    except KeyError:
-      if default is _SENTINEL:
-        raise
-      return default
-    self.remove(component)
-    return component
-
-  def types(self):
-    return self._components.keys()
-
-  def __iter__(self):
-    return iter(self._components.values())
-
-  def __reversed__(self):
-    return reversed(self._components.values())
-
-  def __len__(self):
-    return len(self._components)
-
-  def __contains__(self, obj: object, /):
-    if obj in self._components:
-      return True
-    if isinstance(obj, type):
-      components = self._components
-      for cls in strict_subclasses(obj):
-        if cls in components:
-          return True
-    return False
-
-  def __eq__(self, other: object, /):
-    if self is other:
-      return True
-    if isinstance(other, Entity):
-      return self._components == other._components
-    return NotImplemented
-
-  def clear(self):
-    """Remove all components from self."""
-    self.remove(*self)
-
-  @staticmethod
-  def new_id() -> EntityId:
-    return uuid4().int  # type: ignore
+__all__ = ['Entity']
+
+from collections.abc import Iterable
+from typing import TYPE_CHECKING, NewType, TypeVar, overload
+from uuid import uuid4
+
+from pyriak import _SENTINEL, dead_weakref, strict_subclasses, subclasses
+from pyriak.events import ComponentAdded, ComponentRemoved
+
+
+if TYPE_CHECKING:
+  from weakref import ref as weakref
+
+  from pyriak.managers import EntityManager
+
+
+EntityId = NewType('EntityId', int)
+
+
+_T = TypeVar('_T')
+_D = TypeVar('_D')
+
+
+class Entity:
+  __slots__ = 'id', '_components', '_manager', '__weakref__'
+
+  def __init__(self, components: Iterable[object] = (), /):
+    self.id: EntityId = self.new_id()
+    self._manager: weakref[EntityManager] = dead_weakref
+    comp_dict: dict[type, object] = {}
+    for comp in components:
+      comp_type = type(comp)
+      if comp_type in comp_dict and (
+          (other := comp_dict[comp_type]) is comp or other == comp):
+        continue
+      comp_dict[comp_type] = comp
+    self._components: dict[type, object] = comp_dict
+
+  def add(self, *components: object) -> None:
+    self_components = self._components
+    events: list[ComponentAdded | ComponentRemoved] = []
+    append_event = events.append
+    for component in components:
+      component_type = type(component)
+      if component_type in self_components:
+        other_component = self_components[component_type]
+        if other_component is component or other_component == component:
+          continue
+        append_event(ComponentRemoved(self, other_component))
+      self_components[component_type] = component
+      append_event(ComponentAdded(self, component))
+    manager = self._manager()
+    if manager is not None:
+      manager._components_added(self.id, components, events)
+
+  def remove(self, *components: object) -> None:
+    self_components = self._components
+    manager = self._manager()
+    for i, component in enumerate(components):
+      component_type = type(component)
+      try:
+        other_component = self_components[component_type]
+      except KeyError:
+        pass
+      else:
+        if other_component is component or other_component == component:
+          del self_components[component_type]
+          continue
+      if manager is not None:
+        manager._components_removed(self, components[:i])
+      raise ValueError(component)
+    if manager is not None:
+      manager._components_removed(self, components)
+
+  def __call__(self, *component_types: type[_T]) -> list[_T]:
+    components = self._components
+    return [
+      components[component_type]  # type: ignore
+      for component_type in {
+        comp_type: None for cls in component_types for comp_type in subclasses(cls)
+      }  # dict instead of set to guarantee stable ordering while still removing dupes
+      if component_type in components
+    ]
+
+  def __getitem__(self, component_type: type[_T], /) -> _T:
+    try:
+      return self._components[component_type]  # type: ignore[return-value]
+    except KeyError:
+      components = self._components
+      for cls in strict_subclasses(component_type):
+        if cls in components:
+          return components[cls]  # type: ignore[return-value]
+      raise
+
+  def __setitem__(self, component_type: type[_T], component: _T, /):
+    self.pop(component_type, None)
+    self.add(component)
+
+  def __delitem__(self, component_type: type, /):
+    self.remove(self[component_type])
+
+  @overload
+  def get(self, component_type: type[_T], /) -> _T | None: ...
+  @overload
+  def get(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
+  def get(self, component_type, default=None, /):
+    try:
+      return self._components[component_type]
+    except KeyError:
+      pass
+    components = self._components
+    for cls in strict_subclasses(component_type):
+      if cls in components:
+        return components[cls]
+    return default
+
+  @overload
+  def pop(self, component_type: type[_T], /) -> _T: ...
+  @overload
+  def pop(self, component_type: type[_T], default: _D, /) -> _T | _D: ...
+  def pop(self, component_type, default=_SENTINEL, /):
+    try:
+      component = self[component_type]
+    except KeyError:
+      if default is _SENTINEL:
+        raise
+      return default
+    self.remove(component)
+    return component
+
+  def types(self):
+    return self._components.keys()
+
+  def __iter__(self):
+    return iter(self._components.values())
+
+  def __reversed__(self):
+    return reversed(self._components.values())
+
+  def __len__(self):
+    return len(self._components)
+
+  def __contains__(self, obj: object, /):
+    if obj in self._components:
+      return True
+    if isinstance(obj, type):
+      components = self._components
+      for cls in strict_subclasses(obj):
+        if cls in components:
+          return True
+    return False
+
+  def __eq__(self, other: object, /):
+    if self is other:
+      return True
+    if isinstance(other, Entity):
+      return self._components == other._components
+    return NotImplemented
+
+  def clear(self):
+    """Remove all components from self."""
+    self.remove(*self)
+
+  @staticmethod
+  def new_id() -> EntityId:
+    return uuid4().int  # type: ignore
```

### Comparing `pyriak-0.2.0/src/pyriak/eventkey.py` & `pyriak-0.3.0/src/pyriak/eventkey.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,147 +1,145 @@
-__all__ = ['key_functions', 'set_key', 'KeyFunction']
-
-from collections.abc import Callable, Hashable, Iterator, Mapping
-from typing import Any, TypeAlias, TypeVar, overload
-from weakref import WeakKeyDictionary
-
-from pyriak import _SENTINEL
-
-
-_T = TypeVar('_T')
-_D = TypeVar('_D')
-
-del TypeVar
-
-
-# if it is iterator (especially generator), it is multiple
-# hashable keys, else it is the key itself (must be hashable)
-KeyFunction: TypeAlias = Callable[[_T], Hashable | Iterator[Hashable]]
-
-
-class EventKeyFunctions:
-  """A weakkey dict of event types to key functions or None."""
-
-  __slots__ = ('_data',)
-
-  def __init__(
-    self, dict: Mapping[type, KeyFunction[Any] | None] | None = None
-  ):
-    self._data: WeakKeyDictionary[type, KeyFunction[Any] | None]
-    self._data = WeakKeyDictionary()
-    if dict is not None:
-      self.update(dict)
-
-  @overload
-  def __call__(self, event_type: type[_T]) -> KeyFunction[_T]: ...
-  @overload
-  def __call__(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
-  def __call__(self, event_type, default=_SENTINEL):
-    """Return the key function for event_type.
-
-    A key function is used to extract a key from an event of type event_type.
-
-    Each type in the event_type's method resolution order (__mro__) is checked until
-    a specific key function is found and is not None,
-    in which case the key function is returned.
-    If no key function is found that is not None, default is returned if it is provided,
-    otherwise a KeyError is raised.
-    This is the only method that considers superclasses, other than the exists method.
-    """
-    get = self._data.get
-    for cls in event_type.__mro__:
-      key_function = get(cls)
-      if key_function is not None:
-        return key_function
-    if default is _SENTINEL:
-      raise KeyError(event_type)
-    return default
-
-  def exists(self, event_type: type) -> bool:
-    """Return True if there is a key function for event_type that is not None."""
-    return self(event_type, None) is not None
-
-  def __getitem__(self, event_type: type[_T]) -> KeyFunction[_T] | None:
-    """Return the specific key function for an event_type, ignoring superclasses."""
-    return self._data[event_type]
-
-  def __setitem__(self, event_type: type[_T], key: KeyFunction[_T] | None):
-    data = self._data
-    if event_type in data:
-      raise KeyError(f'cannot reassign event type key: {event_type!r}')
-    data[event_type] = key
-
-  @overload
-  def get(self, event_type: type[_T]) -> KeyFunction[_T] | None: ...
-  @overload
-  def get(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
-  def get(self, event_type, default=None):
-    try:
-      return self._data[event_type]
-    except KeyError:
-      return default
-
-  def setdefault(
-    self, event_type: type[_T], default: KeyFunction[_T] | None = None
-  ) -> KeyFunction[_T] | None:
-    data = self._data
-    if event_type in data:
-      return data[event_type]
-    self[event_type] = default
-    return default
-
-  def update(self, other: Mapping[type, KeyFunction[Any] | None]) -> None:
-    for event_type, key in dict(other).items():
-      self[event_type] = key
-
-  def keys(self):
-    return self._data.keys()
-
-  def values(self):
-    return self._data.values()
-
-  def items(self):
-    return self._data.items()
-
-  def __len__(self):
-    return len(self._data)
-
-  def __contains__(self, event_type: type):
-    return event_type in self._data
-
-  def __iter__(self):
-    return iter(self._data)
-
-  def __or__(self, other: Mapping[type, KeyFunction[Any] | None]):
-    return self._data | other
-
-  def __ror__(self, other: Mapping[type, KeyFunction[Any] | None]):
-    return other | self._data
-
-  def __ior__(self, other: Mapping[type, KeyFunction[Any] | None]):
-    self.update(other)
-    return self
-
-  __copy__ = None  # type: ignore
-
-  def copy(self):
-    return self._data.copy()
-
-  def keyrefs(self):
-    return self._data.keyrefs()
-
-
-key_functions = EventKeyFunctions()
-key_functions[object] = None
-
-
-def set_key(key: KeyFunction[_T] | None, /) -> Callable[[type[_T]], type[_T]]:
-  """Assign a key function (permanently) to an event type.
-
-  Convenience decorator to assign a key function (or None) to an event class definition.
-
-  The operator module has useful functions for creating key functions, e.g. attrgetter.
-  """
-  def decorator(cls: type[_T]) -> type[_T]:
-    key_functions[cls] = key
-    return cls
-  return decorator
+__all__ = ['key_functions', 'set_key', 'KeyFunction']
+
+from collections.abc import Callable, Hashable, Iterator, Mapping
+from typing import Any, TypeAlias, TypeVar, overload
+from weakref import WeakKeyDictionary
+
+from pyriak import _SENTINEL
+
+
+_T = TypeVar('_T')
+_D = TypeVar('_D')
+
+del TypeVar
+
+
+# if it is iterator (especially generator), it is multiple
+# hashable keys, else it is the key itself (must be hashable)
+KeyFunction: TypeAlias = Callable[[_T], Hashable | Iterator[Hashable]]
+
+
+class EventKeyFunctions:
+  """A weakkey dict of event types to key functions or None."""
+
+  __slots__ = ('_data',)
+
+  def __init__(
+    self, dict: Mapping[type, KeyFunction[Any] | None] | None = None
+  ):
+    self._data: WeakKeyDictionary[type, KeyFunction[Any] | None]
+    self._data = WeakKeyDictionary()
+    if dict is not None:
+      self.update(dict)
+
+  @overload
+  def __call__(self, event_type: type[_T]) -> KeyFunction[_T]: ...
+  @overload
+  def __call__(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
+  def __call__(self, event_type, default=_SENTINEL):
+    """Return the key function for event_type.
+
+    A key function is used to extract a key from an event of type event_type.
+
+    Each type in the event_type's method resolution order (__mro__) is checked until
+    a specific key function is found and is not None,
+    in which case the key function is returned.
+    If no key function is found that is not None, default is returned if it is provided,
+    otherwise a KeyError is raised.
+    This is the only method that considers superclasses, other than the exists method.
+    """
+    get = self._data.get
+    for cls in event_type.__mro__:
+      key_function = get(cls)
+      if key_function is not None:
+        return key_function
+    if default is _SENTINEL:
+      raise KeyError(event_type)
+    return default
+
+  def exists(self, event_type: type) -> bool:
+    """Return True if there is a key function for event_type that is not None."""
+    return self(event_type, None) is not None
+
+  def __getitem__(self, event_type: type[_T]) -> KeyFunction[_T] | None:
+    """Return the specific key function for an event_type, ignoring superclasses."""
+    return self._data[event_type]
+
+  def __setitem__(self, event_type: type[_T], key: KeyFunction[_T] | None):
+    data = self._data
+    if event_type in data:
+      raise KeyError(f'cannot reassign event type key: {event_type!r}')
+    data[event_type] = key
+
+  @overload
+  def get(self, event_type: type[_T]) -> KeyFunction[_T] | None: ...
+  @overload
+  def get(self, event_type: type[_T], default: _D) -> KeyFunction[_T] | _D: ...
+  def get(self, event_type, default=None):
+    try:
+      return self._data[event_type]
+    except KeyError:
+      return default
+
+  def setdefault(
+    self, event_type: type[_T], default: KeyFunction[_T] | None = None
+  ) -> KeyFunction[_T] | None:
+    data = self._data
+    if event_type in data:
+      return data[event_type]
+    self[event_type] = default
+    return default
+
+  def update(self, other: Mapping[type, KeyFunction[Any] | None]) -> None:
+    for event_type, key in dict(other).items():
+      self[event_type] = key
+
+  def keys(self):
+    return self._data.keys()
+
+  def values(self):
+    return self._data.values()
+
+  def items(self):
+    return self._data.items()
+
+  def __len__(self):
+    return len(self._data)
+
+  def __contains__(self, event_type: type):
+    return event_type in self._data
+
+  def __iter__(self):
+    return iter(self._data)
+
+  def __or__(self, other: Mapping[type, KeyFunction[Any] | None]):
+    return self._data | other
+
+  def __ror__(self, other: Mapping[type, KeyFunction[Any] | None]):
+    return other | self._data
+
+  def __ior__(self, other: Mapping[type, KeyFunction[Any] | None]):
+    self.update(other)
+    return self
+
+  def copy(self):
+    return self._data.copy()
+
+  def keyrefs(self):
+    return self._data.keyrefs()
+
+
+key_functions = EventKeyFunctions()
+key_functions[object] = None
+
+
+def set_key(key: KeyFunction[_T] | None, /) -> Callable[[type[_T]], type[_T]]:
+  """Assign a key function (permanently) to an event type.
+
+  Convenience decorator to assign a key function (or None) to an event class definition.
+
+  The operator module has useful functions for creating key functions, e.g. attrgetter.
+  """
+  def decorator(cls: type[_T]) -> type[_T]:
+    key_functions[cls] = key
+    return cls
+  return decorator
```

### Comparing `pyriak-0.2.0/src/pyriak/events.py` & `pyriak-0.3.0/src/pyriak/events.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-__all__ = [
-  'SpaceCallback',
-  'SendEvent',
-  'ComponentAdded',
-  'ComponentRemoved',
-  'EntityAdded',
-  'EntityRemoved',
-  'SystemAdded',
-  'SystemRemoved',
-  'EventHandlerAdded',
-  'EventHandlerRemoved',
-  'StateAdded',
-  'StateRemoved',
-]
-
-from collections.abc import Callable, Hashable, Iterator
-from typing import TYPE_CHECKING, Any, Generic, TypeVar
-
-from pyriak import subclasses as _subclasses
-from pyriak.eventkey import set_key as _set_key
-
-
-if TYPE_CHECKING:
-  from pyriak.entity import Entity
-  from pyriak.managers.systemmanager import _EventHandler
-  from pyriak.space import Space
-  from pyriak.system import System, _Callback
-
-
-_T = TypeVar('_T')
-
-
-class SpaceCallback(Generic[_T]):
-  """A SystemManager automatically calls a SpaceCallback Event when it processes one."""
-
-  # TODO: python 3.11 - callback: Callable[['Space', *_Ts], _T]
-
-  def __init__(self, callback: Callable [..., _T], /, *args: Any, **kwargs: Any):
-    self.callback = callback
-    self.args = list(args)
-    self.kwargs = kwargs
-
-  def __call__(self, space: 'Space', /) -> _T:
-    """Execute self's callback with self's args and kwargs."""
-    return self.callback(space, *self.args, **self.kwargs)
-
-
-class SendEvent:
-  """A special built-in Event type for sending Events to specific System(s).
-
-  A SendEvent is basically a wrapper of another Event.
-  When a SendEvent is triggered by a SystemManager, only the SendEvent's receivers
-  receive the wrapped Event, if they can.
-
-  If a receiver can't receive the Event, it is skipped.
-  This can happen if:
-  - the system is not in the system manager
-  - the system does not have a callback bind to that event type
-  Triggering may be slow if the wrapped Event has a lot of binds in the SystemManager.
-
-  The order in which the bound callbacks of the receivers are invoked
-  is no different from normal Event triggering,
-  where higher priority callbacks are called first.
-
-  The actual SendEvent instance itself is never processed.
-  """
-
-  def __init__(self, event: object, *receivers: 'System'):
-    self.event = event
-    self.receivers = set(receivers)
-
-
-def _component_type_key(event: 'ComponentAdded | ComponentRemoved') -> Iterator[type]:
-  yield from type(event.component).__mro__
-
-@_set_key(_component_type_key)
-class ComponentAdded:
-  def __init__(self, entity: 'Entity', component: object):
-    self.entity = entity
-    self.component = component
-
-@_set_key(_component_type_key)
-class ComponentRemoved:
-  def __init__(self, entity: 'Entity', component: object):
-    self.entity = entity
-    self.component = component
-
-
-class EntityAdded:
-  def __init__(self, entity: 'Entity'):
-    self.entity = entity
-
-class EntityRemoved:
-  def __init__(self, entity: 'Entity'):
-    self.entity = entity
-
-
-def _system_key(event: 'SystemAdded | SystemRemoved') -> 'System':
-  return event.system
-
-@_set_key(_system_key)
-class SystemAdded:
-  def __init__(self, system: 'System'):
-    self.system = system
-
-@_set_key(_system_key)
-class SystemRemoved:
-  def __init__(self, system: 'System'):
-    self.system = system
-
-
-def _handler_key(event: 'EventHandlerAdded | EventHandlerRemoved') -> Iterator[type]:
-  yield from _subclasses(event.event_type)
-
-@_set_key(_handler_key)
-class EventHandlerAdded:
-  def __init__(
-    self, _handler: '_EventHandler', _event_type: type, _keys: frozenset[Hashable]
-  ):
-    self._handler = _handler
-    self.event_type = _event_type
-    self.keys = _keys
-
-  @property
-  def system(self):
-    return self._handler.system
-
-  @property
-  def callback(self):
-    return self._handler.callback
-
-  @property
-  def name(self):
-    return self._handler.name
-
-  @property
-  def priority(self):
-    return self._handler.priority
-
-  @property
-  def key(self):
-    [key] = self.keys
-    return key
-
-@_set_key(_handler_key)
-class EventHandlerRemoved:
-  def __init__(
-    self, _system: 'System', _callback: '_Callback', _name: str, _priority: Any,
-    _event_type: type, _keys: frozenset[Hashable]
-  ):
-    self.system = _system
-    self.callback = _callback
-    self.name = _name
-    self.priority = _priority
-    self.event_type = _event_type
-    self.keys = _keys
-
-  @property
-  def key(self):
-    [key] = self.keys
-    return key
-
-
-def _state_type_key(event: 'StateAdded | StateRemoved') -> Iterator[type]:
-  yield from type(event.state).__mro__
-
-@_set_key(_state_type_key)
-class StateAdded:
-  def __init__(self, state: object):
-    self.state = state
-
-@_set_key(_state_type_key)
-class StateRemoved:
-  def __init__(self, state: object):
-    self.state = state
+__all__ = [
+  'SpaceCallback',
+  'SendEvent',
+  'ComponentAdded',
+  'ComponentRemoved',
+  'EntityAdded',
+  'EntityRemoved',
+  'SystemAdded',
+  'SystemRemoved',
+  'EventHandlerAdded',
+  'EventHandlerRemoved',
+  'StateAdded',
+  'StateRemoved',
+]
+
+from collections.abc import Callable, Hashable, Iterator
+from typing import TYPE_CHECKING, Any, Generic, TypeVar
+
+from pyriak import subclasses as _subclasses
+from pyriak.eventkey import set_key as _set_key
+
+
+if TYPE_CHECKING:
+  from pyriak.entity import Entity
+  from pyriak.managers.systemmanager import _EventHandler
+  from pyriak.space import Space
+  from pyriak.system import System, _Callback
+
+
+_T = TypeVar('_T')
+
+
+class SpaceCallback(Generic[_T]):
+  """A SystemManager automatically calls a SpaceCallback Event when it processes one."""
+
+  # TODO: python 3.11 - callback: Callable[['Space', *_Ts], _T]
+
+  def __init__(self, callback: Callable [..., _T], /, *args: Any, **kwargs: Any):
+    self.callback = callback
+    self.args = list(args)
+    self.kwargs = kwargs
+
+  def __call__(self, space: 'Space', /) -> _T:
+    """Execute self's callback with self's args and kwargs."""
+    return self.callback(space, *self.args, **self.kwargs)
+
+
+class SendEvent:
+  """A special built-in Event type for sending Events to specific System(s).
+
+  A SendEvent is basically a wrapper of another Event.
+  When a SendEvent is triggered by a SystemManager, only the SendEvent's receivers
+  receive the wrapped Event, if they can.
+
+  If a receiver can't receive the Event, it is skipped.
+  This can happen if:
+  - the system is not in the system manager
+  - the system does not have a callback bind to that event type
+  Triggering may be slow if the wrapped Event has a lot of binds in the SystemManager.
+
+  The order in which the bound callbacks of the receivers are invoked
+  is no different from normal Event triggering,
+  where higher priority callbacks are called first.
+
+  The actual SendEvent instance itself is never processed.
+  """
+
+  def __init__(self, event: object, *receivers: 'System'):
+    self.event = event
+    self.receivers = set(receivers)
+
+
+def _component_type_key(event: 'ComponentAdded | ComponentRemoved') -> Iterator[type]:
+  yield from type(event.component).__mro__
+
+@_set_key(_component_type_key)
+class ComponentAdded:
+  def __init__(self, entity: 'Entity', component: object):
+    self.entity = entity
+    self.component = component
+
+@_set_key(_component_type_key)
+class ComponentRemoved:
+  def __init__(self, entity: 'Entity', component: object):
+    self.entity = entity
+    self.component = component
+
+
+class EntityAdded:
+  def __init__(self, entity: 'Entity'):
+    self.entity = entity
+
+class EntityRemoved:
+  def __init__(self, entity: 'Entity'):
+    self.entity = entity
+
+
+def _system_key(event: 'SystemAdded | SystemRemoved') -> 'System':
+  return event.system
+
+@_set_key(_system_key)
+class SystemAdded:
+  def __init__(self, system: 'System'):
+    self.system = system
+
+@_set_key(_system_key)
+class SystemRemoved:
+  def __init__(self, system: 'System'):
+    self.system = system
+
+
+def _handler_key(event: 'EventHandlerAdded | EventHandlerRemoved') -> Iterator[type]:
+  yield from _subclasses(event.event_type)
+
+@_set_key(_handler_key)
+class EventHandlerAdded:
+  def __init__(
+    self, _handler: '_EventHandler', _event_type: type, _keys: frozenset[Hashable]
+  ):
+    self._handler = _handler
+    self.event_type = _event_type
+    self.keys = _keys
+
+  @property
+  def system(self):
+    return self._handler.system
+
+  @property
+  def callback(self):
+    return self._handler.callback
+
+  @property
+  def name(self):
+    return self._handler.name
+
+  @property
+  def priority(self):
+    return self._handler.priority
+
+  @property
+  def key(self):
+    [key] = self.keys
+    return key
+
+@_set_key(_handler_key)
+class EventHandlerRemoved:
+  def __init__(
+    self, _system: 'System', _callback: '_Callback', _name: str, _priority: Any,
+    _event_type: type, _keys: frozenset[Hashable]
+  ):
+    self.system = _system
+    self.callback = _callback
+    self.name = _name
+    self.priority = _priority
+    self.event_type = _event_type
+    self.keys = _keys
+
+  @property
+  def key(self):
+    [key] = self.keys
+    return key
+
+
+def _state_type_key(event: 'StateAdded | StateRemoved') -> Iterator[type]:
+  yield from type(event.state).__mro__
+
+@_set_key(_state_type_key)
+class StateAdded:
+  def __init__(self, state: object):
+    self.state = state
+
+@_set_key(_state_type_key)
+class StateRemoved:
+  def __init__(self, state: object):
+    self.state = state
```

### Comparing `pyriak-0.2.0/src/pyriak/managers/entitymanager.py` & `pyriak-0.3.0/src/pyriak/managers/entitymanager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,319 +1,301 @@
-__all__ = ['EntityManager']
-
-from collections.abc import Iterable, Iterator, KeysView
-from typing import Callable, NoReturn, TypeVar, overload
-from weakref import ref as weakref
-
-from pyriak import _SENTINEL, EventQueue, dead_weakref, subclasses
-from pyriak.entity import Entity, EntityId
-from pyriak.events import ComponentAdded, ComponentRemoved, EntityAdded, EntityRemoved
-from pyriak.query import (
-  ComponentQueryResult,
-  EntityQueryResult,
-  IdQueryResult,
-  Query,
-  QueryResult,
-)
-
-
-_T = TypeVar('_T')
-_Q = TypeVar('_Q', bound=QueryResult)
-
-
-class _Components:
-  """The components attribute of an EntityManager instance, exposes more functionality.
-
-  If the EntityManager has been garbage collected, all methods
-  raise TypeError.
-  """
-
-  __slots__ = ('_manager',)
-
-  _manager: Callable[[], 'EntityManager']
-
-  def __call__(self, component_type: type[_T], /) -> Iterator[_T]:
-    manager = self._manager()
-    entities = manager._entities
-    return (
-      component
-      for entity_id in manager._component_types.get(component_type, ())
-      for component in entities[entity_id](component_type)
-    )
-
-  def __getitem__(self, component_type: type[_T], /) -> Iterator[_T]:
-    manager = self._manager()
-    entities = manager._entities
-    return (entities[entity_id][component_type]
-            for entity_id in manager._component_types.get(component_type, ()))
-
-  def types(self) -> KeysView[type]:
-    return self._manager()._component_types.keys()
-
-  def __iter__(self) -> Iterator[object]:
-    for entity in self._manager():
-      yield from entity
-
-  def __reversed__(self) -> Iterator[object]:
-    for entity in reversed(self._manager()):
-      yield from reversed(entity)
-
-  def __len__(self):
-    return sum(len(entity) for entity in self._manager()._entities.values())
-
-  def __contains__(self, obj: object, /):
-    types = self._manager()._component_types
-    if isinstance(obj, type):
-      for cls in subclasses(obj):
-        if cls in types:
-          return True
-    return False
-
-
-class EntityManager:
-  __slots__ = '_entities', '_component_types', 'components', 'event_queue', '__weakref__'
-
-  def __init__(
-    self, entities: Iterable[Entity] = (), /, event_queue: EventQueue | None = None
-  ):
-    self.event_queue = event_queue
-    self.components = _Components()
-    self.components._manager = weakref(self)  # type: ignore
-    self._entities: dict[EntityId, Entity] = {}
-    self._component_types: dict[type, set[EntityId]] = {}
-    self.add(*entities)
-
-  def add(self, *entities: Entity) -> None:
-    component_types = self._component_types
-    self_entities = self._entities
-    self_weakref: weakref[EntityManager] = weakref(self)
-    event_queue = self.event_queue
-    for entity in entities:
-      entity_id = entity.id
-      if entity_id in self_entities:
-        continue
-      if entity._manager() is not None:
-        raise RuntimeError(f'{entity!r} already added to another manager')
-      self_entities[entity_id] = entity
-      entity._manager = self_weakref
-      for component_type in {
-        component_type for cls in entity.types() for component_type in cls.__mro__
-      }:
-        try:
-          component_types[component_type].add(entity_id)
-        except KeyError:
-          component_types[component_type] = {entity_id}
-      if event_queue is not None:
-        event_queue.extend([
-          EntityAdded(entity),
-          *[ComponentAdded(entity, component) for component in entity]
-        ])
-
-  def create(self, *components: object) -> Entity:
-    """Create an Entity with the given components, add it to self, and return it.
-
-    The returned Entity can, of course, be directly modified.
-    """
-    entity: Entity = Entity(components)
-    self.add(entity)
-    return entity
-
-  def remove(self, *entities: Entity) -> None:
-    component_types = self._component_types
-    event_queue = self.event_queue
-    for entity in entities:
-      entity_id = entity.id
-      try:
-        del self._entities[entity_id]
-      except KeyError:
-        raise ValueError(entity) from None
-      entity._manager = dead_weakref
-      for component_type in {
-        component_type for cls in entity.types() for component_type in cls.__mro__
-      }:
-        component_type_entities = component_types[component_type]
-        component_type_entities.remove(entity_id)
-        if not component_type_entities:
-          del component_types[component_type]
-      if event_queue is not None:
-        event_queue.extend([
-          EntityRemoved(entity),
-          *[ComponentRemoved(entity, component) for component in entity]
-        ])
-
-  def __getitem__(self, entity_id: EntityId, /) -> Entity:
-    return self._entities[entity_id]
-
-  def __delitem__(self, entity_id: EntityId, /):
-    self.remove(self._entities[entity_id])
-
-  @overload
-  def get(self, entity_id: EntityId, /) -> Entity | None: ...
-  @overload
-  def get(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
-  def get(self, entity_id, default=None, /):
-    return self._entities.get(entity_id, default)
-
-  @overload
-  def pop(self, entity_id: EntityId, /) -> Entity: ...
-  @overload
-  def pop(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
-  def pop(self, entity_id, default=_SENTINEL, /):
-    try:
-      entity = self._entities[entity_id]
-    except KeyError:
-      if default is _SENTINEL:
-        raise
-      return default
-    self.remove(entity)
-    return entity
-
-  @overload
-  def query(self, query: Query, /) -> ComponentQueryResult: ...
-  @overload
-  def query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> ComponentQueryResult: ...
-  def query(self, /, *types, merge=None):
-    """"""
-    return self._query(ComponentQueryResult, types, merge)
-
-  @overload
-  def entity_query(self, query: Query, /) -> EntityQueryResult: ...
-  @overload
-  def entity_query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def entity_query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> EntityQueryResult: ...
-  def entity_query(self, /, *types, merge=None):
-    """"""
-    return self._query(EntityQueryResult, types, merge)
-
-  @overload
-  def id_query(self, query: Query, /) -> IdQueryResult: ...
-  @overload
-  def id_query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def id_query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> IdQueryResult: ...
-  def id_query(self, /, *types, merge=None):
-    """"""
-    return self._query(IdQueryResult, types, merge)
-
-  def _query(self, result_cls: type[_Q], types, merge=None, /) -> _Q:
-    """"""
-    if len(types) == 1 and isinstance((query := types[0]), Query):
-      if merge is not None:
-        raise TypeError('unexpected keyword argument: merge')
-      types = query.types
-      merge = query.merge
-    elif merge is None:
-      merge = set.intersection
-    if not types:
-      raise ValueError('expected at least one type in component types')
-    self_entities = self._entities
-    self_component_types = self._component_types
-    return result_cls(
-      {
-        id: self_entities[id]
-        for id in merge(*[
-          self_component_types[typ]  # noqa: SIM401
-          if typ in self_component_types else set()
-          for typ in types
-        ])
-      },
-      types,
-      merge
-    )
-
-  def __call__(self, component_type: type, /) -> Iterator[Entity]:
-    """Return a generator of all entities in self that contain component_type."""
-    entities = self._entities
-    return (
-      entities[entity_id] for entity_id in self._component_types.get(component_type, ())
-    )
-
-  @overload
-  def ids(self, /) -> KeysView[EntityId]: ...
-  @overload
-  def ids(self, component_type: type, /) -> set[EntityId]: ...
-  def ids(self, component_type=None, /):
-    """Return a set of all entity ids that contain the given component type.
-
-    If no component type is given, then
-    return a set-like view of all entity ids in self instead.
-    """
-    if component_type is None:
-      return self._entities.keys()
-    component_types = self._component_types
-    if component_type not in component_types:
-      return set()
-    return set(component_types[component_type])
-
-  def __iter__(self):
-    """Return an iterator of all Entities in self.
-
-    The least recently added Entities are first.
-    """
-    return iter(self._entities.values())
-
-  def __reversed__(self):
-    return reversed(self._entities.values())
-
-  def __len__(self):
-    return len(self._entities)
-
-  def __contains__(self, obj: object, /):
-    if isinstance(obj, Entity):
-      return obj.id in self._entities
-    return obj in self._entities
-
-  def clear(self):
-    self.remove(*self)
-
-  def _components_added(
-    self, entity_id: EntityId, components: Iterable[object], events: Iterable[object], /
-  ) -> None:
-    component_types = self._component_types
-    for component_type in {
-      component_type
-      for component in components
-      for component_type in type(component).__mro__
-    }:
-      try:
-        component_types[component_type].add(entity_id)
-      except KeyError:
-        component_types[component_type] = {entity_id}
-    if (queue := self.event_queue) is not None:
-      queue.extend(events)
-
-  def _components_removed(self, entity: Entity, components: Iterable[object], /) -> None:
-    component_types = self._component_types
-    entity_id = entity.id
-    for component_type in {
-      component_type
-      for component in components
-      for component_type in type(component).__mro__
-      if component_type not in entity
-    }:
-      entity_ids = component_types[component_type]
-      entity_ids.remove(entity_id)
-      if not entity_ids:
-        del component_types[component_type]
-    if (queue := self.event_queue) is not None:
-      queue.extend([ComponentRemoved(entity, component) for component in components])
+__all__ = ['EntityManager']
+
+from collections.abc import Iterable, Iterator, KeysView
+from typing import Callable, TypeVar, overload
+from weakref import ref as weakref
+
+from pyriak import _SENTINEL, EventQueue, dead_weakref, subclasses
+from pyriak.entity import Entity, EntityId
+from pyriak.events import ComponentAdded, ComponentRemoved, EntityAdded, EntityRemoved
+from pyriak.query import (
+  ComponentQueryResult,
+  EntityQueryResult,
+  IdQueryResult,
+  Query,
+  QueryResult,
+)
+
+
+_T = TypeVar('_T')
+_Q = TypeVar('_Q', bound=QueryResult)
+
+
+class _Components:
+  """The components attribute of an EntityManager instance, exposes more functionality.
+
+  If the EntityManager has been garbage collected, all methods
+  raise TypeError.
+  """
+
+  __slots__ = ('_manager',)
+
+  _manager: Callable[[], 'EntityManager']
+
+  def __call__(self, component_type: type[_T], /) -> Iterator[_T]:
+    manager = self._manager()
+    entities = manager._entities
+    return (
+      component
+      for entity_id in manager._component_types.get(component_type, ())
+      for component in entities[entity_id](component_type)
+    )
+
+  def __getitem__(self, component_type: type[_T], /) -> Iterator[_T]:
+    manager = self._manager()
+    entities = manager._entities
+    return (entities[entity_id][component_type]
+            for entity_id in manager._component_types.get(component_type, ()))
+
+  def types(self) -> KeysView[type]:
+    return self._manager()._component_types.keys()
+
+  def __iter__(self) -> Iterator[object]:
+    for entity in self._manager():
+      yield from entity
+
+  def __reversed__(self) -> Iterator[object]:
+    for entity in reversed(self._manager()):
+      yield from reversed(entity)
+
+  def __len__(self):
+    return sum(len(entity) for entity in self._manager()._entities.values())
+
+  def __contains__(self, obj: object, /):
+    types = self._manager()._component_types
+    if isinstance(obj, type):
+      for cls in subclasses(obj):
+        if cls in types:
+          return True
+    return False
+
+
+class EntityManager:
+  __slots__ = '_entities', '_component_types', 'components', 'event_queue', '__weakref__'
+
+  def __init__(
+    self, entities: Iterable[Entity] = (), /, event_queue: EventQueue | None = None
+  ):
+    self.event_queue = event_queue
+    self.components = _Components()
+    self.components._manager = weakref(self)  # type: ignore
+    self._entities: dict[EntityId, Entity] = {}
+    self._component_types: dict[type, set[EntityId]] = {}
+    self.add(*entities)
+
+  def add(self, *entities: Entity) -> None:
+    component_types = self._component_types
+    self_entities = self._entities
+    self_weakref: weakref[EntityManager] = weakref(self)
+    event_queue = self.event_queue
+    for entity in entities:
+      entity_id = entity.id
+      if entity_id in self_entities:
+        continue
+      if entity._manager() is not None:
+        raise RuntimeError(f'{entity!r} already added to another manager')
+      self_entities[entity_id] = entity
+      entity._manager = self_weakref
+      for component_type in {
+        component_type for cls in entity.types() for component_type in cls.__mro__
+      }:
+        try:
+          component_types[component_type].add(entity_id)
+        except KeyError:
+          component_types[component_type] = {entity_id}
+      if event_queue is not None:
+        event_queue.extend([
+          EntityAdded(entity),
+          *[ComponentAdded(entity, component) for component in entity]
+        ])
+
+  def create(self, *components: object) -> Entity:
+    """Create an Entity with the given components, add it to self, and return it.
+
+    The returned Entity can, of course, be directly modified.
+    """
+    entity: Entity = Entity(components)
+    self.add(entity)
+    return entity
+
+  def remove(self, *entities: Entity) -> None:
+    component_types = self._component_types
+    event_queue = self.event_queue
+    for entity in entities:
+      entity_id = entity.id
+      try:
+        del self._entities[entity_id]
+      except KeyError:
+        raise ValueError(entity) from None
+      entity._manager = dead_weakref
+      for component_type in {
+        component_type for cls in entity.types() for component_type in cls.__mro__
+      }:
+        component_type_entities = component_types[component_type]
+        component_type_entities.remove(entity_id)
+        if not component_type_entities:
+          del component_types[component_type]
+      if event_queue is not None:
+        event_queue.extend([
+          EntityRemoved(entity),
+          *[ComponentRemoved(entity, component) for component in entity]
+        ])
+
+  def __getitem__(self, entity_id: EntityId, /) -> Entity:
+    return self._entities[entity_id]
+
+  def __delitem__(self, entity_id: EntityId, /):
+    self.remove(self._entities[entity_id])
+
+  @overload
+  def get(self, entity_id: EntityId, /) -> Entity | None: ...
+  @overload
+  def get(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
+  def get(self, entity_id, default=None, /):
+    return self._entities.get(entity_id, default)
+
+  @overload
+  def pop(self, entity_id: EntityId, /) -> Entity: ...
+  @overload
+  def pop(self, entity_id: EntityId, default: _T, /) -> Entity | _T: ...
+  def pop(self, entity_id, default=_SENTINEL, /):
+    try:
+      entity = self._entities[entity_id]
+    except KeyError:
+      if default is _SENTINEL:
+        raise
+      return default
+    self.remove(entity)
+    return entity
+
+  @overload
+  def query(self, query: Query, /) -> ComponentQueryResult: ...
+  @overload
+  def query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> ComponentQueryResult: ...
+  def query(self, /, *types, merge=None):
+    """"""
+    return self._query(ComponentQueryResult, types, merge)
+
+  @overload
+  def entity_query(self, query: Query, /) -> EntityQueryResult: ...
+  @overload
+  def entity_query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> EntityQueryResult: ...
+  def entity_query(self, /, *types, merge=None):
+    """"""
+    return self._query(EntityQueryResult, types, merge)
+
+  @overload
+  def id_query(self, query: Query, /) -> IdQueryResult: ...
+  @overload
+  def id_query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> IdQueryResult: ...
+  def id_query(self, /, *types, merge=None):
+    """"""
+    return self._query(IdQueryResult, types, merge)
+
+  def _query(self, result_cls: type[_Q], types, merge=None, /) -> _Q:
+    """"""
+    if len(types) == 1 and isinstance((query := types[0]), Query):
+      if merge is not None:
+        raise TypeError('unexpected keyword argument: merge')
+      types = query.types
+      merge = query.merge
+    elif merge is None:
+      merge = set.intersection
+    if not types:
+      raise TypeError('expected at least one component type')
+    self_entities = self._entities
+    self_component_types = self._component_types
+    return result_cls(
+      {
+        id: self_entities[id]
+        for id in merge(*[
+          self_component_types[typ]  # noqa: SIM401
+          if typ in self_component_types else set()
+          for typ in types
+        ])
+      },
+      types,
+      merge
+    )
+
+  def __call__(self, component_type: type, /) -> Iterator[Entity]:
+    """Return a generator of all entities in self that contain component_type."""
+    entities = self._entities
+    return (
+      entities[entity_id] for entity_id in self._component_types.get(component_type, ())
+    )
+
+  @overload
+  def ids(self, /) -> KeysView[EntityId]: ...
+  @overload
+  def ids(self, component_type: type, /) -> set[EntityId]: ...
+  def ids(self, component_type=None, /):
+    """Return a set of all entity ids that contain the given component type.
+
+    If no component type is given, then
+    return a set-like view of all entity ids in self instead.
+    """
+    if component_type is None:
+      return self._entities.keys()
+    component_types = self._component_types
+    if component_type not in component_types:
+      return set()
+    return set(component_types[component_type])
+
+  def __iter__(self):
+    """Return an iterator of all Entities in self.
+
+    The least recently added Entities are first.
+    """
+    return iter(self._entities.values())
+
+  def __reversed__(self):
+    return reversed(self._entities.values())
+
+  def __len__(self):
+    return len(self._entities)
+
+  def __contains__(self, obj: object, /):
+    if isinstance(obj, Entity):
+      return obj.id in self._entities
+    return obj in self._entities
+
+  def clear(self):
+    self.remove(*self)
+
+  def _components_added(
+    self, entity_id: EntityId, components: Iterable[object], events: Iterable[object], /
+  ) -> None:
+    component_types = self._component_types
+    for component_type in {
+      component_type
+      for component in components
+      for component_type in type(component).__mro__
+    }:
+      try:
+        component_types[component_type].add(entity_id)
+      except KeyError:
+        component_types[component_type] = {entity_id}
+    if (queue := self.event_queue) is not None:
+      queue.extend(events)
+
+  def _components_removed(self, entity: Entity, components: Iterable[object], /) -> None:
+    component_types = self._component_types
+    entity_id = entity.id
+    for component_type in {
+      component_type
+      for component in components
+      for component_type in type(component).__mro__
+      if component_type not in entity
+    }:
+      entity_ids = component_types[component_type]
+      entity_ids.remove(entity_id)
+      if not entity_ids:
+        del component_types[component_type]
+    if (queue := self.event_queue) is not None:
+      queue.extend([ComponentRemoved(entity, component) for component in components])
```

### Comparing `pyriak-0.2.0/src/pyriak/managers/systemmanager.py` & `pyriak-0.3.0/src/pyriak/managers/systemmanager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,499 +1,543 @@
-__all__ = ['SystemManager']
-
-from collections.abc import Hashable, Iterable, Iterator, Mapping
-from typing import TYPE_CHECKING, Any, NamedTuple
-from weakref import ref as weakref
-
-from pyriak import EventQueue, dead_weakref, strict_subclasses, subclasses
-from pyriak.eventkey import key_functions
-from pyriak.events import (
-  EventHandlerAdded,
-  EventHandlerRemoved,
-  SendEvent,
-  SpaceCallback,
-  SystemAdded,
-  SystemRemoved,
-)
-from pyriak.system import System, _Callback
-
-
-if TYPE_CHECKING:
-  from pyriak.space import Space
-
-
-class _EventHandler(NamedTuple):
-  """Object that holds the info for a single event handler callback in a SystemManager.
-
-  A function on a system can be bound to event types. If a function is bound
-  to at least one event type (most common is just one), then it is an event handler
-  callback. A binding (of an event type), its info (keys and priority),
-  and the callback are considered one event handler.
-  There is usually a separate event handler object for event type for each callback.
-  However, if a function is bound to multiple event types with the same priority object,
-  then the event handler object is shared (implementation detail). Here, keys do
-  not affect sharing because it is not kept in the event handler object.
-  This is a common case for callbacks with multiple bindings because a callback
-  is only a single function, so its event types must usually be very similar and
-  therefore their priority is similar. (Otherwise, it would be two separate callbacks.)
-
-  The data stored in this object is used for invoking, sorting, and storing
-  the event handler.
-  This object stores more data than _Binding because there is less context available.
-  """
-
-  system: System
-  callback: _Callback
-  name: str
-  priority: Any
-
-  def __call__(self, /, *args, **kwargs):
-    return self.callback(*args, **kwargs)
-
-  def __eq__(self, other: object):
-    if self is other:
-      return True
-    if isinstance(other, _EventHandler):
-      return self.name == other.name and self.system == other.system
-    return NotImplemented
-
-  def __hash__(self):
-    return hash((self.name,self.system))
-
-del NamedTuple
-
-
-class SystemManager:
-  __slots__ = (
-    '_space', '_systems', '_handlers', '_key_handlers', 'event_queue', '__weakref__'
-  )
-
-  event_queue: EventQueue | None
-
-  def __init__(
-    self,
-    systems: Iterable[System] = (),
-    /,
-    space: 'Space | None' = None,
-    event_queue: EventQueue | None = None
-  ):
-    self.space = space
-    self.event_queue = event_queue
-    # values aren't used: dict is for insertion order
-    self._systems: dict[System, None] = {}
-    self._handlers: dict[type, list[_EventHandler]] = {}
-    self._key_handlers: dict[type, dict[Hashable, list[_EventHandler]]] = {}
-    self.add(*systems)
-
-  def process(self, event: object, space: 'Space | None' = None) -> bool:
-    """Handle an event. Callbacks of the event are passed space and event.
-
-    If the Event type has no binds, do nothing.
-    If event is an instance of SpaceCallback or SendEvent, it is handled differently.
-    If a callback returns a truthy value, the
-    rest of the callbacks are skipped and True is returned, else False.
-    """
-    if space is None:
-      space = self.space
-      if space is None:
-        raise TypeError("process() missing 'space'")
-    for handler in self._get_handlers(event)[:]:
-      if handler.callback(space, event):
-        return True
-    if isinstance(event, SpaceCallback) and event(space):
-      return True
-    if isinstance(event, SendEvent):
-      receivers = event.receivers
-      event = event.event
-      for handler in [
-        handler for handler in self._get_handlers(event) if handler.system in receivers
-      ]:
-        if handler.callback(space, event):
-          return True
-    return False
-
-  def add(self, *systems: System) -> None:
-    """[[Add systems, their priorities, and systems' event binds to self, from objs.
-
-    Each obj in objs can be:
-    - an argument to be passed into dict(), to construct a dictionary
-      with items of System for key and priority for value.
-      Any priorities that are None are replaced with
-      its corresponding System's default priority.
-    - else (dict construction fails), a System,
-      whose priority will be its default priority.
-
-    The order in which the Systems are added is that Systems from the first objs
-    are added first.
-
-    Adding or removing a system is expensive because of the
-    binding or unbinding of event bind system callbacks.
-    This is so that triggering events is fast.
-    Any Systems already in self have their priority updated (and event binds rebound),
-    and don't trigger SystemAdded event.
-    Systems not already in self get their _added_ method
-    invoked right after they are added and bound.]]
-    """
-    self_systems = self._systems
-    bind = self._bind
-    for system in systems:
-      if system in self_systems:
-        continue
-      self_systems[system] = None
-      events = bind(system)
-      space = self.space
-      event_queue = self.event_queue
-      if space is None:
-        if event_queue is not None:
-          event_queue.extend([
-            SpaceCallback(system._added_), SystemAdded(system), *events
-          ])
-      else:
-        if event_queue is not None:
-          event_queue.extend([SystemAdded(system), *events])
-        system._added_(space)
-
-  def remove(self, *systems: System) -> None:
-    """Remove systems and their event handlers from self.
-
-    Removing Systems is expensive (see SystemManager.add method for why).
-    Right after a System is removed and unbound, its _removed_ method invoked.
-    Raises KeyError if any of the systems are not in self.
-    """
-    self_systems = self._systems
-    unbind = self._unbind
-    for system in systems:
-      del self_systems[system]
-      events = unbind(system)
-      space = self.space
-      event_queue = self.event_queue
-      if space is None:
-        if event_queue is not None:
-          event_queue.extend([
-            SpaceCallback(system._removed_), SystemRemoved(system), *events
-          ])
-      else:
-        if event_queue is not None:
-          event_queue.extend([SystemRemoved(system), *events])
-        system._removed_(space)
-
-  def discard(self, *systems: System) -> None:
-    self_systems = self._systems
-    for system in systems:
-      if system in self_systems:
-        self.remove(system)
-
-  def __iter__(self):
-    """Return an iterator of all systems in self, in the order they were added."""
-    return iter(self._systems)
-
-  def __reversed__(self):
-    return reversed(self._systems)
-
-  def __len__(self):
-    return len(self._systems)
-
-  def __contains__(self, obj: object, /):
-    """Return whether obj is a system added to self (ignoring subclasses)."""
-    return obj in self._systems
-
-  def clear(self):
-    """Remove all systems and event handlers from self.
-
-    Does not trigger any events.
-    Does not invoke System._removed_ method.
-    Does not change self's space or event_queue.
-    """
-    self._handlers.clear()
-    self._key_handlers.clear()
-    self._systems.clear()
-
-  @property
-  def space(self) -> 'Space | None':
-    return self._space()
-
-  @space.setter
-  def space(self, value: 'Space | None'):
-    self._space = dead_weakref if value is None else weakref(value)
-
-  @staticmethod
-  def _insert_handler(list: list[_EventHandler], handler: _EventHandler, /) -> None:
-    """Inserts a handler into a list of other handlers.
-
-    Sorts by: highest priority, then oldest handler.
-    """
-    priority = handler.priority
-    lo = 0
-    hi = len(list)
-    while lo < hi:
-      mid = (lo + hi) // 2
-      if list[mid].priority < priority:
-        hi = mid
-      else:
-        lo = mid + 1
-    list.insert(lo, handler)
-
-  class _SortKey:
-    __slots__ = 'handler', 'systems'
-    def __init__(self, handler: _EventHandler, systems: Iterable[System], /):
-      self.handler = handler
-      self.systems = systems
-    def __lt__(self, other: 'SystemManager._SortKey', /) -> bool:
-      handler = self.handler
-      other_handler = other.handler
-      other_priority = other_handler.priority
-      handler_priority = handler.priority
-      if not (other_priority == handler_priority):
-        return other_priority < handler_priority
-      system = handler.system
-      other_system = other_handler.system
-      if system is not other_system:
-        for s in self.systems:
-          if s is system:
-            return True
-          if s is other_system:
-            return False
-        raise ValueError
-      name = handler.name
-      other_name = other_handler.name
-      for n in system._handlers_:
-        if other_name == n:
-          return False
-        if name == n:
-          return True
-      raise ValueError
-
-  def _sort_handlers(
-    self, handlers: Iterable[_EventHandler], /
-  ) -> list[_EventHandler]:
-    SortKey = self._SortKey
-    systems = self._systems
-    # Uses dict to remove duplicates while preserving some order
-    return sorted(dict.fromkeys(handlers), key=lambda h: SortKey(h, systems))
-
-  def _get_handlers(self, event: object, /) -> list[_EventHandler]:
-    event_type = type(event)
-    try:
-      handlers = self._handlers[event_type]
-    except KeyError:
-      handlers = self._lazy_bind(event_type)
-      if not key_functions.exists(event_type):
-        return handlers
-      key_handlers = self._lazy_key_bind(event_type)
-    else:
-      if event_type not in self._key_handlers:
-        return handlers
-      key_handlers = self._key_handlers[event_type]
-    key = key_functions(event_type)(event)
-    if not isinstance(key, Iterator):
-      try:
-        return key_handlers[key]
-      except KeyError:
-        return handlers
-    keys = {k for k in key if k in key_handlers}
-    if len(keys) > 1:
-      return self._sort_handlers(handler for key in keys for handler in key_handlers[key])
-    if keys:
-      return key_handlers[keys.pop()]
-    return handlers
-
-  def _bind(self, system: System, /) -> list[EventHandlerAdded]:
-    """Bind a system's handlers so that they can process events.
-
-    If a specified event type does not exist, _lazy_bind is called to find
-    bindings for it based on existing superclasses.
-
-    Bindings of an event type are sorted by highest priority,
-    then oldest system, then first one bound in system.
-    """
-    if not isinstance(system, System):
-      raise TypeError(f'{system!r} is not a System')
-    if not system._bindings_:
-      return []
-    handler_events: list[EventHandlerAdded] = []
-    all_handlers = self._handlers
-    all_key_handlers = self._key_handlers
-    insert_handler = self._insert_handler
-    fromkeys = dict.fromkeys
-    for name, bindings in system._bindings_.items():
-      callback = getattr(system, name)
-      if len(bindings) == 1:
-        # the common case of only one event type for a handler (single @bind())
-        [(event_type, binding)] = bindings.items()
-        handler = _EventHandler(system, callback, name, binding.priority)
-        event_handlers = {
-          cls: handler for cls in strict_subclasses(event_type) if cls in all_handlers
-        }
-        key_event_types = event_handlers.keys() & all_key_handlers
-        event_handlers[event_type] = handler
-        if key_functions.exists(event_type):
-          key_event_types.add(event_type)
-        binding_keys = binding.keys
-        handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = (
-          fromkeys(key_event_types, fromkeys(binding_keys, handler))
-          if binding_keys else {}
-        )
-        handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
-      else:
-        event_handlers = {}
-        base_handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = {}
-        cached_handlers: dict[int, _EventHandler] = {}
-        for event_type, binding in bindings.items():
-          priority = binding.priority
-          priority_id = id(priority)
-          if priority_id in cached_handlers:
-            handler = cached_handlers[priority_id]
-          else:
-            handler = cached_handlers[priority_id] = _EventHandler(
-              system, callback, name, priority
-            )
-          event_handlers[event_type] = handler
-          binding_keys = binding.keys
-          if binding_keys:
-            base_handler_keys[event_type] = fromkeys(binding_keys, handler)
-          handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
-        del cached_handlers
-        # Subclasses of bound event types may also trigger the event handler,
-        # and will inherit their binding (keys and priority).
-        # In the rare case that a class is the subclass of multiple bound
-        # event types, the subclass will try to inherit the bindings of all,
-        # but the first bound type in its MRO will take precedence
-        # for shared keys (or when the subclass is keyless).
-        # A bound event type may be the subclass of other bound event types.
-        for cls in {
-          cls
-          for event_type in bindings
-          for cls in strict_subclasses(event_type)
-          if cls in all_handlers
-        }:
-          for base in cls.__mro__:
-            if base in bindings:
-              event_handlers[cls] = event_handlers[base]
-              break
-          else:
-            raise RuntimeError
-        handler_keys = {}
-        key_event_types = event_handlers.keys() & all_key_handlers
-        key_event_types |= {ev_t for ev_t in bindings if key_functions.exists(ev_t)}
-        for cls in key_event_types:
-          inherit_handler_keys: dict[Hashable, _EventHandler] = {}
-          total_len = 0
-          for base in reversed(cls.__mro__):
-            if base in base_handler_keys:
-              inherit_base_keys = base_handler_keys[base]
-              inherit_handler_keys.update(inherit_base_keys)
-              total_len += len(inherit_base_keys)
-          if total_len != len(inherit_handler_keys):
-            # When inheriting multiple of the same key,
-            # the key object of the first type in the MRO is kept
-            inherit_handler_keys = {
-              key: inherit_handler_keys[key]
-              for base in cls.__mro__ for key in base_handler_keys.get(base, ())
-            }
-          handler_keys[cls] = inherit_handler_keys
-
-      for event_type, handler in event_handlers.items():
-        handlers = (
-          all_handlers[event_type] if event_type in all_handlers
-          else self._lazy_bind(event_type)
-        )
-        if event_type not in key_event_types:
-          insert_handler(handlers, handler)
-          continue
-        key_handlers = (
-          all_key_handlers[event_type] if event_type in all_key_handlers
-          else self._lazy_key_bind(event_type)
-        )
-        keys = handler_keys.get(event_type, {})
-        if not keys:
-          insert_handler(handlers, handler)
-          for handlers in key_handlers.values():
-            insert_handler(handlers, handler)
-          continue
-        for key, handler in keys.items():
-          if key not in key_handlers:
-            key_handlers[key] = handlers[:]
-          insert_handler(key_handlers[key], handler)
-    return handler_events
-
-  def _lazy_bind(self, event_type: type, /) -> list[_EventHandler]:
-    """Find bindings for event_type and bind them and return the handlers.
-
-    Subclass instances of an event_type can be processed by superclass handlers.
-    These subclasses are only bound when a subclass is processed. Hence, lazy binding.
-    """
-    all_handlers = self._handlers
-    event_handlers = [
-      handler
-      for ev_t in event_type.__mro__
-      if ev_t in all_handlers
-      for handler in all_handlers[ev_t]
-    ]
-    if event_handlers:
-      event_handlers = self._sort_handlers(event_handlers)
-    all_handlers[event_type] = event_handlers
-    return event_handlers
-
-  def _lazy_key_bind(
-    self, event_type: type, /
-  ) -> dict[Hashable, list[_EventHandler]]:
-    all_key_handlers = self._key_handlers
-    inherit_key_handlers = [
-      item
-      for ev_t in event_type.__mro__
-      if ev_t in all_key_handlers
-      for item in all_key_handlers[ev_t].items()
-    ]
-    if inherit_key_handlers:
-      unsorted_handlers: dict[Hashable, list[list[_EventHandler]]] = {}
-      base_handlers = self._handlers[event_type]
-      for key, handlers in inherit_key_handlers:
-        if key in unsorted_handlers:
-          unsorted_handlers[key].append(handlers)
-        else:
-          unsorted_handlers[key] = [base_handlers, handlers]
-      sort_handlers = self._sort_handlers
-      key_handlers: dict[Hashable, list[_EventHandler]] = {
-        key: sort_handlers(handler for handlers in handlers_list for handler in handlers)
-        for key, handlers_list in unsorted_handlers.items()
-      }
-    else:
-      key_handlers = {}
-    all_key_handlers[event_type] = key_handlers
-    return key_handlers
-
-  def _unbind(self, system: System, /) -> list[EventHandlerRemoved]:
-    """Remove all handlers that belong to system from self.
-
-    If an event type no longer has any handlers, it is removed.
-    This also applies to keys with handlers.
-    """
-    events: list[EventHandlerRemoved] = []
-    all_handlers = self._handlers
-    all_key_handlers = self._key_handlers
-    for name, event_types in system._bindings_.items():
-      for cls, binding in event_types.items():
-        for event_type in subclasses(cls):
-          try:
-            handlers = all_handlers[event_type]
-          except KeyError:
-            continue
-          handlers[:] = [
-            handler for handler in handlers if handler.system is not system
-          ]
-          if not handlers:
-            del all_handlers[event_type]
-          if event_type not in all_key_handlers:
-            continue
-          key_handlers = all_key_handlers[event_type]
-          for key, handlers in key_handlers.items():
-            handlers[:] = [
-              handler for handler in handlers if handler.system is not system
-            ]
-            if not handlers:
-              del key_handlers[key]
-          if not key_handlers:
-            del all_key_handlers[event_type]
-        events.append(EventHandlerRemoved(
-          system, getattr(system, name), name, binding.priority, cls, binding.keys
-        ))
-    return events
+__all__ = ['SystemManager']
+
+from collections.abc import Hashable, Iterable, Iterator, Mapping
+from inspect import getattr_static
+from types import ModuleType
+from typing import TYPE_CHECKING, Any, NamedTuple
+from weakref import ref as weakref
+
+from pyriak import EventQueue, dead_weakref, strict_subclasses, subclasses
+from pyriak.eventkey import key_functions
+from pyriak.events import (
+  EventHandlerAdded,
+  EventHandlerRemoved,
+  SendEvent,
+  SpaceCallback,
+  SystemAdded,
+  SystemRemoved,
+)
+from pyriak.system import BindingWrapper, System, _Callback
+
+
+if TYPE_CHECKING:
+  from pyriak.space import Space
+
+
+class _EventHandler(NamedTuple):
+  """Object that holds the info for a single event handler callback in a SystemManager.
+
+  A function on a system can be bound to event types. If a function is bound
+  to at least one event type (most common is just one), then it is an event handler
+  callback. A binding (of an event type), its info (keys and priority),
+  and the callback are considered one event handler.
+  There is usually a separate event handler object for event type for each callback.
+  However, if a function is bound to multiple event types with the same priority object,
+  then the event handler object is shared (implementation detail). Here, keys do
+  not affect sharing because it is not kept in the event handler object.
+  This is a common case for callbacks with multiple bindings because a callback
+  is only a single function, so its event types must usually be very similar and
+  therefore their priority is similar. (Otherwise, it would be two separate callbacks.)
+
+  The data stored in this object is used for invoking, sorting, and storing
+  the event handler.
+  This object stores more data than _Binding because there is less context available.
+  """
+
+  system: System
+  callback: _Callback
+  name: str
+  priority: Any
+
+  def __call__(self, /, *args, **kwargs):
+    return self.callback(*args, **kwargs)
+
+  def __eq__(self, other: object):
+    if self is other:
+      return True
+    if isinstance(other, _EventHandler):
+      return self.name == other.name and self.system == other.system
+    return NotImplemented
+
+  def __hash__(self):
+    return hash((self.name,self.system))
+
+del NamedTuple
+
+
+class SystemManager:
+  __slots__ = (
+    '_space', '_systems', '_handlers', '_key_handlers', 'event_queue', '__weakref__'
+  )
+
+  event_queue: EventQueue | None
+
+  def __init__(
+    self,
+    systems: Iterable[System] = (),
+    /,
+    space: 'Space | None' = None,
+    event_queue: EventQueue | None = None
+  ):
+    self.space = space
+    self.event_queue = event_queue
+    # values aren't used: dict is for insertion order
+    self._systems: dict[System, None] = {}
+    self._handlers: dict[type, list[_EventHandler]] = {}
+    self._key_handlers: dict[type, dict[Hashable, list[_EventHandler]]] = {}
+    self.add(*systems)
+
+  def process(self, event: object, space: 'Space | None' = None) -> bool:
+    """Handle an event. Callbacks of the event are passed space and event.
+
+    If the Event type has no binds, do nothing.
+    If event is an instance of SpaceCallback or SendEvent, it is handled differently.
+    If a callback returns a truthy value, the
+    rest of the callbacks are skipped and True is returned, else False.
+    """
+    if space is None:
+      space = self.space
+      if space is None:
+        raise TypeError("process() missing 'space'")
+    for handler in self._get_handlers(event)[:]:
+      if handler.callback(space, event):
+        return True
+    if isinstance(event, SpaceCallback) and event(space):
+      return True
+    if isinstance(event, SendEvent):
+      receivers = event.receivers
+      event = event.event
+      for handler in [
+        handler for handler in self._get_handlers(event) if handler.system in receivers
+      ]:
+        if handler.callback(space, event):
+          return True
+    return False
+
+  def add(self, *systems: System) -> None:
+    """[[Add systems, their priorities, and systems' event binds to self, from objs.
+
+    Each obj in objs can be:
+    - an argument to be passed into dict(), to construct a dictionary
+      with items of System for key and priority for value.
+      Any priorities that are None are replaced with
+      its corresponding System's default priority.
+    - else (dict construction fails), a System,
+      whose priority will be its default priority.
+
+    The order in which the Systems are added is that Systems from the first objs
+    are added first.
+
+    Adding or removing a system is expensive because of the
+    binding or unbinding of event bind system callbacks.
+    This is so that triggering events is fast.
+    Any Systems already in self have their priority updated (and event binds rebound),
+    and don't trigger SystemAdded event.
+    Systems not already in self get their _added_ method
+    invoked right after they are added and bound.]]
+    """
+    self_systems = self._systems
+    bind = self._bind
+    for system in systems:
+      if system in self_systems:
+        continue
+      self_systems[system] = None
+      events = bind(system)
+      space = self.space
+      event_queue = self.event_queue
+      if space is not None:
+        if event_queue is not None:
+          event_queue.extend([SystemAdded(system), *events])
+        try:
+          added = system._added_  # type: ignore[attr-defined]
+        except AttributeError:
+          continue
+        added(space)
+      elif event_queue is not None:
+        try:
+          added = system._added_  # type: ignore[attr-defined]
+        except AttributeError:
+          event_queue.extend([SystemAdded(system), *events])
+        else:
+          event_queue.extend([SpaceCallback(added), SystemAdded(system), *events])
+
+  def remove(self, *systems: System) -> None:
+    """Remove systems and their event handlers from self.
+
+    Removing Systems is expensive (see SystemManager.add method for why).
+    Right after a System is removed and unbound, its _removed_ method invoked.
+    Raises KeyError if any of the systems are not in self.
+    """
+    self_systems = self._systems
+    unbind = self._unbind
+    for system in systems:
+      del self_systems[system]
+      events = unbind(system)
+      space = self.space
+      event_queue = self.event_queue
+      if space is not None:
+        if event_queue is not None:
+          event_queue.extend([SystemRemoved(system), *events])
+        try:
+          removed = system._removed_  # type: ignore[attr-defined]
+        except AttributeError:
+          continue
+        removed(space)
+      elif event_queue is not None:
+        try:
+          removed = system._removed_  # type: ignore[attr-defined]
+        except AttributeError:
+          event_queue.extend([SystemRemoved(system), *events])
+        else:
+          event_queue.extend([SpaceCallback(removed), SystemRemoved(system), *events])
+
+  def discard(self, *systems: System) -> None:
+    self_systems = self._systems
+    for system in systems:
+      if system in self_systems:
+        self.remove(system)
+
+  def __iter__(self):
+    """Return an iterator of all systems in self, in the order they were added."""
+    return iter(self._systems)
+
+  def __reversed__(self):
+    return reversed(self._systems)
+
+  def __len__(self):
+    return len(self._systems)
+
+  def __contains__(self, obj: object, /):
+    """Return whether obj is a system added to self (ignoring subclasses)."""
+    return obj in self._systems
+
+  def clear(self):
+    """Remove all systems and event handlers from self.
+
+    Does not trigger any events.
+    Does not invoke System._removed_ method.
+    Does not change self's space or event_queue.
+    """
+    self._handlers.clear()
+    self._key_handlers.clear()
+    self._systems.clear()
+
+  @property
+  def space(self) -> 'Space | None':
+    return self._space()
+
+  @space.setter
+  def space(self, value: 'Space | None'):
+    self._space = dead_weakref if value is None else weakref(value)
+
+  @staticmethod
+  def _insert_handler(list: list[_EventHandler], handler: _EventHandler, /) -> None:
+    """Inserts a handler into a list of other handlers.
+
+    Sorts by: highest priority, then oldest in manager
+    """
+    priority = handler.priority
+    lo = 0
+    hi = len(list)
+    while lo < hi:
+      mid = (lo + hi) // 2
+      if list[mid].priority < priority:
+        hi = mid
+      else:
+        lo = mid + 1
+    list.insert(lo, handler)
+
+  class _SortKey:
+    __slots__ = 'handler', 'systems'
+    def __init__(self, handler: _EventHandler, systems: Iterable[System], /):
+      self.handler = handler
+      self.systems = systems
+    def __lt__(self, other: 'SystemManager._SortKey', /) -> bool:
+      handler = self.handler
+      other_handler = other.handler
+      other_priority = other_handler.priority
+      handler_priority = handler.priority
+      if not (other_priority == handler_priority):
+        return other_priority < handler_priority  # type: ignore[no-any-return]
+      system = handler.system
+      other_system = other_handler.system
+      if system != other_system:
+        for s in self.systems:
+          if s == system:
+            return True
+          if s == other_system:
+            return False
+        raise ValueError
+      name = handler.name
+      other_name = other_handler.name
+      if type(system) is not ModuleType:
+        return name < other_name
+      for n in system.__dict__:
+        if other_name == n:
+          return False
+        if name == n:
+          return True
+      raise ValueError
+
+  def _sort_handlers(
+    self, handlers: Iterable[_EventHandler], /
+  ) -> list[_EventHandler]:
+    """Return a sorted list of handlers.
+
+    Sorts by, in order:
+    - highest priority
+    - least recently added system
+    - (same system) order the handlers were added in
+      - if system is module instance, then order created
+      - otherwise, alphabetical names
+    """
+    SortKey = self._SortKey
+    systems = self._systems
+    # Uses dict to remove duplicates while preserving some order
+    return sorted(dict.fromkeys(handlers), key=lambda h: SortKey(h, systems))
+
+  def _get_handlers(self, event: object, /) -> list[_EventHandler]:
+    event_type = type(event)
+    try:
+      handlers = self._handlers[event_type]
+    except KeyError:
+      handlers = self._lazy_bind(event_type)
+      if not key_functions.exists(event_type):
+        return handlers
+      key_handlers = self._lazy_key_bind(event_type)
+    else:
+      if event_type not in self._key_handlers:
+        return handlers
+      key_handlers = self._key_handlers[event_type]
+    key = key_functions(event_type)(event)
+    if not isinstance(key, Iterator):
+      try:
+        return key_handlers[key]
+      except KeyError:
+        return handlers
+    keys = {k for k in key if k in key_handlers}
+    if len(keys) > 1:
+      return self._sort_handlers(handler for key in keys for handler in key_handlers[key])
+    if keys:
+      return key_handlers[keys.pop()]
+    return handlers
+
+  @staticmethod
+  def _get_bindings(system: System):
+    if type(system) is ModuleType:
+      return [
+        (name, wrapper.__bindings__, wrapper.__wrapped__)
+        for name, wrapper in system.__dict__.items()
+        if isinstance(wrapper, BindingWrapper)
+      ]
+    return [
+      (
+        name, wrapper.__bindings__,
+        c if (c:=getattr(system, name)) is not wrapper else wrapper.__wrapped__
+      )
+      for name in dict.fromkeys(dir(system))
+      if isinstance((wrapper:=getattr_static(system, name)), BindingWrapper)
+    ]
+
+  def _bind(self, system: System, /) -> list[EventHandlerAdded]:
+    """Bind a system's handlers so that they can process events.
+
+    If a specified event type does not exist, _lazy_bind is called to find
+    bindings for it based on existing superclasses.
+
+    Bindings of an event type are sorted by highest priority,
+    then oldest system, then first one bound in system.
+    """
+    system_bindings = self._get_bindings(system)
+    if not system_bindings:
+      return []
+    fromkeys = dict.fromkeys
+    handler_events: list[EventHandlerAdded] = []
+    all_handlers = self._handlers
+    all_key_handlers = self._key_handlers
+    insert_handler = self._insert_handler
+    for name, bindings, callback in system_bindings:
+      if len(bindings) == 1:
+        # the common case of only one event type for a handler (single @bind())
+        binding = bindings[0]
+        event_type = binding.event_type
+        handler = _EventHandler(system, callback, name, binding.priority)
+        binding_keys = binding.keys
+        event_handlers = {
+          cls: handler for cls in strict_subclasses(event_type) if cls in all_handlers
+        }
+        key_event_types = event_handlers.keys() & all_key_handlers
+        event_handlers[event_type] = handler
+        if key_functions.exists(event_type):
+          key_event_types.add(event_type)
+        handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = (
+          fromkeys(key_event_types, fromkeys(binding_keys, handler))
+          if binding_keys else {}
+        )
+        handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
+      else:
+        event_handlers = {}
+        base_handler_keys: dict[type, Mapping[Hashable, _EventHandler]] = {}
+        cached_handlers: dict[int, _EventHandler] = {}
+        for binding in bindings:
+          event_type = binding.event_type
+          priority = binding.priority
+          binding_keys = binding.keys
+          priority_id = id(priority)
+          if priority_id in cached_handlers:
+            handler = cached_handlers[priority_id]
+          else:
+            handler = cached_handlers[priority_id] = _EventHandler(
+              system, callback, name, priority
+            )
+          event_handlers[event_type] = handler
+          if binding_keys:
+            base_handler_keys[event_type] = fromkeys(binding_keys, handler)
+          handler_events.append(EventHandlerAdded(handler, event_type, binding_keys))
+        del cached_handlers
+        # Subclasses of bound event types may also trigger the event handler,
+        # and will inherit their binding (keys and priority).
+        # In the rare case that a class is the subclass of multiple bound
+        # event types, the subclass will try to inherit the bindings of all,
+        # but the first bound type in its MRO will take precedence
+        # for shared keys (or when the subclass is keyless).
+        # A bound event type may be the subclass of other bound event types.
+        event_types = set(event_handlers)
+        for cls in {
+          cls
+          for event_type in event_types
+          for cls in strict_subclasses(event_type)
+          if cls in all_handlers
+        }:
+          for base in cls.__mro__:
+            if base in event_types:
+              event_handlers[cls] = event_handlers[base]
+              break
+          else:
+            raise RuntimeError
+        handler_keys = {}
+        key_event_types = event_handlers.keys() & all_key_handlers
+        key_event_types |= {ev_t for ev_t in event_types if key_functions.exists(ev_t)}
+        for cls in key_event_types:
+          inherit_handler_keys: dict[Hashable, _EventHandler] = {}
+          total_len = 0
+          for base in reversed(cls.__mro__):
+            if base in base_handler_keys:
+              inherit_base_keys = base_handler_keys[base]
+              inherit_handler_keys.update(inherit_base_keys)
+              total_len += len(inherit_base_keys)
+          if total_len != len(inherit_handler_keys):
+            # When inheriting multiple of the same key,
+            # the key object of the first type in the MRO is kept
+            inherit_handler_keys = {
+              key: inherit_handler_keys[key]
+              for base in cls.__mro__ for key in base_handler_keys.get(base, ())
+            }
+          handler_keys[cls] = inherit_handler_keys
+
+      for event_type, handler in event_handlers.items():
+        handlers = (
+          all_handlers[event_type] if event_type in all_handlers
+          else self._lazy_bind(event_type)
+        )
+        if event_type not in key_event_types:
+          insert_handler(handlers, handler)
+          continue
+        key_handlers = (
+          all_key_handlers[event_type] if event_type in all_key_handlers
+          else self._lazy_key_bind(event_type)
+        )
+        keys = handler_keys.get(event_type, {})
+        if not keys:
+          insert_handler(handlers, handler)
+          for handlers in key_handlers.values():
+            insert_handler(handlers, handler)
+          continue
+        for key, handler in keys.items():
+          if key not in key_handlers:
+            key_handlers[key] = handlers[:]
+          insert_handler(key_handlers[key], handler)
+    return handler_events
+
+  def _lazy_bind(self, event_type: type, /) -> list[_EventHandler]:
+    """Find bindings for event_type and bind them and return the handlers.
+
+    Subclass instances of an event_type can be processed by superclass handlers.
+    These subclasses are only bound when a subclass is processed. Hence, lazy binding.
+    """
+    all_handlers = self._handlers
+    event_handlers = [
+      handler
+      for ev_t in event_type.__mro__
+      if ev_t in all_handlers
+      for handler in all_handlers[ev_t]
+    ]
+    if event_handlers:
+      event_handlers = self._sort_handlers(event_handlers)
+    all_handlers[event_type] = event_handlers
+    return event_handlers
+
+  def _lazy_key_bind(
+    self, event_type: type, /
+  ) -> dict[Hashable, list[_EventHandler]]:
+    all_key_handlers = self._key_handlers
+    inherit_key_handlers = [
+      item
+      for ev_t in event_type.__mro__
+      if ev_t in all_key_handlers
+      for item in all_key_handlers[ev_t].items()
+    ]
+    if inherit_key_handlers:
+      unsorted_handlers: dict[Hashable, list[list[_EventHandler]]] = {}
+      base_handlers = self._handlers[event_type]
+      for key, handlers in inherit_key_handlers:
+        if key in unsorted_handlers:
+          unsorted_handlers[key].append(handlers)
+        else:
+          unsorted_handlers[key] = [base_handlers, handlers]
+      sort_handlers = self._sort_handlers
+      key_handlers: dict[Hashable, list[_EventHandler]] = {
+        key: sort_handlers(handler for handlers in handlers_list for handler in handlers)
+        for key, handlers_list in unsorted_handlers.items()
+      }
+    else:
+      key_handlers = {}
+    all_key_handlers[event_type] = key_handlers
+    return key_handlers
+
+  def _unbind(self, system: System, /) -> list[EventHandlerRemoved]:
+    """Remove all handlers that belong to system from self.
+
+    If an event type no longer has any handlers, it is removed.
+    This also applies to keys with handlers.
+    """
+    events: list[EventHandlerRemoved] = []
+    all_handlers = self._handlers
+    all_key_handlers = self._key_handlers
+    for name, bindings, callback in self._get_bindings(system):
+      for binding in bindings:
+        cls = binding.event_type
+        for event_type in subclasses(cls):
+          try:
+            handlers = all_handlers[event_type]
+          except KeyError:
+            continue
+          handlers[:] = [
+            handler for handler in handlers if handler.system != system
+          ]
+          if not handlers:
+            del all_handlers[event_type]
+          if event_type not in all_key_handlers:
+            continue
+          key_handlers = all_key_handlers[event_type]
+          for key, handlers in key_handlers.items():
+            handlers[:] = [
+              handler for handler in handlers if handler.system != system
+            ]
+            if not handlers:
+              del key_handlers[key]
+          if not key_handlers:
+            del all_key_handlers[event_type]
+        events.append(EventHandlerRemoved(
+          system, callback, name, binding.priority, cls, binding.keys
+        ))
+    return events
```

### Comparing `pyriak-0.2.0/src/pyriak/query.py` & `pyriak-0.3.0/src/pyriak/query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,224 @@
-__all__ = [
-  'Query',
-  'QueryResult',
-  'ComponentQueryResult',
-  'EntityQueryResult',
-  'IdQueryResult',
-]
-
-from abc import ABC, abstractmethod
-from collections.abc import Iterator, KeysView, ValuesView
-from typing import Any, Callable, NoReturn, TypeVar, overload
-
-from pyriak.entity import Entity, EntityId
-
-
-_T = TypeVar('_T')
-
-
-class Query:
-  __slots__ = '_types', '_merge'
-
-  @overload
-  def __init__(self, *, merge: Callable[..., set] = set.intersection) -> NoReturn: ...
-  @overload
-  def __init__(
-    self, *component_types: type, merge: Callable[..., set] = set.intersection
-  ): ...
-  def __init__(self, *component_types, merge=set.intersection):
-    if not component_types:
-      raise TypeError('expected at least one component type')
-    self._types = component_types
-    self._merge = merge
-
-  @property
-  def types(self) -> tuple[type, ...]:
-    return self._types
-
-  @property
-  def merge(self):
-    return self._merge
-
-  def count(self, value: type, /):
-    return self._types.count(value)
-
-  def index(self, *args):
-    return self._types.index(*args)
-
-  def __getitem__(self, key, /):
-    return self._types[key]
-
-  def __iter__(self):
-    return iter(self._types)
-
-  def __len__(self):
-    return len(self._types)
-
-  def __contains__(self, obj: object, /):
-    return obj in self._types
-
-  def __eq__(self, other: object, /):
-    if not isinstance(other, Query):
-      return NotImplemented
-    # TODO: investigate unusual problem with type narrowing
-    return self._types == other._types and self._merge == other._merge  # type: ignore
-
-  def __hash__(self):
-    return hash((self._types,self._merge))
-
-  def __repr__(self):
-    return (
-      f'{type(self).__name__}'
-      f'({", ".join(repr(t) for t in self._types)}, merge={self._merge!r})'
-    )
-
-
-class QueryResult(ABC):
-  __slots__ = '_entities', '_types', '_merge'
-
-  def __init__(self, _entities, _types, _merge, /):
-    self._entities = _entities
-    self._types = _types
-    self._merge = _merge
-
-  @property
-  def ids(self) -> KeysView[EntityId]:
-    return self._entities.keys()
-
-  @property
-  def entities(self) -> ValuesView[Entity]:
-    return self._entities.values()
-
-  @property
-  def types(self) -> tuple[type, ...]:
-    return self._types
-
-  @property
-  def merge(self) -> Callable[..., set]:
-    return self._merge
-
-  def query(self) -> Query:
-    """Return a new Query object that describes self."""
-    return Query(*self.types, merge=self.merge)
-
-  @overload
-  def __call__(self) -> Iterator[Any]: ...
-  @overload
-  def __call__(self, *component_types: type[_T]) -> Iterator[_T]: ...
-  def __call__(self, *component_types):
-    if not component_types:
-      component_types = self.types
-    return (comp for ent in self.entities for comp in ent(*component_types))
-
-  # group method
-
-  @overload
-  @abstractmethod
-  def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  @abstractmethod
-  def __getitem__(
-    self, component_types: tuple[type, ...], /
-  ) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  @abstractmethod
-  def __getitem__(
-    self, component_type: type[_T], /
-  ) -> Iterator[_T] | tuple[Iterator[Any], Iterator[_T]]: ...
-  @abstractmethod
-  def __getitem__(self, key, /):
-    ...
-
-  #= get method?
-
-  @abstractmethod
-  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
-    ...
-
-  __iter__ = __hash__ = None  # type: ignore
-
-
-class ComponentQueryResult(QueryResult):
-  @overload
-  def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  def __getitem__(
-    self, component_types: tuple[type[_T], ...], /
-  ) -> tuple[Iterator[_T], ...]: ...
-  @overload
-  def __getitem__(self, component_type: type[_T], /) -> Iterator[_T]: ...
-  def __getitem__(self, key, /):  # type: ignore
-    entities = self.entities
-    if isinstance(key, tuple):
-      return tuple(
-        (ent[comp_type] for ent in entities)
-        for comp_type in (key if key else self.types)
-      )
-    return (ent[key] for ent in entities)
-
-  @overload
-  def zip(self) -> Iterator[tuple[Any, ...]]: ...
-  @overload
-  def zip(self, *component_types: type[_T]) -> Iterator[tuple[_T, ...]]: ...
-  def zip(self, *component_types: type):  # type: ignore
-    if not component_types:
-      component_types = self.types
-    return (
-      tuple(ent[comp_type] for comp_type in component_types) for ent in self.entities
-    )
-
-
-class EntityQueryResult(QueryResult):
-  #@overload
-  #def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  def __getitem__(
-    self, component_types: tuple[type, ...], /
-  ) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  def __getitem__(
-    self, component_type: type[_T], /
-  ) -> tuple[Iterator[Entity], Iterator[_T]]: ...
-  def __getitem__(self, key, /):  # type: ignore
-    entities = self.entities
-    if isinstance(key, tuple):
-      types = key if key else self.types
-      return (
-        iter(entities), *[(ent[comp_type] for ent in entities) for comp_type in types]
-      )
-    return (iter(entities), (ent[key] for ent in entities))
-
-  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
-    if not component_types:
-      component_types = self.types
-    return (
-      (ent, *[ent[comp_type] for comp_type in component_types]) for ent in self.entities
-    )
-
-
-class IdQueryResult(QueryResult):
-  #@overload
-  #def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  def __getitem__(
-    self, component_types: tuple[type, ...], /
-  ) -> tuple[Iterator[Any], ...]: ...
-  @overload
-  def __getitem__(
-    self, component_type: type[_T], /
-  ) -> tuple[Iterator[EntityId], Iterator[_T]]: ...
-  def __getitem__(self, key, /):  # type: ignore
-    entities = self.entities
-    if isinstance(key, tuple):
-      types = key if key else self.types
-      return (
-        iter(self.ids), *[(ent[comp_type] for ent in entities) for comp_type in types]
-      )
-    return (iter(self.ids), (ent[key] for ent in entities))
-
-  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
-    if not component_types:
-      component_types = self.types
-    return (
-      (ent.id, *[ent[comp_type] for comp_type in component_types])
-      for ent in self.entities
-    )
+__all__ = [
+  'Query',
+  'QueryResult',
+  'ComponentQueryResult',
+  'EntityQueryResult',
+  'IdQueryResult',
+]
+
+from abc import ABC, abstractmethod
+from collections.abc import Iterator, KeysView, ValuesView
+from typing import Any, Callable, TypeVar, overload
+
+from pyriak.entity import Entity, EntityId
+
+
+_T = TypeVar('_T')
+
+
+class Query:
+  __slots__ = '_types', '_merge'
+
+  def __init__(
+    self, *component_types: type, merge: Callable[..., set] = set.intersection
+  ):
+    if not component_types:
+      raise TypeError('expected at least one component type')
+    self._types = component_types
+    self._merge = merge
+
+  @property
+  def types(self) -> tuple[type, ...]:
+    return self._types
+
+  @property
+  def merge(self):
+    return self._merge
+
+  def count(self, value: type, /):
+    return self._types.count(value)
+
+  def index(self, *args):
+    return self._types.index(*args)
+
+  def __getitem__(self, key, /):
+    return self._types[key]
+
+  def __iter__(self):
+    return iter(self._types)
+
+  def __len__(self):
+    return len(self._types)
+
+  def __contains__(self, obj: object, /):
+    return obj in self._types
+
+  def __eq__(self, other: object, /):
+    if not isinstance(other, Query):
+      return NotImplemented
+    return self._types == other._types and self._merge == other._merge
+
+  def __hash__(self):
+    return hash((self._types,self._merge))
+
+  def __repr__(self):
+    return (
+      f'{type(self).__name__}'
+      f'({", ".join(repr(t) for t in self._types)}, merge={self._merge!r})'
+    )
+
+
+class QueryResult(ABC):
+  __slots__ = '_entities', '_types', '_merge'
+
+  def __init__(
+    self, _entities: dict[EntityId, Entity],
+    _types: tuple[type, ...],
+    _merge: Callable[..., set], /
+  ):
+    self._entities = _entities
+    self._types = _types
+    self._merge = _merge
+
+  @property
+  def ids(self) -> KeysView[EntityId]:
+    return self._entities.keys()
+
+  @property
+  def entities(self) -> ValuesView[Entity]:
+    return self._entities.values()
+
+  @property
+  def types(self) -> tuple[type, ...]:
+    return self._types
+
+  @property
+  def merge(self) -> Callable[..., set]:
+    return self._merge
+
+  def query(self) -> Query:
+    """Return a new Query object that describes self."""
+    return Query(*self.types, merge=self.merge)
+
+  @overload
+  def __call__(self) -> Iterator[Any]: ...
+  @overload
+  def __call__(self, *component_types: type[_T]) -> Iterator[_T]: ...
+  def __call__(self, *component_types):
+    if not component_types:
+      component_types = self.types
+    return (comp for ent in self.entities for comp in ent(*component_types))
+
+  # group method
+
+  @overload
+  @abstractmethod
+  def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  @abstractmethod
+  def __getitem__(
+    self, component_types: tuple[type, ...], /
+  ) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  @abstractmethod
+  def __getitem__(
+    self, component_type: type[_T], /
+  ) -> Iterator[_T] | tuple[Iterator[Any], Iterator[_T]]: ...
+  @abstractmethod
+  def __getitem__(self, key, /):
+    ...
+
+  #= get method?
+
+  @abstractmethod
+  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
+    ...
+
+  __iter__ = __hash__ = None  # type: ignore
+
+
+class ComponentQueryResult(QueryResult):
+  @overload
+  def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  def __getitem__(
+    self, component_types: tuple[type[_T], ...], /
+  ) -> tuple[Iterator[_T], ...]: ...
+  @overload
+  def __getitem__(self, component_type: type[_T], /) -> Iterator[_T]: ...
+  def __getitem__(self, key, /):  # type: ignore
+    entities = self.entities
+    if isinstance(key, tuple):
+      return tuple(
+        (ent[comp_type] for ent in entities)
+        for comp_type in (key if key else self.types)
+      )
+    return (ent[key] for ent in entities)
+
+  @overload
+  def zip(self) -> Iterator[tuple[Any, ...]]: ...
+  @overload
+  def zip(self, *component_types: type[_T]) -> Iterator[tuple[_T, ...]]: ...
+  def zip(self, *component_types: type):  # type: ignore
+    if not component_types:
+      component_types = self.types
+    return (
+      tuple(ent[comp_type] for comp_type in component_types) for ent in self.entities
+    )
+
+
+class EntityQueryResult(QueryResult):
+  #@overload
+  #def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  def __getitem__(
+    self, component_types: tuple[type, ...], /
+  ) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  def __getitem__(
+    self, component_type: type[_T], /
+  ) -> tuple[Iterator[Entity], Iterator[_T]]: ...
+  def __getitem__(self, key, /):  # type: ignore
+    entities = self.entities
+    if isinstance(key, tuple):
+      types = key if key else self.types
+      return (
+        iter(entities), *[(ent[comp_type] for ent in entities) for comp_type in types]
+      )
+    return (iter(entities), (ent[key] for ent in entities))
+
+  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
+    if not component_types:
+      component_types = self.types
+    return (
+      (ent, *[ent[comp_type] for comp_type in component_types]) for ent in self.entities
+    )
+
+
+class IdQueryResult(QueryResult):
+  #@overload
+  #def __getitem__(self, key: tuple[()], /) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  def __getitem__(
+    self, component_types: tuple[type, ...], /
+  ) -> tuple[Iterator[Any], ...]: ...
+  @overload
+  def __getitem__(
+    self, component_type: type[_T], /
+  ) -> tuple[Iterator[EntityId], Iterator[_T]]: ...
+  def __getitem__(self, key, /):  # type: ignore
+    entities = self.entities
+    if isinstance(key, tuple):
+      types = key if key else self.types
+      return (
+        iter(self.ids), *[(ent[comp_type] for ent in entities) for comp_type in types]
+      )
+    return (iter(self.ids), (ent[key] for ent in entities))
+
+  def zip(self, *component_types: type) -> Iterator[tuple[Any, ...]]:
+    if not component_types:
+      component_types = self.types
+    return (
+      (ent.id, *[ent[comp_type] for comp_type in component_types])
+      for ent in self.entities
+    )
```

### Comparing `pyriak-0.2.0/src/pyriak/space.py` & `pyriak-0.3.0/src/pyriak/space.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,91 @@
-__all__ = ['Space']
-
-from collections import deque
-from collections.abc import Callable
-from typing import NoReturn, overload
-
-from pyriak import EventQueue, managers
-from pyriak.query import ComponentQueryResult, EntityQueryResult, IdQueryResult, Query
-
-
-class Space:
-  __slots__ = 'systems', 'entities', 'states', 'event_queue', '__weakref__'
-
-  def __init__(
-    self, *,
-    systems: managers.SystemManager | None = None,
-    entities: managers.EntityManager | None = None,
-    states: managers.StateManager | None = None,
-    event_queue: EventQueue | None = None
-  ):
-    """A new Space instance, which glues together the managers and the event queue.
-
-    By default, creates the EntityManager, StateManager, and SystemManager.
-    """
-    if systems is None:
-      systems = managers.SystemManager()
-    if entities is None:
-      entities = managers.EntityManager()
-    if states is None:
-      states = managers.StateManager()
-    if event_queue is None:
-      event_queue = deque()
-    self.systems = systems
-    systems.space = self
-    self.entities = entities
-    self.states = states
-    self.event_queue = event_queue
-    systems.event_queue = entities.event_queue = states.event_queue = event_queue
-
-  @overload
-  def query(self, query: Query, /) -> ComponentQueryResult: ...
-  @overload
-  def query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> ComponentQueryResult: ...
-  def query(self, /, *types, merge=None):
-    return self.entities.query(*types, merge=merge)
-
-  @overload
-  def entity_query(self, query: Query, /) -> EntityQueryResult: ...
-  @overload
-  def entity_query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def entity_query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> EntityQueryResult: ...
-  def entity_query(self, /, *types, merge=None):
-    return self.entities.entity_query(*types, merge=merge)
-
-  @overload
-  def id_query(self, query: Query, /) -> IdQueryResult: ...
-  @overload
-  def id_query(
-    self, /, *, merge: Callable[..., set] = set.intersection,
-  ) -> NoReturn: ...
-  @overload
-  def id_query(
-    self, /,
-    *component_types: type,
-    merge: Callable[..., set] = set.intersection,
-  ) -> IdQueryResult: ...
-  def id_query(self, /, *types, merge=None):
-    return self.entities.id_query(*types, merge=merge)
-
-  def process(self, event: object):
-    return self.systems.process(event, space=self)
-
-  def post(self, *events: object) -> None:
-    self.event_queue.extend(events)
-
-  def pump(self, events: int | None = None) -> int:
-    process_event = self.process
-    queue = self.event_queue
-    if isinstance(queue, deque):
-      pop = queue.popleft
-    else:
-      def pop():
-        return queue.pop(0)
-    i = -1
-    if events is None:
-      while queue:
-        i += 1
-        process_event(pop())
-    else:
-      for i in range(events):
-        if not queue:
-          return i
-        process_event(pop())
-    return i + 1
+__all__ = ['Space']
+
+from collections import deque
+from collections.abc import Callable
+from typing import overload
+
+from pyriak import EventQueue, managers
+from pyriak.query import ComponentQueryResult, EntityQueryResult, IdQueryResult, Query
+
+
+class Space:
+  __slots__ = 'systems', 'entities', 'states', 'event_queue', '__weakref__'
+
+  def __init__(
+    self, *,
+    systems: managers.SystemManager | None = None,
+    entities: managers.EntityManager | None = None,
+    states: managers.StateManager | None = None,
+    event_queue: EventQueue | None = None
+  ):
+    """A new Space instance, which glues together the managers and the event queue.
+
+    By default, creates the EntityManager, StateManager, and SystemManager.
+    """
+    if systems is None:
+      systems = managers.SystemManager()
+    if entities is None:
+      entities = managers.EntityManager()
+    if states is None:
+      states = managers.StateManager()
+    if event_queue is None:
+      event_queue = deque()
+    self.systems = systems
+    systems.space = self
+    self.entities = entities
+    self.states = states
+    self.event_queue = event_queue
+    systems.event_queue = entities.event_queue = states.event_queue = event_queue
+
+  @overload
+  def query(self, query: Query, /) -> ComponentQueryResult: ...
+  @overload
+  def query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> ComponentQueryResult: ...
+  def query(self, /, *types, merge=None):
+    return self.entities.query(*types, merge=merge)
+
+  @overload
+  def entity_query(self, query: Query, /) -> EntityQueryResult: ...
+  @overload
+  def entity_query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> EntityQueryResult: ...
+  def entity_query(self, /, *types, merge=None):
+    return self.entities.entity_query(*types, merge=merge)
+
+  @overload
+  def id_query(self, query: Query, /) -> IdQueryResult: ...
+  @overload
+  def id_query(
+    self, /, *component_types: type, merge: Callable[..., set] = set.intersection
+  ) -> IdQueryResult: ...
+  def id_query(self, /, *types, merge=None):
+    return self.entities.id_query(*types, merge=merge)
+
+  def process(self, event: object):
+    return self.systems.process(event, space=self)
+
+  def post(self, *events: object) -> None:
+    self.event_queue.extend(events)
+
+  def pump(self, events: int | None = None) -> int:
+    process_event = self.process
+    queue = self.event_queue
+    if isinstance(queue, deque):
+      pop = queue.popleft
+    else:
+      def pop():
+        return queue.pop(0)
+    i = -1
+    if events is None:
+      while queue:
+        i += 1
+        process_event(pop())
+    else:
+      for i in range(events):
+        if not queue:
+          return i
+        process_event(pop())
+    return i + 1
```

### Comparing `pyriak-0.2.0/PKG-INFO` & `pyriak-0.3.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriak
-Version: 0.2.0
+Version: 0.3.0
 Summary: A lightweight implementation of Entity Component System architecture
 License: MIT
 Author: aatle
 Author-email: 168398276+aatle@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,15 +18,18 @@
 # pyriak
 A lightweight implementation of Entity Component System architecture for Python.
 
 (Originally created August 2, 2022.)
 
 
 ## Concepts
-
+Object oriented programming is used for many projects.
+In larger, more complex projects, it can have some shortcomings.
+The inheritance hierarchies can become messy and inflexible,
+forcing the base classes to grow in size when code reuse is needed.
 
 
 ## Usage
 
 
 
 ### Entity creation
@@ -40,15 +43,15 @@
   components.Player(),
   components.CameraFocus(),
   components.Sprite(),
 )
 ```
 A listening system can extend a created entity.
 ```py
-@bind(ComponentAdded, 200, RocketBooster):
+@bind(ComponentAdded, 200, RocketBooster)
 def add_rocket_exhaust(space, event):
   event.entity.add(ParticleEmitter(rocket_particles))
 ```
 
 Often, multiple systems will need to create a certain set of components that are not
 related enough to put under a single component, but common enough to necessitate code reuse.
 A dedicated module can provide functions that
```

