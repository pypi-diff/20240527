# Comparing `tmp/org-ds-cdk-0.1.6.tar.gz` & `tmp/org-ds-cdk-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "org-ds-cdk-0.1.6.tar", last modified: Sat May 18 09:55:29 2024, max compression
+gzip compressed data, was "org-ds-cdk-0.1.7.tar", last modified: Mon May 27 06:49:34 2024, max compression
```

## Comparing `org-ds-cdk-0.1.6.tar` & `org-ds-cdk-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:55:29.095601 org-ds-cdk-0.1.6/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2024-05-18 09:55:29.091601 org-ds-cdk-0.1.6/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2024-05-18 05:53:16.000000 org-ds-cdk-0.1.6/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:55:29.091601 org-ds-cdk-0.1.6/lib/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:55:29.091601 org-ds-cdk-0.1.6/lib/org_ds_cdk/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      133 2024-05-18 09:55:08.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-05-18 04:59:50.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk/apigateway.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1349 2024-05-18 09:32:10.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk/multilambda.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-18 09:55:29.091601 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1221 2024-05-18 09:55:29.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      293 2024-05-18 09:55:29.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-18 09:55:29.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-18 09:55:29.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-18 09:55:29.000000 org-ds-cdk-0.1.6/lib/org_ds_cdk.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-18 09:55:29.095601 org-ds-cdk-0.1.6/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      662 2024-05-18 09:55:16.000000 org-ds-cdk-0.1.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2349 2024-05-27 06:48:38.000000 org-ds-cdk-0.1.7/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/lib/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/lib/org_ds_cdk/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      133 2024-05-18 09:55:08.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2557 2024-05-27 06:47:36.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk/apigateway copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3549 2024-05-27 06:47:34.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk/multilambda copy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      709 2024-05-27 06:47:35.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2678 2024-05-27 06:47:34.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk/vpc.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2540 2024-05-27 06:49:33.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      349 2024-05-27 06:49:33.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-27 06:49:33.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       40 2024-05-27 06:49:33.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2024-05-27 06:49:33.000000 org-ds-cdk-0.1.7/lib/org_ds_cdk.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-27 06:49:34.021180 org-ds-cdk-0.1.7/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      613 2024-05-27 06:49:09.000000 org-ds-cdk-0.1.7/setup.py
```

### Comparing `org-ds-cdk-0.1.6/lib/org_ds_cdk/apigateway.py` & `org-ds-cdk-0.1.7/lib/org_ds_cdk/apigateway copy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,65 @@
 from constructs import Construct
+from .utils import load_config
 
 from aws_cdk import (
     Stack,
     aws_lambda as _lambda,
     aws_apigateway as apigateway,
+    CfnOutput
 )
 
 
-class ApiGatewayStack(Construct):
+class ApiGatewayConstruct(Construct):
     def __init__(self, scope: Construct, id: str, lambda_stack, config: str, **kwargs) -> None:
         super().__init__(scope, id, **kwargs)
 
+        apiName = config["ApiGateway"]["apiName"]
+        description = config["ApiGateway"]["description"]
+        stageName = config["ApiGateway"]["stageName"]
+        routes = config['ApiGateway']['routes']
+
         # Create an API Gateway
         api = apigateway.RestApi(self, "api",
-            rest_api_name="MyService",
-            description="This service serves my APIs."
+            rest_api_name=apiName,
+            description=description,
         )
 
-        # Create a dictionary to hold the resources for different paths
-        resources = {}
-
-        # Iterate over routes in the configuration
-        for route in config['routes']:
-            # Split the path into individual parts
-            path_parts = route['path'].strip('/').split('/')
-
-            resource = api.root  # Start with the root resource
-
-            # Create nested resources if needed
-            for part in path_parts:
-                if part.startswith('{') and part.endswith('}'):
-                    # If the part is a dynamic parameter, add it as a path parameter
-                    resource = resource.add_resource(f"{{{part[1:-1]}}}")
-                else:
-                    # If the part is a static path, add it as a resource
-                    if part not in resources:
-                        resources[part] = resource.add_resource(part)
-                    resource = resources[part]
-
-            # Iterate over the HTTP methods for the route
-            for method in route['methods']:
-                if route['integration'] == 'lambda':
-                    # If the integration type is Lambda, create a Lambda integration
-                    integration = apigateway.LambdaIntegration(lambda_stack.lambda_functions[route['lambdaFunctionName']], proxy=True)
-                
-                # Add the method to the resource
-                resource.add_method(method, integration)
+        if routes is None:
+            # Add a method to the root resource
+            api.root.add_method('GET')  # GET is just an example, use the appropriate method
+
+        else:
+            # Create a dictionary to hold the resources for different paths
+            resources = {}
+
+            # Iterate over routes in the configuration
+            for route in routes:
+                # Split the path into individual parts
+                path_parts = route['path'].strip('/').split('/')
+
+                resource = api.root  # Start with the root resource
+
+                # Create nested resources if needed
+                for part in path_parts:
+                    if part.startswith('{') and part.endswith('}'):
+                        # If the part is a dynamic parameter, add it as a path parameter
+                        resource = resource.add_resource(f"{{{part[1:-1]}}}")
+                    else:
+                        # If the part is a static path, add it as a resource
+                        if part not in resources:
+                            resources[part] = resource.add_resource(part)
+                        resource = resources[part]
+
+                # Iterate over the HTTP methods for the route
+                for method in route['methods']:
+                    if route['integration'] == 'lambda':
+                        # If the integration type is Lambda, create a Lambda integration
+                        integration = apigateway.LambdaIntegration(lambda_stack.lambda_functions[route['lambdaFunctionName']], proxy=True)
+                    
+                    # Add the method to the resource
+                    resource.add_method(method, integration)
+
+        CfnOutput(self, "ApiGatewayId",
+            value=api.rest_api_id,
+            description="API Gateway ID"
+        )
```

### Comparing `org-ds-cdk-0.1.6/setup.py` & `org-ds-cdk-0.1.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='org-ds-cdk',
-    version='0.1.06',
-    description='Constructs for creating an API Gateway and Routes from input JSON configuration',
+    version='0.1.07',
+    description='DS Organization CDK Constructs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     install_requires=[
         'aws-cdk-lib==2.142.0',
         'constructs>=10.0.0'
```

