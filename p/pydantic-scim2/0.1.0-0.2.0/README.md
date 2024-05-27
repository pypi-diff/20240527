# Comparing `tmp/pydantic_scim2-0.1.0.tar.gz` & `tmp/pydantic_scim2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_scim2-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_scim2-0.2.0.tar", max compression
```

## Comparing `pydantic_scim2-0.1.0.tar` & `pydantic_scim2-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-23 18:23:05.204875 pydantic_scim2-0.1.0/LICENSE
--rw-r--r--   0        0        0      376 2024-05-23 18:29:12.569821 pydantic_scim2-0.1.0/README.md
--rw-r--r--   0        0        0     1691 2024-05-23 18:23:05.204875 pydantic_scim2-0.1.0/pydantic_scim2/__init__.py
--rw-r--r--   0        0        0     1645 2024-05-23 19:56:26.416322 pydantic_scim2-0.1.0/pydantic_scim2/enterprise_user.py
--rw-r--r--   0        0        0      590 2024-05-23 18:26:12.454000 pydantic_scim2-0.1.0/pydantic_scim2/group.py
--rw-r--r--   0        0        0     1773 2024-05-23 20:12:44.231912 pydantic_scim2-0.1.0/pydantic_scim2/resource_type.py
--rw-r--r--   0        0        0     2860 2024-05-23 20:10:56.982398 pydantic_scim2-0.1.0/pydantic_scim2/responses.py
--rw-r--r--   0        0        0     2926 2024-05-23 20:00:24.035256 pydantic_scim2-0.1.0/pydantic_scim2/service_provider.py
--rw-r--r--   0        0        0    12935 2024-05-23 19:02:48.490574 pydantic_scim2-0.1.0/pydantic_scim2/user.py
--rw-r--r--   0        0        0     2379 2024-05-23 20:02:21.638059 pydantic_scim2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 pydantic_scim2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-24 08:22:28.918776 pydantic_scim2-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1188 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/README.md
+-rw-r--r--   0        0        0     2999 2024-05-27 09:29:26.944868 pydantic_scim2-0.2.0/pydantic_scim2/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/base.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/enterprise_user.py
+-rw-r--r--   0        0        0      782 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/group.py
+-rw-r--r--   0        0        0     7109 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/resource.py
+-rw-r--r--   0        0        0     4085 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/resource_type.py
+-rw-r--r--   0        0        0     2881 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/schema.py
+-rw-r--r--   0        0        0     5742 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/service_provider.py
+-rw-r--r--   0        0        0     9225 2024-05-27 10:11:32.665005 pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/user.py
+-rw-r--r--   0        0        0        0 2024-05-27 07:10:21.446187 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/__init__.py
+-rw-r--r--   0        0        0     1949 2024-05-27 10:03:41.991788 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/bulk.py
+-rw-r--r--   0        0        0     2997 2024-05-27 09:29:26.944868 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/error.py
+-rw-r--r--   0        0        0      845 2024-05-27 09:54:02.902271 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/list_response.py
+-rw-r--r--   0        0        0      973 2024-05-27 09:56:02.875382 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/patch_op.py
+-rw-r--r--   0        0        0     1460 2024-05-27 10:11:17.115016 pydantic_scim2-0.2.0/pydantic_scim2/rfc7644/search_request.py
+-rw-r--r--   0        0        0     2565 2024-05-27 10:17:18.041370 pydantic_scim2-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2152 1970-01-01 00:00:00.000000 pydantic_scim2-0.2.0/PKG-INFO
```

### Comparing `pydantic_scim2-0.1.0/LICENSE` & `pydantic_scim2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_scim2-0.1.0/pydantic_scim2/enterprise_user.py` & `pydantic_scim2-0.2.0/pydantic_scim2/rfc7643/enterprise_user.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,50 @@
+from typing import List
 from typing import Optional
 
 from pydantic import AnyUrl
-from pydantic import BaseModel
 from pydantic import Field
 
+from ..base import SCIM2Model
+
+
+class Manager(SCIM2Model):
+    value: Optional[str] = None
+    """The id of the SCIM resource representingthe User's manager."""
 
-class Manager(BaseModel):
-    value: Optional[str] = Field(
-        None,
-        description="The id of the SCIM resource representingthe User's manager.  REQUIRED.",
-    )
     ref: Optional[AnyUrl] = Field(
         None,
         alias="$ref",
-        description="The URI of the SCIM resource representing the User's manager.  REQUIRED.",
-    )
-    displayName: Optional[str] = Field(
-        None,
-        description="The displayName of the User's manager. OPTIONAL and READ-ONLY.",
     )
+    """The URI of the SCIM resource representing the User's manager."""
 
+    display_name: Optional[str] = None
+    """The displayName of the User's manager."""
 
-class EnterpriseUser(BaseModel):
-    employeeNumber: Optional[str] = Field(
-        None,
-        description="Numeric or alphanumeric identifier assigned to a person, typically based on order of hire or association with anorganization.",
-    )
-    costCenter: Optional[str] = Field(
-        None, description="Identifies the name of a cost center."
-    )
-    organization: Optional[str] = Field(
-        None, description="Identifies the name of an organization."
-    )
-    division: Optional[str] = Field(
-        None, description="Identifies the name of a division."
-    )
-    department: Optional[str] = Field(
-        None,
-        description="Numeric or alphanumeric identifier assigned to a person, typically based on order of hire or association with anorganization.",
-    )
-    manager: Optional[Manager] = Field(
-        None,
-        description="The User's manager. A complex type that optionally allows service providers to represent organizational hierarchy by referencing the 'id' attribute of another User.",
-    )
+
+class EnterpriseUser(SCIM2Model):
+    schemas: List[str] = ["urn:ietf:params:scim:schemas:extension:enterprise:2.0:User"]
+
+    employee_number: Optional[str] = None
+    """Numeric or alphanumeric identifier assigned to a person, typically based
+    on order of hire or association with anorganization."""
+
+    cost_center: Optional[str] = None
+    """"Identifies the name of a cost center."""
+
+    organization: Optional[str] = None
+    """Identifies the name of an organization."""
+
+    division: Optional[str] = None
+    """Identifies the name of a division."""
+
+    department: Optional[str] = None
+    """Numeric or alphanumeric identifier assigned to a person, typically based
+    on order of hire or association with anorganization."""
+
+    manager: Optional[Manager] = None
+    """The User's manager.
+
+    A complex type that optionally allows service providers to represent
+    organizational hierarchy by referencing the 'id' attribute of
+    another User.
+    """
```

### Comparing `pydantic_scim2-0.1.0/pyproject.toml` & `pydantic_scim2-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pydantic-scim2"
-version = "0.1.0"
+version = "0.2.0"
 description = "SCIM2 models for pydantic"
 authors = ["Yaal Coop <contact@yaal.coop>"]
 license = "Apache"
 readme = "README.md"
-keywords = ["scim", "scim2", "provisioning"]
+keywords = ["scim", "scim2", "provisioning", "pydantic"]
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -22,27 +22,28 @@
     "Environment :: Web Environment",
     "Programming Language :: Python",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = {version = "^2.5.0", extras = ["email"]}
+pydantic = {version = "^2.3.0", extras = ["email"]}
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.1"
 pytest-coverage = "^0.0"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 autodoc-pydantic = "^2.2.0"
 shibuya = "^2024.5.15"
 sphinx = "^7.3.7"
+myst-parser = "^3.0.1"
 
 [tool.coverage.run]
 source = [
     "pydantic_scim2",
     "tests",
 ]
 omit = [".tox/*"]
@@ -71,14 +72,19 @@
 
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [too.ruff.format]
 docstring-code-format = true
 
+[tool.pytest.ini_options]
+addopts = "--doctest-modules --doctest-glob='*.rst'"
+doctest_optionflags= "ALLOW_UNICODE IGNORE_EXCEPTION_DETAIL ELLIPSIS"
+
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
 skipsdist = true
 envlist =
     style
```

