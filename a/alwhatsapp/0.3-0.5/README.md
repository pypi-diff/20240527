# Comparing `tmp/alwhatsapp-0.3-py3-none-any.whl.zip` & `tmp/alwhatsapp-0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3964 bytes, number of entries: 7
+Zip file size: 4363 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 24-May-05 16:07 alwhatsapp/__init__.py
--rw-r--r--  2.0 unx     5436 b- defN 24-May-05 07:49 alwhatsapp/whatsapp_client.py
--rw-r--r--  2.0 unx     1074 b- defN 24-May-05 16:10 alwhatsapp-0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 24-May-05 16:10 alwhatsapp-0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-05 16:10 alwhatsapp-0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-May-05 16:10 alwhatsapp-0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      556 b- defN 24-May-05 16:10 alwhatsapp-0.3.dist-info/RECORD
-7 files, 7843 bytes uncompressed, 2972 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx     7312 b- defN 24-May-27 13:40 alwhatsapp/whatsapp_client.py
+-rw-r--r--  2.0 unx     1074 b- defN 24-May-27 13:48 alwhatsapp-0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      911 b- defN 24-May-27 13:48 alwhatsapp-0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-27 13:48 alwhatsapp-0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-May-27 13:48 alwhatsapp-0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      556 b- defN 24-May-27 13:48 alwhatsapp-0.5.dist-info/RECORD
+7 files, 9956 bytes uncompressed, 3371 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: alwhatsapp/__init__.py
 Comment: 
 
 Filename: alwhatsapp/whatsapp_client.py
 Comment: 
 
-Filename: alwhatsapp-0.3.dist-info/LICENSE.txt
+Filename: alwhatsapp-0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: alwhatsapp-0.3.dist-info/METADATA
+Filename: alwhatsapp-0.5.dist-info/METADATA
 Comment: 
 
-Filename: alwhatsapp-0.3.dist-info/WHEEL
+Filename: alwhatsapp-0.5.dist-info/WHEEL
 Comment: 
 
-Filename: alwhatsapp-0.3.dist-info/top_level.txt
+Filename: alwhatsapp-0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: alwhatsapp-0.3.dist-info/RECORD
+Filename: alwhatsapp-0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## alwhatsapp/whatsapp_client.py

```diff
@@ -6,25 +6,53 @@
     A class that encapsulates WhatsApp messaging functionalities.
     """
 
     def __init__(self, base_url="https://graph.facebook.com/v18.0/"):
         self.base_url = base_url
         self._auth_token = None
         self._from_number_id = None
-        
+        self._whapi_url = None
+        self._whapi_token = None
+
     def set_credentials(self, auth_token, from_number_id):
         """
         Set the WhatsApp authentication token and from number ID.
 
         Args:
             auth_token: The WhatsApp authentication token.
             from_number_id: The WhatsApp from number ID.
         """
         self.auth_token = auth_token
         self.from_number_id = from_number_id
+    
+    def set_whapi_credentials(self, whapi_url, whapi_token):
+        """
+        Set the Whatspi API url and auth token.
+
+        Args:
+            whapi_url: Provided by Whapi
+            whapi_toke: Provided by Whapi for the channel/subscription
+        """
+        self._whapi_url = whapi_url
+        self._whapi_token = whapi_token
+
+    @property
+    def whapi_url(self):
+        if not self._whapi_url:
+            raise ValueError("Whapi url not set")
+        return self._whapi_url
+    @property
+    def whapi_token(self):
+        if not self._whapi_token:
+            raise ValueError("Whapi token not set")
+        return self._whapi_token
+    
+    @whapi_token.setter
+    def whapi_token(self, token):
+        self._auth_token = token
 
     @property
     def auth_token(self):
         if not self._auth_token:
             raise ValueError("WhatsApp authentication token not set")
         return self._auth_token
 
@@ -108,16 +136,46 @@
                 "sub_type": "Url",
                 "index": "0",
                 "parameters": [{"type": "text", "text": button_link[0]}],
             }
             components.append(button_section)
 
         return {"components": components}
+    
+    def send_whatsapp_message(self,payload, max_retries=3, base_timeout=2):
+        url = f"{self.base_url}{self.from_number_id}/messages"
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.auth_token}",
+        }
+        response = self.send_message(url,headers,payload, max_retries, base_timeout)
+        return response
+
+
+    def send_whapi_message(self,to,message, max_retries=3, base_timeout=2):
+
+        url = f"{self.whapi_url}/messages/text"
+
+        headers = {
+            "accept": "application/json",
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.whapi_token}",
+        }
+        payload = {
+            "to": to,            
+            "body": message
+            #"typing_time": 20,
+            #"ephemeral": 120,
+            #"view_once": False
+        }
+        #response = requests.post(url, json=payload, headers=headers)
+        response = self.send_message(url,headers,payload, max_retries, base_timeout, json_param=True)
+        return response
 
-    def send_message(self,payload, max_retries=3, base_timeout=2):
+    def send_message(self,url,headers,payload, max_retries=3, base_timeout=2,json_param=False):
         """
         Makes a request with exponential backoff for retries on timeout.
 
         Args:
             payload: the data to be posted to whatapp
             url: The URL to send the request to.
             headers: Carries mainly the authorization header, the content-type and any other necessary headers
@@ -126,25 +184,23 @@
 
         Returns:
             The response object from a successful request.
 
         Raises:
             requests.exceptions.RequestException: If the request fails after all retries or if the is a another RequestException type error
         """
-        url = f"{self.base_url}{self.from_number_id}/messages"
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.auth_token}",
-        }
+        
         for attempt in range(1, max_retries + 1):
             timeout_value = base_timeout * 2 ** (attempt - 1)  # exponential backoff
             try:
-                response = requests.request(
-                    "POST", url, headers=headers, data=payload, timeout=timeout_value
-                )
+                if json_param :
+                    response = requests.request("POST", url, headers=headers, json=payload, timeout=timeout_value)
+                else:
+                    response = requests.request("POST", url, headers=headers, data=payload, timeout=timeout_value)
+                
                 return response
             except requests.exceptions.Timeout as e:
                 print(f"Request timed out on attempt {attempt} ({timeout_value}s): {e}")
             except requests.exceptions.RequestException as e:
                 raise e
 
         # Raise an exception after all retries are exhausted
```

## Comparing `alwhatsapp-0.3.dist-info/LICENSE.txt` & `alwhatsapp-0.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `alwhatsapp-0.3.dist-info/METADATA` & `alwhatsapp-0.5.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: alwhatsapp
-Version: 0.3
-Summary: Provides a WhatsApp Notification client supports Meta templates and custom messages and forms part of the AL Notificaiton Modules Suite
+Version: 0.5
+Summary: Provides a WhatsApp Notification client supports Meta templates and custom messages and forms part of the AL Notificaiton Modules Suite. This version includes integration with Whapi Tool (https://panel.whapi.cloud/) to support sending to Whatsapp Groups.
 Home-page: https://al.co.za/
 Author: Autumn Leaf IT South Africa
 Author-email: jason@al.co.za
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires: requests
 Requires: json
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-Provides a WhatsApp Notification client supports Meta templates and custom messages and forms part of the AL Notificaiton Modules Suite
+Provides a WhatsApp Notification client supports Meta templates and custom messages and forms part of the AL Notificaiton Modules Suite.This version includes integration with Whapi Tool (https://panel.whapi.cloud/) to support sending to Whatsapp Groups.
```

