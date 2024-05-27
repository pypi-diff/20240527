# Comparing `tmp/graphene_django_query_optimizer-0.6.0.tar.gz` & `tmp/graphene_django_query_optimizer-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.6.0.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.6.1.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.6.0.tar` & `graphene_django_query_optimizer-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/README.md
--rw-r--r--   0        0        0     6906 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/query_optimizer/ast.py
--rw-r--r--   0        0        0     8785 2024-05-24 17:24:45.535122 graphene_django_query_optimizer-0.6.0/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/errors.py
--rw-r--r--   0        0        0    15533 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/filter.py
--rw-r--r--   0        0        0     5309 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    10926 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/py.typed
--rw-r--r--   0        0        0     3600 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/settings.py
--rw-r--r--   0        0        0     2996 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/types.py
--rw-r--r--   0        0        0     3661 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/typing.py
--rw-r--r--   0        0        0     6842 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-24 17:24:45.539122 graphene_django_query_optimizer-0.6.0/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-27 07:09:48.252355 graphene_django_query_optimizer-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/README.md
+-rw-r--r--   0        0        0     6906 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      496 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8967 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/errors.py
+-rw-r--r--   0        0        0    17282 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5687 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    11776 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3600 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/settings.py
+-rw-r--r--   0        0        0     3212 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/types.py
+-rw-r--r--   0        0        0     3845 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6842 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-27 07:09:48.256355 graphene_django_query_optimizer-0.6.1/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.6.1/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.6.0/LICENSE` & `graphene_django_query_optimizer-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/README.md` & `graphene_django_query_optimizer-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/pyproject.toml` & `graphene_django_query_optimizer-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.6.0"
+version = "0.6.1"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
@@ -57,15 +57,15 @@
 django-settings-holder = ">=0.1.2"
 
 [tool.poetry.extras]
 filter = ["django-filter"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "8.2.1"
-coverage = "7.5.1"
+coverage = "7.5.2"
 pytest-django = "4.8.0"
 pre-commit = "3.7.1"
 tox = "4.15.0"
 tox-gh-actions = "3.2.0"
 faker = "25.2.0"
 factory-boy = "3.3.0"
 sqlparse = "0.5.0"
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,26 +193,30 @@
         # `RelatedField`, `DjangoListField` and `DjangoConnectionField` can define a
         # 'field_name' attribute to specify the actual model field name.
         actual_field_name: Optional[str] = getattr(field, "field_name", None)
         if actual_field_name is not None:
             self.to_attr = field_name
             return self.handle_model_field(field_type, field_node, actual_field_name)
 
-        from .fields import AnnotatedField, MultiField
+        from .fields import AnnotatedField, MultiField, PreResolvingField
 
         if isinstance(field, AnnotatedField):
             self.optimizer.annotations[to_snake_case(field.name)] = field.expression
             if field.aliases is not None:
                 self.optimizer.aliases.update(field.aliases)
             return None
 
         if isinstance(field, MultiField):
             self.optimizer.only_fields.extend(field.fields)
             return None
 
+        if isinstance(field, PreResolvingField):
+            self.optimizer.pre_resolvers[to_snake_case(field.name)] = field.pre_resolver
+            return None
+
         return None  # pragma: no cover
 
     @contextlib.contextmanager
     def use_optimizer(self, optimizer: QueryOptimizer) -> None:
         orig_optimizer = self.optimizer
         try:
             self.optimizer = optimizer
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,23 +18,24 @@
 from .prefetch_hack import fetch_in_context
 from .settings import optimizer_settings
 from .utils import calculate_queryset_slice, is_optimized
 from .validators import validate_pagination_args
 
 if TYPE_CHECKING:
     from django.db import models
-    from django.db.models import Model
+    from django.db.models import Model, QuerySet
     from django.db.models.manager import Manager
     from graphene.relay.connection import Connection
     from graphql_relay import EdgeType
     from graphql_relay.connection.connection import ConnectionType
 
     from .types import DjangoObjectType
     from .typing import (
         Any,
+        ArgTypeInput,
         Callable,
         ConnectionResolver,
         ExpressionKind,
         GQLInfo,
         Iterable,
         ModelResolver,
         ObjectTypeInput,
@@ -385,7 +386,51 @@
         # `parent_resolver` is either a `resolve_{self.name}` method defined
         # on the owner class, or a partial of `dict_or_attr_resolver`.
         self.resolver = parent_resolver
         return self.multi_field_resolver
 
     def multi_field_resolver(self, root: Model, info: GQLInfo, **kwargs: Any) -> Any:
         return self.resolver(root, info, **kwargs)
+
+
+class PreResolvingField(graphene.Field):
+    """
+    Field that has a pre-resolving step.
+
+    Must define a `pre_resolve_{name}(queryset, info, **kwargs)` staticmethod on the object type,
+    where `{name}` is the name of the field defined on the object type, and `kwargs`
+    are the values of 'args' defined on this field.
+
+    The optimizer will run pre-resolving methods as the last filtering step.
+    """
+
+    def __init__(
+        self,
+        type_: UnmountedTypeInput,
+        /,
+        *,
+        args: dict[str, ArgTypeInput],
+        **kwargs: Any,
+    ) -> None:
+        super().__init__(type_, args=args, **kwargs)
+
+    def __set_name__(self, owner: type[DjangoObjectType], name: str) -> None:
+        self.owner = owner
+        self.name = to_camel_case(name)
+
+    def pre_resolver(self, queryset: QuerySet, info: GQLInfo, **kwargs: Any) -> QuerySet:
+        name = to_snake_case(self.name)
+        resolver_name = f"pre_resolve_{name}"
+        resolver: Callable[..., QuerySet] | None = getattr(self.owner, resolver_name, None)
+        if resolver is None:  # pragma: no cover
+            msg = f"Pre-resolver method '{resolver_name}' missing from '{self.owner}'."
+            raise AttributeError(msg)
+        return resolver(queryset, info, **kwargs)
+
+    def wrap_resolve(self, parent_resolver: Callable[..., Any]) -> Callable[..., Any]:
+        # `parent_resolver` is either a `resolve_{self.name}` method defined
+        # on the owner class, or a partial of `dict_or_attr_resolver`.
+        self.resolver = parent_resolver
+        return self.field_resolver
+
+    def field_resolver(self, root: Model, info: GQLInfo, **kwargs: Any) -> Any:
+        return self.resolver(root, info, **kwargs)
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/filter_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,14 +100,22 @@
                 del self.filter_info[name]
 
     def handle_query_class(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         self.add_filter_info(field_type, field_node)
         with self.child_filter_info(field_node):
             super().handle_query_class(field_type, field_node)
 
+    def handle_custom_field(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
+        from .fields import PreResolvingField
+
+        field_name = to_snake_case(field_node.name.value)
+        field = getattr(field_type.graphene_type, field_name, None)
+        if isinstance(field, PreResolvingField):
+            self.add_filter_info(field_type, field_node)
+
     def handle_to_one_field(
         self,
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToOneField,
         related_model: type[Model],
     ) -> None:
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,16 +25,24 @@
     optimizer_logger,
     swappable_by_subclassing,
 )
 from .validators import validate_pagination_args
 
 if TYPE_CHECKING:
     from .types import DjangoObjectType
-    from .typing import Any, ExpressionKind, GQLInfo, GraphQLFilterInfo, Optional, TModel, ToManyField
-
+    from .typing import (
+        Any,
+        ExpressionKind,
+        GQLInfo,
+        GraphQLFilterInfo,
+        Optional,
+        QuerySetResolver,
+        TModel,
+        ToManyField,
+    )
 
 __all__ = [
     "QueryOptimizer",
 ]
 
 
 @dataclasses.dataclass
@@ -53,14 +61,15 @@
         self.info = info
         self.only_fields: list[str] = []
         self.related_fields: list[str] = []
         self.aliases: dict[str, ExpressionKind] = {}
         self.annotations: dict[str, ExpressionKind] = {}
         self.select_related: dict[str, QueryOptimizer] = {}
         self.prefetch_related: dict[str, QueryOptimizer] = {}
+        self.pre_resolvers: dict[str, QuerySetResolver] = {}
         self.total_count: bool = False
         self.name = name
 
     def optimize_queryset(
         self,
         queryset: QuerySet[TModel],
         *,
@@ -71,28 +80,30 @@
 
         :param queryset: QuerySet to optimize.
         :param filter_info: Additional filtering info to use for the optimization.
         """
         if filter_info is None:
             filter_info = get_filter_info(self.info, queryset.model)
 
+        self.pre_compilation(queryset.model)
         results = self.compile(filter_info=filter_info)
 
         if filter_info is not None and filter_info.get("filterset_class") is not None:
             filterset = filter_info["filterset_class"](
                 data=self.process_filters(filter_info["filters"]),
                 queryset=queryset,
                 request=self.info.context,
             )
             if not filterset.is_valid():  # pragma: no cover
                 raise ValidationError(filterset.form.errors.as_json())
 
             queryset = filterset.qs
 
         queryset = self.get_filtered_queryset(queryset)
+        queryset = self.run_pre_resolvers(queryset, filter_info)
 
         if results.select_related:
             queryset = queryset.select_related(*results.select_related)
         if results.prefetch_related:
             queryset = queryset.prefetch_related(*results.prefetch_related)
         if not optimizer_settings.DISABLE_ONLY_FIELDS_OPTIMIZATION and (results.only_fields or self.related_fields):
             queryset = queryset.only(*results.only_fields, *self.related_fields)
@@ -252,7 +263,18 @@
             return object_type.filter_queryset(queryset, self.info)  # type: ignore[union-attr]
         return queryset  # pragma: no cover
 
     def process_filters(self, input_data: dict[str, Any]) -> dict[str, Any]:
         from graphene_django.filter.fields import convert_enum
 
         return {key: convert_enum(value) for key, value in input_data.items()}
+
+    def run_pre_resolvers(self, queryset: QuerySet, filter_info: GraphQLFilterInfo) -> QuerySet:
+        for name, resolver in self.pre_resolvers.items():
+            filters = filter_info["children"][name]["filters"]
+            queryset = resolver(queryset, self.info, **filters)
+        return queryset
+
+    def pre_compilation(self, model: type[Model]) -> None:
+        object_type: Optional[DjangoObjectType] = get_global_registry().get_type_for_model(model)
+        if callable(getattr(object_type, "pre_compilation_hook", None)):
+            object_type.pre_compilation_hook(self)
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/types.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .compiler import optimize_single
 from .settings import optimizer_settings
 from .typing import PK, OptimizedDjangoOptions
 
 if TYPE_CHECKING:
     from django.db.models import Model, QuerySet
 
+    from .optimizer import QueryOptimizer
     from .typing import Any, GQLInfo, Literal, Optional, TModel, Union
 
 
 __all__ = [
     "DjangoObjectType",
 ]
 
@@ -63,14 +64,18 @@
 
     @classmethod
     def filter_queryset(cls, queryset: QuerySet[TModel], info: GQLInfo) -> QuerySet[TModel]:
         """Implement this method filter to the available rows from the model on this node."""
         return queryset
 
     @classmethod
+    def pre_compilation_hook(cls, optimizer: QueryOptimizer) -> None:
+        """A hook for modifying the optimizer results before optimization happens."""
+
+    @classmethod
     def get_queryset(cls, queryset: QuerySet[TModel], info: GQLInfo) -> QuerySet[TModel]:
         return queryset
 
     @classmethod
     def get_node(cls, info: GQLInfo, pk: PK) -> Optional[TModel]:
         queryset = cls._meta.model._default_manager.all()
         maybe_instance = optimize_single(queryset, info, pk=pk, max_complexity=cls._meta.max_complexity)
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     TypeVar,
     Union,
     cast,
     overload,
 )
 
 from django.db import models
+from graphene import Argument, Dynamic
+from graphene.types.structures import Structure
 from graphene.types.unmountedtype import UnmountedType
 from graphene_django import DjangoObjectType
 from graphene_django.types import DjangoObjectTypeOptions
 from graphql_relay import ConnectionType
 
 # New in version 3.10
 try:
@@ -55,61 +57,63 @@
     from django.contrib.auth.models import AnonymousUser, User
     from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
     from django.db.models.sql import Query
     from django_filters import FilterSet
 
 __all__ = [
     "Any",
+    "ArgTypeInput",
     "Callable",
+    "cast",
     "Collection",
     "ConnectionResolver",
     "ContextManager",
     "Expr",
     "ExpressionKind",
-    "GQLInfo",
-    "GRAPHQL_BUILTIN",
     "Generator",
     "Generic",
+    "GQLInfo",
+    "GRAPHQL_BUILTIN",
     "GraphQLFilterInfo",
     "Hashable",
     "Iterable",
     "Literal",
     "ModelField",
     "ModelResolver",
     "NamedTuple",
     "ObjectTypeInput",
     "OptimizedDjangoOptions",
     "Optional",
-    "PK",
+    "overload",
     "ParamSpec",
+    "PK",
     "QuerySetResolver",
     "ToManyField",
     "ToOneField",
     "Type",
+    "TypedDict",
     "TypeGuard",
     "TypeVar",
-    "TypedDict",
     "Union",
     "UnmountedTypeInput",
-    "cast",
-    "overload",
 ]
 
 
 TModel = TypeVar("TModel", bound=Model)
 PK: TypeAlias = Any
 ModelField: TypeAlias = Union[Field, ForeignObjectRel, "GenericForeignKey"]
 ToManyField: TypeAlias = Union["GenericRelation", ManyToManyField, ManyToOneRel, ManyToManyRel]
 ToOneField: TypeAlias = Union["GenericRelation", ForeignObject, ForeignKey, OneToOneField]
 AnyUser: TypeAlias = Union["User", "AnonymousUser"]
 QuerySetResolver: TypeAlias = Callable[..., Union[QuerySet, Manager, None]]
 ModelResolver: TypeAlias = Callable[..., Union[Model, None]]
 ConnectionResolver: TypeAlias = Callable[..., ConnectionType]
-ObjectTypeInput: TypeAlias = Union[type[DjangoObjectType], str, Callable[[], type[DjangoObjectType]]]
-UnmountedTypeInput: TypeAlias = Union[type[UnmountedType], str, Callable[[], type[UnmountedType]]]
+ObjectTypeInput: TypeAlias = Union[str, type[DjangoObjectType], Callable[[], type[DjangoObjectType]]]
+UnmountedTypeInput: TypeAlias = Union[str, type[UnmountedType], Structure, Callable[[], type[UnmountedType]]]
+ArgTypeInput: TypeAlias = Union[Argument, UnmountedType, Dynamic]
 Expr: TypeAlias = Union[models.Expression, models.F, models.Q]
 
 
 GRAPHQL_BUILTIN = (
     "__typename",
     "__schema",
     "__type",
```

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.6.1/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.0/PKG-INFO` & `graphene_django_query_optimizer-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.6.0
+Version: 0.6.1
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

