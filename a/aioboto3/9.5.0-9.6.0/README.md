# Comparing `tmp/aioboto3-9.5.0.tar.gz` & `tmp/aioboto3-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioboto3-9.5.0.tar", max compression
+gzip compressed data, was "aioboto3-9.6.0.tar", max compression
```

## Comparing `aioboto3-9.5.0.tar` & `aioboto3-9.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11314 2022-03-29 20:05:32.560129 aioboto3-9.5.0/LICENSE
--rw-r--r--   0        0        0     7493 2022-03-29 20:05:32.560129 aioboto3-9.5.0/README.rst
--rw-r--r--   0        0        0      503 2022-03-29 20:05:44.528196 aioboto3-9.5.0/aioboto3/__init__.py
--rw-r--r--   0        0        0        0 2022-03-29 20:05:32.560129 aioboto3-9.5.0/aioboto3/dynamodb/__init__.py
--rw-r--r--   0        0        0     5016 2022-03-29 20:05:32.560129 aioboto3-9.5.0/aioboto3/dynamodb/table.py
--rw-r--r--   0        0        0        0 2022-03-29 20:05:32.560129 aioboto3-9.5.0/aioboto3/experimental/__init__.py
--rw-r--r--   0        0        0     1656 2022-03-29 20:05:32.560129 aioboto3-9.5.0/aioboto3/experimental/async_chalice.py
--rw-r--r--   0        0        0        0 2022-03-29 20:05:32.560129 aioboto3-9.5.0/aioboto3/resources/__init__.py
--rw-r--r--   0        0        0     4472 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/resources/action.py
--rw-r--r--   0        0        0      489 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/resources/base.py
--rw-r--r--   0        0        0     6585 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/resources/collection.py
--rw-r--r--   0        0        0    10611 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/resources/factory.py
--rw-r--r--   0        0        0     3954 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/resources/response.py
--rw-r--r--   0        0        0        0 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/s3/__init__.py
--rw-r--r--   0        0        0    22847 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/s3/cse.py
--rw-r--r--   0        0        0    15288 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/s3/inject.py
--rw-r--r--   0        0        0     9742 2022-03-29 20:05:32.564129 aioboto3-9.5.0/aioboto3/session.py
--rw-r--r--   0        0        0     1596 2022-03-29 20:05:44.528196 aioboto3-9.5.0/pyproject.toml
--rw-r--r--   0        0        0     8583 2022-03-29 20:05:44.938538 aioboto3-9.5.0/setup.py
--rw-r--r--   0        0        0     8582 2022-03-29 20:05:44.939735 aioboto3-9.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11314 2022-05-06 19:14:21.969159 aioboto3-9.6.0/LICENSE
+-rw-r--r--   0        0        0     7493 2022-05-06 19:14:21.969159 aioboto3-9.6.0/README.rst
+-rw-r--r--   0        0        0      503 2022-05-06 19:14:28.925243 aioboto3-9.6.0/aioboto3/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/dynamodb/__init__.py
+-rw-r--r--   0        0        0     5016 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/dynamodb/table.py
+-rw-r--r--   0        0        0        0 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/experimental/__init__.py
+-rw-r--r--   0        0        0     1656 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/experimental/async_chalice.py
+-rw-r--r--   0        0        0        0 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/__init__.py
+-rw-r--r--   0        0        0     4472 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/action.py
+-rw-r--r--   0        0        0      489 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/base.py
+-rw-r--r--   0        0        0     6585 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/collection.py
+-rw-r--r--   0        0        0    10611 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/factory.py
+-rw-r--r--   0        0        0     3954 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/resources/response.py
+-rw-r--r--   0        0        0        0 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/s3/__init__.py
+-rw-r--r--   0        0        0    22847 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/s3/cse.py
+-rw-r--r--   0        0        0    15288 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/s3/inject.py
+-rw-r--r--   0        0        0     9742 2022-05-06 19:14:21.969159 aioboto3-9.6.0/aioboto3/session.py
+-rw-r--r--   0        0        0     1596 2022-05-06 19:14:28.925243 aioboto3-9.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8583 2022-05-06 19:14:29.270388 aioboto3-9.6.0/setup.py
+-rw-r--r--   0        0        0     8582 2022-05-06 19:14:29.271452 aioboto3-9.6.0/PKG-INFO
```

### Comparing `aioboto3-9.5.0/LICENSE` & `aioboto3-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/README.rst` & `aioboto3-9.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/dynamodb/table.py` & `aioboto3-9.6.0/aioboto3/dynamodb/table.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/experimental/async_chalice.py` & `aioboto3-9.6.0/aioboto3/experimental/async_chalice.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/resources/action.py` & `aioboto3-9.6.0/aioboto3/resources/action.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/resources/collection.py` & `aioboto3-9.6.0/aioboto3/resources/collection.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/resources/factory.py` & `aioboto3-9.6.0/aioboto3/resources/factory.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/resources/response.py` & `aioboto3-9.6.0/aioboto3/resources/response.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/s3/cse.py` & `aioboto3-9.6.0/aioboto3/s3/cse.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/s3/inject.py` & `aioboto3-9.6.0/aioboto3/s3/inject.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/aioboto3/session.py` & `aioboto3-9.6.0/aioboto3/session.py`

 * *Files identical despite different names*

### Comparing `aioboto3-9.5.0/pyproject.toml` & `aioboto3-9.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioboto3"
-version = "9.5.0"
+version = "9.6.0"
 description = "Async boto3 wrapper"
 authors = ["Terry Cain <terry@terrys-home.co.uk>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://github.com/terrycain/aioboto3"
 repository = "https://github.com/terrycain/aioboto3"
 documentation = "https://readthedocs.org/projects/aioboto3/"
@@ -19,15 +19,15 @@
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aiobotocore = {version = "2.2.0", extras = ["boto3"]}
+aiobotocore = {version = "2.3.0", extras = ["boto3"]}
 cryptography = {version = ">=2.3.1", optional = true}
 chalice = {version = ">=1.24.0", optional = true}
 
 [tool.poetry.extras]
 s3cse = ["cryptography"]
 chalice = ["chalice"]
```

### Comparing `aioboto3-9.5.0/setup.py` & `aioboto3-9.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
  'aioboto3.resources',
  'aioboto3.s3']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['aiobotocore[boto3]==2.2.0']
+['aiobotocore[boto3]==2.3.0']
 
 extras_require = \
 {'chalice': ['chalice>=1.24.0'], 's3cse': ['cryptography>=2.3.1']}
 
 setup_kwargs = {
     'name': 'aioboto3',
-    'version': '9.5.0',
+    'version': '9.6.0',
     'description': 'Async boto3 wrapper',
     'long_description': '========================\nAsync AWS SDK for Python\n========================\n\n\n.. image:: https://img.shields.io/pypi/v/aioboto3.svg\n        :target: https://pypi.python.org/pypi/aioboto3\n\n.. image:: https://github.com/terrycain/aioboto3/actions/workflows/CI.yml/badge.svg\n        :target: https://github.com/terrycain/aioboto3/actions\n\n.. image:: https://readthedocs.org/projects/aioboto3/badge/?version=latest\n        :target: https://aioboto3.readthedocs.io\n        :alt: Documentation Status\n\n.. image:: https://pyup.io/repos/github/terrycain/aioboto3/shield.svg\n     :target: https://pyup.io/repos/github/terrycain/aioboto3/\n     :alt: Updates\n\n**Breaking changes for v9, aioboto3.resource and aioboto3.client methods no longer exist, make a session then call session.client etc...**\nThis was done for various reasons but mainly that it prevents the default session living longer than it should as that breaks situations where eventloops are replaced.\n\n**The .client and .resource functions must now be used as async context managers.**\n\nNow that aiobotocore has reached version 1.0.1, a side effect of the work put in to fix various issues like bucket region redirection and\nsupporting web assume role type credentials, the client must now be instantiated using a context manager, which by extension applies to\nthe resource creator. You used to get away with calling ``res = aioboto3.resource(\'dynamodb\')`` but that no longer works. If you really want\nto do that, you can do ``res = await aioboto3.resource(\'dynamodb\').__aenter__()`` but you\'ll need to remember to call ``__aexit__``.\n\nThere will most likely be some parts that dont work now which I\'ve missed, just make an issue and we\'ll get them resoved quickly.\n\nCreating service resources must also be async now, e.g.\n\n.. code-block:: python\n\n    async def main():\n        session = aioboto3.Session()\n        async with session.resource("s3") as s3:\n            bucket = await s3.Bucket(\'mybucket\')  # <----------------\n            async for s3_object in bucket.objects.all():\n                print(s3_object)\n\n\nUpdating to aiobotocore 1.0.1 also brings with it support for running inside EKS as well as asyncifying ``get_presigned_url``\n\n----\n\nThis package is mostly just a wrapper combining the great work of boto3_ and aiobotocore_.\n\naiobotocore allows you to use near enough all of the boto3 client commands in an async manner just by prefixing the command with ``await``.\n\nWith aioboto3 you can now use the higher level APIs provided by boto3 in an asynchronous manner. Mainly I developed this as I wanted to use the boto3 dynamodb Table object in some async\nmicroservices.\n\nWhile all resources in boto3 should work I havent tested them all, so if what your after is not in the table below then try it out, if it works drop me an issue with a simple test case\nand I\'ll add it to the table.\n\n+---------------------------+--------------------+\n| Services                  | Status             |\n+===========================+====================+\n| DynamoDB Service Resource | Tested and working |\n+---------------------------+--------------------+\n| DynamoDB Table            | Tested and working |\n+---------------------------+--------------------+\n| S3                        | Working            |\n+---------------------------+--------------------+\n| Kinesis                   | Working            |\n+---------------------------+--------------------+\n| SSM Parameter Store       | Working            |\n+---------------------------+--------------------+\n| Athena                    | Working            |\n+---------------------------+--------------------+\n\n\nExample\n-------\n\nSimple example of using aioboto3 to put items into a dynamodb table\n\n.. code-block:: python\n\n    import asyncio\n    import aioboto3\n    from boto3.dynamodb.conditions import Key\n\n\n    async def main():\n        session = aioboto3.Session()\n        async with session.resource(\'dynamodb\', region_name=\'eu-central-1\') as dynamo_resource:\n            table = await dynamo_resource.Table(\'test_table\')\n\n            await table.put_item(\n                Item={\'pk\': \'test1\', \'col1\': \'some_data\'}\n            )\n\n            result = await table.query(\n                KeyConditionExpression=Key(\'pk\').eq(\'test1\')\n            )\n\n            # Example batch write\n            more_items = [{\'pk\': \'t2\', \'col1\': \'c1\'}, \\\n                          {\'pk\': \'t3\', \'col1\': \'c3\'}]\n            async with table.batch_writer() as batch:\n                for item_ in more_items:\n                    await batch.put_item(Item=item_)\n\n    loop = asyncio.get_event_loop()\n    loop.run_until_complete(main())\n\n    # Outputs:\n    #  [{\'col1\': \'some_data\', \'pk\': \'test1\'}]\n\n\nThings that either dont work or have been patched\n-------------------------------------------------\n\nAs this library literally wraps boto3, its inevitable that some things won\'t magically be async.\n\nFixed:\n\n- ``s3_client.download_file*``  This is performed by the s3transfer module. -- Patched with get_object\n- ``s3_client.upload_file*``  This is performed by the s3transfer module. -- Patched with custom multipart upload\n- ``s3_client.copy``  This is performed by the s3transfer module. -- Patched to use get_object -> upload_fileobject\n- ``dynamodb_resource.Table.batch_writer``  This now returns an async context manager which performs the same function\n- Resource waiters - You can now await waiters which are part of resource objects, not just client waiters, e.g. ``await dynamodbtable.wait_until_exists()``\n- Resource object properties are normally autoloaded, now they are all co-routines and the metadata they come from will be loaded on first await and then cached thereafter.\n- S3 Bucket.objects object now works and has been asyncified. Examples here - https://aioboto3.readthedocs.io/en/latest/usage.html#s3-resource-objects\n\n\nAmazon S3 Client-Side Encryption\n--------------------------------\n\nBoto3 doesn\'t support AWS client-side encryption so until they do I\'ve added basic support for it. Docs here CSE_\n\nCSE requires the python ``cryptography`` library so if you do ``pip install aioboto3[s3cse]`` that\'ll also include cryptography.\n\nThis library currently supports client-side encryption using KMS-Managed master keys performing envelope encryption\nusing either AES/CBC/PKCS5Padding or preferably AES/GCM/NoPadding. The files generated are compatible with the Java Encryption SDK\nso I will assume they are compatible with the Ruby, PHP, Go and C++ libraries as well.\n\nNon-KMS managed keys are not yet supported but if you have use of that, raise an issue and i\'ll look into it.\n\n\n\nDocumentation\n-------------\n\nDocs are here - https://aioboto3.readthedocs.io/en/latest/\n\nExamples here - https://aioboto3.readthedocs.io/en/latest/usage.html\n\n\nFeatures\n========\n\n* Closely mimics the usage of boto3.\n\nTodo\n====\n\n* More examples\n* Set up docs\n* Look into monkey-patching the aws xray sdk to be more async if it needs to be.\n\n\nCredits\n-------\n\nThis package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.\nIt also makes use of the aiobotocore_ and boto3_ libraries. All the credit goes to them, this is mainly a wrapper with some examples.\n\n.. _aiobotocore: https://github.com/aio-libs/aiobotocore\n.. _boto3: https://github.com/boto/boto3\n.. _Cookiecutter: https://github.com/audreyr/cookiecutter\n.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage\n.. _CSE: https://aioboto3.readthedocs.io/en/latest/cse.html\n',
     'author': 'Terry Cain',
     'author_email': 'terry@terrys-home.co.uk',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/terrycain/aioboto3',
```

### Comparing `aioboto3-9.5.0/PKG-INFO` & `aioboto3-9.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioboto3
-Version: 9.5.0
+Version: 9.6.0
 Summary: Async boto3 wrapper
 Home-page: https://github.com/terrycain/aioboto3
 License: Apache-2.0
 Keywords: aioboto3,boto3,aws
 Author: Terry Cain
 Author-email: terry@terrys-home.co.uk
 Requires-Python: >=3.7,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: chalice
 Provides-Extra: s3cse
-Requires-Dist: aiobotocore[boto3] (==2.2.0)
+Requires-Dist: aiobotocore[boto3] (==2.3.0)
 Requires-Dist: chalice (>=1.24.0); extra == "chalice"
 Requires-Dist: cryptography (>=2.3.1); extra == "s3cse"
 Project-URL: Documentation, https://readthedocs.org/projects/aioboto3/
 Project-URL: Repository, https://github.com/terrycain/aioboto3
 Description-Content-Type: text/x-rst
 
 ========================
```

