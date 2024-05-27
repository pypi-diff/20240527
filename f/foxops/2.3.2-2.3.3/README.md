# Comparing `tmp/foxops-2.3.2.tar.gz` & `tmp/foxops-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxops-2.3.2.tar", max compression
+gzip compressed data, was "foxops-2.3.3.tar", max compression
```

## Comparing `foxops-2.3.2.tar` & `foxops-2.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11358 2024-03-01 12:39:28.587209 foxops-2.3.2/LICENSE
--rw-r--r--   0        0        0     1467 2024-03-01 12:39:28.587209 foxops-2.3.2/README.md
--rw-r--r--   0        0        0     2245 2024-03-01 12:39:36.567177 foxops-2.3.2/pyproject.toml
--rw-r--r--   0        0        0       72 2024-03-01 12:39:28.603209 foxops-2.3.2/src/foxops/__init__.py
--rw-r--r--   0        0        0     3143 2024-03-01 12:39:28.603209 foxops-2.3.2/src/foxops/__main__.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.603209 foxops-2.3.2/src/foxops/database/__init__.py
--rw-r--r--   0        0        0      697 2024-03-01 12:39:28.603209 foxops-2.3.2/src/foxops/database/engine.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.603209 foxops-2.3.2/src/foxops/database/repositories/__init__.py
--rw-r--r--   0        0        0    13639 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/repositories/change.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/repositories/incarnation/__init__.py
--rw-r--r--   0        0        0      111 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/repositories/incarnation/errors.py
--rw-r--r--   0        0        0      230 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/repositories/incarnation/model.py
--rw-r--r--   0        0        0     2559 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/repositories/incarnation/repository.py
--rw-r--r--   0        0        0     1469 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/database/schema.py
--rw-r--r--   0        0        0     4567 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/dependencies.py
--rw-r--r--   0        0        0      693 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/__init__.py
--rw-r--r--   0        0        0    10241 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/__main__.py
--rw-r--r--   0        0        0      481 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/custom_filters.py
--rw-r--r--   0        0        0      904 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/errors.py
--rw-r--r--   0        0        0     2541 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/initialization.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/models/__init__.py
--rw-r--r--   0        0        0     2135 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/models/incarnation_state.py
--rw-r--r--   0        0        0     5130 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/models/template_config.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/patching/__init__.py
--rw-r--r--   0        0        0     8976 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/patching/git_diff_patch.py
--rw-r--r--   0        0        0     9569 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/rendering.py
--rw-r--r--   0        0        0     7405 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/engine/update.py
--rw-r--r--   0        0        0     1009 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/error_handlers.py
--rw-r--r--   0        0        0     1697 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/errors.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/external/__init__.py
--rw-r--r--   0        0        0     8578 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/external/git.py
--rw-r--r--   0        0        0      121 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/hosters/__init__.py
--rw-r--r--   0        0        0    20618 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/hosters/gitlab.py
--rw-r--r--   0        0        0     9615 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/hosters/local.py
--rw-r--r--   0        0        0     2295 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/hosters/types.py
--rw-r--r--   0        0        0     2711 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/logger.py
--rw-r--r--   0        0        0      988 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/middlewares.py
--rw-r--r--   0        0        0      167 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/models/__init__.py
--rw-r--r--   0        0        0      618 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/models/change.py
--rw-r--r--   0        0        0       77 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/models/errors.py
--rw-r--r--   0        0        0     1270 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/models/incarnation.py
--rw-r--r--   0        0        0      655 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/openapi.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/__init__.py
--rw-r--r--   0        0        0      407 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/auth.py
--rw-r--r--   0        0        0     5396 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/changes.py
--rw-r--r--   0        0        0    15485 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/incarnations.py
--rw-r--r--   0        0        0      331 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/not_found.py
--rw-r--r--   0        0        0      351 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/routers/version.py
--rw-r--r--   0        0        0        0 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/services/__init__.py
--rw-r--r--   0        0        0    31556 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/services/change.py
--rw-r--r--   0        0        0     1600 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/services/incarnation.py
--rw-r--r--   0        0        0     1225 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/settings.py
--rw-r--r--   0        0        0     2201 2024-03-01 12:39:28.607209 foxops-2.3.2/src/foxops/utils.py
--rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 foxops-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-27 19:30:13.849183 foxops-2.3.3/LICENSE
+-rw-r--r--   0        0        0     1467 2024-05-27 19:30:13.849183 foxops-2.3.3/README.md
+-rw-r--r--   0        0        0     2245 2024-05-27 19:30:23.109311 foxops-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/__init__.py
+-rw-r--r--   0        0        0     3143 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/__init__.py
+-rw-r--r--   0        0        0      697 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/engine.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/__init__.py
+-rw-r--r--   0        0        0    13639 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/change.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/incarnation/__init__.py
+-rw-r--r--   0        0        0      111 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/incarnation/errors.py
+-rw-r--r--   0        0        0      230 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/incarnation/model.py
+-rw-r--r--   0        0        0     2559 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/repositories/incarnation/repository.py
+-rw-r--r--   0        0        0     1469 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/database/schema.py
+-rw-r--r--   0        0        0     4567 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/dependencies.py
+-rw-r--r--   0        0        0      693 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/__init__.py
+-rw-r--r--   0        0        0    10241 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/__main__.py
+-rw-r--r--   0        0        0      481 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/custom_filters.py
+-rw-r--r--   0        0        0      904 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/errors.py
+-rw-r--r--   0        0        0     2541 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/initialization.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/models/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/models/incarnation_state.py
+-rw-r--r--   0        0        0     5130 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/models/template_config.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/patching/__init__.py
+-rw-r--r--   0        0        0     8976 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/patching/git_diff_patch.py
+-rw-r--r--   0        0        0     9569 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/rendering.py
+-rw-r--r--   0        0        0     7405 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/engine/update.py
+-rw-r--r--   0        0        0     1009 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/error_handlers.py
+-rw-r--r--   0        0        0     1697 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/errors.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/external/__init__.py
+-rw-r--r--   0        0        0     8578 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/external/git.py
+-rw-r--r--   0        0        0      121 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/hosters/__init__.py
+-rw-r--r--   0        0        0    20618 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/hosters/gitlab.py
+-rw-r--r--   0        0        0     9615 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/hosters/local.py
+-rw-r--r--   0        0        0     2295 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/hosters/types.py
+-rw-r--r--   0        0        0     2711 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/logger.py
+-rw-r--r--   0        0        0      988 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/middlewares.py
+-rw-r--r--   0        0        0      167 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/models/__init__.py
+-rw-r--r--   0        0        0      618 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/models/change.py
+-rw-r--r--   0        0        0       77 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/models/errors.py
+-rw-r--r--   0        0        0     1270 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/models/incarnation.py
+-rw-r--r--   0        0        0      655 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/openapi.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/__init__.py
+-rw-r--r--   0        0        0      407 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/auth.py
+-rw-r--r--   0        0        0     5552 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/changes.py
+-rw-r--r--   0        0        0    15485 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/incarnations.py
+-rw-r--r--   0        0        0      331 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/not_found.py
+-rw-r--r--   0        0        0      351 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/routers/version.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/services/__init__.py
+-rw-r--r--   0        0        0    31811 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/services/change.py
+-rw-r--r--   0        0        0     1600 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/services/incarnation.py
+-rw-r--r--   0        0        0     1225 2024-05-27 19:30:13.865183 foxops-2.3.3/src/foxops/settings.py
+-rw-r--r--   0        0        0     2201 2024-05-27 19:30:13.869183 foxops-2.3.3/src/foxops/utils.py
+-rw-r--r--   0        0        0     2607 1970-01-01 00:00:00.000000 foxops-2.3.3/PKG-INFO
```

### Comparing `foxops-2.3.2/LICENSE` & `foxops-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/README.md` & `foxops-2.3.3/README.md`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/pyproject.toml` & `foxops-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "foxops"
 # managed by poetry-dynamic-versioning, do not change.
-version = "2.3.2"
+version = "2.3.3"
 description = "Foxops 🦊"
 license = "Apache-2.0"
 authors = [
     "Alexander Hungenberg <alexander.hungenberg@roche.com>",
     "Timo Furrer <timo.furrer@roche.com>",
 ]
 readme = "README.md"
```

### Comparing `foxops-2.3.2/src/foxops/__main__.py` & `foxops-2.3.3/src/foxops/__main__.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/database/engine.py` & `foxops-2.3.3/src/foxops/database/engine.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/database/repositories/change.py` & `foxops-2.3.3/src/foxops/database/repositories/change.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/database/repositories/incarnation/repository.py` & `foxops-2.3.3/src/foxops/database/repositories/incarnation/repository.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/database/schema.py` & `foxops-2.3.3/src/foxops/database/schema.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/dependencies.py` & `foxops-2.3.3/src/foxops/dependencies.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/__init__.py` & `foxops-2.3.3/src/foxops/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/__main__.py` & `foxops-2.3.3/src/foxops/engine/__main__.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/errors.py` & `foxops-2.3.3/src/foxops/engine/errors.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/initialization.py` & `foxops-2.3.3/src/foxops/engine/initialization.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/models/incarnation_state.py` & `foxops-2.3.3/src/foxops/engine/models/incarnation_state.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/models/template_config.py` & `foxops-2.3.3/src/foxops/engine/models/template_config.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/patching/git_diff_patch.py` & `foxops-2.3.3/src/foxops/engine/patching/git_diff_patch.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/rendering.py` & `foxops-2.3.3/src/foxops/engine/rendering.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/engine/update.py` & `foxops-2.3.3/src/foxops/engine/update.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/error_handlers.py` & `foxops-2.3.3/src/foxops/error_handlers.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/errors.py` & `foxops-2.3.3/src/foxops/errors.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/external/git.py` & `foxops-2.3.3/src/foxops/external/git.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/hosters/gitlab.py` & `foxops-2.3.3/src/foxops/hosters/gitlab.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/hosters/local.py` & `foxops-2.3.3/src/foxops/hosters/local.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/hosters/types.py` & `foxops-2.3.3/src/foxops/hosters/types.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/logger.py` & `foxops-2.3.3/src/foxops/logger.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/middlewares.py` & `foxops-2.3.3/src/foxops/middlewares.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/models/change.py` & `foxops-2.3.3/src/foxops/models/change.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/models/incarnation.py` & `foxops-2.3.3/src/foxops/models/incarnation.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/openapi.py` & `foxops-2.3.3/src/foxops/openapi.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/routers/changes.py` & `foxops-2.3.3/src/foxops/routers/changes.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,33 +12,38 @@
 from foxops.hosters.types import MergeRequestStatus
 from foxops.models.change import Change, ChangeWithMergeRequest
 from foxops.services.change import CannotRepairChangeException, ChangeService
 
 router = APIRouter()
 
 
-async def get_change(
+async def get_change_id(
     incarnation_id: Annotated[int, Path()],
     revision: Annotated[int, Path(description="Change revision within the given incarnation")],
     change_service: Annotated[ChangeService, Depends(get_change_service)],
-) -> Change | ChangeWithMergeRequest:
+) -> int:
     try:
-        change_id = await change_service.get_change_id_by_revision(incarnation_id, revision)
-
-        match (change_type := await change_service.get_change_type(change_id)):
-            case DatabaseChangeType.MERGE_REQUEST:
-                return await change_service.get_change_with_merge_request(change_id)
-            case DatabaseChangeType.DIRECT:
-                return await change_service.get_change(change_id)
-            case _:
-                raise NotImplementedError(f"Unknown change type {change_type}")
+        return await change_service.get_change_id_by_revision(incarnation_id, revision)
     except ChangeNotFoundError:
         raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail="Change not found")
 
 
+async def get_change(
+    change_id: Annotated[int, Depends(get_change_id)],
+    change_service: Annotated[ChangeService, Depends(get_change_service)],
+) -> Change | ChangeWithMergeRequest:
+    match (change_type := await change_service.get_change_type(change_id)):
+        case DatabaseChangeType.MERGE_REQUEST:
+            return await change_service.get_change_with_merge_request(change_id)
+        case DatabaseChangeType.DIRECT:
+            return await change_service.get_change(change_id)
+        case _:
+            raise NotImplementedError(f"Unknown change type {change_type}")
+
+
 class CreateChangeType(enum.Enum):
     DIRECT = "direct"
     MERGE_REQUEST_MANUAL = "merge_request_manual"
     MERGE_REQUEST_AUTOMERGE = "merge_request_automerge"
 
 
 class CreateChangeRequest(BaseModel):
@@ -138,14 +143,14 @@
     "incarnation repository failed, for example because the hoster was down.",
     responses={
         status.HTTP_404_NOT_FOUND: {"description": "Change not found"},
         status.HTTP_422_UNPROCESSABLE_ENTITY: {"description": "The change cannot be repaired automatically"},
     },
 )
 async def fix_incomplete_change(
-    change: Change = Depends(get_change),
-    change_service: ChangeService = Depends(get_change_service),
+    change_id: Annotated[int, Depends(get_change_id)],
+    change_service: Annotated[ChangeService, Depends(get_change_service)],
 ):
     try:
-        await change_service.update_incomplete_change(change.id)
+        await change_service.update_incomplete_change(change_id)
     except CannotRepairChangeException as e:
         raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
```

### Comparing `foxops-2.3.2/src/foxops/routers/incarnations.py` & `foxops-2.3.3/src/foxops/routers/incarnations.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/services/change.py` & `foxops-2.3.3/src/foxops/services/change.py`

 * *Files 2% similar despite different names*

```diff
@@ -445,15 +445,15 @@
         Returns a change object for the given change ID.
         """
 
         change = await self._change_repository.get_change(change_id)
         if not change.commit_pushed:
             raise IncompleteChange(
                 "the given change is in an incomplete state (commit_pushed=False). "
-                "Try calling update_incomplete_change(change_id) first."
+                f"Try 'POST /api/incarnations/{change.incarnation_id}/changes/{change.revision}/fix'"
             )
 
         return Change(
             id=change.id,
             incarnation_id=change.incarnation_id,
             revision=change.revision,
             requested_version_hash=change.requested_version_hash,
@@ -468,16 +468,19 @@
         change_basic = await self.get_change(change_id)
 
         change_in_db = await self._change_repository.get_change(change_id)
         incarnation_in_db = await self._incarnation_repository.get_by_id(change_in_db.incarnation_id)
 
         if change_in_db.type != ChangeType.MERGE_REQUEST:
             raise ValueError(f"Change {change_id} is not a merge request change.")
-        assert change_in_db.merge_request_id is not None
-        assert change_in_db.merge_request_branch_name is not None
+        if change_in_db.merge_request_id is None or change_in_db.merge_request_branch_name is None:
+            raise IncompleteChange(
+                "the given change is in an incomplete state (MR ID/Branch = null). "
+                f"Try 'POST /api/incarnations/{change_in_db.incarnation_id}/changes/{change_in_db.revision}/fix'"
+            )
 
         status = await self._hoster.get_merge_request_status(
             incarnation_repository=incarnation_in_db.incarnation_repository,
             merge_request_id=change_in_db.merge_request_id,
         )
 
         return ChangeWithMergeRequest(
```

### Comparing `foxops-2.3.2/src/foxops/services/incarnation.py` & `foxops-2.3.3/src/foxops/services/incarnation.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/settings.py` & `foxops-2.3.3/src/foxops/settings.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/src/foxops/utils.py` & `foxops-2.3.3/src/foxops/utils.py`

 * *Files identical despite different names*

### Comparing `foxops-2.3.2/PKG-INFO` & `foxops-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxops
-Version: 2.3.2
+Version: 2.3.3
 Summary: Foxops 🦊
 License: Apache-2.0
 Author: Alexander Hungenberg
 Author-email: alexander.hungenberg@roche.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

