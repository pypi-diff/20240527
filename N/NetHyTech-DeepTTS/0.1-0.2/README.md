# Comparing `tmp/NetHyTech-DeepTTS-0.1.tar.gz` & `tmp/NetHyTech-DeepTTS-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NetHyTech-DeepTTS-0.1.tar", last modified: Sun May 26 16:44:17 2024, max compression
+gzip compressed data, was "NetHyTech-DeepTTS-0.2.tar", last modified: Sun May 26 17:07:41 2024, max compression
```

## Comparing `NetHyTech-DeepTTS-0.1.tar` & `NetHyTech-DeepTTS-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 16:44:17.474534 NetHyTech-DeepTTS-0.1/
-drwxrwxrwx   0        0        0        0 2024-05-26 16:44:17.441222 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS/
--rw-rw-rw-   0        0        0     1184 2024-05-26 15:05:02.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-26 16:44:17.471502 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/
--rw-rw-rw-   0        0        0     3686 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-26 16:44:17.000000 NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3686 2024-05-26 16:44:17.473534 NetHyTech-DeepTTS-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-26 16:44:17.475537 NetHyTech-DeepTTS-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-05-26 15:15:19.000000 NetHyTech-DeepTTS-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:07:41.050347 NetHyTech-DeepTTS-0.2/
+drwxrwxrwx   0        0        0        0 2024-05-26 17:07:41.015707 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS/
+-rw-rw-rw-   0        0        0     1267 2024-05-26 17:04:55.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-26 17:07:41.047133 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/
+-rw-rw-rw-   0        0        0     3223 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      286 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-26 17:07:40.000000 NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3223 2024-05-26 17:07:41.050347 NetHyTech-DeepTTS-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-26 17:07:41.050347 NetHyTech-DeepTTS-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1254 2024-05-26 16:51:11.000000 NetHyTech-DeepTTS-0.2/setup.py
```

### Comparing `NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS/__init__.py` & `NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import playsound
 import requests
 import os
 
 # Voices
 
-'''
 
-"aura-asteria-en" == Sophia (Female US English
-"aura-luna-en" == Emily (Female US English) 
-"aura-stella-en" == Rachel (Female US English)
-"aura-athena-en" == Eliza (Female UK English)
-"aura-hera-en" == Pam  (Female US English) 
-"aura-orion-en" == Kevin  (Male US English) 
-"aura-arcas-en" == Jeff (Male US English) 
-"aura-perseus-en" == Alex (Male US English) 
-"aura-angus-en" == Rory (Male Irish English) 
-"aura-orpheus-en" == John (Male US English) 
-"aura-helios-en" == Pete (Male UK English) 
-"aura-zeus-en" == James (Male US English) 
+a = "aura-asteria-en" # Sophia (Female US English
+b = "aura-luna-en" # Emily (Female US English) 
+c = "aura-stella-en" # Rachel (Female US English)
+d = "aura-athena-en" # Eliza (Female UK English)
+e = "aura-hera-en" # Pam  (Female US English) 
+f = "aura-orion-en" # Kevin  (Male US English) 
+g = "aura-arcas-en" # Jeff (Male US English) 
+h = "aura-perseus-en" # Alex (Male US English) 
+i = "aura-angus-en" # Rory (Male Irish English) 
+j = "aura-orpheus-en" # John (Male US English) 
+k = "aura-helios-en" # Pete (Male UK English) 
+l = "aura-zeus-en" # James (Male US English) 
 
-'''
 
-def speak(text: str, model: str="aura-luna-en", filename :str="data.mp3"):
+def speak(text: str, model: str=id):
+        filename :str="data.mp3"
         url = "https://api.deepai.org/speech_response"
 
         payload = {
             "model": model,
             "text": text
         }
         response = requests.post(url, json=payload)
@@ -33,7 +32,8 @@
         else:
             with open(filename, 'wb') as f:
                 f.write(response.content)
             playsound.playsound(filename)
             os.remove(filename)
 
 
+speak("i dont know sir but i am felling not good today",l)
```

### Comparing `NetHyTech-DeepTTS-0.1/NetHyTech_DeepTTS.egg-info/PKG-INFO` & `NetHyTech-DeepTTS-0.2/NetHyTech_DeepTTS.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetHyTech-DeepTTS
-Version: 0.1
+Version: 0.2
 Summary: A Python package for text-to-speech conversion using DeepAI API.
 Author: Anubhav Chaturvedi
 Author-email: chaturvedianubhav520@example.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: License :: OSI Approved :: MIT License
@@ -15,49 +15,35 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Speech Synthesis with DeepAI API
 
 This Python script uses the DeepAI API to convert text to speech and play the resulting audio. It allows you to choose from various voices provided by DeepAI.
 
+## pip 
+
+```python
+from NetHyTech_DeepTTS import speak
+
+speak("i dont know sir but i am felling not good today",l)
+
+```
+
 ## Prerequisites
 
 Before running the script, ensure you have the following installed:
 - Python 3.11.4
 - `playsound` library
 - `requests` library
 
 You can install the required libraries using pip:
 ```bash
 pip install playsound requests
 ```
 
-## Usage
-
-### Function
-
-The script defines a single function:
-
-```python
-def speak(text: str, model: str="aura-luna-en", filename :str="data.mp3"):
-    url = "https://api.deepai.org/speech_response"
-
-    payload = {
-        "model": model,
-        "text": text
-    }
-    response = requests.post(url, json=payload)
-    if response.status_code != 200: return f"Error: {response.status_code} - {response.text}"
-    else:
-        with open(filename, 'wb') as f:
-            f.write(response.content)
-        playsound.playsound(filename)
-        os.remove(filename)
-```
-
 ### Parameters
 
 - `text` (str): The text you want to convert to speech.
 - `model` (str, optional): The voice model to use. Defaults to "aura-luna-en".
 - `filename` (str, optional): The name of the temporary file to save the audio. Defaults to "data.mp3".
 
 ### Voice Models
@@ -77,15 +63,15 @@
 - `"aura-zeus-en"`: James (Male US English)
 
 ### Example
 
 Here's an example of how to use the `speak` function:
 
 ```python
-speak("Hello, this is a test message.", model="aura-luna-en")
+speak("i dont know sir but i am felling not good today",l) 
 ```
 
 This will convert the text "Hello, this is a test message." to speech using the "aura-luna-en" (Emily, Female US English) voice model and play the resulting audio.
 
 ## Notes
 
 - Ensure you have an active internet connection as the script makes a request to the DeepAI API.
```

### Comparing `NetHyTech-DeepTTS-0.1/PKG-INFO` & `NetHyTech-DeepTTS-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NetHyTech-DeepTTS
-Version: 0.1
+Version: 0.2
 Summary: A Python package for text-to-speech conversion using DeepAI API.
 Author: Anubhav Chaturvedi
 Author-email: chaturvedianubhav520@example.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Speech
 Classifier: License :: OSI Approved :: MIT License
@@ -15,49 +15,35 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Speech Synthesis with DeepAI API
 
 This Python script uses the DeepAI API to convert text to speech and play the resulting audio. It allows you to choose from various voices provided by DeepAI.
 
+## pip 
+
+```python
+from NetHyTech_DeepTTS import speak
+
+speak("i dont know sir but i am felling not good today",l)
+
+```
+
 ## Prerequisites
 
 Before running the script, ensure you have the following installed:
 - Python 3.11.4
 - `playsound` library
 - `requests` library
 
 You can install the required libraries using pip:
 ```bash
 pip install playsound requests
 ```
 
-## Usage
-
-### Function
-
-The script defines a single function:
-
-```python
-def speak(text: str, model: str="aura-luna-en", filename :str="data.mp3"):
-    url = "https://api.deepai.org/speech_response"
-
-    payload = {
-        "model": model,
-        "text": text
-    }
-    response = requests.post(url, json=payload)
-    if response.status_code != 200: return f"Error: {response.status_code} - {response.text}"
-    else:
-        with open(filename, 'wb') as f:
-            f.write(response.content)
-        playsound.playsound(filename)
-        os.remove(filename)
-```
-
 ### Parameters
 
 - `text` (str): The text you want to convert to speech.
 - `model` (str, optional): The voice model to use. Defaults to "aura-luna-en".
 - `filename` (str, optional): The name of the temporary file to save the audio. Defaults to "data.mp3".
 
 ### Voice Models
@@ -77,15 +63,15 @@
 - `"aura-zeus-en"`: James (Male US English)
 
 ### Example
 
 Here's an example of how to use the `speak` function:
 
 ```python
-speak("Hello, this is a test message.", model="aura-luna-en")
+speak("i dont know sir but i am felling not good today",l) 
 ```
 
 This will convert the text "Hello, this is a test message." to speech using the "aura-luna-en" (Emily, Female US English) voice model and play the resulting audio.
 
 ## Notes
 
 - Ensure you have an active internet connection as the script makes a request to the DeepAI API.
```

### Comparing `NetHyTech-DeepTTS-0.1/setup.py` & `NetHyTech-DeepTTS-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Read the content of README.md for long description
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='NetHyTech-DeepTTS',
-    version='0.1',
+    version='0.2',
     author='Anubhav Chaturvedi',
     author_email='chaturvedianubhav520@example.com',
     description='A Python package for text-to-speech conversion using DeepAI API.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

