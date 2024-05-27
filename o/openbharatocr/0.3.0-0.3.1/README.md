# Comparing `tmp/openbharatocr-0.3.0.tar.gz` & `tmp/openbharatocr-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbharatocr-0.3.0.tar", last modified: Thu May 16 05:45:06 2024, max compression
+gzip compressed data, was "openbharatocr-0.3.1.tar", last modified: Mon May 27 05:57:55 2024, max compression
```

## Comparing `openbharatocr-0.3.0.tar` & `openbharatocr-0.3.1.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:45:06.928441 openbharatocr-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-16 05:45:06.928441 openbharatocr-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:45:06.924441 openbharatocr-0.3.0/openbharatocr/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:45:06.928441 openbharatocr-0.3.0/openbharatocr/ocr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/aadhaar.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/driving_licence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/pan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/passport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/vehicle_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7079 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/voter_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/openbharatocr/ocr/water_bill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:45:06.928441 openbharatocr-0.3.0/openbharatocr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 05:45:06.000000 openbharatocr-0.3.0/openbharatocr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 05:45:06.928441 openbharatocr-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 05:45:01.000000 openbharatocr-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/ocr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/aadhaar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/driving_licence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/pan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/passport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/vehicle_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/voter_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4686 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/ocr/water_bill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.174043 openbharatocr-0.3.1/openbharatocr/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/openbharatocr/unit_tests/test_pan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/openbharatocr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 05:57:55.000000 openbharatocr-0.3.1/openbharatocr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-27 05:57:55.178043 openbharatocr-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-27 05:57:50.000000 openbharatocr-0.3.1/setup.py
```

### Comparing `openbharatocr-0.3.0/LICENSE` & `openbharatocr-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.0/PKG-INFO` & `openbharatocr-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.3.0
-Summary: openbharatocr is an opensource python library for ocr Indian government documents 
+Version: 0.3.1
+Summary: openbharatocr is an opensource python library for ocr Indian government documents
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openbharatocr-0.3.0/README.md` & `openbharatocr-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/aadhaar.py` & `openbharatocr-0.3.1/openbharatocr/ocr/aadhaar.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,99 +3,90 @@
 import pytesseract
 from PIL import Image
 import tempfile
 import uuid
 
 
 def extract_name(input):
-
     name_regex = r"\b[A-Z][a-z]+(?:\s+[A-Z][a-z]+)*\b"
     names = re.findall(name_regex, input)
     full_name = ""
     for name in names:
         if "Government" not in name and "India" not in name:
             full_name = name
             break
 
     return full_name
 
 
 def extract_fathers_name(input):
-
     regex = r"(?:S.?O|D.?O)[:\s]*([A-Za-z]+(?: [A-Za-z]+)*)"
     match = re.findall(regex, input)
     fathers_name = ""
     if match:
         fathers_name = match[-1]
 
     return fathers_name
 
 
 def extract_aadhaar(input):
-
     regex = r"\b\d{4}\s?\d{4}\s?\d{4}\b"
     match = re.search(regex, input)
     aadhaar_number = match.group(0) if match else ""
 
     return aadhaar_number
 
 
 def extract_dob(input):
-
     regex = r"\b(\d{2}/\d{2}/\d{4})\b"
     match = re.search(regex, input)
     dob = match.group(0) if match else ""
 
     return dob
 
 
 def extract_yob(input):
-
     regex = r"\b\d{4}\b"
     match = re.search(regex, input)
     yob = match.group(0) if match else ""
 
     return yob
 
 
 def extract_gender(input):
-
     if re.search("Female", input) or re.search("FEMALE", input):
         return "Female"
     if re.search("Male", input) or re.search("MALE", input):
         return "Male"
     return "Other"
 
 
 def extract_address(input):
-
     regex = r"Address:\s*((?:.|\n)*?\d{6})"
     match = re.search(regex, input)
     address = match.group(1) if match else ""
 
     return address
 
 
 def extract_back_aadhaar_details(image_path):
-
     image = Image.open(image_path)
 
     extracted_text = pytesseract.image_to_string(image)
 
     fathers_name = extract_fathers_name(extracted_text)
     address = extract_address(extracted_text)
 
     return {
         "Father's Name": fathers_name,
         "Address": address,
     }
 
 
 def extract_front_aadhaar_details(image_path):
-
     image = Image.open(image_path)
 
     extracted_text = pytesseract.image_to_string(image)
 
     full_name = extract_name(extracted_text)
     dob = extract_dob(extracted_text)
     gender = extract_gender(extracted_text)
```

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/driving_licence.py` & `openbharatocr-0.3.1/openbharatocr/ocr/driving_licence.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,22 @@
 from datetime import datetime
 from dateutil.parser import parse
 import tempfile
 import uuid
 
 
 def extract_driving_licence_number(input):
-
     regex = r"[A-Z]{2}[-\s]\d{13}|[A-Z]{2}[0-9]{2}\s[0-9]{11}"
     match = re.search(regex, input)
     driving_licence_number = match.group(0) if match else ""
 
     return driving_licence_number
 
 
 def extract_all_dates(input):
-
     regex = r"\b\d{2}[/-]\d{2}[/-]\d{4}\b"
     dates = re.findall(regex, input)
     dates = sorted(dates, key=lambda x: int(re.split(r"[-/]", x)[-1]))
 
     seen = set()
     unique_dates = []
 
@@ -51,27 +49,25 @@
         validity.append(unique_dates[i])
         i += 1
 
     return dob, doi, validity
 
 
 def clean_input(match):
-
     cleaned = []
 
     for name in match:
         split_name = name.split("\n")
         for chunk in split_name:
             cleaned.append(chunk)
 
     return cleaned
 
 
 def extract_all_names(input):
-
     regex = r"\b[A-Z\s]+\b"
     match = re.findall(regex, input)
 
     names = []
     cleaned = clean_input(match)
 
     stopwords = [
@@ -109,15 +105,14 @@
         if not any(word in name for word in stopwords) and len(name.strip()) > 3
     ]
 
     return names
 
 
 def extract_address_regex(input):
-
     regex_list = [
         r"Address\s*:\s*\n*(.*?)(?=\n\n|\Z)",
         r"Add\b\s*(.*?)(?=\bPIN|$)",
         r"Address\b\s*(.*?)(?=\bPIN|$)",
         r"Address\s*:\s*((?:(?!(?:Valid Till)).*(?:\n|$))+)",
         r"ADDRESS - (.+?)(?= (?:\b\d{6}\b|$))",
         r"Address\s*:\s*((?:(?!(?:Valid Till)).*(?:\n|$))+)",
@@ -184,15 +179,14 @@
 
         address = " ".join(split_address)
 
         return address
 
 
 def extract_auth_allowed(input):
-
     auth_types, auth_allowed = [
         "MCWG",
         "M.CYL.",
         "LMV-NT",
         "LMV",
         "TRANS",
         "INVCRG",
@@ -202,28 +196,26 @@
         if auth in input:
             auth_allowed.append(auth)
 
     return auth_allowed
 
 
 def expired(input):
-
     try:
         date = parse(input, dayfirst=True)
         curr = datetime.now()
         diff = date - curr
         if diff.days >= 0:
             return False
         return True
     except:
         return False
 
 
 def extract_driving_license_details(image_path):
-
     image = Image.open(image_path)
 
     extracted_text = pytesseract.image_to_string(image)
 
     names = extract_all_names(extracted_text)
     full_name = names[0] if len(names) > 0 else ""
     swd_name = names[1] if len(names) > 1 else ""
```

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/pan.py` & `openbharatocr-0.3.1/openbharatocr/ocr/pan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import re
 import pytesseract
 import imghdr
 from PIL import Image
 
 
 def clean_input(match):
-
     cleaned = []
 
     for name in match:
         split_name = name.split("\n")
         for chunk in split_name:
             cleaned.append(chunk)
 
     return cleaned
 
 
 def extract_all_names(input):
-
     regex = r"\n[A-Z\s]+\b"
     match = re.findall(regex, input)
 
     names = []
     cleaned = clean_input(match)
 
     stopwords = ["INDIA", "OF", "TAX", "GOVT", "DEPARTMENT", "INCOME"]
@@ -32,15 +30,14 @@
         if not any(word in name for word in stopwords) and len(name.strip()) > 3
     ]
 
     return names
 
 
 def extract_pan(input):
-
     regex = r"[A-Z]{5}[0-9]{4}[A-Z]"
     match = re.search(regex, input)
     pan_number = match.group(0) if match else ""
 
     return pan_number
 
 
@@ -57,15 +54,14 @@
     match = re.search(regex, input)
     dob = match.group(0) if match else ""
 
     return dob
 
 
 def extract_pan_details(image_path):
-
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
 
     format = imghdr.what(image_path)
     if format != "jpeg":
         image.save("image.jpg", "JPEG")
```

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/passport.py` & `openbharatocr-0.3.1/openbharatocr/ocr/passport.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import pytesseract
 from PIL import Image
 import cv2
 import numpy as np
 
 
 def preprocess_for_bold_text(image):
-
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1, 1))
     opening = cv2.morphologyEx(gray, cv2.MORPH_OPEN, kernel)
     contrast = cv2.addWeighted(opening, 2, opening, -0.5, 0)
 
     _, binary = cv2.threshold(contrast, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
@@ -18,29 +17,27 @@
         binary, -1, np.array([[0, -1, 0], [-1, 5, -1], [0, -1, 0]])
     )
 
     return sharpened
 
 
 def extract_names(input):
-
     name_regex = r"Names[\s:]+([A-Za-z\s]+)(?:\n|$)"
     surname_regex = r"Surname[\s:]+([A-Za-z\s]+)(?:\n|$)"
 
     name_match = re.search(name_regex, input, re.IGNORECASE)
     surname_match = re.search(surname_regex, input, re.IGNORECASE)
 
     name = name_match.group(1).strip() if name_match else ""
     surname = surname_match.group(1).strip() if surname_match else ""
 
     return name, surname
 
 
 def extract_all_dates(input):
-
     regex = r"\b(\d{2}[/\-.]\d{2}[/\-.](?:\d{4}|\d{2}))\b"
     dates = re.findall(regex, input)
     dates = sorted(dates, key=lambda x: int(re.split(r"[-/]", x)[-1]))
 
     seen = set()
     unique_dates = []
 
@@ -49,15 +46,14 @@
             seen.add(date)
             unique_dates.append(date)
 
     return unique_dates
 
 
 def extract_all_places(input):
-
     dates = re.findall(r"\b(\d{2}[/\-.]\d{2}[/\-.](?:\d{4}|\d{2}))\b", input)
     last_date = dates[-1] if dates else None
 
     all_places = []
 
     if last_date:
         places = input.split("\n")
@@ -65,24 +61,22 @@
             if re.match(r'^[A-Z,. -\'"]+$', place) and place.strip():
                 all_places.append(place)
 
     return all_places
 
 
 def extract_passport_number(input):
-
     regex = r"[A-Z][0-9]{7}"
     match = re.search(regex, input)
     passport_number = match.group(0) if match else ""
 
     return passport_number
 
 
 def extract_details(input):
-
     lines = input.split("\n")
     clean = []
     for line in lines:
         clean_line = re.sub(r"[^a-zA-Z\s]", "", line)
         clean_line = " ".join(word for word in clean_line.split() if len(word) > 1)
         if (
             re.match(r"^[A-Z\s]{3,}$", clean_line)
@@ -103,15 +97,14 @@
         elif "F" in clean[-1]:
             gender = "Female"
 
     return gender, name, surname
 
 
 def extract_passport_details(image_path):
-
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
     image.save("image.jpg", "JPEG")
     image = cv2.imread("image.jpg")
     preprocessed = preprocess_for_bold_text(image)
     cv2.imwrite("preprocessed_image.jpg", preprocessed)
```

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/vehicle_registration.py` & `openbharatocr-0.3.1/openbharatocr/ocr/vehicle_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import re
 import pytesseract
 from PIL import Image
 
 
 def extract_names(input):
-
     regex_swd = r"dual\sOwner\)?\s*:?\s*([A-Z.]+\s[A-Z.]+\s[A-Z.]+)"
     match = re.search(regex_swd, input, re.IGNORECASE)
     swd = match.group(1) if match else ""
 
     regex_name = r"NAME\s*:?\s*([A-Z]+\s[A-Z]+)"
     match_name = re.search(regex_name, input, re.IGNORECASE)
     name = match_name.group(1) if match_name else ""
@@ -23,93 +22,83 @@
         match = re.search(regex_swd, input, re.IGNORECASE)
         swd = match.group(1) if match else ""
 
     return name, swd
 
 
 def extract_reg_number(input):
-
     regex = r"(?=.*\d)[A-Z0-9]{10}"
     match = re.search(regex, input)
     reg_number = match.group(0) if match else ""
 
     return reg_number
 
 
 def extract_chasis(input):
-
     regex = r"[A-Z0-9]{17,18}"
     match = re.search(regex, input)
     chasis = match.group(0) if match else ""
 
     return chasis
 
 
 def extract_fuel_type(input):
-
     regex = r"Fuel(?:\s+Type)?\s*[\s:\.]\s*([A-Z/]+)\s"
     match = re.search(regex, input, re.IGNORECASE)
     fuel_type = match.group(1) if match else ""
     return fuel_type
 
 
 def extract_vehicle_class(input):
-
     regex = r"(?:Veh.c.e\sClass|Veh\sCl)\s*[\s:]\s*([A-Z0-9/()-]+)\s([A-Z0-9/()-]+)\s"
     match = re.search(regex, input, re.IGNORECASE)
     vehicle_class = match.group(1) if match else ""
     return vehicle_class
 
 
 def extract_manufacturer(input):
-
     regex = r"MFR\s*:\s*([A-Z\s]+)\n"
     match = re.search(regex, input, re.IGNORECASE)
     manufacturer = match.group(1) if match else ""
     return manufacturer
 
 
 def extract_tax_info(input):
-
     regex = r"Tax\sUp\s{0,1}to\s*:\s*([A-Z]+)\s"
     match = re.search(regex, input, re.IGNORECASE)
     tax_up_to = match.group(1) if match else ""
     return tax_up_to
 
 
 def extract_model(input):
-
     regex = r"Mode.\s*[\s:]\s*([A-Z0-9/+()-.]+(?:\s+[^\w\n]*[A-Z0-9/+()-.]+){0,3})\s"
     match = re.search(regex, input, re.IGNORECASE)
     model = match.group(1) if match else ""
     return model
 
 
 def extract_all_dates(input_text):
-
     regex = r"\b(\d{1,2}[/\-.](?:\d{2}|\d{4}|\w{3})[/\-.]\d{2,4})\b"
     dates = re.findall(regex, input_text)
     sorted_dates = sorted(
         dates, key=lambda date: int(date.split("/")[-1].split("-")[-1])
     )
 
     return sorted_dates
 
 
 def extract_address(input):
-
     regex = r"Address:?\s*((?:.|\n)*?\d{6})"
     match = re.search(regex, input, re.IGNORECASE)
     address = match.group(1) if match else ""
 
     return address
 
 
 def extract_vehicle_registration_details(image_path):
-
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
 
     names = extract_names(extracted_text)
     name, swd = names[0], names[1]
 
     dates = extract_all_dates(extracted_text)
```

### Comparing `openbharatocr-0.3.0/openbharatocr/ocr/voter_id.py` & `openbharatocr-0.3.1/openbharatocr/ocr/voter_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 )  # https://drive.google.com/file/d/1SEst2lVoFDOgUVLZ5kje9GTb2tHRA8U-/view?usp=sharing
 YOLO_WEIGHT = os.environ.get(
     "YOLO_WEIGHT", "yolov3_custom_6000.weights"
 )  # https://drive.google.com/file/d/1cGGstycfogmO6O7ToB2DAEXOgTWVgINh/view?usp=drive_link
 
 
 def preprocess_for_bold_text(image):
-
     gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
 
     kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (1, 1))
     opening = cv2.morphologyEx(gray, cv2.MORPH_OPEN, kernel)
     contrast = cv2.addWeighted(opening, 2, opening, -0.5, 0)
 
     _, binary = cv2.threshold(contrast, 0, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU)
@@ -97,55 +96,50 @@
                 text = pytesseract.image_to_string(crop_img, config="--psm 6")
                 detected_texts[label] = text.strip()
 
         return detected_texts
 
 
 def extract_voter_id(input):
-
     regex = r".{0,3}[0-9]{7}"
     match = re.search(regex, input)
     voter_id = match.group(0) if match else ""
 
     return voter_id
 
 
 def extract_names(input):
-
     regex = r"Name\s*[:=+]?\s*(.*)"
     matches = re.findall(regex, input, re.IGNORECASE)
     names = [match.strip() for match in matches] if matches else []
 
     return names
 
 
 def extract_lines_with_uppercase_words(input):
-
     lines_with_uppercase_words = []
     pattern = r"\b[A-Z]+(?:\s+[A-Z]+)*\b"
     for line in input.split("\n"):
         if re.search(pattern, line):
             uppercase_words = re.findall(pattern, line)
             for word in uppercase_words:
                 lines_with_uppercase_words.append(word)
     return lines_with_uppercase_words
 
 
 def extract_gender(input):
-
     if "Female" in input or "FEMALE" in input:
         return "Female"
     elif "Male" in input or "MALE" in input:
         return "Male"
     else:
         return ""
 
 
 def extract_date(input):
-
     regex = r"\b([0-9X]{2}[/\-.][0-9X]{2}[/\-.](?:\d{4}|\d{2}))\b"
     match = re.search(regex, input)
     dob = match.group(0) if match else ""
 
     return dob
 
 
@@ -159,15 +153,14 @@
         match = re.search(regex, input)
         address = match.group(0) if match else ""
 
     return address
 
 
 def extract_voterid_details_front(image_path):
-
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
 
     voter_id = extract_voter_id(extracted_text)
 
     names = extract_names(extracted_text)
     electors_name = names[0] if len(names) > 0 else ""
@@ -208,26 +201,24 @@
             "Father's Name": fathers_name,
             "Gender": gender,
             "Date of Birth": dob,
         }
 
 
 def extract_voterid_details_back(image_path):
-
     image = Image.open(image_path)
     extracted_text = pytesseract.image_to_string(image)
 
     address = extract_address(extracted_text)
     doi = extract_date(extracted_text)
 
     return {"Address": address, "Date of Issue": doi}
 
 
 def voter_id_front(front_path):
-
     image = Image.open(front_path)
     extracted_text = pytesseract.image_to_string(image)
 
     if (
         "Date" in extracted_text
         or "Age" in extracted_text
         or "Sex" in extracted_text
```

### Comparing `openbharatocr-0.3.0/openbharatocr.egg-info/PKG-INFO` & `openbharatocr-0.3.1/openbharatocr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openbharatocr
-Version: 0.3.0
-Summary: openbharatocr is an opensource python library for ocr Indian government documents 
+Version: 0.3.1
+Summary: openbharatocr is an opensource python library for ocr Indian government documents
 Home-page: https://github.com/essentiasoftserv/openbharatocr
 Author: essentiasoftserv
 Author-email: kunal@essentia.dev
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `openbharatocr-0.3.0/openbharatocr.egg-info/SOURCES.txt` & `openbharatocr-0.3.1/openbharatocr.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,8 +16,10 @@
 openbharatocr/ocr/api.py
 openbharatocr/ocr/common.py
 openbharatocr/ocr/driving_licence.py
 openbharatocr/ocr/pan.py
 openbharatocr/ocr/passport.py
 openbharatocr/ocr/vehicle_registration.py
 openbharatocr/ocr/voter_id.py
-openbharatocr/ocr/water_bill.py
+openbharatocr/ocr/water_bill.py
+openbharatocr/unit_tests/__init__.py
+openbharatocr/unit_tests/test_pan.py
```

### Comparing `openbharatocr-0.3.0/setup.py` & `openbharatocr-0.3.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(
     name="openbharatocr",
-    version="0.3.0",
-    description="openbharatocr is an opensource python library for ocr Indian government documents ",
+    version="0.3.1",
+    description="openbharatocr is an opensource python library for ocr Indian government documents",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/essentiasoftserv/openbharatocr",
     author="essentiasoftserv",
     python_requires=">=3.6",
     install_requires=install_requires,
     author_email="kunal@essentia.dev",
```

