# Comparing `tmp/django_pony_express-2.0.0.tar.gz` & `tmp/django_pony_express-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pony_express-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pony_express-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pony_express-2.0.0.tar` & `django_pony_express-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,53 @@
--rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-2.0.0/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0      320 2024-04-11 14:12:18.255023 django_pony_express-2.0.0/.coveragerc
--rw-r--r--   0        0        0      288 2024-04-11 14:12:18.256031 django_pony_express-2.0.0/.editorconfig
--rw-r--r--   0        0        0     2213 2024-04-11 14:16:18.950523 django_pony_express-2.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-2.0.0/.gitignore
--rw-r--r--   0        0        0      668 2024-04-11 14:16:18.950523 django_pony_express-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      773 2024-04-11 14:12:18.259031 django_pony_express-2.0.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1652 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/CHANGES.md
--rw-r--r--   0        0        0    71412 2024-04-11 14:12:18.291569 django_pony_express-2.0.0/LICENSE.md
--rw-r--r--   0        0        0      138 2024-04-11 14:12:18.260033 django_pony_express-2.0.0/MANIFEST.in
--rw-r--r--   0        0        0     6287 2024-04-11 14:12:18.272133 django_pony_express-2.0.0/README.md
--rw-r--r--   0        0        0       85 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/django_pony_express/__init__.py
--rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/errors.py
--rw-r--r--   0        0        0     1564 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11100 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/base.py
--rw-r--r--   0        0        0     9771 2023-12-04 15:24:45.663888 django_pony_express-2.0.0/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      654 2024-04-11 14:12:18.279570 django_pony_express-2.0.0/docs/Makefile
--rw-r--r--   0        0        0     2825 2024-04-11 14:16:18.951515 django_pony_express-2.0.0/docs/conf.py
--rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/changelog.rst
--rw-r--r--   0        0        0     9438 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/mail.md
--rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/features/tests.md
--rw-r--r--   0        0        0      264 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/docs/index.rst
--rwxr-xr-x   0        0        0      795 2024-04-11 14:12:18.278560 django_pony_express-2.0.0/docs/make.bat
--rw-r--r--   0        0        0      679 2024-04-11 14:16:18.952522 django_pony_express-2.0.0/manage.py
--rw-r--r--   0        0        0     5402 2024-04-11 14:16:18.952522 django_pony_express-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      121 2024-04-11 14:12:18.281561 django_pony_express-2.0.0/scripts/unix/install_requirements.sh
--rw-r--r--   0        0        0       50 2024-04-11 14:12:18.282568 django_pony_express-2.0.0/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      121 2024-04-11 14:12:18.284573 django_pony_express-2.0.0/scripts/windows/install_requirements.ps1
--rw-r--r--   0        0        0       50 2024-04-11 14:12:18.285570 django_pony_express-2.0.0/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0     1620 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/settings.py
--rw-r--r--   0        0        0      289 2024-04-11 14:12:18.273137 django_pony_express-2.0.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/testapp/__init__.py
--rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-2.0.0/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/files/testfile.txt
--rw-r--r--   0        0        0     9340 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15224 2023-12-04 15:24:45.670166 django_pony_express-2.0.0/tests/test_mail_services.py
--rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 django_pony_express-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2602 2023-12-04 15:24:45.657869 django_pony_express-2.1.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0      320 2024-04-11 14:12:18.255023 django_pony_express-2.1.0/.coveragerc
+-rw-r--r--   0        0        0      288 2024-04-11 14:12:18.256031 django_pony_express-2.1.0/.editorconfig
+-rw-r--r--   0        0        0     2213 2024-04-11 14:16:18.950523 django_pony_express-2.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3137 2023-12-04 15:24:45.661871 django_pony_express-2.1.0/.gitignore
+-rw-r--r--   0        0        0      668 2024-04-11 14:16:18.950523 django_pony_express-2.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      773 2024-04-11 14:12:18.259031 django_pony_express-2.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1901 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/CHANGES.md
+-rw-r--r--   0        0        0    71412 2024-04-11 14:12:18.291569 django_pony_express-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0      138 2024-04-11 14:12:18.260033 django_pony_express-2.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     6287 2024-04-11 14:12:18.272133 django_pony_express-2.1.0/README.md
+-rw-r--r--   0        0        0       85 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      114 2023-12-04 15:24:45.663888 django_pony_express-2.1.0/django_pony_express/errors.py
+-rw-r--r--   0        0        0     2327 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.663888 django_pony_express-2.1.0/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/asynchronous/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/asynchronous/thread.py
+-rw-r--r--   0        0        0    12801 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10179 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      229 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/django_pony_express/settings.py
+-rw-r--r--   0        0        0      654 2024-04-11 14:12:18.279570 django_pony_express-2.1.0/docs/Makefile
+-rw-r--r--   0        0        0     2825 2024-04-11 14:16:18.951515 django_pony_express-2.1.0/docs/conf.py
+-rw-r--r--   0        0        0       32 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0     1480 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/configuration.md
+-rw-r--r--   0        0        0     2789 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/factories.md
+-rw-r--r--   0        0        0     2750 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/internal_api.md
+-rw-r--r--   0        0        0     4588 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/features/introduction.md
+-rw-r--r--   0        0        0     4912 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/docs/features/tests.md
+-rw-r--r--   0        0        0      375 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2024-04-11 14:12:18.278560 django_pony_express-2.1.0/docs/make.bat
+-rw-r--r--   0        0        0      679 2024-04-11 14:16:18.952522 django_pony_express-2.1.0/manage.py
+-rw-r--r--   0        0        0     5402 2024-04-11 14:16:18.952522 django_pony_express-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.281561 django_pony_express-2.1.0/scripts/unix/install_requirements.sh
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.282568 django_pony_express-2.1.0/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      121 2024-04-11 14:12:18.284573 django_pony_express-2.1.0/scripts/windows/install_requirements.ps1
+-rw-r--r--   0        0        0       50 2024-04-11 14:12:18.285570 django_pony_express-2.1.0/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0     1761 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/settings.py
+-rw-r--r--   0        0        0      289 2024-04-11 14:12:18.273137 django_pony_express-2.1.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/testapp/__init__.py
+-rw-r--r--   0        0        0      134 2023-12-04 15:24:45.665922 django_pony_express-2.1.0/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      145 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      137 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       27 2023-12-04 15:24:45.670166 django_pony_express-2.1.0/tests/files/testfile.txt
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/asynchronous/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/asynchronous/test_thread_email.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/__init__.py
+-rw-r--r--   0        0        0     3425 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/test_base_mail_factory.py
+-rw-r--r--   0        0        0    15473 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/base/test_base_mail_service.py
+-rw-r--r--   0        0        0        0 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/tests/__init__.py
+-rw-r--r--   0        0        0     9609 2024-05-27 15:19:31.530860 django_pony_express-2.1.0/tests/services/tests/test_email_test_service.py
+-rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 django_pony_express-2.1.0/PKG-INFO
```

### Comparing `django_pony_express-2.0.0/.ambient-package-update/metadata.py` & `django_pony_express-2.1.0/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/.github/workflows/ci.yml` & `django_pony_express-2.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/.gitignore` & `django_pony_express-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/.pre-commit-config.yaml` & `django_pony_express-2.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/.readthedocs.yaml` & `django_pony_express-2.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/CHANGES.md` & `django_pony_express-2.1.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+* *2.1.0* (2024-05-27)
+  * Added `ThreadEmailService` for simple async sending of emails
+  * Added basic logging with privacy configuration to mail class
+  * Restructured documentation
+  * Restructured unit-tests
+  * Minor test improvements
+
 * *2.0.0* (2024-04-11)
   * Dropped Django 3.2 & 4.1 support (via `ambient-package-update`)
   * Internal updates via `ambient-package-update`
 
 * *1.3.0** (2023-12-04)
   * Added Django 5.0 support
```

### Comparing `django_pony_express-2.0.0/LICENSE.md` & `django_pony_express-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/README.md` & `django_pony_express-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/django_pony_express/locale/de/LC_MESSAGES/django.po` & `django_pony_express-2.1.0/django_pony_express/locale/de/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,63 @@
-# SOME DESCRIPTIVE TITLE.
-# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
-# This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
-msgid ""
-msgstr ""
-"Project-Id-Version: PACKAGE VERSION\n"
-"Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-05-03 15:32+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
-"MIME-Version: 1.0\n"
-"Content-Type: text/plain; charset=UTF-8\n"
-"Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
-
-#: .\django_pony_express\services\base.py:42
-msgid "Email factory requires a mail service class."
-msgstr "E-Mailfactory benötigt eine Mailservice-Klasse."
-
-#: .\django_pony_express\services\base.py:44
-msgid "Email factory requires a target mail address."
-msgstr "E-Mailfactory benötigt eine Ziel-Mailadresse."
-
-#: .\django_pony_express\services\base.py:212
-msgid "Missing or mislabeled data provided for email attachment."
-msgstr "Fehlende oder falsch deklarierte Daten für E-Mailanhänge übergeben."
-
-#: .\django_pony_express\services\base.py:269
-msgid "Email service requires a subject."
-msgstr "E-Mailservice benötigt einen Betreff."
-
-#: .\django_pony_express\services\base.py:271
-msgid "Email service requires a template."
-msgstr "E-Mailservice benötigt ein Template."
-
-#: .\django_pony_express\services\base.py:273
-msgid "Email service requires a target mail address."
-msgstr "E-Mailservice benötigt eine Ziel-Mailadresse."
+# SOME DESCRIPTIVE TITLE.
+# Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
+# This file is distributed under the same license as the PACKAGE package.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
+msgid ""
+msgstr ""
+"Project-Id-Version: PACKAGE VERSION\n"
+"Report-Msgid-Bugs-To: \n"
+"POT-Creation-Date: 2024-05-27 17:11+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
+"MIME-Version: 1.0\n"
+"Content-Type: text/plain; charset=UTF-8\n"
+"Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+
+#: .\django_pony_express\services\base.py:44
+msgid "Email factory requires a mail service class."
+msgstr "E-Mailfactory benötigt eine Mailservice-Klasse."
+
+#: .\django_pony_express\services\base.py:46
+msgid "Email factory requires a target mail address."
+msgstr "E-Mailfactory benötigt eine Ziel-Mailadresse."
+
+#: .\django_pony_express\services\base.py:225
+msgid "Missing or mislabeled data provided for email attachment."
+msgstr "Fehlende oder falsch deklarierte Daten für E-Mailanhänge übergeben."
+
+#: .\django_pony_express\services\base.py:282
+msgid "Email service requires a subject."
+msgstr "E-Mailservice benötigt einen Betreff."
+
+#: .\django_pony_express\services\base.py:284
+msgid "Email service requires a template."
+msgstr "E-Mailservice benötigt ein Template."
+
+#: .\django_pony_express\services\base.py:286
+msgid "Email service requires a target mail address."
+msgstr "E-Mailservice benötigt eine Ziel-Mailadresse."
+
+#: .\django_pony_express\services\base.py:316
+#, python-format
+msgid "Email \"%s\" successfully sent to %s."
+msgstr "E-Mail \"%s\" erfolgreich versendet an %s."
+
+#: .\django_pony_express\services\base.py:318
+#, python-format
+msgid "Email \"%s\" successfully sent."
+msgstr "E-Mail \"%s\" erfolgreich versendet."
+
+#: .\django_pony_express\services\base.py:322
+#, python-format
+msgid "An error occurred sending email \"%s\" to %s: %s"
+msgstr "Beim Versenden der E-Mail \"%s\" an %s ist ein Fehler aufgetreten: %s"
+
+#: .\django_pony_express\services\base.py:325
+#, python-format
+msgid "An error occurred sending email \"%s\": %s"
+msgstr "Beim Versenden der E-Mail \"%s\" ist ein Fehler aufgetreten: %s"
```

### Comparing `django_pony_express-2.0.0/django_pony_express/services/base.py` & `django_pony_express-2.1.0/django_pony_express/services/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,309 +1,339 @@
-from typing import Union
-
-import html2text
-from django.conf import settings
-from django.core.mail import EmailMultiAlternatives
-from django.db.models import QuerySet
-from django.template.loader import render_to_string
-from django.utils import translation
-from django.utils.translation import gettext_lazy as _
-
-from ..errors import EmailServiceAttachmentError, EmailServiceConfigError
-
-
-class BaseEmailServiceFactory:
-    """
-    Factory for creating emails of the same type but with recipient-dependent content.
-    """
-
-    _errors = []
-
-    service_class = None
-    recipient_email_list = []
-
-    def __init__(self, recipient_email_list: Union[list, tuple, QuerySet] = None, **kwargs) -> None:
-        """
-        Initialisation takes optionally a list of recipients. Doesn't have to be a list of strings because
-        fetching the actual email from a complex data structure can be done in the method `get_email_from_recipient()`
-        """
-        # Empty error list on initialisation
-        self._errors = []
-
-        super().__init__()
-        if recipient_email_list:
-            self.recipient_email_list = recipient_email_list
-
-    def is_valid(self, raise_exception: bool = True) -> bool:
-        """
-        This function ensures that all required variables for the email object are set. Can be overridden and extended
-        but again, make sure that super() is called
-        """
-        if not self.service_class:
-            self._errors.append(_("Email factory requires a mail service class."))
-        if not len(self.get_recipient_list()):
-            self._errors.append(_("Email factory requires a target mail address."))
-
-        if self._errors and raise_exception:
-            raise EmailServiceConfigError(self._errors)
-
-        return not bool(len(self._errors))
-
-    def get_recipient_list(self) -> list:
-        """
-        Fetches the recipient list. Provided as a method to be able to customise it in the derived class.
-        """
-        return self.recipient_email_list
-
-    def get_email_from_recipient(self, recipient) -> str:
-        """
-        Fetches the email from the recipient. Sometimes a list of mail addresses is passed, so we just have to
-        return the current variable. But if we get a database object, we need to extract the email first.
-        For example: `return user.email`
-        """
-        return recipient
-
-    def get_context_data(self) -> dict:
-        """
-        Fetch context data required equally for every email created by the factory.
-        """
-        return {}
-
-    def has_errors(self) -> bool:
-        """
-        Check if any errors are stored inside this class instance
-        """
-        return bool(len(self._errors))
-
-    @property
-    def errors(self) -> list:
-        """
-        Getter for fetching the stored error messages.
-        Errors shall not be set manually, that's why we use a property here.
-        """
-        return self._errors
-
-    def process(self, raise_exception: bool = True) -> int:
-        """
-        Create an email of `self.service_class` for every recipient. Per-email logic like setting the salutation
-        is handled within each email class.
-        Returns the number of sent emails.
-        """
-        counter = 0
-        if self.is_valid(raise_exception=raise_exception):
-            for recipient in self.get_recipient_list():
-                email_object = self.service_class(
-                    recipient_email_list=[self.get_email_from_recipient(recipient)],
-                    context_data={"recipient": recipient, **self.get_context_data()},
-                )
-                email_object.process()
-                counter += 1
-
-        return counter
-
-
-class BaseEmailService:
-    """
-    Class for wrapping all required things for email creation.
-    """
-
-    SUBJECT_PREFIX = None
-    FROM_EMAIL = None
-    REPLY_TO_ADDRESS = []
-
-    _errors = []
-
-    subject = None
-    template_name = None
-    template_txt_name = None
-    recipient_email_list = []
-    cc_email_list = []
-    bcc_email_list = []
-    attachment_list = []
-
-    def __init__(
-        self,
-        recipient_email_list: Union[list, tuple, str] = None,
-        context_data: dict = None,
-        attachment_list: list = None,
-        **kwargs,
-    ) -> None:
-        """
-        Initialisation takes a single or list of email addresses and some context data. This context data
-        might be provided from the factory to avoid querying data more than necessary.
-        """
-        # Empty error list on initialisation
-        self._errors = []
-
-        super().__init__()
-
-        # Ensure that a single email address is wrapped in a list, so we can use it in the `to` kwarg.
-        if isinstance(recipient_email_list, str):
-            recipient_email_list = [recipient_email_list]
-
-        self.recipient_email_list = recipient_email_list if recipient_email_list else []
-        self.context_data = context_data if context_data else {}
-        self.attachment_list = attachment_list if attachment_list else []
-
-    def get_context_data(self) -> dict:
-        """
-        This method provides the required variables for the base email template. If more variables are required,
-        just override this method and make sure, super() is called
-        """
-        return self.context_data
-
-    def get_subject(self) -> str:
-        """
-        This method provides the subject of the email. Prefixes every subject to create a similar look and feel across
-        emails. Can be overridden if required.
-        """
-        if self.SUBJECT_PREFIX:
-            return f"{self.SUBJECT_PREFIX} - {self.subject}"
-        return self.subject
-
-    def get_from_email(self) -> str:
-        """
-        Use set `FROM_EMAIL` or the django base `DEFAULT_FROM_EMAIL` if it is not set
-        """
-        return self.FROM_EMAIL if self.FROM_EMAIL else settings.DEFAULT_FROM_EMAIL
-
-    def get_cc_emails(self) -> list:
-        """
-        Returns a list of emails as a string which will be used in the "CC" field of the generated email.
-        """
-        return self.cc_email_list
-
-    def get_bcc_emails(self) -> list:
-        """
-        Returns a list of emails as a string which will be used in the "BCC" field of the generated email.
-        """
-        return self.bcc_email_list
-
-    def get_reply_to_emails(self) -> list:
-        """
-        Ensure "reply to" is a list
-        """
-        return [self.REPLY_TO_ADDRESS] if isinstance(self.REPLY_TO_ADDRESS, str) else self.REPLY_TO_ADDRESS
-
-    def get_translation(self) -> Union[str, None]:
-        """
-        Tries to fetch the current translation from the django settings.
-        """
-        language_str_length = 2
-        try:
-            return (
-                settings.LANGUAGE_CODE[:2]
-                if settings.LANGUAGE_CODE and len(settings.LANGUAGE_CODE) >= language_str_length
-                else None
-            )
-        except TypeError:
-            return None
-
-    def get_attachments(self) -> list:
-        """
-        Method to be overwritten. Returns a list of file-paths which will be attached to the newly created email.
-        """
-        return self.attachment_list
-
-    def _add_attachments(self, msg: EmailMultiAlternatives):
-        """
-        Method to encapsulate logic of adding attachments to an email object.
-        """
-        for attachment in self.get_attachments():
-            if isinstance(attachment, dict):
-                try:
-                    msg.attach(attachment["filename"], attachment["file"], attachment.get("mimetype", None))
-                except KeyError as e:
-                    raise EmailServiceAttachmentError(
-                        _("Missing or mislabeled data provided for email attachment.")
-                    ) from e
-            else:
-                msg.attach_file(attachment)
-
-        return msg
-
-    def _build_mail_object(self) -> EmailMultiAlternatives:
-        """
-        This method creates a mail object. It collects the required variables, sets the subject and makes sure that
-        a "reply_to" is set for maximum convenience during the runtime.
-        The plaintext part of the email is generated from the html to avoid maintaining duplicate templates.
-        """
-        # Optionally set translation language for date formatting etc.
-        language = self.get_translation()
-        if language:
-            translation.activate(language)
-
-        # Gather variables
-        mail_attributes = self.get_context_data()
-
-        # Render HTML body content
-        html_content = render_to_string(self.template_name, mail_attributes)
-
-        # Render TXT body part if a template is explicitly set, otherwise convert HTML template to plain text
-        if not self.template_txt_name:
-            h = html2text.HTML2Text()
-            # Set body width to "infinite" to avoid weird line breaks
-            h.body_width = 0
-            text_content = h.handle(html_content)
-        else:
-            text_content = render_to_string(self.template_txt_name, mail_attributes)
-
-        # Build mail object
-        msg = EmailMultiAlternatives(
-            self.get_subject(),
-            text_content,
-            from_email=self.get_from_email(),
-            cc=self.get_cc_emails(),
-            bcc=self.get_bcc_emails(),
-            reply_to=self.get_reply_to_emails(),
-            to=self.recipient_email_list,
-        )
-        msg.attach_alternative(html_content, "text/html")
-
-        # Add attachments (if available)
-        msg = self._add_attachments(msg)
-
-        # Return mail object
-        return msg
-
-    def is_valid(self, raise_exception: bool = True) -> bool:
-        """
-        This function ensures that all required variables for the email object are set. Can be overridden and extended
-        but again, make sure that super() is called.
-        """
-        if not self.get_subject():
-            self._errors.append(_("Email service requires a subject."))
-        if not self.template_name:
-            self._errors.append(_("Email service requires a template."))
-        if not len(self.recipient_email_list):
-            self._errors.append(_("Email service requires a target mail address."))
-
-        if self._errors and raise_exception:
-            raise EmailServiceConfigError(self._errors)
-
-        return not bool(len(self._errors))
-
-    def has_errors(self) -> bool:
-        """
-        Check if any errors are stored inside this class instance
-        """
-        return bool(len(self._errors))
-
-    @property
-    def errors(self) -> list:
-        """
-        Getter for fetching the stored error messages.
-        Errors shall not be set manually, that's why we use a property here.
-        """
-        return self._errors
-
-    def process(self, raise_exception: bool = True) -> bool:
-        """
-        Public method which is called to actually send an email. Calls validation first and returns the result of
-        "msg.send()"
-        """
-        result = False
-        if self.is_valid(raise_exception=raise_exception):
-            msg = self._build_mail_object()
-            result = msg.send()
-
-        return result
+import logging
+from typing import Union
+
+import html2text
+from django.conf import settings
+from django.core.mail import EmailMultiAlternatives
+from django.db.models import QuerySet
+from django.template.loader import render_to_string
+from django.utils import translation
+from django.utils.translation import gettext_lazy as _
+
+from django_pony_express.errors import EmailServiceAttachmentError, EmailServiceConfigError
+from django_pony_express.settings import PONY_LOG_RECIPIENTS, PONY_LOGGER_NAME
+
+
+class BaseEmailServiceFactory:
+    """
+    Factory for creating emails of the same type but with recipient-dependent content.
+    """
+
+    _errors = []
+
+    service_class = None
+    recipient_email_list = []
+
+    def __init__(self, recipient_email_list: Union[list, tuple, QuerySet] = None, **kwargs) -> None:
+        """
+        Initialisation takes optionally a list of recipients. Doesn't have to be a list of strings because
+        fetching the actual email from a complex data structure can be done in the method `get_email_from_recipient()`
+        """
+        # Empty error list on initialisation
+        self._errors = []
+
+        super().__init__()
+        if recipient_email_list:
+            self.recipient_email_list = recipient_email_list
+
+    def is_valid(self, raise_exception: bool = True) -> bool:
+        """
+        This function ensures that all required variables for the email object are set. Can be overridden and extended
+        but again, make sure that super() is called
+        """
+        if not self.service_class:
+            self._errors.append(_("Email factory requires a mail service class."))
+        if not len(self.get_recipient_list()):
+            self._errors.append(_("Email factory requires a target mail address."))
+
+        if self._errors and raise_exception:
+            raise EmailServiceConfigError(self._errors)
+
+        return not bool(len(self._errors))
+
+    def get_recipient_list(self) -> list:
+        """
+        Fetches the recipient list. Provided as a method to be able to customise it in the derived class.
+        """
+        return self.recipient_email_list
+
+    def get_email_from_recipient(self, recipient) -> str:
+        """
+        Fetches the email from the recipient. Sometimes a list of mail addresses is passed, so we just have to
+        return the current variable. But if we get a database object, we need to extract the email first.
+        For example: `return user.email`
+        """
+        return recipient
+
+    def get_context_data(self) -> dict:
+        """
+        Fetch context data required equally for every email created by the factory.
+        """
+        return {}
+
+    def has_errors(self) -> bool:
+        """
+        Check if any errors are stored inside this class instance
+        """
+        return bool(len(self._errors))
+
+    @property
+    def errors(self) -> list:
+        """
+        Getter for fetching the stored error messages.
+        Errors shall not be set manually, that's why we use a property here.
+        """
+        return self._errors
+
+    def process(self, raise_exception: bool = True) -> int:
+        """
+        Create an email of `self.service_class` for every recipient. Per-email logic like setting the salutation
+        is handled within each email class.
+        Returns the number of sent emails.
+        """
+        counter = 0
+        if self.is_valid(raise_exception=raise_exception):
+            for recipient in self.get_recipient_list():
+                email_object = self.service_class(
+                    recipient_email_list=[self.get_email_from_recipient(recipient)],
+                    context_data={"recipient": recipient, **self.get_context_data()},
+                )
+                email_object.process()
+                counter += 1
+
+        return counter
+
+
+class BaseEmailService:
+    """
+    Class for wrapping all required things for email creation.
+    """
+
+    SUBJECT_PREFIX = None
+    FROM_EMAIL = None
+    REPLY_TO_ADDRESS = []
+
+    _errors = []
+    _logger: logging.Logger = None
+
+    subject = None
+    template_name = None
+    template_txt_name = None
+    recipient_email_list = []
+    cc_email_list = []
+    bcc_email_list = []
+    attachment_list = []
+
+    def __init__(
+        self,
+        recipient_email_list: Union[list, tuple, str] = None,
+        context_data: dict = None,
+        attachment_list: list = None,
+        **kwargs,
+    ) -> None:
+        """
+        Initialisation takes a single or list of email addresses and some context data. This context data
+        might be provided from the factory to avoid querying data more than necessary.
+        """
+        # Empty error list on initialisation
+        self._errors = []
+        self._logger = self._get_logger()
+
+        super().__init__()
+
+        # Ensure that a single email address is wrapped in a list, so we can use it in the `to` kwarg.
+        if isinstance(recipient_email_list, str):
+            recipient_email_list = [recipient_email_list]
+
+        self.recipient_email_list = recipient_email_list if recipient_email_list else []
+        self.context_data = context_data if context_data else {}
+        self.attachment_list = attachment_list if attachment_list else []
+
+    def _get_logger(self) -> logging.Logger:
+        self._logger = logging.getLogger(PONY_LOGGER_NAME) if self._logger is None else self._logger
+        return self._logger
+
+    def get_context_data(self) -> dict:
+        """
+        This method provides the required variables for the base email template. If more variables are required,
+        just override this method and make sure, super() is called
+        """
+        return self.context_data
+
+    def get_subject(self) -> str:
+        """
+        This method provides the subject of the email. Prefixes every subject to create a similar look and feel across
+        emails. Can be overridden if required.
+        """
+        if self.SUBJECT_PREFIX:
+            return f"{self.SUBJECT_PREFIX} - {self.subject}"
+        return self.subject
+
+    def get_from_email(self) -> str:
+        """
+        Use set `FROM_EMAIL` or the django base `DEFAULT_FROM_EMAIL` if it is not set
+        """
+        return self.FROM_EMAIL if self.FROM_EMAIL else settings.DEFAULT_FROM_EMAIL
+
+    def get_cc_emails(self) -> list:
+        """
+        Returns a list of emails as a string which will be used in the "CC" field of the generated email.
+        """
+        return self.cc_email_list
+
+    def get_bcc_emails(self) -> list:
+        """
+        Returns a list of emails as a string which will be used in the "BCC" field of the generated email.
+        """
+        return self.bcc_email_list
+
+    def get_reply_to_emails(self) -> list:
+        """
+        Ensure "reply to" is a list
+        """
+        return [self.REPLY_TO_ADDRESS] if isinstance(self.REPLY_TO_ADDRESS, str) else self.REPLY_TO_ADDRESS
+
+    def get_translation(self) -> Union[str, None]:
+        """
+        Tries to fetch the current translation from the django settings.
+        """
+        language_str_length = 2
+        try:
+            return (
+                settings.LANGUAGE_CODE[:2]
+                if settings.LANGUAGE_CODE and len(settings.LANGUAGE_CODE) >= language_str_length
+                else None
+            )
+        except TypeError:
+            return None
+
+    def get_attachments(self) -> list:
+        """
+        Method to be overwritten. Returns a list of file-paths which will be attached to the newly created email.
+        """
+        return self.attachment_list
+
+    def _add_attachments(self, msg: EmailMultiAlternatives):
+        """
+        Method to encapsulate logic of adding attachments to an email object.
+        """
+        for attachment in self.get_attachments():
+            if isinstance(attachment, dict):
+                try:
+                    msg.attach(attachment["filename"], attachment["file"], attachment.get("mimetype", None))
+                except KeyError as e:
+                    raise EmailServiceAttachmentError(
+                        _("Missing or mislabeled data provided for email attachment.")
+                    ) from e
+            else:
+                msg.attach_file(attachment)
+
+        return msg
+
+    def _build_mail_object(self) -> EmailMultiAlternatives:
+        """
+        This method creates a mail object. It collects the required variables, sets the subject and makes sure that
+        a "reply_to" is set for maximum convenience during the runtime.
+        The plaintext part of the email is generated from the html to avoid maintaining duplicate templates.
+        """
+        # Optionally set translation language for date formatting etc.
+        language = self.get_translation()
+        if language:
+            translation.activate(language)
+
+        # Gather variables
+        mail_attributes = self.get_context_data()
+
+        # Render HTML body content
+        html_content = render_to_string(self.template_name, mail_attributes)
+
+        # Render TXT body part if a template is explicitly set, otherwise convert HTML template to plain text
+        if not self.template_txt_name:
+            h = html2text.HTML2Text()
+            # Set body width to "infinite" to avoid weird line breaks
+            h.body_width = 0
+            text_content = h.handle(html_content)
+        else:
+            text_content = render_to_string(self.template_txt_name, mail_attributes)
+
+        # Build mail object
+        msg = EmailMultiAlternatives(
+            self.get_subject(),
+            text_content,
+            from_email=self.get_from_email(),
+            cc=self.get_cc_emails(),
+            bcc=self.get_bcc_emails(),
+            reply_to=self.get_reply_to_emails(),
+            to=self.recipient_email_list,
+        )
+        msg.attach_alternative(html_content, "text/html")
+
+        # Add attachments (if available)
+        msg = self._add_attachments(msg)
+
+        # Return mail object
+        return msg
+
+    def is_valid(self, raise_exception: bool = True) -> bool:
+        """
+        This function ensures that all required variables for the email object are set. Can be overridden and extended
+        but again, make sure that super() is called.
+        """
+        if not self.get_subject():
+            self._errors.append(_("Email service requires a subject."))
+        if not self.template_name:
+            self._errors.append(_("Email service requires a template."))
+        if not len(self.recipient_email_list):
+            self._errors.append(_("Email service requires a target mail address."))
+
+        if self._errors and raise_exception:
+            raise EmailServiceConfigError(self._errors)
+
+        return not bool(len(self._errors))
+
+    def has_errors(self) -> bool:
+        """
+        Check if any errors are stored inside this class instance
+        """
+        return bool(len(self._errors))
+
+    @property
+    def errors(self) -> list:
+        """
+        Getter for fetching the stored error messages.
+        Errors shall not be set manually, that's why we use a property here.
+        """
+        return self._errors
+
+    def _send_and_log_email(self, msg: EmailMultiAlternatives) -> bool:
+        """
+        Method to be called by the thread. Enables logging since we won't have any sync return values.
+        """
+        result = False
+        recipients_as_string = " ".join(self.recipient_email_list)
+        try:
+            result = msg.send()
+            if PONY_LOG_RECIPIENTS:
+                self._logger.debug(_('Email "%s" successfully sent to %s.') % (msg.subject, recipients_as_string))
+            else:
+                self._logger.debug(_('Email "%s" successfully sent.') % msg.subject)
+        except Exception as e:
+            if PONY_LOG_RECIPIENTS:
+                self._logger.error(
+                    _('An error occurred sending email "%s" to %s: %s') % (msg.subject, recipients_as_string, str(e))
+                )
+            else:
+                self._logger.error(_('An error occurred sending email "%s": %s') % (msg.subject, str(e)))
+
+        return result
+
+    def process(self, raise_exception: bool = True) -> bool:
+        """
+        Public method which is called to actually send an email. Calls validation first and returns the result of
+        "msg.send()"
+        """
+        result = False
+        if self.is_valid(raise_exception=raise_exception):
+            msg = self._build_mail_object()
+            result = self._send_and_log_email(msg=msg)
+
+        return result
```

### Comparing `django_pony_express-2.0.0/django_pony_express/services/tests.py` & `django_pony_express-2.1.0/django_pony_express/services/tests.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,292 +1,294 @@
-import re
-import warnings
-from typing import List
-
-from django.core import mail
-from django.test import TestCase
-
-
-class EmailTestService:
-    _outbox = None
-
-    def _ensure_outbox_is_loaded(self):
-        """
-        Ensures that the outbox attribute is set
-        """
-        if self._outbox is None:
-            self.reload()
-
-    def reload(self):
-        """
-        Loads the current _outbox inside an attribute of this class
-        """
-        self._outbox = mail.outbox
-
-    def empty(self):
-        """
-        Empties the current outbox
-        :return:
-        """
-        mail.outbox = []
-        self.reload()
-
-    def filter(self, to=None, cc=None, bcc=None, subject=None):
-        """
-        Searches in the _outbox for emails matching either to and/or subject.
-        Returns a list of email objects
-        :param to: str
-        :param cc: str
-        :param bcc: str
-        :param subject: str | re.Pattern
-        :return: EmailTestService
-        """
-        # Ensure that outbox is up-to-date
-        self.reload()
-
-        if not any([to, cc, bcc, subject]):
-            raise ValueError("EmailTestService.filter called without parameters")
-
-        if subject and not isinstance(subject, re.Pattern):
-            # If the "subject" is a translatable, we have to cast it to string
-            subject = re.compile(f"^{re.escape(str(subject))}$")
-
-        match_list = []
-        for email in self._outbox:
-            # Check conditions
-            match = True
-            if to and to not in email.to:
-                match = False
-            if cc and cc not in email.cc:
-                match = False
-            if bcc and bcc not in email.bcc:
-                match = False
-            if subject and not re.search(subject, str(email.subject)):
-                match = False
-
-            # Add email if all set conditions are valid
-            if match:
-                match_list.append(email)
-
-        return EmailTestServiceQuerySet(matching_list=match_list)
-
-    def all(self):
-        """
-        Loads all mails from the outbox inside the matching list
-        :return:
-        """
-        # Ensure that outbox is up-to-date
-        self.reload()
-
-        # Load data to matching list
-        match_list = list(self._outbox)
-
-        return EmailTestServiceQuerySet(matching_list=match_list)
-
-
-class EmailTestServiceMail(mail.EmailMultiAlternatives):
-    """
-    Wrapper around a Django EmailMultiAlternatives object with some helper functions to write clean assertions.
-    """
-
-    _testcase = TestCase()  # Hacky way to get access to TestCase.assert* methods without deriving from TestCase
-
-    def _get_html_content(self):
-        """
-        Ensure we just have found one element and then return HTML part of the email
-        :return: str
-        """
-        # Search for string
-        if len(self.alternatives) > 0:
-            return self.alternatives[0][0]
-        return None
-
-    def _get_txt_content(self):
-        """
-        Ensure we just have found one element and then return text part of the email
-        :return: str
-        """
-        # Search for string
-        return self.body
-
-    def assert_subject(self, subject, msg=None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        :param subject: str
-        :param msg: str
-        """
-
-        # Assert expected subject is equal to the generated one
-        self._testcase.assertEqual(subject, self.subject, msg=msg)
-
-    def assert_body_contains(self, search_str, msg=None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        :param search_str: str
-        :param msg: str
-        """
-
-        # Assert string is contained in TXT part
-        self._testcase.assertIn(search_str, self._get_txt_content(), msg=msg)
-        # Assert string is contained in HTML part (if HTML part is set)
-        html_content = self._get_html_content()
-        if html_content is not None:
-            self._testcase.assertIn(search_str, html_content, msg=msg)
-
-    def assert_body_contains_not(self, search_str, msg=None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        :param search_str: str
-        :param msg: str
-        """
-
-        # Assert string is contained in HTML part
-        self._testcase.assertNotIn(search_str, self._get_html_content(), msg=msg)
-        # Assert string is contained in TXT part
-        self._testcase.assertNotIn(search_str, self._get_txt_content(), msg=msg)
-
-    def assert_to_contains(self, *emails: List[str]):
-        for email in emails:
-            self._testcase.assertIn(email, self.to)
-
-
-class EmailTestServiceQuerySet(TestCase):
-    _match_list = None
-
-    def __init__(self, matching_list=None):
-        super().__init__()
-        self._match_list = matching_list
-        for email in self._match_list or []:
-            # Change the class of every EmailMutliAlternative instance, so that it points to
-            # our subclass, which has some additional assertion-methods.
-            email.__class__ = EmailTestServiceMail
-
-    def _get_html_content(self):
-        """
-        Ensure we just have found one element and then return HTML part of the email
-        :return: str
-        """
-        self._validate_lookup_cache_contains_one_element()
-        # Search for string
-        if len(self[0].alternatives) > 0:
-            return self[0].alternatives[0][0]
-        return None
-
-    def _get_txt_content(self):
-        """
-        Ensure we just have found one element and then return text part of the email
-        :return: str
-        """
-        # Search for string
-        self._validate_lookup_cache_contains_one_element()
-        return self[0].body
-
-    def _validate_lookup_cache_contains_one_element(self):
-        """
-        Ensures that in the cached lookup is exactly one element. Needed for full-text-search.
-        """
-        if self.count() > 1:
-            raise RuntimeError("Current lookup has more than one email object and is thus ambiguous.")
-        elif self.count() == 0:
-            raise RuntimeError("Current lookup has zero matches so lookup does not make sense.")
-
-    def _ensure_matching_list_was_populated(self):
-        """
-        Make sure that we queried at least once before working with the results
-        """
-        if self._match_list is None:
-            raise RuntimeError(
-                "Counting of matches called without previous query. " "Please call filter() or all() first."
-            )
-
-    def one(self):
-        """
-        Checks if the previous query returned exactly one element
-        :return: bool
-        """
-        return self.count() == 1
-
-    def count(self):
-        """
-        Returns the number of matches found by a previous call of `find()`
-        :return: int
-        """
-        # Ensure is was queried before using results
-        self._ensure_matching_list_was_populated()
-
-        # Count matches
-        return len(self)
-
-    def first(self):
-        """
-        Returns the first found element
-        :return: EmailMultiAlternatives
-        """
-        # Ensure is was queried before using results
-        self._ensure_matching_list_was_populated()
-        return self[0] if self.count() > 0 else False
-
-    def last(self):
-        """
-        Returns the last found element
-        :return: EmailMultiAlternatives
-        """
-        # Ensure is was queried before using results
-        self._ensure_matching_list_was_populated()
-        return self[-1] if self.count() > 0 else False
-
-    def assert_one(self, msg: str = None):
-        """
-        Makes an assertion to make sure queried element exists exactly once
-        """
-        self.assertEqual(self.one(), True, msg=msg)
-
-    def assert_quantity(self, target_quantity: str, msg: str = None):
-        """
-        Makes an assertion to make sure that amount of queried mails are equal to `target_quantity`
-        :return:
-        """
-        self.assertEqual(self.count(), target_quantity, msg=msg)
-
-    def assert_subject(self, subject: str, msg: str = None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        """
-        warnings.warn(
-            "EmailTestServiceQuerySet.assert_subject is deprecated. Use queryset[0].assert_subject instead.",
-            stacklevel=2,
-        )
-        # Ensure we just have found one element
-        self._validate_lookup_cache_contains_one_element()
-        self[0].assert_subject(subject, msg)
-
-    def assert_body_contains(self, search_str: str, msg: str = None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        """
-        warnings.warn(
-            "EmailTestServiceQuerySet.assert_body_contains is deprecated. "
-            "Use queryset[0].assert_body_contains instead.",
-            stacklevel=2,
-        )
-        # Ensure we just have found one element
-        self._validate_lookup_cache_contains_one_element()
-        self[0].assert_body_contains(search_str, msg)
-
-    def assert_body_contains_not(self, search_str: str, msg: str = None):
-        """
-        Searches in a given email inside the HTML AND TXT part for a given string
-        """
-        warnings.warn(
-            "EmailTestServiceQuerySet.assert_body_contains is deprecated. "
-            "Use queryset[0].assert_body_contains_not instead.",
-            stacklevel=2,
-        )
-        # Ensure we just have found one element
-        self._validate_lookup_cache_contains_one_element()
-        self[0].assert_body_contains_not(search_str, msg)
-
-    def __getitem__(self, item):
-        return self._match_list.__getitem__(item)
-
-    def __len__(self):
-        return self._match_list.__len__()
+import re
+import warnings
+from typing import List
+
+from django.core import mail
+from django.core.mail import EmailMultiAlternatives
+from django.test import TestCase
+
+
+class EmailTestService:
+    _outbox = None
+
+    def _ensure_outbox_is_loaded(self):
+        """
+        Ensures that the outbox attribute is set
+        """
+        if self._outbox is None:
+            self.reload()
+
+    def reload(self):
+        """
+        Loads the current _outbox inside an attribute of this class
+        """
+        self._outbox = mail.outbox
+
+    def empty(self):
+        """
+        Empties the current outbox
+        :return:
+        """
+        mail.outbox = []
+        self.reload()
+
+    def filter(self, to=None, cc=None, bcc=None, subject=None):
+        """
+        Searches in the _outbox for emails matching either to and/or subject.
+        Returns a list of email objects
+        :param to: str
+        :param cc: str
+        :param bcc: str
+        :param subject: str | re.Pattern
+        :return: EmailTestService
+        """
+        # Ensure that outbox is up-to-date
+        self.reload()
+
+        if not any([to, cc, bcc, subject]):
+            raise ValueError("EmailTestService.filter called without parameters")
+
+        if subject and not isinstance(subject, re.Pattern):
+            # If the "subject" is a translatable, we have to cast it to string
+            subject = re.compile(f"^{re.escape(str(subject))}$")
+
+        match_list = []
+        for email in self._outbox:
+            # Check conditions
+            match = True
+            if to and to not in email.to:
+                match = False
+            if cc and cc not in email.cc:
+                match = False
+            if bcc and bcc not in email.bcc:
+                match = False
+            if subject and not re.search(subject, str(email.subject)):
+                match = False
+
+            # Add email if all set conditions are valid
+            if match:
+                match_list.append(email)
+
+        return EmailTestServiceQuerySet(matching_list=match_list)
+
+    def all(self):
+        """
+        Loads all mails from the outbox inside the matching list
+        :return:
+        """
+        # Ensure that outbox is up-to-date
+        self.reload()
+
+        # Load data to matching list
+        match_list = list(self._outbox)
+
+        return EmailTestServiceQuerySet(matching_list=match_list)
+
+
+class EmailTestServiceMail(mail.EmailMultiAlternatives):
+    """
+    Wrapper around a Django EmailMultiAlternatives object with some helper functions to write clean assertions.
+    """
+
+    _testcase = TestCase()  # Hacky way to get access to TestCase.assert* methods without deriving from TestCase
+
+    def _get_html_content(self):
+        """
+        Ensure we just have found one element and then return HTML part of the email
+        :return: str
+        """
+        # Search for string
+        if len(self.alternatives) > 0:
+            return self.alternatives[0][0]
+        return None
+
+    def _get_txt_content(self):
+        """
+        Ensure we just have found one element and then return text part of the email
+        :return: str
+        """
+        # Search for string
+        return self.body
+
+    def assert_subject(self, subject, msg=None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        :param subject: str
+        :param msg: str
+        """
+
+        # Assert expected subject is equal to the generated one
+        self._testcase.assertEqual(subject, self.subject, msg=msg)
+
+    def assert_body_contains(self, search_str, msg=None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        :param search_str: str
+        :param msg: str
+        """
+
+        # Assert string is contained in TXT part
+        self._testcase.assertIn(search_str, self._get_txt_content(), msg=msg)
+        # Assert string is contained in HTML part (if HTML part is set)
+        html_content = self._get_html_content()
+        if html_content is not None:
+            self._testcase.assertIn(search_str, html_content, msg=msg)
+
+    def assert_body_contains_not(self, search_str, msg=None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        :param search_str: str
+        :param msg: str
+        """
+
+        # Assert string is contained in HTML part
+        self._testcase.assertNotIn(search_str, self._get_html_content(), msg=msg)
+        # Assert string is contained in TXT part
+        self._testcase.assertNotIn(search_str, self._get_txt_content(), msg=msg)
+
+    def assert_to_contains(self, *emails: List[str]):
+        for email in emails:
+            self._testcase.assertIn(email, self.to)
+
+
+class EmailTestServiceQuerySet(TestCase):
+    _match_list = None
+
+    def __init__(self, matching_list=None):
+        super().__init__()
+        self._match_list = matching_list
+        for email in self._match_list or []:
+            # Change the class of every EmailMultiAlternative instance, so that it points to
+            # our subclass, which has some additional assertion-methods.
+            if isinstance(email, EmailMultiAlternatives):
+                email.__class__ = EmailTestServiceMail
+
+    def _get_html_content(self):
+        """
+        Ensure we just have found one element and then return HTML part of the email
+        :return: str
+        """
+        self._validate_lookup_cache_contains_one_element()
+        # Search for string
+        if len(self[0].alternatives) > 0:
+            return self[0].alternatives[0][0]
+        return None
+
+    def _get_txt_content(self):
+        """
+        Ensure we just have found one element and then return text part of the email
+        :return: str
+        """
+        # Search for string
+        self._validate_lookup_cache_contains_one_element()
+        return self[0].body
+
+    def _validate_lookup_cache_contains_one_element(self):
+        """
+        Ensures that in the cached lookup is exactly one element. Needed for full-text-search.
+        """
+        if self.count() > 1:
+            raise RuntimeError("Current lookup has more than one email object and is thus ambiguous.")
+        elif self.count() == 0:
+            raise RuntimeError("Current lookup has zero matches so lookup does not make sense.")
+
+    def _ensure_matching_list_was_populated(self):
+        """
+        Make sure that we queried at least once before working with the results
+        """
+        if self._match_list is None:
+            raise RuntimeError(
+                "Counting of matches called without previous query. " "Please call filter() or all() first."
+            )
+
+    def one(self):
+        """
+        Checks if the previous query returned exactly one element
+        :return: bool
+        """
+        return self.count() == 1
+
+    def count(self):
+        """
+        Returns the number of matches found by a previous call of `find()`
+        :return: int
+        """
+        # Ensure is was queried before using results
+        self._ensure_matching_list_was_populated()
+
+        # Count matches
+        return len(self)
+
+    def first(self):
+        """
+        Returns the first found element
+        :return: EmailMultiAlternatives
+        """
+        # Ensure is was queried before using results
+        self._ensure_matching_list_was_populated()
+        return self[0] if self.count() > 0 else False
+
+    def last(self):
+        """
+        Returns the last found element
+        :return: EmailMultiAlternatives
+        """
+        # Ensure is was queried before using results
+        self._ensure_matching_list_was_populated()
+        return self[-1] if self.count() > 0 else False
+
+    def assert_one(self, msg: str = None):
+        """
+        Makes an assertion to make sure queried element exists exactly once
+        """
+        self.assertEqual(self.one(), True, msg=msg)
+
+    def assert_quantity(self, target_quantity: str, msg: str = None):
+        """
+        Makes an assertion to make sure that amount of queried mails are equal to `target_quantity`
+        :return:
+        """
+        self.assertEqual(self.count(), target_quantity, msg=msg)
+
+    def assert_subject(self, subject: str, msg: str = None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        """
+        warnings.warn(
+            "EmailTestServiceQuerySet.assert_subject is deprecated. Use queryset[0].assert_subject instead.",
+            stacklevel=2,
+        )
+        # Ensure we just have found one element
+        self._validate_lookup_cache_contains_one_element()
+        self[0].assert_subject(subject, msg)
+
+    def assert_body_contains(self, search_str: str, msg: str = None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        """
+        warnings.warn(
+            "EmailTestServiceQuerySet.assert_body_contains is deprecated. "
+            "Use queryset[0].assert_body_contains instead.",
+            stacklevel=2,
+        )
+        # Ensure we just have found one element
+        self._validate_lookup_cache_contains_one_element()
+        self[0].assert_body_contains(search_str, msg)
+
+    def assert_body_contains_not(self, search_str: str, msg: str = None):
+        """
+        Searches in a given email inside the HTML AND TXT part for a given string
+        """
+        warnings.warn(
+            "EmailTestServiceQuerySet.assert_body_contains is deprecated. "
+            "Use queryset[0].assert_body_contains_not instead.",
+            stacklevel=2,
+        )
+        # Ensure we just have found one element
+        self._validate_lookup_cache_contains_one_element()
+        self[0].assert_body_contains_not(search_str, msg)
+
+    def __getitem__(self, item):
+        return self._match_list.__getitem__(item)
+
+    def __len__(self):
+        return self._match_list.__len__()
```

### Comparing `django_pony_express-2.0.0/docs/Makefile` & `django_pony_express-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/docs/conf.py` & `django_pony_express-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/docs/features/tests.md` & `django_pony_express-2.1.0/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/docs/make.bat` & `django_pony_express-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/manage.py` & `django_pony_express-2.1.0/manage.py`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/pyproject.toml` & `django_pony_express-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pony_express-2.0.0/settings.py` & `django_pony_express-2.1.0/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,62 +1,67 @@
-from pathlib import Path
-
-BASE_PATH = Path(__file__).resolve(strict=True).parent
-
-INSTALLED_APPS = (
-    "django.contrib.admin",
-    "django.contrib.auth",
-    "django.contrib.contenttypes",
-    "django.contrib.sessions",
-    "django.contrib.messages",
-    "django.contrib.staticfiles",
-    "testapp",
-)
-
-DEBUG = False
-
-ALLOWED_HOSTS = ["localhost:8000"]
-
-SECRET_KEY = "ASDFjklö123456890"
-
-# Routing
-ROOT_URLCONF = "testapp.urls"
-
-DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
-
-DATABASES = {
-    "default": {
-        "ENGINE": "django.db.backends.sqlite3",
-        "NAME": "db.sqlite",
-    }
-}
-
-TEMPLATES = [
-    {
-        "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": ["templates"],
-        "APP_DIRS": True,
-        "OPTIONS": {
-            "context_processors": [
-                "django.template.context_processors.debug",
-                "django.template.context_processors.request",
-                "django.contrib.auth.context_processors.auth",
-                "django.contrib.messages.context_processors.messages",
-            ],
-            "debug": True,
-        },
-    },
-]
-
-MIDDLEWARE = (
-    "django.middleware.security.SecurityMiddleware",
-    "django.contrib.sessions.middleware.SessionMiddleware",
-    "django.middleware.common.CommonMiddleware",
-    "django.middleware.csrf.CsrfViewMiddleware",
-    "django.contrib.auth.middleware.AuthenticationMiddleware",
-    "django.contrib.messages.middleware.MessageMiddleware",
-    "django.middleware.clickjacking.XFrameOptionsMiddleware",
-)
-
-TIME_ZONE = "UTC"
-
-LOCALE_PATHS = [str(BASE_PATH) + "/django_pony_express/locale"]
+from pathlib import Path
+
+BASE_PATH = Path(__file__).resolve(strict=True).parent
+
+INSTALLED_APPS = (
+    "django.contrib.admin",
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "testapp",
+)
+
+DEBUG = False
+
+ALLOWED_HOSTS = ["localhost:8000"]
+
+SECRET_KEY = "ASDFjklö123456890"
+
+# Routing
+ROOT_URLCONF = "testapp.urls"
+
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
+
+DATABASES = {
+    "default": {
+        "ENGINE": "django.db.backends.sqlite3",
+        "NAME": "db.sqlite",
+    }
+}
+
+TEMPLATES = [
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": ["templates"],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "context_processors": [
+                "django.template.context_processors.debug",
+                "django.template.context_processors.request",
+                "django.contrib.auth.context_processors.auth",
+                "django.contrib.messages.context_processors.messages",
+            ],
+            "debug": True,
+        },
+    },
+]
+
+MIDDLEWARE = (
+    "django.middleware.security.SecurityMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+)
+
+USE_TZ = True
+TIME_ZONE = "UTC"
+
+LOCALE_PATHS = [str(BASE_PATH) + "/django_pony_express/locale"]
+
+
+# Pony express
+DJANGO_PONY_EXPRESS_LOG_RECIPIENTS = False
```

### Comparing `django_pony_express-2.0.0/tests/test_email_test_service.py` & `django_pony_express-2.1.0/tests/services/tests/test_email_test_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,248 +1,248 @@
-import re
-
-from django.core import mail
-from django.core.mail import EmailMultiAlternatives
-from django.test import TestCase
-from django.utils.translation import gettext_lazy as _
-
-from django_pony_express.services.tests import EmailTestService, EmailTestServiceMail, EmailTestServiceQuerySet
-
-
-class EmailTestServiceTest(TestCase):
-    @classmethod
-    def setUpClass(cls):
-        super().setUpClass()
-
-        # Mail data
-        cls.subject = "Super great email (definitely not spam!)"
-        cls.to = "spam@world.com"
-        cls.cc = "spam-copy@world.com"
-        cls.bcc = "spam-secret@world.com"
-        cls.content_part = "body part"
-        cls.text_content = "I'm the %s." % cls.content_part
-        cls.html_content = "<html>I'm the %s.</html>" % cls.content_part
-
-        cls.other_mail_subject = "Other mail subject"
-
-        # Initialize django outbox
-        mail.outbox = []
-
-        # Instances
-        cls.ets = EmailTestService()
-
-    def setUp(self):
-        super().setUp()
-
-        # Create email per test case
-        email = EmailMultiAlternatives(self.subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-
-        # Create second email per test case
-        email = EmailMultiAlternatives(
-            self.other_mail_subject, self.text_content, to=["to@world.com"], cc=["cc@world.com"], bcc=["bcc@world.com"]
-        )
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-
-    def tearDown(self) -> None:
-        super().tearDown()
-        # Emtpy mailbox for next test
-        mail.outbox = []
-
-    def test_outbox_is_updated(self):
-        self.assertEqual(self.ets.all().count(), 2)
-        # Create third mail
-        email = EmailMultiAlternatives(
-            self.other_mail_subject, self.text_content, to=["to@world.com"], cc=["cc@world.com"], bcc=["bcc@world.com"]
-        )
-        email.attach_alternative(self.html_content, "text/html")
-        mail.outbox.append(email)
-        self.assertEqual(self.ets.all().count(), 3)
-
-    def test_ensure_outbox_is_loaded(self):
-        ets = EmailTestService()
-        self.assertEqual(ets._outbox, None)
-        ets._ensure_outbox_is_loaded()
-        self.assertIsInstance(ets._outbox, list)
-
-    def test_reload(self):
-        ets = EmailTestService()
-        self.assertEqual(ets._outbox, None)
-        ets.reload()
-        self.assertIsInstance(ets._outbox, list)
-
-    def test_filter_no_params(self):
-        self.assertRaises(ValueError, self.ets.filter)
-
-    def test_filter_to_valid(self):
-        qs = self.ets.filter(to=self.to)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_cc_valid(self):
-        qs = self.ets.filter(cc=self.cc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_bcc_valid(self):
-        qs = self.ets.filter(bcc=self.bcc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_valid(self):
-        qs = self.ets.filter(subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_invalid(self):
-        qs = self.ets.filter(to="not-my@mail.com")
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_cc_invalid(self):
-        qs = self.ets.filter(cc="not-my@mail.com")
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_bcc_invalid(self):
-        qs = self.ets.filter(bcc="not-my@mail.com")
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_invalid(self):
-        qs = self.ets.filter(subject="Not my subject")
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_to_cc_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_subject_valid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_to_cc_bcc_subject_invalid(self):
-        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject="Not my subject")
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_regular(self):
-        qs = self.ets.filter(subject=self.subject)
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_invalid(self):
-        qs = self.ets.filter(subject=re.compile("Not my subject"))
-        self.assertEqual(qs.count(), 0)
-
-    def test_filter_subject_translatable(self):
-        qs = self.ets.filter(subject=_(self.subject))
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_valid_single(self):
-        qs = self.ets.filter(subject=re.compile("definitely not"))
-        self.assertEqual(qs.count(), 1)
-
-    def test_filter_subject_regex_valid_multiple(self):
-        qs = self.ets.filter(subject=re.compile("other|spam", flags=re.IGNORECASE))
-        self.assertEqual(qs.count(), 2)
-
-    def test_all(self):
-        # Assertion
-        self.assertEqual(self.ets.all().count(), 2)
-
-    def test_validate_lookup_cache_contains_one_element_true(self):
-        # Assertion (we have two mails so it's not equal to 1)
-        self.assertEqual(self.ets.all().count(), 2)
-        self.assertRaises(RuntimeError, self.ets.all()._validate_lookup_cache_contains_one_element)
-
-    def test_validate_lookup_cache_contains_one_element_false(self):
-        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
-        self.assertEqual(self.ets.filter(subject=self.subject)._validate_lookup_cache_contains_one_element(), None)
-
-    def test_ensure_matching_list_was_populated_false(self):
-        self.assertRaises(RuntimeError, EmailTestServiceQuerySet()._ensure_matching_list_was_populated)
-
-    def test_ensure_matching_list_was_populated_true(self):
-        self.assertEqual(self.ets.all()._ensure_matching_list_was_populated(), None)
-
-    def test_get_html_content(self):
-        self.assertEqual(self.ets.filter(subject=self.subject)._get_html_content(), self.html_content)
-
-    def test_get_txt_content(self):
-        self.assertEqual(self.ets.filter(subject=self.subject)._get_txt_content(), self.text_content)
-
-    def test_one_true(self):
-        self.assertEqual(self.ets.filter(subject=self.subject).one(), True)
-
-    def test_one_false(self):
-        self.assertEqual(self.ets.all().one(), False)
-
-    def test_count(self):
-        self.assertEqual(self.ets.all().count(), 2)
-        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
-        self.assertEqual(self.ets.filter(subject="Not my subject").count(), 0)
-
-    def test_first(self):
-        self.assertEqual(self.ets.all().first().subject, self.subject)
-
-    def test_last(self):
-        self.assertEqual(self.ets.all().last().subject, self.other_mail_subject)
-
-    def test_assert_one_true(self):
-        self.ets.filter(subject=self.subject).assert_one()
-
-    def test_assert_one_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.all().assert_one()
-
-    def test_assert_quantity_true(self):
-        self.ets.filter(subject=self.subject).assert_quantity(1)
-
-    def test_assert_quantity_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_quantity(0)
-
-    def test_assert_subject_true(self):
-        self.ets.filter(subject=self.subject).assert_subject(self.subject)
-
-    def test_assert_subject_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_subject(self.other_mail_subject)
-
-    def test_assert_body_contains_true(self):
-        self.ets.filter(subject=self.subject).assert_body_contains(self.content_part)
-
-    def test_assert_body_contains_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_body_contains("Not in here!")
-
-    def test_assert_body_contains_not_true(self):
-        self.ets.filter(subject=self.subject).assert_body_contains_not("Not in here!")
-
-    def test_assert_body_contains_not_false(self):
-        with self.assertRaises(AssertionError):
-            self.ets.filter(subject=self.subject).assert_body_contains_not(self.content_part)
-
-    def test_assert_body_contains_no_html_part(self):
-        subject = "No html email"
-        email = EmailMultiAlternatives(subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
-        mail.outbox.append(email)
-
-        self.ets.filter(subject=subject).assert_body_contains(self.content_part)
-
-    def test_can_get_mail_via_item(self):
-        mail_qs = self.ets.all()
-        self.assertIsInstance(mail_qs[0], EmailTestServiceMail)
-
-    def test_can_get_first_email_via_brackets_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(mail_qs[0], mail_qs.first())
-
-    def test_can_get_last_email_via_brackets_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(mail_qs[-1], mail_qs.last())
-
-    def test_can_use_len_operator(self):
-        mail_qs = self.ets.all()
-        self.assertEqual(len(mail_qs), 2)
-
-    def test_assert_to_contains(self):
-        email = self.ets.all()[0]
-        email.assert_to_contains(self.to)
+import re
+
+from django.core import mail
+from django.core.mail import EmailMultiAlternatives
+from django.test import TestCase
+from django.utils.translation import gettext_lazy as _
+
+from django_pony_express.services.tests import EmailTestService, EmailTestServiceMail, EmailTestServiceQuerySet
+
+
+class EmailTestServiceTest(TestCase):
+    @classmethod
+    def setUpClass(cls):
+        super().setUpClass()
+
+        # Mail data
+        cls.subject = "Super great email (definitely not spam!)"
+        cls.to = "spam@world.com"
+        cls.cc = "spam-copy@world.com"
+        cls.bcc = "spam-secret@world.com"
+        cls.content_part = "body part"
+        cls.text_content = "I'm the %s." % cls.content_part
+        cls.html_content = "<html>I'm the %s.</html>" % cls.content_part
+
+        cls.other_mail_subject = "Other mail subject"
+
+        # Initialize django outbox
+        mail.outbox = []
+
+        # Instances
+        cls.ets = EmailTestService()
+
+    def setUp(self):
+        super().setUp()
+
+        # Create email per test case
+        email = EmailMultiAlternatives(self.subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+
+        # Create second email per test case
+        email = EmailMultiAlternatives(
+            self.other_mail_subject, self.text_content, to=["to@world.com"], cc=["cc@world.com"], bcc=["bcc@world.com"]
+        )
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+
+    def tearDown(self) -> None:
+        super().tearDown()
+        # Emtpy mailbox for next test
+        mail.outbox = []
+
+    def test_outbox_is_updated(self):
+        self.assertEqual(self.ets.all().count(), 2)
+        # Create third mail
+        email = EmailMultiAlternatives(
+            self.other_mail_subject, self.text_content, to=["to@world.com"], cc=["cc@world.com"], bcc=["bcc@world.com"]
+        )
+        email.attach_alternative(self.html_content, "text/html")
+        mail.outbox.append(email)
+        self.assertEqual(self.ets.all().count(), 3)
+
+    def test_ensure_outbox_is_loaded(self):
+        ets = EmailTestService()
+        self.assertEqual(ets._outbox, None)
+        ets._ensure_outbox_is_loaded()
+        self.assertIsInstance(ets._outbox, list)
+
+    def test_reload(self):
+        ets = EmailTestService()
+        self.assertEqual(ets._outbox, None)
+        ets.reload()
+        self.assertIsInstance(ets._outbox, list)
+
+    def test_filter_no_params(self):
+        self.assertRaises(ValueError, self.ets.filter)
+
+    def test_filter_to_valid(self):
+        qs = self.ets.filter(to=self.to)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_cc_valid(self):
+        qs = self.ets.filter(cc=self.cc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_bcc_valid(self):
+        qs = self.ets.filter(bcc=self.bcc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_valid(self):
+        qs = self.ets.filter(subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_invalid(self):
+        qs = self.ets.filter(to="not-my@mail.com")
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_cc_invalid(self):
+        qs = self.ets.filter(cc="not-my@mail.com")
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_bcc_invalid(self):
+        qs = self.ets.filter(bcc="not-my@mail.com")
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_invalid(self):
+        qs = self.ets.filter(subject="Not my subject")
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_to_cc_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_subject_valid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_to_cc_bcc_subject_invalid(self):
+        qs = self.ets.filter(to=self.to, cc=self.cc, bcc=self.bcc, subject="Not my subject")
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_regular(self):
+        qs = self.ets.filter(subject=self.subject)
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_invalid(self):
+        qs = self.ets.filter(subject=re.compile("Not my subject"))
+        self.assertEqual(qs.count(), 0)
+
+    def test_filter_subject_translatable(self):
+        qs = self.ets.filter(subject=_(self.subject))
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_valid_single(self):
+        qs = self.ets.filter(subject=re.compile("definitely not"))
+        self.assertEqual(qs.count(), 1)
+
+    def test_filter_subject_regex_valid_multiple(self):
+        qs = self.ets.filter(subject=re.compile("other|spam", flags=re.IGNORECASE))
+        self.assertEqual(qs.count(), 2)
+
+    def test_all(self):
+        # Assertion
+        self.assertEqual(self.ets.all().count(), 2)
+
+    def test_validate_lookup_cache_contains_one_element_true(self):
+        # Assertion (we have two mails so it's not equal to 1)
+        self.assertEqual(self.ets.all().count(), 2)
+        self.assertRaises(RuntimeError, self.ets.all()._validate_lookup_cache_contains_one_element)
+
+    def test_validate_lookup_cache_contains_one_element_false(self):
+        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
+        self.assertEqual(self.ets.filter(subject=self.subject)._validate_lookup_cache_contains_one_element(), None)
+
+    def test_ensure_matching_list_was_populated_false(self):
+        self.assertRaises(RuntimeError, EmailTestServiceQuerySet()._ensure_matching_list_was_populated)
+
+    def test_ensure_matching_list_was_populated_true(self):
+        self.assertEqual(self.ets.all()._ensure_matching_list_was_populated(), None)
+
+    def test_get_html_content(self):
+        self.assertEqual(self.ets.filter(subject=self.subject)._get_html_content(), self.html_content)
+
+    def test_get_txt_content(self):
+        self.assertEqual(self.ets.filter(subject=self.subject)._get_txt_content(), self.text_content)
+
+    def test_one_true(self):
+        self.assertEqual(self.ets.filter(subject=self.subject).one(), True)
+
+    def test_one_false(self):
+        self.assertEqual(self.ets.all().one(), False)
+
+    def test_count(self):
+        self.assertEqual(self.ets.all().count(), 2)
+        self.assertEqual(self.ets.filter(subject=self.subject).count(), 1)
+        self.assertEqual(self.ets.filter(subject="Not my subject").count(), 0)
+
+    def test_first(self):
+        self.assertEqual(self.ets.all().first().subject, self.subject)
+
+    def test_last(self):
+        self.assertEqual(self.ets.all().last().subject, self.other_mail_subject)
+
+    def test_assert_one_true(self):
+        self.ets.filter(subject=self.subject).assert_one()
+
+    def test_assert_one_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.all().assert_one()
+
+    def test_assert_quantity_true(self):
+        self.ets.filter(subject=self.subject).assert_quantity(1)
+
+    def test_assert_quantity_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject).assert_quantity(0)
+
+    def test_assert_subject_true(self):
+        self.ets.filter(subject=self.subject)[0].assert_subject(self.subject)
+
+    def test_assert_subject_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject)[0].assert_subject(self.other_mail_subject)
+
+    def test_assert_body_contains_true(self):
+        self.ets.filter(subject=self.subject)[0].assert_body_contains(self.content_part)
+
+    def test_assert_body_contains_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject)[0].assert_body_contains("Not in here!")
+
+    def test_assert_body_contains_not_true(self):
+        self.ets.filter(subject=self.subject)[0].assert_body_contains_not("Not in here!")
+
+    def test_assert_body_contains_not_false(self):
+        with self.assertRaises(AssertionError):
+            self.ets.filter(subject=self.subject)[0].assert_body_contains_not(self.content_part)
+
+    def test_assert_body_contains_no_html_part(self):
+        subject = "No html email"
+        email = EmailMultiAlternatives(subject, self.text_content, to=[self.to], cc=[self.cc], bcc=[self.bcc])
+        mail.outbox.append(email)
+
+        self.ets.filter(subject=subject)[0].assert_body_contains(self.content_part)
+
+    def test_can_get_mail_via_item(self):
+        mail_qs = self.ets.all()
+        self.assertIsInstance(mail_qs[0], EmailTestServiceMail)
+
+    def test_can_get_first_email_via_brackets_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(mail_qs[0], mail_qs.first())
+
+    def test_can_get_last_email_via_brackets_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(mail_qs[-1], mail_qs.last())
+
+    def test_can_use_len_operator(self):
+        mail_qs = self.ets.all()
+        self.assertEqual(len(mail_qs), 2)
+
+    def test_assert_to_contains(self):
+        email = self.ets.all()[0]
+        email.assert_to_contains(self.to)
```

### Comparing `django_pony_express-2.0.0/tests/test_mail_services.py` & `django_pony_express-2.1.0/tests/services/base/test_base_mail_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,390 +1,374 @@
-from os.path import basename
-
-from django.conf import settings
-from django.core.mail import EmailMultiAlternatives
-from django.test import TestCase, override_settings
-from freezegun import freeze_time
-
-from django_pony_express.errors import EmailServiceAttachmentError, EmailServiceConfigError
-from django_pony_express.services.base import BaseEmailService, BaseEmailServiceFactory
-
-
-class BaseEmailServiceFactoryTest(TestCase):
-    class TestMailService(BaseEmailService):
-        subject = "My subject"
-        template_name = "testapp/test_email.html"
-
-    @classmethod
-    def setUpTestData(cls):
-        super().setUpTestData()
-
-    def test_init_recipient_list_is_set(self):
-        email = "albertus.magnus@example.com"
-        factory = BaseEmailServiceFactory([email])
-        self.assertEqual(factory.recipient_email_list, [email])
-
-    def test_is_valid_positive_case(self):
-        email = "albertus.magnus@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email])
-        factory.service_class = BaseEmailService
-        self.assertTrue(factory.is_valid())
-
-    def test_is_valid_no_recipients(self):
-        factory = BaseEmailServiceFactory()
-        factory.service_class = BaseEmailService
-        with self.assertRaises(EmailServiceConfigError):
-            factory.is_valid()
-
-    def test_is_valid_no_service_class(self):
-        email = "albertus.magnus@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email])
-        with self.assertRaises(EmailServiceConfigError):
-            factory.is_valid()
-
-    def test_is_valid_no_exception_raised(self):
-        factory = BaseEmailServiceFactory()
-        factory.is_valid(raise_exception=False)
-        self.assertEqual(len(factory.errors), 2)
-
-    def test_has_errors_positive_case(self):
-        factory = BaseEmailServiceFactory()
-        factory.is_valid(raise_exception=False)
-        self.assertTrue(factory.has_errors())
-
-    def test_has_errors_negative_case(self):
-        email = "albertus.magnus@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email])
-        factory.service_class = BaseEmailService
-        self.assertFalse(factory.has_errors())
-
-    def test_get_recipient_list_regular(self):
-        email_1 = "albertus.magnus@example.com"
-        email_2 = "thomas.von.aquin@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email_1, email_2])
-        self.assertEqual(factory.get_recipient_list(), [email_1, email_2])
-
-    def test_get_email_from_recipient_regular(self):
-        email_1 = "albertus.magnus@example.com"
-        email_2 = "thomas.von.aquin@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email_1, email_2])
-        self.assertEqual(factory.get_email_from_recipient(factory.get_recipient_list()[1]), email_2)
-
-    def test_get_context_data_regular(self):
-        factory = BaseEmailServiceFactory()
-        self.assertEqual(factory.get_context_data(), {})
-
-    def test_process_regular(self):
-        email_1 = "albertus.magnus@example.com"
-        email_2 = "thomas.von.aquin@example.com"
-        factory = BaseEmailServiceFactory(recipient_email_list=[email_1, email_2])
-        factory.service_class = self.TestMailService
-        self.assertEqual(factory.process(), 2)
-
-    def test_process_with_excepetion(self):
-        factory = BaseEmailServiceFactory()
-        factory.service_class = self.TestMailService
-        with self.assertRaises(EmailServiceConfigError):
-            factory.process()
-
-
-class BaseEmailServiceTest(TestCase):
-    @classmethod
-    def setUpTestData(cls):
-        super().setUpTestData()
-
-    def test_init_recipient_as_str_is_wrapped_to_list(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService(email)
-        self.assertEqual(service.recipient_email_list, [email])
-
-    def test_init_recipient_and_context_are_initialised_empty(self):
-        service = BaseEmailService()
-        self.assertEqual(service.recipient_email_list, [])
-        self.assertEqual(service.context_data, {})
-
-    def test_get_context_data_regular(self):
-        data = {"city": "Cologne"}
-        service = BaseEmailService(context_data=data)
-        self.assertEqual(service.get_context_data(), data)
-
-    def test_get_subject_no_prefix(self):
-        subject = "I am a subject!"
-        service = BaseEmailService()
-        service.subject = subject
-        self.assertEqual(service.get_subject(), subject)
-
-    def test_get_subject_with_prefix(self):
-        prefix = "Ai: Core"
-        subject = "I am a subject!"
-        service = BaseEmailService()
-        service.SUBJECT_PREFIX = prefix
-        service.subject = subject
-        self.assertIn(prefix, service.get_subject())
-        self.assertIn(subject, service.get_subject())
-
-    @override_settings(DEFAULT_FROM_EMAIL="noreply@example.com")
-    def test_get_from_email_from_settings(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_from_email(), "noreply@example.com")
-
-    @override_settings(DEFAULT_FROM_EMAIL="noreply@example.com")
-    def test_get_from_email_from_class(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService()
-        service.FROM_EMAIL = email
-        self.assertEqual(service.get_from_email(), email)
-
-    def test_get_reply_to_email_not_set(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_reply_to_emails(), [])
-
-    def test_get_reply_to_email_is_set(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService()
-        service.REPLY_TO_ADDRESS = email
-        self.assertEqual(service.get_reply_to_emails(), [email])
-
-    def test_get_cc_email_not_set(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_cc_emails(), [])
-
-    def test_get_cc_email_is_set(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService()
-        service.cc_email_list = [email]
-        self.assertEqual(service.get_cc_emails(), [email])
-
-    def test_get_bcc_email_not_set(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_bcc_emails(), [])
-
-    def test_get_bcc_email_is_set(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService()
-        service.bcc_email_list = [email]
-        self.assertEqual(service.get_bcc_emails(), [email])
-
-    @override_settings(LANGUAGE_CODE="de-AT")
-    def test_get_translation_regular_german(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), "de")
-
-    @override_settings(LANGUAGE_CODE="en-GB")
-    def test_get_translation_regular_english(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), "en")
-
-    @override_settings(LANGUAGE_CODE="de")
-    def test_get_translation_settings_short(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), "de")
-
-    @override_settings(LANGUAGE_CODE=None)
-    def test_get_translation_settings_not_set(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), None)
-
-    @override_settings(LANGUAGE_CODE=1)
-    def test_get_translation_settings_invalid_type(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), None)
-
-    @override_settings(LANGUAGE_CODE="a")
-    def test_get_translation_settings_invalid_value(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_translation(), None)
-
-    def test_get_attachments_regular(self):
-        file_path = "usr/albertus/myfile.csv"
-        service = BaseEmailService(attachment_list=[file_path])
-        self.assertEqual(service.get_attachments(), [file_path])
-
-    def test_get_attachments_empty(self):
-        service = BaseEmailService()
-        self.assertEqual(service.get_attachments(), [])
-
-    def test_add_attachments_path_as_str(self):
-        # Setup
-        service = BaseEmailService()
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
-        service.attachment_list = [file_path]
-        msg_obj = service._add_attachments(msg_obj)
-
-        self.assertEqual(len(msg_obj.attachments), 1)
-        self.assertEqual(msg_obj.attachments[0][0], basename(file_path))
-
-    def test_add_attachments_path_as_dict(self):
-        # Setup
-        service = BaseEmailService()
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        filename = "awesome_file.txt"
-        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
-        service.attachment_list = [{"filename": filename, "file": file_path, "mimetype": "text/text"}]
-        msg_obj = service._add_attachments(msg_obj)
-
-        self.assertEqual(len(msg_obj.attachments), 1)
-        self.assertEqual(msg_obj.attachments[0][0], filename)
-
-    def test_add_attachments_path_wrong_dict_data(self):
-        # Setup
-        service = BaseEmailService()
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        filename = "awesome_file.txt"
-        service.attachment_list = [{"filename": filename}]
-
-        with self.assertRaises(EmailServiceAttachmentError):
-            service._add_attachments(msg_obj)
-
-    @freeze_time("2020-06-26")
-    def test_build_mail_object_regular(self):
-        from_email = "noreply@example.com"
-        reply_to_email = "willreply@example.com"
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        my_var = "Lorem ipsum dolor!"
-        service = BaseEmailService(recipient_email_list=[email], context_data={"my_var": my_var})
-        service.FROM_EMAIL = from_email
-        service.REPLY_TO_ADDRESS = reply_to_email
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        # Assertions
-        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
-
-        self.assertEqual(msg_obj.subject, subject)
-
-        self.assertEqual(msg_obj.from_email, from_email)
-        self.assertEqual(msg_obj.to, [email])
-        self.assertEqual(msg_obj.reply_to, [reply_to_email])
-
-        self.assertIn("Friday", msg_obj.body)
-        self.assertIn(my_var, msg_obj.body)
-
-        self.assertIn("Friday", msg_obj.alternatives[0][0])
-        self.assertIn(my_var, msg_obj.alternatives[0][0])
-
-    def test_build_mail_object_with_attachments(self):
-        from_email = "noreply@example.com"
-        reply_to_email = "willreply@example.com"
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        my_var = "Lorem ipsum dolor!"
-        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
-        service = BaseEmailService(
-            recipient_email_list=[email], context_data={"my_var": my_var}, attachment_list=[file_path]
-        )
-        service.FROM_EMAIL = from_email
-        service.REPLY_TO_ADDRESS = reply_to_email
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        # Assertions
-        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
-
-        self.assertEqual(len(msg_obj.attachments), 1)
-        self.assertEqual(msg_obj.attachments[0][0], basename(file_path))
-
-    def test_setting_txt_templates_works(self):
-        my_var = "Lorem ipsum dolor!"
-        service = BaseEmailService(
-            recipient_email_list=["albertus.magnus@example.com"], context_data={"my_var": my_var}
-        )
-        service.FROM_EMAIL = "noreply@example.com"
-        service.subject = "Test mail"
-        service.template_name = "testapp/test_email.html"
-        service.template_txt_name = "testapp/test_email.txt"
-        msg_obj = service._build_mail_object()
-
-        # Assertions
-        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
-
-        self.assertIn("I am a different content", msg_obj.body)
-        self.assertNotIn("I am a different content", msg_obj.alternatives[0][0])
-
-        self.assertIn(my_var, msg_obj.body)
-
-    @freeze_time("2020-06-26")
-    @override_settings(LANGUAGE_CODE="nl-BE")
-    def test_build_mail_object_translation_works(self):
-        service = BaseEmailService(recipient_email_list="noreply@example.com")
-        service.template_name = "testapp/test_email.html"
-        msg_obj = service._build_mail_object()
-
-        # Assertions
-        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
-
-        self.assertIn("vrijdag", msg_obj.body)
-        self.assertIn("vrijdag", msg_obj.alternatives[0][0])
-
-    def test_is_valid_positive_case(self):
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        service = BaseEmailService(recipient_email_list=[email])
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        self.assertTrue(service.is_valid())
-
-    def test_is_valid_no_subject(self):
-        email = "albertus.magnus@example.com"
-        service = BaseEmailService(recipient_email_list=[email])
-        service.template_name = "testapp/test_email.html"
-        with self.assertRaises(EmailServiceConfigError):
-            service.is_valid()
-
-    def test_is_valid_no_template(self):
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        service = BaseEmailService(recipient_email_list=[email])
-        service.subject = subject
-        with self.assertRaises(EmailServiceConfigError):
-            service.is_valid()
-
-    def test_is_valid_no_recipient(self):
-        subject = "Test email"
-        service = BaseEmailService()
-        service.subject = subject
-        with self.assertRaises(EmailServiceConfigError):
-            service.is_valid()
-
-    def test_is_valid_no_exception_raised(self):
-        service = BaseEmailService()
-        service.is_valid(raise_exception=False)
-        self.assertEqual(len(service.errors), 3)
-
-    def test_has_errors_positive_case(self):
-        service = BaseEmailService()
-        service.is_valid(raise_exception=False)
-        self.assertTrue(service.has_errors())
-
-    def test_has_errors_negative_case(self):
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        service = BaseEmailService(recipient_email_list=[email])
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        self.assertFalse(service.has_errors())
-
-    def test_process_regular(self):
-        email = "albertus.magnus@example.com"
-        subject = "Test email"
-        service = BaseEmailService(recipient_email_list=[email])
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        self.assertTrue(service.process())
-
-    def test_process_with_error(self):
-        subject = "Test email"
-        service = BaseEmailService()
-        service.subject = subject
-        service.template_name = "testapp/test_email.html"
-        with self.assertRaises(EmailServiceConfigError):
-            service.process()
+import logging
+from os.path import basename
+from unittest import mock
+
+from django.conf import settings
+from django.core.mail import EmailMultiAlternatives
+from django.test import TestCase, override_settings
+from freezegun import freeze_time
+
+from django_pony_express.errors import EmailServiceAttachmentError, EmailServiceConfigError
+from django_pony_express.services.base import BaseEmailService
+
+
+class BaseEmailServiceTest(TestCase):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+
+    def test_init_recipient_as_str_is_wrapped_to_list(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService(email)
+        self.assertEqual(service.recipient_email_list, [email])
+
+    def test_init_recipient_and_context_are_initialised_empty(self):
+        service = BaseEmailService()
+        self.assertEqual(service.recipient_email_list, [])
+        self.assertEqual(service.context_data, {})
+
+    def test_get_logger_logger_not_set(self):
+        service = BaseEmailService()
+        email_logger = service._get_logger()
+        self.assertEqual(service._logger, email_logger)
+
+    def test_get_logger_logger_set(self):
+        service = BaseEmailService()
+        service._logger = logging.getLogger("my_logger")
+        email_logger = service._get_logger()
+        self.assertEqual(service._logger, email_logger)
+
+    def test_get_context_data_regular(self):
+        data = {"city": "Cologne"}
+        service = BaseEmailService(context_data=data)
+        self.assertEqual(service.get_context_data(), data)
+
+    def test_get_subject_no_prefix(self):
+        subject = "I am a subject!"
+        service = BaseEmailService()
+        service.subject = subject
+        self.assertEqual(service.get_subject(), subject)
+
+    def test_get_subject_with_prefix(self):
+        prefix = "Pony Express"
+        subject = "I am a subject!"
+        service = BaseEmailService()
+        service.SUBJECT_PREFIX = prefix
+        service.subject = subject
+        self.assertIn(prefix, service.get_subject())
+        self.assertIn(subject, service.get_subject())
+
+    @override_settings(DEFAULT_FROM_EMAIL="noreply@example.com")
+    def test_get_from_email_from_settings(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_from_email(), "noreply@example.com")
+
+    @override_settings(DEFAULT_FROM_EMAIL="noreply@example.com")
+    def test_get_from_email_from_class(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService()
+        service.FROM_EMAIL = email
+        self.assertEqual(service.get_from_email(), email)
+
+    def test_get_reply_to_email_not_set(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_reply_to_emails(), [])
+
+    def test_get_reply_to_email_is_set(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService()
+        service.REPLY_TO_ADDRESS = email
+        self.assertEqual(service.get_reply_to_emails(), [email])
+
+    def test_get_cc_email_not_set(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_cc_emails(), [])
+
+    def test_get_cc_email_is_set(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService()
+        service.cc_email_list = [email]
+        self.assertEqual(service.get_cc_emails(), [email])
+
+    def test_get_bcc_email_not_set(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_bcc_emails(), [])
+
+    def test_get_bcc_email_is_set(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService()
+        service.bcc_email_list = [email]
+        self.assertEqual(service.get_bcc_emails(), [email])
+
+    @override_settings(LANGUAGE_CODE="de-AT")
+    def test_get_translation_regular_german(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), "de")
+
+    @override_settings(LANGUAGE_CODE="en-GB")
+    def test_get_translation_regular_english(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), "en")
+
+    @override_settings(LANGUAGE_CODE="de")
+    def test_get_translation_settings_short(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), "de")
+
+    @override_settings(LANGUAGE_CODE=None)
+    def test_get_translation_settings_not_set(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), None)
+
+    @override_settings(LANGUAGE_CODE=1)
+    def test_get_translation_settings_invalid_type(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), None)
+
+    @override_settings(LANGUAGE_CODE="a")
+    def test_get_translation_settings_invalid_value(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_translation(), None)
+
+    def test_get_attachments_regular(self):
+        file_path = "usr/albertus/myfile.csv"
+        service = BaseEmailService(attachment_list=[file_path])
+        self.assertEqual(service.get_attachments(), [file_path])
+
+    def test_get_attachments_empty(self):
+        service = BaseEmailService()
+        self.assertEqual(service.get_attachments(), [])
+
+    def test_add_attachments_path_as_str(self):
+        # Setup
+        service = BaseEmailService()
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
+        service.attachment_list = [file_path]
+        msg_obj = service._add_attachments(msg_obj)
+
+        self.assertEqual(len(msg_obj.attachments), 1)
+        self.assertEqual(msg_obj.attachments[0][0], basename(file_path))
+
+    def test_add_attachments_path_as_dict(self):
+        # Setup
+        service = BaseEmailService()
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        filename = "awesome_file.txt"
+        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
+        service.attachment_list = [{"filename": filename, "file": file_path, "mimetype": "text/text"}]
+        msg_obj = service._add_attachments(msg_obj)
+
+        self.assertEqual(len(msg_obj.attachments), 1)
+        self.assertEqual(msg_obj.attachments[0][0], filename)
+
+    def test_add_attachments_path_wrong_dict_data(self):
+        # Setup
+        service = BaseEmailService()
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        filename = "awesome_file.txt"
+        service.attachment_list = [{"filename": filename}]
+
+        with self.assertRaises(EmailServiceAttachmentError):
+            service._add_attachments(msg_obj)
+
+    @freeze_time("2020-06-26")
+    def test_build_mail_object_regular(self):
+        from_email = "noreply@example.com"
+        reply_to_email = "willreply@example.com"
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        my_var = "Lorem ipsum dolor!"
+        service = BaseEmailService(recipient_email_list=[email], context_data={"my_var": my_var})
+        service.FROM_EMAIL = from_email
+        service.REPLY_TO_ADDRESS = reply_to_email
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        # Assertions
+        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
+
+        self.assertEqual(msg_obj.subject, subject)
+
+        self.assertEqual(msg_obj.from_email, from_email)
+        self.assertEqual(msg_obj.to, [email])
+        self.assertEqual(msg_obj.reply_to, [reply_to_email])
+
+        self.assertIn("Friday", msg_obj.body)
+        self.assertIn(my_var, msg_obj.body)
+
+        self.assertIn("Friday", msg_obj.alternatives[0][0])
+        self.assertIn(my_var, msg_obj.alternatives[0][0])
+
+    def test_build_mail_object_with_attachments(self):
+        from_email = "noreply@example.com"
+        reply_to_email = "willreply@example.com"
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        my_var = "Lorem ipsum dolor!"
+        file_path = settings.BASE_PATH / "tests/files/testfile.txt"
+        service = BaseEmailService(
+            recipient_email_list=[email], context_data={"my_var": my_var}, attachment_list=[file_path]
+        )
+        service.FROM_EMAIL = from_email
+        service.REPLY_TO_ADDRESS = reply_to_email
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        # Assertions
+        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
+
+        self.assertEqual(len(msg_obj.attachments), 1)
+        self.assertEqual(msg_obj.attachments[0][0], basename(file_path))
+
+    def test_setting_txt_templates_works(self):
+        my_var = "Lorem ipsum dolor!"
+        service = BaseEmailService(
+            recipient_email_list=["albertus.magnus@example.com"], context_data={"my_var": my_var}
+        )
+        service.FROM_EMAIL = "noreply@example.com"
+        service.subject = "Test mail"
+        service.template_name = "testapp/test_email.html"
+        service.template_txt_name = "testapp/test_email.txt"
+        msg_obj = service._build_mail_object()
+
+        # Assertions
+        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
+
+        self.assertIn("I am a different content", msg_obj.body)
+        self.assertNotIn("I am a different content", msg_obj.alternatives[0][0])
+
+        self.assertIn(my_var, msg_obj.body)
+
+    @freeze_time("2020-06-26")
+    @override_settings(LANGUAGE_CODE="nl-BE")
+    def test_build_mail_object_translation_works(self):
+        service = BaseEmailService(recipient_email_list="noreply@example.com")
+        service.template_name = "testapp/test_email.html"
+        msg_obj = service._build_mail_object()
+
+        # Assertions
+        self.assertIsInstance(msg_obj, EmailMultiAlternatives)
+
+        self.assertIn("vrijdag", msg_obj.body)
+        self.assertIn("vrijdag", msg_obj.alternatives[0][0])
+
+    def test_is_valid_positive_case(self):
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        service = BaseEmailService(recipient_email_list=[email])
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        self.assertTrue(service.is_valid())
+
+    def test_is_valid_no_subject(self):
+        email = "albertus.magnus@example.com"
+        service = BaseEmailService(recipient_email_list=[email])
+        service.template_name = "testapp/test_email.html"
+        with self.assertRaises(EmailServiceConfigError):
+            service.is_valid()
+
+    def test_is_valid_no_template(self):
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        service = BaseEmailService(recipient_email_list=[email])
+        service.subject = subject
+        with self.assertRaises(EmailServiceConfigError):
+            service.is_valid()
+
+    def test_is_valid_no_recipient(self):
+        subject = "Test email"
+        service = BaseEmailService()
+        service.subject = subject
+        with self.assertRaises(EmailServiceConfigError):
+            service.is_valid()
+
+    def test_is_valid_no_exception_raised(self):
+        service = BaseEmailService()
+        service.is_valid(raise_exception=False)
+        self.assertEqual(len(service.errors), 3)
+
+    def test_has_errors_positive_case(self):
+        service = BaseEmailService()
+        service.is_valid(raise_exception=False)
+        self.assertTrue(service.has_errors())
+
+    def test_has_errors_negative_case(self):
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        service = BaseEmailService(recipient_email_list=[email])
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        self.assertFalse(service.has_errors())
+
+    @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
+    def test_send_and_log_email_success_privacy_active(self, mock_logger):
+        service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
+        result = service._send_and_log_email(
+            msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
+        )
+
+        mock_logger.debug.assert_called_with('Email "The Pony Express" successfully sent.')
+        self.assertEqual(result, 1)
+
+    @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
+    @mock.patch("django_pony_express.services.base.PONY_LOG_RECIPIENTS", True)
+    def test_send_and_log_success_privacy_inactive(self, mock_logger):
+        service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
+        result = service._send_and_log_email(
+            msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
+        )
+
+        mock_logger.debug.assert_called_with('Email "The Pony Express" successfully sent to thomas.aquin@example.com.')
+        self.assertEqual(result, 1)
+
+    @mock.patch.object(EmailMultiAlternatives, "send", side_effect=Exception("Broken pony"))
+    @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
+    def test_send_and_log_email_failure_privacy_active(self, mock_logger, *args):
+        service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
+        result = service._send_and_log_email(
+            msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
+        )
+
+        mock_logger.error('An error occurred sending email "%s": %s', "The Pony Express", "Broken pony")
+        self.assertFalse(result)
+
+    @mock.patch.object(EmailMultiAlternatives, "send", side_effect=Exception("Broken pony"))
+    @mock.patch("django_pony_express.services.base.BaseEmailService._logger")
+    @mock.patch("django_pony_express.services.base.PONY_LOG_RECIPIENTS", True)
+    def test_send_and_log_failure_privacy_inactive(self, mock_logger, *args):
+        service = BaseEmailService(recipient_email_list=["thomas.aquin@example.com"])
+        result = service._send_and_log_email(
+            msg=EmailMultiAlternatives(subject="The Pony Express", to=["thomas.aquin@example.com"])
+        )
+
+        mock_logger.error(
+            'An error occurred sending email "%s" to %s: %s',
+            "The Pony Express",
+            "thomas.aquin@example.com",
+            "Broken pony",
+        )
+        self.assertFalse(result)
+
+    def test_process_regular(self):
+        email = "albertus.magnus@example.com"
+        subject = "Test email"
+        service = BaseEmailService(recipient_email_list=[email])
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        self.assertTrue(service.process())
+
+    def test_process_with_error(self):
+        subject = "Test email"
+        service = BaseEmailService()
+        service.subject = subject
+        service.template_name = "testapp/test_email.html"
+        with self.assertRaises(EmailServiceConfigError):
+            service.process()
```

### Comparing `django_pony_express-2.0.0/PKG-INFO` & `django_pony_express-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 2.0.0
+Version: 2.1.0
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
```

