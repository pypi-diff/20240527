# Comparing `tmp/pykechain-4.8.1.tar.gz` & `tmp/pykechain-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykechain-4.8.1.tar", last modified: Thu Jul  6 08:40:31 2023, max compression
+gzip compressed data, was "pykechain-4.9.0.tar", last modified: Thu Sep 28 10:06:35 2023, max compression
```

## Comparing `pykechain-4.8.1.tar` & `pykechain-4.9.0.tar`

### file list

```diff
@@ -1,987 +1,990 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.690950 pykechain-4.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 08:40:18.000000 pykechain-4.8.1/.env.template
--rw-r--r--   0 runner    (1001) docker     (123)    46010 2023-07-06 08:40:18.000000 pykechain-4.8.1/CHANGELOG-v2-and-older.rst
--rw-r--r--   0 runner    (1001) docker     (123)    53954 2023-07-06 08:40:18.000000 pykechain-4.8.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 08:40:18.000000 pykechain-4.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-07-06 08:40:18.000000 pykechain-4.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-06 08:40:18.000000 pykechain-4.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-06 08:40:31.690950 pykechain-4.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-06 08:40:18.000000 pykechain-4.8.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)     3832 2023-07-06 08:40:18.000000 pykechain-4.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.530948 pykechain-4.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.530948 pykechain-4.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/bikemodel.png
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/bikeproduct.png
--rw-r--r--   0 runner    (1001) docker     (123)    37622 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/bikeproduct2.png
--rw-r--r--   0 runner    (1001) docker     (123)    31811 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/command_window_with_jupyter_notebook_response.png
--rw-r--r--   0 runner    (1001) docker     (123)    33870 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    33974 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/new_folder.png
--rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/_static/open_command_window.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.534948 pykechain-4.8.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/helpers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_activity.rst
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_banner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_base.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_expiring_download.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_form.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_input_checks.rst
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_notification.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_part.rst
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_property.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_representations_all.rst
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_scope.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_service.rst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_sidebar.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_teams.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_validators_all.rst
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_validators_base_validators.rst
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_validators_effects.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_widgets_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/models_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/developer_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/example_bike.rst
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-06 08:40:18.000000 pykechain-4.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 08:40:18.000000 pykechain-4.8.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.534948 pykechain-4.8.1/pykechain/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   165147 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22593 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31690 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/extra_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.538948 pykechain-4.8.1/pykechain/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48178 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/activity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/activity2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/association.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/banner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/base_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/expiring_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    23686 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/input_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    48449 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/part.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/part2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/partset.py
--rw-r--r--   0 runner    (1001) docker     (123)    22665 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2_activity_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2_multi_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property2_selectlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5313 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    12265 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property_multi_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/property_selectlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.542948 pykechain-4.8.1/pykechain/models/representations/
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/representations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/representations/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/representations/representation_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/representations/representations.py
--rw-r--r--   0 runner    (1001) docker     (123)    33719 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/scope2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.542948 pykechain-4.8.1/pykechain/models/sidebar/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/sidebar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/sidebar/sidebar_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/sidebar/sidebar_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/sidebar/sidebar_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/sidebar/sidebar_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/stored_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/tree_traversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.542948 pykechain-4.8.1/pykechain/models/validators/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/mime_types_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/validator_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    20653 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/validators/validators_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/value_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.542948 pykechain-4.8.1/pykechain/models/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    18733 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    21942 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/widget_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/widget_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)   102006 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/widgets/widgets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22214 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/models/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    22213 2023-07-06 08:40:18.000000 pykechain-4.8.1/pykechain/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.534948 pykechain-4.8.1/pykechain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-06 08:40:31.000000 pykechain-4.8.1/pykechain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    62619 2023-07-06 08:40:31.000000 pykechain-4.8.1/pykechain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 08:40:31.000000 pykechain-4.8.1/pykechain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-06 08:40:31.000000 pykechain-4.8.1/pykechain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-06 08:40:31.000000 pykechain-4.8.1/pykechain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-06 08:40:18.000000 pykechain-4.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-06 08:40:31.690950 pykechain-4.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-06 08:40:18.000000 pykechain-4.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.546948 pykechain-4.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/.keep_this_dir
--rw-r--r--   0 runner    (1001) docker     (123)    19475 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_assignees_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_assignees_list_no_assignees_gives_empty_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    14567 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_associated_objects_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    45198 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_associated_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_is_subprocess.json
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_is_task.json
--rw-r--r--   0 runner    (1001) docker     (123)    14817 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move.json
--rw-r--r--   0 runner    (1001) docker     (123)    12181 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move_under_part_object.json
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move_under_task_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    35390 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_parts_of_specific_type.json
--rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_children_of_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    13421 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_children_of_subprocess_with_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)    13207 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_form_collection.json
--rw-r--r--   0 runner    (1001) docker     (123)    13469 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_a_toplevel_task_returns_workflow_root_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_root.json
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_task.json
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_with_refs.json
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_test_workflow_root_object.json
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_without_scope_id_will_fix_itself.json
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_child.json
--rw-r--r--   0 runner    (1001) docker     (123)    16547 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_child_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_count_children.json
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_create_activity_with_incorrect_activity_class_fails.json
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_datetime_with_naive_duedate_only_fails.json
--rw-r--r--   0 runner    (1001) docker     (123)    13565 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_datetime_with_tzinfo_provides_correct_offset.json
--rw-r--r--   0 runner    (1001) docker     (123)    25694 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_assignee.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_clearing_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_naive_dates.json
--rw-r--r--   0 runner    (1001) docker     (123)    13511 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_status.json
--rw-r--r--   0 runner    (1001) docker     (123)    33921 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_cascade_down.json
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_due_date_timezone_aware.json
--rw-r--r--   0 runner    (1001) docker     (123)    13367 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_activities.json
--rw-r--r--   0 runner    (1001) docker     (123)    13317 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_activity_by_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    16909 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_all_children.json
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_children_of_task_fails_for_task.json
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess.json
--rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess_with_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_root.json
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_single_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_too_many_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_unknown_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    15641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_rootlevel_activity_is_rootlevel.json
--rw-r--r--   0 runner    (1001) docker     (123)    13307 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivities.test_subtask_activity_is_not_rootlevel.json
--rw-r--r--   0 runner    (1001) docker     (123)    13373 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test.json
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test_async_via_client.json
--rw-r--r--   0 runner    (1001) docker     (123)    12798 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test_async_via_task.json
--rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test_parent_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test_update.json
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityClone.test_update_incorrect.json
--rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityCloneParts.test.json
--rw-r--r--   0 runner    (1001) docker     (123)    68780 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityCloneParts.test_excluded_models.json
--rw-r--r--   0 runner    (1001) docker     (123)    17941 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widget_to_an_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets.json
--rw-r--r--   0 runner    (1001) docker     (123)    30673 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets_cross_form.json
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_below_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_on_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    29518 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_classification.json
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_classification.json
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_task_as_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    18439 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)   144849 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf.json
--rw-r--r--   0 runner    (1001) docker     (123)    86444 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf_async.json
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link.json
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link_with_from_user.json
--rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf.json
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf_with_from_user.json
--rw-r--r--   0 runner    (1001) docker     (123)    45180 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_association_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    47983 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_clear_associations.json
--rw-r--r--   0 runner    (1001) docker     (123)    49740 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_readable_models.json
--rw-r--r--   0 runner    (1001) docker     (123)    49480 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_remove_associations.json
--rw-r--r--   0 runner    (1001) docker     (123)    43230 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_association_incorrect_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    63616 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_associations.json
--rw-r--r--   0 runner    (1001) docker     (123)    45452 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_associations_interface.json
--rw-r--r--   0 runner    (1001) docker     (123)    45506 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_set_associations.json
--rw-r--r--   0 runner    (1001) docker     (123)    45330 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_set_associations_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)    45336 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_update_associations_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)    49700 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_update_widget_associations.json
--rw-r--r--   0 runner    (1001) docker     (123)    43226 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_model_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    43230 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_widget_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    43230 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_widgets_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    49744 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAssociations.test_writable_models.json
--rw-r--r--   0 runner    (1001) docker     (123)    20985 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_add_with_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)    17908 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_clear_an_attachment_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_has_value_false.json
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_has_value_true.json
--rw-r--r--   0 runner    (1001) docker     (123)    16453 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_attachment.json
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_filename_from_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_set_value_none.json
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_set_value_not_a_path.json
--rw-r--r--   0 runner    (1001) docker     (123)    18029 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestAttachment.test_upload.json
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_create_empty.json
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_create_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)    11550 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_banner_clear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    16407 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_single_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_get_active_banner.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banner.json
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banners.json
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banners_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)   130829 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_model_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_parent_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_model_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    51669 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_value.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsDeletion.test_bulk_delete_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestBulkPartsDeletion.test_bulk_delete_parts_with_wrong_input.json
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientAppVersions.test_compare_versions.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientAppVersions.test_retrieve_versions.json
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_clone_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_clone_scope_with_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_no_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)    16796 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_team_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_team_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_wrong_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_get_current_user.json
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_login.json
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_no_login.json
--rw-r--r--   0 runner    (1001) docker     (123)    25855 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_reload_deleted_object.json
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestClientLive.test_scope_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)    15720 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestCloneScopeAsync.test_clone_asynchronous.json
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContextCreate.test_create_context.json
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_context_consequetive_link_many_activities.json
--rw-r--r--   0 runner    (1001) docker     (123)    20223 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_context_unlink_single_activity_when_more_activities.json
--rw-r--r--   0 runner    (1001) docker     (123)    13457 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_create_contexts_bound_to_an_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    11297 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_link_context_to_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_contexts_via_client_using_scope_filter.json
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_multiple_context_via_client_using_filters.json
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_single_context_via_client_with_pk_filter.json
--rw-r--r--   0 runner    (1001) docker     (123)    15561 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestContexts.test_unlink_context_to_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExceptionsLive.test_api_error_with_argument_and_response.json
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExceptionsLive.test_api_error_with_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   462548 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_create_expiring_download_with_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_retrieve_expiring_downloads.json
--rw-r--r--   0 runner    (1001) docker     (123)   913162 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_save_expiring_download_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7457 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_update_expiring_download.json
--rw-r--r--   0 runner    (1001) docker     (123)   459773 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_upload_expiring_download.json
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_upload_wrong_content_path.json
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    65184 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_is_false.json
--rw-r--r--   0 runner    (1001) docker     (123)    68106 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_is_true.json
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_wrong_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    65534 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_instance_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)    72146 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)    65724 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_model_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)    65844 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_model_edit_with_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)    65446 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_retrieve_by_name_from_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    74065 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope_wrong_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    82343 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_forms_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)    66206 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_forms_retrieve_by_context_from_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    65234 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_forms_retrieve_instances_by_model_from_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    78159 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_cross_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    78116 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_no_target_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    78116 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_same_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    76150 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation.json
--rw-r--r--   0 runner    (1001) docker     (123)    76153 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_client.json
--rw-r--r--   0 runner    (1001) docker     (123)    76153 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    60990 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_wrong_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    94531 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_delete_forms.json
--rw-r--r--   0 runner    (1001) docker     (123)    29288 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_delete_forms_with_wrong_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    85537 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_instantiate_forms.json
--rw-r--r--   0 runner    (1001) docker     (123)   100438 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_apply_transition.json
--rw-r--r--   0 runner    (1001) docker     (123)    92014 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_apply_transition_with_wrong_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    96846 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    97040 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    95088 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_retrieve_possible_transitions.json
--rw-r--r--   0 runner    (1001) docker     (123)   101603 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees.json
--rw-r--r--   0 runner    (1001) docker     (123)    93562 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (123)    95981 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_input.json
--rw-r--r--   0 runner    (1001) docker     (123)    96780 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    96434 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    93883 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_non_connected_contexts_from_form.json
--rw-r--r--   0 runner    (1001) docker     (123)    32429 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_can_be_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    27627 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_with_wrong_payload.json
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17382 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19720 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15300 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_url.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_auth.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_pass.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__scope_id_and_no_pass.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_url.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__only_url.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__other_things_provided.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_and_token.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_token_and_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use_no_vars.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__not_for_travis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project_from_env__not_for_travis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_test_get_project_with_scope_id__not_for_travis.json
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create_with_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_delete_notification.json
--rw-r--r--   0 runner    (1001) docker     (123)    14127 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_delete_notification_from_client.json
--rw-r--r--   0 runner    (1001) docker     (123)    56528 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_all_notifications_retrieval.json
--rw-r--r--   0 runner    (1001) docker     (123)    15002 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit_incorrect_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    18798 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit_notification_clear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_from_user.json
--rw-r--r--   0 runner    (1001) docker     (123)    14490 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_recipient_users.json
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_team.json
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification.json
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification_raise_multiple_found.json
--rw-r--r--   0 runner    (1001) docker     (123)    14184 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification_raise_not_found.json
--rw-r--r--   0 runner    (1001) docker     (123)    12989 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartCreateModelWithProperties.test_create_model_with_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartCreateModelWithProperties.test_create_with_invalid_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_ids_with_bulk.json
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_names_with_bulk.json
--rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_no_bulk.json
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_all_children.json
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child.json
--rw-r--r--   0 runner    (1001) docker     (123)    18775 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_after_construction.json
--rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_caching.json
--rw-r--r--   0 runner    (1001) docker     (123)    13600 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_instances_of_a_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_instances_of_an_instances_raises_notfound.json
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_models_with_descendants_tree.json
--rw-r--r--   0 runner    (1001) docker     (123)    11887 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_parts_with_descendants_tree.json
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model_without_instances_raises_notfounderror.json
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_multiplicity_model_raises_multiplefounderror.json
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_retrieve_parts_with_refs.json
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test.json
--rw-r--r--   0 runner    (1001) docker     (123)    61183 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_bulk_update.json
--rw-r--r--   0 runner    (1001) docker     (123)    16049 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    19259 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    32563 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_attachment.json
--rw-r--r--   0 runner    (1001) docker     (123)    16053 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_missing_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    19442 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_property_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    24725 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_add_proxy_to.json
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_add_to_wrong_categories.json
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_base_comparison.json
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_base_hash.json
--rw-r--r--   0 runner    (1001) docker     (123)    19437 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_clone_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_clone_instance_with_multiplicity_violation.json
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_clone_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_count_children.json
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_count_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_model_where_parent_is_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_part_where_model_is_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_part_where_parent_is_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_proxy_model_where_model_is_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_create_proxy_model_where_parent_is_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    11530 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_clear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_instance_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    14381 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_instance_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    13617 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_model_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_kwargs_on_part_retrieval.json
--rw-r--r--   0 runner    (1001) docker     (123)    23981 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_add_delete_part.json
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_html_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_get_item_invalid.json
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_html_categories.json
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_html_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_iterator.json
--rw-r--r--   0 runner    (1001) docker     (123)    15517 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_with_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_with_limit.json
--rw-r--r--   0 runner    (1001) docker     (123)    27031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_catalog_model_of_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    11785 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_children_of_part.json
--rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_children_of_part_with_additional_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model.json
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model_multiple.json
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model_unknown.json
--rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_models.json
--rw-r--r--   0 runner    (1001) docker     (123)     5641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_non_existent_proxies_of_a_catalog_model_raises_error.json
--rw-r--r--   0 runner    (1001) docker     (123)     9101 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_parent_of_part.json
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_part_multiplicity.json
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_part_properties_in_a_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_proxy_of_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    19905 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_siblings_of_part.json
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_siblings_of_part_with_additional_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_multiple.json
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_part.json
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_unknown.json
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestParts.test_wrongly_create_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    12043 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsClassificationForm.test_classification_forms_exist.json
--rw-r--r--   0 runner    (1001) docker     (123)   269785 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_attachments.json
--rw-r--r--   0 runner    (1001) docker     (123)   132319 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_different_categories.json
--rw-r--r--   0 runner    (1001) docker     (123)   275231 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)   205683 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_model.json
--rw-r--r--   0 runner    (1001) docker     (123)   142227 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_missing_target_parent_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)   288573 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)   193239 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_empty_name_not_include_children.json
--rw-r--r--   0 runner    (1001) docker     (123)   212837 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_given_name_include_children.json
--rw-r--r--   0 runner    (1001) docker     (123)   284568 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_include_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)   150215 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_target_parent_inside_tree.json
--rw-r--r--   0 runner    (1001) docker     (123)   147330 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_too_many_target_parent_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)   247870 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_cross_scope_copy.json
--rw-r--r--   0 runner    (1001) docker     (123)   132319 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_different_categories.json
--rw-r--r--   0 runner    (1001) docker     (123)   176549 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_part_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)   242872 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_part_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    61685 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsImport.test_import_parts_from_client.json
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_not_list.json
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_of_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_names.json
--rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_objects.json
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_wrong_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)    37222 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_instance_to_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_clear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    18145 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    18129 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_unit.json
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_get_invalid_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_get_property_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    18114 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_get_property_by_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)    36892 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_move_property_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    20979 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_move_property_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    19360 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_part_of_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    18048 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_property_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_property_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_property_type.json
--rw-r--r--   0 runner    (1001) docker     (123)    15952 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_property_unit.json
--rw-r--r--   0 runner    (1001) docker     (123)    18166 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)    46288 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties_with_kwargs.json
--rw-r--r--   0 runner    (1001) docker     (123)    22854 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties_with_refs.json
--rw-r--r--   0 runner    (1001) docker     (123)    18056 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_property_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestProperties.test_set_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update.json
--rw-r--r--   0 runner    (1001) docker     (123)    24063 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_manual.json
--rw-r--r--   0 runner    (1001) docker     (123)    25932 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_reset.json
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertiesWithReferenceProperty.test_copy_reference_property_with_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    12986 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_reload.json
--rw-r--r--   0 runner    (1001) docker     (123)    22565 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    20359 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_value_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    21407 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_multiple_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    21415 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_no_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    21411 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_no_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    25810 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    18963 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_and_delete_property_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_incorrect_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_on_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_unknown_type.json
--rw-r--r--   0 runner    (1001) docker     (123)   100603 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_creation_of_all_property_model_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    15036 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_get_datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_iso_formatted.json
--rw-r--r--   0 runner    (1001) docker     (123)    23412 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_pending_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    17201 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    17197 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_iso_string.json
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_non_datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_none.json
--rw-r--r--   0 runner    (1001) docker     (123)    15040 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_to_datetime.json
--rw-r--r--   0 runner    (1001) docker     (123)    18202 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_value_via_part.json
--rw-r--r--   0 runner    (1001) docker     (123)   101867 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    43430 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_prefilter.json
--rw-r--r--   0 runner    (1001) docker     (123)    93445 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_boolean_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93544 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_date_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93432 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_float_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93382 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_int_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93482 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_link_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93816 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_select_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93500 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_test_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)   103921 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)   103993 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid_with_commas.json
--rw-r--r--   0 runner    (1001) docker     (123)    46651 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_prefilter.json
--rw-r--r--   0 runner    (1001) docker     (123)   105523 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_scope_reference_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93794 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_single_select_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    93500 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_text_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    98714 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_user_reference_property_filter_in_grid.json
--rw-r--r--   0 runner    (1001) docker     (123)    74445 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    74449 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_no_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    96470 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    82078 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    39157 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_add_excluded_propmodels_to_reference_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    41294 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_prefilters.json
--rw-r--r--   0 runner    (1001) docker     (123)    33491 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_sorting.json
--rw-r--r--   0 runner    (1001) docker     (123)    37999 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_copy_reference_property_with_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    37975 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    37975 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id_in_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    35243 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part.json
--rw-r--r--   0 runner    (1001) docker     (123)    35255 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part_in_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    28873 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing.json
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing_in_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    33960 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_excluded_propmodel_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    34013 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_prefilters.json
--rw-r--r--   0 runner    (1001) docker     (123)    31217 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_sorting.json
--rw-r--r--   0 runner    (1001) docker     (123)    58674 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_multi_ref_choices.json
--rw-r--r--   0 runner    (1001) docker     (123)    39087 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_excluded_propmodels_on_reference_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    41513 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_prefilters.json
--rw-r--r--   0 runner    (1001) docker     (123)    45000 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_referenced_part_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_selected_part_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    28869 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_list_with_no_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)    36958 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    48641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    48641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)    31683 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_retrieve_scope_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    37681 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_the_wrong_way.json
--rw-r--r--   0 runner    (1001) docker     (123)    34058 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_using_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)    41974 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_with_prefilters_and_validators.json
--rw-r--r--   0 runner    (1001) docker     (123)    47015 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_with_validation.json
--rw-r--r--   0 runner    (1001) docker     (123)    34496 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    34677 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_the_wrong_way.json
--rw-r--r--   0 runner    (1001) docker     (123)    34083 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_using_uuid.json
--rw-r--r--   0 runner    (1001) docker     (123)    42080 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_with_excluded_propmodels_and_validators.json
--rw-r--r--   0 runner    (1001) docker     (123)    34094 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_tuples.json
--rw-r--r--   0 runner    (1001) docker     (123)    44309 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_validation.json
--rw-r--r--   0 runner    (1001) docker     (123)    31217 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    31294 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    36272 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    46391 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_multi_ref_gives_back_all_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)    28865 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_nothing_is_referenced.json
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    32573 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value_using_id.json
--rw-r--r--   0 runner    (1001) docker     (123)    39208 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_fail_to_set_options_on_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_get_options_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    13030 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_illegal_options_are_not_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_integrity_options_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_options_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    15183 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_in_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    13026 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_not_in_options_raises_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_no_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_prefilters.json
--rw-r--r--   0 runner    (1001) docker     (123)    12958 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_reload.json
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_set_active_switch.json
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_set_columns.json
--rw-r--r--   0 runner    (1001) docker     (123)    19617 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    19277 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_value_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_fail_to_set_options_on_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_get_options_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_illegal_options_are_not_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_integrity_options_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)    21463 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_pend_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_options_list.json
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_value_in_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_value_not_in_options_raises_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    15189 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_multiple_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_no_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_no_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    20890 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    81961 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    84179 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    84501 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_validators.json
--rw-r--r--   0 runner    (1001) docker     (123)    84286 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_multiple_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    81973 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_no_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    81975 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_no_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    84204 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_value_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    86274 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_value_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_create.json
--rw-r--r--   0 runner    (1001) docker     (123)    10943 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_no_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_reload.json
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    16839 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_value_ids.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test__eq__.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_creation.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_format.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_parse_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_repr.json
--rw-r--r--   0 runner    (1001) docker     (123)    17143 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_validate.json
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_write_options.json
--rw-r--r--   0 runner    (1001) docker     (123)    19542 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_instance.json
--rw-r--r--   0 runner    (1001) docker     (123)    21871 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_model.json
--rw-r--r--   0 runner    (1001) docker     (123)    19538 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_with_validator_parses.json
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    13987 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_mode.json
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_mode_incorrect.json
--rw-r--r--   0 runner    (1001) docker     (123)    13982 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprActivity.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15274 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17384 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15294 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprButton.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprButton.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19707 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprButton.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprButton.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17341 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17344 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15270 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_mode.json
--rw-r--r--   0 runner    (1001) docker     (123)     9973 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_mode_incorrect.json
--rw-r--r--   0 runner    (1001) docker     (123)    15495 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)     9977 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprScope.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17370 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15288 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15252 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17322 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15256 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17361 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15271 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17524 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19834 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15457 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17551 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15418 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17500 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19841 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15255 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    14802 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_clear_project_info_edit_project.json
--rw-r--r--   0 runner    (1001) docker     (123)    11744 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_project_info.json
--rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope_clearing_values.json
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope_team.json
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_empty_project_info.json
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_get_landing_page.json
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_get_project_info.json
--rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_landing_page.json
--rw-r--r--   0 runner    (1001) docker     (123)    11700 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_project_info.json
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_project_info_with_wrong_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)   143027 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_leadmember.json
--rw-r--r--   0 runner    (1001) docker     (123)   143033 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)   143019 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_member.json
--rw-r--r--   0 runner    (1001) docker     (123)   128427 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_member_by_id.json
--rw-r--r--   0 runner    (1001) docker     (123)   131157 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_non_existing_member.json
--rw-r--r--   0 runner    (1001) docker     (123)   144809 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_supervisor.json
--rw-r--r--   0 runner    (1001) docker     (123)   128427 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_members.json
--rw-r--r--   0 runner    (1001) docker     (123)   148827 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_leadmember.json
--rw-r--r--   0 runner    (1001) docker     (123)   148819 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)   143003 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_member.json
--rw-r--r--   0 runner    (1001) docker     (123)   144801 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_supervisor.json
--rw-r--r--   0 runner    (1001) docker     (123)   128427 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_reset_members.json
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scope_with_kwargs.json
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scope_with_refs.json
--rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scopes.json
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_single_multiple.json
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_single_unknown.json
--rw-r--r--   0 runner    (1001) docker     (123)    18537 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_root_properties.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_scope_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_side_bar.json
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestScopes.test_team_property_of_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_debug_service_execution_terminate.json
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_log_of_service_execution.json
--rw-r--r--   0 runner    (1001) docker     (123)    17636 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_properties_of_service_execution.json
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions.json
--rw-r--r--   0 runner    (1001) docker     (123)    12994 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions_with_kwargs.json
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution.json
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_multiple.json
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_none.json
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_service_execution_conflict.json
--rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_debug_service_execute.json
--rw-r--r--   0 runner    (1001) docker     (123)    12365 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_edit_service_clear_values.json
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_properties_of_service.json
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_service_but_found_multiple.json
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_service_by_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services.json
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services_with_kwargs.json
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services_with_refs.json
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_single_service.json
--rw-r--r--   0 runner    (1001) docker     (123)    11798 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_service_context.json
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServices.test_update_service.json
--rw-r--r--   0 runner    (1001) docker     (123)    16106 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_and_delete_service.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_environment_version.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_service_type.json
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_get_executions_of_service.json
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_save_service_script.json
--rw-r--r--   0 runner    (1001) docker     (123)    14861 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_service_refresh_from_kechain.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_name.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_version.json
--rw-r--r--   0 runner    (1001) docker     (123)    15673 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service.json
--rw-r--r--   0 runner    (1001) docker     (123)    11076 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service_with_wrong_path.json
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_alignment.json
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_attributes_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    14645 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_attributes_sidebar.json
--rw-r--r--   0 runner    (1001) docker     (123)    21508 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_bulk_add_buttons.json
--rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_context_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_create_button.json
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_create_button_incorrect_arguments.json
--rw-r--r--   0 runner    (1001) docker     (123)    15415 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_delete_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    15886 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_edit_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_get_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_insert_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    18924 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_load_buttons.json
--rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_loading_of_existing_buttons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_override_sidebar_property.json
--rw-r--r--   0 runner    (1001) docker     (123)    15411 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_remove_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    16600 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_side_bar_permissions.json
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_sidebar_card_creation_inside_the_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_sidebar_card_object.json
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestSideBar.test_singleton_manager_per_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    70317 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_add_stored_file.json
--rw-r--r--   0 runner    (1001) docker     (123)    38999 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_delete_stored_file.json
--rw-r--r--   0 runner    (1001) docker     (123)    37941 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_edit_name_stored_file.json
--rw-r--r--   0 runner    (1001) docker     (123)    38091 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_edit_stored_file_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    37595 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_retrieve_stored_file.json
--rw-r--r--   0 runner    (1001) docker     (123)    37545 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_retrieve_stored_files.json
--rw-r--r--   0 runner    (1001) docker     (123)    12288 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTagsActivity.test_activity_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTagsActivity.test_activity_tags_may_be_emptied.json
--rw-r--r--   0 runner    (1001) docker     (123)     9259 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTagsScope.test_scope_tags.json
--rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTagsScope.test_scope_tags_may_be_emptied.json
--rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_add_and_remove_member.json
--rw-r--r--   0 runner    (1001) docker     (123)    22482 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_add_scope_to_team.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team_incorrect_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24773 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team_with_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_managers_members_owners.json
--rw-r--r--   0 runner    (1001) docker     (123)    14499 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_member_with_invalid_role.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_members.json
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_multiple_team_raises_error.json
--rw-r--r--   0 runner    (1001) docker     (123)    16205 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_team_with_known_teamname.json
--rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_unknown_team.json
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_teams.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_team_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_team_edit.json
--rw-r--r--   0 runner    (1001) docker     (123)    14503 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestTeams.test_team_edit_wrong_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19690 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17365 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19700 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17369 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19684 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15283 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15285 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19698 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17421 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19746 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15319 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_empty_config_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    17371 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19696 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15289 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17407 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19728 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17419 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15321 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_create_with_prop.json
--rw-r--r--   0 runner    (1001) docker     (123)    17389 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_get_set.json
--rw-r--r--   0 runner    (1001) docker     (123)    19714 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_set_value.json
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_unsupported_value.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_now_in_my_timezone.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_default_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_multiple_user_raises_error.json
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_unknown_user.json
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_id.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_username.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_email.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_language.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_name.json
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_timezone.json
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_users.json
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestUsers.test_user_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    43691 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_download_as_excel.json
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    45331 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_timezone_aware.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_activity_has_metapanel_in_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_can_be_found_with_uuid_in_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_in_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_manager_creation.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_not_found.json
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widgetmanager_has_activity_and_client.json
--rw-r--r--   0 runner    (1001) docker     (123)    25449 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    22335 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_associations_using_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    22335 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_editable_association.json
--rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    73454 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget_ke_chain_pages.json
--rw-r--r--   0 runner    (1001) docker     (123)    35704 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_dashboard_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    30552 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    28134 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget_with_prefilters_and_excluded_propmodels.json
--rw-r--r--   0 runner    (1001) docker     (123)    24095 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_html_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    19261 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    20464 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_with_progress_settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    34846 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_multicolumn_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    33196 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_notebook_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_progress_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    19569 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_project_info_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    32420 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_propertygrid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    20233 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_scope_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    19769 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_scopemembers_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    26408 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_service_card_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    34388 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_service_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    33641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_signature_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    30354 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_super_grid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    21028 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    23576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget_with_filters.json
--rw-r--r--   0 runner    (1001) docker     (123)    22455 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_create_widgets.json
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_all_widgets.json
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    16275 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget_stand_alone.json
--rw-r--r--   0 runner    (1001) docker     (123)    30984 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    30988 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title.json
--rw-r--r--   0 runner    (1001) docker     (123)    31022 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_and_meta.json
--rw-r--r--   0 runner    (1001) docker     (123)    38776 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_is_none.json
--rw-r--r--   0 runner    (1001) docker     (123)    56322 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_insert_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    19172 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_new_widget_using_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    25921 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_parent.json
--rw-r--r--   0 runner    (1001) docker     (123)    25061 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_property_grid_with_associations_using_widget_manager.json
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_scope_widget_invalid_inputs.json
--rw-r--r--   0 runner    (1001) docker     (123)    26454 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_widget_title.json
--rw-r--r--   0 runner    (1001) docker     (123)    28596 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetManagerWeatherWidget.test_weather_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    32600 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_disabled_button.json
--rw-r--r--   0 runner    (1001) docker     (123)    32558 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_external_link.json
--rw-r--r--   0 runner    (1001) docker     (123)    32641 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    32594 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_in_place.json
--rw-r--r--   0 runner    (1001) docker     (123)    27435 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_incorrect_keys.json
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_associated_parts.json
--rw-r--r--   0 runner    (1001) docker     (123)    26583 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_bulk_update.json
--rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_create_widget_in_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    18830 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_retrieve_widgets_in_activity.json
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_widget_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)    14298 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgets.test_widget_meta_attribute_is_not_None.json
--rw-r--r--   0 runner    (1001) docker     (123)    42511 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_copy_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    27155 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_copy_widget_with_wrong_target.json
--rw-r--r--   0 runner    (1001) docker     (123)    43711 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_move_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   130222 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   126346 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget_with_editable_association.json
--rw-r--r--   0 runner    (1001) docker     (123)   139367 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_filtered_grid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   135193 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_propertygrid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   136420 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_signature_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   139168 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_super_grid_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)   129786 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_weather_widget.json
--rw-r--r--   0 runner    (1001) docker     (123)    49396 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_create_delete_status_and_create_delete_workflow_transition.json
--rw-r--r--   0 runner    (1001) docker     (123)    19650 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_edit_workflow_description.json
--rw-r--r--   0 runner    (1001) docker     (123)    25229 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_in_and_activate.json
--rw-r--r--   0 runner    (1001) docker     (123)    31052 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_status_order.json
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_unlink_and_link_transitions.json
--rw-r--r--   0 runner    (1001) docker     (123)    28902 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_clone_workflow_in_a_scope_in_the_same_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    23376 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_clone_workflow_to_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_classmethod_create_workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_client_create_workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_scope_create_workflow.json
--rw-r--r--   0 runner    (1001) docker     (123)    17452 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_import_workflow_in_a_scope_with_import_workflow_method_on_scope.json
--rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_single_workflow_retrieve_on_pk.json
--rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/cassettes/TestWorkflows.test_workflow_attributes.json
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/files/test_import_parts/
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/files/test_import_parts/Wheel.xlsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/files/test_upload_content_to_expiring_download/
--rw-r--r--   0 runner    (1001) docker     (123)   121742 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/files/test_upload_content_to_expiring_download/test_upload_content.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/files/test_upload_image_to_attachment_property/
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/files/test_upload_image_to_attachment_property/test_upload_image.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.686950 pykechain-4.8.1/tests/files/test_upload_script_to_service/
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/files/test_upload_script_to_service/test_upload_script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:31.690950 pykechain-4.8.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_property_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_property_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    57190 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_property_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_property_selectlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_representations.py
--rw-r--r--   0 runner    (1001) docker     (123)    31679 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/models/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    39674 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_activities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_associations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_banners.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_expiring_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    26243 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    33293 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts.py
--rw-r--r--   0 runner    (1001) docker     (123)    30917 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_copy_move.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_create_with_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_reorder_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_parts_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    19790 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    32706 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_property_value_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    18860 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_sidebar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_stored_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6526 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    54557 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/test_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-06 08:40:18.000000 pykechain-4.8.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-06 08:40:18.000000 pykechain-4.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.632915 pykechain-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2023-09-28 10:06:21.000000 pykechain-4.9.0/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)    46010 2023-09-28 10:06:21.000000 pykechain-4.9.0/CHANGELOG-v2-and-older.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    54625 2023-09-28 10:06:21.000000 pykechain-4.9.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-28 10:06:21.000000 pykechain-4.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11375 2023-09-28 10:06:21.000000 pykechain-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-09-28 10:06:21.000000 pykechain-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-09-28 10:06:35.632915 pykechain-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2023-09-28 10:06:21.000000 pykechain-4.9.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2023-09-28 10:06:21.000000 pykechain-4.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.468913 pykechain-4.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.472913 pykechain-4.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    37057 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/bikemodel.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24864 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/bikeproduct.png
+-rw-r--r--   0 runner    (1001) docker     (127)    37622 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/bikeproduct2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31811 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/command_window_with_jupyter_notebook_response.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33870 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33974 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/new_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12262 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/_static/open_command_window.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.480913 pykechain-4.9.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/helpers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_activity.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_banner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_context.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_expiring_download.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_form.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_input_checks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_notification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_part.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_property.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_representations_all.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_scope.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_service.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_sidebar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_teams.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_users.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_validators_all.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_validators_base_validators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_validators_effects.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_widgets_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/models_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/developer_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/example_bike.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-28 10:06:21.000000 pykechain-4.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-09-28 10:06:21.000000 pykechain-4.9.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.484913 pykechain-4.9.0/pykechain/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165147 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22593 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40452 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31690 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/extra_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.496914 pykechain-4.9.0/pykechain/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48419 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/activity2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6137 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/base_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/expiring_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23686 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12232 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/input_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48449 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/part.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/partset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22665 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2_activity_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2_multi_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property2_selectlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property_multi_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/property_selectlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.496914 pykechain-4.9.0/pykechain/models/representations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/representations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/representations/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/representations/representation_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9789 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/representations/representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33719 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/scope2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15045 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.500913 pykechain-4.9.0/pykechain/models/sidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/sidebar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/sidebar/sidebar_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/sidebar/sidebar_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/sidebar/sidebar_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/sidebar/sidebar_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/stored_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/tree_traversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.500913 pykechain-4.9.0/pykechain/models/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/mime_types_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/validator_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20653 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/validators/validators_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/value_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.500913 pykechain-4.9.0/pykechain/models/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18733 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2126 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/widget_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/widget_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102006 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/widgets/widgets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22214 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/models/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22873 2023-09-28 10:06:21.000000 pykechain-4.9.0/pykechain/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.484913 pykechain-4.9.0/pykechain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2023-09-28 10:06:35.000000 pykechain-4.9.0/pykechain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    62889 2023-09-28 10:06:35.000000 pykechain-4.9.0/pykechain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-28 10:06:35.000000 pykechain-4.9.0/pykechain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-09-28 10:06:35.000000 pykechain-4.9.0/pykechain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-28 10:06:35.000000 pykechain-4.9.0/pykechain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-09-28 10:06:21.000000 pykechain-4.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-09-28 10:06:35.632915 pykechain-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4888 2023-09-28 10:06:21.000000 pykechain-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.504913 pykechain-4.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/.keep_this_dir
+-rw-r--r--   0 runner    (1001) docker     (127)    19475 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_assignees_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_assignees_list_no_assignees_gives_empty_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14567 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_associated_objects_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45198 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_associated_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11095 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_is_subprocess.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_is_task.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12181 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move_under_part_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move_under_task_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35390 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_parts_of_specific_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_children_of_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13421 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_children_of_subprocess_with_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13207 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_form_collection.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_a_toplevel_task_returns_workflow_root_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_root.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_task.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11091 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_with_refs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_test_workflow_root_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_without_scope_id_will_fix_itself.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11143 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_child.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16547 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_child_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_count_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_create_activity_with_incorrect_activity_class_fails.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11184 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_datetime_with_naive_duedate_only_fails.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_datetime_with_tzinfo_provides_correct_offset.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25694 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_assignee.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23027 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_clearing_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11234 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_naive_dates.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13511 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_status.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33921 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_cascade_down.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11238 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_due_date_timezone_aware.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_activity_by_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16909 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_all_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_children_of_task_fails_for_task.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess_with_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8829 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_root.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11093 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_single_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_too_many_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10587 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_unknown_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_rootlevel_activity_is_rootlevel.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivities.test_subtask_activity_is_not_rootlevel.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13373 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test_async_via_client.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12798 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test_async_via_task.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16924 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test_parent_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13497 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityClone.test_update_incorrect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72498 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityCloneParts.test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    68780 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityCloneParts.test_excluded_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17941 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widget_to_an_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30673 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets_cross_form.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_below_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10106 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_on_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29518 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_classification.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10590 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_task_as_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18439 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)   144849 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86444 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf_async.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12054 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link_with_from_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12001 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf_with_from_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45180 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_association_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47983 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_clear_associations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49740 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_readable_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49480 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_remove_associations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43230 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_association_incorrect_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    63616 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_associations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45452 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_associations_interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45506 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_set_associations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45330 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_set_associations_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45336 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_update_associations_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49700 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_update_widget_associations.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43226 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_model_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43230 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_widget_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43230 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_widgets_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49744 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAssociations.test_writable_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_add_with_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17908 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_clear_an_attachment_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13505 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_has_value_false.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_has_value_true.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16453 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_attachment.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_filename_from_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15640 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_set_value_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13501 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_set_value_not_a_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18029 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestAttachment.test_upload.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_create_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_create_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10104 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8112 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_edit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11550 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_banner_clear_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16407 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_single_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_get_active_banner.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10004 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banner.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banners.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banners_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130829 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_model_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_parent_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_model_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51669 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsDeletion.test_bulk_delete_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestBulkPartsDeletion.test_bulk_delete_parts_with_wrong_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientAppVersions.test_compare_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientAppVersions.test_retrieve_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_clone_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_clone_scope_with_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11707 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_no_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16796 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_team_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_team_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_wrong_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_get_current_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_login.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_no_login.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25855 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_reload_deleted_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10256 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestClientLive.test_scope_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15720 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestCloneScopeAsync.test_clone_asynchronous.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6997 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContextCreate.test_create_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_context_consequetive_link_many_activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20223 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_context_unlink_single_activity_when_more_activities.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13457 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_create_contexts_bound_to_an_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11297 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_link_context_to_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_contexts_via_client_using_scope_filter.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_multiple_context_via_client_using_filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11257 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_single_context_via_client_with_pk_filter.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15561 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestContexts.test_unlink_context_to_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExceptionsLive.test_api_error_with_argument_and_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExceptionsLive.test_api_error_with_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   462548 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_create_expiring_download_with_content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7620 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_retrieve_expiring_downloads.json
+-rw-r--r--   0 runner    (1001) docker     (127)   913162 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_save_expiring_download_content.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7457 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_update_expiring_download.json
+-rw-r--r--   0 runner    (1001) docker     (127)   459773 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_upload_expiring_download.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_upload_wrong_content_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60990 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60990 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65184 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_is_false.json
+-rw-r--r--   0 runner    (1001) docker     (127)    68106 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_is_true.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60990 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_wrong_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65534 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_instance_edit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    72146 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65724 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_model_edit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65844 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_model_edit_with_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65446 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_retrieve_by_name_from_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    74065 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60990 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope_wrong_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82343 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_forms_delete.json
+-rw-r--r--   0 runner    (1001) docker     (127)    66206 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_forms_retrieve_by_context_from_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    65234 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_forms_retrieve_instances_by_model_from_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    78159 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_cross_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    78116 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_no_target_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    78116 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_same_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76150 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76153 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_client.json
+-rw-r--r--   0 runner    (1001) docker     (127)    76153 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60990 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_wrong_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    94531 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_delete_forms.json
+-rw-r--r--   0 runner    (1001) docker     (127)    29288 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_delete_forms_with_wrong_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    85537 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_instantiate_forms.json
+-rw-r--r--   0 runner    (1001) docker     (127)   100438 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_apply_transition.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92014 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_apply_transition_with_wrong_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    96846 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    97040 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    95088 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_retrieve_possible_transitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)   101603 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93562 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    95981 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_input.json
+-rw-r--r--   0 runner    (1001) docker     (127)    96780 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    96434 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93883 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_non_connected_contexts_from_form.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32429 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_can_be_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27627 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_with_wrong_payload.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15304 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17382 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19720 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15300 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_auth.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_pass.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__scope_id_and_no_pass.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__only_url.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__other_things_provided.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_and_token.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_token_and_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use_no_vars.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__not_for_travis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project_from_env__not_for_travis.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_test_get_project_with_scope_id__not_for_travis.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12873 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21411 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14667 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create_with_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_delete_notification.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14127 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_delete_notification_from_client.json
+-rw-r--r--   0 runner    (1001) docker     (127)    56528 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_all_notifications_retrieval.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit_incorrect_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18798 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit_notification_clear_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14500 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_from_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14490 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_recipient_users.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14720 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_team.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14682 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification_raise_multiple_found.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14184 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification_raise_not_found.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12989 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartCreateModelWithProperties.test_create_model_with_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartCreateModelWithProperties.test_create_with_invalid_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_ids_with_bulk.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16342 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_names_with_bulk.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16343 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_no_bulk.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_all_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11163 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18775 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_after_construction.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_caching.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_instances_of_a_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_instances_of_an_instances_raises_notfound.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_models_with_descendants_tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11887 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_parts_with_descendants_tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9301 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10602 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model_without_instances_raises_notfounderror.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_multiplicity_model_raises_multiplefounderror.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8441 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_retrieve_parts_with_refs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22543 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test.json
+-rw-r--r--   0 runner    (1001) docker     (127)    61183 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_bulk_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16049 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19259 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32563 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_attachment.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_missing_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19442 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_property_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24725 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_add_proxy_to.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_add_to_wrong_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_base_comparison.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_base_hash.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19437 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_clone_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13217 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_clone_instance_with_multiplicity_violation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_clone_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_count_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_count_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11661 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_model_where_parent_is_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_part_where_model_is_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_part_where_parent_is_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_proxy_model_where_model_is_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_create_proxy_model_where_parent_is_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_clear_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_instance_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14381 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_instance_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13617 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_model_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6409 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_kwargs_on_part_retrieval.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23981 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_add_delete_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_html_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_get_item_invalid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_html_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_html_table.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_iterator.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15517 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_with_batch.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_with_limit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_catalog_model_of_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_children_of_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_children_of_part_with_additional_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model_unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_models.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_non_existent_proxies_of_a_catalog_model_raises_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9101 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_parent_of_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_part_multiplicity.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6383 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_part_properties_in_a_dict.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_proxy_of_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19905 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_siblings_of_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_siblings_of_part_with_additional_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12179 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12917 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5965 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestParts.test_wrongly_create_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12043 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsClassificationForm.test_classification_forms_exist.json
+-rw-r--r--   0 runner    (1001) docker     (127)   269785 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_attachments.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132319 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_different_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)   275231 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)   205683 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)   142227 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_missing_target_parent_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)   288573 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)   193239 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_empty_name_not_include_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)   212837 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_given_name_include_children.json
+-rw-r--r--   0 runner    (1001) docker     (127)   284568 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_include_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)   150215 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_target_parent_inside_tree.json
+-rw-r--r--   0 runner    (1001) docker     (127)   147330 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_too_many_target_parent_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)   247870 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_cross_scope_copy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132319 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_different_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)   176549 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_part_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)   242872 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_part_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    61685 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsImport.test_import_parts_from_client.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_not_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_of_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_names.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11369 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_wrong_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37222 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_instance_to_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22610 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_clear_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18145 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18100 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18129 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_unit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_get_invalid_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18056 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_get_property_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18114 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_get_property_by_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36892 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_move_property_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_move_property_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19360 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_part_of_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18048 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_property_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_property_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_property_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15952 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_property_unit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18166 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46288 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties_with_kwargs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22854 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties_with_refs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18056 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17966 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_property_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18081 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestProperties.test_set_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16047 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24063 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_manual.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25932 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_reset.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25053 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertiesWithReferenceProperty.test_copy_reference_property_with_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_reload.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22565 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20359 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_value_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21407 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28074 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_multiple_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21415 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_no_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21411 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_no_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25842 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25810 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18963 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_and_delete_property_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12789 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_incorrect_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_on_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11035 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_unknown_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)   100603 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_creation_of_all_property_model_types.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_get_datetime.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_iso_formatted.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23412 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_pending_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17201 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_iso_string.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_non_datetime.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17167 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_to_datetime.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18202 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_value_via_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)   101867 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43430 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_prefilter.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93445 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_boolean_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93544 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_date_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93432 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_float_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93382 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_int_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93482 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_link_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93816 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_select_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93500 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_test_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)   103921 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)   103993 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid_with_commas.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46651 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_prefilter.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105523 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_scope_reference_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93794 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_single_select_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93500 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_text_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    98714 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_user_reference_property_filter_in_grid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    74445 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    74449 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_no_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    96470 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    82078 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39157 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_add_excluded_propmodels_to_reference_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41294 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_prefilters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33491 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_sorting.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37999 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_copy_reference_property_with_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37975 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37975 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id_in_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35243 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35255 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part_in_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28873 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28865 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing_in_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33960 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_excluded_propmodel_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34013 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_prefilters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31217 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_sorting.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58674 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_multi_ref_choices.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39087 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_excluded_propmodels_on_reference_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41513 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_prefilters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_referenced_part_instances.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39069 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_selected_part_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28869 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_list_with_no_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36958 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    48641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31683 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_retrieve_scope_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34046 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37681 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_the_wrong_way.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34058 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_using_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41974 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_with_prefilters_and_validators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    47015 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_with_validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34496 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34677 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_the_wrong_way.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34083 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_using_uuid.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42080 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_with_excluded_propmodels_and_validators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34094 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_tuples.json
+-rw-r--r--   0 runner    (1001) docker     (127)    44309 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_validation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31217 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31294 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36272 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46391 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_multi_ref_gives_back_all_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28865 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_nothing_is_referenced.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32569 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32573 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value_using_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39208 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_fail_to_set_options_on_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_get_options_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_illegal_options_are_not_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13022 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_integrity_options_dict.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15846 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_options_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_in_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_not_in_options_raises_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10948 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_no_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_prefilters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12958 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_reload.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15375 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_set_active_switch.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13173 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_set_columns.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19617 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19277 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_value_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_fail_to_set_options_on_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_get_options_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_illegal_options_are_not_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_integrity_options_dict.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21463 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_pend_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15851 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_options_list.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_value_in_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13029 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_value_not_in_options_raises_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16731 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22850 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_multiple_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_no_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_no_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20918 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20890 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    81961 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84179 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84501 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_validators.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84286 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_multiple_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    81973 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_no_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    81975 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_no_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    84204 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_value_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    86274 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_value_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10943 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_create.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10943 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_no_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_reload.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16249 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16839 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_value_ids.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test__eq__.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_creation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_format.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_parse_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_repr.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17143 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_validate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_write_options.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19542 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_instance.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21871 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_model.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19538 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_with_validator_parses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11447 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13987 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_mode_incorrect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprActivity.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15274 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17348 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15298 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17384 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19670 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15294 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprButton.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprButton.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19707 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprButton.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprButton.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17341 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19647 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19640 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15270 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15492 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_mode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9973 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_mode_incorrect.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15495 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprScope.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19643 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15248 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17370 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19681 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15288 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15252 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17322 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19637 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15256 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17361 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15271 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15422 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17524 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19834 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15418 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15457 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17551 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19884 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15418 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17500 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19841 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15422 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19637 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_clear_project_info_edit_project.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11744 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_project_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14839 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope_clearing_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21114 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope_team.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_empty_project_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_get_landing_page.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_get_project_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19533 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_landing_page.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_project_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_project_info_with_wrong_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)   143027 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_leadmember.json
+-rw-r--r--   0 runner    (1001) docker     (127)   143033 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)   143019 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_member.json
+-rw-r--r--   0 runner    (1001) docker     (127)   128427 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_member_by_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)   131157 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_non_existing_member.json
+-rw-r--r--   0 runner    (1001) docker     (127)   144809 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_supervisor.json
+-rw-r--r--   0 runner    (1001) docker     (127)   128427 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_members.json
+-rw-r--r--   0 runner    (1001) docker     (127)   148827 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_leadmember.json
+-rw-r--r--   0 runner    (1001) docker     (127)   148819 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)   143003 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_member.json
+-rw-r--r--   0 runner    (1001) docker     (127)   144801 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_supervisor.json
+-rw-r--r--   0 runner    (1001) docker     (127)   128427 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_reset_members.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scope_with_kwargs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scope_with_refs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16753 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scopes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_single_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_single_unknown.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18537 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_root_properties.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_scope_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_side_bar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestScopes.test_team_property_of_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_debug_service_execution_terminate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16945 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_log_of_service_execution.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17636 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_properties_of_service_execution.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12994 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions_with_kwargs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14856 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25156 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_service_execution_conflict.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_debug_service_execute.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_edit_service_clear_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_properties_of_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_service_but_found_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_service_by_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services_with_kwargs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services_with_refs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_single_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_service_context.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServices.test_update_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_and_delete_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_environment_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_service_type.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12356 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_get_executions_of_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_save_service_script.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14861 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_service_refresh_from_kechain.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_version.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15673 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11076 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service_with_wrong_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15540 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_alignment.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15267 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_attributes_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14645 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_attributes_sidebar.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21508 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_bulk_add_buttons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17047 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_context_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12101 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_create_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_create_button_incorrect_arguments.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15415 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_delete_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_edit_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_get_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20445 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_insert_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_load_buttons.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_loading_of_existing_buttons.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11687 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_override_sidebar_property.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_remove_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16600 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_side_bar_permissions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15175 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_sidebar_card_creation_inside_the_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_sidebar_card_object.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestSideBar.test_singleton_manager_per_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    70317 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_add_stored_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38999 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_delete_stored_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37941 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_edit_name_stored_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38091 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_edit_stored_file_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37595 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_retrieve_stored_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    37545 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_retrieve_stored_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12288 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTagsActivity.test_activity_tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTagsActivity.test_activity_tags_may_be_emptied.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9259 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTagsScope.test_scope_tags.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTagsScope.test_scope_tags_may_be_emptied.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_add_and_remove_member.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22482 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_add_scope_to_team.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team_incorrect_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24773 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team_with_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_managers_members_owners.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_member_with_invalid_role.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_members.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16649 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_multiple_team_raises_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_team_with_known_teamname.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15773 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_unknown_team.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17053 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_teams.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_team_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_team_edit.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14503 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTeams.test_team_edit_wrong_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_offset_from_user_timezone.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_timezone_from_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_timezone_from_user_without_timezone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19690 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15291 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15287 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15287 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17369 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15283 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15285 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19698 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19746 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15319 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15297 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19646 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_empty_config_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17371 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19696 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19728 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15309 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17419 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19740 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15311 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_create_with_prop.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_get_set.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19714 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_set_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_unsupported_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_now_in_my_timezone.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_default_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_multiple_user_raises_error.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_unknown_user.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_id.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_username.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_email.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_language.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_name.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_timezone.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_users.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestUsers.test_user_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43691 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_download_as_excel.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17470 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45331 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_timezone_aware.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_activity_has_metapanel_in_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_can_be_found_with_uuid_in_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_in_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_manager_creation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_not_found.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14922 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widgetmanager_has_activity_and_client.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25449 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22335 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_associations_using_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22335 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_editable_association.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39069 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    73454 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget_ke_chain_pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35704 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_dashboard_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30552 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28134 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget_with_prefilters_and_excluded_propmodels.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24095 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_html_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19261 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20464 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_with_progress_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34846 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_multicolumn_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33196 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_notebook_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19643 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_progress_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19569 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_project_info_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32420 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_propertygrid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_scope_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19769 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_scopemembers_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26408 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_service_card_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_service_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_signature_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30354 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_super_grid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21028 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget_with_filters.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22455 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_create_widgets.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_all_widgets.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16271 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16275 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget_stand_alone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30984 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    30988 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31022 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_and_meta.json
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_is_none.json
+-rw-r--r--   0 runner    (1001) docker     (127)    56322 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_insert_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19172 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_new_widget_using_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25921 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_parent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25061 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_property_grid_with_associations_using_widget_manager.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15075 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_scope_widget_invalid_inputs.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26454 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_widget_title.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28596 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetManagerWeatherWidget.test_weather_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32600 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_disabled_button.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32558 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_external_link.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32641 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32594 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_in_place.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27435 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_incorrect_keys.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18224 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_associated_parts.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26583 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_bulk_update.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17163 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_create_widget_in_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_retrieve_widgets_in_activity.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_widget_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14298 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgets.test_widget_meta_attribute_is_not_None.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42511 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_copy_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27155 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_copy_widget_with_wrong_target.json
+-rw-r--r--   0 runner    (1001) docker     (127)    43711 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_move_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   130222 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   126346 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget_with_editable_association.json
+-rw-r--r--   0 runner    (1001) docker     (127)   139367 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_filtered_grid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   135193 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_propertygrid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   136420 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_signature_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   139168 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_super_grid_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)   129786 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_weather_widget.json
+-rw-r--r--   0 runner    (1001) docker     (127)    49396 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_create_delete_status_and_create_delete_workflow_transition.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19650 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_edit_workflow_description.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25229 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_in_and_activate.json
+-rw-r--r--   0 runner    (1001) docker     (127)    31052 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_status_order.json
+-rw-r--r--   0 runner    (1001) docker     (127)    22872 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_unlink_and_link_transitions.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28902 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_clone_workflow_in_a_scope_in_the_same_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23376 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_clone_workflow_to_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_classmethod_create_workflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_client_create_workflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10335 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_scope_create_workflow.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17452 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_import_workflow_in_a_scope_with_import_workflow_method_on_scope.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9019 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_single_workflow_retrieve_on_pk.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/cassettes/TestWorkflows.test_workflow_attributes.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/files/test_import_parts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7489 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/files/test_import_parts/Wheel.xlsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/files/test_upload_content_to_expiring_download/
+-rw-r--r--   0 runner    (1001) docker     (127)   121742 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/files/test_upload_content_to_expiring_download/test_upload_content.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/files/test_upload_image_to_attachment_property/
+-rw-r--r--   0 runner    (1001) docker     (127)     7576 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/files/test_upload_image_to_attachment_property/test_upload_image.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.628914 pykechain-4.9.0/tests/files/test_upload_script_to_service/
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/files/test_upload_script_to_service/test_upload_script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:35.632915 pykechain-4.9.0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4082 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_property_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_property_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57190 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_property_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_property_selectlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15533 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_representations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31679 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/models/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39674 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_activities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_associations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_banners.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14821 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_expiring_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26243 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33293 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_copy_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_create_with_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_reorder_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_parts_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19790 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32706 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_property_value_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16010 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15616 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_sidebar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_stored_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54557 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8269 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2023-09-28 10:06:21.000000 pykechain-4.9.0/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-09-28 10:06:21.000000 pykechain-4.9.0/tox.ini
```

### Comparing `pykechain-4.8.1/.env.template` & `pykechain-4.9.0/.env.template`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/CHANGELOG-v2-and-older.rst` & `pykechain-4.9.0/CHANGELOG-v2-and-older.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/CHANGELOG.rst` & `pykechain-4.9.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Change Log
 ==========
 
+v4.9.0 (28SEP23)
+----------------
+* :+1: Changed the way we download pdf's from activity where we now provide the `timezone` query param in the request URL with timezone info for a more accurate determination of the display of time information in the pdf taking into account the timezone and timesystem info. For compatability sake we maintain the `offset` query param in the request to support older KE-chain backend versions.
+* :+1: dependent versions for development: sphinx (7.2.6 for >= py3.9+ 7.1.2 for <= py3.8), tox (4.11.3), flake8 (6.1.0), jsonschema (4.19.0), importlib-metadata (6.8.0), mypy (1.5.1), pytest (7.4.2), pytz (2023.3.post1), nbsphinx (0.9.3)
+
 v4.8.1 (06JUL23)
----------------
+----------------
 * :star: Added the possibility to set the list of columns and the active switch on a `ScopeReferenceProperty`. (#1340)
 * :+1: dependent versions for development: mypy (1.4.1), tox (4.6.3), pytest (7.4.0), pytest-cov (4.1.0), pytest-xdist (3.3.1)
 
 v4.8.0 (23JUN23)
----------------
+----------------
 * :star: Number of tests on certain modules has been increased. (#1328)
 * :star: The unit of `max_size` on a `FileSizeValidator` has been changed to MB. (#1328)
 * :+1: dependent versions for development: tox (4.6.2), pytest (7.3.2), coverage (7.2.7), semver (3.0.1), pre-commit (3.3.3), importlib-metadata (6.6.0), pytz (2023.3), sphinx (7.0.1), nbsphinx (0.9.2), requests (2.31.0)
 
 v4.7.0 (17APR23)
-_______________
+----------------
 * :star: Added the possibility to create, edit and delete `StoredFiles`. (#1298)
 * :star: Added the concept of a `StoredFilesReferenceProperty`. (#1306)
 * :star: Added `fileDisplay` representation for `StoredFilesReferenceProperty`. (#1306)
 * :+1: dependent versions for development: pre-commit (3.2.2), pytest-xdist (3.2.1), coverage (7.2.3), tox (4.4.12), mypy (1.2.0)
 
 v4.6.0 (16FEB23)
 ----------------
```

### Comparing `pykechain-4.8.1/LICENSE` & `pykechain-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/PKG-INFO` & `pykechain-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykechain
-Version: 4.8.1
+Version: 4.9.0
 Summary: KE-chain Python SDK
 Home-page: https://github.com/KE-works/pykechain
 Author: KE-works BV
 Author-email: support+pykechain@ke-works.com
 License: Apache Open Source License 2.0
 Project-URL: Documentation, https://pykechain.readthedocs.io/en/latest
 Project-URL: Changelog, https://github.com/KE-works/pykechain/blob/master/CHANGELOG.rst
```

### Comparing `pykechain-4.8.1/README.rst` & `pykechain-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/Makefile` & `pykechain-4.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/bikemodel.png` & `pykechain-4.9.0/docs/_static/bikemodel.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/bikeproduct.png` & `pykechain-4.9.0/docs/_static/bikeproduct.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/bikeproduct2.png` & `pykechain-4.9.0/docs/_static/bikeproduct2.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/command_window_with_jupyter_notebook_response.png` & `pykechain-4.9.0/docs/_static/command_window_with_jupyter_notebook_response.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/logo.png` & `pykechain-4.9.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/new_folder.png` & `pykechain-4.9.0/docs/_static/new_folder.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/_static/open_command_window.png` & `pykechain-4.9.0/docs/_static/open_command_window.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/api/models_property.rst` & `pykechain-4.9.0/docs/api/models_property.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/api/models_representations_all.rst` & `pykechain-4.9.0/docs/api/models_representations_all.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/api/models_validators_all.rst` & `pykechain-4.9.0/docs/api/models_validators_all.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/api/models_validators_effects.rst` & `pykechain-4.9.0/docs/api/models_validators_effects.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/api/models_widgets_widgets.rst` & `pykechain-4.9.0/docs/api/models_widgets_widgets.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/conf.py` & `pykechain-4.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/example_bike.rst` & `pykechain-4.9.0/docs/example_bike.rst`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/docs/make.bat` & `pykechain-4.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/__init__.py` & `pykechain-4.9.0/pykechain/__init__.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/client.py` & `pykechain-4.9.0/pykechain/client.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/client_utils.py` & `pykechain-4.9.0/pykechain/client_utils.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/defaults.py` & `pykechain-4.9.0/pykechain/defaults.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/enums.py` & `pykechain-4.9.0/pykechain/enums.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/exceptions.py` & `pykechain-4.9.0/pykechain/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/extra_utils.py` & `pykechain-4.9.0/pykechain/extra_utils.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/helpers.py` & `pykechain-4.9.0/pykechain/helpers.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/__init__.py` & `pykechain-4.9.0/pykechain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/activity.py` & `pykechain-4.9.0/pykechain/models/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from pykechain.models.user import User
 from pykechain.models.widgets.widgets_manager import WidgetsManager
 from pykechain.utils import (
     Empty,
     clean_empty_values,
     empty,
     get_offset_from_user_timezone,
+    get_timezone_from_user,
     is_valid_email,
     parse_datetime,
 )
 
 
 class Activity(TreeObject, TagsMixin):
     """A virtual object representing a KE-chain activity.
@@ -952,15 +953,16 @@
             appendices=check_type(include_appendices, bool, "include_appendices"),
             includeqr=check_type(include_qr_code, bool, "include_qr_code"),
         )
 
         if user:
             user_object = check_type(user, User, "user")
             request_params.update(
-                offset=get_offset_from_user_timezone(user=user_object)
+                offset=get_offset_from_user_timezone(user=user_object),
+                timezone=str(get_timezone_from_user(user=user_object)),
             )
 
         url = self._client._build_url("activity_export", activity_id=self.id)
         response = self._client._request("GET", url, params=request_params)
         if response.status_code != requests.codes.ok:  # pragma: no cover
             raise APIError(
                 f"Could not download PDF of Activity {self}", response=response
@@ -1051,14 +1053,15 @@
         )
 
         if from_user:
             check_user(from_user, User, "from_user")
             params.update(
                 from_user=from_user.id,
                 offset=get_offset_from_user_timezone(user=from_user),
+                timezone=str(get_timezone_from_user(user=from_user)),
             )
 
         url = self._client._build_url("notification_share_activity_link")
 
         response = self._client._request("POST", url, data=params)
 
         if response.status_code not in (
@@ -1142,14 +1145,15 @@
         )
 
         if from_user:
             check_user(from_user, User, "from_user")
             params.update(
                 from_user=from_user.id,
                 offset=get_offset_from_user_timezone(user=from_user),
+                timezone=str(get_timezone_from_user(user=from_user)),
             )
 
         url = self._client._build_url("notification_share_activity_pdf")
 
         response = self._client._request("POST", url, data=params)
 
         if response.status_code not in (
```

### Comparing `pykechain-4.8.1/pykechain/models/activity2.py` & `pykechain-4.9.0/pykechain/models/activity2.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/association.py` & `pykechain-4.9.0/pykechain/models/association.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/banner.py` & `pykechain-4.9.0/pykechain/models/banner.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/base.py` & `pykechain-4.9.0/pykechain/models/base.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/base_reference.py` & `pykechain-4.9.0/pykechain/models/base_reference.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/context.py` & `pykechain-4.9.0/pykechain/models/context.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/expiring_download.py` & `pykechain-4.9.0/pykechain/models/expiring_download.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/form.py` & `pykechain-4.9.0/pykechain/models/form.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/input_checks.py` & `pykechain-4.9.0/pykechain/models/input_checks.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/notification.py` & `pykechain-4.9.0/pykechain/models/notification.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/part.py` & `pykechain-4.9.0/pykechain/models/part.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/partset.py` & `pykechain-4.9.0/pykechain/models/partset.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property.py` & `pykechain-4.9.0/pykechain/models/property.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property2.py` & `pykechain-4.9.0/pykechain/models/property2.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property_attachment.py` & `pykechain-4.9.0/pykechain/models/property_attachment.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property_datetime.py` & `pykechain-4.9.0/pykechain/models/property_datetime.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property_multi_reference.py` & `pykechain-4.9.0/pykechain/models/property_multi_reference.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property_reference.py` & `pykechain-4.9.0/pykechain/models/property_reference.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/property_selectlist.py` & `pykechain-4.9.0/pykechain/models/property_selectlist.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/representations/__init__.py` & `pykechain-4.9.0/pykechain/models/representations/__init__.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/representations/component.py` & `pykechain-4.9.0/pykechain/models/representations/component.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/representations/representation_base.py` & `pykechain-4.9.0/pykechain/models/representations/representation_base.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/representations/representations.py` & `pykechain-4.9.0/pykechain/models/representations/representations.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/scope.py` & `pykechain-4.9.0/pykechain/models/scope.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/service.py` & `pykechain-4.9.0/pykechain/models/service.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/sidebar/sidebar_base.py` & `pykechain-4.9.0/pykechain/models/sidebar/sidebar_base.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/sidebar/sidebar_button.py` & `pykechain-4.9.0/pykechain/models/sidebar/sidebar_button.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/sidebar/sidebar_card.py` & `pykechain-4.9.0/pykechain/models/sidebar/sidebar_card.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/sidebar/sidebar_manager.py` & `pykechain-4.9.0/pykechain/models/sidebar/sidebar_manager.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/stored_file.py` & `pykechain-4.9.0/pykechain/models/stored_file.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/tags.py` & `pykechain-4.9.0/pykechain/models/tags.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/team.py` & `pykechain-4.9.0/pykechain/models/team.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/tree_traversal.py` & `pykechain-4.9.0/pykechain/models/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/user.py` & `pykechain-4.9.0/pykechain/models/user.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/__init__.py` & `pykechain-4.9.0/pykechain/models/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/effects.py` & `pykechain-4.9.0/pykechain/models/validators/effects.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/mime_types_defaults.py` & `pykechain-4.9.0/pykechain/models/validators/mime_types_defaults.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/validator_schemas.py` & `pykechain-4.9.0/pykechain/models/validators/validator_schemas.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/validators.py` & `pykechain-4.9.0/pykechain/models/validators/validators.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/validators/validators_base.py` & `pykechain-4.9.0/pykechain/models/validators/validators_base.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/value_filter.py` & `pykechain-4.9.0/pykechain/models/value_filter.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/__init__.py` & `pykechain-4.9.0/pykechain/models/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/enums.py` & `pykechain-4.9.0/pykechain/models/widgets/enums.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/helpers.py` & `pykechain-4.9.0/pykechain/models/widgets/helpers.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/widget.py` & `pykechain-4.9.0/pykechain/models/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/widget_models.py` & `pykechain-4.9.0/pykechain/models/widgets/widget_models.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/widget_schemas.py` & `pykechain-4.9.0/pykechain/models/widgets/widget_schemas.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/widgets/widgets_manager.py` & `pykechain-4.9.0/pykechain/models/widgets/widgets_manager.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/models/workflow.py` & `pykechain-4.9.0/pykechain/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/pykechain/utils.py` & `pykechain-4.9.0/pykechain/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     List,
     Optional,
     TypeVar,
     Union,
 )  # noqa: F401
 
 import pytz
+from pytz.exceptions import UnknownTimeZoneError
 
 from pykechain.exceptions import MultipleFoundError, NotFoundError
 
 T = TypeVar("T")
 
 UUID_REGEX_PATTERN = (
     r"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
@@ -681,7 +682,28 @@
     :type user: User object
     :return: number of minutes to the nearest integer
     """
     user_timezone = pytz.timezone(user.timezone.zone)
     user_time = datetime.now(user_timezone)
     offset = -int(user_time.tzinfo.utcoffset(user_time).total_seconds() / 60.0)
     return offset
+
+
+def get_timezone_from_user(user: "User") -> pytz.BaseTzInfo:
+    """
+    Get the timezone from the given user.
+
+    If you need the timezone as a string, either wrap it in str() or access
+    timezone.zone.
+
+    :param user: The user object.
+    :return: The timezone object
+    """
+    try:
+        user_timezone = pytz.timezone(user.timezone.zone)
+    except UnknownTimeZoneError:
+        # when there is no timezone defined on the user object, this error is
+        # triggered, so we return UTC by default
+        return pytz.UTC
+    if not user_timezone:
+        return pytz.UTC
+    return user_timezone
```

### Comparing `pykechain-4.8.1/pykechain.egg-info/PKG-INFO` & `pykechain-4.9.0/pykechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykechain
-Version: 4.8.1
+Version: 4.9.0
 Summary: KE-chain Python SDK
 Home-page: https://github.com/KE-works/pykechain
 Author: KE-works BV
 Author-email: support+pykechain@ke-works.com
 License: Apache Open Source License 2.0
 Project-URL: Documentation, https://pykechain.readthedocs.io/en/latest
 Project-URL: Changelog, https://github.com/KE-works/pykechain/blob/master/CHANGELOG.rst
```

### Comparing `pykechain-4.8.1/pykechain.egg-info/SOURCES.txt` & `pykechain-4.9.0/pykechain.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -817,14 +817,17 @@
 tests/cassettes/TestTeams.test_retrieve_single_multiple_team_raises_error.json
 tests/cassettes/TestTeams.test_retrieve_single_team_with_known_teamname.json
 tests/cassettes/TestTeams.test_retrieve_single_unknown_team.json
 tests/cassettes/TestTeams.test_retrieve_teams.json
 tests/cassettes/TestTeams.test_team_attributes.json
 tests/cassettes/TestTeams.test_team_edit.json
 tests/cassettes/TestTeams.test_team_edit_wrong_inputs.json
+tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_offset_from_user_timezone.json
+tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_timezone_from_user.json
+tests/cassettes/TestTimezoneHelperFunctions.test_retrieve_timezone_from_user_without_timezone.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_create_with_prop.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_get_set.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_set_value.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_unsupported_value.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_create_with_prop.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_get_set.json
 tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_set_value.json
```

### Comparing `pykechain-4.8.1/requirements.txt` & `pykechain-4.9.0/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # basis
 requests==2.31.0
 envparse==0.2.0
 
 # json validation (inspector)
-jsonschema==4.17.3
+jsonschema==4.19.0
 
 # for version comparison
 semver==3.0.1
 
 # testing
-pytest==7.4.0
+pytest==7.4.2
 pytest-xdist[psutil]==3.3.1
 betamax==0.8.1
 coverage~=6.5.0  # pinned to <7 as coveralls is preventing v7 for coverage
 pytest-cov==4.1.0
 coveralls==3.3.1
 
 # documentation
-Sphinx==7.0.1
-nbsphinx==0.9.2
+Sphinx==7.2.6; python_version >= '3.9'
+Sphinx~=7.1.2; python_version <= '3.8'
+nbsphinx==0.9.3
 
 # integration
-tox==4.6.3
+tox==4.11.3
 
 # code style
-flake8==6.0.0
-importlib-metadata==6.6.0
+flake8==6.1.0
+importlib-metadata==6.8.0
 pydocstyle==6.3.0
-mypy==1.4.1; python_version >= '3.4'
+mypy==1.5.1; python_version >= '3.4'
 pre-commit==3.3.3
 
 # for package management (uploads)
 twine~=4.0; python_version >= '3.7'
 twine~=3.0; python_version <= '3.6'
 
-pytz==2023.3
+pytz==2023.3.post1
```

### Comparing `pykechain-4.8.1/setup.py` & `pykechain-4.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_assignees_list.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_assignees_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_assignees_list_no_assignees_gives_empty_list.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_assignees_list_no_assignees_gives_empty_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_associated_objects_ids.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_associated_objects_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_associated_parts.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_associated_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_is_subprocess.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_is_subprocess.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_is_task.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_is_task.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move_under_part_object.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move_under_part_object.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_move_under_task_parent.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_move_under_task_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_parts_of_specific_type.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_parts_of_specific_type.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_children_of_parent.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_children_of_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_children_of_subprocess_with_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_children_of_subprocess_with_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_form_collection.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_form_collection.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_a_toplevel_task_returns_workflow_root_id.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_a_toplevel_task_returns_workflow_root_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_root.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_root.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_task.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_parent_of_task.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_retrieve_with_refs.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_retrieve_with_refs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_test_workflow_root_object.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_test_workflow_root_object.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_activity_without_scope_id_will_fix_itself.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_activity_without_scope_id_will_fix_itself.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_child.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_child.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_child_invalid.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_child_invalid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_count_children.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_count_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_create_activity_with_incorrect_activity_class_fails.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_create_activity_with_incorrect_activity_class_fails.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_datetime_with_naive_duedate_only_fails.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_datetime_with_naive_duedate_only_fails.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_datetime_with_tzinfo_provides_correct_offset.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_datetime_with_tzinfo_provides_correct_offset.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_assignee.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_assignee.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_clearing_values.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_clearing_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_description.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_naive_dates.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_naive_dates.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_name.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_activity_status.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_activity_status.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_cascade_down.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_cascade_down.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_edit_due_date_timezone_aware.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_edit_due_date_timezone_aware.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_activities.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_activities.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_activity_by_id.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_activity_by_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_all_children.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_all_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_children_of_task_fails_for_task.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_children_of_task_fails_for_task.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess_with_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_a_task_in_a_subprocess_with_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_siblings_of_root.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_siblings_of_root.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_single_activity.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_single_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_too_many_activity.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_too_many_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_retrieve_unknown_activity.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_retrieve_unknown_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_rootlevel_activity_is_rootlevel.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_rootlevel_activity_is_rootlevel.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivities.test_subtask_activity_is_not_rootlevel.json` & `pykechain-4.9.0/tests/cassettes/TestActivities.test_subtask_activity_is_not_rootlevel.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test_async_via_client.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test_async_via_client.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test_async_via_task.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test_async_via_task.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test_parent_id.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test_parent_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test_update.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test_update.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityClone.test_update_incorrect.json` & `pykechain-4.9.0/tests/cassettes/TestActivityClone.test_update_incorrect.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityCloneParts.test.json` & `pykechain-4.9.0/tests/cassettes/TestActivityCloneParts.test.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityCloneParts.test_excluded_models.json` & `pykechain-4.9.0/tests/cassettes/TestActivityCloneParts.test_excluded_models.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widget_to_an_activity.json` & `pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widget_to_an_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets.json` & `pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets_cross_form.json` & `pykechain-4.9.0/tests/cassettes/TestActivityCloneWidgets.test_clone_widgets_cross_form.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_below_parent.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_below_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_on_scope.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_on_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_classification.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_classification.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_classification.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_classification.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_parent.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_incorrect_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_create_with_task_as_parent.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_create_with_task_as_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityConstruction.test_delete.json` & `pykechain-4.9.0/tests/cassettes/TestActivityConstruction.test_delete.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf_async.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_download_as_pdf_async.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link_with_from_user.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_link_with_from_user.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf_with_from_user.json` & `pykechain-4.9.0/tests/cassettes/TestActivityDownloadAsPDF.test_activity_share_pdf_with_from_user.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_association_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_association_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_clear_associations.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_clear_associations.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_readable_models.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_readable_models.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_remove_associations.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_remove_associations.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_association_incorrect_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_association_incorrect_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_associations.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_associations.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_retrieve_associations_interface.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_retrieve_associations_interface.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_set_associations.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_set_associations.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_set_associations_empty.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_set_associations_empty.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_update_associations_empty.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_update_associations_empty.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_update_widget_associations.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_update_widget_associations.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_model_input.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_model_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_widget_input.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_widget_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_validate_widgets_input.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_validate_widgets_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAssociations.test_writable_models.json` & `pykechain-4.9.0/tests/cassettes/TestAssociations.test_writable_models.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_add_with_properties.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_add_with_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_clear_an_attachment_property.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_clear_an_attachment_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_has_value_false.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_has_value_false.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_has_value_true.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_has_value_true.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_attachment.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_attachment.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_filename_from_value.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_filename_from_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_retrieve_value.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_retrieve_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_set_value_none.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_set_value_none.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_set_value_not_a_path.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_set_value_not_a_path.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestAttachment.test_upload.json` & `pykechain-4.9.0/tests/cassettes/TestAttachment.test_upload.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_create_empty.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_create_empty.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_create_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_create_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_delete.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_delete.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_edit.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_edit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_banner_clear_values.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_banner_clear_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_edit_single_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_edit_single_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_get_active_banner.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_get_active_banner.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banner.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banner.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banners.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banners.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBanners.test_get_banners_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestBanners.test_get_banners_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_model_id.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_model_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_name.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_parent_id.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_parent_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_properties.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_model_id.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_model_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_name.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_value.json` & `pykechain-4.9.0/tests/cassettes/TestBulkPartsCreation.test_bulk_create_parts_without_property_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientAppVersions.test_compare_versions.json` & `pykechain-4.9.0/tests/cassettes/TestClientAppVersions.test_compare_versions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientAppVersions.test_retrieve_versions.json` & `pykechain-4.9.0/tests/cassettes/TestClientAppVersions.test_retrieve_versions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_clone_scope.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_clone_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_clone_scope_with_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_clone_scope_with_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_no_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_no_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_team_name.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_team_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_team_uuid.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_team_uuid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_create_scope_with_wrong_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_create_scope_with_wrong_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_get_current_user.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_get_current_user.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_login.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_login.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_no_login.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_no_login.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_reload_deleted_object.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_reload_deleted_object.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestClientLive.test_scope_delete.json` & `pykechain-4.9.0/tests/cassettes/TestClientLive.test_scope_delete.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestCloneScopeAsync.test_clone_asynchronous.json` & `pykechain-4.9.0/tests/cassettes/TestCloneScopeAsync.test_clone_asynchronous.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContextCreate.test_create_context.json` & `pykechain-4.9.0/tests/cassettes/TestContextCreate.test_create_context.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_context_consequetive_link_many_activities.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_context_consequetive_link_many_activities.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_context_unlink_single_activity_when_more_activities.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_context_unlink_single_activity_when_more_activities.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_create_contexts_bound_to_an_activity.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_create_contexts_bound_to_an_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_link_context_to_activity.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_link_context_to_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_contexts_via_client_using_scope_filter.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_contexts_via_client_using_scope_filter.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_multiple_context_via_client_using_filters.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_multiple_context_via_client_using_filters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_retrieve_single_context_via_client_with_pk_filter.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_retrieve_single_context_via_client_with_pk_filter.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestContexts.test_unlink_context_to_activity.json` & `pykechain-4.9.0/tests/cassettes/TestContexts.test_unlink_context_to_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExceptionsLive.test_api_error_with_argument_and_response.json` & `pykechain-4.9.0/tests/cassettes/TestExceptionsLive.test_api_error_with_argument_and_response.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExceptionsLive.test_api_error_with_response.json` & `pykechain-4.9.0/tests/cassettes/TestExceptionsLive.test_api_error_with_response.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_create_expiring_download_with_content.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_create_expiring_download_with_content.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_retrieve_expiring_downloads.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_retrieve_expiring_downloads.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_save_expiring_download_content.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_save_expiring_download_content.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_update_expiring_download.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_update_expiring_download.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_upload_expiring_download.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_upload_expiring_download.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestExpiringDownloads.test_upload_wrong_content_path.json` & `pykechain-4.9.0/tests/cassettes/TestExpiringDownloads.test_upload_wrong_content_path.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_is_false.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_is_false.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_is_true.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_is_true.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_has_part_wrong_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_has_part_wrong_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_instance_edit.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_instance_edit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_instances.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_model_edit.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_model_edit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_model_edit_with_instances.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_model_edit_with_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_retrieve_by_name_from_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_retrieve_by_name_from_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope_wrong_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_form_workflow_compatible_within_scope_wrong_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_forms_delete.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_forms_delete.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_forms_retrieve_by_context_from_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_forms_retrieve_by_context_from_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_forms_retrieve_instances_by_model_from_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_forms_retrieve_instances_by_model_from_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_cross_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_cross_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_no_target_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_no_target_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_clone_same_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_clone_same_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_client.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_client.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestForms.test_model_form_instantiation_from_wrong_scope.json` & `pykechain-4.9.0/tests/cassettes/TestForms.test_model_form_instantiation_from_wrong_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_delete_forms.json` & `pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_delete_forms.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_delete_forms_with_wrong_input.json` & `pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_delete_forms_with_wrong_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsBulk.test_bulk_instantiate_forms.json` & `pykechain-4.9.0/tests/cassettes/TestFormsBulk.test_bulk_instantiate_forms.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_apply_transition.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_apply_transition.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_apply_transition_with_wrong_input.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_apply_transition_with_wrong_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_instance.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_model.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_link_contexts_to_form_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_retrieve_possible_transitions.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_retrieve_possible_transitions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_format.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_format.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_input.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_set_status_assignees_with_wrong_input.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_instance.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_model.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_contexts_to_form_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsMethods.test_unlink_non_connected_contexts_from_form.json` & `pykechain-4.9.0/tests/cassettes/TestFormsMethods.test_unlink_non_connected_contexts_from_form.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_can_be_set.json` & `pykechain-4.9.0/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_can_be_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_with_wrong_payload.json` & `pykechain-4.9.0/tests/cassettes/TestFormsPreFillPartMethods.test_form_prefill_parts_with_wrong_payload.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGeocoordinateRepresentation.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestGeocoordinateRepresentation.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_scope.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_url.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__auth_and_no_url.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_auth.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_auth.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_pass.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__no_pass.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__scope_id_and_no_pass.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__scope_id_and_no_pass.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_scope.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_url.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelper.test_project_raises_error__token_and_no_url.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__only_url.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__only_url.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__other_things_provided.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__other_things_provided.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_and_token.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_and_token.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_token_and_name.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use__url_token_and_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use_no_vars.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__force_env_use_no_vars.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__not_for_travis.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project__not_for_travis.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project_from_env__not_for_travis.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_get_project_from_env__not_for_travis.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestGetProjectHelperNotForTravis.test_test_get_project_with_scope_id__not_for_travis.json` & `pykechain-4.9.0/tests/cassettes/TestGetProjectHelperNotForTravis.test_test_get_project_with_scope_id__not_for_travis.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_create_with_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_create_with_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_delete_notification.json` & `pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_delete_notification.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotificationCreation.test_delete_notification_from_client.json` & `pykechain-4.9.0/tests/cassettes/TestNotificationCreation.test_delete_notification_from_client.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_all_notifications_retrieval.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_all_notifications_retrieval.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit_incorrect_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit_incorrect_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_edit_notification_clear_values.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_edit_notification_clear_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_from_user.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_from_user.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_recipient_users.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_recipient_users.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_get_team.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_get_team.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification_raise_multiple_found.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification_raise_multiple_found.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestNotifications.test_retrieve_notification_raise_not_found.json` & `pykechain-4.9.0/tests/cassettes/TestNotifications.test_retrieve_notification_raise_not_found.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartCreateModelWithProperties.test_create_model_with_properties.json` & `pykechain-4.9.0/tests/cassettes/TestPartCreateModelWithProperties.test_create_model_with_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartCreateModelWithProperties.test_create_with_invalid_properties.json` & `pykechain-4.9.0/tests/cassettes/TestPartCreateModelWithProperties.test_create_with_invalid_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_ids_with_bulk.json` & `pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_ids_with_bulk.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_names_with_bulk.json` & `pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_names_with_bulk.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_no_bulk.json` & `pykechain-4.9.0/tests/cassettes/TestPartCreateWithProperties.test_create_part_with_properties_no_bulk.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_all_children.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_all_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_after_construction.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_after_construction.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_caching.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_caching.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_child_invalid.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_child_invalid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_instances_of_a_model.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_instances_of_a_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_instances_of_an_instances_raises_notfound.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_instances_of_an_instances_raises_notfound.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_models_with_descendants_tree.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_models_with_descendants_tree.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_parts_with_descendants_tree.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_parts_with_descendants_tree.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model_without_instances_raises_notfounderror.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_model_without_instances_raises_notfounderror.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_multiplicity_model_raises_multiplefounderror.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_get_single_instance_of_a_multiplicity_model_raises_multiplefounderror.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartRetrieve.test_retrieve_parts_with_refs.json` & `pykechain-4.9.0/tests/cassettes/TestPartRetrieve.test_retrieve_parts_with_refs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_bulk_update.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_bulk_update.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_model.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_attachment.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_attachment.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_missing_property.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_missing_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartUpdate.test_with_property_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPartUpdate.test_with_property_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_add_proxy_to.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_add_proxy_to.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_add_to_wrong_categories.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_add_to_wrong_categories.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_base_comparison.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_base_comparison.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_base_hash.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_base_hash.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_clone_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_clone_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_clone_instance_with_multiplicity_violation.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_clone_instance_with_multiplicity_violation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_clone_model.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_clone_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_count_children.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_count_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_count_instances.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_count_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_model.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_model_where_parent_is_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_model_where_parent_is_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_part_where_model_is_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_part_where_model_is_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_part_where_parent_is_model.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_part_where_parent_is_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_proxy_model_where_model_is_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_proxy_model_where_model_is_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_create_proxy_model_where_parent_is_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_create_proxy_model_where_parent_is_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_clear_values.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_clear_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_instance_description.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_instance_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_instance_name.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_instance_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_edit_part_model_name.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_edit_part_model_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_kwargs_on_part_retrieval.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_kwargs_on_part_retrieval.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_add_delete_part.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_add_delete_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_html_table.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_html_table.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_get_item_invalid.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_get_item_invalid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_html_categories.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_html_categories.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_html_table.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_html_table.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_iterator.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_iterator.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_with_batch.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_with_batch.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_part_set_with_limit.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_part_set_with_limit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_catalog_model_of_proxy.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_catalog_model_of_proxy.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_children_of_part.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_children_of_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_children_of_part_with_additional_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_children_of_part_with_additional_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model_multiple.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model_multiple.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_model_unknown.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_model_unknown.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_models.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_models.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_non_existent_proxies_of_a_catalog_model_raises_error.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_non_existent_proxies_of_a_catalog_model_raises_error.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_parent_of_part.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_parent_of_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_part_multiplicity.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_part_multiplicity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_part_properties_in_a_dict.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_part_properties_in_a_dict.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_parts.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_proxy_of_instance.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_proxy_of_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_siblings_of_part.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_siblings_of_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_siblings_of_part_with_additional_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_siblings_of_part_with_additional_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_multiple.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_multiple.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_part.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_retrieve_single_unknown.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_retrieve_single_unknown.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_scope.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestParts.test_wrongly_create_model.json` & `pykechain-4.9.0/tests/cassettes/TestParts.test_wrongly_create_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsClassificationForm.test_classification_forms_exist.json` & `pykechain-4.9.0/tests/cassettes/TestPartsClassificationForm.test_classification_forms_exist.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_attachments.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_attachments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_different_categories.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_different_categories.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_model.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_internal_references_on_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_missing_target_parent_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_missing_target_parent_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_empty_name_not_include_children.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_empty_name_not_include_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_given_name_include_children.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_given_name_include_children.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_part_model_include_instances.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_part_model_include_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_target_parent_inside_tree.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_target_parent_inside_tree.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_copy_too_many_target_parent_instances.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_copy_too_many_target_parent_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_cross_scope_copy.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_cross_scope_copy.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_different_categories.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_different_categories.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_part_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_part_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsCopyMove.test_move_part_model.json` & `pykechain-4.9.0/tests/cassettes/TestPartsCopyMove.test_move_part_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsImport.test_import_parts_from_client.json` & `pykechain-4.9.0/tests/cassettes/TestPartsImport.test_import_parts_from_client.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_not_list.json` & `pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_not_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_of_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_of_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_names.json` & `pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_names.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_objects.json` & `pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_properties_using_objects.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPartsReorderProperties.test_reorder_wrong_properties.json` & `pykechain-4.9.0/tests/cassettes/TestPartsReorderProperties.test_reorder_wrong_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_instance.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_instance_to_model.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_instance_to_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_copy_property_model.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_copy_property_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_clear_values.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_clear_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_description.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_name.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_edit_property_model_unit.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_edit_property_model_unit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_get_invalid_property.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_get_invalid_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_get_property_by_name.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_get_property_by_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_get_property_by_uuid.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_get_property_by_uuid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_move_property_instance.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_move_property_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_move_property_model.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_move_property_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_part_of_property.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_part_of_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_property_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_property_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_property_description.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_property_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_property_type.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_property_type.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_property_unit.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_property_unit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties_with_kwargs.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties_with_kwargs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_properties_with_refs.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_properties_with_refs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_property.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_retrieve_property_model.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_retrieve_property_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestProperties.test_set_property.json` & `pykechain-4.9.0/tests/cassettes/TestProperties.test_set_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update.json` & `pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_manual.json` & `pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_manual.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_reset.json` & `pykechain-4.9.0/tests/cassettes/TestPropertiesUpdateProperties.test_bulk_update_reset.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertiesWithReferenceProperty.test_copy_reference_property_with_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertiesWithReferenceProperty.test_copy_reference_property_with_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_reload.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_reload.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyActivityReference.test_value_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyActivityReference.test_value_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_multiple_values.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_multiple_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_no_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_no_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_no_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_no_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyContextReference.test_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyContextReference.test_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_and_delete_property_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_and_delete_property_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_incorrect_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_incorrect_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_on_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_on_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_create_property_unknown_type.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_create_property_unknown_type.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyCreation.test_creation_of_all_property_model_types.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyCreation.test_creation_of_all_property_model_types.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_get_datetime.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_get_datetime.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_iso_formatted.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_iso_formatted.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_pending_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_pending_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_iso_string.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_iso_string.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_non_datetime.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_non_datetime.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_set_value_none.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_set_value_none.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_to_datetime.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_to_datetime.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyDateTime.test_value_via_part.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyDateTime.test_value_via_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_prefilter.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_activity_reference_property_prefilter.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_boolean_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_boolean_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_date_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_date_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_float_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_float_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_int_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_int_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_link_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_link_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_select_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_select_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_test_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_multi_test_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid_with_commas.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_filter_in_grid_with_commas.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_prefilter.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_part_reference_property_prefilter.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_scope_reference_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_scope_reference_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_single_select_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_single_select_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_text_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_text_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_user_reference_property_filter_in_grid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFilterAllPropertyTypes.test_user_reference_property_filter_in_grid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_no_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_no_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyFormReference.test_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyFormReference.test_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_add_excluded_propmodels_to_reference_property.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_add_excluded_propmodels_to_reference_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_prefilters.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_prefilters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_sorting.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_clear_sorting.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_copy_reference_property_with_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_copy_reference_property_with_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id_in_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_id_in_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part_in_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_referencing_part_in_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing_in_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_create_ref_property_wrongly_referencing_in_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_excluded_propmodel_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_excluded_propmodel_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_prefilters.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_prefilters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_sorting.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_get_sorting.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_multi_ref_choices.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_multi_ref_choices.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_excluded_propmodels_on_reference_property.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_excluded_propmodels_on_reference_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_prefilters.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_overwrite_prefilters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_referenced_part_instances.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_referenced_part_instances.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_selected_part_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_property_clear_selected_part_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_list_with_no_parts.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_list_with_no_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_a_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_parts.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_referencing_multiple_instances_using_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_retrieve_scope_id.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_retrieve_scope_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_the_wrong_way.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_the_wrong_way.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_using_uuid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_using_uuid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_with_prefilters_and_validators.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_on_reference_property_with_prefilters_and_validators.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_with_validation.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_excluded_propmodels_with_validation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_the_wrong_way.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_the_wrong_way.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_using_uuid.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_using_uuid.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_with_excluded_propmodels_and_validators.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_on_reference_property_with_excluded_propmodels_and_validators.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_tuples.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_tuples.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_validation.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_prefilters_with_validation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_name.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_property.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_set_sorting_on_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_multi_ref_gives_back_all_parts.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_multi_ref_gives_back_all_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_nothing_is_referenced.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferenceProperty.test_value_if_nothing_is_referenced.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value_using_id.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_model_value_using_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiReferencePropertyXScope.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_fail_to_set_options_on_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_fail_to_set_options_on_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_get_options_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_get_options_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_illegal_options_are_not_set.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_illegal_options_are_not_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_integrity_options_dict.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_integrity_options_dict.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_options_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_options_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_in_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_in_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_not_in_options_raises_error.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_set_value_not_in_options_raises_error.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyMultiSelectListProperty.test_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyMultiSelectListProperty.test_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_no_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_no_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_prefilters.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_prefilters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_reload.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_reload.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_set_active_switch.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_set_active_switch.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_set_columns.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_set_columns.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyScopeReference.test_value_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyScopeReference.test_value_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_fail_to_set_options_on_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_fail_to_set_options_on_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_get_options_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_get_options_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_illegal_options_are_not_set.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_illegal_options_are_not_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_integrity_options_dict.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_integrity_options_dict.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_pend_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_pend_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_options_list.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_options_list.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_value_in_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_value_in_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_set_value_not_in_options_raises_error.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_set_value_not_in_options_raises_error.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertySelectListProperty.test_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertySelectListProperty.test_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_multiple_values.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_multiple_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_no_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_no_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_no_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_no_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStatusReferences.test_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStatusReferences.test_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_description.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_validators.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_edit_property_model_validators.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_multiple_values.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_multiple_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_no_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_no_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_no_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_no_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_value_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_value_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyStoredFileReference.test_value_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyStoredFileReference.test_value_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_create.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_create.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_no_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_no_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_reload.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_reload.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_value.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyUserReference.test_value_ids.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyUserReference.test_value_ids.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test__eq__.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test__eq__.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_creation.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_creation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_format.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_format.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_parse_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_parse_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_repr.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_repr.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_validate.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_validate.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyValueFilter.test_write_options.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyValueFilter.test_write_options.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_instance.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_instance.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_model.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_add_requiredvalidator_on_model.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_with_validator_parses.json` & `pykechain-4.9.0/tests/cassettes/TestPropertyWithValidatorFromLiveServer.test_numeric_property_with_validator_parses.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_mode.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_mode.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_mode_incorrect.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_mode_incorrect.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprActivity.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprActivity.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofill.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofill.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprAutofillUser.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprAutofillUser.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprButton.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprButton.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprButton.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprButton.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprButton.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprButton.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprButton.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprButton.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprDecimalPlaces.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprDecimalPlaces.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprLinkTarget.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprLinkTarget.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_mode.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_mode.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_mode_incorrect.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_mode_incorrect.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprScope.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprScope.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationClean.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationClean.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationFromCleanToNameAndDate.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignatureRepresentationNameAndDate.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprSignificantDigits.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprSignificantDigits.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationCards.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationFromCardsToText.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprStoredFileDisplayRepresentationText.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestReprThousandsSeparator.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestReprThousandsSeparator.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_clear_project_info_edit_project.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_clear_project_info_edit_project.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_project_info.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_project_info.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope_clearing_values.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope_clearing_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_edit_scope_team.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_edit_scope_team.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_empty_project_info.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_empty_project_info.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_get_landing_page.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_get_landing_page.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_get_project_info.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_get_project_info.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_landing_page.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_landing_page.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_project_info.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_project_info.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeEdit.test_set_project_info_with_wrong_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestScopeEdit.test_set_project_info_with_wrong_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_leadmember.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_leadmember.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_manager.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_member.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_member.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_member_by_id.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_member_by_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_non_existing_member.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_non_existing_member.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_add_supervisor.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_add_supervisor.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_members.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_members.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_leadmember.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_leadmember.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_manager.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_member.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_member.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_remove_supervisor.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_remove_supervisor.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopeMembers.test_reset_members.json` & `pykechain-4.9.0/tests/cassettes/TestScopeMembers.test_reset_members.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scope_with_kwargs.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scope_with_kwargs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scope_with_refs.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scope_with_refs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_scopes.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_scopes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_single_multiple.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_single_multiple.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_retrieve_single_unknown.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_retrieve_single_unknown.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_root_properties.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_root_properties.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_scope_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_scope_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_side_bar.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_side_bar.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestScopes.test_team_property_of_scope.json` & `pykechain-4.9.0/tests/cassettes/TestScopes.test_team_property_of_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_debug_service_execution_terminate.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_debug_service_execution_terminate.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_log_of_service_execution.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_log_of_service_execution.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_properties_of_service_execution.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_properties_of_service_execution.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions_with_kwargs.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_service_executions_with_kwargs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_multiple.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_multiple.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_none.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_retrieve_single_service_execution_but_found_none.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServiceExecutions.test_service_execution_conflict.json` & `pykechain-4.9.0/tests/cassettes/TestServiceExecutions.test_service_execution_conflict.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_debug_service_execute.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_debug_service_execute.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_edit_service_clear_values.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_edit_service_clear_values.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_properties_of_service.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_properties_of_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_service_but_found_multiple.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_service_but_found_multiple.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_service_by_name.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_service_by_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services_with_kwargs.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services_with_kwargs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_services_with_refs.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_services_with_refs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_retrieve_single_service.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_retrieve_single_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_service_context.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_service_context.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServices.test_update_service.json` & `pykechain-4.9.0/tests/cassettes/TestServices.test_update_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_and_delete_service.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_and_delete_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_environment_version.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_environment_version.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_service_type.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_create_service_with_wrong_service_type.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_get_executions_of_service.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_get_executions_of_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_save_service_script.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_save_service_script.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_service_refresh_from_kechain.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_service_refresh_from_kechain.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_description.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_name.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_version.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_update_service_incorrect_version.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service_with_wrong_path.json` & `pykechain-4.9.0/tests/cassettes/TestServicesWithCustomUploadedService.test_upload_script_to_service_with_wrong_path.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_alignment.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_alignment.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_attributes_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_attributes_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_attributes_sidebar.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_attributes_sidebar.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_bulk_add_buttons.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_bulk_add_buttons.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_context_manager.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_context_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_create_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_create_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_create_button_incorrect_arguments.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_create_button_incorrect_arguments.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_delete_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_delete_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_edit_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_edit_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_get_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_get_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_insert_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_insert_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_load_buttons.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_load_buttons.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_loading_of_existing_buttons.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_loading_of_existing_buttons.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_manager.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_override_sidebar_property.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_override_sidebar_property.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_remove_button.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_remove_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_side_bar_permissions.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_side_bar_permissions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_sidebar_card_creation_inside_the_manager.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_sidebar_card_creation_inside_the_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_sidebar_card_object.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_sidebar_card_object.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestSideBar.test_singleton_manager_per_scope.json` & `pykechain-4.9.0/tests/cassettes/TestSideBar.test_singleton_manager_per_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_add_stored_file.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_add_stored_file.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_delete_stored_file.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_delete_stored_file.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_edit_name_stored_file.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_edit_name_stored_file.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_edit_stored_file_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_edit_stored_file_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_retrieve_stored_file.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_retrieve_stored_file.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestStoredFiles.test_retrieve_stored_files.json` & `pykechain-4.9.0/tests/cassettes/TestStoredFiles.test_retrieve_stored_files.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTagsActivity.test_activity_tags.json` & `pykechain-4.9.0/tests/cassettes/TestTagsActivity.test_activity_tags.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTagsActivity.test_activity_tags_may_be_emptied.json` & `pykechain-4.9.0/tests/cassettes/TestTagsActivity.test_activity_tags_may_be_emptied.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTagsScope.test_scope_tags.json` & `pykechain-4.9.0/tests/cassettes/TestTagsScope.test_scope_tags.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTagsScope.test_scope_tags_may_be_emptied.json` & `pykechain-4.9.0/tests/cassettes/TestTagsScope.test_scope_tags_may_be_emptied.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_add_and_remove_member.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_add_and_remove_member.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_add_scope_to_team.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_add_scope_to_team.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team_incorrect_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team_incorrect_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_create_team_with_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_create_team_with_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_managers_members_owners.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_managers_members_owners.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_member_with_invalid_role.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_member_with_invalid_role.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_members.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_members.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_multiple_team_raises_error.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_multiple_team_raises_error.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_team_with_known_teamname.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_team_with_known_teamname.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_single_unknown_team.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_single_unknown_team.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_retrieve_teams.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_retrieve_teams.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_team_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_team_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_team_edit.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_team_edit.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestTeams.test_team_edit_wrong_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestTeams.test_team_edit_wrong_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForCharProperties.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForFloatAreaProperties.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForIntegerAreaProperties.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUseCameraScannerInputRepresentationForTextAreaCharProperties.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForActivityReferences.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_empty_config_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_empty_config_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForPartReferences.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForScopeReferences.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForServiceReferences.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_create_with_prop.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_create_with_prop.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_get_set.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_get_set.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_set_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_set_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_unsupported_value.json` & `pykechain-4.9.0/tests/cassettes/TestUsePropertyNameRepresentationForUserReferences.test_unsupported_value.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_now_in_my_timezone.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_now_in_my_timezone.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_default_name.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_default_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_multiple_user_raises_error.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_multiple_user_raises_error.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_unknown_user.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_unknown_user.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_id.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_id.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_username.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_single_user_with_known_username.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_email.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_email.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_language.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_language.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_name.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_name.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_user_timezone.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_user_timezone.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_retrieve_users.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_retrieve_users.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestUsers.test_user_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestUsers.test_user_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_download_as_excel.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_download_as_excel.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetDownloadAsExcel.test_timezone_aware.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetDownloadAsExcel.test_timezone_aware.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_activity_has_metapanel_in_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_activity_has_metapanel_in_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_can_be_found_with_uuid_in_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_can_be_found_with_uuid_in_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_in_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_in_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_manager_creation.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_manager_creation.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widget_not_found.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widget_not_found.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManager.test_widgetmanager_has_activity_and_client.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManager.test_widgetmanager_has_activity_and_client.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_associations_using_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_associations_using_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_editable_association.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_attachment_widget_with_editable_association.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget_ke_chain_pages.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_card_widget_ke_chain_pages.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_dashboard_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_dashboard_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget_with_prefilters_and_excluded_propmodels.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_filtered_grid_widget_with_prefilters_and_excluded_propmodels.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_html_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_html_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_with_progress_settings.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_metapanel_with_progress_settings.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_multicolumn_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_multicolumn_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_notebook_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_notebook_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_progress_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_progress_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_project_info_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_project_info_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_propertygrid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_propertygrid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_scope_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_scope_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_scopemembers_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_scopemembers_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_service_card_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_service_card_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_service_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_service_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_signature_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_signature_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_super_grid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_super_grid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget_with_filters.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_add_tasks_widget_with_filters.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_create_widgets.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_create_widgets.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_all_widgets.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_all_widgets.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget_stand_alone.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_delete_widget_stand_alone.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_meta.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_meta.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_and_meta.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_and_meta.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_is_none.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_edit_widget_title_is_none.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_insert_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_insert_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_new_widget_using_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_new_widget_using_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_parent.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_parent.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_property_grid_with_associations_using_widget_manager.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_property_grid_with_associations_using_widget_manager.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_scope_widget_invalid_inputs.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_scope_widget_invalid_inputs.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerInActivity.test_widget_title.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerInActivity.test_widget_title.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetManagerWeatherWidget.test_weather_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetManagerWeatherWidget.test_weather_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_disabled_button.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_disabled_button.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_external_link.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_external_link.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_in_place.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_in_place.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_incorrect_keys.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetNavigationBarWidget.test_add_navbar_widget_incorrect_keys.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_associated_parts.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_associated_parts.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_bulk_update.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_bulk_update.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_create_widget_in_activity.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_create_widget_in_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_retrieve_widgets_in_activity.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_retrieve_widgets_in_activity.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_widget_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_widget_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgets.test_widget_meta_attribute_is_not_None.json` & `pykechain-4.9.0/tests/cassettes/TestWidgets.test_widget_meta_attribute_is_not_None.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_copy_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_copy_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_copy_widget_with_wrong_target.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_copy_widget_with_wrong_target.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsCopyMove.test_move_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsCopyMove.test_move_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget_with_editable_association.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_attachment_widget_with_editable_association.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_filtered_grid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_filtered_grid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_propertygrid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_propertygrid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_signature_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_signature_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_add_super_grid_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_add_super_grid_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWidgetsInForm.test_weather_widget.json` & `pykechain-4.9.0/tests/cassettes/TestWidgetsInForm.test_weather_widget.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_create_delete_status_and_create_delete_workflow_transition.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_create_delete_status_and_create_delete_workflow_transition.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_edit_workflow_description.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_edit_workflow_description.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_in_and_activate.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_in_and_activate.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_status_order.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_status_order.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflowMethods.test_workflow_unlink_and_link_transitions.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflowMethods.test_workflow_unlink_and_link_transitions.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_clone_workflow_in_a_scope_in_the_same_scope.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_clone_workflow_in_a_scope_in_the_same_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_clone_workflow_to_scope.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_clone_workflow_to_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_classmethod_create_workflow.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_classmethod_create_workflow.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_client_create_workflow.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_client_create_workflow.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_scope_create_workflow.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_create_a_new_workflow_using_scope_create_workflow.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_import_workflow_in_a_scope_with_import_workflow_method_on_scope.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_import_workflow_in_a_scope_with_import_workflow_method_on_scope.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_single_workflow_retrieve_on_pk.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_single_workflow_retrieve_on_pk.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/cassettes/TestWorkflows.test_workflow_attributes.json` & `pykechain-4.9.0/tests/cassettes/TestWorkflows.test_workflow_attributes.json`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/classes.py` & `pykechain-4.9.0/tests/classes.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/files/test_import_parts/Wheel.xlsx` & `pykechain-4.9.0/tests/files/test_import_parts/Wheel.xlsx`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/files/test_upload_content_to_expiring_download/test_upload_content.pdf` & `pykechain-4.9.0/tests/files/test_upload_content_to_expiring_download/test_upload_content.pdf`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/files/test_upload_image_to_attachment_property/test_upload_image.png` & `pykechain-4.9.0/tests/files/test_upload_image_to_attachment_property/test_upload_image.png`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/files/test_upload_script_to_service/test_upload_script.py` & `pykechain-4.9.0/tests/files/test_upload_script_to_service/test_upload_script.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_base.py` & `pykechain-4.9.0/tests/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_property_attachment.py` & `pykechain-4.9.0/tests/models/test_property_attachment.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_property_datetime.py` & `pykechain-4.9.0/tests/models/test_property_datetime.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_property_reference.py` & `pykechain-4.9.0/tests/models/test_property_reference.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_property_selectlist.py` & `pykechain-4.9.0/tests/models/test_property_selectlist.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_representations.py` & `pykechain-4.9.0/tests/models/test_representations.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/models/test_validators.py` & `pykechain-4.9.0/tests/models/test_validators.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_about.py` & `pykechain-4.9.0/tests/test_about.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_activities.py` & `pykechain-4.9.0/tests/test_activities.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_associations.py` & `pykechain-4.9.0/tests/test_associations.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_banners.py` & `pykechain-4.9.0/tests/test_banners.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_client.py` & `pykechain-4.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_contexts.py` & `pykechain-4.9.0/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_exceptions.py` & `pykechain-4.9.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_expiring_downloads.py` & `pykechain-4.9.0/tests/test_expiring_downloads.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_forms.py` & `pykechain-4.9.0/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_helpers.py` & `pykechain-4.9.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_notifications.py` & `pykechain-4.9.0/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts.py` & `pykechain-4.9.0/tests/test_parts.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_copy_move.py` & `pykechain-4.9.0/tests/test_parts_copy_move.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_create_with_properties.py` & `pykechain-4.9.0/tests/test_parts_create_with_properties.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_import.py` & `pykechain-4.9.0/tests/test_parts_import.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_reorder_properties.py` & `pykechain-4.9.0/tests/test_parts_reorder_properties.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_retrieve.py` & `pykechain-4.9.0/tests/test_parts_retrieve.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_parts_update.py` & `pykechain-4.9.0/tests/test_parts_update.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_properties.py` & `pykechain-4.9.0/tests/test_properties.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_property_value_filter.py` & `pykechain-4.9.0/tests/test_property_value_filter.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_retry.py` & `pykechain-4.9.0/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_scope.py` & `pykechain-4.9.0/tests/test_scope.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_services.py` & `pykechain-4.9.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_sidebar.py` & `pykechain-4.9.0/tests/test_sidebar.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_stored_file.py` & `pykechain-4.9.0/tests/test_stored_file.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_tags.py` & `pykechain-4.9.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_teams.py` & `pykechain-4.9.0/tests/test_teams.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_users.py` & `pykechain-4.9.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_utils.py` & `pykechain-4.9.0/tests/test_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 from unittest import TestCase
 
-from pykechain.utils import Empty, get_in_chunks, is_url, is_valid_email
+from pykechain.utils import (
+    Empty,
+    get_in_chunks,
+    get_offset_from_user_timezone,
+    get_timezone_from_user,
+    is_url,
+    is_valid_email
+)
+from tests.classes import TestBetamax
 
 
 class TestIsURL(TestCase):
     def test_is_url_returns_true_on_valid_url(self):
         addresses = [
             "http://foobar.dk",
             "http://foobar.museum/foobar",
@@ -179,7 +187,27 @@
 
         import types
 
         self.assertIsInstance(chunks, types.GeneratorType)
 
         chunks_list = list(chunks)
         self.assertEqual(9, len(chunks_list))
+
+
+class TestTimezoneHelperFunctions(TestBetamax):
+    def setUp(self):
+        super().setUp()
+
+        self.user_with_timezone = self.client.user("testlead")
+        self.user_without_timezone = self.client.user("radu.test")
+
+    def test_retrieve_offset_from_user_timezone(self):
+        offset = get_offset_from_user_timezone(user=self.user_with_timezone)
+        self.assertEqual(offset, -600)
+
+    def test_retrieve_timezone_from_user(self):
+        timezone = get_timezone_from_user(user=self.user_with_timezone)
+        self.assertEqual(str(timezone), "Pacific/Guam")
+
+    def test_retrieve_timezone_from_user_without_timezone(self):
+        timezone = get_timezone_from_user(user=self.user_without_timezone)
+        self.assertEqual(str(timezone), "UTC")
```

### Comparing `pykechain-4.8.1/tests/test_widgets.py` & `pykechain-4.9.0/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/test_workflows.py` & `pykechain-4.9.0/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tests/utils.py` & `pykechain-4.9.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pykechain-4.8.1/tox.ini` & `pykechain-4.9.0/tox.ini`

 * *Files identical despite different names*

