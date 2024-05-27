# Comparing `tmp/django_global_places-0.8.5.tar.gz` & `tmp/django_global_places-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_global_places-0.8.5.tar", last modified: Wed May 22 14:45:17 2024, max compression
+gzip compressed data, was "django_global_places-0.8.6.tar", last modified: Mon May 27 10:38:13 2024, max compression
```

## Comparing `django_global_places-0.8.5.tar` & `django_global_places-0.8.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.325307 django_global_places-0.8.5/
--rw-rw-rw-   0        0        0       63 2024-03-30 19:07:36.000000 django_global_places-0.8.5/AUTHORS
--rw-rw-rw-   0        0        0     1137 2024-03-30 19:22:19.000000 django_global_places-0.8.5/LICENSE
--rw-rw-rw-   0        0        0     4009 2024-05-22 14:45:17.324293 django_global_places-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     3347 2024-03-30 19:07:36.000000 django_global_places-0.8.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.267869 django_global_places-0.8.5/django_global_places/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/__init__.py
--rw-rw-rw-   0        0        0      429 2024-05-22 13:46:18.000000 django_global_places-0.8.5/django_global_places/__version__.py
--rw-rw-rw-   0        0        0     2157 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/abstract_models.py
--rw-rw-rw-   0        0        0     1217 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/admin.py
--rw-rw-rw-   0        0        0     1175 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/app_settings.py
--rw-rw-rw-   0        0        0      219 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/apps.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.304449 django_global_places-0.8.5/django_global_places/management/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.306708 django_global_places-0.8.5/django_global_places/management/commands/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/commands/__init__.py
--rw-rw-rw-   0        0        0    12320 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/management/commands/populate_global_places.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.310707 django_global_places-0.8.5/django_global_places/migrations/
--rw-rw-rw-   0        0        0     5205 2024-05-22 14:43:55.000000 django_global_places-0.8.5/django_global_places/migrations/0001_initial.py
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/migrations/__init__.py
--rw-rw-rw-   0        0        0      739 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/models.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.316235 django_global_places-0.8.5/django_global_places/serializers/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/__init__.py
--rw-rw-rw-   0        0        0      676 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/cities.py
--rw-rw-rw-   0        0        0      617 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/countries.py
--rw-rw-rw-   0        0        0      702 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/serializers/states.py
--rw-rw-rw-   0        0        0      711 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/urls.py
--rw-rw-rw-   0        0        0      662 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.322778 django_global_places-0.8.5/django_global_places/views/
--rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/__init__.py
--rw-rw-rw-   0        0        0     1438 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/cities.py
--rw-rw-rw-   0        0        0      999 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/countries.py
--rw-rw-rw-   0        0        0     1412 2024-03-30 19:07:36.000000 django_global_places-0.8.5/django_global_places/views/states.py
--rw-rw-rw-   0        0        0      859 2024-03-30 19:10:41.000000 django_global_places-0.8.5/django_global_places/viewsets_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 14:45:17.302448 django_global_places-0.8.5/django_global_places.egg-info/
--rw-rw-rw-   0        0        0     4009 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1216 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 09:18:17.000000 django_global_places-0.8.5/django_global_places.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2024-05-22 14:45:17.000000 django_global_places-0.8.5/django_global_places.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 14:45:17.326308 django_global_places-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1202 2024-03-30 19:07:36.000000 django_global_places-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.880891 django_global_places-0.8.6/
+-rw-rw-rw-   0        0        0       63 2024-03-30 19:07:36.000000 django_global_places-0.8.6/AUTHORS
+-rw-rw-rw-   0        0        0     1137 2024-03-30 19:22:19.000000 django_global_places-0.8.6/LICENSE
+-rw-rw-rw-   0        0        0     4009 2024-05-27 10:38:13.880891 django_global_places-0.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3347 2024-03-30 19:07:36.000000 django_global_places-0.8.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.754434 django_global_places-0.8.6/django_global_places/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/__init__.py
+-rw-rw-rw-   0        0        0      429 2024-05-27 10:38:08.000000 django_global_places-0.8.6/django_global_places/__version__.py
+-rw-rw-rw-   0        0        0     2157 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/abstract_models.py
+-rw-rw-rw-   0        0        0     1217 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/admin.py
+-rw-rw-rw-   0        0        0     1175 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/app_settings.py
+-rw-rw-rw-   0        0        0      219 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/apps.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.787512 django_global_places-0.8.6/django_global_places/management/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.792522 django_global_places-0.8.6/django_global_places/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/management/commands/__init__.py
+-rw-rw-rw-   0        0        0    12423 2024-05-27 10:36:56.000000 django_global_places-0.8.6/django_global_places/management/commands/populate_global_places.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.808602 django_global_places-0.8.6/django_global_places/migrations/
+-rw-rw-rw-   0        0        0     5205 2024-05-22 14:43:55.000000 django_global_places-0.8.6/django_global_places/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/migrations/__init__.py
+-rw-rw-rw-   0        0        0      739 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/models.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.844256 django_global_places-0.8.6/django_global_places/serializers/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/serializers/__init__.py
+-rw-rw-rw-   0        0        0      676 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/serializers/cities.py
+-rw-rw-rw-   0        0        0      617 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/serializers/countries.py
+-rw-rw-rw-   0        0        0      702 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/serializers/states.py
+-rw-rw-rw-   0        0        0      711 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/urls.py
+-rw-rw-rw-   0        0        0      662 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.878877 django_global_places-0.8.6/django_global_places/views/
+-rw-rw-rw-   0        0        0        0 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/views/__init__.py
+-rw-rw-rw-   0        0        0     1438 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/views/cities.py
+-rw-rw-rw-   0        0        0      999 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/views/countries.py
+-rw-rw-rw-   0        0        0     1412 2024-03-30 19:07:36.000000 django_global_places-0.8.6/django_global_places/views/states.py
+-rw-rw-rw-   0        0        0      859 2024-03-30 19:10:41.000000 django_global_places-0.8.6/django_global_places/viewsets_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 10:38:13.786008 django_global_places-0.8.6/django_global_places.egg-info/
+-rw-rw-rw-   0        0        0     4009 2024-05-27 10:38:13.000000 django_global_places-0.8.6/django_global_places.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1216 2024-05-27 10:38:13.000000 django_global_places-0.8.6/django_global_places.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 10:38:13.000000 django_global_places-0.8.6/django_global_places.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-06 09:18:17.000000 django_global_places-0.8.6/django_global_places.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2024-05-27 10:38:13.000000 django_global_places-0.8.6/django_global_places.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2024-05-27 10:38:13.000000 django_global_places-0.8.6/django_global_places.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 10:38:13.881888 django_global_places-0.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1202 2024-03-30 19:07:36.000000 django_global_places-0.8.6/setup.py
```

### Comparing `django_global_places-0.8.5/LICENSE` & `django_global_places-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/PKG-INFO` & `django_global_places-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_global_places
-Version: 0.8.5
+Version: 0.8.6
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
```

### Comparing `django_global_places-0.8.5/README.md` & `django_global_places-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/abstract_models.py` & `django_global_places-0.8.6/django_global_places/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/admin.py` & `django_global_places-0.8.6/django_global_places/admin.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/app_settings.py` & `django_global_places-0.8.6/django_global_places/app_settings.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/management/commands/populate_global_places.py` & `django_global_places-0.8.6/django_global_places/management/commands/populate_global_places.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 from django_global_places.app_settings import api_settings as settings
 from django_global_places import models 
 
 
 class Command(BaseCommand):
     """Django command to populate location models."""
 
-    base_data_url = 'https://raw.githubusercontent.com/dr5hn/countries-states-cities-database/master/'
-
     data_uls = {
-        'country':f'{base_data_url}/countries.json',
-        'state':f'{base_data_url}/countries+states.json',
-        'city':f'{base_data_url}/countries+states+cities.json'
+        'country':f'/countries.json',
+        'state':f'/countries+states.json',
+        'city':f'/countries+states+cities.json'
     }
 
     model_creator = {
         'country': '_create_country_object',    
         'state': '_create_state_object',
         'city': '_create_city_object'
     }
@@ -63,18 +61,22 @@
         if settings.get_user_setting('LOCATION_SCOPE') == 'city' \
         else 0
 
     country_extra_pos = (1 \
                         if settings.get_user_setting('LOCATION_SCOPE') == 'country' \
                         else 0) + extra_pos
 
+    def _get_base_data_urls(self):
+        self.base_data_url = 'https://raw.githubusercontent.com/dr5hn/countries-states-cities-database/master/'
+        self.buenos_aires_data_url = 'https://apis.datos.gob.ar/georef/api/municipios?provincia=06&max=999'
+
     def _get_data_url(self):
         if not settings.get_user_setting('INCLUDE_LOCATION'):
             raise Exception('The "INCLUDE_LOCATION" setting must be True to populate location models')
-        return self.data_uls[settings.get_user_setting('LOCATION_SCOPE')]
+        return self.base_data_url + self.data_uls[settings.get_user_setting('LOCATION_SCOPE')]
 
     def _get_data(self):
         response = requests.get(self._get_data_url())
         if response.status_code != 200:
             raise Exception('Error getting data from url')
         data = pd.read_json(StringIO(response.text))
         return data
@@ -149,16 +151,15 @@
         )
 
     def _add_to_create_list(self, model, item, items_to_create, parent=None):
         item_creator = getattr(self, self.model_creator[model])
         items_to_create.append(item_creator(item, parent))
 
     def _get_buenos_aires_cities(self):
-        url = 'https://apis.datos.gob.ar/georef/api/municipios?provincia=06&max=999'
-        response = requests.get(url)
+        response = requests.get(self.buenos_aires_data_url)
         if response.status_code != 200:
             raise Exception('Error getting data from url')
         response = json.loads(response.text)
         data = pd.DataFrame.from_dict(response['municipios'])
         cities = []
         for city in data.values:
             cities.append(
@@ -168,14 +169,15 @@
                     'latitude':city[0]['lat'],
                     'longitude':city[0]['lon']
                 }
             )
         return cities
 
     def handle(self, *args, **options):
+        self._get_base_data_urls()
         st = time.time()
         """Handle the command."""
         data = self._get_data()
 
         all_countries = self._get_all_countries()
         all_countries_names = all_countries.values_list('name', flat=True)
         counties_to_create = []
```

### Comparing `django_global_places-0.8.5/django_global_places/migrations/0001_initial.py` & `django_global_places-0.8.6/django_global_places/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/models.py` & `django_global_places-0.8.6/django_global_places/models.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/serializers/cities.py` & `django_global_places-0.8.6/django_global_places/serializers/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/serializers/countries.py` & `django_global_places-0.8.6/django_global_places/serializers/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/serializers/states.py` & `django_global_places-0.8.6/django_global_places/serializers/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/urls.py` & `django_global_places-0.8.6/django_global_places/urls.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/utils.py` & `django_global_places-0.8.6/django_global_places/utils.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/views/cities.py` & `django_global_places-0.8.6/django_global_places/views/cities.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/views/countries.py` & `django_global_places-0.8.6/django_global_places/views/countries.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/views/states.py` & `django_global_places-0.8.6/django_global_places/views/states.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places/viewsets_utils.py` & `django_global_places-0.8.6/django_global_places/viewsets_utils.py`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/django_global_places.egg-info/PKG-INFO` & `django_global_places-0.8.6/django_global_places.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-global-places
-Version: 0.8.5
+Version: 0.8.6
 Summary: Django Global Places is a simple Django app to provide a model for global places.
 Home-page: https://github.com/lucacitta/Django-GlobalPlaces
 Author: lucacitta
 Author-email: lucacitta.dev@gmail.com
 License: MIT
 Keywords: django global places
 Classifier: Framework :: Django
```

### Comparing `django_global_places-0.8.5/django_global_places.egg-info/SOURCES.txt` & `django_global_places-0.8.6/django_global_places.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_global_places-0.8.5/setup.py` & `django_global_places-0.8.6/setup.py`

 * *Files identical despite different names*

