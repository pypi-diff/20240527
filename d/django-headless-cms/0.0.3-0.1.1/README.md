# Comparing `tmp/django_headless_cms-0.0.3.tar.gz` & `tmp/django_headless_cms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "django_headless_cms-0.1.1.tar", max compression
```

## Comparing `django_headless_cms-0.0.3.tar` & `django_headless_cms-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,75 @@
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/requirements-tests.txt
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/requirements.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/docs/Makefile
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/docs/conf.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/docs/make.bat
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/docs/requirements.txt
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/admin.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/forms.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/models.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/serializers.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/settings.py
--rw-r--r--   0        0        0     5891 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/widgets.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/auto_translate/__init__.py
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/auto_translate/base_translate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/__init__.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/admin/change_form.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/reversion/object_history.html
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/enhances/templates/reversion/revision_form.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/fields/__init__.py
--rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/fields/boolean_field.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/fields/martor_field.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/schema/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/schema/auto_schema.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/schema/preprocessing_hooks.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/schema/urls.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/schema/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/utils/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/headless_cms/utils/martor_custom_upload.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/LICENSE
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/README.md
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 django_headless_cms-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/LICENSE
+-rw-r--r--   0        0        0      925 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/__init__.py
+-rw-r--r--   0        0        0    14062 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/admin.py
+-rw-r--r--   0        0        0       71 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/__init__.py
+-rw-r--r--   0        0        0     4029 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/base_translate.py
+-rw-r--r--   0        0        0     3617 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/auto_translate/openai_translate.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/__init__.py
+-rw-r--r--   0        0        0      376 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/admin.py
+-rw-r--r--   0        0        0     9496 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/migrations/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_metadata/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/__init__.py
+-rw-r--r--   0        0        0      365 2024-05-27 17:44:44.410931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/admin.py
+-rw-r--r--   0        0        0    11108 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0001_initial.py
+-rw-r--r--   0        0        0    12374 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/0002_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/migrations/__init__.py
+-rw-r--r--   0        0        0     6212 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/models.py
+-rw-r--r--   0        0        0     1327 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_pages/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/admin.py
+-rw-r--r--   0        0        0    10936 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/migrations/__init__.py
+-rw-r--r--   0        0        0     2413 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/models.py
+-rw-r--r--   0        0        0      638 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/serializers.py
+-rw-r--r--   0        0        0      369 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/urls.py
+-rw-r--r--   0        0        0     2093 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_posts/views.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/__init__.py
+-rw-r--r--   0        0        0     1859 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/admin.py
+-rw-r--r--   0        0        0    75728 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/migrations/__init__.py
+-rw-r--r--   0        0        0    15115 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/astrowind_widgets/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/shared/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/shared/serializers.py
+-rw-r--r--   0        0        0      736 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/contrib/astrowind/urls.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     2558 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/clean_outdated_drafts.py
+-rw-r--r--   0        0        0     3912 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/export_cms_data.py
+-rw-r--r--   0        0        0     5165 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/core/management/commands/import_cms_data.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/__init__.py
+-rw-r--r--   0        0        0     3003 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/static/localized_fields/localized-fields-admin.js
+-rw-r--r--   0        0        0     1633 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/admin/change_form.html
+-rw-r--r--   0        0        0       67 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/adminsortable2/edit_inline/stacked-django-5.0.html
+-rw-r--r--   0        0        0       67 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/adminsortable2/edit_inline/tabular-django-5.0.html
+-rw-r--r--   0        0        0      689 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html
+-rw-r--r--   0        0        0     2115 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/object_history.html
+-rw-r--r--   0        0        0     1245 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/revision_form.html
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/boolean_field.py
+-rw-r--r--   0        0        0      559 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/martor_field.py
+-rw-r--r--   0        0        0      753 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/slug_field.py
+-rw-r--r--   0        0        0       89 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/fields/url_field.py
+-rw-r--r--   0        0        0      452 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/forms.py
+-rw-r--r--   0        0        0      302 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/mixins.py
+-rw-r--r--   0        0        0     7213 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/models.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/__init__.py
+-rw-r--r--   0        0        0      490 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/auto_schema.py
+-rw-r--r--   0        0        0      314 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/preprocessing_hooks.py
+-rw-r--r--   0        0        0      831 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/urls.py
+-rw-r--r--   0        0        0      285 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/schema/views.py
+-rw-r--r--   0        0        0      883 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/serializer_fields.py
+-rw-r--r--   0        0        0     5802 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/serializers.py
+-rw-r--r--   0        0        0     1028 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/settings.py
+-rw-r--r--   0        0        0        0 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/__init__.py
+-rw-r--r--   0        0        0     1954 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/custom_import_export.py
+-rw-r--r--   0        0        0     1003 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/markdown.py
+-rw-r--r--   0        0        0     2033 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/martor_custom_upload.py
+-rw-r--r--   0        0        0     2449 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/utils/relations.py
+-rw-r--r--   0        0        0     5424 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/headless_cms/widgets.py
+-rw-r--r--   0        0        0     3909 2024-05-27 17:44:44.414931 django_headless_cms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4673 1970-01-01 00:00:00.000000 django_headless_cms-0.1.1/PKG-INFO
```

### Comparing `django_headless_cms-0.0.3/headless_cms/forms.py` & `django_headless_cms-0.1.1/headless_cms/fields/martor_field.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from localized_fields.forms import LocalizedFieldForm
+from localized_fields.fields import LocalizedField
 from localized_fields.value import LocalizedStringValue
-from martor.fields import MartorFormField
 
-from .widgets import LocalizedMartorWidget
+from ..forms import LocalizedMartorForm
+from ..widgets import AdminLocalizedMartorWidget
 
 
-class _LocalizedMartorField(LocalizedFieldForm):
-    def __init__(self, *args, required: bool | list[str] = False, **kwargs):
-        kwargs.pop("label", None)
-        super().__init__(*args, required=required, **kwargs)
+class LocalizedMartorField(LocalizedField):
+    attr_class = LocalizedStringValue
 
+    def formfield(self, **kwargs):
+        kwargs.pop("widget", None)
 
-class LocalizedMartorForm(LocalizedFieldForm):
-    """Form for a localized integer field, allows editing the field in multiple
-    languages."""
+        defaults = {
+            "form_class": LocalizedMartorForm,
+            "widget": AdminLocalizedMartorWidget,
+        }
 
-    widget = LocalizedMartorWidget
-    field_class = MartorFormField
-    value_class = LocalizedStringValue
+        defaults.update(kwargs)
+        return super().formfield(**defaults)
```

### Comparing `django_headless_cms-0.0.3/headless_cms/widgets.py` & `django_headless_cms-0.1.1/headless_cms/widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 
 class LocalizedMartorWidget(LocalizedFieldWidget):
     widget = MartorWidget
 
 
 class AdminLocalizedMartorWidget(AdminLocalizedFieldWidget):
     widget = AdminMartorWidget
-    localized_template_name = "custom_localized_fields/admin/widget.html"
-    template_name = "django/forms/widgets/textarea.html"
+    template_name = "custom_localized_fields/admin/widget.html"
 
     def markdown_render(self, name, value, attrs=None, renderer=None, **kwargs):
         random_string = "".join(
             random.choice(string.ascii_letters + string.digits) for x in range(10)
         )
         attrs["id"] = attrs["id"] + "-" + random_string
 
@@ -60,15 +59,15 @@
         attributes_to_pass.update(attrs)
 
         # Update and overwrite with any attributes that are on the widget
         # itself. This is also the only way we can push something in without
         # being part of the render chain.
         attributes_to_pass.update(self.attrs)
 
-        template = get_template("martor/%s/editor.html" % get_theme())
+        template = get_template(f"martor/{get_theme()}/editor.html")
         emoji_enabled = MARTOR_ENABLE_CONFIGS.get("emoji") == "true"
         mentions_enabled = MARTOR_ENABLE_CONFIGS.get("mention") == "true"
 
         widget = Textarea(attrs=attributes_to_pass)
         widget = widget.render(name, value)
 
         res = template.render(
@@ -80,39 +79,26 @@
                 "toolbar_buttons": MARTOR_TOOLBAR_BUTTONS,
             }
         )
         return res
 
     def render(self, name, value, attrs=None, renderer=None):
         context = self.get_context(name, value, attrs)
-        widgets = context["widget"]["subwidgets"]
-        for widget in widgets:
-            w_attrs = widget["attrs"]
-            md = self.markdown_render(
-                widget["name"],
-                widget["value"],
-                {
-                    "required": w_attrs["required"],
-                    "id": w_attrs["id"],
-                    "cols": "40",
-                    "rows": "10",
-                },
-            )
-            widget["martor"] = md
-        template = get_template(self.localized_template_name)
-        res = template.render(context)
-        return res
+        widget = context["widget"]
+        md = self.markdown_render(widget["name"], "", attrs)
+        context["widget"]["md"] = md
+        return self._render(self.template_name, context, renderer)
 
     class Media:
         selected_theme = get_theme()
         css = {
             "all": (
                 "plugins/css/ace.min.css",
                 "plugins/css/resizable.min.css",
-                "martor/css/martor.%s.min.css" % selected_theme,
+                f"martor/css/martor.{selected_theme}.min.css",
             )
         }
 
         if MARTOR_ENABLE_ADMIN_CSS:
             admin_theme = ("martor/css/martor-admin.min.css",)
             css["all"] = admin_theme.__add__(css.get("all"))
 
@@ -120,38 +106,38 @@
             "plugins/js/ace.js",
             "plugins/js/mode-markdown.js",
             "plugins/js/ext-language_tools.js",
             "plugins/js/theme-github.js",
             "plugins/js/highlight.min.js",
             "plugins/js/resizable.min.js",
             "plugins/js/emojis.min.js",
-            "martor/js/martor.%s.js" % selected_theme,
+            f"martor/js/martor.{selected_theme}.js",
         )
 
         # Adding the following scripts to the end
         # of the tuple in case it affects behaviour.
         # spellcheck configuration
         if MARTOR_ENABLE_CONFIGS.get("spellcheck") == "true":
             js = ("plugins/js/typo.js", "plugins/js/spellcheck.js").__add__(js)
 
         # support alternative vendor theme file like: bootstrap, semantic)
         # 1. vendor css theme
         if MARTOR_ALTERNATIVE_CSS_FILE_THEME:
             css_theme = MARTOR_ALTERNATIVE_CSS_FILE_THEME
             css["all"] = (css_theme,).__add__(css.get("all"))
         else:
-            css_theme = "plugins/css/%s.min.css" % selected_theme
+            css_theme = f"plugins/css/{selected_theme}.min.css"
             css["all"] = (css_theme,).__add__(css.get("all"))
 
         # 2. vendor js theme
         if MARTOR_ALTERNATIVE_JS_FILE_THEME:
             js_theme = MARTOR_ALTERNATIVE_JS_FILE_THEME
             js = (MARTOR_ALTERNATIVE_JS_FILE_THEME,).__add__(js)
         else:
-            js_theme = "plugins/js/%s.min.js" % selected_theme
+            js_theme = f"plugins/js/{selected_theme}.min.js"
             js = (js_theme,).__add__(js)
 
         # 3. vendor jQUery
         if MARTOR_ALTERNATIVE_JQUERY_JS_FILE:
             js = (MARTOR_ALTERNATIVE_JQUERY_JS_FILE,).__add__(js)
         elif MARTOR_ENABLE_CONFIGS.get("jquery") == "true":
             js = ("plugins/js/jquery.min.js",).__add__(js)
```

### Comparing `django_headless_cms-0.0.3/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html` & `django_headless_cms-0.1.1/headless_cms/enhances/templates/custom_localized_fields/admin/widget.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,17 @@
     <ul class="localized-fields-widget tabs">
     {% for widget in widget.subwidgets %}
         <li class="localized-fields-widget tab">
             <label for="{{ widget_id }}_{{ widget.lang_code }}">{{ widget.lang_name|capfirst }}</label>
         </li>
     {% endfor %}
     </ul>
+{{ widget.md }}
 {% for widget in widget.subwidgets %}
     <div class="localized-panel" role="tabpanel" id="{{ widget_id }}_{{ widget.lang_code }}">
-        {% autoescape off %}
-            {{ widget.martor }}
-        {% endautoescape %}
+        <div style="display: none;">
+            {% include widget.template_name %}
+        </div>
     </div>
 {% endfor %}
 </div>
 {% endwith %}
```

### Comparing `django_headless_cms-0.0.3/headless_cms/enhances/templates/reversion/object_history.html` & `django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/object_history.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.0.3/headless_cms/enhances/templates/reversion/revision_form.html` & `django_headless_cms-0.1.1/headless_cms/enhances/templates/reversion/revision_form.html`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.0.3/headless_cms/fields/boolean_field.py` & `django_headless_cms-0.1.1/headless_cms/fields/boolean_field.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.0.3/headless_cms/utils/martor_custom_upload.py` & `django_headless_cms-0.1.1/headless_cms/utils/martor_custom_upload.py`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.0.3/LICENSE` & `django_headless_cms-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_headless_cms-0.0.3/README.md` & `django_headless_cms-0.1.1/README.md`

 * *Files identical despite different names*

