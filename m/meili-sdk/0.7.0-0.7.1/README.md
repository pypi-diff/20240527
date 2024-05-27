# Comparing `tmp/meili-sdk-0.7.0.tar.gz` & `tmp/meili-sdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meili-sdk-0.7.0.tar", last modified: Fri May  3 08:36:08 2024, max compression
+gzip compressed data, was "meili-sdk-0.7.1.tar", last modified: Mon May 27 10:46:43 2024, max compression
```

## Comparing `meili-sdk-0.7.0.tar` & `meili-sdk-0.7.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     5025 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4735 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.422376 meili-sdk-0.7.0/meili_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.425376 meili-sdk-0.7.0/meili_sdk/clients/
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/apitoken_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/base.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/persistent_token_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/clients/sdk_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.426376 meili-sdk-0.7.0/meili_sdk/config/
--rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/type.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/config/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.428376 meili-sdk-0.7.0/meili_sdk/models/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/form.py
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/organization.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/ros_setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/team.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/trigger.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/user.py
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/models/vehicle.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.429376 meili-sdk-0.7.0/meili_sdk/mqtt/
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/action_client.py
--rw-rw-rw-   0 root         (0) root         (0)     9679 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.430376 meili-sdk-0.7.0/meili_sdk/mqtt/models/
--rw-rw-rw-   0 root         (0) root         (0)      297 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/action.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/factsheet.py
--rw-rw-rw-   0 root         (0) root         (0)     3379 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/order.py
--rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/models/state.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/mqtt/site.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.432376 meili-sdk-0.7.0/meili_sdk/resources/
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5110 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/forms.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/maps.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/organizations.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/ros.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/teams.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/triggers.py
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/users.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/resources/vehicles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.433375 meili-sdk-0.7.0/meili_sdk/schedules/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/schedules/models.py
--rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/site.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/token.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.434376 meili-sdk-0.7.0/meili_sdk/websockets/
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18613 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/client.py
--rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/meili_sdk/websockets/models/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/action_definition.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/cancel_task_message.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/docking_routine_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/move_message.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/path.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/preset.py
--rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/station.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/task_v2.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/topic.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/traffic_control_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/update_map_message.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/meili_sdk/websockets/models/vehicle_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 08:36:08.424376 meili-sdk-0.7.0/meili_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5025 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2320 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-03 08:36:08.000000 meili-sdk-0.7.0/meili_sdk.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-03 08:36:08.437375 meili-sdk-0.7.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-03 08:35:59.000000 meili-sdk-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.477627 meili-sdk-0.7.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-05-27 10:46:43.477627 meili-sdk-0.7.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.464627 meili-sdk-0.7.1/meili_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.466627 meili-sdk-0.7.1/meili_sdk/clients/
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/clients/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/clients/apitoken_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/clients/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/clients/persistent_token_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/clients/sdk_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.467627 meili-sdk-0.7.1/meili_sdk/config/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/config/type.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/config/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.469627 meili-sdk-0.7.1/meili_sdk/models/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/form.py
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/organization.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/ros_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/team.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/trigger.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/models/vehicle.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.470627 meili-sdk-0.7.1/meili_sdk/mqtt/
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/action_client.py
+-rw-rw-rw-   0 root         (0) root         (0)    10085 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.470627 meili-sdk-0.7.1/meili_sdk/mqtt/models/
+-rw-rw-rw-   0 root         (0) root         (0)      297 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/models/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/models/factsheet.py
+-rw-rw-rw-   0 root         (0) root         (0)     3379 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/models/order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5239 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/models/state.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/mqtt/site.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.472627 meili-sdk-0.7.1/meili_sdk/resources/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5110 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/maps.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/organizations.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/ros.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/teams.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/triggers.py
+-rw-rw-rw-   0 root         (0) root         (0)      323 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/users.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/resources/vehicles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.473627 meili-sdk-0.7.1/meili_sdk/schedules/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/schedules/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/schedules/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/schedules/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/schedules/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      544 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/site.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/token.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.474627 meili-sdk-0.7.1/meili_sdk/websockets/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18613 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1828 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.476627 meili-sdk-0.7.1/meili_sdk/websockets/models/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/action_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/cancel_task_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/docking_routine_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7135 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/move_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/preset.py
+-rw-rw-rw-   0 root         (0) root         (0)      179 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/station.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/task_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/topic.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/traffic_control_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      854 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/update_map_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/meili_sdk/websockets/models/vehicle_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 10:46:43.465627 meili-sdk-0.7.1/meili_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5025 2024-05-27 10:46:43.000000 meili-sdk-0.7.1/meili_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-05-27 10:46:43.000000 meili-sdk-0.7.1/meili_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 10:46:43.000000 meili-sdk-0.7.1/meili_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-27 10:46:43.000000 meili-sdk-0.7.1/meili_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-27 10:46:43.000000 meili-sdk-0.7.1/meili_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-27 10:46:43.477627 meili-sdk-0.7.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-05-27 10:46:34.000000 meili-sdk-0.7.1/setup.py
```

### Comparing `meili-sdk-0.7.0/LICENSE.txt` & `meili-sdk-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/PKG-INFO` & `meili-sdk-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.7.0/README.md` & `meili-sdk-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/clients/__init__.py` & `meili-sdk-0.7.1/meili_sdk/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/clients/apitoken_client.py` & `meili-sdk-0.7.1/meili_sdk/clients/apitoken_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/clients/base.py` & `meili-sdk-0.7.1/meili_sdk/clients/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/clients/sdk_client.py` & `meili-sdk-0.7.1/meili_sdk/clients/sdk_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/exceptions.py` & `meili-sdk-0.7.1/meili_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/base.py` & `meili-sdk-0.7.1/meili_sdk/models/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/form.py` & `meili-sdk-0.7.1/meili_sdk/models/form.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/task.py` & `meili-sdk-0.7.1/meili_sdk/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/team.py` & `meili-sdk-0.7.1/meili_sdk/models/team.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/trigger.py` & `meili-sdk-0.7.1/meili_sdk/models/trigger.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/models/vehicle.py` & `meili-sdk-0.7.1/meili_sdk/models/vehicle.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/action_client.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/action_client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/client.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,33 +41,34 @@
         host: t.Optional[str] = None,
         port=1883,
         setup_uuid=None,
         open_handler=None,
         disconnect_handler=None,
         message_handler=None,
         subscribe_handler=None,
+        setup_lwt = None,
     ):
         host = host or get_host()
         self.url = urllib.parse.urlparse(host).hostname
 
         self.port = port
         self.client_id = client_id
         self.setup_uuid = setup_uuid
 
         self.client = _Client(client_id=client_id)
         self.client.username_pw_set(username=client_id, password=token)
         self.client.on_connect = self.__on_connect
         self.client.on_disconnect = self.__on_disconnect
         self.client.on_message = self.__on_message
         self.client.on_subscribe = self.__on_subscribe
-
         self.__open_handler = open_handler
         self.__disconnect_handler = disconnect_handler
         self.__message_handler = message_handler
         self.__subscribe_handler = subscribe_handler
+        self.__setup_lwt = setup_lwt
         self.__topics = {}
 
         self.connection_state = MqttConnectionStatus.UNKNOWN
 
     @classmethod
     def with_auto_token(
         cls,
@@ -89,14 +90,16 @@
     def subscribe_default_topics(self, vehicle_serial_number, manufacturer = "meili"):
         self.subscribe_to_orders(vehicle_serial_number, manufacturer=manufacturer)
         self.subscribe_to_actions(vehicle_serial_number, manufacturer=manufacturer)
         self.subscribe_to_factsheet(vehicle_serial_number, manufacturer=manufacturer)
 
     def run(self, block=False):
         try:
+            if self.__setup_lwt is not None:
+                self.__setup_lwt(self.client)
             self.connection_state = MqttConnectionStatus.CONNECTING
             self.client.connect(
                 self.url, port=self.port, keepalive=True, bind_address=""
             )
         except socket.gaierror as e:
             self.connection_state = MqttConnectionStatus.FAILED
             raise MqttException(
@@ -157,14 +160,18 @@
     def publish_to_state_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/state"
         return self.publish(topic, message, qos)
     
     def publish_to_factsheet_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=0):
         topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/factsheet"
         return self.publish_factsheet(topic, message, qos)
+    
+    def publish_to_connection_topic(self, vehicle_serial_number: str, message: any, manufacturer: str = "meili", qos=1):
+        topic = f"meili/v2/{manufacturer}/{vehicle_serial_number}/connection"
+        return self.publish(topic, message, qos)
 
     def wait_for_connection(self, timeout=10):
         """
         Block execution until connection is established
 
         If connection is still closed after timeout provided, it will raise TimeoutError
```

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/models/action.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/models/action.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/models/factsheet.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/models/factsheet.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/models/order.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/models/order.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/models/state.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/models/state.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/mqtt/site.py` & `meili-sdk-0.7.1/meili_sdk/mqtt/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/base.py` & `meili-sdk-0.7.1/meili_sdk/resources/base.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/forms.py` & `meili-sdk-0.7.1/meili_sdk/resources/forms.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/organizations.py` & `meili-sdk-0.7.1/meili_sdk/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/tasks.py` & `meili-sdk-0.7.1/meili_sdk/resources/tasks.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/teams.py` & `meili-sdk-0.7.1/meili_sdk/resources/teams.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/triggers.py` & `meili-sdk-0.7.1/meili_sdk/resources/triggers.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/resources/vehicles.py` & `meili-sdk-0.7.1/meili_sdk/resources/vehicles.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/schedules/loader.py` & `meili-sdk-0.7.1/meili_sdk/schedules/loader.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/schedules/models.py` & `meili-sdk-0.7.1/meili_sdk/schedules/models.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/site.py` & `meili-sdk-0.7.1/meili_sdk/site.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/client.py` & `meili-sdk-0.7.1/meili_sdk/websockets/client.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/constants.py` & `meili-sdk-0.7.1/meili_sdk/websockets/constants.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/__init__.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/message.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/task.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/task.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/task_v2.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/task_v2.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/traffic_control_action_message.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/traffic_control_action_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk/websockets/models/update_map_message.py` & `meili-sdk-0.7.1/meili_sdk/websockets/models/update_map_message.py`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/meili_sdk.egg-info/PKG-INFO` & `meili-sdk-0.7.1/meili_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meili-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Meili FMS SDK
 Home-page: https://gitlab.com/meilirobots/dev/meili-sdk
 Author: Meili Robots
 Author-email: info@meilirobots.com
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: MQTT
```

### Comparing `meili-sdk-0.7.0/meili_sdk.egg-info/SOURCES.txt` & `meili-sdk-0.7.1/meili_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meili-sdk-0.7.0/setup.cfg` & `meili-sdk-0.7.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = meili-sdk
 description = Meili FMS SDK
-version = 0.7.0
+version = 0.7.1
 license = MIT
 license_files = LICENSE.txt
 description_file = README.md
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Meili Robots
 author_email = info@meilirobots.com
```

