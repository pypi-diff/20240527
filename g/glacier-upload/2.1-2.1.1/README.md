# Comparing `tmp/glacier_upload-2.1.tar.gz` & `tmp/glacier_upload-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glacier_upload-2.1.tar", max compression
+gzip compressed data, was "glacier_upload-2.1.1.tar", max compression
```

## Comparing `glacier_upload-2.1.tar` & `glacier_upload-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35141 2023-07-29 02:58:46.590072 glacier_upload-2.1/LICENSE
--rw-r--r--   0        0        0     4642 2023-07-29 02:58:46.590072 glacier_upload-2.1/README.md
--rw-r--r--   0        0        0     1234 2023-07-29 02:58:46.590072 glacier_upload-2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-29 02:58:46.590072 glacier_upload-2.1/src/glacier_upload/__init__.py
--rw-r--r--   0        0        0     7105 2023-07-29 02:58:46.590072 glacier_upload-2.1/src/glacier_upload/archives.py
--rw-r--r--   0        0        0     5027 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/cli.py
--rw-r--r--   0        0        0     2417 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/inventories.py
--rw-r--r--   0        0        0     9783 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/upload.py
--rw-r--r--   0        0        0     1604 2023-07-29 02:58:46.594072 glacier_upload-2.1/src/glacier_upload/utils/tree_hash.py
--rw-r--r--   0        0        0     5719 1970-01-01 00:00:00.000000 glacier_upload-2.1/setup.py
--rw-r--r--   0        0        0     5917 1970-01-01 00:00:00.000000 glacier_upload-2.1/PKG-INFO
+-rw-r--r--   0        0        0    35141 2024-05-27 10:43:34.317647 glacier_upload-2.1.1/LICENSE
+-rw-r--r--   0        0        0     4642 2024-05-27 10:43:34.317647 glacier_upload-2.1.1/README.md
+-rw-r--r--   0        0        0     1221 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/__init__.py
+-rw-r--r--   0        0        0     7105 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/archives.py
+-rw-r--r--   0        0        0     5027 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/cli.py
+-rw-r--r--   0        0        0     2417 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/inventories.py
+-rw-r--r--   0        0        0     9783 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/upload.py
+-rw-r--r--   0        0        0     1604 2024-05-27 10:43:34.321647 glacier_upload-2.1.1/src/glacier_upload/utils/tree_hash.py
+-rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 glacier_upload-2.1.1/setup.py
+-rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 glacier_upload-2.1.1/PKG-INFO
```

### Comparing `glacier_upload-2.1/LICENSE` & `glacier_upload-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/README.md` & `glacier_upload-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/pyproject.toml` & `glacier_upload-2.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glacier-upload"
-version = "2.1"
+version = "2.1.1"
 description = "A helper tool to upload and manage archives in AWS Glacier Vaults"
 authors = ["Trapsilo Bumi <tbumi@thpd.io>"]
 license = "GPL-3.0+"
 readme = "README.md"
 packages = [{include = "glacier_upload", from = "src"}]
 repository = "https://github.com/tbumi/glacier-upload"
 keywords = ["AWS", "glacier", "upload", "multipart"]
@@ -18,24 +18,24 @@
     "Topic :: System :: Archiving",
     "Topic :: System :: Archiving :: Backup",
     "Topic :: System :: Archiving :: Compression",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-boto3 = "^1.26.47"
-click = "^8.1.3"
-tqdm = "^4.65.0"
+boto3 = "^1.34.113"
+click = "^8.1.7"
+tqdm = "^4.66.4"
 
 [tool.poetry.group.dev.dependencies]
-black = ">=22.12,<24.0"
-flake8 = "^6.0.0"
-mypy = ">=0.991,<1.4"
-isort = "^5.11.4"
-pre-commit = ">=2.21,<4.0"
+black = "^24.4.2"
+flake8 = "^7.0.0"
+mypy = "^1.10.0"
+isort = "^5.13.2"
+pre-commit = "^3.7.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 glacier = "glacier_upload.cli:glacier_cli"
```

### Comparing `glacier_upload-2.1/src/glacier_upload/archives.py` & `glacier_upload-2.1.1/src/glacier_upload/archives.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/src/glacier_upload/cli.py` & `glacier_upload-2.1.1/src/glacier_upload/cli.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/src/glacier_upload/inventories.py` & `glacier_upload-2.1.1/src/glacier_upload/inventories.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/src/glacier_upload/upload.py` & `glacier_upload-2.1.1/src/glacier_upload/upload.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/src/glacier_upload/utils/tree_hash.py` & `glacier_upload-2.1.1/src/glacier_upload/utils/tree_hash.py`

 * *Files identical despite different names*

### Comparing `glacier_upload-2.1/setup.py` & `glacier_upload-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 packages = \
 ['glacier_upload', 'glacier_upload.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['boto3>=1.26.47,<2.0.0', 'click>=8.1.3,<9.0.0', 'tqdm>=4.65.0,<5.0.0']
+['boto3>=1.34.113,<2.0.0', 'click>=8.1.7,<9.0.0', 'tqdm>=4.66.4,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['glacier = glacier_upload.cli:glacier_cli']}
 
 setup_kwargs = {
     'name': 'glacier-upload',
-    'version': '2.1',
+    'version': '2.1.1',
     'description': 'A helper tool to upload and manage archives in AWS Glacier Vaults',
     'long_description': '# glacier-upload\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)\n[![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)\n[![License-GPLv3](https://img.shields.io/github/license/tbumi/glacier-upload)](https://github.com/tbumi/glacier-upload/blob/main/LICENSE)\n\nA helper tool to upload and manage archives in\n[Amazon S3 Glacier](https://docs.aws.amazon.com/amazonglacier/latest/dev/introduction.html)\nVaults. Amazon S3 Glacier is a cloud storage service that is optimized for long\nterm storage for a relatively cheap price. NOT to be confused with Amazon S3\nwith Glacier (Instant Retrieval, Flexible Retrieval, and Deep Archive) tier\nstorage, which uses the S3 API and does not deal with vaults and archives.\n\n## Installation\n\nMinimum required Python version is 3.9. To install, run this in your terminal:\n\n```\n$ pip install glacier_upload\n```\n\n## Usage\n\n### Prerequisites\n\nTo upload an archive to Amazon S3 Glacier vault, ensure you have:\n\n- Created an AWS account\n- Created an Amazon S3 Glacier vault from the AWS CLI tool or the Management\n  Console\n\n### Uploading an archive\n\nAn upload can be performed by running `glacier upload` followed by the vault\nname and the file name(s) that you want to upload.\n\n```\nglacier upload VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n`FILE_NAME` can be one or more files or directories.\n\nThe script will:\n\n1. Read the file(s)\n2. Consolidate them into a `.tar.xz` archive if multiple `FILE_NAME`s are\n   specified or `FILE_NAME` is one or more directories\n3. Upload the file in one go if the file is less than 100 MB in size, or\n4. Split the file into chunks\n5. Spawn a number of threads that will upload the chunks in parallel. Note that\n   it will not read the entire file into memory, but only parts of the file as\n   it processes the chunks.\n6. Return the archive ID when complete. Consider saving this archive ID in a\n   safe place for retrieval purposes, because Amazon Glacier does not provide a\n   list of archives in realtime. See the "Requesting an inventory" section below\n   for details.\n\nThere are additional options to customize your upload, such as adding a\ndescription to the archive or configuring the number of threads or the size of\nparts. Run `glacier upload --help` for more information.\n\nIf a multipart upload is interrupted in the middle (because of an exception,\ninterrupted manually, or other reason), the script will show you the upload ID.\nThat upload ID can be used to resume the upload, using the same command but\nadding the `--upload-id` option, like so:\n\n```\nglacier upload --upload-id UPLOAD_ID VAULT_NAME FILE_NAME [FILE_NAME ...]\n```\n\n### Retrieving an archive\n\nRetrieving an archive in glacier requires two steps. First, initiate a\n"retrieval job" using:\n\n```\nglacier archive init-retrieval VAULT_NAME ARCHIVE_ID\n```\n\nTo see a list of archive IDs in a vault, see "Requesting an inventory" below.\n\nThen, the retrieval job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the archive if it has been\ncompleted.\n\n```\nglacier archive get VAULT_NAME JOB_ID FILE_NAME\n```\n\n### Requesting an inventory\n\nVaults do not provide realtime access to a list of their contents. To know what\na vault contains, you need to request an inventory of the archive, in a similar\nmanner to retrieving an archive. To initiate an inventory, run:\n\n```\nglacier inventory init-retrieval VAULT_NAME\n```\n\nThen, the inventory job will take some time to complete. Run the next step to\nboth check whether the job is complete and retrieve the inventory if it has been\ncompleted.\n\n```\nglacier inventory get VAULT_NAME JOB_ID\n```\n\n### Deleting an archive, deleting an upload job, creating/deleting a vault, etc.\n\nAll jobs other than uploading an archive and requesting/downloading an inventory\nor archive can be done using the AWS CLI. Those functionalities are not\nimplemented here to avoid duplication of work, and minimize maintenance efforts\nof this package.\n\n## Contributing\n\nContributions and/or bug fixes are welcome! Just make sure you\'ve read the below\nrequirements, then feel free to fork, make a topic branch, make your changes,\nand submit a PR.\n\n### Development Requirements\n\nBefore committing to this repo, install [poetry](https://python-poetry.org/) on\nyour local machine, then run these commands to setup your environment:\n\n```sh\npoetry install\npre-commit install\n```\n\nAll code is formatted with [black](https://github.com/psf/black). Consider\ninstalling an integration for it in your favourite text editor.\n',
     'author': 'Trapsilo Bumi',
     'author_email': 'tbumi@thpd.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tbumi/glacier-upload',
```

### Comparing `glacier_upload-2.1/PKG-INFO` & `glacier_upload-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glacier-upload
-Version: 2.1
+Version: 2.1.1
 Summary: A helper tool to upload and manage archives in AWS Glacier Vaults
 Home-page: https://github.com/tbumi/glacier-upload
 License: GPL-3.0+
 Keywords: AWS,glacier,upload,multipart
 Author: Trapsilo Bumi
 Author-email: tbumi@thpd.io
 Requires-Python: >=3.9,<4.0
@@ -18,17 +18,17 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: System :: Archiving :: Compression
-Requires-Dist: boto3 (>=1.26.47,<2.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: boto3 (>=1.34.113,<2.0.0)
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Repository, https://github.com/tbumi/glacier-upload
 Description-Content-Type: text/markdown
 
 # glacier-upload
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![pypi](https://img.shields.io/pypi/v/glacier_upload)](https://pypi.org/project/glacier_upload/)
```

