# Comparing `tmp/huscy.project_design-0.3.3a12.tar.gz` & `tmp/huscy.project_design-0.4.0b13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_design-0.3.3a12.tar", last modified: Fri Feb 23 13:38:19 2024, max compression
+gzip compressed data, was "huscy.project_design-0.4.0b13.tar", last modified: Mon May 27 10:26:37 2024, max compression
```

## Comparing `huscy.project_design-0.3.3a12.tar` & `huscy.project_design-0.4.0b13.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.3.3a12/README.md
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-02-23 13:38:19.517124 huscy.project_design-0.3.3a12/huscy/
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/huscy/project_design/
--rw-r--r--   0 jenkins    (111) jenkins    (115)      167 2024-02-23 12:48:40.000000 huscy.project_design-0.3.3a12/huscy/project_design/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.3.3a12/huscy/project_design/admin.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.3.3a12/huscy/project_design/apps.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/huscy/project_design/migrations/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     3755 2024-02-23 13:38:18.000000 huscy.project_design-0.3.3a12/huscy/project_design/migrations/0001_initial.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.3.3a12/huscy/project_design/migrations/__init__.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2571 2024-02-23 10:51:00.000000 huscy.project_design-0.3.3a12/huscy/project_design/models.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2277 2023-08-03 12:41:53.000000 huscy.project_design-0.3.3a12/huscy/project_design/serializer.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2621 2024-02-23 12:48:40.000000 huscy.project_design-0.3.3a12/huscy/project_design/services.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)      847 2023-09-08 08:27:43.000000 huscy.project_design-0.3.3a12/huscy/project_design/urls.py
--rw-r--r--   0 jenkins    (111) jenkins    (115)     2302 2023-08-03 12:41:53.000000 huscy.project_design-0.3.3a12/huscy/project_design/views.py
-drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-02-23 13:38:19.000000 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (111) jenkins    (115)      579 2024-02-23 13:38:19.000000 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-02-23 13:38:19.000000 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       75 2024-02-23 13:38:19.000000 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/requires.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-02-23 13:38:19.000000 huscy.project_design-0.3.3a12/huscy.project_design.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-02-23 13:38:19.521124 huscy.project_design-0.3.3a12/setup.cfg
--rw-r--r--   0 jenkins    (111) jenkins    (115)     1548 2023-04-17 10:46:38.000000 huscy.project_design-0.3.3a12/setup.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       23 2021-10-25 14:34:42.000000 huscy.project_design-0.4.0b13/README.md
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/huscy/
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/huscy/project_design/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      166 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b13/huscy/project_design/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      151 2021-10-25 14:42:47.000000 huscy.project_design-0.4.0b13/huscy/project_design/admin.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      192 2022-06-23 17:20:37.000000 huscy.project_design-0.4.0b13/huscy/project_design/apps.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/huscy/project_design/migrations/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3755 2024-05-27 10:26:36.000000 huscy.project_design-0.4.0b13/huscy/project_design/migrations/0001_initial.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        0 2021-10-25 14:49:16.000000 huscy.project_design-0.4.0b13/huscy/project_design/migrations/__init__.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2571 2024-02-23 10:51:00.000000 huscy.project_design-0.4.0b13/huscy/project_design/models.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     3054 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b13/huscy/project_design/serializer.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2962 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b13/huscy/project_design/services.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      847 2023-09-08 08:27:43.000000 huscy.project_design-0.4.0b13/huscy/project_design/urls.py
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     2591 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b13/huscy/project_design/views.py
+drwxr-xr-x   0 jenkins    (111) jenkins    (115)        0 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1055 2024-05-27 10:26:36.000000 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (111) jenkins    (115)      579 2024-05-27 10:26:37.000000 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        1 2024-05-27 10:26:36.000000 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       70 2024-05-27 10:26:36.000000 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)        6 2024-05-27 10:26:36.000000 huscy.project_design-0.4.0b13/huscy.project_design.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (111) jenkins    (115)       38 2024-05-27 10:26:37.098806 huscy.project_design-0.4.0b13/setup.cfg
+-rw-r--r--   0 jenkins    (111) jenkins    (115)     1508 2024-05-27 09:33:00.000000 huscy.project_design-0.4.0b13/setup.py
```

### Comparing `huscy.project_design-0.3.3a12/PKG-INFO` & `huscy.project_design-0.4.0b13/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_design
-Version: 0.3.3a12
+Version: 0.4.0b13
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.project_design
```

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/migrations/0001_initial.py` & `huscy.project_design-0.4.0b13/huscy/project_design/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/models.py` & `huscy.project_design-0.4.0b13/huscy/project_design/models.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/serializer.py` & `huscy.project_design-0.4.0b13/huscy/project_design/serializer.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,49 +28,79 @@
 
     def update(self, data_acquisition_method, validated_data):
         return services.update_data_acquisition_method(data_acquisition_method, **validated_data)
 
 
 class SessionSerializer(serializers.ModelSerializer):
     data_acquisition_methods = DataAcquisitionMethodSerializer(many=True, read_only=True)
-    title = serializers.CharField(required=False)
 
     class Meta:
         model = models.Session
         fields = (
             'id',
             'data_acquisition_methods',
             'duration',
             'experiment',
             'order',
             'title',
         )
         read_only_fields = 'id', 'experiment', 'order'
 
+    def update(self, session, validated_data):
+        return services.update_session(session, **validated_data)
+
+
+class CreateSessionSerializer(serializers.ModelSerializer):
+    data_acquisition_method_types = serializers.ListField(required=False)
+    title = serializers.CharField(required=False)
+
+    class Meta:
+        model = models.Session
+        fields = (
+            'data_acquisition_method_types',
+            'duration',
+            'title',
+        )
+
     def create(self, validated_data):
         return services.create_session(**validated_data)
 
-    def update(self, session, validated_data):
-        return services.update_session(session, **validated_data)
+    def to_representation(self, session):
+        return SessionSerializer(instance=session).data
 
 
 class ExperimentSerializer(serializers.ModelSerializer):
     sessions = SessionSerializer(many=True, read_only=True)
-    title = serializers.CharField(required=False)
 
     class Meta:
         model = models.Experiment
         fields = (
             'id',
             'description',
             'order',
             'project',
             'sessions',
             'title',
         )
-        read_only_fields = 'id', 'order', 'project',
+        read_only_fields = 'id', 'project'
+
+    def update(self, experiment, validated_data):
+        return services.update_experiment(experiment, **validated_data)
+
+
+class CreateExperimentSerializer(serializers.ModelSerializer):
+    sessions = SessionSerializer(many=True, required=False)
+    title = serializers.CharField(required=False)
+
+    class Meta:
+        model = models.Experiment
+        fields = (
+            'description',
+            'sessions',
+            'title',
+        )
 
     def create(self, validated_data):
         return services.create_experiment(**validated_data)
 
-    def update(self, experiment, validated_data):
-        return services.update_experiment(experiment, **validated_data)
+    def to_representation(self, experiment):
+        return ExperimentSerializer(instance=experiment).data
```

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/services.py` & `huscy.project_design-0.4.0b13/huscy/project_design/services.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from . import models
 from huscy.project_design.models import DataAcquisitionMethod, Experiment, Session
 
 
-def create_experiment(project, title='', description=''):
+def create_experiment(project, description='', sessions=[], title=''):
     order = project.experiments.count()
 
-    return Experiment.objects.create(
+    experiment = Experiment.objects.create(
         description=description,
         order=order,
         project=project,
         title=title or f'Experiment {order + 1}',
     )
 
+    for session in sessions:
+        create_session(experiment, **session)
 
-def create_session(experiment, duration, title=''):
+    return experiment
+
+
+def create_session(experiment, duration, data_acquisition_method_types=[], title=''):
     order = experiment.sessions.count()
 
-    return Session.objects.create(
+    session = Session.objects.create(
         duration=duration,
         experiment=experiment,
         order=order,
         title=title or f'Session {order + 1}',
     )
 
+    for data_acquisition_method_type in data_acquisition_method_types:
+        create_data_acquisition_method(session, data_acquisition_method_type)
+
+    return session
+
 
-def create_data_acquisition_method(session, type, location, stimulus=None):
-    order = session.data_acquisition_methods.count() + 1
+def create_data_acquisition_method(session, type, location='', stimulus=None):
+    order = session.data_acquisition_methods.count()
 
     if isinstance(type, models.DataAcquisitionMethodType):
         pass
     elif isinstance(type, str):
         type = models.DataAcquisitionMethodType.objects.get(pk=type)
     else:
         raise ValueError('Unknown data type for `type` attribute')
@@ -58,14 +68,15 @@
 def get_data_acquisition_method_type(short_name):
     return models.DataAcquisitionMethodType.objects.get(short_name=short_name)
 
 
 def update_experiment(experiment, **kwargs):
     updatable_fields = (
         'description',
+        'order',
         'title',
     )
     return update(experiment, updatable_fields, **kwargs)
 
 
 def update_session(session, **kwargs):
     updatable_fields = (
```

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/urls.py` & `huscy.project_design-0.4.0b13/huscy/project_design/urls.py`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.3a12/huscy/project_design/views.py` & `huscy.project_design-0.4.0b13/huscy/project_design/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,42 +4,52 @@
 
 from huscy.project_design import models, serializer, services
 from huscy.projects.models import Project
 
 
 class ExperimentViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin, mixins.ListModelMixin,
                         mixins.UpdateModelMixin, viewsets.GenericViewSet):
-    serializer_class = serializer.ExperimentSerializer
     permission_classes = (IsAuthenticated, )
 
     def initial(self, request, *args, **kwargs):
         self.project = get_object_or_404(Project, pk=self.kwargs['project_pk'])
         super().initial(request, *args, **kwargs)
 
     def get_queryset(self):
         return services.get_experiments(self.project)
 
+    def get_serializer_class(self):
+        if self.request.method == 'POST':
+            return serializer.CreateExperimentSerializer
+        else:
+            return serializer.ExperimentSerializer
+
     def perform_create(self, serializer):
         serializer.save(project=self.project)
 
 
 class SessionViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin, mixins.UpdateModelMixin,
                      viewsets.GenericViewSet):
     queryset = models.Session.objects.all()
     permission_classes = (IsAuthenticated, )
-    serializer_class = serializer.SessionSerializer
 
     def initial(self, request, *args, **kwargs):
         self.experiment = get_object_or_404(
             models.Experiment,
             pk=self.kwargs['experiment_pk'],
             project=self.kwargs['project_pk']
         )
         super().initial(request, *args, **kwargs)
 
+    def get_serializer_class(self):
+        if self.request.method == 'POST':
+            return serializer.CreateSessionSerializer
+        else:
+            return serializer.SessionSerializer
+
     def perform_create(self, serializer):
         serializer.save(experiment=self.experiment)
 
 
 class DataAcquisitionMethodViewSet(mixins.CreateModelMixin, mixins.DestroyModelMixin,
                                    mixins.UpdateModelMixin, viewsets.GenericViewSet):
     queryset = models.DataAcquisitionMethod.objects.all()
```

### Comparing `huscy.project_design-0.3.3a12/huscy.project_design.egg-info/PKG-INFO` & `huscy.project_design-0.4.0b13/huscy.project_design.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-design
-Version: 0.3.3a12
+Version: 0.4.0b13
 Summary: UNKNOWN
 Home-page: https://bitbucket.org/huscy/project_design
 Author: Stefan Bunde
 Author-email: stefanbunde+git@posteo.de
 License: AGPLv3+
 Description: # huscy.project_design
```

### Comparing `huscy.project_design-0.3.3a12/huscy.project_design.egg-info/SOURCES.txt` & `huscy.project_design-0.4.0b13/huscy.project_design.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `huscy.project_design-0.3.3a12/setup.py` & `huscy.project_design-0.4.0b13/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,18 +26,15 @@
     packages=find_namespace_packages(include=['huscy.*']),
 
     install_requires=[
         'huscy.projects',
     ],
     extras_require={
         'development': ['psycopg2-binary'],
-        'testing': [
-            'tox',
-            'watchdog==0.9',
-        ],
+        'testing': ['tox', 'watchdog'],
     },
 
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

