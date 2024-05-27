# Comparing `tmp/vpn_server-1.7-py3-none-any.whl.zip` & `tmp/vpn_server-1.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 19836 bytes, number of entries: 15
--rw-r--r--  2.0 unx      223 b- defN 24-Jan-30 16:00 vpn/__init__.py
--rw-r--r--  2.0 unx    30708 b- defN 24-Jan-30 16:00 vpn/main.py
--rw-r--r--  2.0 unx      112 b- defN 24-Jan-30 16:00 vpn/requirements.txt
--rw-r--r--  2.0 unx     5671 b- defN 24-Jan-30 16:00 vpn/models/config.py
--rw-r--r--  2.0 unx      431 b- defN 24-Jan-30 16:00 vpn/models/exceptions.py
--rw-r--r--  2.0 unx     5626 b- defN 24-Jan-30 16:00 vpn/models/image_factory.py
--rw-r--r--  2.0 unx      414 b- defN 24-Jan-30 16:00 vpn/models/logger.py
--rw-r--r--  2.0 unx     3273 b- defN 24-Jan-30 16:00 vpn/models/route53.py
--rw-r--r--  2.0 unx     4887 b- defN 24-Jan-30 16:00 vpn/models/server.py
--rw-r--r--  2.0 unx      935 b- defN 24-Jan-30 16:00 vpn/models/util.py
--rw-r--r--  2.0 unx     1068 b- defN 24-Jan-30 16:00 vpn_server-1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5886 b- defN 24-Jan-30 16:00 vpn_server-1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-30 16:00 vpn_server-1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Jan-30 16:00 vpn_server-1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1152 b- defN 24-Jan-30 16:00 vpn_server-1.7.dist-info/RECORD
-15 files, 60482 bytes uncompressed, 17954 bytes compressed:  70.3%
+Zip file size: 20003 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      221 b- defN 24-May-27 02:11 vpn/__init__.py
+-rw-r--r--  2.0 unx    30983 b- defN 24-May-27 02:11 vpn/main.py
+-rw-r--r--  2.0 unx      112 b- defN 24-May-27 02:11 vpn/requirements.txt
+-rw-r--r--  2.0 unx     7011 b- defN 24-May-27 02:11 vpn/models/config.py
+-rw-r--r--  2.0 unx      431 b- defN 24-May-27 02:11 vpn/models/exceptions.py
+-rw-r--r--  2.0 unx     5626 b- defN 24-May-27 02:11 vpn/models/image_factory.py
+-rw-r--r--  2.0 unx      432 b- defN 24-May-27 02:11 vpn/models/logger.py
+-rw-r--r--  2.0 unx     3273 b- defN 24-May-27 02:11 vpn/models/route53.py
+-rw-r--r--  2.0 unx     4842 b- defN 24-May-27 02:11 vpn/models/server.py
+-rw-r--r--  2.0 unx      935 b- defN 24-May-27 02:11 vpn/models/util.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-27 02:11 vpn_server-1.7.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5888 b- defN 24-May-27 02:11 vpn_server-1.7.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 02:11 vpn_server-1.7.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-May-27 02:11 vpn_server-1.7.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1162 b- defN 24-May-27 02:11 vpn_server-1.7.1.dist-info/RECORD
+15 files, 62080 bytes uncompressed, 18101 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: vpn/models/server.py
 Comment: 
 
 Filename: vpn/models/util.py
 Comment: 
 
-Filename: vpn_server-1.7.dist-info/LICENSE
+Filename: vpn_server-1.7.1.dist-info/LICENSE
 Comment: 
 
-Filename: vpn_server-1.7.dist-info/METADATA
+Filename: vpn_server-1.7.1.dist-info/METADATA
 Comment: 
 
-Filename: vpn_server-1.7.dist-info/WHEEL
+Filename: vpn_server-1.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: vpn_server-1.7.dist-info/top_level.txt
+Filename: vpn_server-1.7.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vpn_server-1.7.dist-info/RECORD
+Filename: vpn_server-1.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vpn/__init__.py

```diff
@@ -1,7 +1,7 @@
 """Place holder for package."""
 
 from vpn.main import VPNServer  # noqa: F401
-from vpn.models import (config, exceptions, image_factory,  # noqa: F401
-                        logger, route53, server, util)
+from vpn.models import image_factory  # noqa: F401
+from vpn.models import config, exceptions, logger, route53, server, util
 
-version = "1.7"
+version = "1.7.1"
```

## vpn/main.py

```diff
@@ -186,34 +186,44 @@
             bool:
             Flag to indicate the calling function, whether the security group was authorized successfully.
         """
         try:
             security_group = self.ec2_resource.SecurityGroup(security_group_id)
             security_group.authorize_ingress(
                 IpPermissions=[
-                    {'IpProtocol': 'tcp',
-                     'FromPort': 22,
-                     'ToPort': 22,
-                     'IpRanges': [{'CidrIp': '0.0.0.0/0'}]},
-                    {'IpProtocol': 'tcp',
-                     'FromPort': 443,
-                     'ToPort': 443,
-                     'IpRanges': [{'CidrIp': '0.0.0.0/0'}]},
-                    {'IpProtocol': 'tcp',
-                     'FromPort': config.env.vpn_port,
-                     'ToPort': config.env.vpn_port,
-                     'IpRanges': [{'CidrIp': '0.0.0.0/0'}]},
-                    {'IpProtocol': 'tcp',
-                     'FromPort': 945,
-                     'ToPort': 945,
-                     'IpRanges': [{'CidrIp': '0.0.0.0/0'}]},
-                    {'IpProtocol': 'udp',
-                     'FromPort': 1194,
-                     'ToPort': 1194,
-                     'IpRanges': [{'CidrIp': '0.0.0.0/0'}]}
+                    {
+                        'IpProtocol': 'tcp',
+                        'FromPort': 22,
+                        'ToPort': 22,
+                        'IpRanges': [{'CidrIp': '0.0.0.0/0'}]
+                    },
+                    {
+                        'IpProtocol': 'tcp',
+                        'FromPort': 443,
+                        'ToPort': 443,
+                        'IpRanges': [{'CidrIp': '0.0.0.0/0'}]
+                    },
+                    {
+                        'IpProtocol': 'tcp',
+                        'FromPort': config.env.vpn_port,
+                        'ToPort': config.env.vpn_port,
+                        'IpRanges': [{'CidrIp': '0.0.0.0/0'}]
+                    },
+                    {
+                        'IpProtocol': 'tcp',
+                        'FromPort': 945,
+                        'ToPort': 945,
+                        'IpRanges': [{'CidrIp': '0.0.0.0/0'}]
+                    },
+                    {
+                        'IpProtocol': 'udp',
+                        'FromPort': 1194,
+                        'ToPort': 1194,
+                        'IpRanges': [{'CidrIp': '0.0.0.0/0'}]
+                    }
                 ])
         except ClientError as error:
             error = str(error)
             if '(InvalidPermission.Duplicate)' in error:
                 self.logger.warning('Identified same permissions in an existing SecurityGroup: %s',
                                     security_group_id)
                 return True
```

## vpn/requirements.txt

```diff
@@ -1,8 +1,8 @@
 boto3
 botocore
 inflect
 paramiko==3.3.1
 paramiko-expect==0.3.5
-pydantic==2.4.0
-pydantic-settings==2.0.3
+pydantic==2.4.*
+pydantic-settings==2.0.*
 requests
```

## vpn/models/config.py

```diff
@@ -20,23 +20,29 @@
 
 
 class AMIBase(BaseModel):
     """Default values to fetch AMI image ID.
 
     >>> AMIBase
 
+    See Also:
+        - Subscription Home Page: https://{REGION}.console.aws.amazon.com/marketplace/home#/subscriptions/{_PRODUCT_ID}
+        - Product ID: Found in the home page URL under Summary as 'Product ID'
+        - Product Code: Offer ID in the home page URL
+        - AMI Alias: Found in configuration page (_BASE_URL) as 'Ami Alias'
+        - Product Code: Found in configuration page (_BASE_URL) as 'Product Code'
     """
 
     _BASE_URL: str = 'https://aws.amazon.com/marketplace/server/configuration?productId={productId}'
     _BASE_SSM: str = '/aws/service/marketplace/prod-{path}'
     _PRODUCT_ID: str = 'fe8020db-5343-4c43-9e65-5ed4a825c931'
 
     PRODUCT_PAGE: HttpUrl = _BASE_URL.format(productId=_PRODUCT_ID)
     NAME: str = f'OpenVPN Access Server QA Image-{_PRODUCT_ID}'
-    ALIAS: str = _BASE_SSM.format(path='qqrkogtl46mpu/2.11.3')
+    ALIAS: str = _BASE_SSM.format(path='qqrkogtl46mpu/2.13.1')
     PRODUCT_CODE: str = 'f2ew2wrz425a1jagnifd02u5t'
 
 
 ami_base = AMIBase()
 
 
 # noinspection PyMethodParameters
@@ -110,36 +116,112 @@
 
 settings = Settings()
 
 
 def configuration_dict(param: EnvConfig) -> List[ConfigurationSettings]:
     """Get configuration interaction as a list of dictionaries."""
     for config_dict in [
-        {'request': "Please enter 'yes' to indicate your agreement \\[no\\]: ", 'response': 'yes', 'timeout': 5,
-         'critical': False},
-        {'request': '> Press ENTER for default \\[yes\\]: ', 'response': 'yes', 'timeout': 1, 'critical': False},
-        {'request': '> Press Enter for default \\[1\\]: ', 'response': '1', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for default \\[rsa\\]:', 'response': 'rsa', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for default \\[ 2048 \\]:', 'response': '2048', 'timeout': 1,
-         'critical': False},
-        {'request': '> Press ENTER for default \\[rsa\\]:', 'response': 'rsa', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for default \\[ 2048 \\]:', 'response': '2048', 'timeout': 1,
-         'critical': False},
-        {'request': '> Press ENTER for default \\[943\\]: ', 'response': param.vpn_port, 'timeout': 1,
-         'critical': False},
-        {'request': '> Press ENTER for default \\[443\\]: ', 'response': '443', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for default \\[no\\]: ', 'response': 'yes', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for default \\[no\\]: ', 'response': 'yes', 'timeout': 1, 'critical': False},
-        {'request': '> Press ENTER for EC2 default \\[yes\\]: ', 'response': 'yes', 'timeout': 1,
-         'critical': False},
-        {'request': '> Press ENTER for default \\[yes\\]: ', 'response': 'no', 'timeout': 1, 'critical': False},
-        {'request': '> Specify the username for an existing user or for the new user account: ',
-         'response': param.vpn_username, 'timeout': 1, 'critical': True},
-        {'request': f"Type a password for the '{param.vpn_username}' account "
-                    "(if left blank, a random password will be generated):",
-         'response': param.vpn_password, 'timeout': 1, 'critical': True},
-        {'request': f"Confirm the password for the '{param.vpn_username}' account:", 'response': param.vpn_password,
-         'timeout': 1, 'critical': True},
-        {'request': '> Please specify your Activation key (or leave blank to specify later): ', 'response': '\n',
-         'timeout': 1, 'critical': False}
+        {
+            "request": "Please enter 'yes' to indicate your agreement \\[no\\]: ",
+            "response": "yes",
+            "timeout": 5,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[yes\\]: ",
+            "response": "yes",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press Enter for default \\[1\\]: ",
+            "response": "1",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[rsa\\]:",
+            "response": "rsa",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[ 2048 \\]:",
+            "response": "2048",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[rsa\\]:",
+            "response": "rsa",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[ 2048 \\]:",
+            "response": "2048",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[943\\]: ",
+            "response": param.vpn_port,
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[443\\]: ",
+            "response": "443",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[no\\]: ",
+            "response": "yes",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[no\\]: ",
+            "response": "yes",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for EC2 default \\[yes\\]: ",
+            "response": "yes",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Press ENTER for default \\[yes\\]: ",
+            "response": "no",
+            "timeout": 1,
+            "critical": False,
+        },
+        {
+            "request": "> Specify the username for an existing user or for the new user account: ",
+            "response": param.vpn_username,
+            "timeout": 1,
+            "critical": True,
+        },
+        {
+            "request": f"Type a password for the '{param.vpn_username}' account "
+            "(if left blank, a random password will be generated):",
+            "response": param.vpn_password,
+            "timeout": 1,
+            "critical": True,
+        },
+        {
+            "request": f"Confirm the password for the '{param.vpn_username}' account:",
+            "response": param.vpn_password,
+            "timeout": 1,
+            "critical": True,
+        },
+        {
+            "request": "> Please specify your Activation key (or leave blank to specify later): ",
+            "response": "\n",
+            "timeout": 1,
+            "critical": False,
+        },
     ]:
         yield ConfigurationSettings(**config_dict)
```

## vpn/models/logger.py

```diff
@@ -4,13 +4,15 @@
 
 """
 
 import logging
 
 LOGGER = logging.getLogger(__name__)
 HANDLER = logging.StreamHandler()
-HANDLER.setFormatter(fmt=logging.Formatter(
-    fmt='%(asctime)s - %(levelname)s - [%(module)s:%(lineno)d] - %(funcName)s - %(message)s',
-    datefmt='%b-%d-%Y %I:%M:%S %p'
-))
+HANDLER.setFormatter(
+    fmt=logging.Formatter(
+        fmt='%(asctime)s - %(levelname)s - [%(module)s:%(lineno)d] - %(funcName)s - %(message)s',
+        datefmt='%b-%d-%Y %I:%M:%S %p'
+    )
+)
 LOGGER.addHandler(hdlr=HANDLER)
 LOGGER.setLevel(level=logging.DEBUG)
```

## vpn/models/server.py

```diff
@@ -27,33 +27,39 @@
         pem_key = RSAKey.from_private_key_file(filename=config.settings.key_pair_file)
         self.ssh_client = SSHClient()
         self.ssh_client.load_system_host_keys()
         self.ssh_client.set_missing_host_key_policy(policy=AutoAddPolicy())
         if username == config.env.vpn_username:
             try:
                 # todo: Manual config accepts username and password, but unable to get authentication pass via paramiko
-                self.ssh_client.connect(hostname=hostname, username=username,
-                                        pkey=pem_key, password=config.env.vpn_password)
+                self.ssh_client.connect(
+                    hostname=hostname,
+                    username=username,
+                    pkey=pem_key,
+                    password=config.env.vpn_password,
+                )
             except AuthenticationException as error:
                 self.logger.warning(error)
-                self.ssh_client.connect(hostname=hostname, username='openvpnas', pkey=pem_key)
+                self.ssh_client.connect(
+                    hostname=hostname, username="openvpnas", pkey=pem_key
+                )
         else:
             self.ssh_client.connect(hostname=hostname, username=username, pkey=pem_key)
         self.logger.info("Connected to %s as %s", hostname, username)
         # Backup before modifying logger to compatible version
         self._formatter = []
         self._level = self.logger.level
 
     def remove_formatter(self) -> None:
         """Remove any logging formatters to allow room for OpenVPN configuration interaction."""
         for handler in self.logger.handlers:
             self._formatter.append(handler.formatter)
             handler.formatter = None
         self.logger.setLevel(level=logging.INFO)
-        sys.stdout = open(os.devnull, 'w')
+        sys.stdout = open(os.devnull, "w")
 
     def add_formatter(self) -> None:
         """Re-add any formatters that were removed during instantiation."""
         for handler in self.logger.handlers:
             assert len(self._formatter) == 1
             handler.formatter = self._formatter[0]
         self.logger.setLevel(level=self._level)
@@ -69,41 +75,43 @@
     def test_service(self, timeout: int, display: bool) -> None:
         """Check status of the service running on remote server.
 
         Args:
             timeout: Default interaction session timeout.
             display: Boolean flag whether to display interaction data on screen.
         """
-        with SSHClientInteraction(client=self.ssh_client,
-                                  timeout=timeout,
-                                  display=display,
-                                  output_callback=lambda msg: self.logger.info(msg)) as interact:
+        with SSHClientInteraction(
+            client=self.ssh_client,
+            timeout=timeout,
+            display=display,
+            output_callback=lambda msg: self.logger.info(msg),
+        ) as interact:
             self.remove_formatter()
-            interact.send("systemctl status openvpnas", '\n')
+            interact.send("systemctl status openvpnas", "\n")
             interact.expect(r".*Started OpenVPN Access Server\..*", timeout)
             self.add_formatter()
 
-    def run_interactive_ssh(self,
-                            display: bool = True,
-                            timeout: int = 30) -> None:
+    def run_interactive_ssh(self, display: bool = True, timeout: int = 30) -> None:
         """Runs interactive ssh commands to configure the VPN server.
 
         Args:
             display: Boolean flag whether to display interaction data on screen.
             timeout: Default interaction session timeout.
 
         Returns:
             bool:
             Flag to indicate the calling function, whether the interactive session has completed successfully.
         """
         self.remove_formatter()
-        with SSHClientInteraction(client=self.ssh_client,
-                                  timeout=timeout,
-                                  display=display,
-                                  output_callback=lambda msg: self.logger.info(msg)) as interact:
+        with SSHClientInteraction(
+            client=self.ssh_client,
+            timeout=timeout,
+            display=display,
+            output_callback=lambda msg: self.logger.info(msg),
+        ) as interact:
             for setting in config.settings.openvpn_config_commands:
                 interact.expect(re_strings=setting.request, timeout=setting.timeout)
                 interact.send(send_string=str(setting.response))
             # Blank to await final steps of configuration
             interact.expect(timeout=timeout)
             self.restart_service()
             interact.send("systemctl status openvpnas")
```

## vpn/models/util.py

```diff
@@ -6,27 +6,27 @@
 def available_instance_types() -> Generator[str]:
     """Get all available EC2 instance types looping through describe instances API call.
 
     Yields:
         Generator[str]:
         Instance type.
     """
-    ec2_client = boto3.client('ec2')
+    ec2_client = boto3.client("ec2")
     describe_args = {}
     while True:
         describe_result = ec2_client.describe_instance_types(**describe_args)
-        yield from [i['InstanceType'] for i in describe_result['InstanceTypes']]
-        if 'NextToken' not in describe_result:
+        yield from [i["InstanceType"] for i in describe_result["InstanceTypes"]]
+        if "NextToken" not in describe_result:
             break
-        describe_args['NextToken'] = describe_result['NextToken']
+        describe_args["NextToken"] = describe_result["NextToken"]
 
 
 def available_regions() -> Generator[str]:
     """Get all available regions with describe regions API call.
 
     Yields:
         Generator[str]:
         Region name.
     """
-    ec2_client = boto3.client('ec2')
-    for region in ec2_client.describe_regions()['Regions']:
-        yield region['RegionName']
+    ec2_client = boto3.client("ec2")
+    for region in ec2_client.describe_regions()["Regions"]:
+        yield region["RegionName"]
```

## Comparing `vpn_server-1.7.dist-info/LICENSE` & `vpn_server-1.7.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `vpn_server-1.7.dist-info/METADATA` & `vpn_server-1.7.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vpn-server
-Version: 1.7
+Version: 1.7.1
 Summary: Create an on-demand VPN Server running OpenVPN using AWS EC2
 Author-email: Vignesh Rao <svignesh1793@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Vignesh Rao
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,16 +41,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: inflect
 Requires-Dist: paramiko ==3.3.1
 Requires-Dist: paramiko-expect ==0.3.5
-Requires-Dist: pydantic ==2.4.0
-Requires-Dist: pydantic-settings ==2.0.3
+Requires-Dist: pydantic ==2.4.*
+Requires-Dist: pydantic-settings ==2.0.*
 Requires-Dist: requests
 Provides-Extra: dev
 Requires-Dist: pre-commit ; extra == 'dev'
 
 ![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)
 
 ###### Platform Supported
```

