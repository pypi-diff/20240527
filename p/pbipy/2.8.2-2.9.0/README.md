# Comparing `tmp/pbipy-2.8.2.tar.gz` & `tmp/pbipy-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbipy-2.8.2.tar", last modified: Mon Feb 26 07:28:21 2024, max compression
+gzip compressed data, was "pbipy-2.9.0.tar", last modified: Mon May 27 17:43:00 2024, max compression
```

## Comparing `pbipy-2.8.2.tar` & `pbipy-2.9.0.tar`

### file list

```diff
@@ -1,26 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-02-26 07:28:21.326398 pbipy-2.8.2/
--rw-rw-rw-   0        0        0    11323 2023-12-20 03:57:58.000000 pbipy-2.8.2/LICENSE
--rw-rw-rw-   0        0        0    12358 2024-02-26 07:28:21.325399 pbipy-2.8.2/PKG-INFO
--rw-rw-rw-   0        0        0    11242 2024-02-26 06:14:34.000000 pbipy-2.8.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-26 07:28:21.304401 pbipy-2.8.2/pbipy/
--rw-rw-rw-   0        0        0       29 2022-11-23 09:01:02.000000 pbipy-2.8.2/pbipy/__init__.py
--rw-rw-rw-   0        0        0      328 2024-02-26 06:59:57.000000 pbipy-2.8.2/pbipy/__version__.py
--rw-rw-rw-   0        0        0    10741 2023-12-20 03:58:08.000000 pbipy-2.8.2/pbipy/_utils.py
--rw-rw-rw-   0        0        0    39053 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/admin.py
--rw-rw-rw-   0        0        0     5510 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/apps.py
--rw-rw-rw-   0        0        0     1786 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/dashboards.py
--rw-rw-rw-   0        0        0     6421 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/dataflows.py
--rw-rw-rw-   0        0        0    20272 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/datasets.py
--rw-rw-rw-   0        0        0     7963 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/groups.py
--rw-rw-rw-   0        0        0    19862 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/powerbi.py
--rw-rw-rw-   0        0        0    13377 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/reports.py
--rw-rw-rw-   0        0        0     1735 2024-02-26 06:14:34.000000 pbipy-2.8.2/pbipy/resources.py
--rw-rw-rw-   0        0        0      106 2023-12-20 03:57:58.000000 pbipy-2.8.2/pbipy/settings.py
-drwxrwxrwx   0        0        0        0 2024-02-26 07:28:21.323401 pbipy-2.8.2/pbipy.egg-info/
--rw-rw-rw-   0        0        0    12358 2024-02-26 07:28:21.000000 pbipy-2.8.2/pbipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-02-26 07:28:21.000000 pbipy-2.8.2/pbipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-26 07:28:21.000000 pbipy-2.8.2/pbipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-02-26 07:28:21.000000 pbipy-2.8.2/pbipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-02-26 07:28:21.000000 pbipy-2.8.2/pbipy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-26 07:28:21.326398 pbipy-2.8.2/setup.cfg
--rw-rw-rw-   0        0        0     3462 2024-02-26 06:14:34.000000 pbipy-2.8.2/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-05-27 17:43:00.732378 pbipy-2.9.0/
+-rw-r--r--   0 andrew     (501) staff       (20)    11323 2023-12-15 06:30:31.000000 pbipy-2.9.0/LICENSE
+-rw-r--r--   0 andrew     (501) staff       (20)    11995 2024-05-27 17:43:00.732202 pbipy-2.9.0/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)    11232 2024-05-27 17:26:34.000000 pbipy-2.9.0/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-05-27 17:43:00.728809 pbipy-2.9.0/pbipy/
+-rw-r--r--   0 andrew     (501) staff       (20)       29 2023-12-15 06:30:31.000000 pbipy-2.9.0/pbipy/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)      328 2024-05-27 17:20:35.000000 pbipy-2.9.0/pbipy/__version__.py
+-rw-r--r--   0 andrew     (501) staff       (20)    10741 2024-05-21 17:52:03.000000 pbipy-2.9.0/pbipy/_utils.py
+-rw-r--r--   0 andrew     (501) staff       (20)    39053 2024-02-25 16:27:13.000000 pbipy-2.9.0/pbipy/admin.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5510 2024-01-11 04:58:53.000000 pbipy-2.9.0/pbipy/apps.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1786 2024-01-11 04:58:53.000000 pbipy-2.9.0/pbipy/dashboards.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6421 2024-01-11 04:58:53.000000 pbipy-2.9.0/pbipy/dataflows.py
+-rw-r--r--   0 andrew     (501) staff       (20)    26172 2024-05-20 17:48:40.000000 pbipy-2.9.0/pbipy/datasets.py
+-rw-r--r--   0 andrew     (501) staff       (20)      382 2024-05-27 17:19:33.000000 pbipy-2.9.0/pbipy/embedtokens.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7963 2024-02-19 05:42:22.000000 pbipy-2.9.0/pbipy/groups.py
+-rw-r--r--   0 andrew     (501) staff       (20)    19862 2024-03-03 16:37:54.000000 pbipy-2.9.0/pbipy/powerbi.py
+-rw-r--r--   0 andrew     (501) staff       (20)    16547 2024-05-27 17:19:33.000000 pbipy-2.9.0/pbipy/reports.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1735 2024-02-18 17:32:07.000000 pbipy-2.9.0/pbipy/resources.py
+-rw-r--r--   0 andrew     (501) staff       (20)      106 2023-12-15 06:30:31.000000 pbipy-2.9.0/pbipy/settings.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-05-27 17:43:00.729511 pbipy-2.9.0/pbipy.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)    11995 2024-05-27 17:43:00.000000 pbipy-2.9.0/pbipy.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      615 2024-05-27 17:43:00.000000 pbipy-2.9.0/pbipy.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2024-05-27 17:43:00.000000 pbipy-2.9.0/pbipy.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       53 2024-05-27 17:43:00.000000 pbipy-2.9.0/pbipy.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        6 2024-05-27 17:43:00.000000 pbipy-2.9.0/pbipy.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       38 2024-05-27 17:43:00.732423 pbipy-2.9.0/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)     3462 2024-02-25 16:27:00.000000 pbipy-2.9.0/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-05-27 17:43:00.731855 pbipy-2.9.0/tests/
+-rw-r--r--   0 andrew     (501) staff       (20)    30529 2024-02-25 16:27:13.000000 pbipy-2.9.0/tests/test_admin.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3557 2023-12-15 06:30:31.000000 pbipy-2.9.0/tests/test_apps.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1670 2023-12-15 06:30:31.000000 pbipy-2.9.0/tests/test_dashboards.py
+-rw-r--r--   0 andrew     (501) staff       (20)     4640 2023-12-15 06:30:31.000000 pbipy-2.9.0/tests/test_dataflows.py
+-rw-r--r--   0 andrew     (501) staff       (20)    34402 2024-05-20 17:32:07.000000 pbipy-2.9.0/tests/test_datasets.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7330 2024-02-19 05:42:22.000000 pbipy-2.9.0/tests/test_groups.py
+-rw-r--r--   0 andrew     (501) staff       (20)    16266 2023-12-15 06:30:31.000000 pbipy-2.9.0/tests/test_powerbi.py
+-rw-r--r--   0 andrew     (501) staff       (20)    18324 2024-05-27 17:19:33.000000 pbipy-2.9.0/tests/test_reports.py
+-rw-r--r--   0 andrew     (501) staff       (20)    11760 2024-01-11 08:07:40.000000 pbipy-2.9.0/tests/test_utils.py
```

### Comparing `pbipy-2.8.2/LICENSE` & `pbipy-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/PKG-INFO` & `pbipy-2.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,353 +1,333 @@
-Metadata-Version: 2.1
-Name: pbipy
-Version: 2.8.2
-Summary: A Python Library for interacting with the Power BI Rest API.
-Home-page: https://github.com/andrewvillazon/pbipy
-Author: Andrew Villazon
-Author-email: andrew.villazon@gmail.com
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Intended Audience :: System Administrators
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# pbipy
-
-![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
-
-
-`pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
-
-`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
-
-## Installation
-
-```console
-pip install pbipy
-```
-
-Or to install the latest development code:
-
-```console
-pip install git+https://github.com/andrewvillazon/pbipy
-```
-
-## Getting Started: Authentication
-
-To use `pbipy` you'll first need to acquire a `bearer_token`.
-
-*How do I get a `bearer_token`?*
-
-To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
-
-To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
-
-Because there are multiple ways to acquire the token, `pbipy` leaves it up to the user do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
-
-This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
-
-* [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
-* [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
-* [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
-
-The example below uses the `msal` library to to get a bearer_token.
-
-```python
-import msal
-
-
-#  msal auth setup
-def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
-    app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
-    result = app.acquire_token_by_username_password(username, password, scopes)
-    return result["access_token"]
-
-
-bearer_token = acquire_bearer_token(
-    username="your-username",
-    password="your-password",
-    azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
-    client_id="your-pbi-client-id",
-    scopes=["https://analysis.windows.net/powerbi/api/.default"],
-)
-```
-
-The code that follows assumes you've authenticated and acquired your `bearer_token`.
-
-## Useage
-
-Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-```
-
-To interact with the API, simply call the relevant method from the client.
-
-```python
-# Grab the datasets from a workspace
-
-pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-```
-
-`pbipy` converts API responses into regular Python objects, with snake case included! 🐍🐍
-
-```python
-sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-print(type(sales))
-print(hasattr(sales, "configured_by"))
-
-# <class 'pbipy.resources.Dataset'>
-# True
-```
-
-Most methods take in an object id...
-
-```python
-dataset = pbi.dataset(
-    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
-)
-```
-
-... or just pass in the object itself.
-
-```python
-group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
-
-dataset = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
-    ,group=group
-)
-```
-
-If you need to access the raw json representation, this is supported to.
-
-```python
-sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-print(sales.raw)
-
-# {
-#   "id": "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-#   "name": "SalesMarketing",
-#   "addRowsAPIEnabled": False,
-#   "configuredBy": "john@contoso.com",
-#   ...
-# }
-```
-
-## Example: Working with Datasets
-
-Let's see how `pbipy` works by performing some operations on a Dataset.
-
-First, we initialize our client.
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-```
-
-Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
-
-```python
-sales = pbi.dataset(
-    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
-)
-
-print(sales)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
-```
-
-Dataset not updating? Let's look at the Refresh History. 
-
-We call the `refresh_history()` method on our Dataset. Easy.
-
-```python
-refresh_history = sales.refresh_history()
-
-for entry in refresh_history:
-    print(entry)
-
-# {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
-```
-
-Need to kick off a refresh? That's easy too.
-
-```python
-sales.refresh()
-```
-
-How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
-
-```python
-# Give John 'Read' access on the dataset
-sales.add_user("john@contoso.com", "User", "Read")
-```
-
-Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
-
-```python
-dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
-print(dxq_result)
-
-# {
-#   "results": [
-#     {
-#       "tables": [
-#         {
-#           "rows": [
-#             {
-#               "MyTable[Year]": 2010,
-#               "MyTable[Quarter]": "Q1"
-#             },
-# ...
-# }
-```
-
-## Example: Working with the Admin object
-
-`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
-
-First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-admin = pbi.admin()
-```
-
-Need to review some access on some reports? We can call the `report_users` method.
-
-```python
-users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
-print(users[0])
-
-# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
-```
-
-What about understanding User activity on your Power BI tenant?
-
-```python
-from datetime import datetime
-
-start_dtm = datetime(2019, 8, 31, 0, 0, 0)
-end_dtm = datetime(2019, 8, 31, 23, 59, 59)
-
-activity_events = admin.activity_events(start_dtm, end_dtm)
-
-print(activity_events)
-
-# [
-#   {
-#       "Id": "41ce06d1", 
-#       "CreationTime": "2019-08-13T07:55:15", 
-#       "Operation": "ViewReport", 
-#       ...
-#   },
-#   {
-#       "Id": "c632aa64", 
-#       "CreationTime": "2019-08-13T07:55:10", 
-#       "Operation": "GetSnapshots", 
-#       ...
-#   }
-# ]
-```
-
-## More examples
-
-### Datasets in a Workspace
-
-```python
-datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-
-for dataset in datasets:
-    print(dataset)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
-# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
-```
-
-### List Workspaces
-
-```python
-groups = pbi.groups()
-
-for group in groups:
-    print(group)
-
-# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
-# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
-```
-
-### Create a Workspace
-
-```python
-group = pbi.create_group("contoso")
-print(group)
-
-# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
-```
-
-### Users and their access
-
-```python
-group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
-users = group.users()
-
-for user in users:
-    print(user)
-
-# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
-# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
-```
-
-## Power BI Rest API Operations
-
-`pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
-
-[Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
-
-
-## What's implemented?
-
-Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
-
-If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
-
-| PowerBI Component   	| Progress 	| Notes 	                                                                            |
-|---------------------	|----------	|-------------------------------------------------------------------------------------- |
-| Datasets            	| Done     	|       	                                                                            |
-| Groups (Workspaces) 	| Done    	|       	                                                                            |
-| Reports             	| Done      |       	                                                                            |
-| Apps                	| Done   	|       	                                                                            |
-| Dataflows           	| Done    	|       	                                                                            |
-| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
-| Dashboards          	| Todo     	|       	                                                                            |
-| Everything else     	| Backlog  	|       	                                                                            |
-
-## Contributing
-
-`pbipy` is an open source project. Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
-
-View [CONTRIBUTING.md](https://github.com/andrewvillazon/pbipy/blob/master/CONTRIBUTING.md) to learn more about contributing.
-
-## Acknowledgements
-
-The design of this library was heavily inspired by (basically copied) the [pycontribs/jira](https://github.com/pycontribs/jira) library. It also borrows elements of [cmberryay's pypowerbi wrapper](https://github.com/cmberryau/pypowerbi).
-
-Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
+# pbipy
+
+![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
+
+
+`pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
+
+`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
+
+## Installation
+
+```console
+pip install pbipy
+```
+
+Or to install the latest development code:
+
+```console
+pip install git+https://github.com/andrewvillazon/pbipy
+```
+
+## Getting Started: Authentication
+
+To use `pbipy` you'll first need to acquire a `bearer_token`.
+
+*How do I get a `bearer_token`?*
+
+To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
+
+To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
+
+Because there are multiple ways to acquire the token, `pbipy` leaves it up to the user do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
+
+This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
+
+* [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
+* [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
+* [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
+
+The example below uses the `msal` library to to get a bearer_token.
+
+```python
+import msal
+
+
+#  msal auth setup
+def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
+    app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
+    result = app.acquire_token_by_username_password(username, password, scopes)
+    return result["access_token"]
+
+
+bearer_token = acquire_bearer_token(
+    username="your-username",
+    password="your-password",
+    azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
+    client_id="your-pbi-client-id",
+    scopes=["https://analysis.windows.net/powerbi/api/.default"],
+)
+```
+
+The code that follows assumes you've authenticated and acquired your `bearer_token`.
+
+## Useage
+
+Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+```
+
+To interact with the API, simply call the relevant method from the client.
+
+```python
+# Grab the datasets from a workspace
+
+pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
+```
+
+`pbipy` converts API responses into regular Python objects, with snake case included! 🐍🐍
+
+```python
+sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+
+print(type(sales))
+print(hasattr(sales, "configured_by"))
+
+# <class 'pbipy.Dataset'>
+# True
+```
+
+Most methods take in an object id...
+
+```python
+dataset = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
+)
+```
+
+... or just pass in the object itself.
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+
+dataset = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
+    ,group=group
+)
+```
+
+If you need to access the raw json representation, this is supported to.
+
+```python
+sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+
+print(sales.raw)
+
+# {
+#   "id": "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+#   "name": "SalesMarketing",
+#   "addRowsAPIEnabled": False,
+#   "configuredBy": "john@contoso.com",
+#   ...
+# }
+```
+
+## Example: Working with Datasets
+
+Let's see how `pbipy` works by performing some operations on a Dataset.
+
+First, we initialize our client.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+```
+
+Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
+
+```python
+sales = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
+)
+
+print(sales)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
+```
+
+Dataset not updating? Let's look at the Refresh History. 
+
+We call the `refresh_history()` method on our Dataset. Easy.
+
+```python
+refresh_history = sales.refresh_history()
+
+for entry in refresh_history:
+    print(entry)
+
+# {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
+```
+
+Need to kick off a refresh? That's easy too.
+
+```python
+sales.refresh()
+```
+
+How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
+
+```python
+# Give John 'Read' access on the dataset
+sales.add_user("john@contoso.com", "User", "Read")
+```
+
+Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
+
+```python
+dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
+print(dxq_result)
+
+# {
+#   "results": [
+#     {
+#       "tables": [
+#         {
+#           "rows": [
+#             {
+#               "MyTable[Year]": 2010,
+#               "MyTable[Quarter]": "Q1"
+#             },
+# ...
+# }
+```
+
+## Example: Working with the Admin object
+
+`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
+
+First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+admin = pbi.admin()
+```
+
+Need to review some access on some reports? We can call the `report_users` method.
+
+```python
+users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
+print(users[0])
+
+# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
+```
+
+What about understanding User activity on your Power BI tenant?
+
+```python
+from datetime import datetime
+
+start_dtm = datetime(2019, 8, 31, 0, 0, 0)
+end_dtm = datetime(2019, 8, 31, 23, 59, 59)
+
+activity_events = admin.activity_events(start_dtm, end_dtm)
+
+print(activity_events)
+
+# [
+#   {
+#       "Id": "41ce06d1", 
+#       "CreationTime": "2019-08-13T07:55:15", 
+#       "Operation": "ViewReport", 
+#       ...
+#   },
+#   {
+#       "Id": "c632aa64", 
+#       "CreationTime": "2019-08-13T07:55:10", 
+#       "Operation": "GetSnapshots", 
+#       ...
+#   }
+# ]
+```
+
+## More examples
+
+### Datasets in a Workspace
+
+```python
+datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
+
+for dataset in datasets:
+    print(dataset)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
+# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+```
+
+### List Workspaces
+
+```python
+groups = pbi.groups()
+
+for group in groups:
+    print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
+```
+
+### Create a Workspace
+
+```python
+group = pbi.create_group("contoso")
+print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+```
+
+### Users and their access
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+users = group.users()
+
+for user in users:
+    print(user)
+
+# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
+# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
+```
+
+## Power BI Rest API Operations
+
+`pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
+
+[Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
+
+
+## What's implemented?
+
+Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
+
+If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
+
+| PowerBI Component   	| Progress 	| Notes 	                                                                            |
+|---------------------	|----------	|-------------------------------------------------------------------------------------- |
+| Datasets            	| Done     	|       	                                                                            |
+| Groups (Workspaces) 	| Done    	|       	                                                                            |
+| Reports             	| Done      |       	                                                                            |
+| Apps                	| Done   	|       	                                                                            |
+| Dataflows           	| Done    	|       	                                                                            |
+| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
+| Dashboards          	| Todo     	|       	                                                                            |
+| Everything else     	| Backlog  	|       	                                                                            |
+
+## Contributing
+
+`pbipy` is an open source project. Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
+
+View [CONTRIBUTING.md](https://github.com/andrewvillazon/pbipy/blob/master/CONTRIBUTING.md) to learn more about contributing.
+
+## Acknowledgements
+
+The design of this library was heavily inspired by (basically copied) the [pycontribs/jira](https://github.com/pycontribs/jira) library. It also borrows elements of [cmberryay's pypowerbi wrapper](https://github.com/cmberryau/pypowerbi).
+
+Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
```

### Comparing `pbipy-2.8.2/README.md` & `pbipy-2.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: pbipy
+Version: 2.9.0
+Summary: A Python Library for interacting with the Power BI Rest API.
+Home-page: https://github.com/andrewvillazon/pbipy
+Author: Andrew Villazon
+Author-email: andrew.villazon@gmail.com
+License: Apache 2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # pbipy
 
 ![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
 
 
 `pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
 
@@ -83,15 +103,15 @@
 
 ```python
 sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
 
 print(type(sales))
 print(hasattr(sales, "configured_by"))
 
-# <class 'pbipy.resources.Dataset'>
+# <class 'pbipy.Dataset'>
 # True
 ```
 
 Most methods take in an object id...
 
 ```python
 dataset = pbi.dataset(
@@ -326,8 +346,8 @@
 
 View [CONTRIBUTING.md](https://github.com/andrewvillazon/pbipy/blob/master/CONTRIBUTING.md) to learn more about contributing.
 
 ## Acknowledgements
 
 The design of this library was heavily inspired by (basically copied) the [pycontribs/jira](https://github.com/pycontribs/jira) library. It also borrows elements of [cmberryay's pypowerbi wrapper](https://github.com/cmberryau/pypowerbi).
 
-Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
+Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
```

### Comparing `pbipy-2.8.2/pbipy/_utils.py` & `pbipy-2.9.0/pbipy/_utils.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/admin.py` & `pbipy-2.9.0/pbipy/admin.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/apps.py` & `pbipy-2.9.0/pbipy/apps.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/dashboards.py` & `pbipy-2.9.0/pbipy/dashboards.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/dataflows.py` & `pbipy-2.9.0/pbipy/dataflows.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/datasets.py` & `pbipy-2.9.0/pbipy/datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,31 +3,52 @@
 
 Full Dataset Operations documentation can be found at:
 
 https://learn.microsoft.com/en-us/rest/api/power-bi/datasets
 
 """
 
+import time
+
 from requests import Session
 
 from pbipy.resources import Resource
 from pbipy import _utils
 
 
+# TODO: Move to an exceptions.py module
+class DatasetRefreshError(Exception):
+    """Error raised when a Dataset refresh did not complete successfully."""
+
+    def __init__(
+        self,
+        refresh_id: str,
+        status: str,
+        refresh_details: dict,
+    ):
+        self.refresh_id = refresh_id
+        self.status = status
+        self.refresh_details = refresh_details
+
+        message = f"Refresh {self.refresh_id} did not complete successfully. Status: {self.status}. See the 'refresh_details' property for more information."
+
+        super().__init__(message)
+
+
 class Dataset(Resource):
     """
     A Power BI Dataset.
-    
-    Users should initialize a `Dataset` object by calling the `dataset()` 
+
+    Users should initialize a `Dataset` object by calling the `dataset()`
     method on the `PowerBI` client, rather than creating directly.
 
     Examples
     --------
     Retrieving a `Dataset` object using a `pbi` client object.
-    
+
     ```
     >>> my_dataset = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
     ```
 
     """
 
     _REPR = [
@@ -285,33 +306,41 @@
         return _utils.get_raw(
             resource,
             self.session,
         )
 
     def refresh(
         self,
-        notify_option: str,
+        notify_option: str = None,
         apply_refresh_policy: bool = None,
         commit_mode: str = None,
         effective_date: str = None,
         max_parallelism: int = None,
         objects: list[dict] = None,
         retry_count: int = None,
         type: str = None,
-    ) -> None:
+    ) -> str:
         """
-        Trigger a refresh of the dataset. An enhanced refresh is triggered
-        only if a request option other than `notify_option` is set.
+        Triggers a refresh, or enhanced refresh, of the Dataset and returns
+        the generated Refresh Id.
+
+        If no parameters, or only `notify_option`, are provided then a
+        standard refresh is triggered.
+
+        To trigger an enhanced refresh, provide one or more of the optional
+        parameters other than `notify_option`. When the enhanced refresh
+        specifies parameters, the API sets unspecified parameters to their
+        default values.
 
         Parameters
         ----------
-        `notify_option` : `str`
+        `notify_option` : `str`, optional
             Mail notification options, e.g., "MailOnCompletion", "MailOnFailure",
             or "NoNotification".
-        `apply_refresh_policy` : bool, optional
+        `apply_refresh_policy` : `bool`, optional
             Determine if the policy is applied or not.
         `commit_mode` : `str`, optional
             Determines if objects will be committed in batches or only when
             complete, e.g., "PartialBatch", or "Transactional".
         `effective_date` : `str`, optional
             If an incremental refresh policy is applied, the `effective_date`
             parameter overrides the current date.
@@ -330,19 +359,30 @@
             ```
         `retry_count` : `int`, optional
             Number of times the operation will retry before failing.
         `type` : `str`, optional
            The type of processing to perform, e.g., "Automatic", "Calculate",
            "ClearValues", "DataOnly", "Defragment", or "Full".
 
+        Returns
+        -------
+        `str`
+            Refresh Id that was created by triggering the refresh. If the
+            triggered refresh was an enhanced refresh, the Refresh Id can
+            be passed to `Dataset.refresh_details` to retrieve execution
+            details for the refresh.
+
         Notes
         -----
         See here for request options in greater detail:
         https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/refresh-dataset#definitions
 
+        Enhanced refresh with the Power BI REST API:
+        https://learn.microsoft.com/en-us/power-bi/connect-data/asynchronous-refresh
+
         """
 
         refresh_request = {
             "applyRefreshPolicy": apply_refresh_policy,
             "commitMode": commit_mode,
             "effectiveDate": effective_date,
             "maxParallelism": max_parallelism,
@@ -351,20 +391,22 @@
             "retryCount": retry_count,
             "type": type,
         }
 
         prepared_request = _utils.remove_no_values(refresh_request)
         resource = self.base_path + "/refreshes"
 
-        _utils.post(
+        response = _utils.post(
             resource,
             self.session,
             prepared_request,
         )
 
+        return response.headers["RequestId"]
+
     def refresh_details(
         self,
         refresh_id: str,
     ) -> dict:
         """
         Returns execution details of an enhanced refresh operation for
         the dataset.
@@ -383,14 +425,130 @@
 
         resource = self.base_path + f"/refreshes/{refresh_id}"
         return _utils.get_raw(
             resource,
             self.session,
         )
 
+    def refresh_and_wait(
+        self,
+        apply_refresh_policy: bool = None,
+        commit_mode: str = None,
+        effective_date: str = None,
+        max_parallelism: int = None,
+        objects: list[dict] = None,
+        retry_count: int = None,
+        type: str = None,
+        check_interval: int = 30,
+    ) -> None:
+        """
+        Triggers an enhanced refresh of the dataset and periodically checks
+        the refresh status until the refresh operation completes. If the
+        refresh completes successfully, control is returned to the caller.
+        If the refresh did not complete successfully an exception is raised.
+
+        Convenience method that triggers an enhanced refresh using `Dataset.refresh`,
+        and then periodically checks the status of the refresh using `Dataset.refreh_details`.
+        The frequency of checking is set via the `check_interval` parameter.
+
+        Parameters
+        ----------
+        `apply_refresh_policy` : `bool`, optional
+            Determine if the policy is applied or not.
+        `commit_mode` : `str`, optional
+            Determines if objects will be committed in batches or only when
+            complete, e.g., "PartialBatch", or "Transactional".
+        `effective_date` : `str`, optional
+            If an incremental refresh policy is applied, the `effective_date`
+            parameter overrides the current date.
+        `max_parallelism` : `int`, optional
+            The maximum number of threads on which to run parallel processing
+            commands.
+        `objects` : `list[dict]`, optional
+            A list of objects to be processed, e.g.,
+            ```
+            [
+                {
+                "table": "Customer",
+                "partition": "Robert"
+                }
+            ]
+            ```
+        `retry_count` : `int`, optional
+            Number of times the operation will retry before failing.
+        `type` : `str`, optional
+           The type of processing to perform, e.g., "Automatic", "Calculate",
+           "ClearValues", "DataOnly", "Defragment", or "Full".
+        `check_interval` : `int`
+            How often, in seconds, to check the status of the triggered
+            refresh.
+
+        Raises
+        ------
+        `ValueError`
+            If no options were provided for the refresh. At least one of the
+            refresh options must be provided to the endpoint to trigger an enhanced
+            refresh.
+        `DatasetRefreshError`
+            When the refresh status finished with an unsuccessful status.
+
+        Notes
+        -----
+        An enhanced refresh is triggered when additional parameters, other
+        than "notifyOption" are provided to the Refresh Dataset endpoint.
+        Due to the Refresh Execution Details endpoint only supporting enhanced
+        refreshes, this method also only supports enhanced refreshes.
+
+        Enhanced refresh with the Power BI REST API:
+        https://learn.microsoft.com/en-us/power-bi/connect-data/asynchronous-refresh
+
+        Refresh Dataset endpoint:
+        https://learn.microsoft.com/en-us/rest/api/power-bi/datasets/refresh-dataset
+
+        """
+
+        if not any(
+            [
+                apply_refresh_policy,
+                commit_mode,
+                effective_date,
+                max_parallelism,
+                objects,
+                retry_count,
+                type,
+            ]
+        ):
+            raise ValueError(
+                "No options were provided for the refresh. Must provide at least one of: apply_refresh_policy, commit_mode, effective_date, max_parallelism, objects, or retry_count."
+            )
+
+        refresh_id = self.refresh(
+            apply_refresh_policy=apply_refresh_policy,
+            commit_mode=commit_mode,
+            effective_date=effective_date,
+            max_parallelism=max_parallelism,
+            objects=objects,
+            retry_count=retry_count,
+            type=type,
+        )
+
+        refresh_details = self.refresh_details(refresh_id)
+        status = refresh_details.get("status", "Unknown")
+
+        finished = ("Completed", "Failed", "Disabled", "Cancelled")
+
+        while status not in finished:
+            time.sleep(check_interval)
+
+            refresh_details = self.refresh_details(refresh_id)
+            status = refresh_details.get("status", "Unknown")
+
+        if status != "Completed":
+            raise DatasetRefreshError(refresh_id, status, refresh_details)
+
     def refresh_history(
         self,
         top: int = None,
     ) -> list[dict]:
         """
         Returns the refresh history for the dataset.
```

### Comparing `pbipy-2.8.2/pbipy/groups.py` & `pbipy-2.9.0/pbipy/groups.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/powerbi.py` & `pbipy-2.9.0/pbipy/powerbi.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy/reports.py` & `pbipy-2.9.0/pbipy/reports.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 
 """
 
 import mimetypes
 from pathlib import Path
 
 from requests import Session
+import gzip
+from urllib.request import Request, urlopen
 
 from pbipy.datasets import Dataset
+from pbipy.embedtokens import EmbedToken
 from pbipy.groups import Group
 from pbipy.resources import Resource
 from pbipy import _utils
 
 
 class Report(Resource):
     """
@@ -171,18 +174,25 @@
         file_path = _utils.file_path_from_components(
             file_name=f_name,
             extension=ext,
             directory=save_to,
         )
 
         resource = self.base_path + "/Export"
-        response = _utils.get(resource, self.session)
-
-        with open(file_path, "wb") as out_file:
-            out_file.write(response.content)
+        request = Request(resource, headers=self.session.headers)
+        with (
+            urlopen(request) as response,
+            gzip.GzipFile(fileobj=response, mode="rb") as uncompressed,
+            open(file_path, "wb") as out_file,
+        ):
+            while True:
+                chunk = uncompressed.read(1024 * 1024)
+                if not chunk:
+                    break
+                out_file.write(chunk)
 
     def download_export(
         self,
         id,
         save_to: str | Path = None,
         file_name: str = None,
     ) -> None:
@@ -294,14 +304,91 @@
             except:
                 retry_after = None
 
             return raw, retry_after
         else:
             return raw
 
+    def generate_token(
+        self,
+        access_level: str = None,
+        allow_save_as: bool = None,
+        dataset_id: str = None,
+        identities: list[dict] = None,
+        lifetime_in_minutes: int = None,
+    ) -> EmbedToken:
+        """
+        Generates an Embed Token to view or edit the Report from the it's
+        workspace.
+
+        Parameters
+        ----------
+        `access_level` : `str`, optional
+            The required access level. Can be one of "Create", "Edit",
+            or "View".
+        `allow_save_as` : `bool`, optional
+            Whether an embedded report can be saved as a new report. API
+            defaults to `false`. Only applies when you generate an embed
+            token for report embedding.
+        `dataset_id` : `str`, optional
+            The dataset ID used for report creation. Only applies when you
+            generate an embed token for report creation.
+        `identities` : `list[dict]`, optional
+            A list of identities to use for row-level security rules. See
+            'Notes' below for documentation describing how to define these.
+        `lifetime_in_minutes` : `int`, optional
+            The maximum lifetime of the token in minutes, starting from
+            the time it was generated. Can be used to shorten the expiration
+            time of a token, but not to extend it. The value must be a positive
+            integer. Zero (0) is equivalent to `null` and will be ignored,
+            resulting in the default expiration time.
+
+        Returns
+        -------
+        `EmbedToken`
+            A Power BI Embed Token.
+
+        Raises
+        ------
+        `TypeError`
+            If the report does not have a `group_id` property, i.e., the
+            report is not in a Workspace.
+
+        Notes
+        -----
+        See below for API Documentation and how to define parameter options.
+
+        https://learn.microsoft.com/en-us/rest/api/power-bi/embed-token/reports-generate-token-for-create-in-group
+
+        """
+
+        if not self.group_id:
+            raise TypeError(
+                "Report does not have a 'group_id'. Generating a token can only be performed on a Report in a Group (Workspace)."
+            )
+
+        initial_payload = {
+            "accessLevel": access_level,
+            "allowSaveAs": allow_save_as,
+            "datasetId": dataset_id,
+            "identities": identities,
+            "lifetimeInMinutes": lifetime_in_minutes,
+        }
+
+        payload = _utils.remove_no_values(initial_payload)
+
+        resource = self.base_path + "/GenerateToken"
+        raw = _utils.post_raw(resource, self.session, payload)
+
+        return EmbedToken(
+            token=raw["token"],
+            token_id=raw["tokenId"],
+            expiration=raw["expiration"],
+        )
+
     def page(
         self,
         name: str,
     ) -> dict:
         """
         Returns the specified page from the report.
```

### Comparing `pbipy-2.8.2/pbipy/resources.py` & `pbipy-2.9.0/pbipy/resources.py`

 * *Files identical despite different names*

### Comparing `pbipy-2.8.2/pbipy.egg-info/PKG-INFO` & `pbipy-2.9.0/pbipy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-Metadata-Version: 2.1
-Name: pbipy
-Version: 2.8.2
-Summary: A Python Library for interacting with the Power BI Rest API.
-Home-page: https://github.com/andrewvillazon/pbipy
-Author: Andrew Villazon
-Author-email: andrew.villazon@gmail.com
-License: Apache 2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Intended Audience :: System Administrators
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-# pbipy
-
-![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
-
-
-`pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
-
-`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
-
-## Installation
-
-```console
-pip install pbipy
-```
-
-Or to install the latest development code:
-
-```console
-pip install git+https://github.com/andrewvillazon/pbipy
-```
-
-## Getting Started: Authentication
-
-To use `pbipy` you'll first need to acquire a `bearer_token`.
-
-*How do I get a `bearer_token`?*
-
-To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
-
-To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
-
-Because there are multiple ways to acquire the token, `pbipy` leaves it up to the user do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
-
-This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
-
-* [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
-* [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
-* [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
-
-The example below uses the `msal` library to to get a bearer_token.
-
-```python
-import msal
-
-
-#  msal auth setup
-def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
-    app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
-    result = app.acquire_token_by_username_password(username, password, scopes)
-    return result["access_token"]
-
-
-bearer_token = acquire_bearer_token(
-    username="your-username",
-    password="your-password",
-    azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
-    client_id="your-pbi-client-id",
-    scopes=["https://analysis.windows.net/powerbi/api/.default"],
-)
-```
-
-The code that follows assumes you've authenticated and acquired your `bearer_token`.
-
-## Useage
-
-Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-```
-
-To interact with the API, simply call the relevant method from the client.
-
-```python
-# Grab the datasets from a workspace
-
-pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-```
-
-`pbipy` converts API responses into regular Python objects, with snake case included! 🐍🐍
-
-```python
-sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-print(type(sales))
-print(hasattr(sales, "configured_by"))
-
-# <class 'pbipy.resources.Dataset'>
-# True
-```
-
-Most methods take in an object id...
-
-```python
-dataset = pbi.dataset(
-    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
-)
-```
-
-... or just pass in the object itself.
-
-```python
-group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
-
-dataset = pbi.dataset(
-    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
-    ,group=group
-)
-```
-
-If you need to access the raw json representation, this is supported to.
-
-```python
-sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
-
-print(sales.raw)
-
-# {
-#   "id": "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-#   "name": "SalesMarketing",
-#   "addRowsAPIEnabled": False,
-#   "configuredBy": "john@contoso.com",
-#   ...
-# }
-```
-
-## Example: Working with Datasets
-
-Let's see how `pbipy` works by performing some operations on a Dataset.
-
-First, we initialize our client.
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-```
-
-Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
-
-```python
-sales = pbi.dataset(
-    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
-    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
-)
-
-print(sales)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
-```
-
-Dataset not updating? Let's look at the Refresh History. 
-
-We call the `refresh_history()` method on our Dataset. Easy.
-
-```python
-refresh_history = sales.refresh_history()
-
-for entry in refresh_history:
-    print(entry)
-
-# {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
-```
-
-Need to kick off a refresh? That's easy too.
-
-```python
-sales.refresh()
-```
-
-How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
-
-```python
-# Give John 'Read' access on the dataset
-sales.add_user("john@contoso.com", "User", "Read")
-```
-
-Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
-
-```python
-dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
-print(dxq_result)
-
-# {
-#   "results": [
-#     {
-#       "tables": [
-#         {
-#           "rows": [
-#             {
-#               "MyTable[Year]": 2010,
-#               "MyTable[Quarter]": "Q1"
-#             },
-# ...
-# }
-```
-
-## Example: Working with the Admin object
-
-`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
-
-First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
-
-```python
-from pbipy import PowerBI
-
-pbi = PowerBI(bearer_token)
-admin = pbi.admin()
-```
-
-Need to review some access on some reports? We can call the `report_users` method.
-
-```python
-users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
-print(users[0])
-
-# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
-```
-
-What about understanding User activity on your Power BI tenant?
-
-```python
-from datetime import datetime
-
-start_dtm = datetime(2019, 8, 31, 0, 0, 0)
-end_dtm = datetime(2019, 8, 31, 23, 59, 59)
-
-activity_events = admin.activity_events(start_dtm, end_dtm)
-
-print(activity_events)
-
-# [
-#   {
-#       "Id": "41ce06d1", 
-#       "CreationTime": "2019-08-13T07:55:15", 
-#       "Operation": "ViewReport", 
-#       ...
-#   },
-#   {
-#       "Id": "c632aa64", 
-#       "CreationTime": "2019-08-13T07:55:10", 
-#       "Operation": "GetSnapshots", 
-#       ...
-#   }
-# ]
-```
-
-## More examples
-
-### Datasets in a Workspace
-
-```python
-datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
-
-for dataset in datasets:
-    print(dataset)
-
-# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
-# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
-```
-
-### List Workspaces
-
-```python
-groups = pbi.groups()
-
-for group in groups:
-    print(group)
-
-# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
-# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
-```
-
-### Create a Workspace
-
-```python
-group = pbi.create_group("contoso")
-print(group)
-
-# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
-```
-
-### Users and their access
-
-```python
-group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
-users = group.users()
-
-for user in users:
-    print(user)
-
-# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
-# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
-```
-
-## Power BI Rest API Operations
-
-`pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
-
-[Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
-
-
-## What's implemented?
-
-Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
-
-If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
-
-| PowerBI Component   	| Progress 	| Notes 	                                                                            |
-|---------------------	|----------	|-------------------------------------------------------------------------------------- |
-| Datasets            	| Done     	|       	                                                                            |
-| Groups (Workspaces) 	| Done    	|       	                                                                            |
-| Reports             	| Done      |       	                                                                            |
-| Apps                	| Done   	|       	                                                                            |
-| Dataflows           	| Done    	|       	                                                                            |
-| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
-| Dashboards          	| Todo     	|       	                                                                            |
-| Everything else     	| Backlog  	|       	                                                                            |
-
-## Contributing
-
-`pbipy` is an open source project. Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
-
-View [CONTRIBUTING.md](https://github.com/andrewvillazon/pbipy/blob/master/CONTRIBUTING.md) to learn more about contributing.
-
-## Acknowledgements
-
-The design of this library was heavily inspired by (basically copied) the [pycontribs/jira](https://github.com/pycontribs/jira) library. It also borrows elements of [cmberryay's pypowerbi wrapper](https://github.com/cmberryau/pypowerbi).
-
-Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
+Metadata-Version: 2.1
+Name: pbipy
+Version: 2.9.0
+Summary: A Python Library for interacting with the Power BI Rest API.
+Home-page: https://github.com/andrewvillazon/pbipy
+Author: Andrew Villazon
+Author-email: andrew.villazon@gmail.com
+License: Apache 2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Intended Audience :: System Administrators
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+# pbipy
+
+![PyPI](https://img.shields.io/pypi/v/pbipy) ![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/andrewvillazon/pbipy) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pbipy) ![GitHub](https://img.shields.io/github/license/andrewvillazon/pbipy) ![Static Badge](https://img.shields.io/badge/Python-blue?logo=python&logoColor=yellow) ![Static Badge](https://img.shields.io/badge/power-bi-yellow?logoColor=yellow&labelColor=yellow&color=black)
+
+
+`pbipy` is a Python Library for interacting with the Power BI Rest API. It aims to simplyify working with the Power BI Rest API and support programatic administration of Power BI in Python.
+
+`pbipy` supports operations for Apps, Dataflows, Datasets, Reports, and Workspaces (Groups), allowing users to perform actions on their PowerBI instance using Python.
+
+## Installation
+
+```console
+pip install pbipy
+```
+
+Or to install the latest development code:
+
+```console
+pip install git+https://github.com/andrewvillazon/pbipy
+```
+
+## Getting Started: Authentication
+
+To use `pbipy` you'll first need to acquire a `bearer_token`.
+
+*How do I get a `bearer_token`?*
+
+To acquire a `bearer_token` you'll need to authenticate against your [Registered Azure Power BI App](https://learn.microsoft.com/en-us/power-bi/developer/embedded/register-app?tabs=customers). Registering is the first step in turning on the Power BI Rest API, so from here on it's assumed your Power BI Rest API is up and running.
+
+To authenticate against the Registered App, Microsoft provides the `MSAL` and `azure-identity` python libraries. These libraries support different ways of acquiring a `bearer_token` and which to use will depend on how your cloud/tenant is configured.
+
+Because there are multiple ways to acquire the token, `pbipy` leaves it up to the user do this in the way that suits, rather than directly handling authentication (of course, this might change in future).
+
+This `README` doesn't cover authentication in detail, however, these are some helpful resources that look at acquiring a `bearer_token` in the context of Power BI:
+
+* [Power BI REST API with Python and MSAL. Part II.](https://www.datalineo.com/post/power-bi-rest-api-with-python-and-msal-part-ii)
+* [Power BI REST API with Python Part III, azure-identity](https://www.datalineo.com/post/power-bi-rest-api-with-python-part-iii-azure-identity)
+* [Monitoring Power BI using REST APIs from Python](https://data-goblins.com/power-bi/power-bi-api-python)
+
+The example below uses the `msal` library to to get a bearer_token.
+
+```python
+import msal
+
+
+#  msal auth setup
+def acquire_bearer_token(username, password, azure_tenant_id, client_id, scopes):
+    app = msal.PublicClientApplication(client_id, authority=azure_tenant_id)
+    result = app.acquire_token_by_username_password(username, password, scopes)
+    return result["access_token"]
+
+
+bearer_token = acquire_bearer_token(
+    username="your-username",
+    password="your-password",
+    azure_tenant_id="https://login.microsoftonline.com/your-azure-tenant-id",
+    client_id="your-pbi-client-id",
+    scopes=["https://analysis.windows.net/powerbi/api/.default"],
+)
+```
+
+The code that follows assumes you've authenticated and acquired your `bearer_token`.
+
+## Useage
+
+Start by creating the `PowerBI()` client. Interactions with the Power BI Rest API go through this object. 
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+```
+
+To interact with the API, simply call the relevant method from the client.
+
+```python
+# Grab the datasets from a workspace
+
+pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
+```
+
+`pbipy` converts API responses into regular Python objects, with snake case included! 🐍🐍
+
+```python
+sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+
+print(type(sales))
+print(hasattr(sales, "configured_by"))
+
+# <class 'pbipy.Dataset'>
+# True
+```
+
+Most methods take in an object id...
+
+```python
+dataset = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="a2f89923-421a-464e-bf4c-25eab39bb09f"
+)
+```
+
+... or just pass in the object itself.
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+
+dataset = pbi.dataset(
+    "cfafbeb1-8037-4d0c-896e-a46fb27ff229"
+    ,group=group
+)
+```
+
+If you need to access the raw json representation, this is supported to.
+
+```python
+sales = pbi.dataset("cfafbeb1-8037-4d0c-896e-a46fb27ff229")
+
+print(sales.raw)
+
+# {
+#   "id": "cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+#   "name": "SalesMarketing",
+#   "addRowsAPIEnabled": False,
+#   "configuredBy": "john@contoso.com",
+#   ...
+# }
+```
+
+## Example: Working with Datasets
+
+Let's see how `pbipy` works by performing some operations on a Dataset.
+
+First, we initialize our client.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+```
+
+Now that we've got a client, we can load a Dataset from the API. To load a Dataset, we call the `dataset()` method with an `id` and `group` argument. In the Power BI Rest API, a **Group** and **Workspace** are synonymous and used interchangeably.
+
+```python
+sales = pbi.dataset(
+    id="cfafbeb1-8037-4d0c-896e-a46fb27ff229",
+    group="f089354e-8366-4e18-aea3-4cb4a3a50b48",
+)
+
+print(sales)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', name='SalesMarketing', ...>
+```
+
+Dataset not updating? Let's look at the Refresh History. 
+
+We call the `refresh_history()` method on our Dataset. Easy.
+
+```python
+refresh_history = sales.refresh_history()
+
+for entry in refresh_history:
+    print(entry)
+
+# {"refreshType":"ViaApi", "startTime":"2017-06-13T09:25:43.153Z", "status": "Completed" ...}
+```
+
+Need to kick off a refresh? That's easy too.
+
+```python
+sales.refresh()
+```
+
+How about adding some user permissions to our Dataset? Just call the `add_user()` method with the User's details and permissions.
+
+```python
+# Give John 'Read' access on the dataset
+sales.add_user("john@contoso.com", "User", "Read")
+```
+
+Lastly, if we're feeling adventurous, we can execute DAX against a Dataset and use the results in Python.
+
+```python
+dxq_result = sales.execute_queries("EVALUATE VALUES(MyTable)")
+print(dxq_result)
+
+# {
+#   "results": [
+#     {
+#       "tables": [
+#         {
+#           "rows": [
+#             {
+#               "MyTable[Year]": 2010,
+#               "MyTable[Quarter]": "Q1"
+#             },
+# ...
+# }
+```
+
+## Example: Working with the Admin object
+
+`pbypi` also supports [Administrator Operations](https://learn.microsoft.com/en-us/rest/api/power-bi/admin), specialized operations available to users with Power BI Admin rights. Let's see how we can use these.
+
+First, we need to initialize our client. Then we call the `admin` method and initialize an `Admin` object.
+
+```python
+from pbipy import PowerBI
+
+pbi = PowerBI(bearer_token)
+admin = pbi.admin()
+```
+
+Need to review some access on some reports? We can call the `report_users` method.
+
+```python
+users = admin.report_users("5b218778-e7a5-4d73-8187-f10824047715")
+print(users[0])
+
+# {"displayName": "John Nick", "emailAddress": "john@contoso.com", ...}
+```
+
+What about understanding User activity on your Power BI tenant?
+
+```python
+from datetime import datetime
+
+start_dtm = datetime(2019, 8, 31, 0, 0, 0)
+end_dtm = datetime(2019, 8, 31, 23, 59, 59)
+
+activity_events = admin.activity_events(start_dtm, end_dtm)
+
+print(activity_events)
+
+# [
+#   {
+#       "Id": "41ce06d1", 
+#       "CreationTime": "2019-08-13T07:55:15", 
+#       "Operation": "ViewReport", 
+#       ...
+#   },
+#   {
+#       "Id": "c632aa64", 
+#       "CreationTime": "2019-08-13T07:55:10", 
+#       "Operation": "GetSnapshots", 
+#       ...
+#   }
+# ]
+```
+
+## More examples
+
+### Datasets in a Workspace
+
+```python
+datasets = pbi.datasets(group="f089354e-8366-4e18-aea3-4cb4a3a50b48")
+
+for dataset in datasets:
+    print(dataset)
+
+# <Dataset id='cfafbeb1-8037-4d0c-896e-a46fb27ff229', ...>
+# <Dataset id='f7fc6510-e151-42a3-850b-d0805a391db0', ...>
+```
+
+### List Workspaces
+
+```python
+groups = pbi.groups()
+
+for group in groups:
+    print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+# <Group id='3d9b93c6-7b6d-4801-a491-1738910904fd', name='marketing'>
+```
+
+### Create a Workspace
+
+```python
+group = pbi.create_group("contoso")
+print(group)
+
+# <Group id='a2f89923-421a-464e-bf4c-25eab39bb09f', name='contoso'>
+```
+
+### Users and their access
+
+```python
+group = pbi.group("a2f89923-421a-464e-bf4c-25eab39bb09f")
+users = group.users()
+
+for user in users:
+    print(user)
+
+# {"identifier": "john@contoso.com", "groupUserAccessRight": "Admin", ... }
+# {"identifier": "Adam@contoso.com", "groupUserAccessRight": "Member", ... }
+```
+
+## Power BI Rest API Operations
+
+`pbipy` methods wrap around the Operations described in the Power BI Rest API Reference:
+
+[Power BI REST APIs for embedded analytics and automation - Power BI REST API](https://learn.microsoft.com/en-us/rest/api/power-bi/)
+
+
+## What's implemented?
+
+Most of the core operations on Datasets, Workspaces (Groups), Reports, Apps, and Dataflows are implemented. Given the many available endpoints, not everything is covered by `pbipy`, so expect a few features to be missing.
+
+If an operation is missing and you think it'd be useful, feel free to suggest it on the [Issues tab](https://github.com/andrewvillazon/pbipy/issues).
+
+| PowerBI Component   	| Progress 	| Notes 	                                                                            |
+|---------------------	|----------	|-------------------------------------------------------------------------------------- |
+| Datasets            	| Done     	|       	                                                                            |
+| Groups (Workspaces) 	| Done    	|       	                                                                            |
+| Reports             	| Done      |       	                                                                            |
+| Apps                	| Done   	|       	                                                                            |
+| Dataflows           	| Done    	|       	                                                                            |
+| Admin Operations     	| Done    	| Implements operations related to Datasets, Groups, Reports, Apps, and Dataflows only. |
+| Dashboards          	| Todo     	|       	                                                                            |
+| Everything else     	| Backlog  	|       	                                                                            |
+
+## Contributing
+
+`pbipy` is an open source project. Contributions such as bug reports, fixes, documentation or docstrings, enhancements, and ideas are welcome. `pbipy` uses github to host code, track issues, record feature requests, and accept pull requests.
+
+View [CONTRIBUTING.md](https://github.com/andrewvillazon/pbipy/blob/master/CONTRIBUTING.md) to learn more about contributing.
+
+## Acknowledgements
+
+The design of this library was heavily inspired by (basically copied) the [pycontribs/jira](https://github.com/pycontribs/jira) library. It also borrows elements of [cmberryay's pypowerbi wrapper](https://github.com/cmberryau/pypowerbi).
+
+Thank You to all the contributors to these libraries for the great examples of what an API Wrapper can be.
```

### Comparing `pbipy-2.8.2/setup.py` & `pbipy-2.9.0/setup.py`

 * *Files identical despite different names*

