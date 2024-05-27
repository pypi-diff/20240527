# Comparing `tmp/resend-1.2.0.tar.gz` & `tmp/resend-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/resend-1.2.0.tar", last modified: Fri May 24 20:34:32 2024, max compression
+gzip compressed data, was "dist/resend-2.0.0.tar", last modified: Mon May 27 17:48:31 2024, max compression
```

## Comparing `resend-1.2.0.tar` & `resend-2.0.0.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.037168 resend-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-24 20:34:32.037361 resend-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1623 2024-05-24 14:17:40.000000 resend-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.015099 resend-1.2.0/resend/
--rw-r--r--   0 root         (0) root         (0)     1003 2024-05-14 01:16:37.000000 resend-1.2.0/resend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.022683 resend-1.2.0/resend/api_keys/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/__init__.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-05-09 01:36:14.000000 resend-1.2.0/resend/api_keys/_api_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.025278 resend-1.2.0/resend/audiences/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1192 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/_audience.py
--rw-r--r--   0 root         (0) root         (0)     2305 2024-05-09 01:36:14.000000 resend-1.2.0/resend/audiences/_audiences.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.027560 resend-1.2.0/resend/contacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1795 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/_contact.py
--rw-r--r--   0 root         (0) root         (0)     4400 2024-05-09 01:36:14.000000 resend-1.2.0/resend/contacts/_contacts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.031464 resend-1.2.0/resend/domains/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1987 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_domain.py
--rw-r--r--   0 root         (0) root         (0)     3887 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_domains.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-05-09 01:36:14.000000 resend-1.2.0/resend/domains/_record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.036515 resend-1.2.0/resend/emails/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/__init__.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/_attachment.py
--rw-r--r--   0 root         (0) root         (0)      991 2024-05-24 14:17:40.000000 resend-1.2.0/resend/emails/_batch.py
--rw-r--r--   0 root         (0) root         (0)     2845 2024-05-24 14:17:40.000000 resend-1.2.0/resend/emails/_email.py
--rw-r--r--   0 root         (0) root         (0)     3281 2024-05-24 19:25:50.000000 resend-1.2.0/resend/emails/_emails.py
--rw-r--r--   0 root         (0) root         (0)      524 2024-05-09 01:36:14.000000 resend-1.2.0/resend/emails/_tag.py
--rw-r--r--   0 root         (0) root         (0)     6108 2024-05-22 00:27:09.000000 resend-1.2.0/resend/exceptions.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-19 17:45:00.000000 resend-1.2.0/resend/py.typed
--rw-r--r--   0 root         (0) root         (0)     2553 2024-05-24 14:17:40.000000 resend-1.2.0/resend/request.py
--rw-r--r--   0 root         (0) root         (0)      562 2024-05-24 14:17:40.000000 resend-1.2.0/resend/utils.py
--rw-r--r--   0 root         (0) root         (0)      133 2024-05-24 19:07:51.000000 resend-1.2.0/resend/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 20:34:32.020609 resend-1.2.0/resend.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2891 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      830 2024-05-24 20:34:32.000000 resend-1.2.0/resend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       35 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-24 20:34:31.000000 resend-1.2.0/resend.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-24 20:34:32.038063 resend-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1222 2024-05-24 14:17:40.000000 resend-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.457321 resend-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-27 17:48:31.457521 resend-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-24 23:45:10.000000 resend-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.433770 resend-2.0.0/resend/
+-rw-r--r--   0 root         (0) root         (0)     1003 2024-05-14 01:16:37.000000 resend-2.0.0/resend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.442171 resend-2.0.0/resend/api_keys/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-2.0.0/resend/api_keys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      281 2024-05-25 15:12:34.000000 resend-2.0.0/resend/api_keys/_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2024-05-25 15:12:34.000000 resend-2.0.0/resend/api_keys/_api_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.444763 resend-2.0.0/resend/audiences/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-2.0.0/resend/audiences/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      390 2024-05-25 15:12:34.000000 resend-2.0.0/resend/audiences/_audience.py
+-rw-r--r--   0 root         (0) root         (0)     2467 2024-05-25 15:12:34.000000 resend-2.0.0/resend/audiences/_audiences.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.447274 resend-2.0.0/resend/contacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-2.0.0/resend/contacts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-25 15:12:34.000000 resend-2.0.0/resend/contacts/_contact.py
+-rw-r--r--   0 root         (0) root         (0)     4531 2024-05-25 15:12:34.000000 resend-2.0.0/resend/contacts/_contacts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.451186 resend-2.0.0/resend/domains/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-2.0.0/resend/domains/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      693 2024-05-25 15:12:34.000000 resend-2.0.0/resend/domains/_domain.py
+-rw-r--r--   0 root         (0) root         (0)     4085 2024-05-25 15:12:34.000000 resend-2.0.0/resend/domains/_domains.py
+-rw-r--r--   0 root         (0) root         (0)      532 2024-05-25 15:12:34.000000 resend-2.0.0/resend/domains/_record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.456713 resend-2.0.0/resend/emails/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 01:36:14.000000 resend-2.0.0/resend/emails/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-05-09 01:36:14.000000 resend-2.0.0/resend/emails/_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2024-05-25 15:12:34.000000 resend-2.0.0/resend/emails/_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1600 2024-05-26 15:56:50.000000 resend-2.0.0/resend/emails/_email.py
+-rw-r--r--   0 root         (0) root         (0)     3398 2024-05-26 15:56:50.000000 resend-2.0.0/resend/emails/_emails.py
+-rw-r--r--   0 root         (0) root         (0)      524 2024-05-09 01:36:14.000000 resend-2.0.0/resend/emails/_tag.py
+-rw-r--r--   0 root         (0) root         (0)     6108 2024-05-22 00:27:09.000000 resend-2.0.0/resend/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-19 17:45:00.000000 resend-2.0.0/resend/py.typed
+-rw-r--r--   0 root         (0) root         (0)     2553 2024-05-24 14:17:40.000000 resend-2.0.0/resend/request.py
+-rw-r--r--   0 root         (0) root         (0)      133 2024-05-27 17:46:22.000000 resend-2.0.0/resend/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 17:48:31.439096 resend-2.0.0/resend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2891 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      814 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       35 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-27 17:48:31.000000 resend-2.0.0/resend.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-27 17:48:31.458200 resend-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1222 2024-05-24 14:17:40.000000 resend-2.0.0/setup.py
```

### Comparing `resend-1.2.0/PKG-INFO` & `resend-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.2.0
+Version: 2.0.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
```

### Comparing `resend-1.2.0/README.md` & `resend-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `resend-1.2.0/resend/__init__.py` & `resend-2.0.0/resend/__init__.py`

 * *Files identical despite different names*

### Comparing `resend-1.2.0/resend/api_keys/_api_keys.py` & `resend-2.0.0/resend/api_keys/_api_keys.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,31 @@
 
 from typing_extensions import NotRequired, TypedDict
 
 from resend import request
 from resend.api_keys._api_key import ApiKey
 
 
+class _ListResponse(TypedDict):
+    data: List[ApiKey]
+    """
+    A list of API key objects
+    """
+
+
 class ApiKeys:
+
+    class ListResponse(_ListResponse):
+        """
+        ListResponse type that wraps a list of API key objects
+
+        Attributes:
+            data (List[Dict[str, Any]]): A list of API key objects
+        """
+
     class CreateParams(TypedDict):
         name: str
         """
         The API key name.
         """
         permission: NotRequired[str]
         """
@@ -33,32 +49,33 @@
         Args:
             params (CreateParams): The API key creation parameters
 
         Returns:
             ApiKey: The new API key object
         """
         path = "/api-keys"
-        return ApiKey.new_from_request(
+        return cast(
+            ApiKey,
             request.Request(
                 path=path, params=cast(Dict[Any, Any], params), verb="post"
-            ).perform()
+            ).perform(),
         )
 
     @classmethod
-    def list(cls) -> List[ApiKey]:
+    def list(cls) -> ListResponse:
         """
         Retrieve a list of API keys for the authenticated user.
         see more: https://resend.com/docs/api-reference/api-keys/list-api-keys
 
         Returns:
-            List[ApiKey]: A list of API key objects
+            ListResponse: A list of API key objects
         """
         path = "/api-keys"
         resp = request.Request(path=path, params={}, verb="get").perform()
-        return [ApiKey.new_from_request(val) for val in resp["data"]]
+        return cast(_ListResponse, resp)
 
     @classmethod
     def remove(cls, api_key_id: str) -> None:
         """
         Remove an existing API key.
         see more: https://resend.com/docs/api-reference/api-keys/delete-api-key
```

### Comparing `resend-1.2.0/resend/audiences/_audiences.py` & `resend-2.0.0/resend/audiences/_audiences.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,31 @@
 from typing_extensions import TypedDict
 
 from resend import request
 
 from ._audience import Audience
 
 
+class _ListResponse(TypedDict):
+    data: List[Audience]
+    """
+    A list of audience objects
+    """
+
+
 class Audiences:
+
+    class ListResponse(_ListResponse):
+        """
+        ListResponse type that wraps a list of audience objects
+
+        Attributes:
+            data (List[Audience]): A list of audience objects
+        """
+
     class CreateParams(TypedDict):
         name: str
         """
         The name of the audience.
         """
 
     @classmethod
@@ -23,63 +39,56 @@
         Args:
             params (CreateParams): The audience creation parameters
 
         Returns:
             Audience: The new audience object
         """
         path = "/audiences"
-        return Audience.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="post"
-            ).perform()
-        )
+        resp = request.Request(
+            path=path, params=cast(Dict[Any, Any], params), verb="post"
+        ).perform()
+        return cast(Audience, resp)
 
     @classmethod
-    def list(cls) -> List[Audience]:
+    def list(cls) -> ListResponse:
         """
         Retrieve a list of audiences.
         see more: https://resend.com/docs/api-reference/audiences/list-audiences
 
         Returns:
-            List[Audience]: A list of audience objects
+            ListResponse: A list of audience objects
         """
         path = "/audiences/"
         resp = request.Request(path=path, params={}, verb="get").perform()
-        return (
-            [Audience.new_from_request(aud) for aud in resp["data"]]
-            if "data" in resp
-            else []
-        )
+        return cast(_ListResponse, resp)
 
     @classmethod
     def get(cls, id: str) -> Audience:
         """
         Retrieve a single audience.
         see more: https://resend.com/docs/api-reference/audiences/get-audience
 
         Args:
             id (str): The audience ID
 
         Returns:
             Audience: The audience object
         """
         path = f"/audiences/{id}"
-        return Audience.new_from_request(
-            request.Request(path=path, params={}, verb="get").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="get").perform()
+        return cast(Audience, resp)
 
     @classmethod
     def remove(cls, id: str) -> Audience:
         """
         Delete a single audience.
         see more: https://resend.com/docs/api-reference/audiences/delete-audience
 
         Args:
             id (str): The audience ID
 
         Returns:
             Audience: The audience object
         """
         path = f"/audiences/{id}"
-        return Audience.new_from_request(
-            request.Request(path=path, params={}, verb="delete").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="delete").perform()
+        return cast(Audience, resp)
```

### Comparing `resend-1.2.0/resend/contacts/_contacts.py` & `resend-2.0.0/resend/contacts/_contacts.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,31 @@
 from typing_extensions import NotRequired, TypedDict
 
 from resend import request
 
 from ._contact import Contact
 
 
+class _ListResponse(TypedDict):
+    data: List[Contact]
+    """
+    A list of contact objects
+    """
+
+
 class Contacts:
+
+    class ListResponse(_ListResponse):
+        """
+        ListResponse type that wraps a list of contact objects
+
+        Attributes:
+            data (List[Contact]): A list of contact objects
+        """
+
     class CreateParams(TypedDict):
         audience_id: str
         """
         The audience id.
         """
         email: str
         """
@@ -65,58 +81,52 @@
         Args:
             params (CreateParams): The contact creation parameters
 
         Returns:
             Contact: The new contact object
         """
         path = f"/audiences/{params['audience_id']}/contacts"
-        return Contact.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="post"
-            ).perform()
-        )
+        resp = request.Request(
+            path=path, params=cast(Dict[Any, Any], params), verb="post"
+        ).perform()
+        return cast(Contact, resp)
 
     @classmethod
     def update(cls, params: UpdateParams) -> Contact:
         """
         Update an existing contact.
         see more: https://resend.com/docs/api-reference/contacts/update-contact
 
         Args:
             params (UpdateParams): The contact update parameters
 
         Returns:
             Contact: The updated contact object
         """
         path = f"/audiences/{params['audience_id']}/contacts/{params['id']}"
-        return Contact.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="patch"
-            ).perform()
-        )
+        resp = request.Request(
+            path=path, params=cast(Dict[Any, Any], params), verb="patch"
+        ).perform()
+        return cast(Contact, resp)
 
     @classmethod
-    def list(cls, audience_id: str) -> List[Contact]:
+    def list(cls, audience_id: str) -> ListResponse:
         """
         List all contacts for the provided audience.
         see more: https://resend.com/docs/api-reference/contacts/list-contacts
 
         Args:
             audience_id (str): The audience ID
 
         Returns:
-            List[Contact]: A list of contact objects
+            ListResponse: A list of contact objects
         """
         path = f"/audiences/{audience_id}/contacts"
         resp = request.Request(path=path, params={}, verb="get").perform()
-        return (
-            [Contact.new_from_request(contact) for contact in resp["data"]]
-            if "data" in resp
-            else []
-        )
+        return cast(_ListResponse, resp)
 
     @classmethod
     def get(cls, id: str, audience_id: str) -> Contact:
         """
         Get a contact.
         see more: https://resend.com/docs/api-reference/contacts/get-contact
 
@@ -124,17 +134,16 @@
             id (str): The contact ID
             audience_id (str): The audience ID
 
         Returns:
             Contact: The contact object
         """
         path = f"/audiences/{audience_id}/contacts/{id}"
-        return Contact.new_from_request(
-            request.Request(path=path, params={}, verb="get").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="get").perform()
+        return cast(Contact, resp)
 
     @classmethod
     def remove(cls, audience_id: str, id: str = "", email: str = "") -> Contact:
         """
         Remove a contact by ID or by Email
         see more: https://resend.com/docs/api-reference/contacts/delete-contact
 
@@ -147,10 +156,9 @@
             Contact: The removed contact object
         """
         contact = email if id == "" else id
         if contact == "":
             raise ValueError("id or email must be provided")
         path = f"/audiences/{audience_id}/contacts/{contact}"
 
-        return Contact.new_from_request(
-            request.Request(path=path, params={}, verb="delete").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="delete").perform()
+        return cast(Contact, resp)
```

### Comparing `resend-1.2.0/resend/domains/_domains.py` & `resend-2.0.0/resend/domains/_domains.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,31 @@
 
 from typing_extensions import NotRequired, TypedDict
 
 from resend import request
 from resend.domains._domain import Domain
 
 
+class _ListResponse(TypedDict):
+    data: List[Domain]
+    """
+    A list of domain objects
+    """
+
+
 class Domains:
+
+    class ListResponse(_ListResponse):
+        """
+        ListResponse type that wraps a list of domain objects
+
+        Attributes:
+            data (List[Domain]): A list of domain objects
+        """
+
     class UpdateParams(TypedDict):
         id: str
         """
         The domain ID.
         """
         click_tracking: NotRequired[bool]
         """
@@ -41,95 +57,90 @@
         Args:
             params (CreateParams): The domain creation parameters
 
         Returns:
             Domain: The new domain object
         """
         path = "/domains"
-        return Domain.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="post"
-            ).perform()
-        )
+        resp = request.Request(
+            path=path, params=cast(Dict[Any, Any], params), verb="post"
+        ).perform()
+        return cast(Domain, resp)
 
     @classmethod
     def update(cls, params: UpdateParams) -> Domain:
         """
         Update an existing domain.
         see more: https://resend.com/docs/api-reference/domains/update-domain
 
         Args:
             params (UpdateParams): The domain update parameters
 
         Returns:
             Domain: The updated domain object
         """
         path = f"/domains/{params['id']}"
-        return Domain.new_from_request(
-            request.Request(
-                path=path, params=cast(Dict[Any, Any], params), verb="patch"
-            ).perform()
-        )
+        resp = request.Request(
+            path=path, params=cast(Dict[Any, Any], params), verb="patch"
+        ).perform()
+        return cast(Domain, resp)
 
     @classmethod
     def get(cls, domain_id: str) -> Domain:
         """
         Retrieve a single domain for the authenticated user.
         see more: https://resend.com/docs/api-reference/domains/get-domain
 
         Args:
             domain_id (str): The domain ID
 
         Returns:
             Domain: The domain object
         """
         path = f"/domains/{domain_id}"
-        return Domain.new_from_request(
-            request.Request(path=path, params={}, verb="get").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="get").perform()
+        return cast(Domain, resp)
 
     @classmethod
-    def list(cls) -> List[Domain]:
+    def list(cls) -> ListResponse:
         """
         Retrieve a list of domains for the authenticated user.
         see more: https://resend.com/docs/api-reference/domains/list-domains
 
         Returns:
-            List[Domain]: A list of domain objects
+            ListResponse: A list of domain objects
         """
         path = "/domains"
         resp = request.Request(path=path, params={}, verb="get").perform()
-        return [Domain.new_from_request(val) for val in resp["data"]]
+        return cast(_ListResponse, resp)
 
     @classmethod
     def remove(cls, domain_id: str) -> Domain:
         """
         Remove an existing domain.
         see more: https://resend.com/docs/api-reference/domains/delete-domain
 
         Args:
             domain_id (str): The domain ID
 
         Returns:
             Domain: The removed domain object
         """
         path = f"/domains/{domain_id}"
-        return Domain.new_from_request(
-            request.Request(path=path, params={}, verb="delete").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="delete").perform()
+        return cast(Domain, resp)
 
     @classmethod
     def verify(cls, domain_id: str) -> Domain:
         """
         Verify an existing domain.
         see more: https://resend.com/docs/api-reference/domains/verify-domain
 
         Args:
             domain_id (str): The domain ID
 
         Returns:
             Domain: The verified domain object
         """
         path = f"/domains/{domain_id}/verify"
-        return Domain.new_from_request(
-            request.Request(path=path, params={}, verb="post").perform()
-        )
+        resp = request.Request(path=path, params={}, verb="post").perform()
+        return cast(Domain, resp)
```

### Comparing `resend-1.2.0/resend/emails/_emails.py` & `resend-2.0.0/resend/emails/_emails.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,27 @@
 
 from typing_extensions import NotRequired, TypedDict
 
 from resend import request
 from resend.emails._attachment import Attachment
 from resend.emails._email import Email
 from resend.emails._tag import Tag
-from resend.utils import replace_params
 
-SendParamsFrom = TypedDict(
-    "SendParamsFrom",
+# SendParamsFrom is declared with functional TypedDict syntax here because
+# "from" is a reserved keyword in Python, and this is the best way to
+# support type-checking for it.
+_SendParamsFrom = TypedDict(
+    "_SendParamsFrom",
     {
         "from": str,
-        "to": Union[str, List[str]],
-        "subject": str,
-        "bcc": NotRequired[Union[List[str], str]],
-        "cc": NotRequired[Union[List[str], str]],
-        "reply_to": NotRequired[Union[List[str], str]],
-        "html": NotRequired[str],
-        "text": NotRequired[str],
-        "headers": NotRequired[Dict[str, str]],
-        "attachments": NotRequired[List[Attachment]],
-        "tags": NotRequired[List[Tag]],
     },
 )
 
 
-class SendParamsDefault(TypedDict):
+class _SendParamsDefault(_SendParamsFrom):
     to: Union[str, List[str]]
     """
     List of email addresses to send the email to.
     """
     subject: str
     """
     The subject of the email.
@@ -65,34 +57,31 @@
     """
     tags: NotRequired[List[Tag]]
     """
     List of tags to be added to the email.
     """
 
 
-class SendParamsFrom_(SendParamsDefault):
-    from_: str
-    """
-    The email address of the sender.
-    "from" is a reserved keyword in python.
-    So we accept either "from_" or "sender"
-    """
-
-
-class SendParamsSender(SendParamsDefault):
-    sender: str
-    """
-    The email address of the sender.
-    "from" is a reserved keyword in python.
-    So we accept either "from_" or "sender"
-    """
-
-
 class Emails:
-    SendParams = Union[SendParamsFrom, SendParamsFrom_, SendParamsSender]
+    class SendParams(_SendParamsDefault):
+        """SendParams is the class that wraps the parameters for the send method.
+
+        Attributes:
+            from (str): The email address to send the email from.
+            to (Union[str, List[str]]): List of email addresses to send the email to.
+            subject (str): The subject of the email.
+            bcc (NotRequired[Union[List[str], str]]): Bcc
+            cc (NotRequired[Union[List[str], str]]): Cc
+            reply_to (NotRequired[Union[List[str], str]]): Reply to
+            html (NotRequired[str]): The HTML content of the email.
+            text (NotRequired[str]): The text content of the email.
+            headers (NotRequired[Dict[str, str]]): Custom headers to be added to the email.
+            attachments (NotRequired[List[Attachment]]): List of attachments to be added to the email.
+            tags (NotRequired[List[Tag]]): List of tags to be added to the email.
+        """
 
     @classmethod
     def send(cls, params: SendParams) -> Email:
         """
         Send an email through the Resend Email API.
         see more: https://resend.com/docs/api-reference/emails/send-email
 
@@ -100,19 +89,19 @@
             params (SendParams): The email parameters
 
         Returns:
             Email: The email object that was sent
         """
         path = "/emails"
 
-        # replace "from_" or "sender" with "from"
-        p = replace_params(cast(Dict[Any, Any], params))
-
-        return Email.new_from_request(
-            request.Request(path=path, params=p, verb="post").perform()
+        return cast(
+            Email,
+            request.Request(
+                path=path, params=cast(Dict[Any, Any], params), verb="post"
+            ).perform(),
         )
 
     @classmethod
     def get(cls, email_id: str) -> Email:
         """
         Retrieve a single email.
         see more: https://resend.com/docs/api-reference/emails/retrieve-email
@@ -120,10 +109,8 @@
         Args:
             email_id (str): The ID of the email to retrieve
 
         Returns:
             Email: The email object that was retrieved
         """
         path = f"/emails/{email_id}"
-        return Email.new_from_request(
-            request.Request(path=path, params={}, verb="get").perform()
-        )
+        return cast(Email, request.Request(path=path, params={}, verb="get").perform())
```

### Comparing `resend-1.2.0/resend/emails/_tag.py` & `resend-2.0.0/resend/emails/_tag.py`

 * *Files identical despite different names*

### Comparing `resend-1.2.0/resend/exceptions.py` & `resend-2.0.0/resend/exceptions.py`

 * *Files identical despite different names*

### Comparing `resend-1.2.0/resend/request.py` & `resend-2.0.0/resend/request.py`

 * *Files identical despite different names*

### Comparing `resend-1.2.0/resend.egg-info/PKG-INFO` & `resend-2.0.0/resend.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resend
-Version: 1.2.0
+Version: 2.0.0
 Summary: Resend Python SDK
 Home-page: https://github.com/resendlabs/resend-python
 Author: Derich Pacheco
 Author-email: carlosderich@gmail.com
 License: UNKNOWN
 Description: # Resend Python SDK
```

### Comparing `resend-1.2.0/resend.egg-info/SOURCES.txt` & `resend-2.0.0/resend.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 README.md
 setup.cfg
 setup.py
 resend/__init__.py
 resend/exceptions.py
 resend/py.typed
 resend/request.py
-resend/utils.py
 resend/version.py
 resend.egg-info/PKG-INFO
 resend.egg-info/SOURCES.txt
 resend.egg-info/dependency_links.txt
 resend.egg-info/not-zip-safe
 resend.egg-info/requires.txt
 resend.egg-info/top_level.txt
```

### Comparing `resend-1.2.0/setup.py` & `resend-2.0.0/setup.py`

 * *Files identical despite different names*

