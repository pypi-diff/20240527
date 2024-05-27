# Comparing `tmp/criterion-site-parser-1.7.tar.gz` & `tmp/criterion_site_parser-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "criterion-site-parser-1.7.tar", last modified: Thu Apr 27 18:31:12 2023, max compression
+gzip compressed data, was "criterion_site_parser-1.8.tar", last modified: Mon May 27 15:34:31 2024, max compression
```

## Comparing `criterion-site-parser-1.7.tar` & `criterion_site_parser-1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/license
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.513909 criterion-site-parser-1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-27 18:31:12.000000 criterion-site-parser-1.7/src/criterion_site_parser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/critparse/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionMiniSeriesParse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionMovieParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/CriterionParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/OutApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/OutText.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/critparse/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:31:12.517909 criterion-site-parser-1.7/src/testcritparse/
--rw-r--r--   0 runner    (1001) docker     (123)    10878 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/testcritparse/test_CriterionMovieParse.py
--rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-27 18:31:01.000000 criterion-site-parser-1.7/src/testcritparse/test_CriterionParser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/license
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:30.998529 criterion_site_parser-1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-27 15:34:30.000000 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-27 15:34:30.000000 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 15:34:30.000000 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-27 15:34:30.000000 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-27 15:34:30.000000 criterion_site_parser-1.8/src/criterion_site_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/src/critparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/CriterionMiniSeriesParse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/CriterionMovieParse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/CriterionParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/OutApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/OutText.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/critparse/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 15:34:31.002529 criterion_site_parser-1.8/src/testcritparse/
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/testcritparse/test_CriterionMovieParse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15461 2024-05-27 15:34:26.000000 criterion_site_parser-1.8/src/testcritparse/test_CriterionParser.py
```

### Comparing `criterion-site-parser-1.7/PKG-INFO` & `criterion_site_parser-1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criterion-site-parser
-Version: 1.7
+Version: 1.8
 Summary: Prints movies information parsed from criterionchannel.com
 Author-email: pistolbarrel <gboes@pistolbarrel.net>
 License: MIT License
         
         Copyright (c) 2022 pistolbarrel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,7 +28,10 @@
 Project-URL: Homepage, https://github.com/pistolbarrel/criterion-site-parser
 Keywords: criterion,parser,movies
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: html5lib
+Requires-Dist: bs4
+Requires-Dist: requests
```

### Comparing `criterion-site-parser-1.7/license` & `criterion_site_parser-1.8/license`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/pyproject.toml` & `criterion_site_parser-1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "criterion-site-parser"
-version = "1.7"
+version = "1.8"
 description = "Prints movies information parsed from criterionchannel.com"
 readme = "README.md"
 authors = [{ name = "pistolbarrel", email = "gboes@pistolbarrel.net" }]
 license = { file = "license" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `criterion-site-parser-1.7/src/criterion_site_parser.egg-info/PKG-INFO` & `criterion_site_parser-1.8/src/criterion_site_parser.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: criterion-site-parser
-Version: 1.7
+Version: 1.8
 Summary: Prints movies information parsed from criterionchannel.com
 Author-email: pistolbarrel <gboes@pistolbarrel.net>
 License: MIT License
         
         Copyright (c) 2022 pistolbarrel
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -28,7 +28,10 @@
 Project-URL: Homepage, https://github.com/pistolbarrel/criterion-site-parser
 Keywords: criterion,parser,movies
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: html5lib
+Requires-Dist: bs4
+Requires-Dist: requests
```

### Comparing `criterion-site-parser-1.7/src/criterion_site_parser.egg-info/SOURCES.txt` & `criterion_site_parser-1.8/src/criterion_site_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/src/critparse/CriterionMiniSeriesParse.py` & `criterion_site_parser-1.8/src/critparse/CriterionMiniSeriesParse.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/src/critparse/CriterionMovieParse.py` & `criterion_site_parser-1.8/src/critparse/CriterionMovieParse.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,25 +69,20 @@
 
     # sometimes you are here but have no stars listed in the movie.
     # i.e., you have diryrcnty descr1 and descr2. Look for this case
     elif "Starring" not in stars:
         descr = stars + "\n\n" + descr
         stars = ""
     country, director, year = process_diryrcnty(diryrcnty)
+    return country, descr, director, stars, year
 
-    # I know of one instance in the Criterion web site  where the country
-    # and year are swapped. It's in the listing for Breathless (1960).
-    # This movie is constantly being added to lists. This is a bit of code
-    # to fix the issue
-    year = year.strip()
-    if not year.isnumeric():
-        # do a simple swap
-        year, country = country, year
 
-    return country, descr, director, stars, year
+def needs_year_country_swap(year):
+    year = year.strip()
+    return not year.isnumeric()
 
 
 def extract_info_len2(info):
     country = descr = director = year = ''
     diryrcnty, descr = info
     if '•' in diryrcnty:
         country, director, year = process_diryrcnty(diryrcnty)
@@ -135,32 +130,42 @@
         director = director.strip()
 
     if country:
         country = country.replace(',', ';')
         country = country.strip()
     return country, director, length, stars, title, just_title
 
+def parse_info(info):
+    country, descr, director, stars, year = '','','','',''
+    if len(info) == 4:
+        country, descr, director, stars, year = extract_info_len4(info)
+    if len(info) == 3:
+        country, descr, director, stars, year = extract_info_len3(info)
+    if len(info) == 2:
+        country, descr, director, year = extract_info_len2(info)
+    if len(info) == 1:
+        descr = info[0]
+    # I know of one instance in the Criterion web site  where the country
+    # and year are swapped. It's in the listing for Breathless (1960).
+    # This movie is constantly being added to lists. This is a bit of code
+    # to fix the issue
+    if needs_year_country_swap(year):
+        year, country = country, year
+    return country, descr, director, stars, year
+
 
 class MovieParse:
     def __init__(self, url, time_supplied=None):
         self.url = url
         r = requests.get(url)
         cmsp_length, table = establish_table(r.content)
-        diryrcnty, stars, descr, director, year, country = '', '', '', '', '', ''
+        diryrcnty = ''
         title, length = extract_title_length(table)
         info = extract_info(table)
-
-        if len(info) == 4:
-            country, descr, director, stars, year = extract_info_len4(info)
-        if len(info) == 3:
-            country, descr, director, stars, year = extract_info_len3(info)
-        if len(info) == 2:
-            country, descr, director, year = extract_info_len2(info)
-        if len(info) == 1:
-            descr = info[0]
+        country, descr, director, stars, year = parse_info(info)
 
         country, director, length, stars, title, just_title \
             = sanitize_data(country, director, length, stars, title, year)
 
         self.length = length
         if cmsp_length:
             self.length = cmsp_length
@@ -170,14 +175,15 @@
         self.title = title
         self.director = director
         self.country = country
         self.stars = stars
         self.descr = descr
         self.year = year.strip()
 
+
     def get_parsed_info(self):
         return [self.just_title, self.year, self.title, self.director, self.country, self.stars,
                 self.descr, self.length, self.url]
 
     def print_info(self, supplied_length=None):
 
         print(self.url)
```

### Comparing `criterion-site-parser-1.7/src/critparse/CriterionParser.py` & `criterion_site_parser-1.8/src/critparse/CriterionParser.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/src/critparse/OutApi.py` & `criterion_site_parser-1.8/src/critparse/OutApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             print('Added "' + movie_info.title + '" via api')
 
     if not suppress_print:
         print()
 
 
 def addViaApi(movie, collection=None, supplied_length=None):
-    put_uri = "http://tower.local:8080/rest/movie"
+    put_uri = "http://tower.local:8080/rest/movies"
     movie_dto = {"title": movie.just_title,
                  "year": movie.year,
                  "actors": movie.stars,
                  "directors": movie.director,
                  "countries": movie.country,
                  "collections": collection,
                  "description": movie.descr}
```

### Comparing `criterion-site-parser-1.7/src/critparse/OutText.py` & `criterion_site_parser-1.8/src/critparse/OutText.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/src/critparse/__main__.py` & `criterion_site_parser-1.8/src/critparse/__main__.py`

 * *Files identical despite different names*

### Comparing `criterion-site-parser-1.7/src/testcritparse/test_CriterionMovieParse.py` & `criterion_site_parser-1.8/src/testcritparse/test_CriterionMovieParse.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,59 +2,68 @@
 from bs4 import BeautifulSoup
 
 from critparse import CriterionMovieParse
 
 
 def test_extract_info4():
     info = ['(“Heads or Tails”)', 'Directed by Guru Dutt • 1954 • India', 'Starring Guru Dutt, Shyama, Jagdish Sethi', 'Guru Dutt blends noir and comedy with delectable results in this tale of Kalu (Dutt), a poor taxi driver in Bombay who finds himself mixed up with two women and organized crime as he attempts to make enough money to marry. O. P. Nayyar’s hugely popular songs helped make this winning mix of humor and suspense one of the first major successes of director-producer Dutt’s career.']
-    country, descr, director, stars, year = CriterionMovieParse.extract_info_len4(info)
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
     assert country == ' India'
     assert descr == 'Guru Dutt blends noir and comedy with delectable results in this tale of Kalu (Dutt), a poor taxi driver in Bombay who finds himself mixed up with two women and organized crime as he attempts to make enough money to marry. O. P. Nayyar’s hugely popular songs helped make this winning mix of humor and suspense one of the first major successes of director-producer Dutt’s career.' + '\n\n' + '(“Heads or Tails”)'
     assert director == 'Directed by Guru Dutt '
     assert stars == 'Starring Guru Dutt, Shyama, Jagdish Sethi'
     assert year == ' 1954 '
 
 
 def test_extract_info_len3():
-    info = ['Directed by Richard Franklin • 1981 •\xa0Australia, United States', 'Starring Stacy Keach, Jamie Lee Curtis, Marion Edward', 'Stacy Keach is Pat Quid, a trucker who plays solitary games to keep his sanity on long hauls through the desolate Australian outback. Jamie Lee Curtis is a free-spirited hitchhiker looking for excitement, with a game of her own. And somewhere up ahead is a maniac in a van whose game may be butchering young women along the highway. But when the killer decides to raise the stakes, Quid’s game becomes personal—and the rules of this road are about to take some deadly turns. Director Richard Franklin packs plenty of Hitchcockian twists and suspense into this sly shocker that ranks among the most surprising thrillers of the 1980s.']
-    country, descr, director, stars, year = CriterionMovieParse.extract_info_len3(info)
-    assert country == ' Australia, United States'
+    info = ['Directed by Richard Franklin • 1981 • Australia, United States', 'Starring Stacy Keach, Jamie Lee Curtis, Marion Edward', 'Stacy Keach is Pat Quid, a trucker who plays solitary games to keep his sanity on long hauls through the desolate Australian outback. Jamie Lee Curtis is a free-spirited hitchhiker looking for excitement, with a game of her own. And somewhere up ahead is a maniac in a van whose game may be butchering young women along the highway. But when the killer decides to raise the stakes, Quid’s game becomes personal—and the rules of this road are about to take some deadly turns. Director Richard Franklin packs plenty of Hitchcockian twists and suspense into this sly shocker that ranks among the most surprising thrillers of the 1980s.']
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
+    assert country.strip() == 'Australia, United States'
     assert descr == 'Stacy Keach is Pat Quid, a trucker who plays solitary games to keep his sanity on long hauls through the desolate Australian outback. Jamie Lee Curtis is a free-spirited hitchhiker looking for excitement, with a game of her own. And somewhere up ahead is a maniac in a van whose game may be butchering young women along the highway. But when the killer decides to raise the stakes, Quid’s game becomes personal—and the rules of this road are about to take some deadly turns. Director Richard Franklin packs plenty of Hitchcockian twists and suspense into this sly shocker that ranks among the most surprising thrillers of the 1980s.'
     assert director == 'Directed by Richard Franklin '
     assert stars == 'Starring Stacy Keach, Jamie Lee Curtis, Marion Edward'
-    assert year == '1981'
+    assert year.strip() == '1981'
 
 
 def test_extract_info_len3_2():
     info = ['ANDREI BOLKONSKY', 'Directed by Sergei Bondarchuk • 1966 • Soviet Union', 'At the height of the Cold War, the Soviet film industry set out to prove it could outdo Hollywood with a production that would dazzle the world: a titanic, awe-inspiring adaptation of Tolstoy’s classic tome in which the fates of three souls—the blundering, good-hearted Pierre; the heroically tragic Prince Andrei; and the radiant, tempestuous Natasha—collide amid the tumult of the Napoleonic Wars. Employing a cast of thousands and an array of innovative camera techniques, director Sergei Bondarchuk conjures a sweeping vision of grand balls that glitter with rococo beauty and breathtaking battles that overwhelm with their expressionistic power. As a statement of Soviet cinema’s might, WAR AND PEACE succeeded wildly, garnering the Academy Award for best foreign-language film and setting a new standard for epic moviemaking.']
-    country, descr, director, stars, year = CriterionMovieParse.extract_info_len3(info)
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
     assert country == ' Soviet Union'
     assert descr == 'ANDREI BOLKONSKY' + '\n\n' + 'At the height of the Cold War, the Soviet film industry set out to prove it could outdo Hollywood with a production that would dazzle the world: a titanic, awe-inspiring adaptation of Tolstoy’s classic tome in which the fates of three souls—the blundering, good-hearted Pierre; the heroically tragic Prince Andrei; and the radiant, tempestuous Natasha—collide amid the tumult of the Napoleonic Wars. Employing a cast of thousands and an array of innovative camera techniques, director Sergei Bondarchuk conjures a sweeping vision of grand balls that glitter with rococo beauty and breathtaking battles that overwhelm with their expressionistic power. As a statement of Soviet cinema’s might, WAR AND PEACE succeeded wildly, garnering the Academy Award for best foreign-language film and setting a new standard for epic moviemaking.'
     assert director == 'Directed by Sergei Bondarchuk '
     assert stars == ''
-    assert year == '1966'
+    assert year.strip() == '1966'
 
 
 def test_extract_info_len3_3():
     info =['Directed by Agnès Varda • 1970 • United States', 'Agnès Varda turns her camera on an Oakland demonstration against the imprisonment of activist and Black Panthers cofounder Huey P. Newton. In addition to evincing Varda’s fascination with her adopted surroundings and her empathy, this perceptive short is also a powerful political statement.', 'Restored by the Cineteca di Bologna at L’Immagine Ritrovata in association with Ciné-Tamaris and The Film Foundation. Restoration funding provided by the Annenberg Foundation, the Los Angeles County Museum of Art (LACMA) and The Film Foundation.']
-    country, descr, director, stars, year = CriterionMovieParse.extract_info_len3(info)
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
     assert country == ' United States'
     assert descr =='Agnès Varda turns her camera on an Oakland demonstration against the imprisonment of activist and Black Panthers cofounder Huey P. Newton. In addition to evincing Varda’s fascination with her adopted surroundings and her empathy, this perceptive short is also a powerful political statement.' + "\n\n" + 'Restored by the Cineteca di Bologna at L’Immagine Ritrovata in association with Ciné-Tamaris and The Film Foundation. Restoration funding provided by the Annenberg Foundation, the Los Angeles County Museum of Art (LACMA) and The Film Foundation.'
     assert director =='Directed by Agnès Varda '
     assert stars == ''
-    assert year == '1970'
+    assert year.strip() == '1970'
 
 
 def test_extract_info_len2():
     info = ['Directed by Joel Coen and Ethan Coen • 1984 • United States', "Joel and Ethan Coen's career-long darkly comic road trip through misfit America began with this razor-sharp, hard-boiled neonoir set somewhere in Texas, where a sleazy bar owner releases a torrent of violence with one murderous thought. Actor M. Emmet Walsh looms over the proceedings as a slippery private eye with a yellow suit, a cowboy hat, and no moral compass, and Frances McDormand's cunning debut performance set her on the road to stardom. The tight scripting and inventive style that have marked the Coens' work for decades are all here in their first film, in which cinematographer Barry Sonnenfeld abandons black-and-white chiaroscuro for neon signs and jukebox colors that combine with Carter Burwell's haunting score to lurid and thrilling effect. Blending elements from pulp fiction and low-budget horror flicks, BLOOD SIMPLE reinvented the film noir for a new generation, marking the arrival of a filmmaking ensemble that would transform the American independent cinema scene."]
-    country, descr, director, year = CriterionMovieParse.extract_info_len2(info)
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
     assert country == ' United States'
     assert descr == "Joel and Ethan Coen's career-long darkly comic road trip through misfit America began with this razor-sharp, hard-boiled neonoir set somewhere in Texas, where a sleazy bar owner releases a torrent of violence with one murderous thought. Actor M. Emmet Walsh looms over the proceedings as a slippery private eye with a yellow suit, a cowboy hat, and no moral compass, and Frances McDormand's cunning debut performance set her on the road to stardom. The tight scripting and inventive style that have marked the Coens' work for decades are all here in their first film, in which cinematographer Barry Sonnenfeld abandons black-and-white chiaroscuro for neon signs and jukebox colors that combine with Carter Burwell's haunting score to lurid and thrilling effect. Blending elements from pulp fiction and low-budget horror flicks, BLOOD SIMPLE reinvented the film noir for a new generation, marking the arrival of a filmmaking ensemble that would transform the American independent cinema scene."
     assert director == 'Directed by Joel Coen and Ethan Coen '
-    assert year == ' 1984 '
+    assert year.strip() == '1984'
+
+
+def test_parse_info_breathless_fix():
+    info = ['Directed by Joel Coen and Ethan Coen • United States • 2018', "Joel and Ethan Coen's career-long darkly comic road trip through misfit America began with this razor-sharp, hard-boiled neonoir set somewhere in Texas, where a sleazy bar owner releases a torrent of violence with one murderous thought. Actor M. Emmet Walsh looms over the proceedings as a slippery private eye with a yellow suit, a cowboy hat, and no moral compass, and Frances McDormand's cunning debut performance set her on the road to stardom. The tight scripting and inventive style that have marked the Coens' work for decades are all here in their first film, in which cinematographer Barry Sonnenfeld abandons black-and-white chiaroscuro for neon signs and jukebox colors that combine with Carter Burwell's haunting score to lurid and thrilling effect. Blending elements from pulp fiction and low-budget horror flicks, BLOOD SIMPLE reinvented the film noir for a new generation, marking the arrival of a filmmaking ensemble that would transform the American independent cinema scene."]
+    country, descr, director, stars, year = CriterionMovieParse.parse_info(info)
+    assert country.strip() == 'United States'
+    assert descr == "Joel and Ethan Coen's career-long darkly comic road trip through misfit America began with this razor-sharp, hard-boiled neonoir set somewhere in Texas, where a sleazy bar owner releases a torrent of violence with one murderous thought. Actor M. Emmet Walsh looms over the proceedings as a slippery private eye with a yellow suit, a cowboy hat, and no moral compass, and Frances McDormand's cunning debut performance set her on the road to stardom. The tight scripting and inventive style that have marked the Coens' work for decades are all here in their first film, in which cinematographer Barry Sonnenfeld abandons black-and-white chiaroscuro for neon signs and jukebox colors that combine with Carter Burwell's haunting score to lurid and thrilling effect. Blending elements from pulp fiction and low-budget horror flicks, BLOOD SIMPLE reinvented the film noir for a new generation, marking the arrival of a filmmaking ensemble that would transform the American independent cinema scene."
+    assert director == 'Directed by Joel Coen and Ethan Coen '
+    assert year.strip() == '2018'
 
 
 def test_sanitize_data():
     country = ' United States'
     director = 'Directed by Joel Coen and Ethan Coen '
     length = 'Blood Simple\n' + '•\n' + '1h 35m'
     stars = ""
```

### Comparing `criterion-site-parser-1.7/src/testcritparse/test_CriterionParser.py` & `criterion_site_parser-1.8/src/testcritparse/test_CriterionParser.py`

 * *Files identical despite different names*

