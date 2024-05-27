# Comparing `tmp/analytics_mesh-0.1.8-py3-none-any.whl.zip` & `tmp/analytics_mesh-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,33 +1,35 @@
-Zip file size: 33868 bytes, number of entries: 31
--rw-rw-rw-  2.0 unx     6490 b- defN 21-Dec-08 14:09 analytics_mesh-0.1.8.data/data/LICENSE
--rwxrwxrwx  2.0 unx     1577 b- defN 21-Dec-08 14:09 analytics_mesh-0.1.8.data/scripts/deploy_k8s.sh
--rw-r--r--  2.0 unx      298 b- defN 21-Dec-08 14:09 mesh/__init__.py
--rw-r--r--  2.0 unx     1176 b- defN 21-Dec-08 14:09 mesh/logger.py
--rw-r--r--  2.0 unx    10544 b- defN 21-Dec-08 14:09 mesh/pipeline.py
--rw-r--r--  2.0 unx     6349 b- defN 21-Dec-08 14:09 mesh/stores.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/connectors/__init__.py
--rw-r--r--  2.0 unx      310 b- defN 21-Dec-08 14:09 mesh/connectors/base.py
--rw-r--r--  2.0 unx     3264 b- defN 21-Dec-08 14:09 mesh/connectors/postgres.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/dataframes/__init__.py
--rw-r--r--  2.0 unx     1793 b- defN 21-Dec-08 14:09 mesh/dataframes/frame_operators.py
--rw-r--r--  2.0 unx     1312 b- defN 21-Dec-08 14:09 mesh/dataframes/row_operations.py
--rw-r--r--  2.0 unx     1540 b- defN 21-Dec-08 14:09 mesh/dataframes/validators.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/dates/__init__.py
--rw-r--r--  2.0 unx     1186 b- defN 21-Dec-08 14:09 mesh/dates/wrangler.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/google/__init__.py
--rwxrwxrwx  2.0 unx     1577 b- defN 21-Dec-08 14:09 mesh/google/deploy_k8s.sh
--rw-r--r--  2.0 unx     1565 b- defN 21-Dec-08 14:09 mesh/google/secrets.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/google/connectors/__init__.py
--rw-r--r--  2.0 unx    14679 b- defN 21-Dec-08 14:09 mesh/google/connectors/bigquery.py
--rw-r--r--  2.0 unx    11165 b- defN 21-Dec-08 14:09 mesh/google/connectors/gcs.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/notifiers/__init__.py
--rw-r--r--  2.0 unx      893 b- defN 21-Dec-08 14:09 mesh/notifiers/slackrapper.py
--rw-r--r--  2.0 unx        0 b- defN 21-Dec-08 14:09 mesh/projects/__init__.py
--rw-r--r--  2.0 unx     6109 b- defN 21-Dec-08 14:09 mesh/projects/context.py
--rw-r--r--  2.0 unx     2876 b- defN 21-Dec-08 14:09 mesh/projects/conventions.py
--rw-rw-rw-  2.0 unx     6490 b- defN 21-Dec-08 14:10 analytics_mesh-0.1.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     3524 b- defN 21-Dec-08 14:10 analytics_mesh-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-08 14:10 analytics_mesh-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 21-Dec-08 14:10 analytics_mesh-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2569 b- defN 21-Dec-08 14:10 analytics_mesh-0.1.8.dist-info/RECORD
-31 files, 87383 bytes uncompressed, 29726 bytes compressed:  66.0%
+Zip file size: 34827 bytes, number of entries: 33
+-rw-rw-rw-  2.0 unx     6490 b- defN 22-Jan-07 08:38 analytics_mesh-0.1.9.data/data/LICENSE
+-rwxrwxrwx  2.0 unx     1577 b- defN 22-Jan-07 08:38 analytics_mesh-0.1.9.data/scripts/deploy_k8s.sh
+-rw-r--r--  2.0 unx      298 b- defN 22-Jan-07 08:38 mesh/__init__.py
+-rw-r--r--  2.0 unx     1176 b- defN 22-Jan-07 08:38 mesh/logger.py
+-rw-r--r--  2.0 unx    10544 b- defN 22-Jan-07 08:38 mesh/pipeline.py
+-rw-r--r--  2.0 unx     6349 b- defN 22-Jan-07 08:38 mesh/stores.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/connectors/__init__.py
+-rw-r--r--  2.0 unx      310 b- defN 22-Jan-07 08:38 mesh/connectors/base.py
+-rw-r--r--  2.0 unx     3264 b- defN 22-Jan-07 08:38 mesh/connectors/postgres.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/dataframes/__init__.py
+-rw-r--r--  2.0 unx     1793 b- defN 22-Jan-07 08:38 mesh/dataframes/frame_operators.py
+-rw-r--r--  2.0 unx     1312 b- defN 22-Jan-07 08:38 mesh/dataframes/row_operations.py
+-rw-r--r--  2.0 unx     1540 b- defN 22-Jan-07 08:38 mesh/dataframes/validators.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/dates/__init__.py
+-rw-r--r--  2.0 unx     1186 b- defN 22-Jan-07 08:38 mesh/dates/wrangler.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/google/__init__.py
+-rwxrwxrwx  2.0 unx     1577 b- defN 22-Jan-07 08:38 mesh/google/deploy_k8s.sh
+-rw-r--r--  2.0 unx     1565 b- defN 22-Jan-07 08:38 mesh/google/secrets.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/google/connectors/__init__.py
+-rw-r--r--  2.0 unx    14679 b- defN 22-Jan-07 08:38 mesh/google/connectors/bigquery.py
+-rw-r--r--  2.0 unx    11165 b- defN 22-Jan-07 08:38 mesh/google/connectors/gcs.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/metrics/__init__.py
+-rw-r--r--  2.0 unx     1639 b- defN 22-Jan-07 08:38 mesh/metrics/mase.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/notifiers/__init__.py
+-rw-r--r--  2.0 unx      956 b- defN 22-Jan-07 08:38 mesh/notifiers/slackrapper.py
+-rw-r--r--  2.0 unx        0 b- defN 22-Jan-07 08:38 mesh/projects/__init__.py
+-rw-r--r--  2.0 unx     6109 b- defN 22-Jan-07 08:38 mesh/projects/context.py
+-rw-r--r--  2.0 unx     2876 b- defN 22-Jan-07 08:38 mesh/projects/conventions.py
+-rw-rw-rw-  2.0 unx     6490 b- defN 22-Jan-07 08:39 analytics_mesh-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3555 b- defN 22-Jan-07 08:39 analytics_mesh-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-07 08:39 analytics_mesh-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 22-Jan-07 08:39 analytics_mesh-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2724 b- defN 22-Jan-07 08:39 analytics_mesh-0.1.9.dist-info/RECORD
+33 files, 89271 bytes uncompressed, 30445 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: analytics_mesh-0.1.8.data/data/LICENSE
+Filename: analytics_mesh-0.1.9.data/data/LICENSE
 Comment: 
 
-Filename: analytics_mesh-0.1.8.data/scripts/deploy_k8s.sh
+Filename: analytics_mesh-0.1.9.data/scripts/deploy_k8s.sh
 Comment: 
 
 Filename: mesh/__init__.py
 Comment: 
 
 Filename: mesh/logger.py
 Comment: 
@@ -57,14 +57,20 @@
 
 Filename: mesh/google/connectors/bigquery.py
 Comment: 
 
 Filename: mesh/google/connectors/gcs.py
 Comment: 
 
+Filename: mesh/metrics/__init__.py
+Comment: 
+
+Filename: mesh/metrics/mase.py
+Comment: 
+
 Filename: mesh/notifiers/__init__.py
 Comment: 
 
 Filename: mesh/notifiers/slackrapper.py
 Comment: 
 
 Filename: mesh/projects/__init__.py
@@ -72,23 +78,23 @@
 
 Filename: mesh/projects/context.py
 Comment: 
 
 Filename: mesh/projects/conventions.py
 Comment: 
 
-Filename: analytics_mesh-0.1.8.dist-info/LICENSE
+Filename: analytics_mesh-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: analytics_mesh-0.1.8.dist-info/METADATA
+Filename: analytics_mesh-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: analytics_mesh-0.1.8.dist-info/WHEEL
+Filename: analytics_mesh-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: analytics_mesh-0.1.8.dist-info/top_level.txt
+Filename: analytics_mesh-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: analytics_mesh-0.1.8.dist-info/RECORD
+Filename: analytics_mesh-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mesh/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 
 # thanks tensorflow open source :D
 # Special dunders that we choose to export:
 _exported_dunders = set([
     '__version__',
     '__git_version__'
```

## mesh/notifiers/slackrapper.py

```diff
@@ -1,24 +1,28 @@
 import logging
 import slack_alerts
+import os
 
 log = logging.getLogger(__name__)
 
 class SlackRapper(object):
-    def __init__(self, **kwargs):
+    def __init__(self, webhook_filename=None):
         """
         :param webhook_filename: The webhook filename pointing to a channel that you want to post a message to
         """
         self.slack_alerter = logging.getLogger(__name__)
         try:
-            self.filename = kwargs['webhook_filename']
+            env = os.environ["NODE_ENV"]
+        except: 
+            env = None
+        try:
+            self.filename = webhook_filename
             with open(self.filename, 'r') as file:
                 webhook = file.read()
             self.slack_alerter = slack_alerts.Alerter('{}'.format(webhook))
-        except FileNotFoundError as e:
-            self.slack_alerter.error(f'{self.filename} file not found; using default logger')
-            raise
-        except KeyError as e:
-            self.slack_alerter.warning(f"file not provided; using default logger")
-
+        except (TypeError, FileNotFoundError) as e:
+            self.slack_alerter.error(f'Type or file not found error, using default logger')
+            if env not in['dev', None]:
+                raise e
+            
     def notify(self, message):
         self.slack_alerter.info(message)
```

## Comparing `analytics_mesh-0.1.8.data/data/LICENSE` & `analytics_mesh-0.1.9.data/data/LICENSE`

 * *Files identical despite different names*

## Comparing `analytics_mesh-0.1.8.data/scripts/deploy_k8s.sh` & `analytics_mesh-0.1.9.data/scripts/deploy_k8s.sh`

 * *Files identical despite different names*

## Comparing `analytics_mesh-0.1.8.dist-info/LICENSE` & `analytics_mesh-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `analytics_mesh-0.1.8.dist-info/METADATA` & `analytics_mesh-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: analytics-mesh
-Version: 0.1.8
+Version: 0.1.9
 Summary: Facades and common functions necessary for data science and data engineering workflows
 Home-page: UNKNOWN
 Author: Jacques du Toit, Carl du Plessis, Lydia de Lange, Bernie Lindner
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -29,14 +29,15 @@
 Requires-Dist: python-dateutil (>=2.8.0)
 Requires-Dist: pylint (>=2.6.0)
 Requires-Dist: pylint-exit (>=1.2.0)
 Requires-Dist: PyYAML (>=5.1.2)
 Requires-Dist: python-box (>=5.1.1)
 Requires-Dist: pytz (>=2019.2)
 Requires-Dist: slack-alerts (>=1.0.0)
+Requires-Dist: sklearn (>=0.0)
 
 # analytics-mesh
 Interfaces and facades that facilitate a common approach to analytics tasks
 
 
 # Getting Started
```

## Comparing `analytics_mesh-0.1.8.dist-info/RECORD` & `analytics_mesh-0.1.9.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-analytics_mesh-0.1.8.data/data/LICENSE,sha256=9miXFJMD9Gc3bpA4EKdwTNXNKOxPRIY26VKRmpklKr8,6490
-analytics_mesh-0.1.8.data/scripts/deploy_k8s.sh,sha256=gtxItmIeDTWzB0qZrmNnF0Zw60i91cJnGdlx_5uyD3g,1577
-mesh/__init__.py,sha256=dShSaPVksJz_KnNXd15fIHsCRV2FzunnSS7_lp7Hcgk,298
+analytics_mesh-0.1.9.data/data/LICENSE,sha256=9miXFJMD9Gc3bpA4EKdwTNXNKOxPRIY26VKRmpklKr8,6490
+analytics_mesh-0.1.9.data/scripts/deploy_k8s.sh,sha256=gtxItmIeDTWzB0qZrmNnF0Zw60i91cJnGdlx_5uyD3g,1577
+mesh/__init__.py,sha256=IszH7fQW4TutMPi031_BNj1J8g2Y0Gdro1fwT1kP7AA,298
 mesh/logger.py,sha256=r_w6tAdKTotBggrECrjXTw2h_bYeqxpEmATtiKr82uo,1176
 mesh/pipeline.py,sha256=6pVd2FNqQSsjLNDDLQOgoUZ_4xhUtKI2itraeZGXbEk,10544
 mesh/stores.py,sha256=7ddeIfny7vT_RynzhZAyUG_WlfmiOTa5wMDsjJg8M7E,6349
 mesh/connectors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh/connectors/base.py,sha256=CPaF9IdAh7bdAAykBPEnok9e7B5Ow2g7y2GpzxqNTns,310
 mesh/connectors/postgres.py,sha256=pTah2aG9I6wAtmgzEftBGQkr5Oe0qO93y6uVDLVe5u0,3264
 mesh/dataframes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -15,17 +15,19 @@
 mesh/dates/wrangler.py,sha256=-hYoC6oj14xi-t27r0ykmML5ARxpXbZC1t56KhHZk4g,1186
 mesh/google/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh/google/deploy_k8s.sh,sha256=gtxItmIeDTWzB0qZrmNnF0Zw60i91cJnGdlx_5uyD3g,1577
 mesh/google/secrets.py,sha256=45jqLeGsOcDJi4Nofgc4HCEBFuLU-z9DYoebuOAVdT0,1565
 mesh/google/connectors/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh/google/connectors/bigquery.py,sha256=lmOhfZchyM_lOR6o45EjyoLewdFjutIw_NqivN023Cg,14679
 mesh/google/connectors/gcs.py,sha256=cxXUknO74-1oKNrS-qdLazCMzyHm--rs33I_qGk61Mw,11165
+mesh/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mesh/metrics/mase.py,sha256=buggC6b0cLPPTbElAxWg11AK1Jvlniab5hwiS6sYtgw,1639
 mesh/notifiers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mesh/notifiers/slackrapper.py,sha256=BMXNmHZVRqdKX_IhfkXzsz4bjOwxCPRnU7abJJKPV70,893
+mesh/notifiers/slackrapper.py,sha256=qzI9bsQwTLRUyksBRi0EOlFtoxDAoZjMUdaIDTffgf0,956
 mesh/projects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mesh/projects/context.py,sha256=uzxoiUyr719_VMoRLEiUqXrHzmNU_qx-roQTJtVKACE,6109
 mesh/projects/conventions.py,sha256=VzEShImsk8U2jPXixZ9iB3J_mAEer3WUZ3ySDbf1F4E,2876
-analytics_mesh-0.1.8.dist-info/LICENSE,sha256=9miXFJMD9Gc3bpA4EKdwTNXNKOxPRIY26VKRmpklKr8,6490
-analytics_mesh-0.1.8.dist-info/METADATA,sha256=tZI0a97s8AzD6-gN-E7QqJ7wXQWNZkERorJMX2TeNg8,3524
-analytics_mesh-0.1.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-analytics_mesh-0.1.8.dist-info/top_level.txt,sha256=9TJpknW1CazBq5sbZ4N1q-DzUDPVdHuu5ygt1fbLK0s,5
-analytics_mesh-0.1.8.dist-info/RECORD,,
+analytics_mesh-0.1.9.dist-info/LICENSE,sha256=9miXFJMD9Gc3bpA4EKdwTNXNKOxPRIY26VKRmpklKr8,6490
+analytics_mesh-0.1.9.dist-info/METADATA,sha256=pss8EQ37eptkyQKGiStkk1GU8ZrzvqhTvz-CXgmSGI8,3555
+analytics_mesh-0.1.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+analytics_mesh-0.1.9.dist-info/top_level.txt,sha256=9TJpknW1CazBq5sbZ4N1q-DzUDPVdHuu5ygt1fbLK0s,5
+analytics_mesh-0.1.9.dist-info/RECORD,,
```

