# Comparing `tmp/calculate_savings-0.1.3.tar.gz` & `tmp/calculate_savings-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calculate_savings-0.1.3.tar", last modified: Sun May 26 12:48:05 2024, max compression
+gzip compressed data, was "calculate_savings-0.1.4.tar", last modified: Mon May 27 04:29:28 2024, max compression
```

## Comparing `calculate_savings-0.1.3.tar` & `calculate_savings-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.999641 calculate_savings-0.1.3/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       23 2024-05-21 13:12:43.000000 calculate_savings-0.1.3/MANIFEST.in
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1228 2024-05-26 12:48:04.999439 calculate_savings-0.1.3/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      666 2024-05-26 12:46:41.000000 calculate_savings-0.1.3/README.md
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-26 12:48:04.999678 calculate_savings-0.1.3/setup.cfg
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1094 2024-05-26 12:47:37.000000 calculate_savings-0.1.3/setup.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.983550 calculate_savings-0.1.3/src/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     6148 2024-05-21 13:35:14.000000 calculate_savings-0.1.3/src/.DS_Store
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.999164 calculate_savings-0.1.3/src/calculate_savings.egg-info/
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     1228 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/PKG-INFO
--rw-r--r--   0 takenakayuuki   (501) staff       (20)      329 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/SOURCES.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/dependency_links.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/entry_points.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-26 12:48:04.000000 calculate_savings-0.1.3/src/calculate_savings.egg-info/top_level.txt
--rw-r--r--   0 takenakayuuki   (501) staff       (20)     4747 2024-05-25 11:19:57.000000 calculate_savings-0.1.3/src/calculate_savings.py
-drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-26 12:48:04.984221 calculate_savings-0.1.3/src/data/
--rw-r--r--   0 takenakayuuki   (501) staff       (20) 19188118 2024-05-21 05:28:42.000000 calculate_savings-0.1.3/src/data/hon-maikin-k-jissu.csv
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-27 04:29:28.336243 calculate_savings-0.1.4/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       23 2024-05-21 13:12:43.000000 calculate_savings-0.1.4/MANIFEST.in
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1238 2024-05-27 04:29:28.336034 calculate_savings-0.1.4/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      676 2024-05-27 04:27:51.000000 calculate_savings-0.1.4/README.md
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       38 2024-05-27 04:29:28.336296 calculate_savings-0.1.4/setup.cfg
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1094 2024-05-27 04:28:08.000000 calculate_savings-0.1.4/setup.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-27 04:29:28.319567 calculate_savings-0.1.4/src/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     6148 2024-05-27 04:24:35.000000 calculate_savings-0.1.4/src/.DS_Store
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-27 04:29:28.335752 calculate_savings-0.1.4/src/calculate_savings.egg-info/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     1238 2024-05-27 04:29:28.000000 calculate_savings-0.1.4/src/calculate_savings.egg-info/PKG-INFO
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)      329 2024-05-27 04:29:28.000000 calculate_savings-0.1.4/src/calculate_savings.egg-info/SOURCES.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)        1 2024-05-27 04:29:28.000000 calculate_savings-0.1.4/src/calculate_savings.egg-info/dependency_links.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       61 2024-05-27 04:29:28.000000 calculate_savings-0.1.4/src/calculate_savings.egg-info/entry_points.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)       18 2024-05-27 04:29:28.000000 calculate_savings-0.1.4/src/calculate_savings.egg-info/top_level.txt
+-rw-r--r--   0 takenakayuuki   (501) staff       (20)     4758 2024-05-27 04:26:53.000000 calculate_savings-0.1.4/src/calculate_savings.py
+drwxr-xr-x   0 takenakayuuki   (501) staff       (20)        0 2024-05-27 04:29:28.320225 calculate_savings-0.1.4/src/data/
+-rw-r--r--   0 takenakayuuki   (501) staff       (20) 19188118 2024-05-21 05:28:42.000000 calculate_savings-0.1.4/src/data/hon-maikin-k-jissu.csv
```

### Comparing `calculate_savings-0.1.3/PKG-INFO` & `calculate_savings-0.1.4/src/calculate_savings.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calculate_savings
-Version: 0.1.3
+Name: calculate-savings
+Version: 0.1.4
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 __calculate-savings__<br>
 Using data from Japan's Monthly Survey of Labour Statistics, the salary in 10 years' time is predicted using scikit-learn linear regression from 55 years' salary. Based on this, the amount of savings in 10 years' time is predicted using cost of living and extra expenditure as inputs.
 
 __How to run calculate_savings__<br>
-calculate_savings
+$ calculate_savings
 
 __output__
 -  Savings till 10 years(yen): xxxxx
 -  result.png
 
-__Use of data__
-出典：「毎月勤労統計調査」厚生労働省
+__Use of data__<br>
+出典：「毎月勤労統計調査」厚生労働省<br>
 https://www.e-stat.go.jp/stat-search/files?page=1&layout=datalist&toukei=00450071&tstat=000001011791&cycle=0&tclass1=000001035519&tclass2=000001144508&tclass3val=0
```

### Comparing `calculate_savings-0.1.3/README.md` & `calculate_savings-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __calculate-savings__<br>
 Using data from Japan's Monthly Survey of Labour Statistics, the salary in 10 years' time is predicted using scikit-learn linear regression from 55 years' salary. Based on this, the amount of savings in 10 years' time is predicted using cost of living and extra expenditure as inputs.
 
 __How to run calculate_savings__<br>
-calculate_savings
+$ calculate_savings
 
 __output__
 -  Savings till 10 years(yen): xxxxx
 -  result.png
 
-__Use of data__
-出典：「毎月勤労統計調査」厚生労働省
+__Use of data__<br>
+出典：「毎月勤労統計調査」厚生労働省<br>
 https://www.e-stat.go.jp/stat-search/files?page=1&layout=datalist&toukei=00450071&tstat=000001011791&cycle=0&tclass1=000001035519&tclass2=000001144508&tclass3val=0
```

### Comparing `calculate_savings-0.1.3/setup.py` & `calculate_savings-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="calculate_savings",
-    version="0.1.3",
+    version="0.1.4",
     author="YukiTakenaka",
     author_email="s2222024@stu.musashino-u.ac.jp",
     description="How much can you save in 10 years by predicting your salary?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/takenakayuuki0901/calculate_savings.git",
     project_urls={
```

### Comparing `calculate_savings-0.1.3/src/.DS_Store` & `calculate_savings-0.1.4/src/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -91,16 +91,16 @@
 000005a0: 6200 0000 b862 706c 6973 7430 30d6 0102  b....bplist00...
 000005b0: 0304 0506 0707 0907 0b07 5d53 686f 7753  ..........]ShowS
 000005c0: 7461 7475 7342 6172 5b53 686f 7754 6f6f  tatusBar[ShowToo
 000005d0: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
 000005e0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
 000005f0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
 00000600: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-00000610: 0909 0809 5f10 187b 7b37 3832 2c20 3330  ...._..{{782, 30
-00000620: 347d 2c20 7b36 3736 2c20 3636 347d 7d09  4}, {676, 664}}.
+00000610: 0909 0809 5f10 187b 7b38 3039 2c20 2d35  ...._..{{809, -5
+00000620: 307d 2c20 7b36 3736 2c20 3636 347d 7d09  0}, {676, 664}}.
 00000630: 0815 232f 3b52 5f6b 6c6d 6e6f 8a00 0000  ..#/;R_klmno....
 00000640: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
 00000650: 0000 0000 0000 0000 0000 0000 8b00 0000  ................
 00000660: 0400 6400 6100 7400 616c 6731 5363 6f6d  ..d.a.t.alg1Scom
 00000670: 7000 0000 0000 0000 0000 0000 0400 6400  p.............d.
 00000680: 6100 7400 616d 6f44 4462 6c6f 6200 0000  a.t.amoDDblob...
 00000690: 0888 3100 216a fec5 4100 0000 0400 6400  ..1.!j..A.....d.
```

### Comparing `calculate_savings-0.1.3/src/calculate_savings.egg-info/PKG-INFO` & `calculate_savings-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: calculate-savings
-Version: 0.1.3
+Name: calculate_savings
+Version: 0.1.4
 Summary: How much can you save in 10 years by predicting your salary?
 Home-page: https://github.com/takenakayuuki0901/calculate_savings.git
 Author: YukiTakenaka
 Author-email: s2222024@stu.musashino-u.ac.jp
 Project-URL: Bug Tracker, https://github.com/takenakayuuki0901/calculate_savings.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,16 +12,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 __calculate-savings__<br>
 Using data from Japan's Monthly Survey of Labour Statistics, the salary in 10 years' time is predicted using scikit-learn linear regression from 55 years' salary. Based on this, the amount of savings in 10 years' time is predicted using cost of living and extra expenditure as inputs.
 
 __How to run calculate_savings__<br>
-calculate_savings
+$ calculate_savings
 
 __output__
 -  Savings till 10 years(yen): xxxxx
 -  result.png
 
-__Use of data__
-出典：「毎月勤労統計調査」厚生労働省
+__Use of data__<br>
+出典：「毎月勤労統計調査」厚生労働省<br>
 https://www.e-stat.go.jp/stat-search/files?page=1&layout=datalist&toukei=00450071&tstat=000001011791&cycle=0&tclass1=000001035519&tclass2=000001144508&tclass3val=0
```

### Comparing `calculate_savings-0.1.3/src/calculate_savings.py` & `calculate_savings-0.1.4/src/calculate_savings.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     future_X = future_dates.year.values.reshape(-1, 1)
     future_y = model.predict(future_X)
 
     # 10年後までの貯金を計算
     savings = 0
     for projected_income in future_y:
-        savings += projected_income - (living_expenses + discretionary_spending)
+        savings += (projected_income - (living_expenses + discretionary_spending)) * 12
         print(
             f"{savings} = {projected_income} - {living_expenses} - {discretionary_spending}"
         )
 
     # プロット
     plt.figure(figsize=(12, 8))
 
@@ -137,17 +137,17 @@
 
     return savings
 
 
 def main():
     # Asking the user for living expenses and discretionary spending
     try:
-        living_expenses = float(input("Enter your living expenses for 1 year: "))
+        living_expenses = float(input("Enter your living expenses for 1 mounth: "))
         discretionary_spending = float(
-            input("Enter your discretionary spending for 1 year: ")
+            input("Enter your discretionary spending for 1 mounth: ")
         )
     except ValueError:
         print("Invalid input. Please enter numeric values.")
         return
 
     print(
         "Savings till 10 years(yen): ",
```

### Comparing `calculate_savings-0.1.3/src/data/hon-maikin-k-jissu.csv` & `calculate_savings-0.1.4/src/data/hon-maikin-k-jissu.csv`

 * *Files identical despite different names*

