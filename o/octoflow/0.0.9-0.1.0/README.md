# Comparing `tmp/octoflow-0.0.9.tar.gz` & `tmp/octoflow-0.1.0.tar.gz`

## Comparing `octoflow-0.0.9.tar` & `octoflow-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,37 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/__init__.py
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/logging.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/__init__.py
--rw-r--r--   0        0        0     9698 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/base.py
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/client.py
--rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/experiment.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/package.py
--rw-r--r--   0        0        0    12973 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/run.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/value.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/value_utils.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/variable.py
--rw-r--r--   0        0        0     5371 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/artifact/__init__.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/core/artifact/handler.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/__init__.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/json_.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/pandas_.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/pickle_.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/safetensors_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/torch_.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/plugins/artifacts/transformers_.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/utils/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 octoflow-0.0.9/octoflow/utils/mutation.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 octoflow-0.0.9/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.0.9/AUTHORS.md
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.0.9/LICENSE
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.0.9/README.md
--rw-r--r--   0        0        0     8110 2020-02-02 00:00:00.000000 octoflow-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 octoflow-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/config.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/constants.py
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/core.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/exceptions.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/logging.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/plugin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/typing.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/__init__.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/base.py
+-rw-r--r--   0        0        0     5384 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/dataclass.py
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/dataset.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/expression.py
+-rw-r--r--   0        0        0     8824 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/loaders.py
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/metadata.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/sampler.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/schema.py
+-rw-r--r--   0        0        0    10791 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/data/types.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/tracking/__init__.py
+-rw-r--r--   0        0        0    12425 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/tracking/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/tracking/artifact/__init__.py
+-rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/tracking/artifact/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/__init__.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/cache.py
+-rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/collections.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/config.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/escape.py
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/func.py
+-rw-r--r--   0        0        0    11582 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/hashing.py
+-rw-r--r--   0        0        0     4234 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/objects.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 octoflow-0.1.0/octoflow/utils/rsync.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 octoflow-0.1.0/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 octoflow-0.1.0/AUTHORS.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 octoflow-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 octoflow-0.1.0/README.md
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 octoflow-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 octoflow-0.1.0/PKG-INFO
```

### Comparing `octoflow-0.0.9/octoflow/logging.py` & `octoflow-0.1.0/octoflow/logging.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,87 @@
 import logging
-from typing import Optional, Sequence, Union
+from typing import Optional, Union
 
-CONSOLE_HANDLER = "console"
-
-PACKAGE_NAME = next(iter(__name__.split(".")))
-DEFAULT_LOGGING_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
-DEFAULT_LOGGING_HANDLERS = {
-    CONSOLE_HANDLER,
-}
-
-
-class LoggingFactory:
-    def __init__(
-        self,
-        name: Optional[str] = None,
-        level: Union[int, str] = logging.INFO,
-        formatter: str = DEFAULT_LOGGING_FORMAT,
-        handlers: Sequence[str] = DEFAULT_LOGGING_HANDLERS,
-    ) -> None:
-        logger = logging.getLogger(name)
+try:
+    from rich.logging import RichHandler
+except ImportError:
+    RichHandler = None
+
+__all__ = [
+    "get_logger",
+    "set_level",
+]
+
+logger: logging.Logger
+
+CRITICAL = logging.CRITICAL
+FATAL = CRITICAL
+ERROR = logging.ERROR
+WARNING = logging.WARNING
+WARN = WARNING
+INFO = logging.INFO
+DEBUG = logging.DEBUG
+NOTSET = logging.NOTSET
+
+
+def get_logger(
+    name: Optional[str] = None,
+    level: Union[int, str, None] = None,
+    formatter: Optional[str] = None,
+) -> logging.Logger:
+    """
+    Get a logger with the given name and level.
+
+    Parameters
+    ----------
+    name : str, optional
+        Name of the logger.
+    level : int or str, optional
+        Logging level.
+    formatter : str, optional
+        Formatter string.
+    handlers : Sequence[str], optional
+        Sequence of handlers to use.
+
+    Returns
+    -------
+    logging.Logger
+        Logger instance.
+    """
+    logger = logging.getLogger(name)
+    if level is not None:
         logger.setLevel(level)
-        if CONSOLE_HANDLER in handlers:
-            stream_handler = logging.StreamHandler()
-            stream_handler.setLevel(logging.DEBUG)
-            if not isinstance(formatter, logging.Formatter):
-                # Create a formatter
-                formatter = logging.Formatter(formatter)
-            # add it to the handlers
-            stream_handler.setFormatter(formatter)
-            # Add the handlers to the logger
-            logger.addHandler(stream_handler)
-        self.base_logger = logger
-
-    def __call__(self, name: Optional[str] = None) -> logging.Logger:
-        return logging.getLogger(name)
-
-
-get_logger = LoggingFactory(PACKAGE_NAME)
+    if RichHandler is None:
+        handler = logging.StreamHandler()
+    else:
+        handler = RichHandler(
+            show_time=False,
+            show_level=False,
+            show_path=False,
+        )
+    handler.setLevel(logging.DEBUG)
+    if not isinstance(formatter, logging.Formatter):
+        # Create a formatter
+        formatter = logging.Formatter(formatter)
+    # add it to the handlers
+    handler.setFormatter(formatter)
+    # Add the handlers to the logger
+    logger.addHandler(handler)
+    return logger
+
+
+def set_level(level: Union[int, str], logger: Optional[logging.Logger] = None):
+    """
+    Set the logging level of the logger.
+
+    Parameters
+    ----------
+    logger : logging.Logger
+        Logger instance.
+    level : int or str
+        Logging level.
+    """
+    if logger is None:
+        logger = globals().get("logger", logging.getLogger())
+    if isinstance(level, str):
+        level = logging.getLevelName(level)
+    logger.setLevel(level)
```

### Comparing `octoflow-0.0.9/octoflow/core/artifact/__init__.py` & `octoflow-0.1.0/octoflow/tracking/artifact/handler.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,192 +1,175 @@
 from __future__ import annotations
 
-from datetime import datetime
-from distutils.version import Version
+import abc
+import shutil
 from pathlib import Path
-from typing import Any, Type, Union
+from typing import Any, Dict, List, Type, Union
 
-from sqlalchemy import (
-    DateTime,
-    ForeignKey,
-    Index,
-    Integer,
-    String,
-    text,
-    types,
-)
-from sqlalchemy.orm import Mapped, mapped_column
-
-from octoflow.core.artifact import handler
-from octoflow.core.artifact.handler import (
-    ArtifactHandler,
-    get_handler_type,
-    get_handler_type_by_object,
-    list_handler_types,
-)
-from octoflow.core.base import Base
-
-__all__ = [
-    "Artifact",
-    "handler",
-    "get_handler_type",
-    "get_handler_type_by_object",
-    "list_handler_types",
-]
-
-
-class ArtifactHandlerType(types.TypeDecorator):
-    """A SQLAlchemy type decorator for ArtifactHandler."""
-
-    impl = types.Unicode
-
-    cache_ok = True
-
-    def process_bind_param(self, value: Type[ArtifactHandler], dialect) -> str:  # noqa: PLR6301
-        """Gets the name from the handler type."""
-        if not issubclass(value, ArtifactHandler):
-            msg = f"'{value}' is not a subclass of 'ArtifactHandler'"
-            raise ValueError(msg)
-        return value.name
+from octoflow.data.metadata import Metadata
 
-    def process_result_value(self, value: str, dialect) -> Type[ArtifactHandler]:  # noqa: PLR6301
-        """Gets the handler type for the given name."""
-        return get_handler_type(value)
-
-
-class VersionType(types.TypeDecorator):
-    """A SQLAlchemy type decorator for Version."""
-
-    impl = types.Unicode
-
-    cache_ok = True
-
-    def process_bind_param(self, value: Union[str, Version], dialect) -> str:  # noqa: PLR6301
-        """Converts the value to a string."""
-        if not isinstance(value, Version):
-            value = Version(value)
-        return str(value)
-
-    def process_result_value(self, value: str, dialect) -> Version:  # noqa: PLR6301
-        """Converts the value to a Version."""
-        return Version(value)
-
-
-class Artifact(Base):
-    __tablename__ = "artifact"
-    id: Mapped[int] = mapped_column(Integer, primary_key=True)
-    run_id: Mapped[int] = mapped_column(Integer, ForeignKey("run.id"), nullable=False)
-    key: Mapped[str] = mapped_column(String(255), nullable=False)
-    version: Mapped[Version] = mapped_column(String(128), nullable=False, default="0.0.0")
-    handler_type: Mapped[Type[ArtifactHandler]] = mapped_column(ArtifactHandlerType, nullable=False)
-    timestamp: Mapped[datetime] = mapped_column(DateTime, nullable=False, default=datetime.utcnow)
-
-    __table_args__ = (
-        Index(
-            "ix_artifact_run_id_key",
-            "run_id",
-            "key",
-            "version",
-            unique=True,
-        ),
-    )
+_handler_types: Dict[str, Type[ArtifactHandler]] = {}
+
+METADATA_FILENAME = "metadata.json"
+TYPE_FIELD = "type"
+
+
+def get_handler_type(name: str) -> Type[ArtifactHandler]:
+    try:
+        return _handler_types[name]
+    except KeyError:
+        msg = f"handler '{name}' not found"
+        raise ValueError(msg) from None
 
-    @property
-    def path(self) -> Path:
-        if hasattr(self, "_path") and self._path is not None:
-            return self._path
-        with self.session() as session:
-            query = text("SELECT r.experiment_id, r.uuid FROM run as r WHERE r.id = :run_id")
-            exper_id, run_uuid = session.execute(query, {"run_id": self.run_id}).one()
-            query = text("SELECT e.artifact_uri FROM experiment as e WHERE e.id = :experiment_id")
-            arifact_uri = session.execute(query, {"experiment_id": exper_id}).scalar()
-            path: Path = Path(arifact_uri) / run_uuid / f"{self.key}-v{self.version}"
-            if not path.exists():
-                path.mkdir(parents=True)
-            self._path = path
-        return self._path
+
+def get_handler_type_by_object(obj: Any) -> Type[ArtifactHandler]:
+    handler = None
+    for handler_type in _handler_types.values():
+        if not handler_type.can_handle(obj):
+            continue
+        if handler is not None:
+            msg = f"multiple handlers found for '{type(obj).__name__}'"
+            raise ValueError(msg)
+        handler = handler_type
+    if handler is not None:
+        return handler
+    # if we get here, we didn't find an appropriate handler for the object
+    msg = f"'{obj.__class__.__name__}' has no handler"
+    raise ValueError(msg)
+
+
+def get_handler_type_by_path(path: Union[str, Path]) -> Type[ArtifactHandler]:
+    metadata = Metadata(Path(path) / METADATA_FILENAME)
+    if not path.exists():
+        msg = f"artifact without metadata at '{path}'"
+        raise FileNotFoundError(msg)
+    if TYPE_FIELD not in metadata:
+        msg = f"artifact metadata missing 'type' at '{path}'"
+        raise KeyError(msg)
+    handler_type_str = metadata[TYPE_FIELD]
+    return get_handler_type(handler_type_str)
+
+
+def list_handler_types() -> List[str]:
+    return list(_handler_types.keys())
+
+
+class ArtifactHandlerType(abc.ABCMeta):
+    def __new__(cls, *args, **kwargs):
+        handler_cls = super().__new__(cls, *args)
+        base = args[1]  # base class
+        if len(base) > 0:
+            handler_cls._handler_type_name = kwargs.get("name", args[0])
+            _handler_types[handler_cls._handler_type_name] = handler_cls
+        return handler_cls
 
     @property
-    def handler(self) -> ArtifactHandler:
-        """Return the handler for this artifact."""
-        if not hasattr(self, "_handler") or self._handler is None:
-            self._handler = self.handler_type(
-                self.path,
+    def name(cls) -> str:
+        return cls._handler_type_name
+
+
+class ArtifactHandler(metaclass=ArtifactHandlerType):
+    def __init__(self, path: Union[str, Path]) -> None:
+        """
+        Abstract base class for artifact handlers.
+
+        Parameters
+        ----------
+        path : str
+            The path to the artifact
+        """
+        super().__init__()
+        path = Path(path)
+        (path / "data").mkdir(parents=True, exist_ok=True)
+        self.metadata = Metadata(path / METADATA_FILENAME)
+        if TYPE_FIELD in self.metadata:
+            if self.metadata[TYPE_FIELD] == self.__class__.name:
+                return
+            msg = (
+                f"metadata type '{self.metadata[TYPE_FIELD]}' does "
+                f"not match handler type '{self.__class__.name}'"
             )
-        return self._handler
+            raise ValueError(msg)
+        else:
+            self.metadata[TYPE_FIELD] = self.__class__.name
 
+    @property
+    def path(self) -> Path:
+        return self.metadata._path.parent / "data"
+
+    @abc.abstractmethod
     def load(self) -> Any:
         """
-        Load the artifact.
+        Load the artifact from the path.
 
         Returns
         -------
         Any
             The loaded artifact.
         """
-        return self.handler.load()
+        raise NotImplementedError
 
-    def save(self, obj: Any, **kwargs) -> None:
+    @abc.abstractmethod
+    def save(self, obj: Any, *args, **kwargs):
         """
-        Save an object to the artifact.
+        Save the given artifact to the path.
 
         Parameters
         ----------
         obj : Any
-            The object to save.
+            The artifact to save.
+        args : tuple
+            Additional positional arguments.
         kwargs : dict
             Additional keyword arguments.
+
+        Returns
+        -------
+        None
         """
-        self.handler.save(obj, **kwargs)
+        raise NotImplementedError
 
-    def exists(self) -> bool:
+    @classmethod
+    @abc.abstractmethod
+    def can_handle(cls, obj: object) -> bool:
         """
-        Return True if the artifact exists.
+        Return True if this handler can handle the given object type.
+
+        Parameters
+        ----------
+        obj : object
+            The object to check.
 
         Returns
         -------
         bool
-            True if the artifact exists.
+            True if this handler can handle the given object type.
         """
-        return self.handler.exists()
+        raise NotImplementedError
 
-    def unlink(self) -> None:
+    def exists(self) -> bool:
         """
-        Unlink/delete the artifact.
-
-        Notes
-        -----
-        This will only delete the artifact, not the database record.
+        Return True if the artifact exists.
 
         Returns
         -------
-        None
-            None
+        bool
+            True if the artifact exists.
         """
-        self.handler.unlink()
+        raise NotImplementedError
 
-    def delete(self, unlink: bool = False) -> None:
+    def unlink(self):
         """
-        Delete the artifact.
-
-        Parameters
-        ----------
-        unlink : bool, optional
-            If True, unlink the artifact, by default False.
-
-        Notes
-        -----
-        This will delete the database record and unlink the artifact if `unlink` is True.
+        Unlink/delete the artifact.
 
         Returns
         -------
         None
             None
         """
-        try:
-            # delete the database record
-            super().delete()
-            if unlink:
-                # unlink the artifact
-                self.handler.unlink()
-        except ValueError as ex:
-            raise ex
+        path = Path(self.path)
+        if not path.exists():
+            return
+        if path.is_dir():
+            shutil.rmtree(path)
+        else:
+            path.unlink()
```

### Comparing `octoflow-0.0.9/octoflow/utils/mutation.py` & `octoflow-0.1.0/octoflow/utils/collections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,46 @@
 from __future__ import annotations
 
 import functools
 import weakref
 from collections import defaultdict
-from typing import Dict, Generator, Iterable, MutableMapping, MutableSequence, Optional, Set, TypeVar
+from typing import (
+    Any,
+    Dict,
+    Generator,
+    Iterable,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Optional,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+)
 from typing import MutableSet as MutableSetType
 
+__all__ = [
+    "flatten",
+]
+
+
+__all__ = [
+    "MutableCollection",
+    "MutableDict",
+    "MutableList",
+    "MutableSet",
+]
+
 K, V = TypeVar("K"), TypeVar("V")
 
 
 class EventTarget:
     def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+        super(EventTarget, self).__init__()
         self._event_listeners: Dict[str, Set[callable]] = defaultdict(set)
 
     def add_event_listener(self, type: str, listener: callable):
         self._event_listeners[type].add(listener)
 
     def remove_event_listener(self, type: str, listener: callable):
         self._event_listeners[type].remove(listener)
@@ -140,7 +165,48 @@
         yield from self._data
 
     def __len__(self) -> int:
         return len(self._data)
 
     def __repr__(self) -> str:
         return repr(self._data)
+
+
+def flatten(
+    data: Dict[str, Any],
+    *,
+    separator: str = ".",
+    parent_key: Optional[str] = None,
+) -> Dict[Union[str, Tuple[str]], Any]:
+    """
+    Flatten a nested dictionary.
+
+    Parameters
+    ----------
+    data : Dict[str, Any]
+        The nested dictionary to flatten.
+    separator : str, optional
+        The separator, by default "."
+    parent_key : Optional[str], optional
+        The parent key, by default None
+
+    Returns
+    -------
+    Dict[str | tuple[str], Any]
+        The flattened dictionary.
+    """
+    if separator is not None and parent_key is None:
+        parent_key = ""
+    items = []
+    for key, value in data.items():
+        # escape dots
+        if separator is None:
+            new_key = (parent_key, key) if parent_key is not None else key
+        else:
+            new_key = parent_key + separator + key if parent_key else key
+        if isinstance(value, Mapping):
+            items.extend(
+                flatten(value, parent_key=new_key, separator=separator).items()
+            )
+        else:
+            items.append((new_key, value))
+    return dict(items)
```

### Comparing `octoflow-0.0.9/.gitignore` & `octoflow-0.1.0/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -156,7 +156,10 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 .DS_Store
 logs/
+scratch/
+examples/data.jsonl
+examples/project/
```

### Comparing `octoflow-0.0.9/LICENSE` & `octoflow-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.9/README.md` & `octoflow-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `octoflow-0.0.9/pyproject.toml` & `octoflow-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,27 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 # direct dependencies of this package, installed when users `pip install octoflow` later.
 dependencies = [
+    "octoflow-plugins",
+    "sqlalchemy",
+    "cloudpickle",
+    # for fast hashing
+    "xxhash",
+    # for pickling
+    "dill",
+    "omegaconf>=2.3.0",
+    "pyarrow>=16.0.0",
+    "pandas>=2.2.2",
+    "polars>=0.20.22",
+    "tqdm>=4.66.2",
+    "filelock>=3.13.4",
     # "typer",
     # "numpy",
     # "matplotlib",
     # "seaborn",
 ]
 dynamic = ["version"]
 
@@ -106,15 +119,15 @@
 #     "if __name__ == .__main__.:",
 #     "if TYPE_CHECKING:",
 # ]
 
 [tool.ruff]
 extend-include = ["*.ipynb"]
 target-version = "py38"
-line-length = 120
+line-length = 79
 preview = true # preview features & checks, use with caution
 extend-select = [ # features in preview
     "W292", # missing-newline-at-end-of-file
 ]
 include = ["src/**/*.py", "src/**/*.pyi", "tests/**/*.py", "tests/**/*.pyi"]
 select = [
     "A",
@@ -218,52 +231,52 @@
 #     "ruff",
 # ]
 # [tool.hatch.envs.default.scripts]
 # cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=src/octoflow --cov=tests {args}"
 # no-cov = "cov --no-cov {args}"
 # debug = "cov --no-cov -s --pdb --pdbcls=IPython.core.debugger:Pdb {args}"
 
-# # Docs environment
-# [tool.hatch.envs.docs]
-# dependencies = [
-#     "mkdocs~=1.4.0",
-#     "mkdocs-material~=8.5.6",
-#     # Plugins
-#     "mkdocs-include-markdown-plugin",
-#     "mkdocs-gen-files",
-#     "mkdocs-literate-nav",
-#     "mkdocs-minify-plugin~=0.5.0",
-#     "mkdocs-section-index",
-#     "mkdocs-git-revision-date-localized-plugin~=1.1.0",
-#     "mkdocstrings[python]",
-#     "mkdocs-redirects~=1.1.0",
-#     "mkdocs-glightbox~=0.3.0",
-#     # https://github.com/jimporter/mike/issues/82#issuecomment-1172913929
-#     "mike @ https://github.com/jimporter/mike/archive/392d57b8bb9d14bcedf2451a0dc302709f8055eb.zip",
-#     # Extensions
-#     "pymdown-extensions~=9.6.0",
-#     # Necessary for syntax highlighting in code blocks
-#     "pygments~=2.13.0",
-#     # Validation
-#     # https://github.com/linkchecker/linkchecker/pull/669#issuecomment-1267236287
-#     "linkchecker @ git+https://github.com/linkchecker/linkchecker.git@d9265bb71c2054bf57b8c5734a4825d62505c779",
-# ]
-# [tool.hatch.envs.docs.env-vars]
-# SOURCE_DATE_EPOCH = "1580601600"
-# PYTHONUNBUFFERED = "1"
-# MKDOCS_CONFIG = "mkdocs.yml"
-
-# [tool.hatch.envs.docs.scripts]
-# build = "mkdocs build --config-file {env:MKDOCS_CONFIG} --clean --strict {args}"
-# serve = "mkdocs serve --config-file {env:MKDOCS_CONFIG} --dev-addr localhost:8000 {args}"
-# ci-build = "mike deploy --config-file {env:MKDOCS_CONFIG} --update-aliases {args}"
-# # --ignore-url=None since the SUMMARY.md file leaves a <toc>None</toc> in sitemap.xml
-# validate = "linkchecker --config .linkcheckerrc --ignore-url=/reference --ignore-url=None site"
-# # https://github.com/linkchecker/linkchecker/issues/678
-# build-check = ["build", "validate"]
+# Docs environment
+[tool.hatch.envs.docs]
+dependencies = [
+    "mkdocs~=1.5.0",
+    "mkdocs-material~=9.5.0",
+    # Plugins
+    "mkdocs-include-markdown-plugin",
+    "mkdocs-gen-files",
+    "mkdocs-literate-nav",
+    "mkdocs-minify-plugin~=0.5.0",
+    "mkdocs-section-index",
+    "mkdocs-git-revision-date-localized-plugin~=1.1.0",
+    "mkdocstrings[python]",
+    "mkdocs-redirects~=1.1.0",
+    "mkdocs-glightbox~=0.3.0",
+    # https://github.com/jimporter/mike/issues/82#issuecomment-1172913929
+    "mike @ https://github.com/jimporter/mike/archive/392d57b8bb9d14bcedf2451a0dc302709f8055eb.zip",
+    # Extensions
+    "pymdown-extensions~=10.7.0",
+    # Necessary for syntax highlighting in code blocks
+    "pygments~=2.17.0",
+    # Validation
+    # https://github.com/linkchecker/linkchecker/pull/669#issuecomment-1267236287
+    "linkchecker @ git+https://github.com/linkchecker/linkchecker.git@d9265bb71c2054bf57b8c5734a4825d62505c779",
+]
+[tool.hatch.envs.docs.env-vars]
+SOURCE_DATE_EPOCH = "1580601600"
+PYTHONUNBUFFERED = "1"
+MKDOCS_CONFIG = "mkdocs.yml"
+
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build --config-file {env:MKDOCS_CONFIG} --clean --strict {args}"
+serve = "mkdocs serve --config-file {env:MKDOCS_CONFIG} --dev-addr localhost:8000 {args}"
+ci-build = "mike deploy --config-file {env:MKDOCS_CONFIG} --update-aliases {args}"
+# --ignore-url=None since the SUMMARY.md file leaves a <toc>None</toc> in sitemap.xml
+validate = "linkchecker --config .linkcheckerrc --ignore-url=/reference --ignore-url=None site"
+# https://github.com/linkchecker/linkchecker/issues/678
+build-check = ["build", "validate"]
 
 # # Lint environment
 # [tool.hatch.envs.lint]
 # skip-install = true
 # dependencies = ["mypy~=1.6", "ruff==0.1.4"]
 
 # [tool.hatch.envs.lint.scripts]
```

### Comparing `octoflow-0.0.9/PKG-INFO` & `octoflow-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
 Name: octoflow
-Version: 0.0.9
+Version: 0.1.0
 Summary: Streamlining machine learning tracking for seamless experiment management.
 Project-URL: Documentation, https://github.com/ysenarath/octoflow
 Project-URL: Source, https://github.com/ysenarath/octoflow
 Author-email: Yasas Senarath <email@example.com>
 License-Expression: MIT
 License-File: AUTHORS.md
 License-File: LICENSE
 Keywords: machine-learning,tracking
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
+Requires-Dist: cloudpickle
+Requires-Dist: dill
+Requires-Dist: filelock>=3.13.4
+Requires-Dist: octoflow-plugins
+Requires-Dist: omegaconf>=2.3.0
+Requires-Dist: pandas>=2.2.2
+Requires-Dist: polars>=0.20.22
+Requires-Dist: pyarrow>=16.0.0
+Requires-Dist: sqlalchemy
+Requires-Dist: tqdm>=4.66.2
+Requires-Dist: xxhash
 Description-Content-Type: text/markdown
 
 # OctoFlow
 
 Streamlining machine learning tracking for seamless experiment management.
 
 ## Features
```

