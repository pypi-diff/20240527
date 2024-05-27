# Comparing `tmp/nokey-0.7.0.tar.gz` & `tmp/nokey-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nokey-0.7.0.tar", max compression
+gzip compressed data, was "nokey-0.7.1.tar", max compression
```

## Comparing `nokey-0.7.0.tar` & `nokey-0.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.7.0/LICENSE
--rw-r--r--   0        0        0     3407 2024-05-25 13:37:22.426835 nokey-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.0/nokey/__init__.py
--rw-r--r--   0        0        0     5358 2024-05-25 13:32:20.882835 nokey-0.7.0/nokey/activities/bored_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.010835 nokey-0.7.0/nokey/animals/__init__.py
--rw-r--r--   0        0        0     2991 2024-05-25 13:32:21.014835 nokey-0.7.0/nokey/animals/dog_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.130835 nokey-0.7.0/nokey/art_and_images/__init__.py
--rw-r--r--   0        0        0    93276 2024-05-25 13:32:21.126835 nokey-0.7.0/nokey/art_and_images/artic.py
--rw-r--r--   0        0        0     8014 2024-05-25 13:32:21.134835 nokey-0.7.0/nokey/art_and_images/lorem_picsum.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.118835 nokey-0.7.0/nokey/books_and_literature/__init__.py
--rw-r--r--   0        0        0     6320 2024-05-25 13:32:21.122835 nokey-0.7.0/nokey/books_and_literature/gutendex.py
--rw-r--r--   0        0        0     3495 2024-05-25 13:32:21.106835 nokey-0.7.0/nokey/books_and_literature/stephen_king.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.898835 nokey-0.7.0/nokey/calendar/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-25 13:32:20.894835 nokey-0.7.0/nokey/calendar/nager_date.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.978835 nokey-0.7.0/nokey/country_info/__init__.py
--rw-r--r--   0        0        0     4985 2024-05-25 13:32:20.978835 nokey-0.7.0/nokey/country_info/rest_country.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.162835 nokey-0.7.0/nokey/developer_tools/__init__.py
--rw-r--r--   0        0        0     4187 2024-05-25 13:32:21.158835 nokey-0.7.0/nokey/developer_tools/apis_guru.py
--rw-r--r--   0        0        0     3809 2024-05-25 13:32:21.150835 nokey-0.7.0/nokey/developer_tools/filter_lists.py
--rw-r--r--   0        0        0     2862 2024-05-25 13:32:21.154835 nokey-0.7.0/nokey/developer_tools/microlink.py
--rw-r--r--   0        0        0     7552 2024-05-25 13:32:21.166835 nokey-0.7.0/nokey/developer_tools/url_haus.py
--rw-r--r--   0        0        0     1964 2024-05-25 13:32:21.162835 nokey-0.7.0/nokey/developer_tools/url_shortener.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.966835 nokey-0.7.0/nokey/education/__init__.py
--rw-r--r--   0        0        0     2591 2024-05-25 13:32:20.970835 nokey-0.7.0/nokey/education/university_domains_and_names.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.042835 nokey-0.7.0/nokey/finance_and_crypto/__init__.py
--rw-r--r--   0        0        0     6117 2024-05-25 13:32:21.050835 nokey-0.7.0/nokey/finance_and_crypto/coinmap.py
--rw-r--r--   0        0        0     2758 2024-05-25 13:32:21.046835 nokey-0.7.0/nokey/finance_and_crypto/exchange_api.py
--rw-r--r--   0        0        0     1382 2024-05-25 13:32:21.054835 nokey-0.7.0/nokey/finance_and_crypto/wallstreet_bets.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.090835 nokey-0.7.0/nokey/food/__init__.py
--rw-r--r--   0        0        0     3441 2024-05-25 13:32:21.094835 nokey-0.7.0/nokey/food/fruityvice.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.082835 nokey-0.7.0/nokey/games/__init__.py
--rw-r--r--   0        0        0     6785 2024-05-25 13:32:21.082835 nokey-0.7.0/nokey/games/free_to_game.py
--rw-r--r--   0        0        0     5626 2024-05-25 13:32:21.074835 nokey-0.7.0/nokey/games/open_trivia_db.py
--rw-r--r--   0        0        0    30480 2024-05-25 13:32:21.078835 nokey-0.7.0/nokey/games/shadify.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.866835 nokey-0.7.0/nokey/geolocation/__init__.py
--rw-r--r--   0        0        0     1377 2024-05-25 13:32:20.862835 nokey-0.7.0/nokey/geolocation/ip_api.py
--rw-r--r--   0        0        0     2119 2024-05-25 13:32:20.866835 nokey-0.7.0/nokey/geolocation/zippopotamus.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.062835 nokey-0.7.0/nokey/government/__init__.py
--rw-r--r--   0        0        0    10908 2024-05-25 13:32:21.062835 nokey-0.7.0/nokey/government/federal_register.py
--rw-r--r--   0        0        0   157578 2024-05-25 13:32:21.066835 nokey-0.7.0/nokey/government/usa_spending.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.906835 nokey-0.7.0/nokey/health/__init__.py
--rw-r--r--   0        0        0    32273 2024-05-25 13:32:20.906835 nokey-0.7.0/nokey/health/open_disease.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.926835 nokey-0.7.0/nokey/helperFuncs/__init__.py
--rw-r--r--   0        0        0      822 2024-05-25 13:32:20.930835 nokey-0.7.0/nokey/helperFuncs/get_api_list.py
--rw-r--r--   0        0        0     6851 2024-05-25 13:32:20.926835 nokey-0.7.0/nokey/helperFuncs/make_request.py
--rw-r--r--   0        0        0     1076 2024-05-25 13:32:20.934835 nokey-0.7.0/nokey/helperFuncs/nokey_apis.py
--rw-r--r--   0        0        0     1514 2024-05-25 13:32:20.962835 nokey-0.7.0/nokey/helperFuncs/throttler.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.838835 nokey-0.7.0/nokey/inspiration/__init__.py
--rw-r--r--   0        0        0     6164 2024-05-25 13:32:20.834835 nokey-0.7.0/nokey/inspiration/dictum.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.038835 nokey-0.7.0/nokey/jokes/__init__.py
--rw-r--r--   0        0        0     3342 2024-05-25 13:32:21.034835 nokey-0.7.0/nokey/jokes/joke_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.006835 nokey-0.7.0/nokey/language/__init__.py
--rw-r--r--   0        0        0     1433 2024-05-25 13:32:21.006835 nokey-0.7.0/nokey/language/free_dictionary.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.998835 nokey-0.7.0/nokey/random/__init__.py
--rw-r--r--   0        0        0     1363 2024-05-25 13:32:20.998835 nokey-0.7.0/nokey/random/random_user.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:21.182835 nokey-0.7.0/nokey/science_and_nature/__init__.py
--rw-r--r--   0        0        0    50832 2024-05-25 13:32:21.174835 nokey-0.7.0/nokey/science_and_nature/integrated_taxonomic_information_system.py
--rw-r--r--   0        0        0     3192 2024-05-25 13:32:21.178835 nokey-0.7.0/nokey/science_and_nature/nobel_prize.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.0/nokey/spaceflight/__init__.py
--rw-r--r--   0        0        0     9033 2024-05-25 13:32:20.986835 nokey-0.7.0/nokey/spaceflight/spaceflight_news.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.874835 nokey-0.7.0/nokey/tv_and_film/__init__.py
--rw-r--r--   0        0        0    43761 2024-05-25 13:32:20.878835 nokey-0.7.0/nokey/tv_and_film/star_trek_api.py
--rw-r--r--   0        0        0        0 2024-05-25 13:32:20.846835 nokey-0.7.0/nokey/weather/__init__.py
--rw-r--r--   0        0        0    26351 2024-05-25 13:32:20.842835 nokey-0.7.0/nokey/weather/national_weather_service.py
--rw-r--r--   0        0        0      711 2024-05-25 13:39:44.190835 nokey-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 nokey-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 23:28:41.225586 nokey-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3407 2024-05-25 13:37:22.426835 nokey-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.1/nokey/__init__.py
+-rw-r--r--   0        0        0     5359 2024-05-27 14:42:41.748021 nokey-0.7.1/nokey/activities/bored_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.010835 nokey-0.7.1/nokey/animals/__init__.py
+-rw-r--r--   0        0        0     2991 2024-05-27 14:42:17.448020 nokey-0.7.1/nokey/animals/dog_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.130835 nokey-0.7.1/nokey/art_and_images/__init__.py
+-rw-r--r--   0        0        0    93276 2024-05-25 13:32:21.126835 nokey-0.7.1/nokey/art_and_images/artic.py
+-rw-r--r--   0        0        0     8014 2024-05-25 13:32:21.134835 nokey-0.7.1/nokey/art_and_images/lorem_picsum.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.118835 nokey-0.7.1/nokey/books_and_literature/__init__.py
+-rw-r--r--   0        0        0     6320 2024-05-25 13:32:21.122835 nokey-0.7.1/nokey/books_and_literature/gutendex.py
+-rw-r--r--   0        0        0     3495 2024-05-25 13:32:21.106835 nokey-0.7.1/nokey/books_and_literature/stephen_king.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.898835 nokey-0.7.1/nokey/calendar/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-25 13:32:20.894835 nokey-0.7.1/nokey/calendar/nager_date.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.978835 nokey-0.7.1/nokey/country_info/__init__.py
+-rw-r--r--   0        0        0     4985 2024-05-25 13:32:20.978835 nokey-0.7.1/nokey/country_info/rest_country.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.162835 nokey-0.7.1/nokey/developer_tools/__init__.py
+-rw-r--r--   0        0        0     4187 2024-05-25 13:32:21.158835 nokey-0.7.1/nokey/developer_tools/apis_guru.py
+-rw-r--r--   0        0        0     3809 2024-05-25 13:32:21.150835 nokey-0.7.1/nokey/developer_tools/filter_lists.py
+-rw-r--r--   0        0        0     2862 2024-05-25 13:32:21.154835 nokey-0.7.1/nokey/developer_tools/microlink.py
+-rw-r--r--   0        0        0     7552 2024-05-25 13:32:21.166835 nokey-0.7.1/nokey/developer_tools/url_haus.py
+-rw-r--r--   0        0        0     1964 2024-05-25 13:32:21.162835 nokey-0.7.1/nokey/developer_tools/url_shortener.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.966835 nokey-0.7.1/nokey/education/__init__.py
+-rw-r--r--   0        0        0     2591 2024-05-25 13:32:20.970835 nokey-0.7.1/nokey/education/university_domains_and_names.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.042835 nokey-0.7.1/nokey/finance_and_crypto/__init__.py
+-rw-r--r--   0        0        0     6117 2024-05-25 13:32:21.050835 nokey-0.7.1/nokey/finance_and_crypto/coinmap.py
+-rw-r--r--   0        0        0     2758 2024-05-25 13:32:21.046835 nokey-0.7.1/nokey/finance_and_crypto/exchange_api.py
+-rw-r--r--   0        0        0     1382 2024-05-25 13:32:21.054835 nokey-0.7.1/nokey/finance_and_crypto/wallstreet_bets.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.090835 nokey-0.7.1/nokey/food/__init__.py
+-rw-r--r--   0        0        0     3441 2024-05-25 13:32:21.094835 nokey-0.7.1/nokey/food/fruityvice.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.082835 nokey-0.7.1/nokey/games/__init__.py
+-rw-r--r--   0        0        0     6785 2024-05-25 13:32:21.082835 nokey-0.7.1/nokey/games/free_to_game.py
+-rw-r--r--   0        0        0     5626 2024-05-25 13:32:21.074835 nokey-0.7.1/nokey/games/open_trivia_db.py
+-rw-r--r--   0        0        0    30480 2024-05-25 13:32:21.078835 nokey-0.7.1/nokey/games/shadify.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.866835 nokey-0.7.1/nokey/geolocation/__init__.py
+-rw-r--r--   0        0        0     1377 2024-05-25 13:32:20.862835 nokey-0.7.1/nokey/geolocation/ip_api.py
+-rw-r--r--   0        0        0     2119 2024-05-25 13:32:20.866835 nokey-0.7.1/nokey/geolocation/zippopotamus.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.062835 nokey-0.7.1/nokey/government/__init__.py
+-rw-r--r--   0        0        0    10908 2024-05-25 13:32:21.062835 nokey-0.7.1/nokey/government/federal_register.py
+-rw-r--r--   0        0        0   157578 2024-05-25 13:32:21.066835 nokey-0.7.1/nokey/government/usa_spending.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.906835 nokey-0.7.1/nokey/health/__init__.py
+-rw-r--r--   0        0        0    32273 2024-05-25 13:32:20.906835 nokey-0.7.1/nokey/health/open_disease.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.926835 nokey-0.7.1/nokey/helperFuncs/__init__.py
+-rw-r--r--   0        0        0      822 2024-05-25 13:32:20.930835 nokey-0.7.1/nokey/helperFuncs/get_api_list.py
+-rw-r--r--   0        0        0     6851 2024-05-25 13:32:20.926835 nokey-0.7.1/nokey/helperFuncs/make_request.py
+-rw-r--r--   0        0        0     1076 2024-05-25 13:32:20.934835 nokey-0.7.1/nokey/helperFuncs/nokey_apis.py
+-rw-r--r--   0        0        0     1514 2024-05-25 13:32:20.962835 nokey-0.7.1/nokey/helperFuncs/throttler.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.838835 nokey-0.7.1/nokey/inspiration/__init__.py
+-rw-r--r--   0        0        0     6164 2024-05-25 13:32:20.834835 nokey-0.7.1/nokey/inspiration/dictum.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.038835 nokey-0.7.1/nokey/jokes/__init__.py
+-rw-r--r--   0        0        0     3342 2024-05-25 13:32:21.034835 nokey-0.7.1/nokey/jokes/joke_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.006835 nokey-0.7.1/nokey/language/__init__.py
+-rw-r--r--   0        0        0     1433 2024-05-25 13:32:21.006835 nokey-0.7.1/nokey/language/free_dictionary.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.998835 nokey-0.7.1/nokey/random/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-25 13:32:20.998835 nokey-0.7.1/nokey/random/random_user.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:21.182835 nokey-0.7.1/nokey/science_and_nature/__init__.py
+-rw-r--r--   0        0        0    50832 2024-05-25 13:32:21.174835 nokey-0.7.1/nokey/science_and_nature/integrated_taxonomic_information_system.py
+-rw-r--r--   0        0        0     3192 2024-05-25 13:32:21.178835 nokey-0.7.1/nokey/science_and_nature/nobel_prize.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.990835 nokey-0.7.1/nokey/spaceflight/__init__.py
+-rw-r--r--   0        0        0     9033 2024-05-25 13:32:20.986835 nokey-0.7.1/nokey/spaceflight/spaceflight_news.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.874835 nokey-0.7.1/nokey/tv_and_film/__init__.py
+-rw-r--r--   0        0        0    43761 2024-05-25 13:32:20.878835 nokey-0.7.1/nokey/tv_and_film/star_trek_api.py
+-rw-r--r--   0        0        0        0 2024-05-25 13:32:20.846835 nokey-0.7.1/nokey/weather/__init__.py
+-rw-r--r--   0        0        0    26351 2024-05-25 13:32:20.842835 nokey-0.7.1/nokey/weather/national_weather_service.py
+-rw-r--r--   0        0        0      711 2024-05-27 14:47:00.236020 nokey-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     4323 1970-01-01 00:00:00.000000 nokey-0.7.1/PKG-INFO
```

### Comparing `nokey-0.7.0/LICENSE` & `nokey-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/README.md` & `nokey-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/activities/bored_api.py` & `nokey-0.7.1/nokey/activities/bored_api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -139,8 +139,8 @@
   
         
         
     
     
     
     
-        
+
```

### Comparing `nokey-0.7.0/nokey/animals/dog_api.py` & `nokey-0.7.1/nokey/animals/dog_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     - about: A short description of the API.
     """
     def __init__(self, use_caching=False, cache_name="dog_api_cache", backend="sqlite", expire_after=3600):
         self.base_url = "https://dog.ceo/api/"
         self.about = "The Dog API returns URLs for dog images, either at random or by breed."
         
         if use_caching:
-            requests_cache.install_cache(cache_name, baackend=backend, expire_after=expire_after)
+            requests_cache.install_cache(cache_name, backend=backend, expire_after=expire_after)
         
     def get_docs_url(self):
         """
         Returns the URL for the Dog API documentation.
         
         Args:
         - None
@@ -91,8 +91,8 @@
         - dict: Dictionary the URL for a random dog image of the specified breed.
         """
         endpoint = f"breed/{breed.lower()}/images/random"
         return mr.make_request(self.base_url+endpoint)
   
    
         
-    
+
```

### Comparing `nokey-0.7.0/nokey/art_and_images/artic.py` & `nokey-0.7.1/nokey/art_and_images/artic.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/art_and_images/lorem_picsum.py` & `nokey-0.7.1/nokey/art_and_images/lorem_picsum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/books_and_literature/gutendex.py` & `nokey-0.7.1/nokey/books_and_literature/gutendex.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/books_and_literature/stephen_king.py` & `nokey-0.7.1/nokey/books_and_literature/stephen_king.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/calendar/nager_date.py` & `nokey-0.7.1/nokey/calendar/nager_date.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/country_info/rest_country.py` & `nokey-0.7.1/nokey/country_info/rest_country.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/developer_tools/apis_guru.py` & `nokey-0.7.1/nokey/developer_tools/apis_guru.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/developer_tools/filter_lists.py` & `nokey-0.7.1/nokey/developer_tools/filter_lists.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/developer_tools/microlink.py` & `nokey-0.7.1/nokey/developer_tools/microlink.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/developer_tools/url_haus.py` & `nokey-0.7.1/nokey/developer_tools/url_haus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/developer_tools/url_shortener.py` & `nokey-0.7.1/nokey/developer_tools/url_shortener.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/education/university_domains_and_names.py` & `nokey-0.7.1/nokey/education/university_domains_and_names.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/finance_and_crypto/coinmap.py` & `nokey-0.7.1/nokey/finance_and_crypto/coinmap.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/finance_and_crypto/exchange_api.py` & `nokey-0.7.1/nokey/finance_and_crypto/exchange_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/finance_and_crypto/wallstreet_bets.py` & `nokey-0.7.1/nokey/finance_and_crypto/wallstreet_bets.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/food/fruityvice.py` & `nokey-0.7.1/nokey/food/fruityvice.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/games/free_to_game.py` & `nokey-0.7.1/nokey/games/free_to_game.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/games/open_trivia_db.py` & `nokey-0.7.1/nokey/games/open_trivia_db.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/games/shadify.py` & `nokey-0.7.1/nokey/games/shadify.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/geolocation/ip_api.py` & `nokey-0.7.1/nokey/geolocation/ip_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/geolocation/zippopotamus.py` & `nokey-0.7.1/nokey/geolocation/zippopotamus.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/government/federal_register.py` & `nokey-0.7.1/nokey/government/federal_register.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/government/usa_spending.py` & `nokey-0.7.1/nokey/government/usa_spending.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/health/open_disease.py` & `nokey-0.7.1/nokey/health/open_disease.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/helperFuncs/get_api_list.py` & `nokey-0.7.1/nokey/helperFuncs/get_api_list.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/helperFuncs/make_request.py` & `nokey-0.7.1/nokey/helperFuncs/make_request.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/helperFuncs/nokey_apis.py` & `nokey-0.7.1/nokey/helperFuncs/nokey_apis.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/helperFuncs/throttler.py` & `nokey-0.7.1/nokey/helperFuncs/throttler.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/inspiration/dictum.py` & `nokey-0.7.1/nokey/inspiration/dictum.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/jokes/joke_api.py` & `nokey-0.7.1/nokey/jokes/joke_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/language/free_dictionary.py` & `nokey-0.7.1/nokey/language/free_dictionary.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/random/random_user.py` & `nokey-0.7.1/nokey/random/random_user.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/science_and_nature/integrated_taxonomic_information_system.py` & `nokey-0.7.1/nokey/science_and_nature/integrated_taxonomic_information_system.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/science_and_nature/nobel_prize.py` & `nokey-0.7.1/nokey/science_and_nature/nobel_prize.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/spaceflight/spaceflight_news.py` & `nokey-0.7.1/nokey/spaceflight/spaceflight_news.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/tv_and_film/star_trek_api.py` & `nokey-0.7.1/nokey/tv_and_film/star_trek_api.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/nokey/weather/national_weather_service.py` & `nokey-0.7.1/nokey/weather/national_weather_service.py`

 * *Files identical despite different names*

### Comparing `nokey-0.7.0/pyproject.toml` & `nokey-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nokey"
-version = "0.7.0"
+version = "0.7.1"
 description = "A python package for accessing APIs that require no key."
 authors = ["Spyder Rex <billyjohnsonauthor@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/SpyderRex/nokey"
 repository = "https://github.com/SpyderRex/nokey"
 license = "MIT"
 keywords = ["API", "requests", "xmltodict"]
```

### Comparing `nokey-0.7.0/PKG-INFO` & `nokey-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nokey
-Version: 0.7.0
+Version: 0.7.1
 Summary: A python package for accessing APIs that require no key.
 Home-page: https://github.com/SpyderRex/nokey
 License: MIT
 Keywords: API,requests,xmltodict
 Author: Spyder Rex
 Author-email: billyjohnsonauthor@gmail.com
 Requires-Python: >=3.8,<4.0
```

